# Comparing `tmp/pyOpenSSL-23.1.1.tar.gz` & `tmp/pyOpenSSL-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyOpenSSL-23.1.1.tar", last modified: Tue Mar 28 03:09:15 2023, max compression
+gzip compressed data, was "pyOpenSSL-23.2.0.tar", last modified: Wed May 31 03:18:51 2023, max compression
```

## Comparing `pyOpenSSL-23.1.1.tar` & `pyOpenSSL-23.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.759644 pyOpenSSL-23.1.1/
--rw-r--r--   0 pkehrer    (501) staff       (20)      192 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/.coveragerc
--rw-r--r--   0 pkehrer    (501) staff       (20)    19356 2023-03-28 03:07:36.000000 pyOpenSSL-23.1.1/CHANGELOG.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     3337 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     5216 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/CONTRIBUTING.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     1191 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/INSTALL.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)    11358 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/LICENSE
--rw-r--r--   0 pkehrer    (501) staff       (20)      234 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/MANIFEST.in
--rw-r--r--   0 pkehrer    (501) staff       (20)     9962 2023-03-28 03:09:15.759759 pyOpenSSL-23.1.1/PKG-INFO
--rw-r--r--   0 pkehrer    (501) staff       (20)     1822 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/README.rst
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.756333 pyOpenSSL-23.1.1/doc/
--rw-r--r--   0 pkehrer    (501) staff       (20)    31050 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/ChangeLog_old.txt
--rw-r--r--   0 pkehrer    (501) staff       (20)     4602 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/Makefile
--rw-r--r--   0 pkehrer    (501) staff       (20)      126 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/Quotes
--rw-r--r--   0 pkehrer    (501) staff       (20)      131 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/README
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.756539 pyOpenSSL-23.1.1/doc/api/
--rw-r--r--   0 pkehrer    (501) staff       (20)     5230 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/api/crypto.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     8437 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/api/ssl.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)      359 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/api.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)      400 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/backward-compatibility.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)       30 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/changelog.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     8222 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/conf.py
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.756950 pyOpenSSL-23.1.1/doc/images/
--rw-r--r--   0 pkehrer    (501) staff       (20)     3636 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/images/pyopenssl-brand.png
--rw-r--r--   0 pkehrer    (501) staff       (20)      428 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/images/pyopenssl-icon.png
--rw-r--r--   0 pkehrer    (501) staff       (20)     1483 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/images/pyopenssl-logo.png
--rw-r--r--   0 pkehrer    (501) staff       (20)     8486 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/images/pyopenssl.svg
--rw-r--r--   0 pkehrer    (501) staff       (20)      661 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/index.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)       28 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/install.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     3190 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/internals.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     1410 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/introduction.rst
--rw-r--r--   0 pkehrer    (501) staff       (20)     4517 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/doc/make.bat
--rw-r--r--   0 pkehrer    (501) staff       (20)       57 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/pyproject.toml
--rw-r--r--   0 pkehrer    (501) staff       (20)      312 2023-03-28 03:09:15.760071 pyOpenSSL-23.1.1/setup.cfg
--rw-r--r--   0 pkehrer    (501) staff       (20)     3220 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/setup.py
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.753668 pyOpenSSL-23.1.1/src/
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.757755 pyOpenSSL-23.1.1/src/OpenSSL/
--rw-r--r--   0 pkehrer    (501) staff       (20)    96651 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/src/OpenSSL/SSL.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      498 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/src/OpenSSL/__init__.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     3539 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/src/OpenSSL/_util.py
--rw-r--r--   0 pkehrer    (501) staff       (20)   109269 2023-03-28 03:07:36.000000 pyOpenSSL-23.1.1/src/OpenSSL/crypto.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     1049 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/src/OpenSSL/debug.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     1069 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/src/OpenSSL/rand.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      650 2023-03-28 03:07:36.000000 pyOpenSSL-23.1.1/src/OpenSSL/version.py
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.758239 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/
--rw-r--r--   0 pkehrer    (501) staff       (20)     9962 2023-03-28 03:09:15.000000 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 pkehrer    (501) staff       (20)     1007 2023-03-28 03:09:15.000000 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 pkehrer    (501) staff       (20)        1 2023-03-28 03:09:15.000000 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 pkehrer    (501) staff       (20)      114 2023-03-28 03:09:15.000000 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 pkehrer    (501) staff       (20)        8 2023-03-28 03:09:15.000000 pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/top_level.txt
-drwxr-xr-x   0 pkehrer    (501) staff       (20)        0 2023-03-28 03:09:15.759432 pyOpenSSL-23.1.1/tests/
--rw-r--r--   0 pkehrer    (501) staff       (20)      125 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/__init__.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      609 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/conftest.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     1997 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/memdbg.py
--rw-r--r--   0 pkehrer    (501) staff       (20)   173834 2023-03-28 03:07:36.000000 pyOpenSSL-23.1.1/tests/test_crypto.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      225 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/test_debug.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      786 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/test_rand.py
--rw-r--r--   0 pkehrer    (501) staff       (20)   156990 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/test_ssl.py
--rw-r--r--   0 pkehrer    (501) staff       (20)      610 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/test_util.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     4732 2023-03-28 03:07:24.000000 pyOpenSSL-23.1.1/tests/util.py
--rw-r--r--   0 pkehrer    (501) staff       (20)     1853 2023-03-28 03:07:36.000000 pyOpenSSL-23.1.1/tox.ini
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.908732 pyOpenSSL-23.2.0/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      192 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/.coveragerc
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)    19868 2023-05-31 03:17:39.000000 pyOpenSSL-23.2.0/CHANGELOG.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     3337 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     5216 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1191 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/INSTALL.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)    11358 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/LICENSE
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      234 2022-09-16 12:23:19.000000 pyOpenSSL-23.2.0/MANIFEST.in
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)    10454 2023-05-31 03:18:51.908789 pyOpenSSL-23.2.0/PKG-INFO
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1822 2022-09-16 12:23:19.000000 pyOpenSSL-23.2.0/README.rst
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.903849 pyOpenSSL-23.2.0/doc/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)    31050 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/ChangeLog_old.txt
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     4602 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/Makefile
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      126 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/Quotes
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      131 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/README
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.904222 pyOpenSSL-23.2.0/doc/api/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     5230 2022-12-16 03:25:25.000000 pyOpenSSL-23.2.0/doc/api/crypto.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     8437 2022-09-16 13:13:45.000000 pyOpenSSL-23.2.0/doc/api/ssl.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      359 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/api.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      400 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/backward-compatibility.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)       30 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/changelog.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     8252 2023-04-29 01:22:33.000000 pyOpenSSL-23.2.0/doc/conf.py
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.904929 pyOpenSSL-23.2.0/doc/images/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     3636 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/images/pyopenssl-brand.png
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      428 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/images/pyopenssl-icon.png
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1483 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/images/pyopenssl-logo.png
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     8486 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/images/pyopenssl.svg
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      661 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/index.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)       28 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/install.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     3190 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/internals.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1410 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/introduction.rst
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     4517 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/doc/make.bat
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)       57 2021-12-03 00:57:58.000000 pyOpenSSL-23.2.0/pyproject.toml
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      313 2023-05-31 03:18:51.909044 pyOpenSSL-23.2.0/setup.cfg
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     3316 2023-05-31 03:17:39.000000 pyOpenSSL-23.2.0/setup.py
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.898550 pyOpenSSL-23.2.0/src/
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.906333 pyOpenSSL-23.2.0/src/OpenSSL/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)   101432 2023-04-29 01:22:33.000000 pyOpenSSL-23.2.0/src/OpenSSL/SSL.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      498 2022-03-12 21:19:41.000000 pyOpenSSL-23.2.0/src/OpenSSL/__init__.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     3539 2022-09-16 12:23:19.000000 pyOpenSSL-23.2.0/src/OpenSSL/_util.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)   109453 2023-04-29 01:22:33.000000 pyOpenSSL-23.2.0/src/OpenSSL/crypto.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1049 2022-03-12 21:19:41.000000 pyOpenSSL-23.2.0/src/OpenSSL/debug.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1069 2022-09-16 12:23:19.000000 pyOpenSSL-23.2.0/src/OpenSSL/rand.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      650 2023-05-31 03:17:39.000000 pyOpenSSL-23.2.0/src/OpenSSL/version.py
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.906942 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)    10454 2023-05-31 03:18:51.000000 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1007 2023-05-31 03:18:51.000000 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)        1 2023-05-31 03:18:51.000000 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      132 2023-05-31 03:18:51.000000 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)        8 2023-05-31 03:18:51.000000 pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 alex_gaynor   (501) staff       (20)        0 2023-05-31 03:18:51.908609 pyOpenSSL-23.2.0/tests/
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      125 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/tests/__init__.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      609 2021-11-14 22:39:04.000000 pyOpenSSL-23.2.0/tests/conftest.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1997 2022-03-12 21:19:41.000000 pyOpenSSL-23.2.0/tests/memdbg.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)   173737 2023-05-31 03:17:39.000000 pyOpenSSL-23.2.0/tests/test_crypto.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      225 2022-03-12 21:19:41.000000 pyOpenSSL-23.2.0/tests/test_debug.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      786 2022-01-30 17:32:02.000000 pyOpenSSL-23.2.0/tests/test_rand.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)   156991 2023-05-31 03:17:39.000000 pyOpenSSL-23.2.0/tests/test_ssl.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)      610 2022-01-30 17:32:02.000000 pyOpenSSL-23.2.0/tests/test_util.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     4732 2022-01-30 17:32:02.000000 pyOpenSSL-23.2.0/tests/util.py
+-rw-r--r--   0 alex_gaynor   (501) staff       (20)     1737 2023-04-29 01:22:33.000000 pyOpenSSL-23.2.0/tox.ini
```

### Comparing `pyOpenSSL-23.1.1/CHANGELOG.rst` & `pyOpenSSL-23.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 Changelog
 =========
 
 Versions are year-based with a strict backward-compatibility policy.
 The third digit is only for regressions.
 
