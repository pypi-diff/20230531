# Comparing `tmp/pytest-embedded-1.2.5.tar.gz` & `tmp/pytest-embedded-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-1.2.5.tar", last modified: Tue Apr 11 05:40:50 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-1.3.0.tar", last modified: Wed May 31 13:09:02 2023, max compression
```

## Comparing `pytest-embedded-1.2.5.tar` & `pytest-embedded-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50776 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/unity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/setup.py
```

### Comparing `pytest-embedded-1.2.5/PKG-INFO` & `pytest-embedded-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
```

### Comparing `pytest-embedded-1.2.5/pytest_embedded/app.py` & `pytest-embedded-1.3.0/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.5/pytest_embedded/dut.py` & `pytest-embedded-1.3.0/pytest_embedded/dut.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from typing import AnyStr, Callable, List, Match, Optional, Union
 
 import pexpect
 
 from .app import App
 from .log import PexpectProcess
 from .unity import UNITY_SUMMARY_LINE_REGEX, TestSuite
-from .utils import Meta, remove_asci_color_code, to_bytes, to_list
+from .utils import Meta, _InjectMixinCls, remove_asci_color_code, to_bytes, to_list
 
 
-class Dut:
+class Dut(_InjectMixinCls):
     """
     Device under test (DUT) base class
 
     Attributes:
         pexpect_proc (PexpectProcess): `PexpectProcess` instance
         app (App): `App` instance
         logfile (str): log file path
@@ -156,21 +156,43 @@
                 Use this argument when need to run `expect` functions between one unity test call.
 
         Notes:
             - Would raise AssertionError at the end of the test if any unity test case result is "FAIL"
             - Would raise TIMEOUT exception at the end of the test if any unity test case execution took longer
                 than timeout value
 
-        Warnings:
+        Warning:
             - All unity test cases record would be missed if the final report block is uncaught.
         """
         self.expect(UNITY_SUMMARY_LINE_REGEX, timeout=timeout)
 
         if extra_before:
             log = to_bytes(extra_before) + self.pexpect_proc.before
         else:
             log = self.pexpect_proc.before
 
         if remove_asci_escape_code:
             log = remove_asci_color_code(log)
 
         self.testsuite.add_unity_test_cases(log)
+
+    @_InjectMixinCls.require_services('idf')
+    def run_all_single_board_cases(
+        self,
+        group: Optional[str] = None,
+        reset: bool = False,
+        timeout: float = 30,
+        run_ignore_cases: bool = False,
+    ):
+        """
+        Run all multi_stage cases
+
+        Args:
+            group: test case group
+            reset: whether to perform a hardware reset before running a case
+            timeout: timeout. (Default: 30 seconds)
+            run_ignore_cases: run ignored test cases or not
+
+        Warning:
+            requires enable service `idf`
+        """
+        pass
```

### Comparing `pytest-embedded-1.2.5/pytest_embedded/log.py` & `pytest-embedded-1.3.0/pytest_embedded/log.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.5/pytest_embedded/plugin.py` & `pytest-embedded-1.3.0/pytest_embedded/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,25 +212,34 @@
     )
     qemu_group.addoption(
         '--qemu-prog-path',
         help='QEMU program path. (Default: "qemu-system-xtensa")',
     )
     qemu_group.addoption(
         '--qemu-cli-args',
-        help='QEMU cli default arguments. (Default: "-nographic -no-reboot -machine esp32")',
+        help='QEMU cli default arguments. (Default: "-nographic -machine esp32")',
     )
     qemu_group.addoption(
         '--qemu-extra-args',
         help='QEMU cli extra arguments, will append to the argument list. (Default: None)',
     )
     qemu_group.addoption(
         '--skip-regenerate-image',
         help='y/yes/true for True and n/no/false for False. '
         'Set to True to disable auto regenerate image. (Default: False)',
     )
