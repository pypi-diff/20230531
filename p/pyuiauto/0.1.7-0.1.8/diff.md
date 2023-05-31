# Comparing `tmp/pyuiauto-0.1.7.tar.gz` & `tmp/pyuiauto-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuiauto-0.1.7.tar", max compression
+gzip compressed data, was "pyuiauto-0.1.8.tar", max compression
```

## Comparing `pyuiauto-0.1.7.tar` & `pyuiauto-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35823 2023-05-11 11:46:20.965940 pyuiauto-0.1.7/LICENSE
--rw-r--r--   0        0        0      956 2023-05-15 10:43:29.284240 pyuiauto-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 10:13:35.566412 pyuiauto-0.1.7/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-05-11 11:46:20.969173 pyuiauto-0.1.7/pyuiauto/application.py
--rw-r--r--   0        0        0     9796 2023-05-15 10:14:01.090897 pyuiauto-0.1.7/pyuiauto/base/__pycache__/application.cpython-39.pyc
--rw-r--r--   0        0        0    18104 2023-05-15 10:14:01.088892 pyuiauto-0.1.7/pyuiauto/base/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     7851 2023-05-15 10:08:51.151711 pyuiauto-0.1.7/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16607 2023-05-15 10:08:51.151711 pyuiauto-0.1.7/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     7883 2023-05-15 10:08:51.152715 pyuiauto-0.1.7/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    11678 2023-05-15 10:08:51.152715 pyuiauto-0.1.7/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2522 2023-05-11 11:46:20.971889 pyuiauto-0.1.7/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-05-11 11:46:20.971889 pyuiauto-0.1.7/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0      162 2023-05-15 09:48:46.590621 pyuiauto-0.1.7/pyuiauto/win/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9121 2023-05-15 11:28:34.364215 pyuiauto-0.1.7/pyuiauto/win/__pycache__/application.cpython-39.pyc
--rw-r--r--   0        0        0    13624 2023-05-15 10:14:01.084613 pyuiauto-0.1.7/pyuiauto/win/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     8665 2023-05-15 11:28:19.266546 pyuiauto-0.1.7/pyuiauto/win/application.py
--rw-r--r--   0        0        0    10557 2023-05-15 10:08:51.154160 pyuiauto-0.1.7/pyuiauto/win/components.py
--rw-r--r--   0        0        0     4403 2023-05-15 10:08:51.148948 pyuiauto-0.1.7/README.md
--rw-r--r--   0        0        0     5470 1970-01-01 00:00:00.000000 pyuiauto-0.1.7/setup.py
--rw-r--r--   0        0        0     5413 1970-01-01 00:00:00.000000 pyuiauto-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-05-11 11:46:20.965940 pyuiauto-0.1.8/LICENSE
+-rw-r--r--   0        0        0      956 2023-05-31 12:14:25.293598 pyuiauto-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 10:13:35.566412 pyuiauto-0.1.8/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-11 11:46:20.969173 pyuiauto-0.1.8/pyuiauto/application.py
+-rw-r--r--   0        0        0     9796 2023-05-15 10:14:01.090897 pyuiauto-0.1.8/pyuiauto/base/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    18104 2023-05-15 10:14:01.088892 pyuiauto-0.1.8/pyuiauto/base/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     7850 2023-05-16 09:13:11.658254 pyuiauto-0.1.8/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16607 2023-05-15 10:08:51.151711 pyuiauto-0.1.8/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.970476 pyuiauto-0.1.8/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     7883 2023-05-15 10:08:51.152715 pyuiauto-0.1.8/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    11721 2023-05-30 10:51:06.055613 pyuiauto-0.1.8/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-11 11:46:20.971889 pyuiauto-0.1.8/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.971889 pyuiauto-0.1.8/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0      162 2023-05-15 09:48:46.590621 pyuiauto-0.1.8/pyuiauto/win/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9121 2023-05-15 11:28:34.364215 pyuiauto-0.1.8/pyuiauto/win/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    13624 2023-05-15 10:14:01.084613 pyuiauto-0.1.8/pyuiauto/win/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     8702 2023-05-16 09:13:52.371143 pyuiauto-0.1.8/pyuiauto/win/application.py
+-rw-r--r--   0        0        0    10568 2023-05-30 16:19:57.774682 pyuiauto-0.1.8/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     4621 2023-05-31 12:14:15.945342 pyuiauto-0.1.8/README.md
+-rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 pyuiauto-0.1.8/setup.py
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 pyuiauto-0.1.8/PKG-INFO
```

### Comparing `pyuiauto-0.1.7/LICENSE` & `pyuiauto-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyproject.toml` & `pyuiauto-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyuiauto-0.1.7/pyuiauto/base/__pycache__/application.cpython-39.pyc` & `pyuiauto-0.1.8/pyuiauto/base/__pycache__/application.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/base/__pycache__/components.cpython-39.pyc` & `pyuiauto-0.1.8/pyuiauto/base/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/base/application.py` & `pyuiauto-0.1.8/pyuiauto/base/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         '''Application class get crash report method\n
         Gets all crash reports between the start and end time of the application running.'''
 
     def relaunchApp(self):
         '''Application class relaunch app method\n
         Uses it's context manager __enter__ __exit__ methods to quit and reopen the application.'''
         self.__exit__()