+23.2.0 (2023-05-30)
+-------------------
+
+Backward-incompatible changes:
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Removed ``X509StoreFlags.NOTIFY_POLICY``.
+  `#1213 <https://github.com/pyca/pyopenssl/pull/1213>`_.
+
+Deprecations:
+^^^^^^^^^^^^^
+
+Changes:
+^^^^^^^^
+
+- ``cryptography`` maximum version has been increased to 41.0.x.
+- Invalid versions are now rejected in ``OpenSSL.crypto.X509Req.set_version``.
+- Added ``X509VerificationCodes`` to ``OpenSSL.SSL``.
+  `#1202 <https://github.com/pyca/pyopenssl/pull/1202>`_.
+
 23.1.1 (2023-03-28)
 -------------------
 
 Backward-incompatible changes:
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Deprecations:
```

### Comparing `pyOpenSSL-23.1.1/CODE_OF_CONDUCT.rst` & `pyOpenSSL-23.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/CONTRIBUTING.rst` & `pyOpenSSL-23.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/INSTALL.rst` & `pyOpenSSL-23.2.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/LICENSE` & `pyOpenSSL-23.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/PKG-INFO` & `pyOpenSSL-23.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyOpenSSL
-Version: 23.1.1
+Version: 23.2.0
 Summary: Python wrapper module around the OpenSSL library
 Home-page: https://pyopenssl.org/
 Author: The pyOpenSSL developers
 Author-email: cryptography-dev@python.org
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/pyca/pyopenssl
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -78,14 +77,34 @@
 .. _GitHub: https://github.com/pyca/pyopenssl
 .. _`pyca/cryptography`: https://github.com/pyca/cryptography
 
 
 Release Information
 ===================
 
