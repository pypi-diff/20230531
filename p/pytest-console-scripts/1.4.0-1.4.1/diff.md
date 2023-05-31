# Comparing `tmp/pytest-console-scripts-1.4.0.tar.gz` & `tmp/pytest-console-scripts-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-console-scripts-1.4.0.tar", last modified: Mon May 22 15:17:21 2023, max compression
+gzip compressed data, was "pytest-console-scripts-1.4.1.tar", last modified: Wed May 31 08:36:22 2023, max compression
```

## Comparing `pytest-console-scripts-1.4.0.tar` & `pytest-console-scripts-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.910737 pytest-console-scripts-1.4.0/
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.883577 pytest-console-scripts-1.4.0/.github/
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.891069 pytest-console-scripts-1.4.0/.github/workflows/
--rw-r--r--   0 kvas       (501) staff       (20)      735 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/.github/workflows/test.yml
--rw-r--r--   0 kvas       (501) staff       (20)      874 2019-01-11 19:15:43.000000 pytest-console-scripts-1.4.0/.gitignore
--rw-r--r--   0 kvas       (501) staff       (20)      417 2020-09-01 21:57:39.000000 pytest-console-scripts-1.4.0/CHANGELOG.md
--rw-r--r--   0 kvas       (501) staff       (20)     1082 2016-10-26 10:42:08.000000 pytest-console-scripts-1.4.0/LICENSE
--rw-r--r--   0 kvas       (501) staff       (20)       96 2020-11-19 19:53:12.000000 pytest-console-scripts-1.4.0/MANIFEST.in
--rw-r--r--   0 kvas       (501) staff       (20)    12052 2023-05-22 15:17:21.913662 pytest-console-scripts-1.4.0/PKG-INFO
--rw-r--r--   0 kvas       (501) staff       (20)     9056 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/README.md
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.892508 pytest-console-scripts-1.4.0/pytest_console_scripts/
--rw-r--r--   0 kvas       (501) staff       (20)    14470 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/pytest_console_scripts/__init__.py
--rw-r--r--   0 kvas       (501) staff       (20)        0 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/pytest_console_scripts/py.typed
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.896340 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/
--rw-r--r--   0 kvas       (501) staff       (20)    12052 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kvas       (501) staff       (20)      526 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kvas       (501) staff       (20)        1 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kvas       (501) staff       (20)       53 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/entry_points.txt
--rw-r--r--   0 kvas       (501) staff       (20)       66 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/requires.txt
--rw-r--r--   0 kvas       (501) staff       (20)       23 2023-05-22 15:17:21.000000 pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/top_level.txt
--rw-r--r--   0 kvas       (501) staff       (20)       63 2023-05-22 15:17:21.917099 pytest-console-scripts-1.4.0/setup.cfg
--rw-r--r--   0 kvas       (501) staff       (20)     1663 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/setup.py
-drwxr-xr-x   0 kvas       (501) staff       (20)        0 2023-05-22 15:17:21.906618 pytest-console-scripts-1.4.0/tests/
--rw-r--r--   0 kvas       (501) staff       (20)       28 2016-10-26 10:42:08.000000 pytest-console-scripts-1.4.0/tests/conftest.py
--rw-r--r--   0 kvas       (501) staff       (20)     3634 2023-05-15 20:16:04.000000 pytest-console-scripts-1.4.0/tests/test_console_scripts.py
--rw-r--r--   0 kvas       (501) staff       (20)    14149 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/tests/test_run_scripts.py
--rw-r--r--   0 kvas       (501) staff       (20)     1107 2023-05-22 15:06:38.000000 pytest-console-scripts-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.710072 pytest-console-scripts-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.702072 pytest-console-scripts-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.706072 pytest-console-scripts-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-31 08:36:22.710072 pytest-console-scripts-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.706072 pytest-console-scripts-1.4.1/pytest_console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/pytest_console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/pytest_console_scripts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.710072 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 08:36:22.000000 pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 08:36:22.710072 pytest-console-scripts-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:36:22.710072 pytest-console-scripts-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/tests/test_console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/tests/test_run_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 08:36:13.000000 pytest-console-scripts-1.4.1/tox.ini
```

### Comparing `pytest-console-scripts-1.4.0/.gitignore` & `pytest-console-scripts-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.4.0/LICENSE` & `pytest-console-scripts-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.4.0/PKG-INFO` & `pytest-console-scripts-1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,269 +1,279 @@
 Metadata-Version: 2.1
 Name: pytest-console-scripts
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pytest plugin for testing console scripts
 Home-page: https://github.com/kvas-it/pytest-console-scripts
 Author: Vasily Kuznetsov
 Author-email: kvas.it@gmail.com
-Maintainer: Vasily Kuznetsov
-Maintainer-email: kvas.it@gmail.com
+Maintainer: Vasily Kuznetsov, Kyle Benesch
+Maintainer-email: kvas.it@gmail.com, 4b796c65+github@gmail.com
 License: MIT