+    qemu_group.addoption(
+        '--encrypt',
+        help='y/yes/true for True and n/no/false for False. '
+        'Set to True for pre-encryption workflow (Default: False)',
+    )
+    qemu_group.addoption(
+        '--keyfile',
+        help='Flash Encryption (pre-encrypted workflow) key path. (Default: None)',
+    )
 
 
 ###########
 # helpers #
 ###########
 _COUNT = 1
 
@@ -894,14 +903,28 @@
 @pytest.fixture
 @multi_dut_argument
 def skip_regenerate_image(request: FixtureRequest) -> t.Optional[str]:
     """Enable parametrization for the same cli option"""
     return _request_param_or_config_option_or_default(request, 'skip_regenerate_image', None)
 
 
+@pytest.fixture
+@multi_dut_argument
+def encrypt(request: FixtureRequest) -> t.Optional[str]:
+    """Enable parametrization for the same cli option"""
+    return _request_param_or_config_option_or_default(request, 'encrypt', None)
+
+
+@pytest.fixture
+@multi_dut_argument
+def keyfile(request: FixtureRequest) -> t.Optional[str]:
+    """Enable parametrization for the same cli option"""
+    return _request_param_or_config_option_or_default(request, 'keyfile', None)
+
+
 ####################
 # Private Fixtures #
 ####################
 @pytest.fixture
 @multi_dut_fixture
 def _services(embedded_services: t.Optional[str]) -> t.List[str]:
     if not embedded_services:
@@ -920,14 +943,15 @@
 
     return ['base'] + services
 
 
 @dataclass
 class ClassCliOptions:
     classes: t.Dict[str, type]
