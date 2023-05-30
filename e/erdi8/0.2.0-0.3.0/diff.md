# Comparing `tmp/erdi8-0.2.0.tar.gz` & `tmp/erdi8-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdi8-0.2.0.tar", last modified: Sat Dec 31 12:50:18 2022, max compression
+gzip compressed data, was "erdi8-0.3.0.tar", last modified: Tue May 30 22:32:34 2023, max compression
```

## Comparing `erdi8-0.2.0.tar` & `erdi8-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2022-12-31 12:50:18.655543 erdi8-0.2.0/
--rw-rw-r--   0 andreas   (1000) andreas   (1000)    35149 2022-05-15 15:48:18.000000 erdi8-0.2.0/LICENSE
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       18 2022-05-15 15:48:18.000000 erdi8-0.2.0/MANIFEST.in
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     5221 2022-12-31 12:50:18.655543 erdi8-0.2.0/PKG-INFO
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     4443 2022-12-31 09:31:10.000000 erdi8-0.2.0/README.md
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2022-12-31 12:50:18.655543 erdi8-0.2.0/erdi8/
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       30 2022-05-15 15:48:18.000000 erdi8-0.2.0/erdi8/__init__.py
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     4059 2022-12-28 23:27:11.000000 erdi8-0.2.0/erdi8/erdi8.py
-drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2022-12-31 12:50:18.655543 erdi8-0.2.0/erdi8.egg-info/
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     5221 2022-12-31 12:50:18.000000 erdi8-0.2.0/erdi8.egg-info/PKG-INFO
--rw-rw-r--   0 andreas   (1000) andreas   (1000)      187 2022-12-31 12:50:18.000000 erdi8-0.2.0/erdi8.egg-info/SOURCES.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)        1 2022-12-31 12:50:18.000000 erdi8-0.2.0/erdi8.egg-info/dependency_links.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)        6 2022-12-31 12:50:18.000000 erdi8-0.2.0/erdi8.egg-info/top_level.txt
--rw-rw-r--   0 andreas   (1000) andreas   (1000)       38 2022-12-31 12:50:18.655543 erdi8-0.2.0/setup.cfg
--rw-rw-r--   0 andreas   (1000) andreas   (1000)     1786 2022-12-31 12:49:32.000000 erdi8-0.2.0/setup.py
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-30 22:32:34.852519 erdi8-0.3.0/
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)    35149 2022-05-15 15:48:18.000000 erdi8-0.3.0/LICENSE
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       18 2022-05-15 15:48:18.000000 erdi8-0.3.0/MANIFEST.in
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     6691 2023-05-30 22:32:34.852519 erdi8-0.3.0/PKG-INFO
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     5950 2023-05-30 22:26:59.000000 erdi8-0.3.0/README.md
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-30 22:32:34.852519 erdi8-0.3.0/erdi8/
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       30 2022-05-15 15:48:18.000000 erdi8-0.3.0/erdi8/__init__.py
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     5178 2023-05-30 21:17:53.000000 erdi8-0.3.0/erdi8/erdi8.py
+drwxrwxr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-30 22:32:34.852519 erdi8-0.3.0/erdi8.egg-info/
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     6691 2023-05-30 22:32:34.000000 erdi8-0.3.0/erdi8.egg-info/PKG-INFO
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)      187 2023-05-30 22:32:34.000000 erdi8-0.3.0/erdi8.egg-info/SOURCES.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)        1 2023-05-30 22:32:34.000000 erdi8-0.3.0/erdi8.egg-info/dependency_links.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)        6 2023-05-30 22:32:34.000000 erdi8-0.3.0/erdi8.egg-info/top_level.txt
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)       38 2023-05-30 22:32:34.852519 erdi8-0.3.0/setup.cfg
+-rw-rw-r--   0 andreas   (1000) andreas   (1000)     1786 2023-05-30 22:27:49.000000 erdi8-0.3.0/setup.py
```

### Comparing `erdi8-0.2.0/LICENSE` & `erdi8-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdi8-0.2.0/PKG-INFO` & `erdi8-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,104 @@
-Metadata-Version: 2.1
-Name: erdi8
-Version: 0.2.0
-Summary: Count according to lower case alphabet and numbers (without ambiguous 0, 1, and l) and always start with a letter
-Home-page: https://github.com/athalhammer/erdi8
-Author: Andreas Thalhammer
-Author-email: andreas@thalhammer.bayern
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![example workflow](https://github.com/athalhammer/erdi8/actions/workflows/unit_tests.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/erdi8)](https://pypi.org/project/erdi8)
 [![GitHub license](https://img.shields.io/github/license/athalhammer/erdi8.svg)](https://github.com/athalhammer/erdi8/blob/master/LICENSE)
 
 # erdi8
 
-erdi8 is a [unique identifier](https://www.wikidata.org/wiki/Q6545185) scheme and counter that operates on the following alphabet:
+erdi8 is a [unique identifier](https://www.wikidata.org/wiki/Q6545185) scheme and identifier generator that counts with the following alphabet:
 
 ```
 ['2', '3', '4', '5', '6', '7', '8', '9', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 
 'i', 'j', 'k', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
 ```
 
 It is basically a base36 alphabet that intentionally avoids the ambiguous characters `[0, 1, and l]` and therefore shrinks to 33. In addition to that, it ensures that no identifier starts with a numeric value by using an offset of 8. The zero is represented by 'a', 25 is represented by 'a2', etc. With three characters or less one can create 28'075 (25 + 25 * 33 + 25 * 33 * 33) different identifiers. With 6 characters or less we have 1'008'959'350 options. In a traditional identifier world, one would use a prefix, e.g. M, and then an integer. This only gives you 100k identifiers (M0 to M99999) with up to 6 characters. The scheme enables consecutive counting and is therefore free of collisions. In particular, it is __not__ a method to create secret identifiers.
 
 ## Usage
 
 
-### Basic
+### Basic (counting)
 ```
 $ python3
 
 >>> from erdi8 import Erdi8
 >>> e8 = Erdi8()
 >>> e8.increment("erdi8")
 'erdi9'
 >>> e8.decode_int("erdi8")
 6545185
 >>> e8.encode_int(6545185)
 'erdi8'
 ```
 
-### Advanced
+### Advanced (still counting)
 Fixed length "fancy" identifiers with `safe=True` 
 
 ```
 $ python3
 
 >>> from erdi8 import Erdi8
 >>> safe = True
 >>> start = 'b222222222'
->>> seed = 453459956896834
+>>> stride = 30321718760514
 >>> e8 = Erdi8(safe)
->>> e8.increment_fancy(start, seed)
+>>> e8.increment_fancy(start, stride)
 'fmzz7cwc43'
->>> current = e8.increment_fancy('fmzz7cwc43', seed)
+>>> current = e8.increment_fancy('fmzz7cwc43', stride)
 >>> print(current)
 k7zydqrp64
+
+# reverse engineer stride from two consecutive identifiers
+>>> e8.compute_stride('fmzz7cwc43', current)
+{'stride_effective': 30321718760517, 'stride_other_candidates': [30321718760516, 30321718760515, 30321718760514]}
 ```
 
 **NOTE**
 
 0. These sequences may have a "fancy" appearance but __they are not random__. They are perfectly predictable and are designed to "fill up the whole mod space" before previously coined identifiers start re-appearing.
 1. The `safe=True` option helps you to avoid unintended words (i.e. removes the characters `[aeiou]` from the alphabet)
 2. The fancy increment works with fixed lengths. If you work with a length of 10 (like above) You will have `20 * 28^9 = 211'569'119'068'160` options with `safe=True`. If you think you have more things to identify at some point you have two options: a) start directly with more characters or b) check for the start value (in this case `b222222222`) to re-appear - this will be the identifier that will "show up twice" first.
-3. Store the following four parts in a safe place: a) `safe` parameter b) the `start` value c) the `seed` value. On top, keep good track of the `current` value.
+3. Store the following four parts in a safe place: a) `safe` parameter b) the `start` value c) the `stride` value. On top, keep good track of the `current` value.
+
+
+### Advanced (random)
+Also see documentation of Python's integrated [`random`](https://docs.python.org/3/library/random.html) and [`secrets`](https://docs.python.org/3/library/secrets.html) modules, in particular for `random`: "The pseudo-random generators of this module should not be used for security purposes. For security or cryptographic uses, see the `secrets` module". In any case, you should know what you are doing.
+
+`random` module:
+
+```
+$ python3
+
+>>> import random
+>>> from erdi8 import Erdi8
+>>> e8 = Erdi8()
+
+# get random erdi8 identifiers with length 10
+>>> mini, maxi, space = e8.mod_space(10)
+>>> e8.encode_int(random.randint(mini, maxi))
+'vvctyx7c6o'
+```
 
