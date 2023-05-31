# Comparing `tmp/pginter-0.1.0.tar.gz` & `tmp/pginter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.1.0.tar", last modified: Wed Feb 22 19:28:31 2023, max compression
+gzip compressed data, was "pginter-0.2.0.tar", last modified: Wed May 31 11:58:06 2023, max compression
```

## Comparing `pginter-0.1.0.tar` & `pginter-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.760057 pginter-0.1.0/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.1.0/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       53 2023-02-10 14:14:25.000000 pginter-0.1.0/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-02-22 19:28:31.760057 pginter-0.1.0/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.1.0/README.md
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)      115 2023-02-04 12:18:07.000000 pginter-0.1.0/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-02-22 19:28:31.760057 pginter-0.1.0/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-02-22 19:27:41.000000 pginter-0.1.0/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.750057 pginter-0.1.0/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.753391 pginter-0.1.0/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    16305 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.753391 pginter-0.1.0/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3782 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.753391 pginter-0.1.0/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      275 2023-02-10 18:24:14.000000 pginter-0.1.0/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.756724 pginter-0.1.0/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      134 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3428 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      454 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      123 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/types/_geo_types.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.756724 pginter-0.1.0/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      424 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.760057 pginter-0.1.0/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      143 2023-02-10 18:08:23.000000 pginter-0.1.0/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    13781 2023-02-10 18:20:18.000000 pginter-0.1.0/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    16242 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     2090 2023-02-10 18:28:34.000000 pginter-0.1.0/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.1.0/src/pginter/widgets/_supports_children.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-02-22 19:28:31.753391 pginter-0.1.0/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-02-22 19:28:31.000000 pginter-0.1.0/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      744 2023-02-22 19:28:31.000000 pginter-0.1.0/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-02-22 19:28:31.000000 pginter-0.1.0/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-02-22 19:28:31.000000 pginter-0.1.0/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.106671 pginter-0.2.0/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.0/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       53 2023-02-10 14:14:25.000000 pginter-0.2.0/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 11:58:06.106671 pginter-0.2.0/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.0/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.0/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 11:58:06.106671 pginter-0.2.0/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      936 2023-05-24 18:38:46.000000 pginter-0.2.0/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.093338 pginter-0.2.0/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.096671 pginter-0.2.0/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20454 2023-05-25 15:22:29.000000 pginter-0.2.0/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.100005 pginter-0.2.0/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.103338 pginter-0.2.0/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.0/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.0/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.0/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.0/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.0/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.0/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.0/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.0/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.103338 pginter-0.2.0/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.0/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.106671 pginter-0.2.0/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.0/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.0/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.0/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    22121 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    23874 2023-05-25 23:31:06.000000 pginter-0.2.0/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.0/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.0/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.0/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 11:58:06.100005 pginter-0.2.0/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      956 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 11:58:06.000000 pginter-0.2.0/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.1.0/LICENSE` & `pginter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.1.0/setup.py` & `pginter-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.1.0",
+    version="0.2.0",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
     #     "Official Website": "http://info.fridrich.xyz",
     # },
     classifiers=[
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     include_package_data=True
     # data_files=[
     #     ('pginter/theme/themes/', ['src/pginter/theme/themes/default.json'])
     # ]
 )
```

### Comparing `pginter-0.1.0/src/pginter/_pg_root.py` & `pginter-0.2.0/src/pginter/_pg_root.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,44 +3,70 @@
 04. February 2023
 
 the root of the window
 
 Author:
 Nilusink
 """
+from concurrent.futures import ThreadPoolExecutor as Pool, Future
 from .widgets import GeometryManager
 from .theme import ThemeManager
+from time import perf_counter
 from copy import deepcopy
 from .types import *
 import typing as tp
 import pygame as pg
 import os.path
 
 
 DEFAULT_TITLE: str = "Window"
 DEFAULT_ICON: str = os.path.dirname(__file__) + "/icon.png"
 
 
+RES_T = tp.TypeVar("RES_T")
+
+
+class _TimeoutCandidate(tp.TypedDict):
+    timeout_left: float
+    function: tp.Callable[[tp.Any], RES_T]
+    future: Future[RES_T]
+    args: tuple[tp.Any, ...]
+    kwargs: dict[str, tp.Any]
+
+
 class PgRoot(GeometryManager):
+    _focus_item: GeometryManager | None = None
     _running: bool = True
     _theme: ThemeManager = ...
     __background: pg.Surface = ...
     layout_params: BetterDict = ...
     _min_size: tuple[int, int] = ...
     _bg_configured: bool = False
+    _mouse_pos: tuple[int, int] = ...
+    _max_framerate: int = ...
+
+    __timeouts: list[_TimeoutCandidate]
+    _last_it_call: float
+    _tpool: Pool
 
     def __init__(
             self,
             title: str = ...,
             icon_path: str = ...,
             size: tuple[int, int] = ...,
             bg_color: Color = ...,
             padding: int = 0,
             margin: int = 0,
+            max_framerate: int = 30
     ):
+        self._last_it_call = perf_counter()
+        self._max_framerate = max_framerate
+        self._tpool = Pool(max_workers=10)
+        self.__timeouts = []
+
         super().__init__()
         self._theme = ThemeManager()
         self._theme.notify_on(ThemeManager.NotifyEvent.theme_reload, self.notify)
         self._min_size = (0, 0)
 
         # args
         self._bg_configured = bg_color is not ...
@@ -50,24 +76,27 @@
             "padding": padding,
             "margin": margin,
         })
 
         # pg init
         pg.init()
         pg.font.init()
+        self._clk = pg.time.Clock()
 
         if size is not ...:
             self.__background = pg.display.set_mode(size, flags=pg.RESIZABLE)
 
         else:
             self.__background = pg.display.set_mode(flags=pg.RESIZABLE)
 
         # set icon and caption
         pg.display.set_caption(DEFAULT_TITLE if title is ... else title)
-        img = pg.image.load(DEFAULT_ICON if icon_path is ... else icon_path, "icon")
+        img = pg.image.load(
+            DEFAULT_ICON if icon_path is ... else icon_path, "icon"
+        )
         pg.display.set_icon(img)
 
     # config
     @property
     def title(self) -> str:
         return pg.display.get_caption()[0]
 
@@ -75,16 +104,51 @@
     def title(self, value: str) -> None:
         pg.display.set_caption(value)
 
     @property
     def theme(self) -> ThemeManager:
         return self._theme
 
+    @property
+    def mouse_pos(self) -> tuple[int, int]:
+        return self._mouse_pos
+
+    @property
+    def root(self) -> tp.Self:
+        return self
+
+    def get_focus(self) -> GeometryManager | None:
+        """
+        get the currently focused item
+        """
+        return self._focus_item
+
+    def set_focus(
+            self,
+            widget: tp.Union["GeometryManager", None, tp.Any] = None
+    ) -> None:
+        """
+        set the focused item
+        """
+        if self._focus_item is not None:
+            self._focus_item.stop_focus()
+
+        if widget is not None:
+            widget.set_focus()
+            self._focus_item = widget
+
+    def notify_focus(self, widget: tp.Union["GeometryManager", None] = None):
+        """
+        notify the root that a widget has been set as focus
+        """
+        if self._focus_item != widget:
+            self.set_focus(widget)
+
     # interfacing
-    def notify(self, event: ThemeManager.NotifyEvent) -> None:
+    def notify(self, event: ThemeManager.NotifyEvent, _info=...) -> None:
         """
         gets called by another class
         """
         match event:
             case ThemeManager.NotifyEvent.theme_reload:
                 # the theme has been reloaded
                 if not self._bg_configured:
@@ -96,63 +160,107 @@
         handle the events raised by pygame
         """
         for event in pg.event.get():
             match event.type:
                 case pg.QUIT:
                     self._running = False
 
+                case pg.KEYDOWN:
+                    if self._focus_item is not None:
+                        self._focus_item.notify(
+                            KeyboardNotifyEvent.key_down,
+                            event
+                        )
+
+                case pg.KEYUP:
+                    if self._focus_item is not None:
+                        self._focus_item.notify(
+                            KeyboardNotifyEvent.key_up,
+                            event
+                        )
+
                 # case pg.VIDEORESIZE:  # window size changed
                 #     width, height = event.size
                 #
                 #     print("updating size: ", (width, height), "\t", self._min_size)
                 #
                 #     width = max([width, self._min_size[0]])
                 #     height = max([height, self._min_size[1]])
                 #
                 #     # self.__background = pg.display.set_mode((width, height), flags=pg.RESIZABLE | pg.HWSURFACE | pg.DOUBLEBUF)
 