+    mixins: t.Dict[str, t.List[type]]
     kwargs: t.Dict[str, t.Dict[str, t.Any]]
 
 
 @pytest.fixture
 @multi_dut_fixture
 def _fixture_classes_and_options(
     _services,
@@ -954,14 +978,16 @@
     gdb_cli_args,
     no_gdb,
     qemu_image_path,
     qemu_prog_path,
     qemu_cli_args,
     qemu_extra_args,
     skip_regenerate_image,
+    encrypt,
+    keyfile,
     # pre-initialized fixtures
     dut_index,
     _pexpect_logfile,
     test_case_name,
     pexpect_proc,
     msg_queue,
     _meta,
@@ -981,14 +1007,15 @@
         },
         }
     }
         ...
     }
     """
     classes: t.Dict[str, type] = {}
+    mixins: t.Dict[str, t.List[type]] = defaultdict(list)
     kwargs: t.Dict[str, t.Dict[str, t.Any]] = defaultdict(dict)
 
     for fixture in FIXTURES_SERVICES.keys():
         if fixture == 'app':
             kwargs['app'] = {'app_path': app_path, 'build_dir': build_dir}
             if 'idf' in _services:
                 if 'qemu' in _services:
@@ -997,14 +1024,16 @@
                     classes[fixture] = QemuApp
                     kwargs[fixture].update(
                         {
                             'msg_queue': msg_queue,
                             'part_tool': part_tool,
                             'qemu_image_path': qemu_image_path,
                             'skip_regenerate_image': skip_regenerate_image,
+                            'encrypt': encrypt,
+                            'keyfile': keyfile,
                         }
                     )
                 else:
                     from pytest_embedded_idf import IdfApp
 
                     classes[fixture] = IdfApp
                     kwargs[fixture].update(
@@ -1095,24 +1124,31 @@
                         'msg_queue': msg_queue,
                         'gdb_prog_path': gdb_prog_path,
                         'gdb_cli_args': gdb_cli_args,
                         'meta': _meta,
                     }
         elif fixture == 'qemu':
             if 'qemu' in _services:
-                from pytest_embedded_qemu import DEFAULT_IMAGE_FN, Qemu
+                from pytest_embedded_qemu import (
+                    DEFAULT_IMAGE_FN,
+                    ENCRYPTED_IMAGE_FN,
+                    Qemu,
+                )
 
                 classes[fixture] = Qemu
                 kwargs[fixture] = {
                     'msg_queue': msg_queue,
                     'qemu_image_path': qemu_image_path
-                    or os.path.join(app_path or '', build_dir or 'build', DEFAULT_IMAGE_FN),
+                    or os.path.join(
+                        app_path or '', build_dir or 'build', ENCRYPTED_IMAGE_FN if encrypt else DEFAULT_IMAGE_FN
+                    ),
                     'qemu_prog_path': qemu_prog_path,
                     'qemu_cli_args': qemu_cli_args,
                     'qemu_extra_args': qemu_extra_args,
+                    'app': None,
                     'meta': _meta,
                 }
         elif fixture == 'dut':
             classes[fixture] = Dut
             kwargs[fixture] = {
                 'pexpect_proc': pexpect_proc,
                 'msg_queue': msg_queue,
@@ -1126,14 +1162,19 @@
 
                 classes[fixture] = QemuDut
                 kwargs[fixture].update(
                     {
                         'qemu': None,
                     }
                 )
+
+                if 'idf' in _services:
+                    from pytest_embedded_idf.unity_tester import IdfUnityDutMixin
+
+                    mixins[fixture].append(IdfUnityDutMixin)
             elif 'jtag' in _services:
                 if 'idf' in _services:
                     from pytest_embedded_idf import IdfDut
 
                     classes[fixture] = IdfDut
                 else:
                     from pytest_embedded_serial import SerialDut
@@ -1165,15 +1206,15 @@
 
                 kwargs[fixture].update(
                     {
                         'serial': None,
                     }
                 )
 
-    return ClassCliOptions(classes, kwargs)
+    return ClassCliOptions(classes, mixins, kwargs)
 
 
 ####################
 # Derived Fixtures #
 ####################
 @pytest.fixture
 @multi_dut_fixture
@@ -1264,14 +1305,15 @@
         cls = LinuxDut
         kwargs = _fixture_classes_and_options.kwargs['dut']
         kwargs['serial'] = serial
 
         return cls(**kwargs)
 
     cls = _fixture_classes_and_options.classes['dut']
+    mixins = _fixture_classes_and_options.mixins['dut']
     kwargs = _fixture_classes_and_options.kwargs['dut']
 
     for k, v in kwargs.items():
         if v is None:
             if k == 'app':
                 kwargs[k] = app
             elif k == 'serial':
@@ -1279,15 +1321,15 @@
             elif k == 'openocd':
                 kwargs[k] = openocd
             elif k == 'gdb':
                 kwargs[k] = gdb
             elif k == 'qemu':
                 kwargs[k] = qemu
 
-    return cls(**_drop_none_kwargs(kwargs))
+    return cls(**_drop_none_kwargs(kwargs), mixins=mixins)
 
 
 @pytest.fixture
 def unity_tester(dut: t.Union['IdfDut', t.Tuple['IdfDut']]) -> t.Optional['CaseTester']:
     try:
         from pytest_embedded_idf import CaseTester, IdfDut
     except ImportError:
```

### Comparing `pytest-embedded-1.2.5/pytest_embedded/unity.py` & `pytest-embedded-1.3.0/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.5/pytest_embedded/utils.py` & `pytest-embedded-1.3.0/pytest_embedded/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     'gdb': ['jtag'],
     'qemu': ['qemu'],
     'dut': ['base', 'serial', 'jtag', 'qemu', 'idf'],
 }
 
 _T = t.TypeVar('_T')
 
+_MIXIN_REQUIRED_SERVICES = {
+    'IdfUnityMixin': ['idf'],
+}
+
+_MIXIN_REQUIRED_SERVICES_KEY = '_based_on_services'
+
 
 #######################
 # Errors and Warnings #
 #######################
 class UserHint(Warning):
     pass
 
@@ -50,14 +56,24 @@
     def __init__(self, service: str) -> None:
         super().__init__(
             f'Package {SERVICE_LIB_NAMES[service]} is not found but required by service {service}. '
             f'Please run "pip install -U {SERVICE_LIB_NAMES[service]}"'
         )
 
 
+class RequireServiceError(SystemExit):
+    def __init__(self, func_name: str, services: t.Union[str, t.List[str]]) -> None:
+        services_str = ','.join(to_list(services))
+        super().__init__(
+            f'function {func_name} requires enabling one of the service(s) {services_str}. '
+            f'Please enable by passing CLI options "--embedded-services {services_str}". '
+            f'For more details, please refer to "pytest --help".'
+        )
+
+
 #####################
 # Utility Functions #
 #####################
 def to_str(bytes_str: t.AnyStr) -> str:
     """
     Turn `bytes` or `str` to `str`
 