-### More advanced
+`secrets` module:
+
+```
+$ python3
+
+>>> import secrets
+>>> from erdi8 import Erdi8
+>>> e8 = Erdi8()
+
+>>> e8.encode_int(int.from_bytes(secrets.token_bytes()))
+'jtx3i83pii8wo98wzuucu7uag6khrfpabrdn3qrqrxdxauvcgjg'
+
+>>> e8.encode_int(secrets.randbits(256))
+'a53mpn3xntywcbdcvfa932ub34evne9oha8pzoy6ii3ur2e364z'
+```
+
+### Even more advanced
 Run a light-weight erdi8 identifier service via [fasterid](https://github.com/athalhammer/fasterid)
 
 
 ## Test cases
 
 ```
 $ python3 -m unittest test/erdi8_test.py 
@@ -89,18 +108,16 @@
 
 __Why no upper case characters?__
 
 _Because we don't want to `erdi8` to be confused with `Erdi8`._
 
 __Why no start with a number?__
 
-_Because we want to avoid "number-only" identifiers. If we allowed to start with a number, we would have identifiers of the type `42` and `322` which could be mistaken for integers. We could achieve this with a more complex scheme avoiding any number-only combinations (would therefore still allow ids like `2z`, to be investigated)._
+_Because we want to avoid "number-only" identifiers. If we allowed to start with a number, we would have identifiers of the type `42` and `322` which could be mistaken for integers. We could achieve this with a more complex scheme avoiding any number-only combinations (would therefore still allow ids like `2z`, to be investigated). In essence it is important to note that programs like Excel are really creative when transforming input data, for example `08342 -> 8342`, `12e34 -> 12E+34`, `SEPT1 -> Sep-01` etc. erdi8 with the safe option on avoids 99% of these types of issues._
 
 __How about combinations that form actual (bad) words?__
 
 _This depends on the use case and the way erdi8 is used. Therefore, we can recommend to work with filter lists. In addition, an erdi8 object that avoids the `aeiou` characters can be created with `Erdi8(safe=True)`. This shrinks the available character space to 28 and the produced output is not compatible to `Erdi8(safe=False)` (default). The danger that unintended English words are created is lower with this setting.  It is recommended for erdi8 identifiers that are longer than three characters where filter lists start to become impractical._
 
 __How does this relate to binary-to-text encodings such as base32 and base64?__
 
 _erdi8 can be used for a binary-to-text encoding and the basic functions to implement this are provided with `encode_int` and `decode_int`. However, the primary purpose is to provide a short counting scheme for identifiers._
-
-
```

### Comparing `erdi8-0.2.0/erdi8.egg-info/PKG-INFO` & `erdi8-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: erdi8
-Version: 0.2.0
+Version: 0.3.0
 Summary: Count according to lower case alphabet and numbers (without ambiguous 0, 1, and l) and always start with a letter
 Home-page: https://github.com/athalhammer/erdi8
 Author: Andreas Thalhammer
 Author-email: andreas@thalhammer.bayern
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
@@ -20,66 +18,105 @@
 
 ![example workflow](https://github.com/athalhammer/erdi8/actions/workflows/unit_tests.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/erdi8)](https://pypi.org/project/erdi8)
 [![GitHub license](https://img.shields.io/github/license/athalhammer/erdi8.svg)](https://github.com/athalhammer/erdi8/blob/master/LICENSE)
 
 # erdi8
 
-erdi8 is a [unique identifier](https://www.wikidata.org/wiki/Q6545185) scheme and counter that operates on the following alphabet:
+erdi8 is a [unique identifier](https://www.wikidata.org/wiki/Q6545185) scheme and identifier generator that counts with the following alphabet:
 
 ```
 ['2', '3', '4', '5', '6', '7', '8', '9', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 
 'i', 'j', 'k', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
 ```
 
 It is basically a base36 alphabet that intentionally avoids the ambiguous characters `[0, 1, and l]` and therefore shrinks to 33. In addition to that, it ensures that no identifier starts with a numeric value by using an offset of 8. The zero is represented by 'a', 25 is represented by 'a2', etc. With three characters or less one can create 28'075 (25 + 25 * 33 + 25 * 33 * 33) different identifiers. With 6 characters or less we have 1'008'959'350 options. In a traditional identifier world, one would use a prefix, e.g. M, and then an integer. This only gives you 100k identifiers (M0 to M99999) with up to 6 characters. The scheme enables consecutive counting and is therefore free of collisions. In particular, it is __not__ a method to create secret identifiers.
 
 ## Usage
 
 
-### Basic
+### Basic (counting)
 ```
 $ python3
 
 >>> from erdi8 import Erdi8
 >>> e8 = Erdi8()
 >>> e8.increment("erdi8")
 'erdi9'
 >>> e8.decode_int("erdi8")
 6545185
 >>> e8.encode_int(6545185)
 'erdi8'
 ```
 
-### Advanced
+### Advanced (still counting)
 Fixed length "fancy" identifiers with `safe=True` 
 
 ```
 $ python3
 
 >>> from erdi8 import Erdi8
 >>> safe = True
 >>> start = 'b222222222'
->>> seed = 453459956896834
+>>> stride = 30321718760514
 >>> e8 = Erdi8(safe)
->>> e8.increment_fancy(start, seed)
+>>> e8.increment_fancy(start, stride)
 'fmzz7cwc43'
->>> current = e8.increment_fancy('fmzz7cwc43', seed)
+>>> current = e8.increment_fancy('fmzz7cwc43', stride)
 >>> print(current)
 k7zydqrp64
+
+# reverse engineer stride from two consecutive identifiers
+>>> e8.compute_stride('fmzz7cwc43', current)
+{'stride_effective': 30321718760517, 'stride_other_candidates': [30321718760516, 30321718760515, 30321718760514]}
 ```
 
 **NOTE**
 
 0. These sequences may have a "fancy" appearance but __they are not random__. They are perfectly predictable and are designed to "fill up the whole mod space" before previously coined identifiers start re-appearing.
 1. The `safe=True` option helps you to avoid unintended words (i.e. removes the characters `[aeiou]` from the alphabet)
 2. The fancy increment works with fixed lengths. If you work with a length of 10 (like above) You will have `20 * 28^9 = 211'569'119'068'160` options with `safe=True`. If you think you have more things to identify at some point you have two options: a) start directly with more characters or b) check for the start value (in this case `b222222222`) to re-appear - this will be the identifier that will "show up twice" first.
-3. Store the following four parts in a safe place: a) `safe` parameter b) the `start` value c) the `seed` value. On top, keep good track of the `current` value.
+3. Store the following four parts in a safe place: a) `safe` parameter b) the `start` value c) the `stride` value. On top, keep good track of the `current` value.
+
+
+### Advanced (random)
+Also see documentation of Python's integrated [`random`](https://docs.python.org/3/library/random.html) and [`secrets`](https://docs.python.org/3/library/secrets.html) modules, in particular for `random`: "The pseudo-random generators of this module should not be used for security purposes. For security or cryptographic uses, see the `secrets` module". In any case, you should know what you are doing.
+
+`random` module:
+
+```
+$ python3
+
+>>> import random
+>>> from erdi8 import Erdi8
+>>> e8 = Erdi8()
+
+# get random erdi8 identifiers with length 10
+>>> mini, maxi, space = e8.mod_space(10)
+>>> e8.encode_int(random.randint(mini, maxi))
+'vvctyx7c6o'
+```
 