-    def update_screen(self) -> None:
+        self._mouse_pos = pg.mouse.get_pos()
+
+        self._notify_child_active_hover(self.mouse_pos)
+
+    def update_idletasks(self) -> None:
+        """
+        updates all the functional tasks
+        """
+        self._event_handler()
+
+        # handle timeouts
+        for to in self.__timeouts.copy():
+            # calculate time since last function call
+            now = perf_counter()
+            delta = now - self._last_it_call
+            self._last_it_call = now
+
+            # remove time from timeout
+            to["timeout_left"] -= delta * 1000
+
+            # if the timeout is finished, execute the function
+            if to["timeout_left"] <= 0:
+                # create a function that populates the timeout future's result
+                # with the function return value
+                def curr_func():
+                    to["future"].set_result(to["function"](
+                        *to["args"], **to["kwargs"]
+                    ))
+
+                # submit the created function to the threadpool
+                # and remove it from the active timeouts
+                self._tpool.submit(curr_func)
+                self.__timeouts.remove(to)
+
+    def update(self) -> None:
         """
         update the screen
         """
         self.__background.fill(self._bg)
 
         self.calculate_geometry()
         for child, params in self._child_params:
             child.draw(self.__background)
 
         pg.display.flip()
 
-    def update(self) -> None:
-        """
-        update events
-        """
-        self._event_handler()
-
     def mainloop(self):
         """
         run the windows main loop
         """
         while self._running:
+            self.update_idletasks()
             self.update()
-            self.update_screen()
+
+            self._clk.tick(self._max_framerate)
 
     def calculate_geometry(self):
         """
         calculate how each individual child should be placed
         """
         match self._layout:
-            case 0:  # Absolute
+            case Layout.Absolute:  # Absolute
                 # since the positioning is absolute, the children should not influence the parents size
                 for child, params in self._child_params:
                     child.set_position(params.x, params.y)
 
                 return
 
-            case 1:
+            case Layout.Pack:
                 directional_dict: dict[str, int | list] = {"total_x": 0, "total_y": 0, "children": [], "sizes": []}
                 top = deepcopy(directional_dict)
                 bottom = deepcopy(directional_dict)
                 left = deepcopy(directional_dict)
                 right = deepcopy(directional_dict)
 
                 # get all sizes and group by anchor
@@ -224,15 +332,15 @@
 
                     # bottom
                 y_now = total_y - self._layout_params.margin
                 for child, size in zip(bottom["children"], bottom["sizes"]):
                     child.set_position(x_cen - size[0] / 2, y_now - size[1])
                     y_now -= size[1] + self._layout_params.padding
 
-            case 2:
+            case Layout.Grid:
                 rows: list[dict[str, tp.Any | float]] = []
                 columns: list[dict[str, tp.Any | float]] = []
 
                 for child, params in self._child_params:
                     row, column = params["row"], params["column"]
 
                     # if row was not yet made, make all previous ones
@@ -424,7 +532,36 @@
 
     def calculate_size(self) -> tuple[int, int]:
         """
         calculate how big the container should be
         """
         # make sure the geometry is up-to-date
         return pg.display.get_window_size()
+
+    # tool functions
+    def after(
+            self,
+            timeout: int,
+            function: tp.Callable[[tp.Any], RES_T],
+            *args,
+            **kwargs
+    ) -> Future[RES_T]:
+        """
+        calls the given function after timeout milliseconds
+
+        :param timeout: timeout in milliseconds
+        :param function: the function to call
+        :param args: the given functions positional arguments
+        :param kwargs: the given functions keyword arguments
+        :returns: a future with the function's result
+        """
+        n_future = Future[RES_T]()
+
+        self.__timeouts.append({
+            "timeout_left": timeout,
+            "function": function,
+            "future": n_future,
+            "args": args,
+            "kwargs": kwargs
+        })
+
+        return n_future
```

### Comparing `pginter-0.1.0/src/pginter/icon.png` & `pginter-0.2.0/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.1.0/src/pginter/theme/_manager.py` & `pginter-0.2.0/src/pginter/theme/_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 
 class Appearance(Enum):
     dark = 0
     light = 1
 
 
-class NotifyEvent(Enum):
+class _NotifyEvent(Enum):
     theme_reload = 0
 
 
 class ThemeManager:
     """
     the build-in theme manager
     """
     Appearance = Appearance
-    NotifyEvent = NotifyEvent
+    NotifyEvent = _NotifyEvent
     _appearance: Appearance = Appearance.dark
     _notify_on: dict[NotifyEvent, list[tp.Callable]] = ...
     _config: dict[str, str | dict] = ...
     _theme_path: str = ...
     instance = ...
 
     def __new__(cls, *args, **kwargs):
@@ -47,15 +47,15 @@
 
         return cls.instance
 
     def __init__(self, theme_path: str = ...) -> None:
         # load the theme
         self._theme_path = theme_path
         self._notify_on = {
-            NotifyEvent.theme_reload: []
+            _NotifyEvent.theme_reload: []
         }
 
         self.reload_theme()
 
     def notify_on(self, event: NotifyEvent, who: tp.Callable) -> None:
         """
         notify the given class on events
@@ -65,28 +65,37 @@
         """
         self._notify_on[event].append(who)
 
     def reload_theme(self) -> None:
         """
         reload the config theme
         """
-        self._config = json.load(open(DEFAULT_THEME if self.theme_path is ... else self.theme_path, "r"))
+        self._config = json.load(
+            open(
+                DEFAULT_THEME if self.theme_path is ... else self.theme_path,
+                "r"
+            )
+        )
 
         # convert each color to a color class instance
         def convert_color(color):
             if isinstance(color, str):
                 # differentiate between hex and rgb values
                 if color.startswith("#"):
                     return Color.from_hex(color, 255)
 
                 elif color.startswith("rgb"):
-                    return Color.from_rgb(*[int(val) for val in color.lstrip("rgb").split(",")])
+                    return Color.from_rgb(
+                        *[int(val) for val in color.lstrip("rgb").split(",")]
+                    )
 
                 else:
-                    raise ValueError(f"Invalid color value in theme file: \"{color}\"")
+                    raise ValueError(
+                        f"Invalid color value in theme file: \"{color}\""
+                    )
 
             # rgb values written as tuple
             elif isinstance(color, list):
                 if isinstance(color[0], float) or isinstance(color[0], int):
                     return Color.from_rgb(*color)
 
                 elif isinstance(color[0], list) or isinstance(color[0], str):
@@ -95,28 +104,31 @@
             return color
 
         for key in self._config.copy():
             for ckey, color in self._config[key].items():
                 self._config[key][ckey] = convert_color(color)
 
         # notify
-        for element in self._notify_on[NotifyEvent.theme_reload]:
-            element(NotifyEvent.theme_reload)
+        for element in self._notify_on[_NotifyEvent.theme_reload]:
+            element(_NotifyEvent.theme_reload)
 
     def set_appearance(self, appearance: Appearance) -> None:
         """
         set the appearance theme
 
         :param appearance: must be contained in cls.appearance
         """
         if appearance in Appearance:
             self._appearance = appearance
 
         else:
-            raise ValueError(f"Expected \"Appearance\", got \"{appearance.__class__.__name__}\"")
+            raise ValueError(
+                f"Expected \"Appearance\", got "
+                f"\"{appearance.__class__.__name__}\""
+            )
 
         self.reload_theme()
 
     @property
     def theme_path(self) -> str:
         return self._theme_path
```

### Comparing `pginter-0.1.0/src/pginter/types/_color.py` & `pginter-0.2.0/src/pginter/types/_color.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     _hex: str = ...
 
     def __init__(self) -> None:
         self.rgb = 0, 0, 0, 0
 
     # constructors
     @classmethod
-    def from_rgb(cls, red: float, green: float, blue: float, alpha: float = ...) -> "Color":
+    def from_rgb(
+            cls,
+            red: float,
+            green: float,
+            blue: float,
+            alpha: float = ...
+    ) -> "Color":
         new = cls()
         new.rgb = [red, green, blue] + ([255] if alpha is ... else [alpha])
 
         return new
 
     @classmethod
     def from_hex(cls, hex_value: str, alpha: float = ...) -> "Color":