+23.2.0 (2023-05-30)
+-------------------
+
+Backward-incompatible changes:
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Removed ``X509StoreFlags.NOTIFY_POLICY``.
+  `#1213 <https://github.com/pyca/pyopenssl/pull/1213>`_.
+
+Deprecations:
+^^^^^^^^^^^^^
+
+Changes:
+^^^^^^^^
+
+- ``cryptography`` maximum version has been increased to 41.0.x.
+- Invalid versions are now rejected in ``OpenSSL.crypto.X509Req.set_version``.
+- Added ``X509VerificationCodes`` to ``OpenSSL.SSL``.
+  `#1202 <https://github.com/pyca/pyopenssl/pull/1202>`_.
+
 23.1.1 (2023-03-28)
 -------------------
 
 Backward-incompatible changes:
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Deprecations:
@@ -282,9 +301,7 @@
 - Support ``bytearray`` in ``SSL.Connection.send()`` by using cffi's from_buffer.
   `#852 <https://github.com/pyca/pyopenssl/pull/852>`_
 - The ``OpenSSL.SSL.Context.set_alpn_select_callback`` can return a new ``NO_OVERLAPPING_PROTOCOLS`` sentinel value
   to allow a TLS handshake to complete without an application protocol.
 
 `Full changelog <https://pyopenssl.org/en/stable/changelog.html>`_.
 
-
-
```

### Comparing `pyOpenSSL-23.1.1/README.rst` & `pyOpenSSL-23.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/ChangeLog_old.txt` & `pyOpenSSL-23.2.0/doc/ChangeLog_old.txt`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/Makefile` & `pyOpenSSL-23.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/api/crypto.rst` & `pyOpenSSL-23.2.0/doc/api/crypto.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/api/ssl.rst` & `pyOpenSSL-23.2.0/doc/api/ssl.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/conf.py` & `pyOpenSSL-23.2.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,10 +247,10 @@
 # -- Options for manual page output -------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [("index", "pyopenssl", "pyOpenSSL Documentation", [authors], 1)]
 
 intersphinx_mapping = {
-    "https://docs.python.org/3": None,
-    "https://cryptography.io/en/latest/": None,
+    "python": ("https://docs.python.org/3", None),
+    "cryptography": ("https://cryptography.io/en/latest/", None),
 }
```

### Comparing `pyOpenSSL-23.1.1/doc/images/pyopenssl-brand.png` & `pyOpenSSL-23.2.0/doc/images/pyopenssl-brand.png`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/images/pyopenssl-logo.png` & `pyOpenSSL-23.2.0/doc/images/pyopenssl-logo.png`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/images/pyopenssl.svg` & `pyOpenSSL-23.2.0/doc/images/pyopenssl.svg`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/index.rst` & `pyOpenSSL-23.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/internals.rst` & `pyOpenSSL-23.2.0/doc/internals.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/introduction.rst` & `pyOpenSSL-23.2.0/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/doc/make.bat` & `pyOpenSSL-23.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/setup.py` & `pyOpenSSL-23.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             "Topic :: System :: Networking",
         ],
         python_requires=">=3.6",
         packages=find_packages(where="src"),
         package_dir={"": "src"},
         install_requires=[
             # Fix cryptographyMinimum in tox.ini when changing this!
-            "cryptography>=38.0.0,<41",
+            # 40.0.0 and .1 are missing X509_V_* constants that we re-export.
+            "cryptography>=38.0.0,<42,!=40.0.0,!=40.0.1",
         ],
         extras_require={
             "test": ["flaky", "pretend", "pytest>=3.0.1"],
             "docs": ["sphinx!=5.2.0,!=5.2.0.post0", "sphinx_rtd_theme"],
         },
     )
