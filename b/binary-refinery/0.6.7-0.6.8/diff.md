# Comparing `tmp/binary-refinery-0.6.7.tar.gz` & `tmp/binary-refinery-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-nue5hsdn/binary-refinery-0.6.7.tar", last modified: Thu May 25 16:52:04 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-3ww3hmkt/binary-refinery-0.6.8.tar", last modified: Wed May 31 10:28:49 2023, max compression
```

## Comparing `binary-refinery-0.6.7.tar` & `binary-refinery-0.6.8.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34707 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/chaskey.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtgz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/msi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/tnetmtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59251 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19591 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34707 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/chaskey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtgz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/msi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/tnetmtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10672 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/setup.py
```

### Comparing `binary-refinery-0.6.7/LICENSE` & `binary-refinery-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/PKG-INFO` & `binary-refinery-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.7
+Version: 0.6.8
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.7/README.md` & `binary-refinery-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.8/binary_refinery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.7
+Version: 0.6.8
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.7/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.8/binary_refinery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.8/binary_refinery.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.8/binary_refinery.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 pefile
 pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-asn1crypto
-openpyxl
-decompyle3
-Pillow
 pycdlib
-msoffcrypto-tool
 python-registry
-uncompyle6
-javaobj-py3>=0.4.0.1
+decompyle3
+capstone
 pyonenote
-olefile
-LnkParse3
-xdis
+XLMMacroDeobfuscator
+xlrd2
 PyPDF2>=3.0.0
+asn1crypto
+openpyxl
+chardet
+javaobj-py3>=0.4.0.1
+LnkParse3
+uncompyle6
 pyxlsb2
-XLMMacroDeobfuscator
+xdis
 cabarchive
+olefile
 py7zr
-capstone
 phpserialize
-extract-msg
-chardet
 pyperclip
-xlrd2
+extract-msg
+msoffcrypto-tool
+Pillow
 
 [add]
 numpy
 
 [all]
-angr
-numpy
-pyzipper
 pypcapkit[scapy]<0.16.0
+capstone
+pyzipper
+oletools
 intervaltree
+numpy
+angr
 colorama
-oletools
+unicorn
+python-evtx
 jsbeautifier
-capstone
 mitmproxy
 chardet
-python-evtx
-unicorn
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -128,16 +128,16 @@
 oletools
 
 [vmemref]
 angr
 
 [vstack]
 unicorn
-capstone
 intervaltree
+capstone
 
 [xor]
 numpy
 
 [xtrtf]
 oletools
```

### Comparing `binary-refinery-0.6.7/refinery/__init__.pkl` & `binary-refinery-0.6.8/refinery/__init__.pkl`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/__init__.py` & `binary-refinery-0.6.8/refinery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.7/refinery/data/rich.json` & `binary-refinery-0.6.8/refinery/data/rich.json`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/explore.py` & `binary-refinery-0.6.8/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/argformats.py` & `binary-refinery-0.6.8/refinery/lib/argformats.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,23 @@
     def __call__(self, data):
         expression = self.expr
         if pending(expression):
             expression = expression(data).decode('utf8')
         return sliceobj(expression, data)
 
 
+def percent(expression: str):
+    """
+    Allows specification of percentages.
+    """
+    if expression.endswith('%'):
+        return float(expression[:-1].strip()) / 100
+    return float(expression)
+
+
 def sliceobj(expression: Union[int, str, slice], data: Optional[Chunk] = None, range=False, final=False) -> Union[slice, SliceAgain]:
     """
     Uses `refinery.lib.argformats.PythonExpression` to parse slice expressions
     where the bounds can be given as arithmetic expressions. For example, this
     argument format type will process the string `0x11:0x11+4*0x34` as the slice
     object `slice(17, 225, None)`.
     """
```

### Comparing `binary-refinery-0.6.7/refinery/lib/argparser.py` & `binary-refinery-0.6.8/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/chunks.py` & `binary-refinery-0.6.8/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/crypto.py` & `binary-refinery-0.6.8/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/decompression.py` & `binary-refinery-0.6.8/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/decorators.py` & `binary-refinery-0.6.8/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.8/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/dex.py` & `binary-refinery-0.6.8/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.8/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.8/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.8/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.8/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/environment.py` & `binary-refinery-0.6.8/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/executable.py` & `binary-refinery-0.6.8/refinery/lib/executable.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from typing import TYPE_CHECKING, NamedTuple
 from os import devnull as DEVNULL
 from abc import ABC, abstractmethod
 from enum import Enum
 from functools import lru_cache
 
