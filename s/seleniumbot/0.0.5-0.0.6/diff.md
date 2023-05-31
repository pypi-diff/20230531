# Comparing `tmp/seleniumbot-0.0.5.tar.gz` & `tmp/seleniumbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seleniumbot-0.0.5.tar", last modified: Tue May 30 20:49:27 2023, max compression
+gzip compressed data, was "seleniumbot-0.0.6.tar", last modified: Wed May 31 17:11:50 2023, max compression
```

## Comparing `seleniumbot-0.0.5.tar` & `seleniumbot-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4528 2023-05-23 19:49:50.000000 seleniumbot-0.0.5/README.md
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.411940 seleniumbot-0.0.5/seleniumbot/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      270 2023-05-30 18:59:50.000000 seleniumbot-0.0.5/seleniumbot/__init__.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot/core/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.5/seleniumbot/core/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1495 2023-05-30 20:43:09.000000 seleniumbot-0.0.5/seleniumbot/core/action.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3290 2023-05-30 20:39:13.000000 seleniumbot-0.0.5/seleniumbot/core/client.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     2485 2023-05-30 20:45:10.000000 seleniumbot-0.0.5/seleniumbot/core/seleniumbot.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot/utils/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.5/seleniumbot/utils/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      322 2023-05-30 18:59:50.000000 seleniumbot-0.0.5/seleniumbot/utils/logger.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.5/seleniumbot/utils/randomizer.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot.egg-info/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/SOURCES.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/dependency_links.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       23 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/requires.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/top_level.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/setup.cfg
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      651 2023-05-30 20:46:29.000000 seleniumbot-0.0.5/setup.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4528 2023-05-23 19:49:50.000000 seleniumbot-0.0.6/README.md
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/seleniumbot/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      270 2023-05-30 18:59:50.000000 seleniumbot-0.0.6/seleniumbot/__init__.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/seleniumbot/core/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.6/seleniumbot/core/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1503 2023-05-31 17:06:48.000000 seleniumbot-0.0.6/seleniumbot/core/action.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3290 2023-05-30 20:39:13.000000 seleniumbot-0.0.6/seleniumbot/core/client.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     2592 2023-05-31 17:06:48.000000 seleniumbot-0.0.6/seleniumbot/core/seleniumbot.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/seleniumbot/utils/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.6/seleniumbot/utils/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      322 2023-05-30 18:59:50.000000 seleniumbot-0.0.6/seleniumbot/utils/logger.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.6/seleniumbot/utils/randomizer.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/seleniumbot.egg-info/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-31 17:11:50.000000 seleniumbot-0.0.6/seleniumbot.egg-info/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-31 17:11:50.000000 seleniumbot-0.0.6/seleniumbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-31 17:11:50.000000 seleniumbot-0.0.6/seleniumbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       23 2023-05-31 17:11:50.000000 seleniumbot-0.0.6/seleniumbot.egg-info/requires.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-31 17:11:50.000000 seleniumbot-0.0.6/seleniumbot.egg-info/top_level.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-31 17:11:50.291308 seleniumbot-0.0.6/setup.cfg
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      651 2023-05-31 17:10:28.000000 seleniumbot-0.0.6/setup.py
```

### Comparing `seleniumbot-0.0.5/PKG-INFO` & `seleniumbot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: SeleniumBot
 Home-page: https://github.com/Mercurial5
 Author: Mercurial5
 Author-email: dias.nespayev@gmail.com
 Keywords: SeleniumBot
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `seleniumbot-0.0.5/README.md` & `seleniumbot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.5/seleniumbot/core/action.py` & `seleniumbot-0.0.6/seleniumbot/core/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from abc import ABC, abstractmethod
 
 from selenium.common.exceptions import WebDriverException
 
 from seleniumbot.core.client import SeleniumClient
 from seleniumbot.utils import get_logger
 
-logger = get_logger()
+logger = get_logger(__name__)
 
 
 class ActionException(Exception):
     pass
 
 
 class Action(ABC):
```

### Comparing `seleniumbot-0.0.5/seleniumbot/core/client.py` & `seleniumbot-0.0.6/seleniumbot/core/client.py`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.5/seleniumbot/core/seleniumbot.py` & `seleniumbot-0.0.6/seleniumbot/core/seleniumbot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+import inspect
 import random
 from datetime import timedelta, datetime
 from typing import Type
 
 from seleniumbot.core.action import Action, AFKAction, ActionException
 from seleniumbot.core.client import SeleniumClient
 from seleniumbot.utils import get_logger
 from seleniumbot.utils.randomizer import Randomizer
 
 logger = get_logger(__name__)
 
 
 class SeleniumBot:
-    def __init__(self, start_action: Type[Action], work_time: timedelta, **kwargs):
+    def __init__(self, start_action: Type[Action] | Action, work_time: timedelta, **kwargs):
         self.start_time = datetime.now()
         self.end_time = self.start_time + work_time
 
         options = kwargs.get('options')
         seleniumwire_options = kwargs.get('seleniumwire_options')
         self.client = SeleniumClient(options=options, seleniumwire_options=seleniumwire_options)
 
         self.navigations = []
         self.actions: list[Action] = []
         self.last_action: Action | None = None
 
-        start_action().execute(self.client, self.last_action)
+        if inspect.isclass(start_action):
+            start_action = start_action()
+
+        start_action.execute(self.client, self.last_action)
 
         self.history = set()
 
         self.__comp = lambda action, x: action.coefficient > x
 
     def set_navigation_actions(self, actions: list[Type[Action]]):
         self.navigations = [action() for action in actions]
```

### Comparing `seleniumbot-0.0.5/seleniumbot/utils/randomizer.py` & `seleniumbot-0.0.6/seleniumbot/utils/randomizer.py`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.5/seleniumbot.egg-info/PKG-INFO` & `seleniumbot-0.0.6/seleniumbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: SeleniumBot
 Home-page: https://github.com/Mercurial5
 Author: Mercurial5
 Author-email: dias.nespayev@gmail.com
 Keywords: SeleniumBot
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `seleniumbot-0.0.5/setup.py` & `seleniumbot-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='seleniumbot',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     url='https://github.com/Mercurial5',
     author='Mercurial5',
     author_email='dias.nespayev@gmail.com',
     keywords='SeleniumBot',
     description='SeleniumBot',
     python_requires=">=3.11",
```

