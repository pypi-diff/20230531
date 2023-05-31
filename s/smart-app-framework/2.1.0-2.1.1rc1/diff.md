# Comparing `tmp/smart_app_framework-2.1.0-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.1.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 306540 bytes, number of entries: 334
+Zip file size: 306604 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -306,15 +306,15 @@
 -rw-r--r--  2.0 unx     5686 b- defN 80-Jan-01 00:00 smart_kit/template/static/references/tests/hello_scenario_tests.json
 -rw-r--r--  2.0 unx     1838 b- defN 80-Jan-01 00:00 smart_kit/template/wsgi.py-tpl
 -rw-r--r--  2.0 unx      337 b- defN 80-Jan-01 00:00 smart_kit/template/wsgi_config.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/testing/__init__.py
 -rw-r--r--  2.0 unx     7833 b- defN 80-Jan-01 00:00 smart_kit/testing/local.py
 -rw-r--r--  2.0 unx     1409 b- defN 80-Jan-01 00:00 smart_kit/testing/ssml_test/ssml_string_parser.py
 -rw-r--r--  2.0 unx     4067 b- defN 80-Jan-01 00:00 smart_kit/testing/ssml_test/suite.py
--rw-r--r--  2.0 unx    11471 b- defN 80-Jan-01 00:00 smart_kit/testing/suite.py
+-rw-r--r--  2.0 unx    11689 b- defN 80-Jan-01 00:00 smart_kit/testing/suite.py
 -rw-r--r--  2.0 unx     6630 b- defN 80-Jan-01 00:00 smart_kit/testing/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/__init__.py
 -rw-r--r--  2.0 unx      607 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/base_text_normalizer.py
 -rw-r--r--  2.0 unx     3718 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/http_text_normalizer.py
 -rw-r--r--  2.0 unx     6190 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/local_text_normalizer.py
 -rw-r--r--  2.0 unx     9894 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/nltk_tokenizer_binding.py
 -rw-r--r--  2.0 unx     6126 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/pymorphy2_morph_wrapper.py
@@ -326,11 +326,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10819 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32366 b- defN 16-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/RECORD
-334 files, 985903 bytes uncompressed, 253776 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.1.1rc1.dist-info/RECORD
+334 files, 986134 bytes uncompressed, 253822 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -987,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.1.0.dist-info/METADATA
+Filename: smart_app_framework-2.1.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.1.0.dist-info/WHEEL
+Filename: smart_app_framework-2.1.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.1.0.dist-info/RECORD
+Filename: smart_app_framework-2.1.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smart_kit/testing/suite.py

```diff
@@ -22,15 +22,16 @@
         settings: Settings,
         user_cls: type,
         parametrizer_cls: type,
         from_msg_cls: type,
         test_case_cls: type,
         storaged_predefined_fields: Dict[str, Any],
         csv_file_callback: Optional[Callable[[str], Callable[[Any], None]]] = None,
-        interactive: bool = False
+        interactive: bool = False,
+        test_suite: Optional["TestSuite"] = None,
 ) -> Tuple[int, int]:
     test_file_path = os.path.join(path, file)
     if not os.path.isfile(test_file_path) or not test_file_path.endswith('.json'):
         raise FileNotFoundError
     with open(test_file_path, "r") as test_file:
         json_obj = json.load(test_file)
     success = 0
@@ -49,14 +50,15 @@
             user_cls,
             parametrizer_cls,
             from_msg_cls,
             **test_params,
             storaged_predefined_fields=storaged_predefined_fields,
             interactive=interactive,
             csv_case_callback=csv_case_callback,
+            test_suite=test_suite,
         ).run()):
             print(f"[+] {test_case} OK")
             success += 1
     print(f"[+] {file} {success}/{len(json_obj)}")
     return len(json_obj), success
 
 
@@ -126,35 +128,38 @@
                     self.app_model,
                     self.settings,
                     self.app_config.USER,
                     self.app_config.PARAMETRIZER,
                     self.app_config.FROM_MSG,
                     self.app_config.TEST_CASE,
                     self.storaged_predefined_fields,
-                    csv_file_callback
+                    csv_file_callback,
+                    test_suite=self,
                 )
                 total += file_total
                 total_success += file_success
 
         print(f"[+] Total: {total_success}/{total}")
         return total_success == total
 
 
 class TestCase:
     def __init__(self, app_model: SmartAppModel, settings: Settings, user_cls: type, parametrizer_cls: type,
                  from_msg_cls: type, messages: dict, storaged_predefined_fields: Dict[str, Any], interactive: bool,
-                 csv_case_callback: Optional[Callable[[Any], None]] = None, user: Optional[dict] = None):
+                 csv_case_callback: Optional[Callable[[Any], None]] = None, test_suite: Optional[TestSuite] = None,
+                 user: Optional[dict] = None):
         self.messages = messages
         self.user_state = json.dumps(user)
         self.interactive = interactive
 
         self.app_model = app_model
         self.settings = settings
         self.storaged_predefined_fields = storaged_predefined_fields
         self.csv_case_callback = csv_case_callback
+        self.test_suite = test_suite
 
         self.__parametrizer_cls = parametrizer_cls
         self.__user_cls = user_cls
         self.__from_msg_cls = from_msg_cls
 
     async def _run(self) -> bool:
         success = True
```