@@ -53,35 +59,71 @@
         """
         black
         """
         return cls.from_hex("#000")
 
     # properties
     @property
+    def r(self) -> float:
+        return self._rgb[0]
+
+    @property
+    def g(self) -> float:
+        return self._rgb[1]
+
+    @property
+    def b(self) -> float:
+        return self._rgb[2]
+
+    @property
     def rgb(self) -> tuple[float, float, float]:
         return self._rgb
 
     @property
+    def irgb(self) -> tuple[int, int, int]:
+        return (
+            int(self.r),
+            int(self.g),
+            int(self.b)
+        )
+
+    @property
     def rgba(self) -> tuple[float, float, float, float]:
         return tuple(self._rgb) + (self._alpha,)
 
     @rgb.setter
-    def rgb(self, value: tuple[float, float, float] | tuple[float, float, float, float]) -> None:
+    def rgb(
+            self,
+            value: tuple[float, float, float]
+            | tuple[float, float, float, float]
+    ) -> None:
         if len(value) == 4:
             *self._rgb, self._alpha = value
 
         elif len(value) == 3:
             self._rgb = value
 
         else:
-            raise ValueError(f"The rgb tuple must have a length of either 3 or 4!  (not {len(value)})")
+            raise ValueError(
+                f"The rgb tuple must have a length"
+                f"of either 3 or 4!  (not {len(value)})"
+            )
 
         self._recalculate_colors("r")
 
     @property
+    def irgba(self) -> tuple[int, int, int, int]:
+        return (
+            int(self.r),
+            int(self.g),
+            int(self.b),
+            int(self._alpha)
+        )
+
+    @property
     def hex(self) -> str:
         return self._hex
 
     @hex.setter
     def hex(self, value: str) -> None:
         if len(value) == 3:  # ex: fff
             self._hex = "#" + 2*value[0] + 2*value[1] + 2*value[2]
@@ -92,28 +134,34 @@
         elif len(value) == 6:  # ex: ffffff
             self._hex = "#" + value
 
         elif len(value) == 7:  # ex: #ffffff
             self._hex = value
 
         else:
-            raise ValueError(f"The hex string must be either 3, 4 or 6 or 7 characters long! (not {len(value)})")
+            raise ValueError(
+                f"The hex string must be either 3, 4"
+                f"or 6 or 7 characters long! (not {len(value)})"
+            )
 
         self._recalculate_colors("h")
 
     @property
     def alpha(self) -> float:
         return self.alpha
 
     @alpha.setter
     def alpha(self, value: float) -> None:
         self._alpha = value
 
     # internal stuff
-    def _recalculate_colors(self, calc_from: tp.Literal["r", "rgb", "h", "hex"]):
+    def _recalculate_colors(
+            self,
+            calc_from: tp.Literal["r", "rgb", "h", "hex"]
+    ):
         if calc_from in ("rgb", "r"):
             self._hex = f"#" \
                         f"{hex(self.rgb[0].__floor__())[2:]}" \
                         f"{hex(self.rgb[1].__floor__())[2:]}" \
                         f"{hex(self.rgb[2].__floor__())[2:]}".upper()
 
         elif calc_from in ("hex", "h"):
```

### Comparing `pginter-0.1.0/src/pginter/widgets/_frame.py` & `pginter-0.2.0/src/pginter/widgets/_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,393 +1,419 @@
 """
-_frame.py
-04. February 2023
+_entry.py
+22. February 2023
 
-Frame - the base widget
+<description>
 
 Author:
 Nilusink
 """
-from ._geo_manager import GeometryManager
-from ..utils import arg_or_default
+from ..types import (
+    GeoNotes, KeyboardNotifyEvent, FrameBind, StringVar, Scheme, Style, Color,
+)
 from ..theme import ThemeManager
-from ..types import *
+from contextlib import suppress
+from ._label import Label
+from ._frame import Frame
 import typing as tp
 import pygame as pg
+import time
 
 
-class DisplayConfig(tp.TypedDict):
-    bg: Color
-    ulr: int  # border radii
-    urr: int
-    llr: int
-    lrr: int
-    border_width: int
-    border_color: Color
-
-
-class DisplayConfigConfigured(tp.TypedDict):
-    bg: bool
-    ulr: bool
-    urr: bool
-    llr: bool
-    lrr: bool
-    border_width: bool
-    border_color: bool
-
-
-def display_configurify(key: str) -> str:
-    """
-    convert a Frame init key to it's corresponding DisplayConfig key
-    """
-    replaces = [
-        ("bg_color", "bg"),
-        ("border_bottom_left_radius", "blr"),
-        ("border_bottom_right_radius", "brr"),
-        ("border_top_left_radius", "ulr"),
-        ("border_top_right_radius", "urr"),
-    ]
-
-    for init, config in replaces:
-        if key == init:
-            return config
-
-    return key
-
-
-class Frame(GeometryManager):
-    """
-    The base widget
-    """
-    __parent: tp.Union["Frame", tp.Any] = ...
-    _display_config: BetterDict = ...
-    _display_config_configured: BetterDict = ...
-    _x: int = -1
-    _y: int = -1
+class Entry(Frame):
+    _label: Label = ...
+    _string_var: StringVar = ...
+    _placeholder_text: str = ...
+    _placeholder_color: Color = ...
+    _cursor_pos: int = 0
+    _max_length: int | None = None
+    _allowed: str = ...
+    _scheme: Scheme
+    _f_lower: bool = False
+    _f_upper: bool = False
 
     def __init__(
             self,
             parent: tp.Union["Frame", tp.Any],
             width: int = ...,
             height: int = ...,
-            bg: Color = ...,
-            layout: int = 0,
-            border_radius: int = ...,
-            border_bottom_radius: int = ...,
-            border_top_radius: int = ...,
-            border_bottom_left_radius: int = ...,
-            border_bottom_right_radius: int = ...,
-            border_top_left_radius: int = ...,
-            border_top_right_radius: int = ...,
             border_width: int = ...,
             border_color: Color = ...,
-            margin: int = ...,
-            padding: int = ...,
-            min_width: int = ...,
-            min_height: int = ...
+            textvariable: StringVar = ...,
+            placeholder_text: str = ...,
+            placeholder_color: Color = ...,
+            bg: Color = ...,
+            fg: Color = ...,
+            valid_symbols: str = ...,
+            scheme: Scheme = ...,
+            force_uppercase: bool = False,
+            force_lowercase: bool = False,
+            max_length: int | None = None,
+            **kwargs
     ) -> None:
         """
-        the most basic widget: a frame
+        A widget where you can enter text
 
-        :param parent: the frames parent container
-        :param width: width of the frame
-        :param height: height of the frame
-        :param bg: background color of the frame
-        :param border_radius: border radius of the box (all four corners)
-        :param border_width: how thick the border of the box should be
-        :param border_color: the color of the border
+        :param valid_symbols: if given, the entry only allows the given
+        characters. If scheme is given, this option will be ignored
         """
+        self._f_lower = force_lowercase
+        self._f_upper = force_uppercase
+        self._max_length = max_length
+        self._allowed = valid_symbols
+        self._scheme = scheme
 
-        if min_width is not ...:
-            self._width = min_width
-
-        if min_height is not ...:
-            self._height = min_height
-
-        self.__parent = parent
+        if placeholder_text is ...:
+            placeholder_text = "Entry"
 
-        self.__parent.theme.notify_on(ThemeManager.NotifyEvent.theme_reload, self.notify)
+        if placeholder_color is ...:
+            placeholder_color = Color.from_hex("#666")
 
-        # mutable defaults
-        display_config: DisplayConfig = {
-            "bg": ...,
-            "ulr": self.theme.frame.border_top_left_radius if "border_top_left_radius" in self.theme.frame else 0,
-            "urr": self.theme.frame.border_top_right_radius if "border_top_right_radius" in self.theme.frame else 0,
-            "llr": self.theme.frame.border_bottom_left_radius if "border_bottom_left_radius" in self.theme.frame else 0,
-            "lrr": self.theme.frame.border_bottom_right_radius if "border_bottom_right_radius" in self.theme.frame else 0,
-            "border_width": self.theme.frame.border_width if "border_width" in self.theme.frame else 0,
-            "border_color": self.theme.frame.border if "border" in self.theme.frame else Color.from_rgb(255, 0, 0),
-        }
+        self._placeholder_text = placeholder_text
+        self._placeholder_color = placeholder_color
 