```

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/SSL.py` & `pyOpenSSL-23.2.0/src/OpenSSL/SSL.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     "ZeroReturnError",
     "SysCallError",
     "NO_OVERLAPPING_PROTOCOLS",
     "SSLeay_version",
     "Session",
     "Context",
     "Connection",
+    "X509VerificationCodes",
 ]
 
 
 OPENSSL_VERSION_NUMBER = _lib.OPENSSL_VERSION_NUMBER
 OPENSSL_VERSION = SSLEAY_VERSION = _lib.OPENSSL_VERSION
 OPENSSL_CFLAGS = SSLEAY_CFLAGS = _lib.OPENSSL_CFLAGS
 OPENSSL_PLATFORM = SSLEAY_PLATFORM = _lib.OPENSSL_PLATFORM
@@ -246,14 +247,121 @@
 SSL_CB_ACCEPT_LOOP = _lib.SSL_CB_ACCEPT_LOOP
 SSL_CB_ACCEPT_EXIT = _lib.SSL_CB_ACCEPT_EXIT
 SSL_CB_CONNECT_LOOP = _lib.SSL_CB_CONNECT_LOOP
 SSL_CB_CONNECT_EXIT = _lib.SSL_CB_CONNECT_EXIT
 SSL_CB_HANDSHAKE_START = _lib.SSL_CB_HANDSHAKE_START
 SSL_CB_HANDSHAKE_DONE = _lib.SSL_CB_HANDSHAKE_DONE
 
+
+class X509VerificationCodes:
+    """
+    Success and error codes for X509 verification, as returned by the
+    underlying ``X509_STORE_CTX_get_error()`` function and passed by pyOpenSSL
+    to verification callback functions.
+
+    See `OpenSSL Verification Errors
+    <https://www.openssl.org/docs/manmaster/man3/X509_verify_cert_error_string.html#ERROR-CODES>`_
+    for details.
+    """
+
+    OK = _lib.X509_V_OK
+    ERR_UNABLE_TO_GET_ISSUER_CERT = _lib.X509_V_ERR_UNABLE_TO_GET_ISSUER_CERT
+    ERR_UNABLE_TO_GET_CRL = _lib.X509_V_ERR_UNABLE_TO_GET_CRL
+    ERR_UNABLE_TO_DECRYPT_CERT_SIGNATURE = (
+        _lib.X509_V_ERR_UNABLE_TO_DECRYPT_CERT_SIGNATURE
+    )
+    ERR_UNABLE_TO_DECRYPT_CRL_SIGNATURE = (
+        _lib.X509_V_ERR_UNABLE_TO_DECRYPT_CRL_SIGNATURE
+    )
+    ERR_UNABLE_TO_DECODE_ISSUER_PUBLIC_KEY = (
+        _lib.X509_V_ERR_UNABLE_TO_DECODE_ISSUER_PUBLIC_KEY
+    )
+    ERR_CERT_SIGNATURE_FAILURE = _lib.X509_V_ERR_CERT_SIGNATURE_FAILURE
+    ERR_CRL_SIGNATURE_FAILURE = _lib.X509_V_ERR_CRL_SIGNATURE_FAILURE
+    ERR_CERT_NOT_YET_VALID = _lib.X509_V_ERR_CERT_NOT_YET_VALID
+    ERR_CERT_HAS_EXPIRED = _lib.X509_V_ERR_CERT_HAS_EXPIRED
+    ERR_CRL_NOT_YET_VALID = _lib.X509_V_ERR_CRL_NOT_YET_VALID
+    ERR_CRL_HAS_EXPIRED = _lib.X509_V_ERR_CRL_HAS_EXPIRED
+    ERR_ERROR_IN_CERT_NOT_BEFORE_FIELD = (
+        _lib.X509_V_ERR_ERROR_IN_CERT_NOT_BEFORE_FIELD
+    )
+    ERR_ERROR_IN_CERT_NOT_AFTER_FIELD = (
+        _lib.X509_V_ERR_ERROR_IN_CERT_NOT_AFTER_FIELD
+    )
+    ERR_ERROR_IN_CRL_LAST_UPDATE_FIELD = (
+        _lib.X509_V_ERR_ERROR_IN_CRL_LAST_UPDATE_FIELD
+    )
+    ERR_ERROR_IN_CRL_NEXT_UPDATE_FIELD = (
+        _lib.X509_V_ERR_ERROR_IN_CRL_NEXT_UPDATE_FIELD
+    )
+    ERR_OUT_OF_MEM = _lib.X509_V_ERR_OUT_OF_MEM
+    ERR_DEPTH_ZERO_SELF_SIGNED_CERT = (
+        _lib.X509_V_ERR_DEPTH_ZERO_SELF_SIGNED_CERT
+    )
+    ERR_SELF_SIGNED_CERT_IN_CHAIN = _lib.X509_V_ERR_SELF_SIGNED_CERT_IN_CHAIN
+    ERR_UNABLE_TO_GET_ISSUER_CERT_LOCALLY = (
+        _lib.X509_V_ERR_UNABLE_TO_GET_ISSUER_CERT_LOCALLY
+    )
+    ERR_UNABLE_TO_VERIFY_LEAF_SIGNATURE = (
+        _lib.X509_V_ERR_UNABLE_TO_VERIFY_LEAF_SIGNATURE
+    )
+    ERR_CERT_CHAIN_TOO_LONG = _lib.X509_V_ERR_CERT_CHAIN_TOO_LONG
+    ERR_CERT_REVOKED = _lib.X509_V_ERR_CERT_REVOKED
+    ERR_INVALID_CA = _lib.X509_V_ERR_INVALID_CA
+    ERR_PATH_LENGTH_EXCEEDED = _lib.X509_V_ERR_PATH_LENGTH_EXCEEDED
+    ERR_INVALID_PURPOSE = _lib.X509_V_ERR_INVALID_PURPOSE
+    ERR_CERT_UNTRUSTED = _lib.X509_V_ERR_CERT_UNTRUSTED
+    ERR_CERT_REJECTED = _lib.X509_V_ERR_CERT_REJECTED
+    ERR_SUBJECT_ISSUER_MISMATCH = _lib.X509_V_ERR_SUBJECT_ISSUER_MISMATCH
+    ERR_AKID_SKID_MISMATCH = _lib.X509_V_ERR_AKID_SKID_MISMATCH
+    ERR_AKID_ISSUER_SERIAL_MISMATCH = (
+        _lib.X509_V_ERR_AKID_ISSUER_SERIAL_MISMATCH
+    )
+    ERR_KEYUSAGE_NO_CERTSIGN = _lib.X509_V_ERR_KEYUSAGE_NO_CERTSIGN
+    ERR_UNABLE_TO_GET_CRL_ISSUER = _lib.X509_V_ERR_UNABLE_TO_GET_CRL_ISSUER
+    ERR_UNHANDLED_CRITICAL_EXTENSION = (
+        _lib.X509_V_ERR_UNHANDLED_CRITICAL_EXTENSION
+    )
+    ERR_KEYUSAGE_NO_CRL_SIGN = _lib.X509_V_ERR_KEYUSAGE_NO_CRL_SIGN
+    ERR_UNHANDLED_CRITICAL_CRL_EXTENSION = (
+        _lib.X509_V_ERR_UNHANDLED_CRITICAL_CRL_EXTENSION
+    )
+    ERR_INVALID_NON_CA = _lib.X509_V_ERR_INVALID_NON_CA
+    ERR_PROXY_PATH_LENGTH_EXCEEDED = _lib.X509_V_ERR_PROXY_PATH_LENGTH_EXCEEDED
+    ERR_KEYUSAGE_NO_DIGITAL_SIGNATURE = (
+        _lib.X509_V_ERR_KEYUSAGE_NO_DIGITAL_SIGNATURE
+    )
+    ERR_PROXY_CERTIFICATES_NOT_ALLOWED = (
+        _lib.X509_V_ERR_PROXY_CERTIFICATES_NOT_ALLOWED
+    )
+    ERR_INVALID_EXTENSION = _lib.X509_V_ERR_INVALID_EXTENSION
+    ERR_INVALID_POLICY_EXTENSION = _lib.X509_V_ERR_INVALID_POLICY_EXTENSION
+    ERR_NO_EXPLICIT_POLICY = _lib.X509_V_ERR_NO_EXPLICIT_POLICY
+    ERR_DIFFERENT_CRL_SCOPE = _lib.X509_V_ERR_DIFFERENT_CRL_SCOPE
+    ERR_UNSUPPORTED_EXTENSION_FEATURE = (
+        _lib.X509_V_ERR_UNSUPPORTED_EXTENSION_FEATURE
+    )
+    ERR_UNNESTED_RESOURCE = _lib.X509_V_ERR_UNNESTED_RESOURCE
+    ERR_PERMITTED_VIOLATION = _lib.X509_V_ERR_PERMITTED_VIOLATION
+    ERR_EXCLUDED_VIOLATION = _lib.X509_V_ERR_EXCLUDED_VIOLATION
+    ERR_SUBTREE_MINMAX = _lib.X509_V_ERR_SUBTREE_MINMAX
+    ERR_UNSUPPORTED_CONSTRAINT_TYPE = (
+        _lib.X509_V_ERR_UNSUPPORTED_CONSTRAINT_TYPE
+    )
+    ERR_UNSUPPORTED_CONSTRAINT_SYNTAX = (
+        _lib.X509_V_ERR_UNSUPPORTED_CONSTRAINT_SYNTAX
+    )
+    ERR_UNSUPPORTED_NAME_SYNTAX = _lib.X509_V_ERR_UNSUPPORTED_NAME_SYNTAX
+    ERR_CRL_PATH_VALIDATION_ERROR = _lib.X509_V_ERR_CRL_PATH_VALIDATION_ERROR
+    ERR_HOSTNAME_MISMATCH = _lib.X509_V_ERR_HOSTNAME_MISMATCH
+    ERR_EMAIL_MISMATCH = _lib.X509_V_ERR_EMAIL_MISMATCH
+    ERR_IP_ADDRESS_MISMATCH = _lib.X509_V_ERR_IP_ADDRESS_MISMATCH
+    ERR_APPLICATION_VERIFICATION = _lib.X509_V_ERR_APPLICATION_VERIFICATION
+
+
 # Taken from https://golang.org/src/crypto/x509/root_linux.go
 _CERTIFICATE_FILE_LOCATIONS = [
     "/etc/ssl/certs/ca-certificates.crt",  # Debian/Ubuntu/Gentoo etc.
     "/etc/pki/tls/certs/ca-bundle.crt",  # Fedora/RHEL 6
     "/etc/ssl/ca-bundle.pem",  # OpenSUSE
     "/etc/pki/tls/cacert.pem",  # OpenELEC
     "/etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem",  # CentOS/RHEL 7
```

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/_util.py` & `pyOpenSSL-23.2.0/src/OpenSSL/_util.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/crypto.py` & `pyOpenSSL-23.2.0/src/OpenSSL/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1006,14 +1006,20 @@
         """
         Set the version subfield (RFC 2986, section 4.1) of the certificate
         request.
 
         :param int version: The version number.
         :return: ``None``
         """
+        if not isinstance(version, int):
+            raise TypeError("version must be an int")
+        if version != 0:
+            raise ValueError(
+                "Invalid version. The only valid version for X509Req is 0."
+            )
         set_result = _lib.X509_REQ_set_version(self._req, version)
         _openssl_assert(set_result == 1)
 
     def get_version(self) -> int:
         """
         Get the version subfield (RFC 2459, section 4.1.2.1) of the certificate
         request.