## Comparing `smart_app_framework-2.1.0.dist-info/METADATA` & `smart_app_framework-2.1.1rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.1.0
+Version: 2.1.1rc1
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Requires-Dist: ics (==0.6)
 Requires-Dist: incremental (==21.3.0)
 Requires-Dist: keras (==2.12.0) ; extra == "ml"
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: nltk (==3.5)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: objgraph (==3.4.1)
-Requires-Dist: prometheus-client (==0.7.1)
+Requires-Dist: prometheus-client (==0.11.0)
 Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: psutil (==5.8.0)
 Requires-Dist: pyignite (==0.5.2)
 Requires-Dist: pymorphy2 (==0.8)
 Requires-Dist: pymorphy2_dicts (==2.4.393442.3710985)
 Requires-Dist: python-dateutil (==2.7.3)
 Requires-Dist: python-json-logger (==0.1.11)
```

## Comparing `smart_app_framework-2.1.0.dist-info/RECORD` & `smart_app_framework-2.1.1rc1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
 smart_kit/template/static/references/tests/hello_scenario_tests.json,sha256=WPZ08Jui9H5WVasMrWcgzb9ls9sv83kMj0hirxXOkcM,5686
 smart_kit/template/wsgi.py-tpl,sha256=Y5mMuIvtpPlg07HrmGotuJ5ezB7modw7T7jZamJVtko,1838
 smart_kit/template/wsgi_config.py-tpl,sha256=nQOOf4builgRYfnOo_2cCWak3hKNzjGQU5kXeAZTCzk,337
 smart_kit/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/testing/local.py,sha256=xCzBCEdbWVHKYKakygPdspKVKfQBwFc3FD605jeaKbo,7833
 smart_kit/testing/ssml_test/ssml_string_parser.py,sha256=Ro8UbPGsaO86RBi9EbkEf8jn3wzTVH26OHXBmdAvHSg,1409
 smart_kit/testing/ssml_test/suite.py,sha256=6-XgovyY2jlz6N0v-HwkdBMtCkvVwslFP2QEWZcyKY4,4067
-smart_kit/testing/suite.py,sha256=R7Uqlz-qKUWANU0DlRVM5ZrZOOJSlYhuMtLPQNByXfM,11471
+smart_kit/testing/suite.py,sha256=L7ca6q2QbfCjmIfCzoSjlrflBaeEu5dBV-A13mTds1I,11689
 smart_kit/testing/utils.py,sha256=eQT3UXz0YSmAyGcBqinS0LMeFP_dszPNum29jfLdRDU,6630
 smart_kit/text_preprocessing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/text_preprocessing/base_text_normalizer.py,sha256=516_iatoGuJDVOJILwzuGavdLxqaGjuhAWCOxdeGwHc,607
 smart_kit/text_preprocessing/http_text_normalizer.py,sha256=D9BN7JxOXn1AepAfLOCNex4tZbsMlDBtgmW7NNpcNBA,3718
 smart_kit/text_preprocessing/local_text_normalizer.py,sha256=xuaxK0gFX6MsMdg-SREPcu5TqlkGuKvzgBp000j09B4,6190
 smart_kit/text_preprocessing/nltk_tokenizer_binding.py,sha256=pN7thYgSnks55n_44ZIcDJHxInN0QFgkH8aWT2XFHgY,9894
 smart_kit/text_preprocessing/pymorphy2_morph_wrapper.py,sha256=0SBv6IzvZT_SDiwRIroHa28d8Tdps1Kgq2q0a3-SJjo,6126
@@ -325,10 +325,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=bC7tdYW480irANhxaFxiKgnAsvmz-luf52WSu7ZjnIU,3385
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.1.0.dist-info/METADATA,sha256=fnCTVaNZ8FX0HB1KM8-OvK6qd1Yn-BfTSrwgDs0PL4o,10819
-smart_app_framework-2.1.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-smart_app_framework-2.1.0.dist-info/RECORD,,
+smart_app_framework-2.1.1rc1.dist-info/METADATA,sha256=zTgsP0HpEs3wudTEq9i_PZGJ5nkX0T3Lf1NVzQ-BrkY,10823
+smart_app_framework-2.1.1rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.1.1rc1.dist-info/RECORD,,
```

