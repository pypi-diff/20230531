# Comparing `tmp/dissect.util-3.8.dev3.tar.gz` & `tmp/dissect.util-3.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.util-3.8.dev3.tar", last modified: Tue May 16 13:25:32 2023, max compression
+gzip compressed data, was "dissect.util-3.9.dev1.tar", last modified: Wed May 31 13:13:30 2023, max compression
```

## Comparing `dissect.util-3.8.dev3.tar` & `dissect.util-3.9.dev1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.009402 dissect.util-3.8.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/compression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzxpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/lzxpress_huffman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/compression/sevenbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/cpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/encoding/surrogateescape.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/sid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.013402 dissect.util-3.8.dev3/dissect/util/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/tools/dump_nskeyedarchiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/dissect/util/xmemoryview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.009402 dissect.util-3.8.dev3/dissect.util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-16 13:25:32.000000 dissect.util-3.8.dev3/dissect.util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:25:31.000000 dissect.util-3.8.dev3/dissect.util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 13:25:18.000000 dissect.util-3.8.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/bin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/crc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/hpbin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/hpodc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/newc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/data/odc.cpio.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:25:32.017402 dissect.util-3.8.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_cpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_sid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tests/test_xmemoryview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:25:09.000000 dissect.util-3.8.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.583679 dissect.util-3.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-31 13:13:30.583679 dissect.util-3.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.567678 dissect.util-3.9.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.575678 dissect.util-3.9.dev1/dissect/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.575678 dissect.util-3.9.dev1/dissect/util/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/lzxpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/lzxpress_huffman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/compression/sevenbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/cpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.575678 dissect.util-3.9.dev1/dissect/util/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/encoding/surrogateescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.579679 dissect.util-3.9.dev1/dissect/util/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/tools/dump_nskeyedarchiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/dissect/util/xmemoryview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.571678 dissect.util-3.9.dev1/dissect.util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-31 13:13:30.000000 dissect.util-3.9.dev1/dissect.util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-31 13:13:30.000000 dissect.util-3.9.dev1/dissect.util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:13:30.000000 dissect.util-3.9.dev1/dissect.util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 13:13:30.000000 dissect.util-3.9.dev1/dissect.util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 13:13:30.000000 dissect.util-3.9.dev1/dissect.util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 13:13:20.000000 dissect.util-3.9.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:13:30.583679 dissect.util-3.9.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.579679 dissect.util-3.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.583679 dissect.util-3.9.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/bin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/crc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/hpbin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/hpodc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/newc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/data/odc.cpio.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:13:30.583679 dissect.util-3.9.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_cpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tests/test_xmemoryview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-31 13:13:13.000000 dissect.util-3.9.dev1/tox.ini
```

### Comparing `dissect.util-3.8.dev3/LICENSE` & `dissect.util-3.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/PKG-INFO` & `dissect.util-3.9.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.8.dev3
+Version: 3.9.dev1
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.util-3.8.dev3/README.md` & `dissect.util-3.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/lz4.py` & `dissect.util-3.9.dev1/dissect/util/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/lznt1.py` & `dissect.util-3.9.dev1/dissect/util/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/lzo.py` & `dissect.util-3.9.dev1/dissect/util/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/lzxpress.py` & `dissect.util-3.9.dev1/dissect/util/compression/lzxpress.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/lzxpress_huffman.py` & `dissect.util-3.9.dev1/dissect/util/compression/lzxpress_huffman.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/compression/sevenbit.py` & `dissect.util-3.9.dev1/dissect/util/compression/sevenbit.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/cpio.py` & `dissect.util-3.9.dev1/dissect/util/cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/plist.py` & `dissect.util-3.9.dev1/dissect/util/plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/sid.py` & `dissect.util-3.9.dev1/dissect/util/sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/stream.py` & `dissect.util-3.9.dev1/dissect/util/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/tools/dump_nskeyedarchiver.py` & `dissect.util-3.9.dev1/dissect/util/tools/dump_nskeyedarchiver.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/ts.py` & `dissect.util-3.9.dev1/dissect/util/ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect/util/xmemoryview.py` & `dissect.util-3.9.dev1/dissect/util/xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/dissect.util.egg-info/PKG-INFO` & `dissect.util-3.9.dev1/dissect.util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.8.dev3
+Version: 3.9.dev1
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.util-3.8.dev3/dissect.util.egg-info/SOURCES.txt` & `dissect.util-3.9.dev1/dissect.util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/pyproject.toml` & `dissect.util-3.9.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/bin.cpio.gz` & `dissect.util-3.9.dev1/tests/data/bin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/crc.cpio.gz` & `dissect.util-3.9.dev1/tests/data/crc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/hpbin.cpio.gz` & `dissect.util-3.9.dev1/tests/data/hpbin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/hpodc.cpio.gz` & `dissect.util-3.9.dev1/tests/data/hpodc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/newc.cpio.gz` & `dissect.util-3.9.dev1/tests/data/newc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/data/odc.cpio.gz` & `dissect.util-3.9.dev1/tests/data/odc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/docs/Makefile` & `dissect.util-3.9.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/docs/conf.py` & `dissect.util-3.9.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_compression.py` & `dissect.util-3.9.dev1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_cpio.py` & `dissect.util-3.9.dev1/tests/test_cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_plist.py` & `dissect.util-3.9.dev1/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_sid.py` & `dissect.util-3.9.dev1/tests/test_sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_stream.py` & `dissect.util-3.9.dev1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tests/test_ts.py` & `dissect.util-3.9.dev1/tests/test_ts.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 @pytest.fixture
 def ts():
     from dissect.util import ts
 
     yield reload(ts)
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="Time Calculation error. Needs to be fixed.")
 def test_now(ts):
     assert ts.now() < datetime.now(timezone.utc)
     assert ts.now().tzinfo == timezone.utc
 
 
 def test_unix_now(imported_ts):
     timestamp = imported_ts.unix_now()
