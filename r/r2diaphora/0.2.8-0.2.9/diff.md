# Comparing `tmp/r2diaphora-0.2.8.tar.gz` & `tmp/r2diaphora-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2diaphora-0.2.8.tar", last modified: Mon May 22 08:50:50 2023, max compression
+gzip compressed data, was "r2diaphora-0.2.9.tar", last modified: Wed May 31 14:17:17 2023, max compression
```

## Comparing `r2diaphora-0.2.8.tar` & `r2diaphora-0.2.9.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/LICENSE
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/MANIFEST.in
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/README.md
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.654807 r2diaphora-0.2.8/r2diaphora/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/__init__.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94459 2023-05-22 08:45:18.000000 r2diaphora-0.2.8/r2diaphora/diaphora.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/diaphora_heuristics.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41947 2023-05-22 08:47:09.000000 r2diaphora-0.2.8/r2diaphora/diaphora_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/difflibparser.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/html_diff.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.658807 r2diaphora-0.2.8/r2diaphora/idaapi/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/idaapi/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    22800 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/idaapi/idaapi_to_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/idaapi/instructions.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.658807 r2diaphora-0.2.8/r2diaphora/jkutils/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/jkutils/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/jkutils/factor.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/jkutils/graph_hashes.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/jkutils/kfuzzy.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.658807 r2diaphora-0.2.8/r2diaphora/others/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/others/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/others/tarjan_sort.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.654807 r2diaphora-0.2.8/r2diaphora/pycparser/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.670808 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.670808 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_ansi.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_syslist.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/aio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/alloca.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/argz.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.670808 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/arpa/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.670808 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/asm-generic/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/assert.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/complex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/cpio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/dirent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/dlfcn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/emmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/endian.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/envz.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/errno.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/fastmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/fcntl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/features.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/fenv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/float.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/fnmatch.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ftw.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/getopt.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/glob.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/grp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/iconv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ieeefp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/immintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/inttypes.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/iso646.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/langinfo.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/libgen.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/libintl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/limits.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.674809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/linux/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/linux/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/linux/version.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/locale.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/malloc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/math.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.674809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/monetary.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/mqueue.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ndbm.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.674809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/net/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/net/if.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/netdb.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.674809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/netinet/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/netinet/in.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/newlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/nl_types.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.674809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/err.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/paths.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/process.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/pthread.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/pwd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/reent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/regdef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/regex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sched.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/search.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/semaphore.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/setjmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/signal.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/smmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/spawn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdarg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdatomic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdbool.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stddef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdint.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/string.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/strings.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/stropts.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/mman.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/msg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/resource.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/select.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/sem.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/shm.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/stat.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/times.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/uio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/un.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/sys/wait.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/syslog.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/tar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/termios.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/tgmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/threads.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/trace.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/ulimit.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/unctrl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/unistd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/utime.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/utmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/utmpx.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/wchar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/wctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/wordexp.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/xcb/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/zlib.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.654807 r2diaphora-0.2.8/r2diaphora/signatures/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/r2diaphora/signatures/flirt/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_arm.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_mips.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_ppc.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_sh4.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_x86-64.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_x86.sig
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.658807 r2diaphora-0.2.8/r2diaphora.egg-info/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/SOURCES.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/dependency_links.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/entry_points.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/requires.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-05-22 08:50:50.000000 r2diaphora-0.2.8/r2diaphora.egg-info/top_level.txt
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/scripts/
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/scripts/r2diaphora-bulk
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-05-16 15:00:43.000000 r2diaphora-0.2.8/scripts/r2diaphora-db
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-05-22 08:50:50.678809 r2diaphora-0.2.8/setup.cfg
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-05-22 08:48:01.000000 r2diaphora-0.2.8/setup.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/LICENSE
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/MANIFEST.in
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/README.md
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/__init__.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94459 2023-05-22 08:45:18.000000 r2diaphora-0.2.9/r2diaphora/diaphora.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/diaphora_heuristics.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41947 2023-05-31 10:24:37.000000 r2diaphora-0.2.9/r2diaphora/diaphora_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/difflibparser.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/html_diff.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/idaapi/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/idaapi/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    22997 2023-05-31 10:23:39.000000 r2diaphora-0.2.9/r2diaphora/idaapi/idaapi_to_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/idaapi/instructions.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/jkutils/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/factor.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/graph_hashes.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/kfuzzy.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/others/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/others/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/others/tarjan_sort.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.641971 r2diaphora-0.2.9/r2diaphora/pycparser/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.661973 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_ansi.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_syslist.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/aio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/alloca.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/argz.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/arpa/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/asm-generic/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/assert.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/complex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/cpio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/dirent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/dlfcn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/emmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/endian.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/envz.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/errno.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fastmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fcntl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/features.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fenv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/float.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fnmatch.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ftw.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/getopt.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/glob.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/grp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/iconv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ieeefp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/immintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/inttypes.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/iso646.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/langinfo.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/libgen.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/libintl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/limits.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/version.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/locale.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/malloc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/math.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/monetary.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mqueue.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ndbm.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/net/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/net/if.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netdb.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/in.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/newlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/nl_types.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/err.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/paths.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/process.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/pthread.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/pwd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/reent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/regdef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/regex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sched.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/search.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/semaphore.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/setjmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/signal.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/smmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/spawn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdarg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdatomic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdbool.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stddef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdint.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/string.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/strings.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stropts.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.669974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/mman.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/msg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/resource.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/select.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/sem.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/shm.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/stat.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/times.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/uio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/un.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/wait.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/syslog.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/tar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/termios.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/tgmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/threads.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/trace.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ulimit.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/unctrl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/unistd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utime.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utmpx.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wchar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wordexp.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.669974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/xcb/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/zlib.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.641971 r2diaphora-0.2.9/r2diaphora/signatures/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/r2diaphora/signatures/flirt/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_arm.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_mips.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_ppc.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_sh4.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86-64.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86.sig
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora.egg-info/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/entry_points.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/requires.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/top_level.txt
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/scripts/
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/scripts/r2diaphora-bulk
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/scripts/r2diaphora-db
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/setup.cfg
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-05-31 14:17:02.000000 r2diaphora-0.2.9/setup.py
```

### Comparing `r2diaphora-0.2.8/LICENSE` & `r2diaphora-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/README.md` & `r2diaphora-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/diaphora.py` & `r2diaphora-0.2.9/r2diaphora/diaphora.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/diaphora_heuristics.py` & `r2diaphora-0.2.9/r2diaphora/diaphora_heuristics.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/diaphora_r2.py` & `r2diaphora-0.2.9/r2diaphora/diaphora_r2.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/difflibparser.py` & `r2diaphora-0.2.9/r2diaphora/difflibparser.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/html_diff.py` & `r2diaphora-0.2.9/r2diaphora/html_diff.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/idaapi/idaapi_to_r2.py` & `r2diaphora-0.2.9/r2diaphora/idaapi/idaapi_to_r2.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,16 +528,23 @@
 
     ins = log_exec_r2_cmdj(f"aoj 1 @ {x}")[0]
     return ins["size"], ins
 
 #-----------------------------------------------------------------------
 def SegStart(ea):
     # Just return the segment's start address