-        display_config_configured: DisplayConfigConfigured = {
-            "bg": bg is not ...,
-            "ulr": border_radius is not ... or border_top_radius is not ... or border_top_left_radius is not ...,
-            "urr": border_radius is not ... or border_top_radius is not ... or border_top_right_radius is not ...,
-            "llr": border_radius is not ... or border_bottom_radius is not ... or border_bottom_left_radius is not ...,
-            "lrr": border_radius is not ... or border_bottom_radius is not ... or border_bottom_right_radius is not ...,
-            "border_width": border_width is not ...,
-            "border_color": border_color is not ...,
-        }
+        # initialize text-variable
+        self._string_var = textvariable
+        if textvariable is ...:
+            self._string_var = StringVar(value="")
 
-        self._display_config = BetterDict(display_config)
-        self._display_config_configured = BetterDict(display_config_configured)
+        # set theme colors
+        if bg is ... and "bg" in parent.theme.entry:
+            bg = parent.theme.entry.bg
 
-        if margin is ...:
-            margin = self.theme.frame.margin if "margin" in self.theme.frame else 0
+        if fg is ... and "fg" in parent.theme.entry:
+            fg = parent.theme.entry.fg
 
-        if padding is ...:
-            padding = self.theme.frame.padding if "padding" in self.theme.frame else 0
+        if border_width is ... and "border_width" in parent.theme.entry:
+            border_width = parent.theme.entry.border_width
 
-        super().__init__(layout, margin, padding)
+        if border_color is ... and "border_color" in parent.theme.entry:
+            border_color = parent.theme.entry.border_color
 
-        # arguments
-        if width is not ...:
-            self.width = width
+        hover_border_color = ...
+        active_border_color = ...
+        if "hover_border_color" in parent.theme.entry:
+            hover_border_color = parent.theme.entry.hover_border_color
 
-        if height is not ...:
-            self.height = height
+        if "active_border_color" in parent.theme.entry:
+            active_border_color = parent.theme.entry.active_border_color
 
-        self._display_config["bg"] = self.theme.frame.bg1 if bg is ... else bg
-        if isinstance(self.__parent, Frame) and self.__parent._display_config["bg"] == self.theme.frame.bg1:
-            self._display_config["bg"] = self.theme.frame.bg2 if bg is ... else bg
+        if "style" in kwargs:
+            if kwargs["style"].backgroundColor is ...:
+                kwargs["style"].backgroundColor = bg
 
-        print(f"set background: ", self._display_config.bg, bg)
+            if kwargs["style"].color is ...:
+                kwargs["style"].color = fg
 
-        if border_width is not ...:
-            self._display_config["border_width"] = border_width
+            if kwargs["style"].border_width is ...:
+                kwargs["style"].border_width = border_width
 
-        self._display_config["border_color"] = self.theme.frame.border if border_color is ... else border_color
+            if kwargs["style"].borderColor is ...:
+                kwargs["style"].borderColor = border_color
 
-        # border radii
-        if border_radius is ... and "border_radius" in self.theme.frame:
-            border_radius = self.theme.frame.border_radius
+        # create hover and active style if they don't exist in kwargs
+        if "hover_style" not in kwargs:
+            kwargs["hover_style"] = Style()
 
-        if border_bottom_radius is ... and "border_bottom_radius" in self.theme.frame:
-            border_bottom_radius = self.theme.frame.border_bottom_radius
+        if "active_style" not in kwargs:
+            kwargs["active_style"] = Style()
 
-        if border_top_radius is ... and "border_top_radius" in self.theme.frame:
-            border_top_radius = self.theme.frame.border_top_radius
+        # apply default arguments
+        if kwargs["hover_style"].borderColor is ...:
+            kwargs["hover_style"].borderColor = hover_border_color
 
-        self._display_config["ulr"] = self._display_config["urr"] = border_radius
-        self._display_config["llr"] = self._display_config["lrr"] = border_radius
+        if kwargs["active_style"].borderColor is ...:
+            kwargs["active_style"].borderColor = active_border_color
 
-        if border_top_radius is not ...:
-            self._display_config["ulr"] = border_top_radius
-            self._display_config["urr"] = border_top_radius
-
-        if border_bottom_radius is not ...:
-            self._display_config["llr"] = border_bottom_radius
-            self._display_config["lrr"] = border_bottom_radius
+        super().__init__(
+            parent=parent,
+            width=width,
+            height=height,
+            border_width=border_width,
+            border_color=border_color,
+            bg=bg,
+            min_width=100,
+            min_height=10,
+            **kwargs
+        )
+        self.style.color = fg
 
-        self._display_config.ulr = arg_or_default(border_top_left_radius, self._display_config.ulr, ...)
-        self._display_config.urr = arg_or_default(border_top_right_radius, self._display_config.urr, ...)
+        self.grid_columnconfigure(0, weight=1)
+        self.grid_rowconfigure(0, weight=1)
 
-        self._display_config.llr = arg_or_default(border_bottom_left_radius, self._display_config.llr, ...)
-        self._display_config.lrl = arg_or_default(border_bottom_right_radius, self._display_config.lrr, ...)
+        self._label = Label(
+            parent=self,
+            text=""
+        )
+        self._label.grid(0, 0, sticky="nsew")
 
-    @property
-    def theme(self) -> ThemeManager:
-        return self.__parent.theme
+        self._sync_label_style("color", "normal")
+        self._sync_label_style("color", "hover")
+        self._sync_label_style("color", "active")
 
-    @property
-    def parent(self) -> tp.Union["Frame", tp.Any]:
-        return self.__parent
+        self.style.notify_on(
+            "color", lambda *_: self._sync_label_style("color")
+        )
+        self.hover_style.notify_on(
+            "color", lambda *_: self._sync_label_style("color", "hover")
+        )
+        self.active_style.notify_on(
+            "color", lambda *_: self._sync_label_style("color", "active")
+        )
 
-    def configure(self, **kwargs) -> None:
+    def _sync_label_style(
+            self, key: str,
+            style_type: tp.Literal["normal", "hover", "active"] = "normal"
+    ) -> None:
         """
-        configure any of the init parameters (except parent)
+        sync a label style with the button style
         """
-        for key, value in kwargs.items():
-            match key:
-                case "width":
-                    self.width = value
-
-                case "height":
-                    self.height = value
-
-                case "min_width":
-                    self._width = value
-
-                case "min_height":
-                    self._height = value
-
-                case "border_radius":
-                    self._display_config.ulr = value
-                    self._display_config.urr = value
-                    self._display_config.blr = value
-                    self._display_config.brr = value
-
-                case "border_bottom_radius":
-                    self._display_config.blr = value
-                    self._display_config.brr = value
-
-                case "border_top_radius":
-                    self._display_config.ulr = value
-                    self._display_config.urr = value
-
-                case _:
-                    # check if in display config
-                    new_key = display_configurify(key)
-
-                    if new_key in self._display_config:
-                        if isinstance(value, type(self._display_config[new_key])):
-                            raise TypeError(
-                                f"Can't change \"{self._display_config[new_key]}\" to \"{value}\": "
-                                f"invalid type!"
-                            )
+        if style_type == "normal":
+            self._label.style[key] = self.style[key]
 
-                        self._display_config[key] = value
+        elif style_type == "hover":
+            self._label.hover_style[key] = self.hover_style[key]
 
-                    elif key in self.layout_params:
-                        if isinstance(value, type(self.layout_params[new_key])):
-                            raise TypeError(
-                                f"Can't change \"{self.layout_params[new_key]}\" to \"{value}\": "
-                                f"invalid type!"
-                            )
+        elif style_type == "active":
+            self._label.active_style[key] = self.active_style[key]
 
-                        self.layout_params[key] = value
+        else:
+            raise ValueError("Invalid label sync type: ", style_type)
 
-    # interfacing
-    def notify(self, event: ThemeManager.NotifyEvent) -> None:
+    # focus stuff
+    def _on_hover(self) -> None:
         """
-        gets called by another class
+        change mouse
         """
-        match event:
-            case ThemeManager.NotifyEvent.theme_reload:
-                # the theme has been reloaded
-                if not self._display_config_configured.bg:
-                    if isinstance(self.__parent, Frame) and self.__parent._display_config["bg"] == self.theme.frame.bg1:
-                        self._display_config.bg = self.theme.frame.bg2
-
-                    else:
-                        self._display_config.bg = self.theme.frame.bg1
+        pg.mouse.set_cursor(pg.SYSTEM_CURSOR_IBEAM)
+        super()._on_hover()
 