-### More advanced
+`secrets` module:
+
+```
+$ python3
+
+>>> import secrets
+>>> from erdi8 import Erdi8
+>>> e8 = Erdi8()
+
+>>> e8.encode_int(int.from_bytes(secrets.token_bytes()))
+'jtx3i83pii8wo98wzuucu7uag6khrfpabrdn3qrqrxdxauvcgjg'
+
+>>> e8.encode_int(secrets.randbits(256))
+'a53mpn3xntywcbdcvfa932ub34evne9oha8pzoy6ii3ur2e364z'
+```
+
+### Even more advanced
 Run a light-weight erdi8 identifier service via [fasterid](https://github.com/athalhammer/fasterid)
 
 
 ## Test cases
 
 ```
 $ python3 -m unittest test/erdi8_test.py 
@@ -89,18 +126,16 @@
 
 __Why no upper case characters?__
 
 _Because we don't want to `erdi8` to be confused with `Erdi8`._
 
 __Why no start with a number?__
 
-_Because we want to avoid "number-only" identifiers. If we allowed to start with a number, we would have identifiers of the type `42` and `322` which could be mistaken for integers. We could achieve this with a more complex scheme avoiding any number-only combinations (would therefore still allow ids like `2z`, to be investigated)._
+_Because we want to avoid "number-only" identifiers. If we allowed to start with a number, we would have identifiers of the type `42` and `322` which could be mistaken for integers. We could achieve this with a more complex scheme avoiding any number-only combinations (would therefore still allow ids like `2z`, to be investigated). In essence it is important to note that programs like Excel are really creative when transforming input data, for example `08342 -> 8342`, `12e34 -> 12E+34`, `SEPT1 -> Sep-01` etc. erdi8 with the safe option on avoids 99% of these types of issues._
 
 __How about combinations that form actual (bad) words?__
 
 _This depends on the use case and the way erdi8 is used. Therefore, we can recommend to work with filter lists. In addition, an erdi8 object that avoids the `aeiou` characters can be created with `Erdi8(safe=True)`. This shrinks the available character space to 28 and the produced output is not compatible to `Erdi8(safe=False)` (default). The danger that unintended English words are created is lower with this setting.  It is recommended for erdi8 identifiers that are longer than three characters where filter lists start to become impractical._
 
 __How does this relate to binary-to-text encodings such as base32 and base64?__
 
 _erdi8 can be used for a binary-to-text encoding and the basic functions to implement this are provided with `encode_int` and `decode_int`. However, the primary purpose is to provide a short counting scheme for identifiers._
-
-
```

### Comparing `erdi8-0.2.0/setup.py` & `erdi8-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='erdi8',
-    version='0.2.0',
+    version='0.3.0',
     url='https://github.com/athalhammer/erdi8',
     author='Andreas Thalhammer',
     author_email='andreas@thalhammer.bayern',
     description='Count according to lower case alphabet and numbers (without ambiguous 0, 1, and l) and always start with a letter',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['erdi8'],
```