-        self.launchApp()
+        time.sleep(0.5)
         self.__enter__()
 
     def __enter__(self) -> UIApplicationWrapper:
         self.launchApp()
         self.connectApp()
         return self
```

### Comparing `pyuiauto-0.1.7/pyuiauto/base/components.py` & `pyuiauto-0.1.8/pyuiauto/base/components.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/exceptions.py` & `pyuiauto-0.1.8/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/mac/application.py` & `pyuiauto-0.1.8/pyuiauto/mac/application.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/mac/components.py` & `pyuiauto-0.1.8/pyuiauto/mac/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
         """Construct the control wrapper"""
         return super(UIBaseComponent, cls)._create_wrapper(cls, component, UIBaseComponent)
 
     # -----------------------------------------------------------
     def __init__(self, component: NativeUIElement):
         UIBaseComponentWrapper.__init__(self, component)
 
+        self.component: NativeUIElement
+
     def getValue(self):
         return self.component.AXValue
     
     def setValue(self, value):
         self.component.AXValue = value
     
     def setFocus(self):
```

### Comparing `pyuiauto-0.1.7/pyuiauto/wait.py` & `pyuiauto-0.1.8/pyuiauto/wait.py`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/win/__pycache__/application.cpython-39.pyc` & `pyuiauto-0.1.8/pyuiauto/win/__pycache__/application.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/win/__pycache__/components.cpython-39.pyc` & `pyuiauto-0.1.8/pyuiauto/win/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyuiauto-0.1.7/pyuiauto/win/application.py` & `pyuiauto-0.1.8/pyuiauto/win/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         try:
             self._getIcon(backendExplorer.taskbar)
         except:
                 self.__systrayExpandWindow = None
                 self._iconHidden = True
     
     def _getIcon(self, parent: pywinauto.WindowSpecification) -> UIButton:
-        icon = parent.child_window(title_re=f".* {self.app.appName}", control_type="Button", found_index=0)
+        icon = parent.child_window(title_re=f".*{self.app.appName}", control_type="Button", class_name="SystemTray.NormalButton", found_index=0)
         icon.wait('exists', timeout=2)
         icon.wrapper_object()
         return UIButton(icon)
 
     def __openSystemTrayExpand(self) -> pywinauto.WindowSpecification:
         # Open the system tray
         backendExplorer.taskbarExpand.invoke()
```

### Comparing `pyuiauto-0.1.7/pyuiauto/win/components.py` & `pyuiauto-0.1.8/pyuiauto/win/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,13 +312,13 @@
 
 class UIProgressBar(UIProgressBarWrapper, UIBaseComponent):
     @classmethod
     @property
     def native_control_type(cls) -> str:
         return "ProgressBar"
 
-    def getValue(self):
-        return int(self.component.legacy_properties()['Value'])
+    def getValue(self) -> float:
+        return float(self.component.legacy_properties()['Value'])
 
 # !!! Mac Specific !!!
 
 class UIMenuBarItem(UIMenuItem, UIBaseComponent): ...
```

### Comparing `pyuiauto-0.1.7/README.md` & `pyuiauto-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -96,13 +96,19 @@
     - Added isOnTop method for components
     - Fixed isVisible method for components
     - Added checks for components existing in helper methods
   - 0.1.7
     - Added MacOS compatibility
     - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)
     - Fixed menu path select and system tray popup select methods on mac
+  - 0.1.8
+    - Fixed progress bar get value method
+    - Added better python intellisense for pylance
+    - Added further checks for system tray icon
+    - Updated application.py
+    - Upgraded package versions
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyuiauto-0.1.7/setup.py` & `pyuiauto-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\n\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n\nex. [atomacos](https://github.com/daveenguyen/atomacos)\n\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n  - 0.1.6\n    - Added isOnTop method for components\n    - Fixed isVisible method for components\n    - Added checks for components existing in helper methods\n  - 0.1.7\n    - Added MacOS compatibility\n    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)\n    - Fixed menu path select and system tray popup select methods on mac\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\n\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n\nex. [atomacos](https://github.com/daveenguyen/atomacos)\n\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n  - 0.1.6\n    - Added isOnTop method for components\n    - Fixed isVisible method for components\n    - Added checks for components existing in helper methods\n  - 0.1.7\n    - Added MacOS compatibility\n    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)\n    - Fixed menu path select and system tray popup select methods on mac\n  - 0.1.8\n    - Fixed progress bar get value method\n    - Added better python intellisense for pylance\n    - Added further checks for system tray icon\n    - Updated application.py\n    - Upgraded package versions\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyuiauto-0.1.7/PKG-INFO` & `pyuiauto-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -121,14 +121,20 @@
     - Added isOnTop method for components
     - Fixed isVisible method for components
     - Added checks for components existing in helper methods
   - 0.1.7
     - Added MacOS compatibility
     - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)
     - Fixed menu path select and system tray popup select methods on mac
+  - 0.1.8
+    - Fixed progress bar get value method
+    - Added better python intellisense for pylance
+    - Added further checks for system tray icon
+    - Updated application.py
+    - Upgraded package versions
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