@@ -1635,15 +1641,14 @@
     CRL_CHECK_ALL: int = _lib.X509_V_FLAG_CRL_CHECK_ALL
     IGNORE_CRITICAL: int = _lib.X509_V_FLAG_IGNORE_CRITICAL
     X509_STRICT: int = _lib.X509_V_FLAG_X509_STRICT
     ALLOW_PROXY_CERTS: int = _lib.X509_V_FLAG_ALLOW_PROXY_CERTS
     POLICY_CHECK: int = _lib.X509_V_FLAG_POLICY_CHECK
     EXPLICIT_POLICY: int = _lib.X509_V_FLAG_EXPLICIT_POLICY
     INHIBIT_MAP: int = _lib.X509_V_FLAG_INHIBIT_MAP
-    NOTIFY_POLICY: int = _lib.X509_V_FLAG_NOTIFY_POLICY
     CHECK_SS_SIGNATURE: int = _lib.X509_V_FLAG_CHECK_SS_SIGNATURE
     PARTIAL_CHAIN: int = _lib.X509_V_FLAG_PARTIAL_CHAIN
 
 
 class X509Store:
     """
     An X.509 store.
```

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/debug.py` & `pyOpenSSL-23.2.0/src/OpenSSL/debug.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/rand.py` & `pyOpenSSL-23.2.0/src/OpenSSL/rand.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/src/OpenSSL/version.py` & `pyOpenSSL-23.2.0/src/OpenSSL/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "__license__",
     "__summary__",
     "__title__",
     "__uri__",
     "__version__",
 ]
 
-__version__ = "23.1.1"
+__version__ = "23.2.0"
 
 __title__ = "pyOpenSSL"
 __uri__ = "https://pyopenssl.org/"
 __summary__ = "Python wrapper module around the OpenSSL library"
 __author__ = "The pyOpenSSL developers"
 __email__ = "cryptography-dev@python.org"
 __license__ = "Apache License, Version 2.0"
```

### Comparing `pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/PKG-INFO` & `pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyOpenSSL
-Version: 23.1.1
+Version: 23.2.0
 Summary: Python wrapper module around the OpenSSL library
 Home-page: https://pyopenssl.org/
 Author: The pyOpenSSL developers
 Author-email: cryptography-dev@python.org
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/pyca/pyopenssl
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -78,14 +77,34 @@
 .. _GitHub: https://github.com/pyca/pyopenssl
 .. _`pyca/cryptography`: https://github.com/pyca/cryptography
 
 
 Release Information
 ===================
 
+23.2.0 (2023-05-30)
+-------------------
+
+Backward-incompatible changes:
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Removed ``X509StoreFlags.NOTIFY_POLICY``.
+  `#1213 <https://github.com/pyca/pyopenssl/pull/1213>`_.
+
+Deprecations:
+^^^^^^^^^^^^^
+
+Changes:
+^^^^^^^^
+
+- ``cryptography`` maximum version has been increased to 41.0.x.
+- Invalid versions are now rejected in ``OpenSSL.crypto.X509Req.set_version``.
+- Added ``X509VerificationCodes`` to ``OpenSSL.SSL``.
+  `#1202 <https://github.com/pyca/pyopenssl/pull/1202>`_.
+
 23.1.1 (2023-03-28)
 -------------------
 
 Backward-incompatible changes:
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Deprecations:
@@ -282,9 +301,7 @@
 - Support ``bytearray`` in ``SSL.Connection.send()`` by using cffi's from_buffer.
   `#852 <https://github.com/pyca/pyopenssl/pull/852>`_
 - The ``OpenSSL.SSL.Context.set_alpn_select_callback`` can return a new ``NO_OVERLAPPING_PROTOCOLS`` sentinel value
   to allow a TLS handshake to complete without an application protocol.
 
 `Full changelog <https://pyopenssl.org/en/stable/changelog.html>`_.
 
-
-
```

### Comparing `pyOpenSSL-23.1.1/src/pyOpenSSL.egg-info/SOURCES.txt` & `pyOpenSSL-23.2.0/src/pyOpenSSL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tests/conftest.py` & `pyOpenSSL-23.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tests/memdbg.py` & `pyOpenSSL-23.2.0/tests/memdbg.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tests/test_crypto.py` & `pyOpenSSL-23.2.0/tests/test_crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # See LICENSE file for details.
 
 """
 Unit tests for :py:mod:`OpenSSL.crypto`.
 """
 import base64
 import sys
+import warnings
 from datetime import datetime, timedelta
 from subprocess import PIPE, Popen
-from warnings import simplefilter
 
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ec, ed25519, ed448, rsa
 
 import flaky
 
@@ -46,22 +46,23 @@
     dump_privatekey,
     dump_publickey,
     get_elliptic_curve,
     get_elliptic_curves,
     load_certificate,
     load_certificate_request,
     load_crl,
-    load_pkcs12,
-    load_pkcs7_data,
     load_privatekey,
     load_publickey,
     sign,
     verify,
 )
 
+with pytest.warns(DeprecationWarning):
+    from OpenSSL.crypto import load_pkcs12, load_pkcs7_data
+
 from .util import (
     EqualityTestsMixin,
     NON_ASCII,
     WARNING_TYPE_EXPECTED,
     is_consistent_type,
 )
 
@@ -1597,37 +1598,31 @@
         request = X509Req()
         assert isinstance(request, X509Req)
 
     def test_version(self):
         """
         `X509Req.set_version` sets the X.509 version of the certificate
         request. `X509Req.get_version` returns the X.509 version of the