-from macholib.MachO import MachO
+from macholib.MachO import load_command, MachO, MachOHeader
 from pefile import PE as PEFile, SectionStructure, MACHINE_TYPE, DIRECTORY_ENTRY
 from elftools.elf.elffile import ELFFile
 
 from refinery.lib.structures import MemoryFile
 from refinery.lib.types import INF, ByteStr
 
 if TYPE_CHECKING:
@@ -175,14 +175,19 @@
 
 class ET(str, Enum):
     ELF = 'ELF'
     MachO = 'MachO'
     PE = 'PE'
 
 
+class BO(str, Enum):
+    BE = 'big'
+    LE = 'little'
+
+
 class Section(NamedTuple):
     name: str
     physical: Range
     virtual: Range
 
     def as_segment(self, populate_sections=False) -> Segment:
         sections = [self] if populate_sections else None
@@ -347,14 +352,18 @@
                     BoxedOffset(segment.physical, segment.physical.lower + location - segment.virtual.lower),
                     BoxedOffset(segment.virtual, location)
                 )
         else:
             raise CompartmentNotFound(lt, location)
 
     @abstractmethod
+    def byte_order(self) -> BO:
+        ...
+
+    @abstractmethod
     def image_defined_base(self) -> int:
         ...
 
     @abstractmethod
     def arch(self) -> Arch:
         ...
 
@@ -441,14 +450,17 @@
                 'IMAGE_FILE_MACHINE_THUMB'  : Arch.ARM32,
                 'IMAGE_FILE_MACHINE_ARMNT'  : Arch.ARM64,
                 'IMAGE_FILE_MACHINE_MIPS16' : Arch.MIPS16,
             }[arch]
         except KeyError:
             raise LookupError(F'Unsupported architecture: {arch}')
 
+    def byte_order(self) -> BO:
+        return BO.LE
+
 
 class ExecutableELF(Executable):
 
     _head: ELFFile
     _type = ET.ELF
 
     @lru_cache(maxsize=1)
@@ -515,28 +527,33 @@
                 'EM_PPC'     : Arch.PPC32,
                 'EM_PPC64'   : Arch.PPC64,
                 'EM_ARM'     : Arch.ARM32,
             }[arch]
         except KeyError:
             raise LookupError(F'Unsupported architecture: {arch}')
 
+    def byte_order(self) -> BO:
+        return BO.LE if self.head.little_endian else BO.BE
+
 
 class ExecutableMachO(Executable):
 
     _head: MachO
     _type = ET.MachO
 
     @lru_cache(maxsize=1)
     def image_defined_base(self) -> int:
         return min(seg.vmaddr for seg, _ in self._macho_segments() if seg.vmaddr > 0)
 
     def _macho_segments(self):
-        for header in self._head.headers:
-            for header, segment, sections in header.commands:
-                if not header.get_cmd_name().startswith('LC_SEGMENT'):
+        headers: List[MachOHeader] = self._head.headers
+        for header in headers:
+            for cmd, segment, sections in header.commands:
+                cmd: load_command
+                if not cmd.get_cmd_name().startswith('LC_SEGMENT'):
                     continue
                 if segment.filesize <= 0:
                     continue
                 yield segment, sections
 
     def segments(self, populate_sections=False) -> Generator[Segment, None, None]:
         for segment, sections in self._macho_segments():
@@ -591,7 +608,14 @@
                 'ARM'       : Arch.ARM32,
                 'SPARC'     : Arch.SPARC32,
                 'POWERPC'   : Arch.PPC32,
                 'POWERPC64' : Arch.PPC64,
             }[arch]
         except KeyError:
             raise LookupError(F'Unsupported architecture: {arch}')
