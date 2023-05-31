# Comparing `tmp/cpp-automation-utility-0.0.1.tar.gz` & `tmp/cpp-automation-utility-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpp-automation-utility-0.0.1.tar", last modified: Tue May 30 05:09:33 2023, max compression
+gzip compressed data, was "cpp-automation-utility-0.0.2.tar", last modified: Wed May 31 04:21:10 2023, max compression
```

## Comparing `cpp-automation-utility-0.0.1.tar` & `cpp-automation-utility-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.813555 cpp-automation-utility-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 05:09:33.812555 cpp-automation-utility-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.809555 cpp-automation-utility-0.0.1/cau/
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/cau_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.810555 cpp-automation-utility-0.0.1/cau/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 05:09:25.000000 cpp-automation-utility-0.0.1/cau/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4280 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.810555 cpp-automation-utility-0.0.1/cau/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)     9416 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/Clang.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/Git.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.811555 cpp-automation-utility-0.0.1/cau/wrappers/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 05:09:25.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Coverage.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Git.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 05:09:33.812555 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-30 05:09:33.000000 cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 05:09:33.813555 cpp-automation-utility-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1162 2023-05-30 05:09:24.000000 cpp-automation-utility-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.958018 cpp-automation-utility-0.0.2/cau/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/cau_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.958018 cpp-automation-utility-0.0.2/cau/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.959018 cpp-automation-utility-0.0.2/cau/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)     9416 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Clang.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Git.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.959018 cpp-automation-utility-0.0.2/cau/wrappers/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Git.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.960018 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/setup.py
```

### Comparing `cpp-automation-utility-0.0.1/LICENSE` & `cpp-automation-utility-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/PKG-INFO` & `cpp-automation-utility-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.1/README.md` & `cpp-automation-utility-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/cau_cli.py` & `cpp-automation-utility-0.0.2/cau/cau_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,28 @@
 
 sys.tracebacklimit = 1
 
 logger = logging.getLogger("CAU")
 
 restore_help = "Skip restoration of Conan sources"
 build_directory_help = "Build directory of project"
+build_type_help = "Build type (Debug|Release)"
+platform_help = "Build platform (linux|win64)"
+
+@cau_cli.command(help="Restores conan dependencies")
+@click.option("-b", "--build-directory", default="build", help=build_directory_help)
+@click.option("-t", "--build-type", default="Debug", help=build_type_help)
+@click.option("-p", "--platform", default="linux", help=platform_help)
+def restore(build_directory: str, build_type: str, platform: str):
+    """
+    Restores conan dependencies
+    """
+    conan = cau.Conan(build_directory=build_directory, build_type=build_type, platform=platform)
+    result = conan.restore()
+    sys.exit(result.returncode)
 
 @cau_cli.command(help="Runs clang-tidy to lint C++ source files.")
 @click.option("-s", "--skip-restore", is_flag=True, default=False, help=restore_help)
 @click.option("-b", "--build-directory", default="build", help=build_directory_help)
 @cau.timer
 def lint(skip_restore: bool, build_directory: str):
     """
@@ -38,20 +52,22 @@
     linter = cau.Tidy(touched_files=changes)
     result = linter.lint()
     sys.exit(0 if result else 1)
 
 @cau_cli.command(help="Build project via conan")
 @click.option("-s", "--skip-restore", is_flag=True, default=False, help=restore_help)
 @click.option("-b", "--build-directory", default="build", help=build_directory_help)
+@click.option("-t", "--build-type", default="Debug", help=build_type_help)
+@click.option("-p", "--platform", default="linux", help=platform_help)
 @cau.timer
-def build(skip_restore: bool, build_directory: str):
+def build(skip_restore: bool, build_directory: str, build_type: str, platform: str):
     """
     Build command build the project via conan
     """
-    conan = cau.Conan(build_directory=build_directory)
+    conan = cau.Conan(build_directory=build_directory, build_type=build_type, platform=platform)
     if not skip_restore:
         conan.restore()
     result = conan.build()
     sys.exit(result.returncode)
 
 @cau_cli.command(help="Cleans project build files")
 @click.option("-b", "--build-directory", default="build", help=build_directory_help)
```

### Comparing `cpp-automation-utility-0.0.1/cau/tests/conftest.py` & `cpp-automation-utility-0.0.2/cau/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     class MockConan:
 
         def __init__(self, *args, **kwargs) -> None:
             pass
 
         def restore(self):
             print("Restored Conan")
+            return MockProcess()
 
         def build(self):
             print("Build successful")
             return MockProcess()
 
         def clean_build(self):
             print("Cleaned out build directory")
```

### Comparing `cpp-automation-utility-0.0.1/cau/tests/test_cli.py` & `cpp-automation-utility-0.0.2/cau/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,35 @@
 """
 import pytest
 
 from click import testing as ctest
 
 from ..cau_cli import cau_cli
 
+@pytest.mark.usefixtures("mock_conan")
+class TestRestore():
+    """
+    Tests for restore command
+    """
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        """
+        Setup of test fixtures
+        """
+        self.runner = ctest.CliRunner()
+
+    def test_default_restore(self):
+        """
+        Asserts default restore correctly executes
+        """
+        result = self.runner.invoke(cau_cli, ["restore"])
+        assert result.exit_code == 0
+        assert "Restored Conan" in result.output
+
 @pytest.mark.usefixtures("mock_conan", "mock_git", "mock_tidy")
 class TestLint():
     """
     Tests for lint command
     """
 
     @pytest.fixture(autouse=True)
```

### Comparing `cpp-automation-utility-0.0.1/cau/timer.py` & `cpp-automation-utility-0.0.2/cau/timer.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/Clang.py` & `cpp-automation-utility-0.0.2/cau/wrappers/Clang.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/Conan.py` & `cpp-automation-utility-0.0.2/cau/wrappers/Conan.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/Git.py` & `cpp-automation-utility-0.0.2/cau/wrappers/Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/tests/conftest.py` & `cpp-automation-utility-0.0.2/cau/wrappers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Conan.py` & `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Conan.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Coverage.py` & `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Coverage.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Git.py` & `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cau/wrappers/tests/test_Tidy.py` & `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Tidy.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/PKG-INFO` & `cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.1/cpp_automation_utility.egg-info/SOURCES.txt` & `cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.1/setup.py` & `cpp-automation-utility-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = req.readlines()
 
 with open(pathlib.Path(__file__).parent/"README.md", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="cpp-automation-utility",
-    version=os.environ.get("CI_COMMIT_TAG", "0.0.1"),
+    version=os.environ.get("CI_COMMIT_TAG", "0.0.2"),
     author="AldridgeSoftwareDesigns",
     author_email="aldridge.robert.james@gmail.com",
     description="CLI utility to assist C++ in a devops environment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/aldridgesoftwaredesigns/cau",
     packages=setuptools.find_packages(),
```