-                if not self._display_config_configured.border_color:
-                    self._display_config.border_color = self.theme.frame.border
+    def _on_no_active_hover(
+            self,
+            from_active: bool = False,
+            from_hover: bool = False
+    ) -> None:
+        pg.mouse.set_cursor(pg.SYSTEM_CURSOR_ARROW)
 
-                if not self._display_config_configured.border_radius:
-                    self._display_config.border_radius = self.theme.frame.border_radius
+        super()._on_no_active_hover(from_active, from_hover)
 
-    def get_size(self) -> tuple[int, int]:
+    def stop_focus(self) -> None:
         """
-        get the frames size (including children)
+        called when the entry is unfocused
         """
-        # width
-        width = self._width if self._width_configured else self.assigned_width
-
-        # height
-        height = self._height if self._height_configured else self.assigned_height
-
-        return width.__floor__(), height.__floor__()
+        self._on_no_active_hover(True, False)
+        super().stop_focus()
 
     def draw(self, surface: pg.Surface) -> None:
         """
-        draw the frame
+        insert cursor if active
         """
-        width, height = self.get_size()
-        # print(f"drawing: \"{type(self).__name__}\"", (width, height), self._x, self._y, self._display_config.bg)
-        _surface = pg.Surface((width, height), pg.SRCALPHA)
-
-        # draw the frame
-        r_rect = pg.Rect((0, 0, width, height))
-        pg.draw.rect(
-            _surface,
-            self._display_config.bg.rgba,
-            r_rect,
-            border_top_left_radius=self._display_config.ulr,
-            border_top_right_radius=self._display_config.urr,
-            border_bottom_left_radius=self._display_config.llr,
-            border_bottom_right_radius=self._display_config.lrr,
-        )
+        self._is_active = self.focused
+        bg_width, bg_height = self._label.get_size()
 
-        if self._display_config.border_width > 0:
-            pg.draw.rect(
-                _surface,
-                self._display_config.border_color.rgba,
-                r_rect,
-                width=self._display_config.border_width,
-                border_top_left_radius=self._display_config.ulr,
-                border_top_right_radius=self._display_config.urr,
-                border_bottom_left_radius=self._display_config.llr,
-                border_bottom_right_radius=self._display_config.lrr,
-            )
-
-        # draw children
-        for child, params in self._child_params:
-            child.draw(_surface)
-
-        # draw
-        surface.blit(_surface, (self._x, self._y))
-
-    def place(
-            self,
-            x: int,
-            y: int,
-    ) -> None:
-        """
-        place the frame in a parent container
+        current_style = self.style
 
-        :param x: x-position
-        :param y: y-position
-        """
-        if self.__parent.layout is not Absolute:
-            raise TypeError("can't place in a container that is not managed by \"Absolute\"")
+        if self.is_hover:
+            current_style = self.style.overwrite(self.hover_style)
 
-        self.__parent.add_child(self, x=x, y=y)
+        if self.is_active:
+            current_style = self.style.overwrite(self.hover_style).overwrite(
+                self.active_style
+            )
 
-    def pack(
-            self,
-            anchor: tp.Literal["top", "bottom", "left", "right"] = TOP,
-    ) -> None:
-        """
-        pack the frame into a parent container
+        # set the label color to placeholder_color if no text has been entered
+        is_placeholder = not self._string_var.get()
+        if is_placeholder:
+            self._label.text_variable.set(self._placeholder_text)
+            self._label.style.color = self._placeholder_color
+
+        else:
+            self._label.text_variable.set(self._string_var.get())
+            self._label.style.color = self.style.color
+
+        super().draw(surface)
+
+        # cursor only when active and blink
+        if self.focused and int((2 * time.time()) % 2):
+            # calculate cursor position
+            x, y = self._label.get_position()
+            width, height = self._label.text_size
+
+            # get frame center
+            center_x = self._x + x + bg_width / 2
+            center_y = self._y + y + bg_height / 2
+
+            cursor_text = self._label._font.render(
+                self._string_var.get()[:self._cursor_pos],
+                True,
+                current_style.color.irgba
+            )
+            x_off = cursor_text.get_size()[0]
 
-        :param anchor: where to orient the frame at (direction)
-        """
-        if self.__parent.layout is not Pack:
-            raise TypeError("can't pack in a container that is not managed by \"Pack\"")
+            # center label on frame center
+            label_end = (
+                center_x - (0 if is_placeholder else width / 2) + x_off,
+                center_y - height / 2
+            )
 
-        self.__parent.add_child(self, anchor=anchor.lower())
+            pg.draw.rect(
+                surface,
+                current_style.color.irgb,
+                pg.Rect(label_end, (3, height))
+            )
 