+
+    def byte_order(self) -> BO:
+        headers: List[MachOHeader] = self._head.headers
+        return {
+            '<': BO.LE,
+            '>': BO.BE,
+        }[headers[0].endian]
```

### Comparing `binary-refinery-0.6.7/refinery/lib/frame.py` & `binary-refinery-0.6.8/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/inline.py` & `binary-refinery-0.6.8/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/java.py` & `binary-refinery-0.6.8/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/json.py` & `binary-refinery-0.6.8/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/loader.py` & `binary-refinery-0.6.8/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/magic.py` & `binary-refinery-0.6.8/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/meta.py` & `binary-refinery-0.6.8/refinery/lib/meta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/mime.py` & `binary-refinery-0.6.8/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/mscrypto.py` & `binary-refinery-0.6.8/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/murmur.py` & `binary-refinery-0.6.8/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.8/refinery/lib/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.8/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/powershell.py` & `binary-refinery-0.6.8/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/ripemd128.py` & `binary-refinery-0.6.8/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/serpent.py` & `binary-refinery-0.6.8/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/structures.py` & `binary-refinery-0.6.8/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/suffixtree.py` & `binary-refinery-0.6.8/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.8/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.8/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.8/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.8/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/tools.py` & `binary-refinery-0.6.8/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/types.py` & `binary-refinery-0.6.8/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/vfs.py` & `binary-refinery-0.6.8/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/lib/xml.py` & `binary-refinery-0.6.8/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/__init__.py` & `binary-refinery-0.6.8/refinery/units/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.8/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.8/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.8/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.8/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/map.py` & `binary-refinery-0.6.8/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.8/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.8/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.8/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.8/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/ap.py` & `binary-refinery-0.6.8/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/blz.py` & `binary-refinery-0.6.8/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/bz2.py` & `binary-refinery-0.6.8/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/decompress.py` & `binary-refinery-0.6.8/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.8/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lz.py` & `binary-refinery-0.6.8/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lz4.py` & `binary-refinery-0.6.8/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lzf.py` & `binary-refinery-0.6.8/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lzg.py` & `binary-refinery-0.6.8/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lzip.py` & `binary-refinery-0.6.8/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.8/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.8/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/lzo.py` & `binary-refinery-0.6.8/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/mscf.py` & `binary-refinery-0.6.8/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/qlz.py` & `binary-refinery-0.6.8/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/szdd.py` & `binary-refinery-0.6.8/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/compression/zl.py` & `binary-refinery-0.6.8/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,31 +73,34 @@
 
 class StreamCipherUnit(CipherUnit, abstract=True):
 
     block_size = 1
 
     def __init__(
         self, key,
+        discard: Arg.Number('-d', help='Discard the first {varname} bytes of the keystream, {default} by default.') = 0,
         stateful: Arg.Switch('-s', help='Do not reset the key stream while processing the chunks of one frame.') = False,
         **keywords
     ):
-        super().__init__(key=key, stateful=stateful, **keywords)
+        super().__init__(key=key, stateful=stateful, discard=discard, **keywords)
         self._keystream = None
 
     @abc.abstractmethod
     def keystream(self) -> Iterable[int]:
         raise NotImplementedError
 
     @Unit.Requires('numpy')
     def _numpy():
         import numpy
         return numpy
 
     def encrypt(self, data: bytearray) -> bytearray:
         it = self._keystream or self.keystream()
+        for _ in range(self.args.discard):
+            next(it)
         try:
             np = self._numpy
         except ImportError:
             self.log_info('this unit could perform faster if numpy was installed.')
             out = bytearray(a ^ b for a, b in zip(it, data))
         else:
             key = np.fromiter(it, dtype=np.uint8, count=len(data))
@@ -358,21 +361,21 @@
 
 
 class LatinCipherUnit(StreamCipherUnit, abstract=True):
     key_size = {16, 32}
     block_size = 1
 
     def __init__(
-        self, key,
+        self, key, stateful=False, discard=0,
         nonce: Arg(help='The nonce. Default is the string {default}.') = B'REFINERY',
         magic: Arg('-m', help='The magic constant; depends on the key size by default.') = B'',
         offset: Arg.Number('-x', help='Optionally specify the stream index, default is {default}.') = 0,
         rounds: Arg.Number('-r', help='The number of rounds. Has to be an even number.') = 20,
     ):
-        super().__init__(key=key, nonce=nonce, magic=magic, offset=offset, rounds=rounds)
+        super().__init__(key=key, nonce=nonce, magic=magic, offset=offset, rounds=rounds, stateful=stateful, discard=discard)
 
 
 class LatinCipherStandardUnit(StandardCipherUnit):
     def __init__(self, key, nonce: Arg(help='The nonce. Default is the string {default}.') = B'REFINERY'):
         super().__init__(key, nonce=nonce)
 
     def _new_cipher(self, **optionals) -> Any:
```

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/chaskey.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/chaskey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rabbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,14 @@
 
 class rabbit(StreamCipherUnit):
     """
     RABBIT encryption and decryption.
     """
     key_size = {16}
 
-    def __init__(self, key, stateful=False, iv: Arg('-i', '--iv', help='Optional initialization vector.') = B''):
-        super().__init__(key=key, iv=iv, stateful=stateful)
+    def __init__(self, key, discard=0, stateful=False, iv: Arg('-i', '--iv', help='Optional initialization vector.') = B''):
+        super().__init__(key=key, iv=iv, stateful=stateful, discard=discard)
 
     def keystream(self) -> Iterable[int]:
         if len(self.args.iv) not in (0, 8):
             raise ValueError('The IV length must be exactly 8 bytes.')
         return RabbitCipher(self.args.key, self.args.iv)
```

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4mod.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 class rc4mod(StreamCipherUnit):
     """
     Implements a modified version of the RC4 stream cipher where the size of the RC4 SBox can be altered.
     """
 
     def __init__(
-        self, key, stateful=False, *,
+        self, key, stateful=False, discard=0, *,
         size: Arg.Number('-t', help='Table size, {default} by default.', bound=(1, None)) = 0x100
     ):
-        super().__init__(key=key, stateful=stateful, size=size)
+        super().__init__(key=key, stateful=stateful, discard=discard, size=size)
 
     def keystream(self):
         size = self.args.size
         tablerange = range(max(size, 0x100))
         b, table = 0, bytearray(k & 0xFF for k in tablerange)
         for a, keybyte in zip(tablerange, cycle(self.args.key)):
             t = table[a]
```

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.8/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.8/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.8/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.8/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/b32.py` & `binary-refinery-0.6.8/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/b64.py` & `binary-refinery-0.6.8/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/base.py` & `binary-refinery-0.6.8/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/esc.py` & `binary-refinery-0.6.8/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/hex.py` & `binary-refinery-0.6.8/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.8/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.8/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/recode.py` & `binary-refinery-0.6.8/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/url.py` & `binary-refinery-0.6.8/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.8/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.8/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/__init__.py` & `binary-refinery-0.6.8/refinery/units/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/a3x.py` & `binary-refinery-0.6.8/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtgz.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtgz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtnode.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtnode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtnsis.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtpyi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.8/refinery/units/formats/archive/xtzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/bat.py` & `binary-refinery-0.6.8/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/csv.py` & `binary-refinery-0.6.8/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.8/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/email.py` & `binary-refinery-0.6.8/refinery/units/formats/email.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/evtx.py` & `binary-refinery-0.6.8/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.8/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.8/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.8/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.8/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.8/refinery/units/formats/exe/vstack.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,28 @@
     from unicorn import Uc
     from intervaltree import IntervalTree, Interval
 
 
 @dataclass
 class EmuState:
     executable: Executable
-    address: int
     writes: IntervalTree
     disassembler: Optional[Cs] = None
     waiting: int = 0
-    calling: bool = False
 
     def disassemble(self, address: int, size: int):
         if self.disassembler is None:
             return None
-        pos = self.executable.location_from_address(address).physical.position
-        end = pos + size
-        return next(self.disassembler.disasm(
-            bytes(self.executable.data[pos:end]), address, 1))
+        try:
+            pos = self.executable.location_from_address(address).physical.position
+            end = pos + size
+            return next(self.disassembler.disasm(
+                bytes(self.executable.data[pos:end]), address, 1))
+        except Exception:
+            return None
 
 
 class vstack(Unit):
     """
     The unit emulates instructions at a given address in the input executable (PE/ELF/MachO) and
     extracts data patches that are written to the stack during emulation. Emulation is halted as
     soon as a certain number of instructions has not performed any memory writes, or when an error
@@ -107,15 +108,15 @@
         image = memoryview(data)
 
         if self.log_debug():
             disassembler = self._capstone.Cs(*self._cs_arch(arch))
         else:
             disassembler = None
 
-        state = EmuState(exe, address, tree, disassembler)
+        state = EmuState(exe, tree, disassembler)
 
         emulator.mem_map(stack_addr, stack_size * 3)
         emulator.reg_write({
             Arch.X8632   : uc.x86_const.UC_X86_REG_ESP,
             Arch.X8664   : uc.x86_const.UC_X86_REG_RSP,
             Arch.ARM32   : uc.arm_const.UC_ARM_REG_SP,
             Arch.ARM32   : uc.arm_const.UC_ARM_REG_SP,
@@ -190,19 +191,23 @@
                 continue
             if size < self.args.min:
                 continue
             self.log_info(F'memory patch at 0x{interval.begin:0{exe.pointer_size//4}X} of size {size}')
             yield emulator.mem_read(interval.begin, size)
 
     def _hook_mem_write(self, emu: Uc, access: int, address: int, size: int, value: int, state: EmuState):
-        if not state.calling:
-            state.waiting = 0
-            state.writes.addi(address, address + size + 1)
-            state.writes.merge_overlaps()
-            self.log_info(F'memory write to 0x{address:0{state.executable.pointer_size//4}X}: {value:0{size*2}X}')
+        state.waiting = 0
+        state.writes.addi(address, address + size + 1)
+        state.writes.merge_overlaps()
+
+        def info():
+            mask = (1 << (size * 8)) - 1
+            data = (value & mask).to_bytes(size, state.executable.byte_order().value).hex().upper()
+            return F'memory write to 0x{address:0{state.executable.pointer_size//4}X}: {data}'
+        self.log_info(info)
 
     def _hook_insn_error(self, emu: Uc, state: EmuState):
         self.log_debug('aborting emulation; instruction error')
         emu.emu_stop()
         return False
 
     def _hook_mem_error(self, emu: Uc, access: int, address: int, size: int, value: int, state: EmuState):
@@ -213,33 +218,26 @@
         emu.emu_stop()
         return False
 
     def _hook_code(self, emu: Uc, address: int, size: int, state: EmuState):
         try:
             waiting = state.waiting
 
-            if address == state.address:
-                if waiting > self.args.halt_after:
-                    emu.emu_stop()
-                    return False
-                state.waiting += 1
-                state.address += size
-                state.calling = False
-            else:
-                instruction = state.disassemble(address, size)
-                if instruction and instruction.mnemonic == 'call':
-                    state.calling = True
+            if waiting > self.args.halt_after:
+                emu.emu_stop()
+                return False
+            state.waiting += 1
 
             def debug_message():
                 instruction = state.disassemble(address, size)
-                flags = 'C' if state.calling else ' '
-                return (
-                    F'emulating [wait={waiting}] [{flags}] 0x{address:0{state.executable.pointer_size//4}X}: '
-                    F'{instruction.mnemonic} {instruction.op_str}'
-                )
+                if instruction:
+                    instruction = F'{instruction.mnemonic} {instruction.op_str}'
+                else:
+                    instruction = '<DISASSEMBLER FAILURE>'
+                return F'emulating [wait={waiting:02d}] 0x{address:0{state.executable.pointer_size//4}X}: {instruction}'
 
             self.log_debug(debug_message)
 
         except KeyboardInterrupt:
             emu.emu_stop()
             return False
```