-        certificate request. The only defined version is 0. Others may or
-        may not be supported depending on backend.
+        certificate request. The only defined version is 0.
         """
         request = X509Req()
         assert request.get_version() == 0
         request.set_version(0)
         assert request.get_version() == 0
-        try:
-            request.set_version(1)
-            assert request.get_version() == 1
-            request.set_version(3)
-            assert request.get_version() == 3
-        except Error:
-            pass
 
     def test_version_wrong_args(self):
         """
         `X509Req.set_version` raises `TypeError` if called with a non-`int`
         argument.
         """
         request = X509Req()
         with pytest.raises(TypeError):
             request.set_version("foo")
+        with pytest.raises(ValueError):
+            request.set_version(2)
 
     def test_get_subject(self):
         """
         `X509Req.get_subject` returns an `X509Name` for the subject of the
         request and which is valid even after the request object is
         otherwise dead.
         """
@@ -2606,15 +2601,15 @@
             b"pkcs12",
             b"-export",
             b"-clcerts",
             b"-passout",
             b"pass:" + passwd,
         )
         with pytest.warns(DeprecationWarning) as w:
-            simplefilter("always")
+            warnings.simplefilter("always")
             p12 = load_pkcs12(p12_str, passphrase=b"whatever".decode("ascii"))
             msg = "{0} for passphrase is no longer accepted, use bytes".format(
                 WARNING_TYPE_EXPECTED
             )
             assert msg == str(w[-1].message)
 
         self.verify_pkcs12_container(p12)
@@ -2825,15 +2820,15 @@
     def test_export_without_bytes(self):
         """
         Test `PKCS12.export` with text not bytes as passphrase
         """
         p12 = self.gen_pkcs12(server_cert_pem, server_key_pem, root_cert_pem)
 
         with pytest.warns(DeprecationWarning) as w:
-            simplefilter("always")
+            warnings.simplefilter("always")
             dumped_p12 = p12.export(passphrase=b"randomtext".decode("ascii"))
             msg = "{0} for passphrase is no longer accepted, use bytes".format(
                 WARNING_TYPE_EXPECTED
             )
             assert msg == str(w[-1].message)
         self.check_recovery(
             dumped_p12,
@@ -3680,16 +3675,16 @@
 
     def test_export_md5_digest(self):
         """
         If passed md5 as the digest function, ``CRL.export`` uses md5 and does
         not emit a deprecation warning.
         """
         crl = self._get_crl()
-        with pytest.warns(None) as catcher:
-            simplefilter("always")
+        with warnings.catch_warnings(record=True) as catcher:
+            warnings.simplefilter("always")
         assert 0 == len(catcher)
         dumped_crl = crl.export(self.cert, self.pkey, digest=b"md5")
         text = _runopenssl(dumped_crl, b"crl", b"-noout", b"-text")
         text.index(b"Signature Algorithm: md5")
 
     def test_export_default_digest(self):
         """
