# Comparing `tmp/pywebgo-0.0.4.tar.gz` & `tmp/pywebgo-0.0.5.tar.gz`

## Comparing `pywebgo-0.0.4.tar` & `pywebgo-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,11 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/pywebgo.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pywebgo-0.0.4/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pywebgo-0.0.4/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    14906 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.5/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.5/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.5/PKG-INFO
```

### Comparing `pywebgo-0.0.4/src/pywebgo/controller.py` & `pywebgo-0.0.5/src/pywebgo/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .elements import ElementsHandler
 from selenium import webdriver
 from selenium.common import NoSuchElementException
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.remote.webelement import WebElement
+from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.common.action_chains import ActionChains
 
 
 class WebController(webdriver.Chrome):
     """
     Implements search, action execution and data retrieval successively for given element dictionaries.
 
@@ -22,15 +23,16 @@
     - :class:`list` urls --> non-linked web pages to traverse through
     - :class:`bool` teardown --> closes the browser after execution if true
     - :class:`float` wait --> time delay for executing each action
     - :class:`ElementsHandler` elem_handler --> instance of ElementsHandler class to manage elements
     - :class:`DataHandler` data_handler --> instance of DataHandler class to manage data associated with the elements
     """
 
-    def __init__(self, urls: list, teardown: bool = True, wait: float = 0, options: list = None):
+    def __init__(self, urls: list, teardown: bool = True, wait: float = 0,
+                 options: list = None, retry_attempts: int = 1):
         """
         Initialize a new instance of the WebController class.
 
         :param urls: non-linked web pages to traverse through
         :param teardown: closes the browser after execution if true
         :param wait: time delay for executing each action
         """
@@ -42,14 +44,15 @@
 
         super(WebController, self).__init__(chrome_options=chrome_options)
 
         # ---- Private Variables ----- #
         self.urls = urls
         self.wait = wait
         self.teardown = teardown
+        self.retry_attempts = retry_attempts
         self.elem_handler = ElementsHandler()
         self.data_handler = DataHandler()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Exit the runtime context related to this object.
 
@@ -132,14 +135,16 @@
                 element['custom'](self, element)
                 continue
             web_element = self.get_element(element, timeout)
             self.elem_handler.store_web_element(web_element)
             self.retrieve_data(web_element, element)
             self.execute_actions(web_element, element)
             self.load_next_page(index)
+            # Handle alert if appears after any action
+            self.handle_alert(element, web_element)
 
     def get_active_element(self, timeout):
         """
         Switch to and return the active web element object.
 
         :param timeout: time before throwing exception if the element is not found
         :return: active web element
@@ -160,30 +165,49 @@
         # If locator is active, get the active element
         if element['loc'] == 'active':
             return self.get_active_element(timeout)
 
         # Get element identifiers
         identifiers = utils.get_element_identifiers(element)
         strategy, locator, index = identifiers.values()
-        self.wait_for_element_load(element, timeout)
-        if index:
-            return self.find_elements(strategy, locator)[int(index)]
-        return self.find_element(strategy, locator)
+        retry_count = 0
+        while retry_count <= self.retry_attempts:
+            try:
+                self.wait_for_element_load(element, timeout)
+                if index:
+                    return self.find_elements(strategy, locator)[int(index)]
+                return self.find_element(strategy, locator)
+            except NoSuchElementException:
+                retry_count += 1
+                time.sleep(1)  # Wait for a second before retrying
+        raise NoSuchElementException(f"Element not found after {self.retry_attempts} attempts.")
 
     def get_page_html(self, url: str = None) -> str:
         """
         Retrieve and return the HTML of the current page or from a given url.
 
         :param url: URL of a web page
         :return: requested HTML of a web page
         """
         if url:
             self.load_page(url)
         return self.page_source
 
+    def handle_alert(self, element, web_element) -> None:
+        """
+        Handle any alert that may be present on the page.
+        """
+        try:
+            alert = self.switch_to.alert
+            alert.accept()
+            # Retry the last operation
+            self.execute_actions(web_element, element)
+        except NoAlertPresentException:
+            pass
+
     def load_page(self, url: str) -> None:
         """
         Load the web page from the given URL.
 
         :param url: URL of the web page to be loaded
         """
         self.get(url)
@@ -237,23 +261,22 @@
             'text': web_element.text,
             'tag': web_element.tag_name,
             'aria-role': web_element.aria_role,
             'id': web_element.id,
             'location': web_element.location,
             'accessible-name': web_element.accessible_name
         }
-        element_data = utils.match_label(retrieve, retrieve_options)
         attribute = re.search('^attr', element['retrieve'])
-
         if attribute:
-            self.get_element_attribute(element, web_element)
+            element_data = self.get_element_attribute(element, web_element)
+        else:
+            element_data = utils.match_label(retrieve, retrieve_options)
 
-        if element_data:
-            index = self.elem_handler.elements.index(element)
-            self.data_handler.add_data(index, element['retrieve'], element_data)
+        index = self.elem_handler.elements.index(element)
+        self.data_handler.add_data(index, element['retrieve'], element_data)
 
     @staticmethod
     def get_element_attribute(element: dict, web_element: WebElement) -> str:
         """
         Return the requested attribute value for a given element.
 
         :param element: a dictionary containing WebElement specifications
@@ -278,14 +301,17 @@
     def wait_for_action(element: dict) -> bool:
         """
         Wait (in seconds) before executing a particular action.
 
         :param element: dictionary containing element specifications
         :return: true if the action is delayed
         """
+        if 'wait' not in element:
+            return False
+
         if element['wait']:
             time.sleep(element['wait'])
             return True
 
     def wait_for_all_actions(self) -> None:
         """
         Wait (in seconds) for a certain period for all actions.
```

### Comparing `pywebgo-0.0.4/src/pywebgo/data.py` & `pywebgo-0.0.5/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.4/src/pywebgo/elements.py` & `pywebgo-0.0.5/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.4/src/pywebgo/utils.py` & `pywebgo-0.0.5/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.4/.gitignore` & `pywebgo-0.0.5/.gitignore`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
```

### Comparing `pywebgo-0.0.4/LICENSE` & `pywebgo-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Adil Zafar Khan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Adil Zafar Khan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pywebgo-0.0.4/pyproject.toml` & `pywebgo-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.4/PKG-INFO` & `pywebgo-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