@@ -241,7 +257,84 @@
             imported = getattr(module, object_name)
             name_obj_dict[object_name] = imported
             return imported
         else:
             raise AttributeError('Attribute %s not found in module %s', object_name, base_module.__name__)
 
     return __getattr__
+
+
+class _InjectMixinMeta(type):
+    def __call__(cls, *args, **kwargs):
+        try:
+            mixins = kwargs.pop('mixins', None)
+            if mixins:
+                mixins = to_list(mixins)
+                name = cls.__name__ + 'With' + 'And'.join([m.__name__ for m in mixins])
+                cls = type(name, tuple([*mixins, cls]), {})
+
+                # users should only know concept "services", not mixins
+                _based_on_services = set()
+                for m in mixins:
+                    if m.__name__ not in _MIXIN_REQUIRED_SERVICES:
+                        continue
+
+                    _based_on_services.update(to_list(_MIXIN_REQUIRED_SERVICES[m.__name__]))
+                kwargs[_MIXIN_REQUIRED_SERVICES_KEY] = sorted(_based_on_services)
+        except KeyError:
+            pass
+        return type.__call__(cls, *args, **kwargs)
+
+
+class _InjectMixinCls(metaclass=_InjectMixinMeta):
+    """
+    This class provide a check function `require_services()` to check if the function is injected by
+    enabling one of the required services.
+
+    The benefits are:
+    - provide the autocompletion for the functions provided by the mixins
+    - check the requirement at runtime
+
+    Examples:
+
+        class IdfUnityMixin:
+            def foo(self):
+                print('foo from MixinOne')
+
+
+        class Test(_InjectMixinCls):
+            def __init__(self, **kwargs):
+                for k, v in kwargs.items():
+                    setattr(self, k, v)
+
+            @_InjectMixinCls.require_services('idf')
+            def foo(self):
+                pass
+
+
+        # mro(): TestWithIdfUnityMixin, IdfUnityMixin, Test, object
+        s1 = Test(mixins=IdfUnityMixin)
+        # mro(): Test, object
+        s2 = Test()
+        s1.foo()  # foo from IdfUnityMixin
+        s2.foo()  # function foo requires enabling one of the service(s) idf.
+    """
+
+    def require_services(*services):
+        def decorator(func):
+            def wrapped(self, *args, **kwargs):
+                based = False
+                for service in services:
+                    if hasattr(self, _MIXIN_REQUIRED_SERVICES_KEY) and service in getattr(
+                        self, _MIXIN_REQUIRED_SERVICES_KEY
+                    ):
+                        based = True
+                        break
+
+                if based:
+                    return func(self, *args, **kwargs)
+                else:
+                    raise RequireServiceError(func.__name__, services)
+
+            return wrapped
+
+        return decorator
```

### Comparing `pytest-embedded-1.2.5/pytest_embedded.egg-info/PKG-INFO` & `pytest-embedded-1.3.0/pytest_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
```

### Comparing `pytest-embedded-1.2.5/setup.py` & `pytest-embedded-1.3.0/setup.py`

 * *Files identical despite different names*