+    curr_seg = {}
     try:
-        return int(log_exec_r2_cmd("iS.~1[3]"), 16)
+        segments = log_exec_r2_cmdj("iSj")
+        for seg in segments:
+            if seg["vaddr"] <= ea <= seg["vaddr"] + seg["size"]:
+                curr_seg = seg
+                break
+
+        return curr_seg.get("vaddr", 0)
     except Exception:
         return 0
 
 #-----------------------------------------------------------------------
 def GetFunctionFlags(fcn):
     # TODO: Return if it looks like a function library, a thunk or a jump
     return -1 # FUNC_LIB
```

### Comparing `r2diaphora-0.2.8/r2diaphora/idaapi/instructions.py` & `r2diaphora-0.2.9/r2diaphora/idaapi/instructions.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/jkutils/factor.py` & `r2diaphora-0.2.9/r2diaphora/jkutils/factor.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/jkutils/graph_hashes.py` & `r2diaphora-0.2.9/r2diaphora/jkutils/graph_hashes.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/jkutils/kfuzzy.py` & `r2diaphora-0.2.9/r2diaphora/jkutils/kfuzzy.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/others/tarjan_sort.py` & `r2diaphora-0.2.9/r2diaphora/others/tarjan_sort.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h` & `r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_fake_defines.h` & `r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h` & `r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/pycparser/fake_libc_include/zlib.h` & `r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/zlib.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_arm.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_arm.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_mips.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_mips.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_ppc.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_ppc.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_sh4.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_sh4.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_x86-64.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86-64.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora/signatures/flirt/uclibc_x86.sig` & `r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/r2diaphora.egg-info/SOURCES.txt` & `r2diaphora-0.2.9/r2diaphora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/scripts/r2diaphora-bulk` & `r2diaphora-0.2.9/scripts/r2diaphora-bulk`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/scripts/r2diaphora-db` & `r2diaphora-0.2.9/scripts/r2diaphora-db`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.8/setup.py` & `r2diaphora-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             shutil.copy2(
                 f,
                 os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt")
             )
 
 setup(
     name="r2diaphora",
-    version="0.2.8",
+    version="0.2.9",
     description="radare2 port of diaphora",
     url="https://github.com/FernandoDoming/r2diaphora",
     author="Fernando Domínguez",
     author_email="fernando.dom.del@gmail.com",
     license="GNU GPL v3",
     packages=[
         "r2diaphora",
```