-    def grid(
+    def notify(
             self,
-            row: int,
-            column: int,
-            sticky: str = "",
-            margin: int = 0,
+            event: (
+                    ThemeManager.NotifyEvent
+                    | Style.NotifyEvent
+                    | KeyboardNotifyEvent
+            ),
+            info: tp.Any = ...
     ) -> None:
-        """
-        grid the frame into a parent container
-
-        :param row: the row the item should be placed in
-        :param column: the column the item should be placed in
-        :param sticky: expansion, can be a combination of "n", "e", "s", "w"
-        :param margin: the distance to the grids borders
-        """
-        if self.__parent.layout is not Grid:
-            raise TypeError("can't grid in a container that is not managed by \"Grid\"")
-
-        self.__parent.add_child(self, row=row, column=column, sticky=sticky, margin=margin)
-
-    def set_position(self, x: int, y: int) -> None:
-        """
-        set the child's position (used by parents)
-        """
-        self._x = x
-        self._y = y
-
-    def set_size(self, width: float, height: float) -> None:
-        """
-        set the child's size (used by parens)
-        """
-        self.width = width
-        self.height = height
-
-    def delete(self) -> None:
-        """
-        delete the widget
-        """
-        self.__parent = ...
+        match event:
+            case KeyboardNotifyEvent.key_down:
+                if info.key == pg.K_BACKSPACE:
+                    s_len = len(self._string_var.get())
+
+                    # deletion if a scheme is given
+                    if self._scheme is not ...:
+                        if s_len > 0:
+                            if self._cursor_pos < s_len:
+                                # split string at the cursor and replace
+                                # the next character with a space character
+                                prev_string = self._string_var.get()
+                                self._string_var.set(
+                                    prev_string[
+                                        :self._cursor_pos
+                                    ]
+                                    + " "
+                                    + prev_string[self._cursor_pos + 1:]
+                                )
+
+                            else:
+                                # split the string at the cursor and delete
+                                # the next character
+                                prev_string = self._string_var.get()
+                                self._string_var.set(
+                                    prev_string[
+                                        :self._cursor_pos - 1
+                                    ]
+                                    + prev_string[self._cursor_pos:]
+                                )
+
+                                # de-increment cursor (if not already at 0)
+                                if self._cursor_pos >= 0:
+                                    self._cursor_pos -= 1
+
+                        return
+
+                    # normal deletion
+                    if s_len > 0:
+                        # split the string at the cursor and delete
+                        # the next character
+                        prev_string = self._string_var.get()
+                        self._string_var.set(
+                            prev_string[:self._cursor_pos-1]
+                            + prev_string[self._cursor_pos:]
+                        )
+
+                        # de-increment cursor (if not already at 0)
+                        if self._cursor_pos >= 0:
+                            self._cursor_pos -= 1
+
+                elif info.key == pg.K_RETURN:
+                    self.root.set_focus(self.root)
+                    self._execute_event(FrameBind.key_return)
+
+                elif info.key == pg.K_LEFT:
+                    if self._cursor_pos >= 0:
+                        self._cursor_pos -= 1
+
+                elif info.key == pg.K_RIGHT:
+                    if self._cursor_pos < len(self._string_var.get()):
+                        self._cursor_pos += 1
+
+                # if none of the above apply and a unicode character is
+                # present, add it to the string
+                elif info.unicode:
+                    override = False
+                    set_character = None
+                    next_valid = False
+
+                    # force capitalize - lower the character
+                    if self._f_upper:
+                        info.unicode = info.unicode.upper()
+
+                    if self._f_lower:
+                        info.unicode = info.unicode.lower()
+
+                    # check max length
+                    if self._max_length is not None and\
+                            self._cursor_pos >= self._max_length:
+                        return
+
+                    # check valid symbols
+                    if self._allowed is not ... and\
+                            info.unicode not in self._allowed\
+                            and self._scheme is ...:
+                        return
+
+                    if self._scheme is not ...:
+                        override = True
+                        try:
+                            # check current character
+                            is_valid, punct = self._scheme.validate(
+                                self._cursor_pos,
+                                info.unicode
+                            )
 
-        # terminate all children
-        for child in self._children:
-            child.delete()
+                            # check next character
+                            with suppress(IndexError):
+                                next_valid, _ = self._scheme.validate(
+                                    self._cursor_pos + 1, info.unicode
+                                )
+
+                            if is_valid:
+                                if punct is not None:
+                                    set_character = punct
+
+                            else:
+                                return
+
+                        except IndexError:
+                            return
+
+                    # insert character at cursor position
+                    prev_string = self._string_var.get()
+                    self._string_var.set(
+                        prev_string[:self._cursor_pos]
+                        + (set_character if set_character is not None else "")
+                        + info.unicode
+                        + prev_string[self._cursor_pos+override:]
+                    )
+                    self._cursor_pos += 1 + (
+                            next_valid and set_character is not None
+                    )
+
+            case GeoNotes.SetActive:
+                new_index = self._label.get_index_on_position(
+                    info[0] - self._x
+                )
+
+                if 0 <= new_index <= len(self._string_var.get()):
+                    self._cursor_pos = new_index
+
+                print("index: ", new_index)
+
+                if self._notify_child_active_hover(info):
+                    self.set_no_hover_active()
+                else:
+                    self.set_active()
+
+            case _:
+                super().notify(event, info)
+
+
+# TODO: clickable cursor
+# TODO: enabled / disabled
+# TODO: not shown if no height | width | sticky is given
```

### Comparing `pginter-0.1.0/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.0/src/pginter/widgets/_geo_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,124 +3,320 @@
 04. February 2023
 
 How children are placed
 
 Author:
 Nilusink
 """
-from ..types import Absolute, Pack, Grid, BetterDict, TOP, BOTTOM, LEFT, RIGHT
+from ..types import Layout, BetterDict, TOP, BOTTOM, LEFT, RIGHT, GeoNotes
 from ._supports_children import SupportsChildren
+from ..utils import point_in_box
 from copy import deepcopy
 import typing as tp
+import pygame as pg
+
+
+if tp.TYPE_CHECKING:
+    from ._frame import Frame
 
 
 class GeometryManager(SupportsChildren):
     """
     Manages how children are placed inside a parent container
     """
-    _layout: int = Absolute
-    _width: float = 0   # -1 means not configured -> takes minimum size required by its children
+    _layout: Layout = Layout.Absolute
+    _width: float = 0   # -1 means not configured -> takes minimum size
+    # required by its children
     _height: float = 0  # or the size it gets by the parents geometry manager
     assigned_width: float = 0
     assigned_height: float = 0
     _width_configured: bool = False
     _height_configured: bool = False
     _child_params: list[tuple[tp.Any, BetterDict]] = ...
     layout_params: BetterDict = ...
     _grid_params: BetterDict = ...
 
+    _child_override: bool = False
+    _is_active: bool = False
+    _is_hover: bool = False
+
     def __init__(
             self,
-            layout: int = ...,
+            layout: Layout = ...,
             margin: int = 0,
             padding: int = 0
     ):
         super().__init__()
 
-        self._layout = Absolute if layout is ... else layout
+        if layout is not ...:
+            if layout not in (Layout.Grid, Layout.Pack, Layout.Absolute):
+                raise ValueError(f"Invalid layout type: {layout}")
+
+        self._layout = Layout.Absolute if layout is ... else layout
         self.layout_params = BetterDict({
             "margin": margin,
             "padding": padding
         })
         self._child_params = []
         self._grid_params = BetterDict({
             "rows": {},
             "columns": {}
         })
 
     @property
-    def layout(self) -> int:
+    def layout(self) -> Layout:
         """
         the containers layout type
         """
         return self._layout
 
     @property
     def width(self) -> float:
         return self._width
     
     @width.setter
     def width(self, value: float) -> None:
         self._width = value
         self._width_configured = True
 
+    def unset_width(self) -> None:
+        """
+        act as if the width has never been set
+        """
+        self._width_configured = False
+
     @property
     def height(self) -> float:
         return self._height
 
     @height.setter
     def height(self, value: float) -> None:
         self._height = value
         self._height_configured = True
 
+    def unset_height(self) -> None:
+        """
+        act as if the height has never been set
+        """
+        self._height_configured = False
+
+    @property
+    def is_hover(self) -> bool:
+        return self._is_hover
+
+    @property
+    def is_active(self) -> bool:
+        return self._is_active
+
+    def set_focus(self, widget: tp.Union["GeometryManager", None]):
+        """
+        set this item as currently focused
+        """
+
+    def stop_focus(self):
+        """
+        remove focus from this item
+        """
+
+    def _on_active(self) -> None:
+        """
+        called when button is clicked
+        not implemented by default
+        """
+
+    def _on_hover(self) -> None:
+        """
+        called on hover
+        not implemented by default
+        """
+
+    def _on_no_active_hover(
+            self,
+            from_active: bool = False,
+            from_hover: bool = False
+    ) -> None:
+        """
+        called when either hover or active goes back to normal
+        not implemented by default
+        """
+
+    def set_active(self, override: bool = False) -> None:
+        """
+        change the widget to an active state
+        """
+        if not self._child_override:
+            if not self._is_active:  # only call on new event
+                self._on_active()
+
+            self._is_hover = False
+            self._is_active = True
+
+        self._child_override = self._child_override or override
+
+    def set_hover(self, override: bool = False) -> None:
+        """
+        set the widget to a hover state
+        """
+        if not self._child_override:
+            if not self._is_hover:  # only call on new event
+                self._on_hover()
+
+            self._is_hover = True
+            self._is_active = False
+
+        self._child_override = self._child_override or override
+
+    def set_no_hover_active(self, override: bool = False) -> None:
+        """
+        set the widget to "normal" mode
+        """
+        if not self._child_override:
+            if self._is_hover or self._is_active:  # only call no new event
+                self._on_no_active_hover(self._is_active, self._is_hover)
+
+            self._is_hover = False
+            self._is_active = False
+
+        self._child_override = self._child_override or override
+
+    def _notify_child_active_hover(self, mouse_pos: tuple[int, int]) -> bool:
+        has_hit: bool = False
+
+        for child in self._children:
+            child: Frame
+
+            pos = child.get_position()
+            size = child.get_size()
+
+            # noinspection PyTypeChecker
+            if point_in_box(mouse_pos, (*pos, *size)):
+                has_hit = True
+                child.notify(
+                    GeoNotes.SetActive if pg.mouse.get_pressed(3)[0]
+                    else GeoNotes.SetHover,
+                    (mouse_pos[0] - pos[0], mouse_pos[1] - pos[1])
+                )
+                continue
+
+            child.notify(GeoNotes.SetNormal)
+
+        return has_hit
+
+    def notify(self, event, info) -> None:
+        """
+        for notifications from child / parent classes
+        """
+        self._child_override = False
+        match event:
+            case GeoNotes.SetHover:
+                if self._notify_child_active_hover(info):
+                    self.set_no_hover_active()
+                else:
+                    self.set_hover()
+
+            case GeoNotes.SetActive:
+                if self._notify_child_active_hover(info):
+                    self.set_no_hover_active()
+                else:
+                    self.set_active()
+
+            case GeoNotes.SetNormal:
+                # also set children to inactive
+                self._notify_child_active_hover((-1, -1))
+
+                self.set_no_hover_active()
+
     # layout configuration
-    def set_layout(self, layout: int) -> None:
+    def set_layout(self, layout: Layout) -> None:
         """
         set the container's layout type
         """
-        if layout not in (Absolute, Pack, Grid):
+        if layout not in Layout:
             raise ValueError("Invalid container layout: ", layout)
 
-        if len(self._child_params) > 0:
-            # if children are already present, delete them
-            for child, _param in self._child_params:
-                child.delete()
+        if self._layout != layout:
+            if len(self._child_params) > 0:
+                # if children are already present, delete them
+                for child, _param in self._child_params:
+                    child.delete()
 
-            self._child_params.clear()
+                self._child_params.clear()
 
-            raise RuntimeWarning("changing layout with children already present!")
+                raise RuntimeWarning(
+                    "changing layout with children already present!"
+                )
 
-        self._layout = layout
+            self._layout = layout
 
-    def grid_columnconfigure(self, column: int | tp.Iterable[int], weight: float = 1) -> None:
+    def check_set_layout(self, layout: Layout) -> bool:
+        """
+        checks if the layout can be changed
+        """
+        # not a real layout type
+        if layout not in Layout:
+            return False
+
+        # is already the same layout
+        if self._layout == layout:
+            return True
+
+        # no children present - can be easily changed
+        if len(self._children) == 0:
+            return True
+
+        return False
+
+    def grid_columnconfigure(
+            self,
+            column: int | tp.Iterable[int],
+            weight: float = 1
+    ) -> None:
         """
         configure one or more grid columns
         """
-        # if the column is given as a list, call this function with an integer as parameter
+        # if the column is given as a list,
+        # call this function with an integer as parameter
         if isinstance(column, tp.Iterable):
             for c in column:
                 self.grid_columnconfigure(c, weight=weight)
 
             return
 
+        # check if the layout is "grid"
+        if not self.check_set_layout(Layout.Grid):
+            raise ValueError("Invalid geometry type for grid-configuration")
+
+        self.set_layout(Layout.Grid)
+
         self._grid_params["columns"][column] = {
             "weight": weight
         }
 
-    def grid_rowconfigure(self, row: int | tp.Iterable[int], weight: float = 1) -> None:
+    def grid_rowconfigure(
+            self,
+            row: int | tp.Iterable[int],
+            weight: float = 1
+    ) -> None:
         """
         configure one or more grid rows
         """
-        # if the row is given a list, call this function with an integer as parameter
+        # if the row is given a list, call this
+        # function with an integer as parameter
         if isinstance(row, tp.Iterable):
             for r in row:
                 self.grid_rowconfigure(r, weight=weight)
 
             return
 
+        # check if the layout is "grid"
+        if not self.check_set_layout(Layout.Grid):
+            raise ValueError("Invalid geometry type for grid-configuration")
+
+        self.set_layout(Layout.Grid)
+
         self._grid_params["rows"][row] = {
             "weight": weight
         }
 
     # other stuff
     def add_child(self, child: tp.Any, **params) -> None:
         """
@@ -131,21 +327,27 @@
             self._child_params.append((child, BetterDict(params)))
 
     def calculate_geometry(self):
         """
         calculate how each individual child should be placed
         """
         match self._layout:
-            case 0:  # Absolute
-                # since the positioning is absolute, the children should not influence the parents size
+            case Layout.Absolute:
+                # since the positioning is absolute,
+                # the children should not influence the parents size
                 for child, params in self._child_params:
                     child.set_position(params.x, params.y)
 
-            case 1:  # pack
-                directional_dict: dict[str, int | list] = {"total_x": 0, "total_y": 0, "children": [], "sizes": []}
+            case Layout.Pack:
+                directional_dict: dict[str, int | list] = {
+                    "total_x": 0,
+                    "total_y": 0,
+                    "children": [],
+                    "sizes": []
+                }
                 top = deepcopy(directional_dict)
                 bottom = deepcopy(directional_dict)
                 left = deepcopy(directional_dict)
                 right = deepcopy(directional_dict)
 
                 # get all sizes and group by anchor
                 for child, param in self._child_params:
@@ -171,23 +373,33 @@
 
                     elif param.anchor == RIGHT:
                         right["children"].append(child)
                         right["sizes"].append(child_size)
                         right["total_x"] += child_size[0]
                         right["total_y"] += child_size[1]
 
-                top["total_y"] += self.layout_params.padding * len(top["children"]) - 1
-                bottom["total_y"] += self.layout_params.padding * len(bottom["children"]) - 1
-
-                left["total_x"] += self.layout_params.padding * len(left["children"]) - 1
-                right["total_x"] += self.layout_params.padding * len(right["children"]) - 1
+                top["total_y"] += self.layout_params.padding * len(
+                    top["children"]
+                ) - 1
+                bottom["total_y"] += self.layout_params.padding * len(
+                    bottom["children"]
+                ) - 1
+
+                left["total_x"] += self.layout_params.padding * len(
+                    left["children"]
+                ) - 1
+                right["total_x"] += self.layout_params.padding * len(
+                    right["children"]
+                ) - 1
 
                 # if not configured, set own size
-                total_x = max([top["total_x"], bottom["total_x"], left["total_x"] + right["total_x"]])
-                total_y = max([left["total_y"], right["total_y"], top["total_y"] + bottom["total_y"]])
+                total_x = max([top["total_x"], bottom["total_x"],
+                               left["total_x"] + right["total_x"]])
+                total_y = max([left["total_y"], right["total_y"],
+                               top["total_y"] + bottom["total_y"]])
 
                 # add margin
                 total_x += self.layout_params.margin * 2
                 total_y += self.layout_params.margin * 2
 
                 if not self._width_configured:
                     self._width = total_x
@@ -225,194 +437,260 @@
 
                 # bottom
                 y_now = total_y - self.layout_params.margin
                 for child, size in zip(bottom["children"], bottom["sizes"]):
                     child.set_position(x_cen - size[0] / 2, y_now - size[1])
                     y_now -= size[1] + self.layout_params.padding
 
-            case 2:  # grid
-                rows: list[dict[str, tp.Any | float]] = []
-                columns: list[dict[str, tp.Any | float]] = []
+            case Layout.Grid:
+                rows: list[dict[
+                    str,
+                    list[tuple[tp.Any, BetterDict, bool]] | float
+                ]] = []
+                columns: list[dict[
+                    str,
+                    list[tuple[tp.Any, BetterDict, bool]] | float
+                ]] = []
 
                 for child, params in self._child_params:
                     row, column = params["row"], params["column"]
 
                     # if row was not yet made, make all previous ones
-                    if len(rows) <= row:
-                        for n_row in range(len(rows), row+1):
+                    min_rows = row + params.rowspan - 1
+                    min_columns = column + params.columnspan - 1
+
+                    if len(rows) <= min_rows:
+                        for n_row in range(len(rows), min_rows+1):
                             out = {
                                 "weight": 0,
                                 "children": []
                             }
 
                             if n_row in self._grid_params.rows:
                                 config = self._grid_params.rows[n_row]
 
                                 if "weight" in config:
                                     out["weight"] = config["weight"]
 
                             rows.append(out)
 
-                    if len(columns) <= column:
-                        for n_col in range(len(columns), column+1):
+                    if len(columns) <= min_columns:
+                        for n_col in range(len(columns), min_columns+1):
                             out = {
                                 "weight": 0,
                                 "children": []
                             }
 
                             if n_col in self._grid_params.columns:
                                 config = self._grid_params.columns[n_col]
 
                                 if "weight" in config:
                                     out["weight"] = config["weight"]
 
                             columns.append(out)
 
-                    rows[row]["children"].append((child, params))
-                    columns[column]["children"].append((child, params))
+                    rows[row]["children"].append((child, params, True))
+                    
+                    # if rowspan is given, also add the widget to all the
+                    # corresponding other rows
+                    if "rowspan" in params:
+                        for row_incrementor in range(1, params.rowspan):
+                            rows[row + row_incrementor]["children"]\
+                                .append(
+                                (child, params, False)
+                            )
+
+                    columns[column]["children"].append((child, params, True))
+
+                    if "columnspan" in params:
+                        for column_incrementor in range(1, params.columnspan):
+                            columns[column + column_incrementor]["children"]\
+                                .append(
+                                (child, params, False)
+                            )
 
                 matrix: list[list] = []
 
+                # append all the children to a 2d matrix and check if one
+                # cell has multiple children
                 for r in range(len(rows)):
                     matrix.append([])
 
                     for c in range(len(columns)):
-                        # child = set(rows[r]["children"]) & set(columns[c]["children"])
-                        child = [chi for chi in rows[r]["children"] if chi in columns[c]["children"]]
+                        child = [
+                            chi for chi in rows[r]["children"]
+                            if chi in columns[c]["children"]
+                        ]
                         child = list(child)
 
                         if len(child) > 1:
-                            raise ValueError(f"{len(child)} children assigned to row {r} column {c}!")
+                            raise ValueError(
+                                f"{len(child)} children assigned "
+                                f"to row {r} column {c}!"
+                            )
 
                         if child:
                             matrix[r].append(child[0])
 
                         else:
                             matrix[r].append(...)
 
                 # calculate the minimal size for each row
                 for r, row in enumerate(rows):
                     rows[r]["max_size"] = 0
 
-                    for child, params in row["children"]:
-                        _, y = child.calculate_size()
+                    for child, params, _is_widget in row["children"]:
+                        child.calculate_size()
+                        _, y = child.get_size()
 
                         y += 2 * params.margin
 
+                        # split size between rows
+                        y /= params.rowspan
+
                         if y > rows[r]["max_size"]:
                             rows[r]["max_size"] = y
 
-                    # calculate the minimal size for each column
+                # calculate the minimal size for each column
                 for c, column in enumerate(columns):
                     columns[c]["max_size"] = 0
 
-                    for child, params in column["children"]:
-                        x, _ = child.calculate_size()
+                    for child, params, _is_widget in column["children"]:
+                        child.calculate_size()
+                        x, _ = child.get_size()
 
                         x += 2 * params.margin
 
+                        # split size between columns
+                        x /= params.columnspan
+
                         if x > columns[c]["max_size"]:
                             columns[c]["max_size"] = x
 
                 # calculate the container size
                 width, height = self.assigned_width, self.assigned_height
 
                 # only subtract rows that don't have a weight
                 min_width = sum([c["max_size"] for c in columns])
                 min_height = sum([r["max_size"] for r in rows])
 
-                # assign extra space
-                extra_width = width - sum([c["max_size"] for c in columns if c["weight"] == 0])
-                extra_height = height - sum([r["max_size"] for r in rows if r["weight"] == 0])
+                if len(columns) + len(rows) > 0:
+                    if width == 0 or height == 0 and not\
+                            self._width_configured:
+                        self._width = min_width
+
+                    if width == 0 or height == 0 and not\
+                            self._height_configured:
+                        self._height = min_height
 
-                total_row_weight = sum([row["weight"] for row in rows])
-                total_column_weight = sum([column["weight"] for column in columns])
+                if self._width_configured:
+                    width = self._width
 
-                # print(f"\n\nwindow_size=[{width}, {height}]\tmin_size={[min_width, min_height]}")
-                # print(f"{total_row_weight=}")
-                # print(f"{total_column_weight=}")
-                # print(f"{extra_height=}")
-                # print(f"{extra_width=}")
+                if self._height_configured:
+                    height = self.height
+
+                # assign extra space
+                extra_width = width - sum(
+                    [c["max_size"] for c in columns if c["weight"] == 0]
+                )
+                extra_height = height - sum(
+                    [r["max_size"] for r in rows if r["weight"] == 0]
+                )
+
+                total_row_weight = sum(
+                    [row["weight"] for row in rows]
+                )
+                total_column_weight = sum(
+                    [column["weight"] for column in columns]
+                )
 
                 # assign each row and column a specific size
                 for r in range(len(rows)):
                     if total_row_weight == 0:
                         rows[r]["height"] = 0
-                    else:
-                        # assign either the minimum size or the calculated dynamic one
-                        w_size = ((rows[r]["weight"] / total_row_weight) * extra_height).__floor__()
-                        rows[r]["height"] = max([w_size, rows[r]["max_size"]])
-                        # print(f"{w_size=}\t{rows[r]['max_size']=}")
 
-                    # rows[r]["height"] += rows[r]["max_size"]
-                    rows[r]["y_start"] = sum([prev_row["height"] for prev_row in rows[:r]])
+                    else:
+                        # assign either the minimum size or the
+                        # calculated dynamic one
+                        w_size = (
+                                (rows[r]["weight"] / total_row_weight)
+                                * extra_height
+                        ).__floor__()
+                        rows[r]["height"] = w_size
+
+                    rows[r]["y_start"] = self.layout_params.padding / 2 + sum(
+                        [prev_row["height"] for prev_row in rows[:r]]
+                    )
 
                     for c in range(len(columns)):
                         if total_column_weight == 0:
                             columns[c]["width"] = 0
-                        else:
-                            # assign either the minimum size or the calculated dynamic one
-                            w_size = ((columns[c]["weight"] / total_column_weight) * extra_width).__floor__()
-                            columns[c]["width"] = max([w_size, columns[c]["max_size"]])
-                            # print(f"{w_size=}\t{columns[c]['max_size']=}")
 
-                        # columns[c]["width"] += columns[c]["max_size"]
-                        columns[c]["x_start"] = sum([prev_col["width"] for prev_col in columns[:c]])
+                        else:
+                            # assign either the minimum size or the
+                            # calculated dynamic one
+                            w_size = (
+                                    (
+                                            columns[c]["weight"]
+                                            / total_column_weight
+                                    )
+                                    * extra_width
+                            ).__floor__()
+                            columns[c]["width"] = w_size
+
+                        columns[c]["x_start"] = self.layout_params.padding / 2\
+                            + sum(
+                            [prev_col["width"] for prev_col in columns[:c]]
+                        )
 
                 # place children
                 for child, params in self._child_params:
                     # place the child proportional to the table and stickiness
                     # size = list(child.calculate_size())
                     size = [child._width, child._height]
 
-                    row, column = params["row"], params["column"]
-                    sticky = params["sticky"]
-
-                    width = columns[column]["width"]
-                    height = rows[row]["height"]
+                    row, column = params.row, params.column
+                    sticky = params.sticky
+                    margin = params.margin
+
+                    width = sum([
+                        columns[c]["width"] for c in
+                        range(column, column + params.columnspan)
+                    ])
+                    height = sum([
+                        rows[r]["height"] for r in
+                        range(row, row + params.rowspan)
+                    ])
 
                     x = columns[column]["x_start"]
                     y = rows[row]["y_start"]
 
-                    x_cen = x + width / 2
-                    y_cen = y + height / 2
-
                     x_diff = width - size[0]
                     y_diff = height - size[1]
 
-                    # print(f"calc: {x_diff}, {y_diff}\t{size}\t{width},{height}")
-                    # print(f"{sticky=}")
-
-                    box_x = x_cen - size[0] / 2
-                    box_y = y_cen - size[1] / 2
-
                     # assign stickiness
                     if not child._width_configured:
                         if "w" in sticky:
                             size[0] += (x_diff / 2) - params.margin
-                            box_x = x + params.margin
 
                         if "e" in sticky:
                             size[0] += (x_diff / 2) - params.margin
 
                         child.assigned_width = size[0]
 
                     if not child._height_configured:
                         if "n" in sticky:
                             size[1] += (y_diff / 2) - params.margin
-                            box_y = y + params.margin
-                            # print("north: ", size, box_x, box_y, "\t\t", width, height)
 
                         if "s" in sticky:
                             size[1] += (y_diff / 2) - params.margin
-                            # print("south: ", size, box_x, box_y, "\t\t", width, height)
 
                         child.assigned_height = size[1]
 
-                    child.set_position(box_x, box_y)
+                    child.set_position(x + margin, y + margin)
 
             case _:
                 raise ValueError(f"Invalid geometry type: {self._layout}")
 
     def calculate_size(self) -> tuple[int, int]:
         """
         calculate how big the container should be
```

### Comparing `pginter-0.1.0/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.0/src/pginter.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,27 @@
 src/pginter/icon.png
 src/pginter.egg-info/PKG-INFO
 src/pginter.egg-info/SOURCES.txt
 src/pginter.egg-info/dependency_links.txt
 src/pginter.egg-info/top_level.txt
 src/pginter/theme/__init__.py
 src/pginter/theme/_manager.py
-src/pginter/theme/themes/default.json
 src/pginter/types/__init__.py
 src/pginter/types/_better_dict.py
+src/pginter/types/_binds.py
 src/pginter/types/_color.py
 src/pginter/types/_constants.py
 src/pginter/types/_geo_types.py
+src/pginter/types/_notifications.py
+src/pginter/types/_scheme.py
+src/pginter/types/_style.py
+src/pginter/types/_tk_vars.py
 src/pginter/utils/__init__.py
 src/pginter/utils/_funcs.py
 src/pginter/widgets/__init__.py
+src/pginter/widgets/_button.py
+src/pginter/widgets/_entry.py
 src/pginter/widgets/_frame.py
 src/pginter/widgets/_geo_manager.py
 src/pginter/widgets/_label.py
-src/pginter/widgets/_supports_children.py
+src/pginter/widgets/_supports_children.py
+src/pginter/widgets/_surface_frame.py
```