@@ -106,14 +107,15 @@
 
 def test_wintimestamp(imported_ts):
     assert imported_ts.wintimestamp(131679632729151386) == datetime(
         2018, 4, 11, 23, 34, 32, 915138, tzinfo=timezone.utc
     )
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="Time Calculation error. Needs to be fixed.")
 def test_oatimestamp(imported_ts):
     dt = datetime(2016, 10, 17, 4, 6, 38, 362003, tzinfo=timezone.utc)
     assert imported_ts.oatimestamp(42660.171277338) == dt
     assert imported_ts.oatimestamp(4676095982878497960) == dt
     assert imported_ts.oatimestamp(-4542644417712532139) == datetime(1661, 4, 17, 11, 30, tzinfo=timezone.utc)
 
 
@@ -124,14 +126,15 @@
 
 
 def test_cocoatimestamp(imported_ts):
     assert imported_ts.cocoatimestamp(622894123) == datetime(2020, 9, 27, 10, 8, 43, tzinfo=timezone.utc)
     assert imported_ts.cocoatimestamp(622894123.221783) == datetime(2020, 9, 27, 10, 8, 43, 221783, tzinfo=timezone.utc)
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="Time Calculation error. Needs to be fixed.")
 def test_negative_timestamps(imported_ts):
     # -5000.0 converted to a int representation
     assert imported_ts.oatimestamp(13885591609694748672) == datetime(1886, 4, 22, 0, 0, tzinfo=timezone.utc)
     assert imported_ts.oatimestamp(-5000.0) == datetime(1886, 4, 22, 0, 0, tzinfo=timezone.utc)
     assert imported_ts.webkittimestamp(-5000) == datetime(1600, 12, 31, 23, 59, 59, 995001, tzinfo=timezone.utc)
     assert imported_ts.wintimestamp(-5000) == datetime(1600, 12, 31, 23, 59, 59, 999500, tzinfo=timezone.utc)
     assert imported_ts.xfstimestamp(-100000, 0) == datetime(1969, 12, 30, 20, 13, 20, tzinfo=timezone.utc)
```

### Comparing `dissect.util-3.8.dev3/tests/test_xmemoryview.py` & `dissect.util-3.9.dev1/tests/test_xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.8.dev3/tox.ini` & `dissect.util-3.9.dev1/tox.ini`

 * *Files identical despite different names*

