# Comparing `tmp/unblob-23.5.5.tar.gz` & `tmp/unblob-23.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unblob-23.5.5.tar", max compression
+gzip compressed data, was "unblob-23.5.9.tar", max compression
```

## Comparing `unblob-23.5.5.tar` & `unblob-23.5.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     2255 2023-05-05 14:46:44.706125 unblob-23.5.5/LICENSE
--rw-r--r--   0        0        0     4348 2023-05-05 14:46:44.710125 unblob-23.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/__init__.py
--rwxr-xr-x   0        0        0     6954 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/cli.py
--rw-r--r--   0        0        0      344 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/cli_options.py
--rw-r--r--   0        0        0     1044 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/dependencies.py
--rw-r--r--   0        0        0     4100 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractor.py
--rw-r--r--   0        0        0      196 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/README.md
--rw-r--r--   0        0        0       40 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/extractors/command.py
--rw-r--r--   0        0        0    10384 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/file_utils.py
--rw-r--r--   0        0        0     5715 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/finder.py
--rw-r--r--   0        0        0     2371 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/__init__.py
--rw-r--r--   0        0        0     1218 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/_safe_tarfile.py
--rw-r--r--   0        0        0     1694 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/ar.py
--rw-r--r--   0        0        0     2775 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/arc.py
--rw-r--r--   0        0        0     5683 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/arj.py
--rw-r--r--   0        0        0     2505 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/cab.py
--rw-r--r--   0        0        0     7632 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/cpio.py
--rw-r--r--   0        0        0     2250 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dlink/encrpted_img.py
--rw-r--r--   0        0        0     3589 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dlink/shrs.py
--rw-r--r--   0        0        0     3700 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/dmg.py
--rw-r--r--   0        0        0     3018 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/engeniustech/engenius.py
--rw-r--r--   0        0        0     3282 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/hp/bdl.py
--rw-r--r--   0        0        0     3689 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/hp/ipkg.py
--rw-r--r--   0        0        0     2946 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/instar/bneg.py
--rw-r--r--   0        0        0     1416 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/instar/instar_hd.py
--rw-r--r--   0        0        0     2553 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/netgear/chk.py
--rw-r--r--   0        0        0     3895 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/netgear/trx.py
--rw-r--r--   0        0        0     5527 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/qnap/qnap_nas.py
--rw-r--r--   0        0        0     1158 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/rar.py
--rw-r--r--   0        0        0     2591 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/sevenzip.py
--rw-r--r--   0        0        0     2332 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/stuffit.py
--rw-r--r--   0        0        0     4298 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/tar.py
--rw-r--r--   0        0        0     6107 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/xiaomi/hdr.py
--rw-r--r--   0        0        0     6412 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/archive/zip.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/_gzip_reader.py
--rw-r--r--   0        0        0     4693 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/bzip2.py
--rw-r--r--   0        0        0     8898 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/compress.py
--rw-r--r--   0        0        0     3800 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/gzip.py
--rw-r--r--   0        0        0     5675 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lz4.py
--rw-r--r--   0        0        0     2876 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lzh.py
--rw-r--r--   0        0        0     1423 2023-05-05 14:46:45.330129 unblob-23.5.5/unblob/handlers/compression/lzip.py
--rw-r--r--   0        0        0     3508 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/lzma.py
--rw-r--r--   0        0        0     4147 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/lzo.py
--rw-r--r--   0        0        0     6073 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/xz.py
--rw-r--r--   0        0        0     1935 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/zlib.py
--rw-r--r--   0        0        0     2662 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/compression/zstd.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/executable/__init__.py
--rw-r--r--   0        0        0    15477 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/executable/elf.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/android/__init__.py
--rw-r--r--   0        0        0     2889 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/android/sparse.py
--rw-r--r--   0        0        0     2320 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/cramfs.py
--rw-r--r--   0        0        0     4841 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/extfs.py
--rw-r--r--   0        0        0     6278 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/fat.py
--rw-r--r--   0        0        0     4604 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/iso9660.py
--rw-r--r--   0        0        0     5213 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/jffs2.py
--rw-r--r--   0        0        0     2246 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/ntfs.py
--rw-r--r--   0        0        0    13617 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/romfs.py
--rw-r--r--   0        0        0     9619 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/squashfs.py
--rw-r--r--   0        0        0     5738 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/ubi.py
--rw-r--r--   0        0        0    28094 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/handlers/filesystem/yaffs.py
--rw-r--r--   0        0        0      315 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/hookspecs.py
--rw-r--r--   0        0        0      515 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/identifiers.py
--rw-r--r--   0        0        0      587 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/iter_utils.py
--rw-r--r--   0        0        0     3739 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/logging.py
--rw-r--r--   0        0        0     9964 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/models.py
--rw-r--r--   0        0        0     2252 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/parser.py
--rw-r--r--   0        0        0     3408 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/plugins.py
--rw-r--r--   0        0        0     4090 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/pool.py
--rw-r--r--   0        0        0    19578 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/processing.py
--rw-r--r--   0        0        0        0 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/py.typed
--rw-r--r--   0        0        0     5120 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/report.py
--rw-r--r--   0        0        0     1538 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/signals.py
--rw-r--r--   0        0        0     3336 2023-05-05 14:46:45.334129 unblob-23.5.5/unblob/testing.py
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 unblob-23.5.5/PKG-INFO
+-rw-r--r--   0        0        0     2255 2023-05-09 10:34:43.313597 unblob-23.5.9/LICENSE
+-rw-r--r--   0        0        0     4327 2023-05-09 10:34:43.317597 unblob-23.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/__init__.py
+-rwxr-xr-x   0        0        0     6954 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/cli.py
+-rw-r--r--   0        0        0      344 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/cli_options.py
+-rw-r--r--   0        0        0     1044 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/dependencies.py
+-rw-r--r--   0        0        0     4142 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/extractor.py
+-rw-r--r--   0        0        0      196 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/extractors/README.md
+-rw-r--r--   0        0        0       40 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/extractors/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/extractors/command.py
+-rw-r--r--   0        0        0    10384 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/file_utils.py
+-rw-r--r--   0        0        0     5715 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/finder.py
+-rw-r--r--   0        0        0     2371 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/__init__.py
+-rw-r--r--   0        0        0     1218 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/_safe_tarfile.py
+-rw-r--r--   0        0        0     1694 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/ar.py
+-rw-r--r--   0        0        0     2775 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/arc.py
+-rw-r--r--   0        0        0     5683 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/arj.py
+-rw-r--r--   0        0        0     2505 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/cab.py
+-rw-r--r--   0        0        0     7632 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/cpio.py
+-rw-r--r--   0        0        0     2250 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/dlink/encrpted_img.py
+-rw-r--r--   0        0        0     3589 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/dlink/shrs.py
+-rw-r--r--   0        0        0     3700 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/dmg.py
+-rw-r--r--   0        0        0     3018 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/engeniustech/engenius.py
+-rw-r--r--   0        0        0     3282 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/hp/bdl.py
+-rw-r--r--   0        0        0     3689 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/hp/ipkg.py
+-rw-r--r--   0        0        0     2946 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/instar/bneg.py
+-rw-r--r--   0        0        0     1416 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/instar/instar_hd.py
+-rw-r--r--   0        0        0     2553 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/netgear/chk.py
+-rw-r--r--   0        0        0     3895 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/netgear/trx.py
+-rw-r--r--   0        0        0     5527 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/qnap/qnap_nas.py
+-rw-r--r--   0        0        0     1158 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/rar.py
+-rw-r--r--   0        0        0     2591 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/sevenzip.py
+-rw-r--r--   0        0        0     2332 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/stuffit.py
+-rw-r--r--   0        0        0     4298 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/tar.py
+-rw-r--r--   0        0        0     6107 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/xiaomi/hdr.py
+-rw-r--r--   0        0        0     6412 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/archive/zip.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/_gzip_reader.py
+-rw-r--r--   0        0        0     4693 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/bzip2.py
+-rw-r--r--   0        0        0     8898 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/compress.py
+-rw-r--r--   0        0        0     3800 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/gzip.py
+-rw-r--r--   0        0        0     5675 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/lz4.py
+-rw-r--r--   0        0        0     2876 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/lzh.py
+-rw-r--r--   0        0        0     1423 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/lzip.py
+-rw-r--r--   0        0        0     3508 2023-05-09 10:34:43.905638 unblob-23.5.9/unblob/handlers/compression/lzma.py
+-rw-r--r--   0        0        0     4150 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/compression/lzo.py
+-rw-r--r--   0        0        0     6073 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/compression/xz.py
+-rw-r--r--   0        0        0     1935 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/compression/zlib.py
+-rw-r--r--   0        0        0     2662 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/compression/zstd.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/executable/__init__.py
+-rw-r--r--   0        0        0    15477 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/executable/elf.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/android/__init__.py
+-rw-r--r--   0        0        0     2889 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/android/sparse.py
+-rw-r--r--   0        0        0     2320 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/cramfs.py
+-rw-r--r--   0        0        0     4841 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/extfs.py
+-rw-r--r--   0        0        0     6278 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/fat.py
+-rw-r--r--   0        0        0     4604 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/iso9660.py
+-rw-r--r--   0        0        0     5213 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/jffs2.py
+-rw-r--r--   0        0        0     2246 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/ntfs.py
+-rw-r--r--   0        0        0    13617 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/romfs.py
+-rw-r--r--   0        0        0     9619 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/squashfs.py
+-rw-r--r--   0        0        0     5738 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/ubi.py
+-rw-r--r--   0        0        0    28241 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/handlers/filesystem/yaffs.py
+-rw-r--r--   0        0        0      315 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/hookspecs.py
+-rw-r--r--   0        0        0      515 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/identifiers.py
+-rw-r--r--   0        0        0      587 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/iter_utils.py
+-rw-r--r--   0        0        0     3739 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/logging.py
+-rw-r--r--   0        0        0     9964 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/models.py
+-rw-r--r--   0        0        0     2252 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/parser.py
+-rw-r--r--   0        0        0     3408 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/plugins.py
+-rw-r--r--   0        0        0     4090 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/pool.py
+-rw-r--r--   0        0        0    19578 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/processing.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/py.typed
+-rw-r--r--   0        0        0     5120 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/report.py
+-rw-r--r--   0        0        0     1538 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/signals.py
+-rw-r--r--   0        0        0     3336 2023-05-09 10:34:43.909639 unblob-23.5.9/unblob/testing.py
+-rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 unblob-23.5.9/PKG-INFO
```

### Comparing `unblob-23.5.5/LICENSE` & `unblob-23.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/pyproject.toml` & `unblob-23.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unblob"
-version = "23.5.5"
+version = "23.5.9"
 description = "Extract files from any kind of container formats"
 authors = ["ONEKEY <support@onekey.com>"]
 license = "MIT"
 packages = [
     { include = "unblob" },
 ]
 