@@ -4370,22 +4365,22 @@
             b"prevent a swirl of gritty dust from entering along with him."
         ).decode("ascii")
 
         priv_key = load_privatekey(FILETYPE_PEM, root_key_pem)
         cert = load_certificate(FILETYPE_PEM, root_cert_pem)
         for digest in ["md5", "sha1", "sha256"]:
             with pytest.warns(DeprecationWarning) as w:
-                simplefilter("always")
+                warnings.simplefilter("always")
                 sig = sign(priv_key, content, digest)
             assert "{0} for data is no longer accepted, use bytes".format(
                 WARNING_TYPE_EXPECTED
             ) == str(w[-1].message)
 
             with pytest.warns(DeprecationWarning) as w:
-                simplefilter("always")
+                warnings.simplefilter("always")
                 verify(cert, sig, content, digest)
             assert "{0} for data is no longer accepted, use bytes".format(
                 WARNING_TYPE_EXPECTED
             ) == str(w[-1].message)
 
     def test_sign_verify_ecdsa(self):
         """
```

### Comparing `pyOpenSSL-23.1.1/tests/test_rand.py` & `pyOpenSSL-23.2.0/tests/test_rand.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tests/test_ssl.py` & `pyOpenSSL-23.2.0/tests/test_ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2765,15 +2765,15 @@
         re-use the session it represents when the SSL handshake is performed.
         """
         key = load_privatekey(FILETYPE_PEM, server_key_pem)
         cert = load_certificate(FILETYPE_PEM, server_cert_pem)
         ctx = Context(TLSv1_2_METHOD)
         ctx.use_privatekey(key)
         ctx.use_certificate(cert)