### Comparing `binary-refinery-0.6.7/refinery/units/formats/hexload.py` & `binary-refinery-0.6.8/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/html.py` & `binary-refinery-0.6.8/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.8/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/ifps.py` & `binary-refinery-0.6.8/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.8/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.8/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.8/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/json.py` & `binary-refinery-0.6.8/refinery/units/formats/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/lnk.py` & `binary-refinery-0.6.8/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.8/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/msi.py` & `binary-refinery-0.6.8/refinery/units/formats/msi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.8/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.8/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.8/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.8/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.8/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pcap.py` & `binary-refinery-0.6.8/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.8/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pdf.py` & `binary-refinery-0.6.8/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.8/refinery/units/formats/pe/pestrip.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 from typing import Generator, Iterable, Optional
 
 from refinery.units.formats.pe import OverlayUnit, Arg
 from refinery.units.formats.pe.perc import RSRC
 from refinery.lib.executable import Executable
-from refinery.lib.tools import entropy
+from refinery.lib.argformats import percent
 from refinery.lib.meta import TerseSizeInt as TI, SizeInt
 
+import re
+import zlib
+
 from fnmatch import fnmatch
 from pefile import PE, Structure, SectionStructure, DIRECTORY_ENTRY
 
 _KB = 1000
 _MB = _KB * _KB
 