@@ -13,15 +13,14 @@
 click = "^8.1.3"
 "dissect.cstruct" = "^2.0"
 attrs = "^22.2.0"
 structlog = "^21.2.0"
 arpy = "^2.2.0"
 rarfile = "^4.0"
 ubi-reader = "^0.8.5"
-python-lzo = "^1.14"
 plotext = ">=4.2.0,<6.0"
 pluggy = "^1.0.0"
 python-magic = "^0.4.27"
 pyperscan = "^0.2.2"
 lark = "^1.1.2"
 lz4 = "^4.0.0"
 lief = "^0.12.3"
```

### Comparing `unblob-23.5.5/unblob/cli.py` & `unblob-23.5.9/unblob/cli.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/dependencies.py` & `unblob-23.5.9/unblob/dependencies.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/extractor.py` & `unblob-23.5.9/unblob/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
     with carve_path.open("xb") as f:
         for data in iterate_file(file, chunk.start_offset, chunk.size):
             f.write(data)
 
 
 def fix_permission(path: Path):
+    if path.is_symlink():
+        return
+
     if path.is_file():
         path.chmod(0o644)
     elif path.is_dir():
         path.chmod(0o775)
 
 
 def is_safe_path(basedir: Path, path: Path) -> bool:
```

### Comparing `unblob-23.5.5/unblob/extractors/command.py` & `unblob-23.5.9/unblob/extractors/command.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/file_utils.py` & `unblob-23.5.9/unblob/file_utils.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/finder.py` & `unblob-23.5.9/unblob/finder.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/__init__.py` & `unblob-23.5.9/unblob/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/_safe_tarfile.py` & `unblob-23.5.9/unblob/handlers/archive/_safe_tarfile.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/ar.py` & `unblob-23.5.9/unblob/handlers/archive/ar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/arc.py` & `unblob-23.5.9/unblob/handlers/archive/arc.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/arj.py` & `unblob-23.5.9/unblob/handlers/archive/arj.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/cab.py` & `unblob-23.5.9/unblob/handlers/archive/cab.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/cpio.py` & `unblob-23.5.9/unblob/handlers/archive/cpio.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/dlink/encrpted_img.py` & `unblob-23.5.9/unblob/handlers/archive/dlink/encrpted_img.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/dlink/shrs.py` & `unblob-23.5.9/unblob/handlers/archive/dlink/shrs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/dmg.py` & `unblob-23.5.9/unblob/handlers/archive/dmg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/engeniustech/engenius.py` & `unblob-23.5.9/unblob/handlers/archive/engeniustech/engenius.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/hp/bdl.py` & `unblob-23.5.9/unblob/handlers/archive/hp/bdl.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/hp/ipkg.py` & `unblob-23.5.9/unblob/handlers/archive/hp/ipkg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/instar/bneg.py` & `unblob-23.5.9/unblob/handlers/archive/instar/bneg.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/instar/instar_hd.py` & `unblob-23.5.9/unblob/handlers/archive/instar/instar_hd.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/netgear/chk.py` & `unblob-23.5.9/unblob/handlers/archive/netgear/chk.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/netgear/trx.py` & `unblob-23.5.9/unblob/handlers/archive/netgear/trx.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/qnap/qnap_nas.py` & `unblob-23.5.9/unblob/handlers/archive/qnap/qnap_nas.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/rar.py` & `unblob-23.5.9/unblob/handlers/archive/rar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/sevenzip.py` & `unblob-23.5.9/unblob/handlers/archive/sevenzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/stuffit.py` & `unblob-23.5.9/unblob/handlers/archive/stuffit.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/tar.py` & `unblob-23.5.9/unblob/handlers/archive/tar.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/xiaomi/hdr.py` & `unblob-23.5.9/unblob/handlers/archive/xiaomi/hdr.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/archive/zip.py` & `unblob-23.5.9/unblob/handlers/archive/zip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/_gzip_reader.py` & `unblob-23.5.9/unblob/handlers/compression/_gzip_reader.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/bzip2.py` & `unblob-23.5.9/unblob/handlers/compression/bzip2.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/compress.py` & `unblob-23.5.9/unblob/handlers/compression/compress.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/gzip.py` & `unblob-23.5.9/unblob/handlers/compression/gzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/lz4.py` & `unblob-23.5.9/unblob/handlers/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/lzh.py` & `unblob-23.5.9/unblob/handlers/compression/lzh.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/lzip.py` & `unblob-23.5.9/unblob/handlers/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/lzma.py` & `unblob-23.5.9/unblob/handlers/compression/lzma.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/lzo.py` & `unblob-23.5.9/unblob/handlers/compression/lzo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
+import zlib
 from enum import IntEnum
 from typing import Optional
 