-        ctx.set_session_id("unity-test")
+        ctx.set_session_id(b"unity-test")
 
         def makeServer(socket):
             server = Connection(ctx, socket)
             server.set_accept_state()
             return server
 
         originalServer, originalClient = loopback(server_factory=makeServer)
```

### Comparing `pyOpenSSL-23.1.1/tests/test_util.py` & `pyOpenSSL-23.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tests/util.py` & `pyOpenSSL-23.2.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `pyOpenSSL-23.1.1/tox.ini` & `pyOpenSSL-23.2.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py{py,py3,36,37,38,39,310,311}{,-cryptographyMain,-cryptographyMinimum}{,-useWheel}{,-randomorder},py37-twistedTrunk,check-manifest,flake8,py36-mypy,docs,coverage-report
+envlist = py{py,py3,36,37,38,39,310,311}{,-cryptographyMinimum}{,-useWheel}{,-randomorder},py311-twistedTrunk,check-manifest,flake8,py311-mypy,docs,coverage-report
 
 [testenv]
 allowlist_externals =
     openssl
 passenv =
     ARCHFLAGS
     CFLAGS
@@ -14,51 +14,51 @@
     TERM
     RUSTUP_TOOLCHAIN
     RUSTUP_HOME
 extras =
     test
 deps =
     coverage>=4.2
-    cryptographyMain: git+https://github.com/pyca/cryptography.git
     cryptographyMinimum: cryptography==38.0.0
     randomorder: pytest-randomly
 setenv =
     # Do not allow the executing environment to pollute the test environment
     # with extra packages.
     PYTHONPATH=
     PIP_NO_BINARY=cryptography
     useWheel: PIP_NO_BINARY=
 commands =
+    cryptographyMain: pip install -U git+https://github.com/pyca/cryptography.git
     openssl version
     coverage run --parallel -m OpenSSL.debug
     coverage run --parallel -m pytest -v {posargs}
 
-[testenv:py37-twistedTrunk]
+[testenv:py311-twistedTrunk]
 deps =
+    pyasn1!=0.5.0
     Twisted[all_non_platform] @ git+https://github.com/twisted/twisted
 setenv =
 commands =
-    python -c "import OpenSSL.SSL; print(OpenSSL.SSL.SSLeay_version(OpenSSL.SSL.SSLEAY_VERSION))"
-    python -c "import cryptography; print(cryptography.__version__)"
-    python -m twisted.trial --reporter=text twisted
+    python -m OpenSSL.debug
+    python -m twisted.trial -j4 --reporter=text twisted
 
 [testenv:flake8]
 basepython = python3
 deps =
     black
     flake8
     flake8-import-order
 skip_install = true
 commands =
     black --check .
     flake8 .
 
-[testenv:py36-mypy]
+[testenv:py311-mypy]
 deps =
-    mypy==0.950
+    mypy==1.1.1
 skip_install = true
 commands =
     mypy src
 
 [testenv:check-manifest]
 deps =
     check-manifest
```