+_STRIP = TI(10 * _MB)
 _ASCII = Executable.ascii
 
 
 class pestrip(OverlayUnit):
     """
     Removes the overlay of a PE file and returns the stipped executable. Use `refinery.peoverlay`
     to extract the overlay. The unit can also remove resources and entire sections that exceed a
@@ -27,62 +31,91 @@
     def __init__(
         self,
         *names: Arg(type=str),
         certificate=False,
         directories=False,
         memdump=False,
         resources: Arg.Switch('-r', help='Strip large resources.') = False,
-        sections: Arg.Switch('-s', help='Strip large sections.') = False,
-        entropy: Arg('-e', metavar='E', type=float, help=(
-            'Trailing data from resources and sections with entropy lower than this value is '
-            'removed. The default value is {default}. Set this to 1 to ignore the entropy limit '
-            'entirely and trim every structure as much as possible without violating alignment. '
-            'Setting this value to 0 will strip all occurrences of the last byte.')) = 0.05,
-        size_limit: Arg.Number('-l',
-            help='Structures below this size are not stripped. The default is {default}.') = TI(10 * _MB),
-        aggressive: Arg.Switch('-a',
-            help='Equivalent to -sre1: Entirely strip all large sections and resources.') = False,
+        sections : Arg.Switch('-s', help='Strip large sections.') = False,
+        threshold: Arg('-t', metavar='T', type=percent, help=(
+            'Trailing data from resources and sections is stripped until the compression ratio '
+            'of the remaining rises above this threshold. The default value is {default}. Set '
+            'this to 1 to ignore the limit entirely and trim every structure as much as possible '
+            'without violating alignment. Setting this value to 0 will only strip repeated '
+            'occurrences of the last byte.')) = 0.05,
+        size_limit: Arg.Number('-l', help=(
+            'Structures below this size are not stripped. Default is {default!r}.')) = _STRIP,
+        keep_limit: Arg.Switch('-k', help=(
+            'Do not strip structures to below the above size limit.')) = False,
+        aggressive: Arg.Switch('-a', help=(
+            'Equivalent to -srt1: Strip large sections and resources aggressively.')) = False,
     ):
         if aggressive:
             sections = True
             resources = True
-            entropy = 1
+            threshold = 1
 
         super().__init__(
             certificate,
             directories,
             memdump,
             sections=sections,
             resources=resources,
             size_limit=size_limit,
-            entropy=entropy,
+            keep_limit=keep_limit,
+            threshold=threshold,
             names=names,
         )
 
-    def _right_strip_low_entropy(self, pe: PE, data: memoryview, block_size=_MB) -> int:
-        threshold = self.args.entropy
+    def _right_strip_data(self, pe: PE, data: memoryview, block_size=_MB) -> int:
+        threshold = self.args.threshold
         alignment = pe.OPTIONAL_HEADER.FileAlignment
         data_overhang = len(data) % alignment
         result = data_overhang
+
         if not data:
             return 0
-        if not threshold:
-            import re
-            match = re.search(B'(?s).(?=\\x%02x+$)' % data[-1], data)
-            if match is not None:
-                result = match.start() + 1
-        elif threshold < 1:
-            for k in reversed(range(0, len(data), block_size)):
-                if entropy(data[k:k + block_size]) > threshold:
-                    result = k + block_size
-                    break
+
+        if 0 < threshold < 1:
+            def compression_ratio(offset: int):
+                ratio = len(zlib.compress(data[:offset], level=1)) / offset
+                self.log_debug(F'compressing {SizeInt(offset)!r} ratio={ratio:6.4f}')
+                return ratio
+            upper = len(data)
+            lower = result
+            if compression_ratio(upper) <= threshold:
+                while block_size < upper - lower:
+                    pivot = (lower + upper) // 2
+                    ratio = compression_ratio(pivot)
+                    if ratio > threshold:
+                        lower = pivot + 1
+                        continue
+                    upper = pivot
+                    if abs(ratio - threshold) < 1e-10:
+                        break
+            result = upper
+
+        match = re.search(B'(?s).(?=\\x%02x+$)' % data[result - 1], data[:result])
+        if match is not None:
+            cutoff = match.start() - 1
+            length = result - cutoff
+            if length > block_size:
+                self.log_debug(F'removing additional {TI(length)!r} of repeated byte 0x{data[result-1]:02X}')
+                result = cutoff
+
         result = max(result, data_overhang)
-        result += (data_overhang - result) % alignment
+
+        if self.args.keep_limit:
+            result = max(result, self.args.size_limit)
+
+        result = result + (data_overhang - result) % alignment
+
         while result > len(data):
             result -= alignment
+
         return result
 
     def _adjust_offsets(self, pe: PE, gap_offset: int, gap_size: int):
         base = pe.OPTIONAL_HEADER.ImageBase
         alignment = pe.OPTIONAL_HEADER.FileAlignment
         rva_offset = pe.get_rva_from_offset(gap_offset)
         tva_offset = rva_offset + base
@@ -159,19 +192,19 @@
                 'AddressOfCallBacks',
             ))
             adjust_attributes_of_structure(structure, gap_offset, None, None, (
                 'OffsetModuleName',
                 'PointerToRawData',
             ))
             for attribute in (
-                'CvHeaderOffset'
-                'OffsetIn2Qwords'
-                'OffsetInQwords'
-                'Offset'
-                'OffsetLow'
+                'CvHeaderOffset',
+                'OffsetIn2Qwords',
+                'OffsetInQwords',
+                'Offset',
+                'OffsetLow',
                 'OffsetHigh'
             ):
                 if not hasattr(structure, attribute):
                     continue
                 self.log_warn(F'potential offset in structure {structure.name} ignored: {attribute}')
 
         section.SizeOfRawData = new_section_size
@@ -184,26 +217,26 @@
             section: SectionStructure
             offset = section.PointerToRawData
             name = _ASCII(section.Name)
             old_size = section.SizeOfRawData
             if old_size <= S and not any(fnmatch(name, p) for p in P):
                 self.log_debug(F'criteria not satisfied for section: {SizeInt(old_size)!r} {name}')
                 continue
-            new_size = self._right_strip_low_entropy(pe, memoryview(data)[offset:offset + old_size])
-            self.log_info(F'stripping section {name} from {old_size} to {new_size}')
+            new_size = self._right_strip_data(pe, memoryview(data)[offset:offset + old_size])
+            self.log_info(F'stripping section {name} from {TI(old_size)!r} to {TI(new_size)!r}')
             gap_size = old_size - new_size
             gap_offset = offset + new_size
             if gap_size <= 0:
                 continue
             self._adjust_offsets(pe, gap_offset, gap_size)
             trimmed += gap_size
             data[gap_offset:gap_offset + gap_size] = []
         return trimmed
 
-    def _trim_resources(self, pe: PE, data: bytearray) -> int:
+    def _trim_pe_resources(self, pe: PE, data: bytearray) -> int:
         S = self.args.size_limit
         P = self.args.names
         trimmed = 0
 
         def find_bloated_resources(pe: PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
             for entry in directory.entries:
                 name = getattr(entry, 'name')
@@ -220,30 +253,37 @@
                 struct: Structure = entry.data.struct
                 name = '/'.join((*path, name))
                 if struct.Size <= S and not any(fnmatch(name, p) for p in P):
                     self.log_debug(F'criteria not satisfied for resource: {SizeInt(struct.Size)!r} {name}')
                     continue
                 yield name, struct
 
-        pe.parse_data_directories(directories=[DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']])
+        RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
+        pe.parse_data_directories(directories=[RSRC_INDEX])
 
-        for name, resource in find_bloated_resources(pe, pe.DIRECTORY_ENTRY_RESOURCE):
+        try:
+            resources = pe.DIRECTORY_ENTRY_RESOURCE
+        except AttributeError:
+            return 0
+        for name, resource in find_bloated_resources(pe, resources):
             offset = pe.get_offset_from_rva(resource.OffsetToData)
             old_size = resource.Size
-            new_size = self._right_strip_low_entropy(pe, memoryview(data)[offset:offset + old_size])
+            new_size = self._right_strip_data(pe, memoryview(data)[offset:offset + old_size])
             self.log_info(F'stripping resource {name} from {old_size} to {new_size}')
             gap_size = old_size - new_size
             gap_offset = offset + new_size
             if gap_size <= 0:
                 continue
             resource.Size = new_size
             self._adjust_offsets(pe, gap_offset, gap_size)
             trimmed += gap_size
             data[gap_offset:gap_offset + gap_size] = []
 
+        pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= trimmed
+        self.log_debug(F'trimming size of resource data directory by {TI(trimmed)!r}')
         return trimmed
 
     def process(self, data: bytearray) -> bytearray:
         body_size = self._get_size(data)
         if body_size < len(data):
             if isinstance(data, bytearray):
                 data[body_size:] = []
@@ -260,17 +300,17 @@
             view = memoryview(view)
             try:
                 view[0] = 0x4D
             except Exception:
                 copy = True
                 view = bytearray(pe.__data__)
         if self.args.resources:
-            trimmed += self._trim_resources(pe, view)
+            trimmed += self._trim_pe_resources(pe, view)
         if self.args.sections:
             trimmed += self._trim_sections(pe, view)
         if copy:
             pe.__data__ = view
         data = pe.write()
         end = total - trimmed
         if end < len(data):
-            self.log_warn(F'output contains {end-len(data)} trailing bytes')
+            self.log_warn(F'output contains {len(data)-end} trailing bytes')
         return data
```

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.8/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.8/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/stego.py` & `binary-refinery-0.6.8/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/tnetmtm.py` & `binary-refinery-0.6.8/refinery/units/formats/tnetmtm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/winreg.py` & `binary-refinery-0.6.8/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/formats/xml.py` & `binary-refinery-0.6.8/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/malware/n40.py` & `binary-refinery-0.6.8/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/__init__.py` & `binary-refinery-0.6.8/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/chop.py` & `binary-refinery-0.6.8/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/cm.py` & `binary-refinery-0.6.8/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/cull.py` & `binary-refinery-0.6.8/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/dedup.py` & `binary-refinery-0.6.8/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/eat.py` & `binary-refinery-0.6.8/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/ef.py` & `binary-refinery-0.6.8/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/emit.py` & `binary-refinery-0.6.8/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/group.py` & `binary-refinery-0.6.8/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/groupby.py` & `binary-refinery-0.6.8/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/iff.py` & `binary-refinery-0.6.8/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/iffp.py` & `binary-refinery-0.6.8/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/iffs.py` & `binary-refinery-0.6.8/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/iffx.py` & `binary-refinery-0.6.8/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/max.py` & `binary-refinery-0.6.8/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/min.py` & `binary-refinery-0.6.8/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/mvc.py` & `binary-refinery-0.6.8/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/mvg.py` & `binary-refinery-0.6.8/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/pad.py` & `binary-refinery-0.6.8/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/pick.py` & `binary-refinery-0.6.8/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/pop.py` & `binary-refinery-0.6.8/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/push.py` & `binary-refinery-0.6.8/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/put.py` & `binary-refinery-0.6.8/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/queue.py` & `binary-refinery-0.6.8/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/reduce.py` & `binary-refinery-0.6.8/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/scope.py` & `binary-refinery-0.6.8/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/sep.py` & `binary-refinery-0.6.8/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/sorted.py` & `binary-refinery-0.6.8/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/swap.py` & `binary-refinery-0.6.8/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/transpose.py` & `binary-refinery-0.6.8/refinery/units/meta/transpose.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.8/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.8/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/couple.py` & `binary-refinery-0.6.8/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/datefix.py` & `binary-refinery-0.6.8/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/drp.py` & `binary-refinery-0.6.8/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/nop.py` & `binary-refinery-0.6.8/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.8/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/misc/xkey.py` & `binary-refinery-0.6.8/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.8/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.8/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/defang.py` & `binary-refinery-0.6.8/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.8/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.8/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.8/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/resub.py` & `binary-refinery-0.6.8/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/rex.py` & `binary-refinery-0.6.8/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.8/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.8/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.8/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.8/refinery/units/pattern/xtp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.8/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.8/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/asm.py` & `binary-refinery-0.6.8/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/dump.py` & `binary-refinery-0.6.8/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.8/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/peek.py` & `binary-refinery-0.6.8/refinery/units/sinks/peek.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 
     def _peekmeta(self, linewidth, sep, _x_peek=None, **meta) -> Generator[str, None, None]:
         if not meta and not _x_peek:
             return
         width = max((len(name) for name in meta), default=0)
         separators = iter([sep])
         if _x_peek is not None:
+            if len(_x_peek) > linewidth:
+                _x_peek = _x_peek[:linewidth - 3] + '...'
             yield from separators
             yield _x_peek
         for name in sorted(meta):
             value = meta[name]
             if value is None:
                 continue
             if isinstance(value, CustomStringRepresentation):
```

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.8/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.8/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.8/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.8/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/cswap.py` & `binary-refinery-0.6.8/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/rep.py` & `binary-refinery-0.6.8/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/repl.py` & `binary-refinery-0.6.8/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/snip.py` & `binary-refinery-0.6.8/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/stretch.py` & `binary-refinery-0.6.8/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/termfit.py` & `binary-refinery-0.6.8/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/refinery/units/strings/trim.py` & `binary-refinery-0.6.8/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.7/setup.py` & `binary-refinery-0.6.8/setup.py`

 * *Files identical despite different names*