-import lzo
 from structlog import get_logger
 
 from unblob.extractors import Command
 
 from ...file_utils import Endian, convert_int32
 from ...models import File, HexString, StructHandler, ValidChunk
 
@@ -91,19 +91,19 @@
             file.seek(start_offset)
             header = self.cparser_be.lzo_header_filter_t(file)
 
         logger.debug("LZO header parsed", header=header, _verbosity=3)
 
         # Checksum excludes the magic and the checksum itself
         if header.flags & HeaderFlags.H_CRC32:
-            calculated_checksum = lzo.crc32(
+            calculated_checksum = zlib.crc32(
                 header.dumps()[MAGIC_LENGTH:-CHECKSUM_LENGTH]
             )
         else:
-            calculated_checksum = lzo.adler32(
+            calculated_checksum = zlib.adler32(
                 header.dumps()[MAGIC_LENGTH:-CHECKSUM_LENGTH]
             )
 
         if header.header_checksum != calculated_checksum:
             logger.debug("Header checksum verification failed")
             return None
```

### Comparing `unblob-23.5.5/unblob/handlers/compression/xz.py` & `unblob-23.5.9/unblob/handlers/compression/xz.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/zlib.py` & `unblob-23.5.9/unblob/handlers/compression/zlib.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/compression/zstd.py` & `unblob-23.5.9/unblob/handlers/compression/zstd.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/executable/elf.py` & `unblob-23.5.9/unblob/handlers/executable/elf.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/android/sparse.py` & `unblob-23.5.9/unblob/handlers/filesystem/android/sparse.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/cramfs.py` & `unblob-23.5.9/unblob/handlers/filesystem/cramfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/extfs.py` & `unblob-23.5.9/unblob/handlers/filesystem/extfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/fat.py` & `unblob-23.5.9/unblob/handlers/filesystem/fat.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/iso9660.py` & `unblob-23.5.9/unblob/handlers/filesystem/iso9660.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/jffs2.py` & `unblob-23.5.9/unblob/handlers/filesystem/jffs2.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/ntfs.py` & `unblob-23.5.9/unblob/handlers/filesystem/ntfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/romfs.py` & `unblob-23.5.9/unblob/handlers/filesystem/romfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/squashfs.py` & `unblob-23.5.9/unblob/handlers/filesystem/squashfs.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/ubi.py` & `unblob-23.5.9/unblob/handlers/filesystem/ubi.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/handlers/filesystem/yaffs.py` & `unblob-23.5.9/unblob/handlers/filesystem/yaffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,15 @@
         raise NotImplementedError
 
     def init_tree(self):
         return
 
     def parse(self, store: bool = False):  # noqa: C901,FBT001,FBT002
         self.init_tree()
+        entries = 0
         for offset, page, spare in iterate_over_file(self.file, self.config):
             try:
                 data_chunk = self.build_chunk(
                     spare, offset - self.config.page_size - self.config.spare_size
                 )
             except EOFError:
                 break
@@ -321,16 +322,19 @@
                     break
 
                 if not is_valid_header(header):
                     break
 
                 if store:
                     self.insert_entry(self.build_entry(header, data_chunk))
+                entries += 1
             elif store:
                 self.data_chunks[data_chunk.object_id].append(data_chunk)
+        if not entries:
+            raise InvalidInputFormat("YAFFS filesystem with no entries.")
         self.end_offset = self.file.tell()
 
     def auto_detect(self) -> YAFFSConfig:
         """Auto-detect page_size, spare_size, and ECC using known signatures."""
         page_size = 0
         config = None
         for page_size in VALID_PAGE_SIZES:
```

### Comparing `unblob-23.5.5/unblob/identifiers.py` & `unblob-23.5.9/unblob/identifiers.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/iter_utils.py` & `unblob-23.5.9/unblob/iter_utils.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/logging.py` & `unblob-23.5.9/unblob/logging.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/models.py` & `unblob-23.5.9/unblob/models.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/parser.py` & `unblob-23.5.9/unblob/parser.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/plugins.py` & `unblob-23.5.9/unblob/plugins.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/pool.py` & `unblob-23.5.9/unblob/pool.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/processing.py` & `unblob-23.5.9/unblob/processing.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/report.py` & `unblob-23.5.9/unblob/report.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/signals.py` & `unblob-23.5.9/unblob/signals.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/unblob/testing.py` & `unblob-23.5.9/unblob/testing.py`

 * *Files identical despite different names*

### Comparing `unblob-23.5.5/PKG-INFO` & `unblob-23.5.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unblob
-Version: 23.5.5
+Version: 23.5.9
 Summary: Extract files from any kind of container formats
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,13 @@
 Requires-Dist: jefferson (>=0.4.2,<0.5.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: lief (>=0.12.3,<0.13.0)
 Requires-Dist: lz4 (>=4.0.0,<5.0.0)
 Requires-Dist: plotext (>=4.2.0,<6.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
 Requires-Dist: pyperscan (>=0.2.2,<0.3.0)
-Requires-Dist: python-lzo (>=1.14,<2.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: structlog (>=21.2.0,<22.0.0)
 Requires-Dist: treelib (>=1.6.1,<2.0.0)
 Requires-Dist: ubi-reader (>=0.8.5,<0.9.0)
 Requires-Dist: unblob-native (>=0.1.0,<0.2.0)
```

