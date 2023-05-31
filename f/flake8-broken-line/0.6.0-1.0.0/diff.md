# Comparing `tmp/flake8-broken-line-0.6.0.tar.gz` & `tmp/flake8_broken_line-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-broken-line-0.6.0.tar", max compression
+gzip compressed data, was "flake8_broken_line-1.0.0.tar", max compression
```

## Comparing `flake8-broken-line-0.6.0.tar` & `flake8_broken_line-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1071 2022-10-03 05:03:59.304042 flake8-broken-line-0.6.0/LICENSE
--rw-r--r--   0        0        0     2160 2022-10-03 05:15:53.281305 flake8-broken-line-0.6.0/README.md
--rw-r--r--   0        0        0     1704 2022-10-03 05:15:53.283511 flake8-broken-line-0.6.0/flake8_broken_line.py
--rw-r--r--   0        0        0     1597 2022-10-03 05:15:53.286178 flake8-broken-line-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 flake8-broken-line-0.6.0/setup.py
--rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 flake8-broken-line-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 09:57:48.513662 flake8_broken_line-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2160 2023-05-31 09:57:48.513755 flake8_broken_line-1.0.0/README.md
+-rw-r--r--   0        0        0     1572 2023-05-31 10:09:04.904389 flake8_broken_line-1.0.0/flake8_broken_line.py
+-rw-r--r--   0        0        0     1242 2023-05-31 10:09:04.904797 flake8_broken_line-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 flake8_broken_line-1.0.0/PKG-INFO
```

### Comparing `flake8-broken-line-0.6.0/LICENSE` & `flake8_broken_line-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-broken-line-0.6.0/README.md` & `flake8_broken_line-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-broken-line-0.6.0/flake8_broken_line.py` & `flake8_broken_line-1.0.0/flake8_broken_line.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import re
 import tokenize
 from typing import Iterator, Sequence, Set, Tuple
-
-try:  # pragma: no cover
-    from importlib import metadata as importlib_metadata  # type: ignore
-except ImportError:  # pragma: no cover
-    import importlib_metadata  # type: ignore
+from importlib import metadata as importlib_metadata
 
 #: This is a name that we use to install this library:
 pkg_name = 'flake8-broken-line'
 
 #: We store the version number inside the `pyproject.toml`:
 pkg_version = importlib_metadata.version(pkg_name)
```

### Comparing `flake8-broken-line-0.6.0/setup.py` & `flake8_broken_line-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flake8-broken-line
+Version: 1.0.0
+Summary: Flake8 plugin to forbid backslashes for line breaks
+Home-page: https://github.com/wemake-services/flake8-broken-line
+License: MIT
+Keywords: flake8,flake8-plugin,linting,linter,wemake.services,code quality
+Author: Nikita Sobolev
+Author-email: mail@sobolevn.me
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Flake8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: flake8 (>5)
+Project-URL: Funding, https://opencollective.com/wemake-python-styleguide
+Project-URL: Repository, https://github.com/wemake-services/flake8-broken-line
+Description-Content-Type: text/markdown
 
-modules = \
-['flake8_broken_line']
-install_requires = \
-['flake8>=3.5,<6']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata']}
-
-entry_points = \
-{'flake8.extension': ['N4 = flake8_broken_line:check_line_breaks']}
-
-setup_kwargs = {
-    'name': 'flake8-broken-line',
-    'version': '0.6.0',
-    'description': 'Flake8 plugin to forbid backslashes for line breaks',
-    'long_description': '# flake8-broken-line\n\n[![wemake.services](https://img.shields.io/badge/-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)\n[![Build Status](https://github.com/wemake-services/flake8-broken-line/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/flake8-broken-line/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/wemake-services/flake8-broken-line/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/flake8-broken-line)\n[![Python Version](https://img.shields.io/pypi/pyversions/flake8-broken-line.svg)](https://pypi.org/project/flake8-broken-line/)\n[![PyPI version](https://badge.fury.io/py/flake8-broken-line.svg)](https://pypi.org/project/flake8-broken-line/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nDo not break the line! 🚨\n\n\n## Installation\n\n```bash\npip install flake8-broken-line\n```\n\nIt is also a valuable part of [`wemake-python-styleguide`](https://github.com/wemake-services/wemake-python-styleguide).\n\n\n## Code example\n\nThings we check with this plugin:\n\n```python\n# String line breaks, use `()` or `"""` instead:\n\nsome_string = \'first line\\\nsecond line\'\n\n# Use a single line, `()`, or new variables instead:\n\nif 1 == 1 and \\\n    2 == 2:\n    print(\'Do not do that!\')\n\n# Do not use for method chaining:\nsome_object \\\n  .call_method(param1, param2) \\\n  .call_other(keyword=value) \\\n  .finalize()\n\n# Instead use:\nsome_objects.call_method(\n    param1, param2,\n).call_other(\n    keyword=value\n).finalize()\n\n```\n\n\n## Error codes\n\n| Error code |                   Description                  |\n|:----------:|:----------------------------------------------:|\n|    N400    | Found backslash that is used for line breaking |\n\n\n## License\n\nMIT.\n',
-    'author': 'Nikita Sobolev',
-    'author_email': 'mail@sobolevn.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/wemake-services/flake8-broken-line',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+# flake8-broken-line
 
+[![wemake.services](https://img.shields.io/badge/-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)
+[![Build Status](https://github.com/wemake-services/flake8-broken-line/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/flake8-broken-line/actions?query=workflow%3Atest)
+[![codecov](https://codecov.io/gh/wemake-services/flake8-broken-line/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/flake8-broken-line)
+[![Python Version](https://img.shields.io/pypi/pyversions/flake8-broken-line.svg)](https://pypi.org/project/flake8-broken-line/)
+[![PyPI version](https://badge.fury.io/py/flake8-broken-line.svg)](https://pypi.org/project/flake8-broken-line/)
+[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
+
+Do not break the line! 🚨
+
+
+## Installation
+
+```bash
+pip install flake8-broken-line
+```
+
+It is also a valuable part of [`wemake-python-styleguide`](https://github.com/wemake-services/wemake-python-styleguide).
+
+
+## Code example
+
+Things we check with this plugin:
+
+```python
+# String line breaks, use `()` or `"""` instead:
+
+some_string = 'first line\
+second line'
+
+# Use a single line, `()`, or new variables instead:
+
+if 1 == 1 and \
+    2 == 2:
+    print('Do not do that!')
+
+# Do not use for method chaining:
+some_object \
+  .call_method(param1, param2) \
+  .call_other(keyword=value) \
+  .finalize()
+
+# Instead use:
+some_objects.call_method(
+    param1, param2,
+).call_other(
+    keyword=value
+).finalize()
+
+```
+
+
+## Error codes
+
+| Error code |                   Description                  |
+|:----------:|:----------------------------------------------:|
+|    N400    | Found backslash that is used for line breaking |
+
+
+## License
+
+MIT.
 
-setup(**setup_kwargs)
```