-Description: pytest-console-scripts
-        ======================
-        
-        Pytest-console-scripts is a [pytest][1] plugin for running python scripts from
-        within tests. It's quite similar to `subprocess.run()`, but it also has an
-        in-process mode, where the scripts are executed by the interpreter that's
-        running `pytest` (using some amount of sandboxing).
-        
-        In-process mode significantly reduces the run time of the test suites that
-        run many external scripts. This is speeds up development. In the CI environment
-        subprocess mode can be used to make sure the scripts also work (and behave the
-        same) when run by a fresh interpreter.
-        
-        Requirements
-        ------------
-        
-        - Python 3.7+, or PyPy3,
-        - Pytest 4.0 or newer.
-        
-        Installation
-        ------------
-        
-        You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
-        
-        ```sh
-        $ pip install pytest-console-scripts
-        ```
-        
-        Normally you would add it as a test dependency in `tox.ini` (see [tox
-        documentation][9]).
-        
-        Usage
-        -----
-        
-        This plugin will run scripts that are installed via `console_scripts` entry
-        point in `setup.py`, python files in current directory (or anywhere else, if
-        given the path), and Python scripts anywhere else in the path. It will also run
-        executables that are not Python scripts, but only in subprocess mode (there's
-        no benefit in using `pytest-console-scripts` for this, you should just use
-        `subprocess.run`).
-        
-        Here's an example with `console_scripts` entry point. Imagine we have a python
-        package `foo` with the following `setup.py`:
-        
-        ```py
-        setup(
-            name='foo',
-            version='0.0.1',
-            py_modules=['foo'],
-            entry_points={
-                'console_scripts': ['foobar=foo:bar']
-            },
-        )
-        ```
-        
-        We could use pytest-console-scripts to test the `foobar` script:
-        
-        ```py
-        def test_foo_bar(script_runner):
-            result = script_runner.run(['foobar', '--version'])
-            assert result.returncode == 0
-            assert result.stdout == '3.2.1\n'
-            assert result.stderr == ''
-        
-            script_runner.run('foobar --version', shell=True, check=True)
-        ```
-        
-        This would use the `script_runner` fixture provided by the plugin to
-        run the script and capture its output.
-        
-        The arguments of `script_runner.run` are the command name of the script and
-        any command line arguments that should be passed to it. Additionally the
-        following keyword arguments can be used:
-        
-        - `cwd` - set the working directory of the script under test.
-        - `env` - a dictionary with environment variables to use instead of the current
-          environment.
-        - `stdin` - a file-like object that will be piped to standard input of the
-          script.
-        - `check` - raises an exception if `returncode != 0`, defaults to False.
-        - `shell` - mimic shell execution, this should work well for simple cases,
-          defaults to False.
-        
-        Type-hinting is also supported.
-        You may type-hint the fixture with the following code:
-        
-        ```py
-        from pytest_console_scripts import ScriptRunner
-        
-        def test_foo_bar(script_runner: ScriptRunner) -> None:
-            ...
-        ```
-        
-        Configuring script execution mode
-        ---------------------------------
-        
-        In the example above the `foobar` script would run in in-process mode (which is
-        the default). This is fast and good for quick iteration during development.
-        After we're happy with the functionality, it's time to run the script in
-        subprocess mode to simulate real invocation more closely. There are several
-        ways to do this. We can configure it via pytest configuration (for example in
-        `tox.ini`):
-        
-        ```ini
-        [pytest]
-        script_launch_mode = subprocess
-        ```
-        
-        We can give a command line option to pytest (this will override the
-        configuration file):
-        
-        ```sh
-        $ pytest --script-launch-mode=subprocess test_foobar.py
-        ```
-        
-        We can also mark individual tests to run in a specific mode:
-        
-        ```py
-        @pytest.mark.script_launch_mode('subprocess')
-        def test_foobar(script_runner):
-            ...
-        ```
-        
-        Between these three methods the marking of the tests has priority before the
-        command line option that in turn overrides the configuration setting. All three
-        can take three possible values: "inprocess", "subprocess", and "both" (which
-        will cause the test to be run twice: in in-process and in subprocess modes).
-        
-        Interaction with mocking
-        ------------------------
-        
-        It is possible to mock objects and functions inside of console scripts when
-        they are run using `pytest-console-scripts` but only in inprocess mode. When
-        the script is run in subprocess mode, it is executed by a separate Python
-        interpreter and the test can't mock anything inside of it.
-        
-        Another limitation of mocking is that with simple Python scripts that are not
-        installed via [`console_scripts` entry point][14] mocking of objects inside of
-        the main script will not work. The reason for that is that when we run
-        `myscript.py` with `$ python myscript.py` the script gets imported into
-        `__main__` namespace instead of `myscript` namespace. Our patching of
-        `myscript.myfunction` will have no effect on what the code in `__main__`
-        namespace sees when it's calling `myfunction` defined in the same file.
-        
-        See [this stackoverflow answer](https://stackoverflow.com/a/66693954/1595738)
-        for some ideas of how to get around this.
-        
-        Suppressing the printing of script run results
-        ----------------------------------------------
-        
-        When tests involving `pytest-console-scripts` fail, it tends to be quite
-        useful to see the output of the scripts that were executed in them. We try
-        to be helpful and print it out just before returning the result from
-        `script_runner.run()`. Normally PyTest [captures][12] all the output during a
-        test run and it's not shown to the user unless some tests fail. This is exactly
-        what we want.
-        
-        However, in some cases it might be useful to disable the output capturing and
-        PyTest provides [ways to do it][13]. When capturing is disabled, all test run
-        results will be printed out and this might make it harder to inspect the other
-        output of the tests. To deal with this, `pytest-console-scripts` has an option
-        to disable the printing of script run results:
-        
-        ```sh
-        $ pytest --hide-run-results test_foobar.py
-        ```
-        
-        It's also possible to disable it just for one script run:
-        
-        ```py
-        result = script_runner.run('foobar', print_result=False)
-        ```
-        
-        When printing of script run results is disabled, script output won't be
-        visible even when the test fails. Unfortunately there's no automatic way to
-        print it only if the test fails because by the time a script run completes we
-        don't know whether the test will fail or not. It's possible to do it manually
-        from the test by using:
-        
-        ```py
-        result.print()
-        ```
-        
-        This, combined with `--hide-run-results` or `print_result=False` can be used to
-        only print interesting run results when capturing is off.
-        
-        Package installation and testing during development
-        ---------------------------------------------------
-        
-        Since `pytest-console-scripts` relies on the scripts being located in the path,
-        it can only run the console scripts from packages that have been installed (if
-        you are interested in working on removing this limitation, take a look at [this
-        ticket](https://github.com/kvas-it/pytest-console-scripts/issues/34) and in
-        particular [this comment](https://github.com/kvas-it/pytest-console-scripts/issues/34#issuecomment-649497564)).
-        If you want to run the tests quickly during development, the additional
-        installation step would add a significant overhead and slow you down.
-        
-        There's a way around this: install your package in [development mode][10] using
-        `python setup.py develop`. If you use [tox][9], you can take one of its
-        existing virtualenvs (they live in `.tox/`). Otherwise create a
-        [virtualenv][11] just for development, activate it and run `python setup.py
-        develop` to install your package in development mode. You will need to
-        re-install every time you add a new console script, but otherwise all the
-        changes to your code will be immediately picked up by the tests.
-        
-        Contributing
-        ------------
-        
-        Contributions are very welcome. Tests can be run with `tox`, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        License
-        -------
-        
-        Distributed under the terms of the [MIT][8] license, "pytest-console-scripts"
-        is free and open source software.
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please [file an issue][7] along with a detailed
-        description.
-        
-        ----
-        
-        Pytest-console-scripts was initially generated with [Cookiecutter][4] along
-        with [@hackebrot][5]'s [Cookiecutter-pytest-plugin][6] template.
-        
-        [1]: https://github.com/pytest-dev/pytest
-        [2]: https://pypi.python.org/pypi/pip/
-        [3]: https://pypi.python.org/pypi
-        [4]: https://github.com/audreyr/cookiecutter
-        [5]: https://github.com/hackebrot
-        [6]: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-        [7]: https://github.com/kvas-it/pytest-console-scripts/issues
-        [8]: http://opensource.org/licenses/MIT
-        [9]: https://tox.readthedocs.org/en/latest/
-        [10]: https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode
-        [11]: https://docs.python.org/3/library/venv.html
-        [12]: https://docs.pytest.org/en/stable/capture.html
-        [13]: https://docs.pytest.org/en/stable/capture.html#setting-capturing-methods-or-disabling-capturing
-        [14]: https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+pytest-console-scripts
+======================
+
+[![PyPI](https://img.shields.io/pypi/v/pytest-console-scripts)](https://pypi.org/project/pytest-console-scripts/)
+[![PyPI - License](https://img.shields.io/pypi/l/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/blob/master/LICENSE)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kvas-it/pytest-console-scripts/test.yml)](https://github.com/kvas-it/pytest-console-scripts/actions)
+[![codecov](https://codecov.io/gh/kvas-it/pytest-console-scripts/branch/master/graph/badge.svg?token=RfELxcqvpF)](https://codecov.io/gh/kvas-it/pytest-console-scripts)
+
+[![GitHub issues](https://img.shields.io/github/issues/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/pulls)
+[![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/kvas-it/pytest-console-scripts/latest)](https://github.com/kvas-it/pytest-console-scripts/blob/master/CHANGELOG.md)
+
+Pytest-console-scripts is a [pytest][1] plugin for running python scripts from
+within tests. It's quite similar to `subprocess.run()`, but it also has an
+in-process mode, where the scripts are executed by the interpreter that's
+running `pytest` (using some amount of sandboxing).
+
+In-process mode significantly reduces the run time of the test suites that
+run many external scripts. This is speeds up development. In the CI environment
+subprocess mode can be used to make sure the scripts also work (and behave the
+same) when run by a fresh interpreter.
+
+Requirements
+------------
+
+- Python 3.8+, or PyPy3,
+- Pytest 4.0 or newer.
+
+Installation
+------------
+
+You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
+
+```sh
+$ pip install pytest-console-scripts
+```
+
+Normally you would add it as a test dependency in `tox.ini` (see [tox
+documentation][9]).
+
+Usage
+-----
+
+This plugin will run scripts that are installed via `console_scripts` entry
+point in `setup.py`, python files in current directory (or anywhere else, if
+given the path), and Python scripts anywhere else in the path. It will also run
+executables that are not Python scripts, but only in subprocess mode (there's
+no benefit in using `pytest-console-scripts` for this, you should just use
+`subprocess.run`).
+
+Here's an example with `console_scripts` entry point. Imagine we have a python
+package `foo` with the following `setup.py`:
+
+```py
+setup(
+    name='foo',
+    version='0.0.1',
+    py_modules=['foo'],
+    entry_points={
+        'console_scripts': ['foobar=foo:bar']
+    },
+)
+```
+
+We could use pytest-console-scripts to test the `foobar` script:
+
+```py
+def test_foo_bar(script_runner):
+    result = script_runner.run(['foobar', '--version'])
+    assert result.returncode == 0
+    assert result.stdout == '3.2.1\n'
+    assert result.stderr == ''
+
+    script_runner.run('foobar --version', shell=True, check=True)
+```
+
+This would use the `script_runner` fixture provided by the plugin to
+run the script and capture its output.
+
+The arguments of `script_runner.run` are the command name of the script and
+any command line arguments that should be passed to it. Additionally the
+following keyword arguments can be used:
+
+- `cwd` - set the working directory of the script under test.
+- `env` - a dictionary with environment variables to use instead of the current
+  environment.
+- `stdin` - a file-like object that will be piped to standard input of the
+  script.
+- `check` - raises an exception if `returncode != 0`, defaults to False.
+- `shell` - mimic shell execution, this should work well for simple cases,
+  defaults to False.
+
+Type-hinting is also supported.
+You may type-hint the fixture with the following code:
+
+```py
+from pytest_console_scripts import ScriptRunner
+
+def test_foo_bar(script_runner: ScriptRunner) -> None:
+    ...
+```
+
+Configuring script execution mode
+---------------------------------
+
+In the example above the `foobar` script would run in in-process mode (which is
+the default). This is fast and good for quick iteration during development.
+After we're happy with the functionality, it's time to run the script in
+subprocess mode to simulate real invocation more closely. There are several
+ways to do this. We can configure it via pytest configuration (for example in
+`tox.ini`):
+
+```ini
+[pytest]
+script_launch_mode = subprocess
+```
+
+We can give a command line option to pytest (this will override the
+configuration file):
+
+```sh
+$ pytest --script-launch-mode=subprocess test_foobar.py
+```
+
+We can also mark individual tests to run in a specific mode:
+
+```py
+@pytest.mark.script_launch_mode('subprocess')
+def test_foobar(script_runner):
+    ...
+```
+
+Between these three methods the marking of the tests has priority before the
+command line option that in turn overrides the configuration setting. All three
+can take three possible values: "inprocess", "subprocess", and "both" (which
+will cause the test to be run twice: in in-process and in subprocess modes).
+
+Interaction with mocking
+------------------------
+
+It is possible to mock objects and functions inside of console scripts when
+they are run using `pytest-console-scripts` but only in inprocess mode. When
+the script is run in subprocess mode, it is executed by a separate Python
+interpreter and the test can't mock anything inside of it.
+
+Another limitation of mocking is that with simple Python scripts that are not
+installed via [`console_scripts` entry point][14] mocking of objects inside of
+the main script will not work. The reason for that is that when we run
+`myscript.py` with `$ python myscript.py` the script gets imported into
+`__main__` namespace instead of `myscript` namespace. Our patching of
+`myscript.myfunction` will have no effect on what the code in `__main__`
+namespace sees when it's calling `myfunction` defined in the same file.
+
+See [this stackoverflow answer](https://stackoverflow.com/a/66693954/1595738)
+for some ideas of how to get around this.
+
+Suppressing the printing of script run results
+----------------------------------------------
+
+When tests involving `pytest-console-scripts` fail, it tends to be quite
+useful to see the output of the scripts that were executed in them. We try
+to be helpful and print it out just before returning the result from
+`script_runner.run()`. Normally PyTest [captures][12] all the output during a
+test run and it's not shown to the user unless some tests fail. This is exactly
+what we want.
+
+However, in some cases it might be useful to disable the output capturing and
+PyTest provides [ways to do it][13]. When capturing is disabled, all test run
+results will be printed out and this might make it harder to inspect the other
+output of the tests. To deal with this, `pytest-console-scripts` has an option
+to disable the printing of script run results:
+
+```sh
+$ pytest --hide-run-results test_foobar.py
+```
+
+It's also possible to disable it just for one script run:
+
+```py
+result = script_runner.run('foobar', print_result=False)
+```
+
+When printing of script run results is disabled, script output won't be
+visible even when the test fails. Unfortunately there's no automatic way to
+print it only if the test fails because by the time a script run completes we
+don't know whether the test will fail or not. It's possible to do it manually
+from the test by using:
+
+```py
+result.print()
+```
+
+This, combined with `--hide-run-results` or `print_result=False` can be used to
+only print interesting run results when capturing is off.
+
+Package installation and testing during development
+---------------------------------------------------
+
+Since `pytest-console-scripts` relies on the scripts being located in the path,
+it can only run the console scripts from packages that have been installed (if
+you are interested in working on removing this limitation, take a look at [this
+ticket](https://github.com/kvas-it/pytest-console-scripts/issues/34) and in
+particular [this comment](https://github.com/kvas-it/pytest-console-scripts/issues/34#issuecomment-649497564)).
+If you want to run the tests quickly during development, the additional
+installation step would add a significant overhead and slow you down.
+
+There's a way around this: install your package in [development mode][10] using
+`pip install -e .`. If you use [tox][9], you can take one of its
+existing virtualenvs (they live in `.tox/`). Otherwise create a
+[virtualenv][11] just for development, activate it and run `python setup.py
+develop` to install your package in development mode. You will need to
+re-install every time you add a new console script, but otherwise all the
+changes to your code will be immediately picked up by the tests.
+
+Contributing
+------------
+
+Contributions are very welcome. Tests can be run with `tox`, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+License
+-------
+
+Distributed under the terms of the [MIT][8] license, "pytest-console-scripts"
+is free and open source software.
+
+Issues
+------
+
+If you encounter any problems, please [file an issue][7] along with a detailed
+description.
+
+----
+
+Pytest-console-scripts was initially generated with [Cookiecutter][4] along
+with [@hackebrot][5]'s [Cookiecutter-pytest-plugin][6] template.
+
+[1]: https://github.com/pytest-dev/pytest
+[2]: https://pypi.python.org/pypi/pip/
+[3]: https://pypi.python.org/pypi
+[4]: https://github.com/audreyr/cookiecutter
+[5]: https://github.com/hackebrot
+[6]: https://github.com/pytest-dev/cookiecutter-pytest-plugin
+[7]: https://github.com/kvas-it/pytest-console-scripts/issues
+[8]: http://opensource.org/licenses/MIT
+[9]: https://tox.readthedocs.org/en/latest/
+[10]: https://setuptools.pypa.io/en/latest/userguide/development_mode.html
+[11]: https://docs.python.org/3/library/venv.html
+[12]: https://docs.pytest.org/en/stable/capture.html
+[13]: https://docs.pytest.org/en/stable/capture.html#setting-capturing-methods-or-disabling-capturing
+[14]: https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
```

### Comparing `pytest-console-scripts-1.4.0/README.md` & `pytest-console-scripts-1.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 pytest-console-scripts
 ======================
 
+[![PyPI](https://img.shields.io/pypi/v/pytest-console-scripts)](https://pypi.org/project/pytest-console-scripts/)
+[![PyPI - License](https://img.shields.io/pypi/l/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/blob/master/LICENSE)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kvas-it/pytest-console-scripts/test.yml)](https://github.com/kvas-it/pytest-console-scripts/actions)
+[![codecov](https://codecov.io/gh/kvas-it/pytest-console-scripts/branch/master/graph/badge.svg?token=RfELxcqvpF)](https://codecov.io/gh/kvas-it/pytest-console-scripts)
+
+[![GitHub issues](https://img.shields.io/github/issues/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/pulls)
+[![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/kvas-it/pytest-console-scripts/latest)](https://github.com/kvas-it/pytest-console-scripts/blob/master/CHANGELOG.md)
+
 Pytest-console-scripts is a [pytest][1] plugin for running python scripts from
 within tests. It's quite similar to `subprocess.run()`, but it also has an
 in-process mode, where the scripts are executed by the interpreter that's
 running `pytest` (using some amount of sandboxing).
 
 In-process mode significantly reduces the run time of the test suites that
 run many external scripts. This is speeds up development. In the CI environment
 subprocess mode can be used to make sure the scripts also work (and behave the
 same) when run by a fresh interpreter.
 
 Requirements
 ------------
 
-- Python 3.7+, or PyPy3,
+- Python 3.8+, or PyPy3,
 - Pytest 4.0 or newer.
 
 Installation
 ------------
 
 You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
 
@@ -192,15 +201,15 @@
 you are interested in working on removing this limitation, take a look at [this
 ticket](https://github.com/kvas-it/pytest-console-scripts/issues/34) and in
 particular [this comment](https://github.com/kvas-it/pytest-console-scripts/issues/34#issuecomment-649497564)).
 If you want to run the tests quickly during development, the additional
 installation step would add a significant overhead and slow you down.
 
 There's a way around this: install your package in [development mode][10] using
-`python setup.py develop`. If you use [tox][9], you can take one of its
+`pip install -e .`. If you use [tox][9], you can take one of its
 existing virtualenvs (they live in `.tox/`). Otherwise create a
 [virtualenv][11] just for development, activate it and run `python setup.py
 develop` to install your package in development mode. You will need to
 re-install every time you add a new console script, but otherwise all the
 changes to your code will be immediately picked up by the tests.
 
 Contributing
@@ -231,12 +240,12 @@
 [3]: https://pypi.python.org/pypi
 [4]: https://github.com/audreyr/cookiecutter
 [5]: https://github.com/hackebrot
 [6]: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 [7]: https://github.com/kvas-it/pytest-console-scripts/issues
 [8]: http://opensource.org/licenses/MIT
 [9]: https://tox.readthedocs.org/en/latest/
-[10]: https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode
+[10]: https://setuptools.pypa.io/en/latest/userguide/development_mode.html
 [11]: https://docs.python.org/3/library/venv.html
 [12]: https://docs.pytest.org/en/stable/capture.html
 [13]: https://docs.pytest.org/en/stable/capture.html#setting-capturing-methods-or-disabling-capturing
 [14]: https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
```

### Comparing `pytest-console-scripts-1.4.0/pytest_console_scripts/__init__.py` & `pytest-console-scripts-1.4.1/pytest_console_scripts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,35 +133,39 @@
         print('# Script stderr:', self.stderr, sep='\n')
 
 
 def _handle_command_args(
     command: _Command,
     *args: _StrOrPath,
     shell: bool = False,
+    stacklevel: int = 1,
 ) -> Sequence[_StrOrPath]:
     """Return command arguments in a consistent list format.
 
     If shell=True then this function tries to mimic local shell execution.
     """
     if shell:
         if args or not isinstance(command, (str, os.PathLike)):
             command = subprocess.list2cmdline(
                 str(arg)
-                for arg in _handle_command_args(command, *args, shell=False)
+                for arg in _handle_command_args(
+                    command, *args, shell=False, stacklevel=stacklevel + 1
+                )
             )
         command = shlex.split(str(command), posix=os.name == 'posix')
         args = ()
 
     if args:
         warnings.warn(
             'script_runner commands should be passed as a single sequence,'
             ' not as multiple arguments.'
             '\nReplace `script_runner.run(a, b, c)` calls with'
             ' `script_runner.run([a, b, c])`',
             DeprecationWarning,
+            stacklevel=stacklevel + 1,
         )
         if not isinstance(command, (str, os.PathLike)):
             return [*command, *args]
         return [command, *args]
     if isinstance(command, (str, os.PathLike)):
         return [command]
     return command
@@ -259,14 +263,15 @@
             *arguments,
             print_result=print_result,
             shell=shell,
             cwd=cwd,
             env=env,
             stdin=stdin,
             check=check,
+            _stacklevel=2,
             **options,
         )
 
     @staticmethod
     def _locate_script(
         command: _StrOrPath,
         *,
@@ -304,17 +309,18 @@
                     s: Callable[[], int | None] = entry_points[0].load()
                     return s()
                 return console_script
 
         script_path = cls._locate_script(command, cwd=cwd, env=env)
 
         def exec_script() -> int:
-            with open(script_path, 'rt', encoding='utf-8') as script:
-                compiled = compile(script.read(), str(script), 'exec', flags=0)
-                exec(compiled, {'__name__': '__main__'})
+            compiled = compile(
+                script_path.read_bytes(), str(script_path), 'exec', flags=0
+            )
+            exec(compiled, {'__name__': '__main__'})
             return 0
 
         return exec_script
 
     @classmethod
     def run_inprocess(
         cls,
@@ -322,22 +328,26 @@
         *arguments: _StrOrPath,
         shell: bool = False,
         cwd: _StrOrPath | None = None,
         env: dict[str, str] | None = None,
         print_result: bool = True,
         stdin: io.IOBase | None = None,
         check: bool = False,
+        _stacklevel: int = 1,
         **options: Any,
     ) -> RunResult:
         for key in options:
             warnings.warn(
                 f'Keyword argument {key!r} was ignored.'
-                '\nConsider using subprocess mode or raising an issue.'
+                '\nConsider using subprocess mode or raising an issue.',
+                stacklevel=_stacklevel + 1,
             )
-        cmd_args = _handle_command_args(command, *arguments, shell=shell)
+        cmd_args = _handle_command_args(
+            command, *arguments, shell=shell, stacklevel=_stacklevel + 1
+        )
         script = cls._load_script(cmd_args[0], cwd=cwd, env=env)
         cmd_args = [str(cmd) for cmd in cmd_args]
         stdin_stream = stdin if stdin is not None else StreamMock()
         stdout_stream = StreamMock()
         stderr_stream = StreamMock()
         with contextlib.ExitStack() as stack:
             stack.enter_context(mock.patch('sys.stdin', new=stdin_stream))
@@ -392,51 +402,55 @@
         print_result: bool = True,
         shell: bool = False,
         cwd: _StrOrPath | None = None,
         env: dict[str, str] | None = None,
         stdin: io.IOBase | None = None,
         check: bool = False,
         universal_newlines: bool = True,
+        _stacklevel: int = 1,
         **options: Any,
     ) -> RunResult:
         stdin_input: str | bytes | None = None
         if stdin is not None:
             stdin_input = stdin.read()
 
-        script_path = cls._locate_script(_handle_command_args(
-            command, *arguments, shell=shell)[0], cwd=cwd, env=env
+        script_path = cls._locate_script(
+            _handle_command_args(
+                command, *arguments, shell=shell, stacklevel=_stacklevel + 1
+            )[0],
+            cwd=cwd,
+            env=env,
         )
         if arguments:
-            command = _handle_command_args(command, *arguments, shell=shell)
+            command = _handle_command_args(
+                command, *arguments, shell=shell, stacklevel=_stacklevel + 1
+            )
 
         if _is_nonexecutable_python_file(script_path):
-            command = _handle_command_args(command, shell=shell)
+            command = _handle_command_args(
+                command, shell=shell, stacklevel=_stacklevel + 1
+            )
             command = [sys.executable or 'python', *command]
 
-        if sys.version_info < (3, 8):
-            if isinstance(command, os.PathLike):
-                command = [command]
-            if not isinstance(command, str):
-                command = [
-                    str(Path(arg)) if isinstance(arg, os.PathLike) else arg
-                    for arg in command
-                ]
-
-        cp = subprocess.run(
-            command,
-            input=stdin_input,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            shell=shell,
-            cwd=cwd,
-            env=env,
-            check=check,
-            universal_newlines=universal_newlines,
-            **options,
-        )
+        try:
+            cp = subprocess.run(
+                command,
+                input=stdin_input,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                shell=shell,
+                cwd=cwd,
+                env=env,
+                check=check,
+                universal_newlines=universal_newlines,
+                **options,
+            )
+        except subprocess.CalledProcessError as exc:
+            RunResult(exc.returncode, exc.stdout, exc.stderr, print_result)
+            raise
         return RunResult(cp.returncode, cp.stdout, cp.stderr, print_result)
 
 
 @pytest.fixture
 def script_launch_mode(request: pytest.FixtureRequest) -> str:
     return str(request.param)
```

### Comparing `pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/PKG-INFO` & `pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,269 +1,279 @@
 Metadata-Version: 2.1
 Name: pytest-console-scripts
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pytest plugin for testing console scripts
 Home-page: https://github.com/kvas-it/pytest-console-scripts
 Author: Vasily Kuznetsov
 Author-email: kvas.it@gmail.com
-Maintainer: Vasily Kuznetsov
-Maintainer-email: kvas.it@gmail.com
+Maintainer: Vasily Kuznetsov, Kyle Benesch
+Maintainer-email: kvas.it@gmail.com, 4b796c65+github@gmail.com
 License: MIT
-Description: pytest-console-scripts
-        ======================
-        
-        Pytest-console-scripts is a [pytest][1] plugin for running python scripts from
-        within tests. It's quite similar to `subprocess.run()`, but it also has an
-        in-process mode, where the scripts are executed by the interpreter that's
-        running `pytest` (using some amount of sandboxing).
-        
-        In-process mode significantly reduces the run time of the test suites that
-        run many external scripts. This is speeds up development. In the CI environment
-        subprocess mode can be used to make sure the scripts also work (and behave the
-        same) when run by a fresh interpreter.
-        
-        Requirements
-        ------------
-        
-        - Python 3.7+, or PyPy3,
-        - Pytest 4.0 or newer.
-        
-        Installation
-        ------------
-        
-        You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
-        
-        ```sh
-        $ pip install pytest-console-scripts
-        ```
-        
-        Normally you would add it as a test dependency in `tox.ini` (see [tox
-        documentation][9]).
-        
-        Usage
-        -----
-        
-        This plugin will run scripts that are installed via `console_scripts` entry
-        point in `setup.py`, python files in current directory (or anywhere else, if
-        given the path), and Python scripts anywhere else in the path. It will also run
-        executables that are not Python scripts, but only in subprocess mode (there's
-        no benefit in using `pytest-console-scripts` for this, you should just use
-        `subprocess.run`).
-        
-        Here's an example with `console_scripts` entry point. Imagine we have a python
-        package `foo` with the following `setup.py`:
-        
-        ```py
-        setup(
-            name='foo',
-            version='0.0.1',
-            py_modules=['foo'],
-            entry_points={
-                'console_scripts': ['foobar=foo:bar']
-            },
-        )
-        ```
-        
-        We could use pytest-console-scripts to test the `foobar` script:
-        
-        ```py
-        def test_foo_bar(script_runner):
-            result = script_runner.run(['foobar', '--version'])
-            assert result.returncode == 0
-            assert result.stdout == '3.2.1\n'
-            assert result.stderr == ''
-        
-            script_runner.run('foobar --version', shell=True, check=True)
-        ```
-        
-        This would use the `script_runner` fixture provided by the plugin to
-        run the script and capture its output.
-        
-        The arguments of `script_runner.run` are the command name of the script and
-        any command line arguments that should be passed to it. Additionally the
-        following keyword arguments can be used:
-        
-        - `cwd` - set the working directory of the script under test.
-        - `env` - a dictionary with environment variables to use instead of the current
-          environment.
-        - `stdin` - a file-like object that will be piped to standard input of the
-          script.
-        - `check` - raises an exception if `returncode != 0`, defaults to False.
-        - `shell` - mimic shell execution, this should work well for simple cases,
-          defaults to False.
-        
-        Type-hinting is also supported.
-        You may type-hint the fixture with the following code:
-        
-        ```py
-        from pytest_console_scripts import ScriptRunner
-        
-        def test_foo_bar(script_runner: ScriptRunner) -> None:
-            ...
-        ```
-        
-        Configuring script execution mode
-        ---------------------------------
-        
-        In the example above the `foobar` script would run in in-process mode (which is
-        the default). This is fast and good for quick iteration during development.
-        After we're happy with the functionality, it's time to run the script in
-        subprocess mode to simulate real invocation more closely. There are several
-        ways to do this. We can configure it via pytest configuration (for example in
-        `tox.ini`):
-        
-        ```ini
-        [pytest]
-        script_launch_mode = subprocess
-        ```
-        
-        We can give a command line option to pytest (this will override the
-        configuration file):
-        
-        ```sh
-        $ pytest --script-launch-mode=subprocess test_foobar.py
-        ```
-        
-        We can also mark individual tests to run in a specific mode:
-        
-        ```py
-        @pytest.mark.script_launch_mode('subprocess')
-        def test_foobar(script_runner):
-            ...
-        ```
-        
-        Between these three methods the marking of the tests has priority before the
-        command line option that in turn overrides the configuration setting. All three
-        can take three possible values: "inprocess", "subprocess", and "both" (which
-        will cause the test to be run twice: in in-process and in subprocess modes).
-        
-        Interaction with mocking
-        ------------------------
-        
-        It is possible to mock objects and functions inside of console scripts when
-        they are run using `pytest-console-scripts` but only in inprocess mode. When
-        the script is run in subprocess mode, it is executed by a separate Python
-        interpreter and the test can't mock anything inside of it.
-        
-        Another limitation of mocking is that with simple Python scripts that are not
-        installed via [`console_scripts` entry point][14] mocking of objects inside of
-        the main script will not work. The reason for that is that when we run
-        `myscript.py` with `$ python myscript.py` the script gets imported into
-        `__main__` namespace instead of `myscript` namespace. Our patching of
-        `myscript.myfunction` will have no effect on what the code in `__main__`
-        namespace sees when it's calling `myfunction` defined in the same file.
-        
-        See [this stackoverflow answer](https://stackoverflow.com/a/66693954/1595738)
-        for some ideas of how to get around this.
-        
-        Suppressing the printing of script run results
-        ----------------------------------------------
-        
-        When tests involving `pytest-console-scripts` fail, it tends to be quite
-        useful to see the output of the scripts that were executed in them. We try
-        to be helpful and print it out just before returning the result from
-        `script_runner.run()`. Normally PyTest [captures][12] all the output during a
-        test run and it's not shown to the user unless some tests fail. This is exactly
-        what we want.
-        
-        However, in some cases it might be useful to disable the output capturing and
-        PyTest provides [ways to do it][13]. When capturing is disabled, all test run
-        results will be printed out and this might make it harder to inspect the other
-        output of the tests. To deal with this, `pytest-console-scripts` has an option
-        to disable the printing of script run results:
-        
-        ```sh
-        $ pytest --hide-run-results test_foobar.py
-        ```
-        
-        It's also possible to disable it just for one script run:
-        
-        ```py
-        result = script_runner.run('foobar', print_result=False)
-        ```
-        
-        When printing of script run results is disabled, script output won't be
-        visible even when the test fails. Unfortunately there's no automatic way to
-        print it only if the test fails because by the time a script run completes we
-        don't know whether the test will fail or not. It's possible to do it manually
-        from the test by using:
-        
-        ```py
-        result.print()
-        ```
-        
-        This, combined with `--hide-run-results` or `print_result=False` can be used to
-        only print interesting run results when capturing is off.
-        
-        Package installation and testing during development
-        ---------------------------------------------------
-        
-        Since `pytest-console-scripts` relies on the scripts being located in the path,
-        it can only run the console scripts from packages that have been installed (if
-        you are interested in working on removing this limitation, take a look at [this
-        ticket](https://github.com/kvas-it/pytest-console-scripts/issues/34) and in
-        particular [this comment](https://github.com/kvas-it/pytest-console-scripts/issues/34#issuecomment-649497564)).
-        If you want to run the tests quickly during development, the additional
-        installation step would add a significant overhead and slow you down.
-        
-        There's a way around this: install your package in [development mode][10] using
-        `python setup.py develop`. If you use [tox][9], you can take one of its
-        existing virtualenvs (they live in `.tox/`). Otherwise create a
-        [virtualenv][11] just for development, activate it and run `python setup.py
-        develop` to install your package in development mode. You will need to
-        re-install every time you add a new console script, but otherwise all the
-        changes to your code will be immediately picked up by the tests.
-        
-        Contributing
-        ------------
-        
-        Contributions are very welcome. Tests can be run with `tox`, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        License
-        -------
-        
-        Distributed under the terms of the [MIT][8] license, "pytest-console-scripts"
-        is free and open source software.
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please [file an issue][7] along with a detailed
-        description.
-        
-        ----
-        
-        Pytest-console-scripts was initially generated with [Cookiecutter][4] along
-        with [@hackebrot][5]'s [Cookiecutter-pytest-plugin][6] template.
-        
-        [1]: https://github.com/pytest-dev/pytest
-        [2]: https://pypi.python.org/pypi/pip/
-        [3]: https://pypi.python.org/pypi
-        [4]: https://github.com/audreyr/cookiecutter
-        [5]: https://github.com/hackebrot
-        [6]: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-        [7]: https://github.com/kvas-it/pytest-console-scripts/issues
-        [8]: http://opensource.org/licenses/MIT
-        [9]: https://tox.readthedocs.org/en/latest/
-        [10]: https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode
-        [11]: https://docs.python.org/3/library/venv.html
-        [12]: https://docs.pytest.org/en/stable/capture.html
-        [13]: https://docs.pytest.org/en/stable/capture.html#setting-capturing-methods-or-disabling-capturing
-        [14]: https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+pytest-console-scripts
+======================
+
+[![PyPI](https://img.shields.io/pypi/v/pytest-console-scripts)](https://pypi.org/project/pytest-console-scripts/)
+[![PyPI - License](https://img.shields.io/pypi/l/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/blob/master/LICENSE)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kvas-it/pytest-console-scripts/test.yml)](https://github.com/kvas-it/pytest-console-scripts/actions)
+[![codecov](https://codecov.io/gh/kvas-it/pytest-console-scripts/branch/master/graph/badge.svg?token=RfELxcqvpF)](https://codecov.io/gh/kvas-it/pytest-console-scripts)
+
+[![GitHub issues](https://img.shields.io/github/issues/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/kvas-it/pytest-console-scripts)](https://github.com/kvas-it/pytest-console-scripts/pulls)
+[![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/kvas-it/pytest-console-scripts/latest)](https://github.com/kvas-it/pytest-console-scripts/blob/master/CHANGELOG.md)
+
+Pytest-console-scripts is a [pytest][1] plugin for running python scripts from
+within tests. It's quite similar to `subprocess.run()`, but it also has an
+in-process mode, where the scripts are executed by the interpreter that's
+running `pytest` (using some amount of sandboxing).
+
+In-process mode significantly reduces the run time of the test suites that
+run many external scripts. This is speeds up development. In the CI environment
+subprocess mode can be used to make sure the scripts also work (and behave the
+same) when run by a fresh interpreter.
+
+Requirements
+------------
+
+- Python 3.8+, or PyPy3,
+- Pytest 4.0 or newer.
+
+Installation
+------------
+
+You can install "pytest-console-scripts" via [pip][2] from [PyPI][3]:
+
+```sh
+$ pip install pytest-console-scripts
+```
+
+Normally you would add it as a test dependency in `tox.ini` (see [tox
+documentation][9]).
+
+Usage
+-----
+
+This plugin will run scripts that are installed via `console_scripts` entry
+point in `setup.py`, python files in current directory (or anywhere else, if
+given the path), and Python scripts anywhere else in the path. It will also run
+executables that are not Python scripts, but only in subprocess mode (there's
+no benefit in using `pytest-console-scripts` for this, you should just use
+`subprocess.run`).
+
+Here's an example with `console_scripts` entry point. Imagine we have a python
+package `foo` with the following `setup.py`:
+
+```py
+setup(
+    name='foo',
+    version='0.0.1',
+    py_modules=['foo'],
+    entry_points={
+        'console_scripts': ['foobar=foo:bar']
+    },
+)
+```
+
+We could use pytest-console-scripts to test the `foobar` script:
+
+```py
+def test_foo_bar(script_runner):
+    result = script_runner.run(['foobar', '--version'])
+    assert result.returncode == 0
+    assert result.stdout == '3.2.1\n'
+    assert result.stderr == ''
+
+    script_runner.run('foobar --version', shell=True, check=True)
+```
+
+This would use the `script_runner` fixture provided by the plugin to
+run the script and capture its output.
+
+The arguments of `script_runner.run` are the command name of the script and
+any command line arguments that should be passed to it. Additionally the
+following keyword arguments can be used:
+
+- `cwd` - set the working directory of the script under test.
+- `env` - a dictionary with environment variables to use instead of the current
+  environment.
+- `stdin` - a file-like object that will be piped to standard input of the
+  script.
+- `check` - raises an exception if `returncode != 0`, defaults to False.
+- `shell` - mimic shell execution, this should work well for simple cases,
+  defaults to False.
+
+Type-hinting is also supported.
+You may type-hint the fixture with the following code:
+
+```py
+from pytest_console_scripts import ScriptRunner
+
+def test_foo_bar(script_runner: ScriptRunner) -> None:
+    ...
+```
+
+Configuring script execution mode
+---------------------------------
+
+In the example above the `foobar` script would run in in-process mode (which is
+the default). This is fast and good for quick iteration during development.
+After we're happy with the functionality, it's time to run the script in
+subprocess mode to simulate real invocation more closely. There are several
+ways to do this. We can configure it via pytest configuration (for example in
+`tox.ini`):
+
+```ini
+[pytest]
+script_launch_mode = subprocess
+```
+
+We can give a command line option to pytest (this will override the
+configuration file):
+
+```sh
+$ pytest --script-launch-mode=subprocess test_foobar.py
+```
+
+We can also mark individual tests to run in a specific mode:
+
+```py
+@pytest.mark.script_launch_mode('subprocess')
+def test_foobar(script_runner):
+    ...
+```
+
+Between these three methods the marking of the tests has priority before the
+command line option that in turn overrides the configuration setting. All three
+can take three possible values: "inprocess", "subprocess", and "both" (which
+will cause the test to be run twice: in in-process and in subprocess modes).
+
+Interaction with mocking
+------------------------
+
+It is possible to mock objects and functions inside of console scripts when
+they are run using `pytest-console-scripts` but only in inprocess mode. When
+the script is run in subprocess mode, it is executed by a separate Python
+interpreter and the test can't mock anything inside of it.
+
+Another limitation of mocking is that with simple Python scripts that are not
+installed via [`console_scripts` entry point][14] mocking of objects inside of
+the main script will not work. The reason for that is that when we run
+`myscript.py` with `$ python myscript.py` the script gets imported into
+`__main__` namespace instead of `myscript` namespace. Our patching of
+`myscript.myfunction` will have no effect on what the code in `__main__`
+namespace sees when it's calling `myfunction` defined in the same file.
+
+See [this stackoverflow answer](https://stackoverflow.com/a/66693954/1595738)
+for some ideas of how to get around this.
+
+Suppressing the printing of script run results
+----------------------------------------------
+
+When tests involving `pytest-console-scripts` fail, it tends to be quite
+useful to see the output of the scripts that were executed in them. We try
+to be helpful and print it out just before returning the result from
+`script_runner.run()`. Normally PyTest [captures][12] all the output during a
+test run and it's not shown to the user unless some tests fail. This is exactly
+what we want.
+
+However, in some cases it might be useful to disable the output capturing and
+PyTest provides [ways to do it][13]. When capturing is disabled, all test run
+results will be printed out and this might make it harder to inspect the other
+output of the tests. To deal with this, `pytest-console-scripts` has an option
+to disable the printing of script run results:
+
+```sh
+$ pytest --hide-run-results test_foobar.py
+```
+
+It's also possible to disable it just for one script run:
+
+```py
+result = script_runner.run('foobar', print_result=False)
+```
+
+When printing of script run results is disabled, script output won't be
+visible even when the test fails. Unfortunately there's no automatic way to
+print it only if the test fails because by the time a script run completes we
+don't know whether the test will fail or not. It's possible to do it manually
+from the test by using:
+
+```py
+result.print()
+```
+
+This, combined with `--hide-run-results` or `print_result=False` can be used to
+only print interesting run results when capturing is off.
+
+Package installation and testing during development
+---------------------------------------------------
+
+Since `pytest-console-scripts` relies on the scripts being located in the path,
+it can only run the console scripts from packages that have been installed (if
+you are interested in working on removing this limitation, take a look at [this
+ticket](https://github.com/kvas-it/pytest-console-scripts/issues/34) and in
+particular [this comment](https://github.com/kvas-it/pytest-console-scripts/issues/34#issuecomment-649497564)).
+If you want to run the tests quickly during development, the additional
+installation step would add a significant overhead and slow you down.
+
+There's a way around this: install your package in [development mode][10] using
+`pip install -e .`. If you use [tox][9], you can take one of its
+existing virtualenvs (they live in `.tox/`). Otherwise create a
+[virtualenv][11] just for development, activate it and run `python setup.py
+develop` to install your package in development mode. You will need to
+re-install every time you add a new console script, but otherwise all the
+changes to your code will be immediately picked up by the tests.
+
+Contributing
+------------
+
+Contributions are very welcome. Tests can be run with `tox`, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+License
+-------
+
+Distributed under the terms of the [MIT][8] license, "pytest-console-scripts"
+is free and open source software.
+
+Issues
+------
+
+If you encounter any problems, please [file an issue][7] along with a detailed
+description.
+
+----
+
+Pytest-console-scripts was initially generated with [Cookiecutter][4] along
+with [@hackebrot][5]'s [Cookiecutter-pytest-plugin][6] template.
+
+[1]: https://github.com/pytest-dev/pytest
+[2]: https://pypi.python.org/pypi/pip/
+[3]: https://pypi.python.org/pypi
+[4]: https://github.com/audreyr/cookiecutter
+[5]: https://github.com/hackebrot
+[6]: https://github.com/pytest-dev/cookiecutter-pytest-plugin
+[7]: https://github.com/kvas-it/pytest-console-scripts/issues
+[8]: http://opensource.org/licenses/MIT
+[9]: https://tox.readthedocs.org/en/latest/
+[10]: https://setuptools.pypa.io/en/latest/userguide/development_mode.html
+[11]: https://docs.python.org/3/library/venv.html
+[12]: https://docs.pytest.org/en/stable/capture.html
+[13]: https://docs.pytest.org/en/stable/capture.html#setting-capturing-methods-or-disabling-capturing
+[14]: https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
```

### Comparing `pytest-console-scripts-1.4.0/pytest_console_scripts.egg-info/SOURCES.txt` & `pytest-console-scripts-1.4.1/pytest_console_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.4.0/setup.py` & `pytest-console-scripts-1.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,40 @@
 
 
 setup(
     name='pytest-console-scripts',
     use_scm_version=True,
     author='Vasily Kuznetsov',
     author_email='kvas.it@gmail.com',
-    maintainer='Vasily Kuznetsov',
-    maintainer_email='kvas.it@gmail.com',
+    maintainer='Vasily Kuznetsov, Kyle Benesch',
+    maintainer_email='kvas.it@gmail.com, 4b796c65+github@gmail.com',
     license='MIT',
     url='https://github.com/kvas-it/pytest-console-scripts',
     description='Pytest plugin for testing console scripts',
     long_description=README_TEXT,
     long_description_content_type='text/markdown',
     packages=['pytest_console_scripts'],
     package_data={'pytest_console_scripts': ['py.typed']},
     install_requires=[
         'pytest >=4.0.0',
         "importlib_metadata >=3.6; python_version < '3.10'",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     setup_requires=['setuptools-scm'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
     ],
     entry_points={
         'pytest11': [
```

### Comparing `pytest-console-scripts-1.4.0/tests/test_console_scripts.py` & `pytest-console-scripts-1.4.1/tests/test_console_scripts.py`

 * *Files identical despite different names*

### Comparing `pytest-console-scripts-1.4.0/tests/test_run_scripts.py` & `pytest-console-scripts-1.4.1/tests/test_run_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Test running of scripts with various modes and options."""
 from __future__ import annotations
 
+import contextlib
 import importlib
 import io
 import os
 import sys
 from pathlib import Path
 from subprocess import CalledProcessError
 from types import ModuleType
-from typing import Any
+from typing import Any, ContextManager
 from unittest import mock
 
 import pytest
 
 from pytest_console_scripts import ScriptRunner
 
 
@@ -88,17 +89,15 @@
     #   option to pytest and will check that the execution of the inner script
     #   is performed in accordance with its value.
     #
     # We're also testing all 4 combinations of inprocess/subprocess modes for
     # inner and outer script runners.
 
     result = script_runner.run(
-        'pytest',
-        str(test),
-        '--script-launch-mode=' + launch_mode,
+        ['pytest', test, f'--script-launch-mode={launch_mode}']
     )
     assert result.success
 
 
 @pytest.mark.script_launch_mode('inprocess')
 def test_return_None(
     console_script: Path, script_runner: ScriptRunner
@@ -226,39 +225,46 @@
     )
     result = script_runner.run(str(console_script))
     assert result.success
     assert result.stderr == 'INFO:root:shown\n'
 
 
 @pytest.mark.parametrize('fail', [True, False])
+@pytest.mark.parametrize('check', [True, False])
 def test_print_stdio_on_error(
     console_script: Path,
     script_runner: ScriptRunner,
     tmp_path: Path,
     fail: bool,
+    check: bool,
     launch_mode: str,
 ) -> None:
     """Output of the script is printed when the test fails."""
     console_script.write_text('print("12345")\nraise Exception("54321")')
-    test = tmp_path / f'test_{fail}_{launch_mode}.py'
+    test = tmp_path / f'test_{fail}_{check}_{launch_mode}.py'
+    command = [str(console_script), 'arg']
     test.write_text(
         f"""
+import subprocess
+
 def test_fail(script_runner):
-    ret = script_runner.run(R'''{console_script}''', 'arg')
-    assert ret.success is {fail}
+    try:
+        ret = script_runner.run({command}, check={check})
+    except subprocess.CalledProcessError as exc:
+        assert (exc.returncode == 0) is {fail}
+    else:
+        assert ret.success is {fail}
         """
     )
     result = script_runner.run(
-        'pytest',
-        str(test),
-        '--script-launch-mode=' + launch_mode,
+        ['pytest', test, f'--script-launch-mode={launch_mode}']
     )
     assert result.success != fail
     if fail:
-        assert (f'# Running console script: {console_script} arg\n'
+        assert (f'# Running console script: {command}\n'
                 in result.stdout)
         assert '# Script return code: 1\n' in result.stdout
         assert '# Script stdout:\n12345\n' in result.stdout
         assert '# Script stderr:\nTraceback' in result.stdout
         assert 'Exception: 54321' in result.stdout
     else:
         assert '# Running console script' not in result.stdout
@@ -302,15 +308,15 @@
 import pytest
 
 @pytest.mark.script_launch_mode('both')
 def test_script(script_runner):
     script_runner.run(R'''{console_script}''', print_result=False)
         """
     )
-    result = script_runner.run('pytest', '-s', str(test))
+    result = script_runner.run(['pytest', '-s', test])
     assert result.success
     assert 'the answer is 42' not in result.stdout
     assert 'Running console script' not in result.stdout
 
 
 def test_hide_run_result_opt(
     tmp_path: Path, console_script: Path, script_runner: ScriptRunner
@@ -323,15 +329,15 @@
 import pytest
 
 @pytest.mark.script_launch_mode('both')
 def test_script(script_runner):
     script_runner.run(R'''{console_script}''')
         """
     )
-    result = script_runner.run('pytest', '-s', '--hide-run-results', str(test))
+    result = script_runner.run(['pytest', '-s', '--hide-run-results', test])
     assert result.success
     assert 'the answer is 42' not in result.stdout
     assert 'Running console script' not in result.stdout
 
 
 class MockEntryPoint:
     module: ModuleType
@@ -401,29 +407,25 @@
     assert result.stderr == ''
 
 
 @pytest.mark.script_launch_mode('both')
 def test_deprecated_args(
     console_script: Path, script_runner: ScriptRunner
 ) -> None:
-    if (
-        script_runner.launch_mode == 'subprocess'
-        and sys.platform == 'win32'
-        and sys.version_info < (3, 8)
-    ):
-        pytest.xfail("PathLike's might not be supported this far back")
     console_script.write_text(
         """
 import sys
 print(sys.argv[1:])
         """
     )
-    result = script_runner.run(console_script, 'A', 'B', check=True)
+    with pytest.warns(match=r".*multiple arguments."):
+        result = script_runner.run(console_script, 'A', 'B', check=True)
     assert result.stdout == "['A', 'B']\n"
-    result = script_runner.run([console_script, 'C'], 'D', check=True)
+    with pytest.warns(match=r".*multiple arguments."):
+        result = script_runner.run([console_script, 'C'], 'D', check=True)
     assert result.stdout == "['C', 'D']\n"
 
 
 @pytest.mark.script_launch_mode('both')
 def test_check(
     console_script: Path, script_runner: ScriptRunner
 ) -> None:
@@ -432,17 +434,22 @@
         script_runner.run(str(console_script), check=True)
 
 
 @pytest.mark.script_launch_mode('both')
 def test_ignore_universal_newlines(
     console_script: Path, script_runner: ScriptRunner
 ) -> None:
-    result = script_runner.run(
-        str(console_script), check=True, universal_newlines=True
-    )
+    expectation: dict[str, ContextManager[Any]] = {
+        'inprocess': pytest.warns(match=r"Keyword argument .* was ignored"),
+        'subprocess': contextlib.nullcontext(),
+    }
+    with expectation[script_runner.launch_mode]:
+        result = script_runner.run(
+            str(console_script), check=True, universal_newlines=True
+        )
     assert result.stdout == 'foo\n'
     assert result.stderr == ''
 
 
 @pytest.mark.script_launch_mode('subprocess')
 def test_disable_universal_newlines(
     console_script: Path, script_runner: ScriptRunner
@@ -463,7 +470,25 @@
     result = script_runner.run(console_script, check=True)
     assert result.stdout == 'foo\n'
     assert result.stderr == ''
     console_script.chmod(0o777)
     result = script_runner.run(console_script, check=True)
     assert result.stdout == 'foo\n'
     assert result.stderr == ''
+
+
+@pytest.mark.script_launch_mode('both')
+def test_run_script_codecs(
+    console_script: Path, script_runner: ScriptRunner
+) -> None:
+    """Check that non-UTF-8 scripts can load"""
+    console_script.write_text(
+        """\
+# -*- coding: cp437 -*-
+import sys  # Non UTF-8 characters -> ≡≡≡
+print('foo')
+        """,
+        encoding="cp437",
+    )
+    result = script_runner.run(console_script, check=True)
+    assert result.stdout == 'foo\n'
+    assert result.stderr == ''
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-console-scripts-1.4.0/tox.ini` & `pytest-console-scripts-1.4.1/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # For more information about tox, see https://tox.readthedocs.org/en/latest/
 [tox]
-envlist = clean,lint,py37,py38,py39,py310,py311,pypy3,report
+envlist = clean,lint,py38,py39,py310,py311,pypy3,report
 
 [testenv]
 deps =
     pytest
     pytest-cov
 usedevelop = true
 commands = pytest tests --cov=pytest_console_scripts --cov-append --cov-report=term-missing {posargs}
 depends =
-    {py37,py38,py39,py310,py311,pypy3}: clean
-    report: py37,py38,py39,py310,py311,pypy3
+    {py38,py39,py310,py311,pypy3}: clean
+    report: py38,py39,py310,py311,pypy3
 
 [testenv:clean]
 deps = coverage
 skip_install = true
 commands = coverage erase
 
 [testenv:report]
```

