# Comparing `tmp/primer3-py-1.2.2.tar.gz` & `tmp/primer3-py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primer3-py-1.2.2.tar", last modified: Tue May 16 16:13:49 2023, max compression
+gzip compressed data, was "primer3-py-2.0.0.tar", last modified: Wed May 31 15:46:37 2023, max compression
```

## Comparing `primer3-py-1.2.2.tar` & `primer3-py-2.0.0.tar`

### file list

```diff
@@ -1,204 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.651435 primer3-py-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 16:13:43.000000 primer3-py-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-16 16:13:43.000000 primer3-py-1.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-16 16:13:43.000000 primer3-py-1.2.2/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-16 16:13:43.000000 primer3-py-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-16 16:13:43.000000 primer3-py-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-16 16:13:49.651435 primer3-py-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 16:13:43.000000 primer3-py-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 16:13:43.000000 primer3-py-1.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.631435 primer3-py-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.631435 primer3-py-1.2.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/api/bindings.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/api/p3helpers.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/api/thermoanalysis.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/changes_link.md
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/cython_help.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/miscellany.md
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-16 16:13:43.000000 primer3-py-1.2.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.631435 primer3-py-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-16 16:13:43.000000 primer3-py-1.2.2/examples/basicprimerdesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-16 16:13:43.000000 primer3-py-1.2.2/examples/orthogonalprimers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.631435 primer3-py-1.2.2/primer3/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/argdefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/p3helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/p3helpers.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.627435 primer3-py-1.2.2/primer3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.635435 primer3-py-1.2.2/primer3/src/libprimer3/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/ABOUT.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/amplicontm.c
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/amplicontm.h
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/amplicontm_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    38114 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/dpal.c
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/dpal.h
--rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/format_output.c
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/format_output.h
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/gpl-2.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.635435 primer3-py-1.2.2/primer3/src/libprimer3/klib/
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/klib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/klib/khash.h
--rw-r--r--   0 runner    (1001) docker     (123)   349509 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/libprimer3.c
--rw-r--r--   0 runner    (1001) docker     (123)    58440 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/libprimer3.h
--rw-r--r--   0 runner    (1001) docker     (123)   342261 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/libprimer3flex.c
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/libprimer3flex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/long_seq_tm_test_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/masker.c
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/masker.h
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/masker_main.c
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/ntdpal_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/oligotm.c
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/oligotm.h
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/oligotm_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/p3_seq_lib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/p3_seq_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_boulder_main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.639435 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/dangle.ds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.639435 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/loops.dh
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/loops.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stack.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stackmm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stackmm.ds
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tetraloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tetraloop.ds
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/triloop.ds
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack2.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack2.ds
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds
--rw-r--r--   0 runner    (1001) docker     (123)    24711 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/print_boulder.c
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/print_boulder.h
--rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/read_boulder.c
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/read_boulder.h
--rw-r--r--   0 runner    (1001) docker     (123)   107486 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thal.c
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thal_main.c
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thal_parameters.c
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thal_parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)    93448 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thalflex.c
--rw-r--r--   0 runner    (1001) docker     (123)    41139 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thalflex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/src/libprimer3/thalflexsignatures.h
--rw-r--r--   0 runner    (1001) docker     (123)    24108 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/thermoanalysis.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    79451 2023-05-16 16:13:43.000000 primer3-py-1.2.2/primer3/thermoanalysis.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.639435 primer3-py-1.2.2/primer3_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-16 16:13:49.000000 primer3-py-1.2.2/primer3_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-16 16:13:49.000000 primer3-py-1.2.2/primer3_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:13:49.000000 primer3-py-1.2.2/primer3_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:13:49.000000 primer3-py-1.2.2/primer3_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 16:13:49.000000 primer3-py-1.2.2/primer3_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-16 16:13:49.651435 primer3-py-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-16 16:13:43.000000 primer3-py-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.639435 primer3-py-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/_simulatedbindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/checkdatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:13:49.651435 primer3-py-1.2.2/tests/input_files/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/dv_conc_vs_dntp_conc_input
--rw-r--r--   0 runner    (1001) docker     (123)   119850 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/long_seq_input
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/p3-tmpl-mispriming_input
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/p3_3_prime_0_input
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/p3_3_prime_n_input
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer1_input
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer1_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer3_v1_1_4_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer3web_v0_4_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer3web_v3_0_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer3web_v4_0_0_default_settings_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_all_settingsfiles_input
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_annealing_temp_input
--rw-r--r--   0 runner    (1001) docker     (123)    41194 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_boundary1_input
--rw-r--r--   0 runner    (1001) docker     (123)    45207 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_boundary_input
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_check_input
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_dmso_formamide_input
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_end_pathology_input
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_first_base_index_input
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_gc_end_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_high_gc_load_set_input
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_high_tm_load_set_input
--rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_human_input
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_input
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_internal1_input
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_internal_input
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_internal_position_input
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_lib_amb_codes_input
--rw-r--r--   0 runner    (1001) docker     (123)    95632 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_masker_input
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_mispriming_boundary1_input
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_mispriming_boundary2_input
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_mispriming_input
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_mispriming_long_lib_input
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_mispriming_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_must_match_input
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_must_overlap_point_input
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_must_use_input
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_must_use_op_input
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_must_use_th_input
--rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_new_tasks_input
--rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_new_tasks_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_num_best_input
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_obj_fn_input
--rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_ok_regions2_input
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_ok_regions_input
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_overhang_input
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_overhang_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_overlap_junction_input
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_poly_x_input
--rw-r--r--   0 runner    (1001) docker     (123)    52293 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_position_penalty_input
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_quality_boundary_input
--rw-r--r--   0 runner    (1001) docker     (123)   141931 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_rat_input
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_renewed_tasks_input
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_sec_struct_dpal_input
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_sec_struct_thal_input
--rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_start_codon_input
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_syntax_input
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_task_input
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_task_th_input
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_thal_args_input
--rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_thal_max_seq_error_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    12821 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_thermod_align_input
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_three_prime_distance_input
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_tm_lc_masking_input
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/primer_windows_newlines_input
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/test_compl_error_input
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/test_left_to_right_of_right_input
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/th-w-other-tasks_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/thal_input
--rwxr-xr-x   0 runner    (1001) docker     (123)    45696 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/input_files/thal_output
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_argdefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_ntthal_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_p3helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19790 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_primerdesign.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_thermoanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/test_threadsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-16 16:13:43.000000 primer3-py-1.2.2/tests/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.773731 primer3-py-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-31 15:46:32.000000 primer3-py-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-31 15:46:32.000000 primer3-py-2.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-31 15:46:32.000000 primer3-py-2.0.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-31 15:46:32.000000 primer3-py-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-31 15:46:32.000000 primer3-py-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-31 15:46:37.773731 primer3-py-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-31 15:46:32.000000 primer3-py-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 15:46:32.000000 primer3-py-2.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.749730 primer3-py-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.749730 primer3-py-2.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/api/bindings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/api/p3helpers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/api/thermoanalysis.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/changes_link.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/cython_help.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/miscellany.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-31 15:46:32.000000 primer3-py-2.0.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.749730 primer3-py-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-31 15:46:32.000000 primer3-py-2.0.0/examples/basicprimerdesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-31 15:46:32.000000 primer3-py-2.0.0/examples/orthogonalprimers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.753731 primer3-py-2.0.0/primer3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/argdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/p3helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/p3helpers.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.749730 primer3-py-2.0.0/primer3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.757731 primer3-py-2.0.0/primer3/src/libprimer3/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/ABOUT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/amplicontm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/amplicontm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/amplicontm_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38114 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/dpal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/dpal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/format_output.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/format_output.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/gpl-2.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.757731 primer3-py-2.0.0/primer3/src/libprimer3/klib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/klib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/klib/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)   349788 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/libprimer3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58440 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/libprimer3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   342539 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/libprimer3flex.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/libprimer3flex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/long_seq_tm_test_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/masker.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/masker.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/masker_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/ntdpal_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/oligotm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/oligotm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/oligotm_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/p3_seq_lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/p3_seq_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_boulder_main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.757731 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/dangle.ds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.761731 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/triloop_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/loops.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/loops.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stack.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stackmm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stackmm.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tetraloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tetraloop.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/triloop.ds
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack2.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack2.ds
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds
+-rw-r--r--   0 runner    (1001) docker     (123)    24711 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/print_boulder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/print_boulder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/read_boulder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/read_boulder.h
+-rw-r--r--   0 runner    (1001) docker     (123)   107516 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thal_main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thal_parameters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thal_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93477 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thalflex.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41139 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thalflex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/src/libprimer3/thalflexsignatures.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/thermoanalysis.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/thermoanalysis.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)    88578 2023-05-31 15:46:32.000000 primer3-py-2.0.0/primer3/thermoanalysis.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.761731 primer3-py-2.0.0/primer3_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-31 15:46:37.000000 primer3-py-2.0.0/primer3_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-31 15:46:37.000000 primer3-py-2.0.0/primer3_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:37.000000 primer3-py-2.0.0/primer3_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:37.000000 primer3-py-2.0.0/primer3_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 15:46:37.000000 primer3-py-2.0.0/primer3_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 15:46:37.773731 primer3-py-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-05-31 15:46:32.000000 primer3-py-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.761731 primer3-py-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/_simulatedbindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/checkdatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:37.773731 primer3-py-2.0.0/tests/input_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/dv_conc_vs_dntp_conc_input
+-rw-r--r--   0 runner    (1001) docker     (123)   119850 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/long_seq_input
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/p3-tmpl-mispriming_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/p3_3_prime_0_input
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/p3_3_prime_n_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer1_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer1_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer3_v1_1_4_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer3web_v0_4_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer3web_v3_0_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer3web_v4_0_0_default_settings_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_all_settingsfiles_input
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_annealing_temp_input
+-rw-r--r--   0 runner    (1001) docker     (123)    41194 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_boundary1_input
+-rw-r--r--   0 runner    (1001) docker     (123)    45207 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_boundary_input
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_check_input
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_dmso_formamide_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_end_pathology_input
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_first_base_index_input
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_gc_end_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_high_gc_load_set_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_high_tm_load_set_input
+-rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_human_input
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_internal1_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_internal_input
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_internal_position_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_lib_amb_codes_input
+-rw-r--r--   0 runner    (1001) docker     (123)    95632 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_masker_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_mispriming_boundary1_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_mispriming_boundary2_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_mispriming_input
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_mispriming_long_lib_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_mispriming_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_must_match_input
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_must_overlap_point_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_must_use_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_must_use_op_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_must_use_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_new_tasks_input
+-rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_new_tasks_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_num_best_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_obj_fn_input
+-rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_ok_regions2_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_ok_regions_input
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_overhang_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_overhang_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_overlap_junction_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_poly_x_input
+-rw-r--r--   0 runner    (1001) docker     (123)    52293 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_position_penalty_input
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_quality_boundary_input
+-rw-r--r--   0 runner    (1001) docker     (123)   141931 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_rat_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_renewed_tasks_input
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_sec_struct_dpal_input
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_sec_struct_thal_input
+-rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_start_codon_input
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_syntax_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_task_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_task_th_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_thal_args_input
+-rw-r--r--   0 runner    (1001) docker     (123)    20583 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_thal_max_seq_error_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12821 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_thermod_align_input
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_three_prime_distance_input
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_tm_lc_masking_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/primer_windows_newlines_input
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/test_compl_error_input
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/test_left_to_right_of_right_input
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/th-w-other-tasks_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/thal_input
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45696 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/input_files/thal_output
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_argdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_ntthal_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_p3helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22742 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_primerdesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_thermoanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/test_threadsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-31 15:46:32.000000 primer3-py-2.0.0/tests/wrappers.py
```

### Comparing `primer3-py-1.2.2/.pre-commit-config.yaml` & `primer3-py-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/AUTHORS` & `primer3-py-2.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/CHANGES` & `primer3-py-2.0.0/CHANGES`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 # Changelog
 
+## Version 2.0.0 (May 30, 2023)
+
+- Migrated primer3 header file Cython extern imports to `thermoanalysis.pxi`
+- Optional C structure string argument `c_ascii_structure` added to `_ThermoAnalysis` methods to enable 3rd party use for structures
+- Version bump to 2.0.0 due to breaking change
+- Fix issue whereby no_structure is not correctly 1 set to 1 when no secondary structure in found
+- Add list version of `PRIMER_{PAIR, LEFT, RIGHT, INTERNAL}` to design output dictionary keys.Retaining original keys as well for compatibility.
+- Fix for  missing `thal_result.sec_struct` and `dpal_results.sec_struct` initialization to `NULL` in `recalc_primer_sec_struct`
+
 ## Version 1.2.2 (May 16, 2023)
+
 - Bug fixes for output formatting related to penalty, "problem", and mispriming fields
 
 ## Version 1.2.1 (April 28, 2023)
+
 - Bug fixes for `pdh_create_seq_lib` to correct missing `seq_lib` datastructure allocation and variable name typos.
 - Increase test coverage to include `misprime_lib` and `mishyb_lib` arguments
 
 ## Version 1.2.0 (March 22, 2023)
 
 - Threadsafe changes made to `thal.c` resulting in new  `thalflex.c` and `thalflex.h` and `thalflexsignatures.h`.
 - Threadsafe changes made to `libprimer3.c` resulting in new  `libprimer3flex.c` and `ibprimer3flex.c.h`.
 - `libprimer3.seq_args` datatype is now renamed to `libprimer3.seq_args_t`
 - `test_threadsafe.py` add and `nogil` instituted for calls to `thal()` and `seqtm()` added `run_design` and `calc_heterodimer` threadsafe tests
 - `ThermoAnalysis` class no longer needs to be a `Singleton` so this was removed as a parent class
 - `p3helpers.pyx` houses new sequence and design helper functions
 - `setup.py` `package_data` and `MANIFEST.in` to assist with future builds from `tar.gz` (`conda`)
 
 ## Version 1.1.0 (March 1, 2023)
+
  - Added specificity to error non-N IUPAC error for issue #59
  - Wheel build support for python 3.8 to move towards following the CPython EOL model for issue #88. See https://devguide.python.org/versions/
 
 
 ## Version 1.0.0 (February 11, 2023)
 
 - Migrated `primer3` source to 2.6.1 version, which adds new arguments for melting temperature code
```

### Comparing `primer3-py-1.2.2/LICENSE` & `primer3-py-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/MANIFEST.in` & `primer3-py-2.0.0/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 include README.md LICENSE CHANGES AUTHORS setup.py
 include .pre-commit-config.yaml dev-requirements.txt setup.cfg
-include primer3/*.pxd primer3/*.pyx primer3/*.h
+include primer3/*.pxd primer3/*.pxi primer3/*.pyx primer3/*.h
 include primer3/src/libprimer3/*.h primer3/src/libprimer3/*.c
 include primer3/src/libprimer3/klib/khash.h
 include primer3/src/libprimer3/klib/README.md
 include primer3/src/libprimer3/gpl-2.0.txt
 include primer3/src/libprimer3/ABOUT.txt
 include primer3/src/libprimer3/primer3_config/*.ds
 include primer3/src/libprimer3/primer3_config/*.dh
```

### Comparing `primer3-py-1.2.2/PKG-INFO` & `primer3-py-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primer3-py
-Version: 1.2.2
+Version: 2.0.0
 Summary: Python bindings for Primer3
 Home-page: https://github.com/libnano/primer3-py
 Author: Ben Pruitt, Nick Conway
 Author-email: bpruittvt@gmail.com
 License: GPLv2
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: primer3-py Version: 1.2.2 Summary: Python bindings
+Metadata-Version: 2.1 Name: primer3-py Version: 2.0.0 Summary: Python bindings
 for Primer3 Home-page: https://github.com/libnano/primer3-py Author: Ben
 Pruitt, Nick Conway Author-email: bpruittvt@gmail.com License: GPLv2
 Classifier: Programming Language :: C Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 4 - Beta
```

### Comparing `primer3-py-1.2.2/README.md` & `primer3-py-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/Makefile` & `primer3-py-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/conf.py` & `primer3-py-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/cython_help.md` & `primer3-py-2.0.0/docs/cython_help.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,8 +36,12 @@
     ...
     my_ext = Extension(
         ...
         include_dirs=primer3.includes()
         ...)
 ```
 
-and it should work
+and it should work.
+
+## Notes
+- Many `_ThermoAnalysis` methods (e.g. `calc_heterodimer_c`) have C string argument
+`c_ascii_structure` to enable 3rd party use for structures reuse
```

### Comparing `primer3-py-1.2.2/docs/index.md` & `primer3-py-2.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/make.bat` & `primer3-py-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/miscellany.md` & `primer3-py-2.0.0/docs/miscellany.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/docs/quickstart.md` & `primer3-py-2.0.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/examples/basicprimerdesign.py` & `primer3-py-2.0.0/examples/basicprimerdesign.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/examples/orthogonalprimers.py` & `primer3-py-2.0.0/examples/orthogonalprimers.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/__init__.py` & `primer3-py-2.0.0/primer3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 oligonucleotide thermodynamics library.
 
 '''
 import os
 from typing import List
 
 # Per PEP-440 https://peps.python.org/pep-0440/#public-version-identifiers
-__version__ = '1.2.2'
+__version__ = '2.0.0'
 __author__ = 'Ben Pruitt, Nick Conway'
 __copyright__ = (
     'Copyright 2014-2023, Ben Pruitt & Nick Conway; 2014-2018 Wyss Institute'
 )
 __license__ = 'GPLv2'
 DESCRIPTION = 'Python bindings for Primer3'
```

### Comparing `primer3-py-1.2.2/primer3/argdefaults.py` & `primer3-py-2.0.0/primer3/argdefaults.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/bindings.py` & `primer3-py-2.0.0/primer3/bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,15 @@
 def design_primers(
         seq_args: Dict[str, Any],
         global_args: Dict[str, Any],
         misprime_lib: Optional[Dict[str, Any]] = None,
         mishyb_lib: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
     '''Run the Primer3 design process.
+    This is a wrapper around :meth:`_ThermoAnalysis.run_design`.
 
     Args:
         seq_args: Primer3 sequence/design args as per Primer3 docs
         global_args: Primer3 global args as per Primer3 docs
         misprime_lib: `Sequence name: sequence` dictionary for mispriming
             checks.
         mishyb_lib: `Sequence name: sequence` dictionary for mishybridization
```

### Comparing `primer3-py-1.2.2/primer3/p3helpers.h` & `primer3-py-2.0.0/primer3/p3helpers.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/p3helpers.pyx` & `primer3-py-2.0.0/primer3/p3helpers.pyx`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/LICENSE.txt` & `primer3-py-2.0.0/primer3/src/libprimer3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/Makefile` & `primer3-py-2.0.0/primer3/src/libprimer3/Makefile`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/amplicontm.c` & `primer3-py-2.0.0/primer3/src/libprimer3/amplicontm.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/amplicontm.h` & `primer3-py-2.0.0/primer3/src/libprimer3/amplicontm.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/amplicontm_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/amplicontm_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/dpal.c` & `primer3-py-2.0.0/primer3/src/libprimer3/dpal.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/dpal.h` & `primer3-py-2.0.0/primer3/src/libprimer3/dpal.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/format_output.c` & `primer3-py-2.0.0/primer3/src/libprimer3/format_output.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/format_output.h` & `primer3-py-2.0.0/primer3/src/libprimer3/format_output.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/gpl-2.0.txt` & `primer3-py-2.0.0/primer3/src/libprimer3/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/klib/README.md` & `primer3-py-2.0.0/primer3/src/libprimer3/klib/README.md`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/klib/khash.h` & `primer3-py-2.0.0/primer3/src/libprimer3/klib/khash.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/libprimer3.c` & `primer3-py-2.0.0/primer3/src/libprimer3/libprimer3.c`

 * *Files 0% similar despite different names*

```diff
@@ -5279,16 +5279,15 @@
       );
     }
   } else {
     /* Get how may primers should be max. printed */
     num_print = retval->best_pairs.num_pairs;
     for (int i = 0 ; i < num_print ; i++) {
       recalc_primer_sec_struct(
-        retval->best_pairs.pairs[i].
-        left,
+        retval->best_pairs.pairs[i].left,
         0,
         pa,
         sa,
         dpal_arg_to_use,
         thal_arg_to_use
       );
       recalc_primer_sec_struct(
@@ -5377,14 +5376,18 @@
       );
     }
     p3_reverse_complement(s1_rev, s1);
   }
 
   if (pa->thermodynamic_oligo_alignment==0) {
     dpal_results any, end;
+    /* NOTE: important to set these values to NULL to prevent segfaults */
+    any.sec_struct = NULL;
+    end.sec_struct = NULL;
+
     if (p_rec->self_any > 0.0) {
       dpal((const unsigned char *) s1, (const unsigned char *) s1_rev,
            dpal_arg_to_use->local, DPM_STRUCT, &any);
       p_rec->self_any = any.score / PR_ALIGN_SCORE_PRECISION;
       save_overwrite_sec_struct(&p_rec->self_any_struct, any.sec_struct);
     }
     if (p_rec->self_end > 0.0) {
@@ -5393,14 +5396,19 @@
       p_rec->self_end = end.score / PR_ALIGN_SCORE_PRECISION;
       save_overwrite_sec_struct(&p_rec->self_end_struct, end.sec_struct);
     }
   }
   /* Thermodynamic approach, fwd-primer */
   if (pa->thermodynamic_oligo_alignment==1) {
     thal_results any, end, hair;
+    /* NOTE: important to set these values to NULL to prevent segfaults */
+    any.sec_struct = NULL;
+    end.sec_struct = NULL;
+    hair.sec_struct = NULL;
+
     if (p_rec->self_any > 0.0 ) {
       thal(
         (const unsigned char *) s1,
         (const unsigned char *) s1,
         thal_arg_to_use->any,
         THL_STRUCT,
         &any,
```

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/libprimer3.h` & `primer3-py-2.0.0/primer3/src/libprimer3/libprimer3.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/libprimer3flex.c` & `primer3-py-2.0.0/primer3/src/libprimer3/libprimer3flex.c`

 * *Files 0% similar despite different names*

```diff
@@ -6178,16 +6178,15 @@
       );
     }
   } else {
     /* Get how may primers should be max. printed */
     num_print = retval->best_pairs.num_pairs;
     for (int i = 0 ; i < num_print ; i++) {
       recalc_primer_sec_struct(
-        retval->best_pairs.pairs[i].
-        left,
+        retval->best_pairs.pairs[i].left,
         0,
         pa,
         sa,
         dpal_arg_to_use,
         thal_arg_to_use
       );
       recalc_primer_sec_struct(
@@ -6228,15 +6227,15 @@
     const seq_args_t* sa,
     const dpal_arg_holder* dpal_arg_to_use,
     const thal_arg_holder* thal_arg_to_use
 ) {
   char s1[THAL_MAX_ALIGN+1], s1_rev[THAL_MAX_ALIGN+1];
   int overhang_len;
   /* s1 is the forward oligo. */
-  if (primer_type == 0) {  /*left */
+  if (primer_type == 0) {  /* left */
     if (NULL != sa->overhang_left) {
       overhang_len = strlen(sa->overhang_left);
       strcpy(s1, sa->overhang_left);
       _pr_shift_substr(
         sa->trimmed_seq,
         p_rec->start,
         p_rec->length,
@@ -6283,17 +6282,19 @@
         p_rec->start - p_rec->length + 1,
         p_rec->length,
         s1_rev
       );
     }
     p3_reverse_complement(s1_rev, s1);
   }
-
   if (pa->thermodynamic_oligo_alignment==0) {
     dpal_results any, end;
+    /* NOTE: important to set these values to NULL to prevent segfaults */
+    any.sec_struct = NULL;
+    end.sec_struct = NULL;
     if (p_rec->self_any > 0.0) {
       dpal(
         (const unsigned char*) s1,
         (const unsigned char*) s1_rev,
         dpal_arg_to_use->local,
         DPM_STRUCT,
         &any
@@ -6318,14 +6319,19 @@
         end.sec_struct
       );
     }
   }
   /* Thermodynamic approach, fwd-primer */
   if (pa->thermodynamic_oligo_alignment==1) {
     thal_results any, end, hair;
+    /* NOTE: important to set these values to NULL to prevent segfaults */
+    any.sec_struct = NULL;
+    end.sec_struct = NULL;
+    hair.sec_struct = NULL;
+
     if (p_rec->self_any > 0.0 ) {
       thal(
         (const unsigned char*) s1,
         (const unsigned char*) s1,
         thal_arg_to_use->any,
         THL_STRUCT,
         &any,
```

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/libprimer3flex.h` & `primer3-py-2.0.0/primer3/src/libprimer3/libprimer3flex.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/long_seq_tm_test_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/long_seq_tm_test_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/masker.c` & `primer3-py-2.0.0/primer3/src/libprimer3/masker.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/masker.h` & `primer3-py-2.0.0/primer3/src/libprimer3/masker.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/masker_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/masker_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/ntdpal_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/ntdpal_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/oligotm.c` & `primer3-py-2.0.0/primer3/src/libprimer3/oligotm.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/oligotm.h` & `primer3-py-2.0.0/primer3/src/libprimer3/oligotm.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/oligotm_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/oligotm_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/p3_seq_lib.c` & `primer3-py-2.0.0/primer3/src/libprimer3/p3_seq_lib.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/p3_seq_lib.h` & `primer3-py-2.0.0/primer3/src/libprimer3/p3_seq_lib.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_boulder_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_boulder_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/dangle.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/dangle.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/dangle_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/loops_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stack_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/stackmm_i_mm.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tetraloop_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack2_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/interpretations/tstack_tm_inf_i.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/loops.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/loops.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stack.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stack.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stack.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stack.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stackmm.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stackmm.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/stackmm.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/stackmm.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tetraloop.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tetraloop.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tetraloop.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tetraloop.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack2.dh` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack2.dh`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack2.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack2.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds` & `primer3-py-2.0.0/primer3/src/libprimer3/primer3_config/tstack_tm_inf.ds`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/print_boulder.c` & `primer3-py-2.0.0/primer3/src/libprimer3/print_boulder.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/print_boulder.h` & `primer3-py-2.0.0/primer3/src/libprimer3/print_boulder.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/read_boulder.c` & `primer3-py-2.0.0/primer3/src/libprimer3/read_boulder.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/read_boulder.h` & `primer3-py-2.0.0/primer3/src/libprimer3/read_boulder.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thal.c` & `primer3-py-2.0.0/primer3/src/libprimer3/thal.c`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
    structure for dimer or for monomer */
 void
 thal(const unsigned char *oligo_f,
      const unsigned char *oligo_r,
      const thal_args *a,
      const thal_mode mode,
      thal_results *o,
-     const int print_output)  /* primer3-py modification argumen */
+     const int print_output)  /* primer3-py modification argument */
 {
   double* SH;
   int i, j;
   int len_f, len_r;
   // double T1; primer3-py commented out variable
   int k;
   int *bp;
@@ -676,14 +676,15 @@
         drawHairpin(bp, mh, ms, do_temponly, a->temp, o);
       }
 
     } else if((mode != THL_FAST) && (mode != THL_DEBUG_F) && (mode != THL_STRUCT)) {
         if (print_output == 1) { /* primer3-py update to supress undesired printing */
           fputs("No secondary structure could be calculated\n", stderr);
         }
+        o->no_structure = 1;
     }
 
     if(o->temp == -_INFINITY && (!strcmp(o->msg, ""))) { o->temp=0.0; }
     free(bp);
     free(enthalpyDPT);
     free(entropyDPT);
     free(numSeq1);
```

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thal.h` & `primer3-py-2.0.0/primer3/src/libprimer3/thal.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thal_main.c` & `primer3-py-2.0.0/primer3/src/libprimer3/thal_main.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thal_parameters.c` & `primer3-py-2.0.0/primer3/src/libprimer3/thal_parameters.c`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thal_parameters.h` & `primer3-py-2.0.0/primer3/src/libprimer3/thal_parameters.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thalflex.c` & `primer3-py-2.0.0/primer3/src/libprimer3/thalflex.c`

 * *Files 0% similar despite different names*

```diff
@@ -648,14 +648,15 @@
         );
       }
 
     } else if((mode != THL_FAST) && (mode != THL_DEBUG_F) && (mode != THL_STRUCT)) {
         if (print_output == 1) { /* primer3-py update to supress undesired printing */
           fputs("No secondary structure could be calculated\n", stderr);
         }
+        o->no_structure = 1;
     }
 
     if(o->temp == -_INFINITY && (!strcmp(o->msg, ""))) { o->temp=0.0; }
     free(bp);
     free(enthalpyDPT);
     free(entropyDPT);
     free(numSeq1);
```

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thalflex.h` & `primer3-py-2.0.0/primer3/src/libprimer3/thalflex.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/src/libprimer3/thalflexsignatures.h` & `primer3-py-2.0.0/primer3/src/libprimer3/thalflexsignatures.h`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/primer3/thermoanalysis.pxd` & `primer3-py-2.0.0/primer3/thermoanalysis.pxi`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 '''
-thermoanalysis.pxd
+thermoanalysis.pxi
 ~~~~~~~~~~~~~~~~~~
 
-Cython header file for thermoanalysis.pyx -- allows for cross-project Cython /
-C integration of the low-level thermodynamic analysis bindings.
+Cython INCLUDE file for thermoanalysis.pyx
 
 '''
+
 from libc.float cimport DBL_MAX
 from libc.stdio cimport FILE
 from libc.stdlib cimport free
 from libc.string cimport strlen
 
 
 cdef extern from "thal.h":
@@ -587,101 +587,7 @@
         seq_args_t*sarg,
         pr_append_str *fatal_err,
         pr_append_str *nonfatal_err,
         pr_append_str *warnings,
         read_boulder_record_results *,
         char*
     )
-
-
-cdef class ThermoResult:
-    cdef thal_results thalres
-    cdef public object ascii_structure
-
-
-cdef class _ThermoAnalysis:
-    cdef:
-        thal_args thalargs
-        int eval_mode
-        public int max_nn_length
-        public int _tm_method
-        public object _tm_methods_int_dict
-
-        public int _salt_correction_method
-        public object _salt_correction_methods_int_dict
-
-        public float dmso_conc
-        public float dmso_fact
-        public float formamide_conc
-        public float annealing_temp_c
-
-        p3_global_settings* global_settings_data
-        seq_args_t* sequence_args_data
-
-    cdef inline ThermoResult calc_heterodimer_c(
-            _ThermoAnalysis self,
-            unsigned char* s1,
-            unsigned char* s2,
-            bint output_structure
-    )
-
-    cdef inline ThermoResult calc_homodimer_c(
-            _ThermoAnalysis self,
-            unsigned char* s1,
-            bint output_structure
-    )
-
-    cdef inline ThermoResult calc_hairpin_c(
-            _ThermoAnalysis self,
-            unsigned char* s1,
-            bint output_structure
-    )
-
-    cdef inline ThermoResult calc_end_stability_c(
-            _ThermoAnalysis self,
-            unsigned char* s1,
-            unsigned char* s2,
-    )
-
-    cdef inline double calc_tm_c(_ThermoAnalysis self, char* s1)
-
-    cpdef ThermoResult calc_heterodimer(
-            _ThermoAnalysis self,
-            object seq1,
-            object seq2,
-            bint output_structure = *,
-    )
-
-    cpdef ThermoResult calc_homodimer(
-            _ThermoAnalysis self,
-            object seq1,
-            bint output_structure = *,
-    )
-
-    cpdef ThermoResult calc_hairpin(
-            _ThermoAnalysis self,
-            object seq1,
-            bint output_structure = *,
-    )
-
-    cpdef tuple mispriming_check(
-            _ThermoAnalysis self,
-            object putative_seq,
-            object sequences,
-            double tm_threshold,
-    )
-
-cdef:
-    int pdh_wrap_set_seq_args_globals(
-        p3_global_settings* global_settings_data,
-        seq_args_t* sequence_args_data,
-        object kmer_lists_path,
-        char* in_buffer,
-    ) except -1
-
-    seq_lib* pdh_create_seq_lib(object seq_dict) except NULL
-
-    object pdh_design_output_to_dict(
-        const p3_global_settings* global_settings_data,
-        const seq_args_t* sequence_args_data,
-        const p3retval *retval,
-    )
```

### Comparing `primer3-py-1.2.2/primer3/thermoanalysis.pyx` & `primer3-py-2.0.0/primer3/thermoanalysis.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 from primer3 import argdefaults
 
 _DID_LOAD_THERM_PARAMS = False
 _DEFAULT_WORD_LEN_2 = 16  # see masker.h
 DEFAULT_P3_ARGS = argdefaults.Primer3PyArguments()
 SNAKE_CASE_DEPRECATED_MSG = 'Function deprecated please use "%s" instead'
 
+include 'thermoanalysis.pxi'
+
 # This lock is required for thread safety for 1.0.0 major release.
 # The goal is remove this requirement in related changes in v1.1.x+ minor
 # release
 
 
 Str_Bytes_T = Union[str, bytes]
 
@@ -445,20 +447,24 @@
 
     def __dealloc__(self):
         '''Cleanup memory for design data structures
 
         '''
         if self.global_settings_data != NULL:
             # Free memory for previous global settings
-            p3_destroy_global_settings(self.global_settings_data)
+            p3_destroy_global_settings(
+                <p3_global_settings*> self.global_settings_data
+            )
             self.global_settings_data = NULL
 
         if self.sequence_args_data != NULL:
             # Free memory for previous seq args
-            destroy_seq_args(self.sequence_args_data)
+            destroy_seq_args(
+                <seq_args_t*> self.sequence_args_data
+            )
             self.sequence_args_data = NULL
 
 
     # ~~~~~~~~~~~~~~~~~~~~~~ Property getters / setters ~~~~~~~~~~~~~~~~~~~~~ #
     @property
     def mv_conc(self) -> float:
         ''' Concentration of monovalent cations (mM) '''
@@ -609,58 +615,70 @@
     # ~~~~~~~~~~~~~~ Thermodynamic calculation instance methods ~~~~~~~~~~~~~ #
 
     cdef inline ThermoResult calc_heterodimer_c(
             _ThermoAnalysis self,
             unsigned char *s1,
             unsigned char *s2,
             bint output_structure,
+            char* c_ascii_structure,
     ):
         '''
         C only heterodimer computation
 
         Args:
             s1: sequence string 1
             s2: sequence string 2
             output_structure: If True, build output structure.
+            c_ascii_structure: Optional C structure string
 
         Returns:
             Computed heterodimer result
 
         '''
         cdef:
             ThermoResult tr_obj = ThermoResult()
-            char* c_ascii_structure = NULL
+            bint did_allocate = 0
 
         self.thalargs.dimer = 1
         self.thalargs.type = <thal_alignment_type> 1 # thal_alignment_any
         if output_structure:
-            c_ascii_structure = <char *>malloc(
-                (strlen(<const char*>s1) + strlen(<const char*>s2)) * 4 + 24)
-            c_ascii_structure[0] = b'\0'
+            if c_ascii_structure == NULL:
+                c_ascii_structure = <char*> malloc(
+                    (
+                        (strlen(<const char*> s1) +
+                        strlen(<const char*> s2)) * 4 +
+                        24
+                    )
+                )
+                c_ascii_structure[0] = b'\0'
+                did_allocate = 1
             tr_obj.thalres.sec_struct = c_ascii_structure
 
         cdef:
-            thal_args* targs = &self.thalargs
+            thal_args* targs = <thal_args*> &self.thalargs
             int emode = self.eval_mode
-            thal_results* thalres = &tr_obj.thalres
+            thal_results* thalres = <thal_results*> &tr_obj.thalres
             int do_output = 1 if output_structure else 0
+
         with nogil:
             thal(
                 <const unsigned char*> s1,
                 <const unsigned char*> s2,
-                <const thal_args *> targs,
+                <const thal_args*> targs,
                 <const thal_mode> emode,
                 thalres,
                 do_output,
             )
         if output_structure:
             try:
                 tr_obj.ascii_structure = c_ascii_structure.decode('utf8')
             finally:
-                free(tr_obj.thalres.sec_struct)
+                if did_allocate:
+                    free(c_ascii_structure)
+                    c_ascii_structure = NULL
                 tr_obj.thalres.sec_struct = NULL
         return tr_obj
 
     cpdef ThermoResult calc_heterodimer(
             _ThermoAnalysis self,
             object seq1,
             object seq2,
@@ -687,14 +705,15 @@
         cdef unsigned char* s2 = py_s2
 
         tr_obj = _ThermoAnalysis.calc_heterodimer_c(
             <_ThermoAnalysis> self,
             s1,
             s2,
             output_structure,
+            NULL,
         )
         return tr_obj
 
     cpdef tuple mispriming_check(
             _ThermoAnalysis self,
             object putative_seq,
             object sequences,
@@ -734,71 +753,78 @@
             py_s2 = <bytes> _bytes(seq)
             s2 = py_s2
             offtarget_tm = _ThermoAnalysis.calc_heterodimer_c(
                 <_ThermoAnalysis> self,
                 s1,
                 s2,
                 0,
+                NULL,
             ).tm
             if offtarget_tm > max_offtarget_tm:
                 max_offtarget_seq_idx = i
                 max_offtarget_tm = offtarget_tm
             if offtarget_tm > tm_threshold:
                 is_offtarget = True
                 break
         return is_offtarget, max_offtarget_seq_idx, max_offtarget_tm
 
     cdef inline ThermoResult calc_homodimer_c(
             _ThermoAnalysis self,
             unsigned char *s1,
             bint output_structure,
+            char* c_ascii_structure,
     ):
         '''
         C only homodimer computation
 
         Args:
             s1: sequence string 1
             output_structure: If True, build output structure.
+            c_ascii_structure: Optional C structure string
 
         Returns:
             Computed homodimer ``ThermoResult``
 
         '''
         cdef:
             ThermoResult tr_obj = ThermoResult()
-            char* c_ascii_structure = NULL
+            thal_args* targs = <thal_args*> &self.thalargs
+            int emode = self.eval_mode
+            thal_results* thalres = <thal_results*> &tr_obj.thalres
+            int do_output = 1 if output_structure else 0
+            bint did_allocate = 0
 
         self.thalargs.dimer = 1
         self.thalargs.type = <thal_alignment_type> 1 # thal_alignment_any
+
         if output_structure:
-            c_ascii_structure = <char *> malloc(
-                (strlen(<const char*> s1) * 8 + 24)
-            )
-            c_ascii_structure[0] = b'\0'
+            if c_ascii_structure == NULL:
+                did_allocate = 1
+                c_ascii_structure = <char *> malloc(
+                    (strlen(<const char*> s1) * 8 + 24)
+                )
+                c_ascii_structure[0] = b'\0'
             tr_obj.thalres.sec_struct = c_ascii_structure
 
-        cdef:
-            thal_args* targs = &self.thalargs
-            int emode = self.eval_mode
-            thal_results* thalres = &tr_obj.thalres
-            int do_output = 1 if output_structure else 0
         with nogil:
             thal(
                 <const unsigned char*> s1,
                 <const unsigned char*> s1,
-                <const thal_args *> targs,
+                <const thal_args*> targs,
                 <const thal_mode> emode,
                 thalres,
                 do_output,
             )
         if output_structure:
             try:
                 tr_obj.ascii_structure = c_ascii_structure.decode('utf8')
             finally:
-                free(c_ascii_structure)
+                if did_allocate:
+                    free(c_ascii_structure)
+                    c_ascii_structure = NULL
                 tr_obj.thalres.sec_struct = NULL
         return tr_obj
 
     cpdef ThermoResult calc_homodimer(
             _ThermoAnalysis self,
             object seq1,
             bint output_structure = False,
@@ -819,65 +845,72 @@
         py_s1 = <bytes> _bytes(seq1)
         cdef unsigned char* s1 = py_s1
 
         return _ThermoAnalysis.calc_homodimer_c(
             <_ThermoAnalysis> self,
             s1,
             output_structure,
+            NULL,
         )
 
     cdef inline ThermoResult calc_hairpin_c(
             _ThermoAnalysis self,
             unsigned char *s1,
             bint output_structure,
+            char* c_ascii_structure,
     ):
         '''
         C only hairpin computation
 
         Args:
             s1: sequence string 1
             output_structure: If True, build output structure.
+            c_ascii_structure: Optional C structure string
 
         Returns:
             Computed hairpin ``ThermoResult``
 
         '''
         cdef:
             ThermoResult tr_obj = ThermoResult()
-            char* c_ascii_structure = NULL
+            bint did_allocate = 0
 
         self.thalargs.dimer = 0
         self.thalargs.type = <thal_alignment_type> 4 # thal_alignment_hairpin
         if output_structure:
-            c_ascii_structure = <char *> malloc(
-                (strlen(<const char*> s1) * 2 + 64)
-            )
-            c_ascii_structure[0] = b'\0'
+            if c_ascii_structure == NULL:
+                c_ascii_structure = <char*> malloc(
+                    (strlen(<const char*> s1) * 2 + 64)
+                )
+                c_ascii_structure[0] = b'\0'
+                did_allocate = 1
             tr_obj.thalres.sec_struct = c_ascii_structure
 
         cdef:
-            thal_args* targs = &self.thalargs
+            thal_args* targs = <thal_args*> &self.thalargs
             int emode = self.eval_mode
-            thal_results* thalres = &tr_obj.thalres
+            thal_results* thalres = <thal_results*> &tr_obj.thalres
             int do_output = 1 if output_structure else 0
         with nogil:
             thal(
                 <const unsigned char*> s1,
                 <const unsigned char*> s1,
-                <const thal_args *> targs,
+                <const thal_args*> targs,
                 <const thal_mode> emode,
                 thalres,
                 do_output,
             )
 
         if output_structure:
             try:
                 tr_obj.ascii_structure = c_ascii_structure.decode('utf8')
             finally:
-                free(c_ascii_structure)
+                if did_allocate:
+                    free(c_ascii_structure)
+                    c_ascii_structure = NULL
                 tr_obj.thalres.sec_struct = NULL
         return tr_obj
 
     cpdef ThermoResult calc_hairpin(
             _ThermoAnalysis self,
             object seq1,
             bint output_structure = False,
@@ -898,14 +931,15 @@
         py_s1 = <bytes> _bytes(seq1)
         cdef unsigned char* s1 = py_s1
 
         tr_obj =  _ThermoAnalysis.calc_hairpin_c(
             <_ThermoAnalysis> self,
             s1,
             output_structure,
+            NULL,
         )
         return tr_obj
 
 
     cdef inline ThermoResult calc_end_stability_c(
             _ThermoAnalysis self,
             unsigned char *s1,
@@ -924,23 +958,23 @@
         '''
         cdef ThermoResult tr_obj = ThermoResult()
 
         self.thalargs.dimer = 1
         self.thalargs.type = <thal_alignment_type> 2 # thal_alignment_end1
 
         cdef:
-            thal_args* targs = &self.thalargs
+            thal_args* targs = <thal_args*> &self.thalargs
             int emode = self.eval_mode
-            thal_results* thalres = &tr_obj.thalres
+            thal_results* thalres = <thal_results*> &tr_obj.thalres
 
         with nogil:
             thal(
                 <const unsigned char*> s1,
                 <const unsigned char*> s2,
-                <const thal_args *> targs,
+                <const thal_args*> targs,
                 <const thal_mode> emode,
                 thalres,
                 0,
             )
         return tr_obj
 
     def calc_end_stability(
@@ -971,53 +1005,59 @@
                 <_ThermoAnalysis> self,
                 s1,
                 s2,
             )
         return tr_obj
 
 
-    cdef inline double calc_tm_c(_ThermoAnalysis self, char *s1):
+    cdef inline double calc_tm_c(
+            _ThermoAnalysis self,
+            char *s1,
+    ):
         '''
         C only Tm computation
 
         Args:
             s1: sequence string 1
 
         Returns:
             floating point Tm result
         '''
         cdef:
-            thal_args *ta = &self.thalargs
+            thal_args* targs = <thal_args*> &self.thalargs
             double dmso_conc = self.dmso_conc
             double dmso_fact = self.dmso_fact
             double formamide_conc = self.formamide_conc
             int max_nn_length = self.max_nn_length
             int tmmeth = self._tm_method
             int salt_correction_method = self._salt_correction_method
             double annealing_temp_c = self.annealing_temp_c
             tm_ret tm_val
 
         with nogil:
             tm_val = seqtm(
                 <const char*> s1,
-                ta.dna_conc,
-                ta.mv,
-                ta.dv,
-                ta.dntp,
+                targs.dna_conc,
+                targs.mv,
+                targs.dv,
+                targs.dntp,
                 dmso_conc,
                 dmso_fact,
                 formamide_conc,
                 max_nn_length,
                 <tm_method_type> tmmeth,
                 <salt_correction_type> salt_correction_method,
                 annealing_temp_c,
             )
         return tm_val.Tm
 
-    def calc_tm(_ThermoAnalysis self, seq1: Union[str, bytes]) -> float:
+    def calc_tm(
+            _ThermoAnalysis self,
+            seq1: Union[str, bytes],
+    ) -> float:
         '''Calculate the melting temperature (Tm) of a DNA sequence (deg. C).
 
         Args:
             seq1: (str | bytes) sequence string 1
 
         Returns:
             floating point Tm result
@@ -1048,72 +1088,78 @@
             # 'debug':        self.thalargs.debug,
             'max_nn_length': self.max_nn_length,
             'tm_method':    self.tm_method,
             'salt_correction_method': self.salt_correction_method
         }
 
     def _set_globals_and_seq_args(
-        self,
-        global_args: Dict[str, Any],
-        seq_args: Optional[Dict[str, Any]],
-        misprime_lib: Optional[Dict[str, Any]] = None,
-        mishyb_lib: Optional[Dict[str, Any]] = None,
+            self,
+            global_args: Dict[str, Any],
+            seq_args: Optional[Dict[str, Any]],
+            misprime_lib: Optional[Dict[str, Any]] = None,
+            mishyb_lib: Optional[Dict[str, Any]] = None,
     ) -> None:
         '''
         Sets the Primer3 global settings and sequence settings from a Python
         dictionaries containing `key: value` pairs that correspond to the
         documented Primer3 global and sequence argument parameters.
         Also accepts a mispriming or mishybridization library organized as
         ``seq_name``:``seq_value`` key:value pairs.
 
         Args:
-            seq_args: Primer3 sequence/design args as per Primer3 docs
             global_args: Primer3 global args as per Primer3 docs
+            seq_args: Primer3 sequence/design args as per Primer3 docs
             misprime_lib: `Sequence name: sequence` dictionary for mispriming
                 checks.
             mishyb_lib: `Sequence name: sequence` dictionary for
                 mishybridization checks.
 
         Raises:
             :class:`OSError`: Could not allocate memory
 
         '''
         cdef:
             seq_lib* mp_lib = NULL
             seq_lib* mh_lib = NULL
             char* arg_input_buffer = NULL
+            p3_global_settings* global_settings_data = NULL
+            seq_args_t* sequence_args_data = NULL
 
 
         err_msg = ''
 
         if self.sequence_args_data != NULL:
             # Free memory for previous seq args
-            destroy_seq_args(self.sequence_args_data)
+            destroy_seq_args(
+                <seq_args_t*> self.sequence_args_data
+            )
             self.sequence_args_data = NULL
 
         if seq_args:
-            self.sequence_args_data = create_seq_arg()
+            self.sequence_args_data = <void*> create_seq_arg()
 
             if self.sequence_args_data == NULL:
                 raise OSError('Could not allocate memory for seq_arg')
 
             global_args.update(seq_args)
 
         global_arg_bytes = argdefaults.format_boulder_io(global_args)
         arg_input_buffer = global_arg_bytes
         if arg_input_buffer == NULL:
             raise ValueError(global_arg_bytes)
 
         if self.global_settings_data != NULL:
             # Free memory for previous global settings
-            p3_destroy_global_settings(self.global_settings_data)
+            p3_destroy_global_settings(
+                <p3_global_settings*> self.global_settings_data
+            )
             self.global_settings_data = NULL
 
         # Allocate memory for global settings
-        self.global_settings_data = p3_create_global_settings()
+        self.global_settings_data = <void*> p3_create_global_settings()
         if self.global_settings_data == NULL:
             raise OSError('Could not allocate memory for p3 globals')
 
         kmer_lists_path = global_args.get('PRIMER_MASK_KMERLIST_PATH', '')
         if kmer_lists_path:
             local_dir = op.dirname(op.realpath(get_dunder_file()))
             libprimer3_dir = op.join(local_dir, 'src', 'libprimer3')
@@ -1132,73 +1178,86 @@
                 raise ValueError(
                     f'PRIMER_MASK_KMERLIST_PATH: path {kmer_lists_path} '
                     'not found'
                 )
 
         try:
             pdh_wrap_set_seq_args_globals(
-                self.global_settings_data,
-                self.sequence_args_data,
+                <p3_global_settings*> self.global_settings_data,
+                <seq_args_t*> self.sequence_args_data,
                 kmer_lists_path,
                 arg_input_buffer,
             )
         except BaseException:
             print(
                 f'Issue setting globals. bytes provided: \n\t{global_arg_bytes}'
             )
-            p3_destroy_global_settings(self.global_settings_data)
+            p3_destroy_global_settings(
+                <p3_global_settings*> self.global_settings_data
+            )
             self.global_settings_data = NULL
             if seq_args:
-                destroy_seq_args(self.sequence_args_data)
+                destroy_seq_args(
+                    <seq_args_t*> self.sequence_args_data
+                )
                 self.sequence_args_data = NULL
             raise
 
         # NOTE: This check is super important to prevent errors in edge cases
         if self.global_settings_data == NULL or self.sequence_args_data == NULL:
             raise ValueError(
                 'Error setting Primer3 global args and sequence args\n'
                 'seq_args {seq_args}\n\n'
                 'global_args {global_args}\n\n'
             )
 
         err_msg = ''
         try:
+            global_settings_data = <p3_global_settings*> self.global_settings_data
             if misprime_lib != None:
                 mp_lib = pdh_create_seq_lib(misprime_lib)
                 if mp_lib == NULL:
                     err_msg = f'Issue creating misprime_lib {misprime_lib}'
                     raise ValueError(
                         f'Issue creating misprime_lib {misprime_lib}'
                     )
-                self.global_settings_data[0].p_args.repeat_lib = mp_lib
+
+                global_settings_data[0].p_args.repeat_lib = mp_lib
 
             if mishyb_lib != None:
                 mh_lib = pdh_create_seq_lib(mishyb_lib)
                 if mh_lib == NULL:
                     err_msg = f'Issue creating mishyb_lib: {mishyb_lib}'
                     raise ValueError(err_msg)
-                self.global_settings_data[0].o_args.repeat_lib = mh_lib
+                global_settings_data[0].o_args.repeat_lib = mh_lib
         except (OSError, TypeError) as exc:
-            p3_destroy_global_settings(self.global_settings_data)
+            p3_destroy_global_settings(
+                <p3_global_settings*> self.global_settings_data
+            )
             self.global_settings_data = NULL
-            destroy_seq_args(self.sequence_args_data)
+            destroy_seq_args(
+                <seq_args_t*> self.sequence_args_data
+            )
             self.sequence_args_data = NULL
             raise OSError(err_msg) from exc
 
     def run_design(
-        self,
-        global_args: Dict[str, Any],
-        seq_args: Optional[Dict[str, Any]],
-        misprime_lib: Optional[Dict[str, Any]] = None,
-        mishyb_lib: Optional[Dict[str, Any]] = None,
+            self,
+            global_args: Dict[str, Any],
+            seq_args: Optional[Dict[str, Any]],
+            misprime_lib: Optional[Dict[str, Any]] = None,
+            mishyb_lib: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
-        '''
-        Wraps the primer design functionality of Primer3. Should be called
-        after setting the global and sequence-specific Primer3 parameters
-        (see setGlobals and setSeqArgs, above)
+        '''Wraps the primer design functionality of Primer3.
+
+        .. versionadded:: 2.0.0
+            List versions of `PRIMER_{PAIR, LEFT, RIGHT, INTERNAL}` are added
+            to the design output dictionary keys as a convenience.
+            Original per item `PRIMER_` keys are retained as well for
+            compatibility.
 
         Args:
             seq_args: Primer3 sequence/design args as per Primer3 docs
             global_args: Primer3 global args as per Primer3 docs
             misprime_lib: `Sequence name: sequence` dictionary for mispriming
                 checks.
             mishyb_lib: `Sequence name: sequence` dictionary for
@@ -1216,28 +1275,29 @@
             seq_args=seq_args,
             global_args=global_args,
             misprime_lib=misprime_lib,
             mishyb_lib=mishyb_lib,
         )
 
         retval = choose_primers(
-            self.global_settings_data,
-            self.sequence_args_data,
+            <p3_global_settings*> self.global_settings_data,
+            <seq_args_t*> self.sequence_args_data,
         )
+
         if retval == NULL:
             raise ValueError('Issue choosing primers')
         try:
             results_dict = pdh_design_output_to_dict(
-                self.global_settings_data,
-                self.sequence_args_data,
+                <p3_global_settings*> self.global_settings_data,
+                <seq_args_t*> self.sequence_args_data,
                 retval,
             )
         finally:
             destroy_secundary_structures(
-                self.global_settings_data,
+                <p3_global_settings*> self.global_settings_data,
                 retval,
             )
             destroy_p3retval(retval)
             retval = NULL
             destroy_dpal_thal_arg_holder()
         return results_dict
 
@@ -1247,15 +1307,15 @@
         (pa[0].inside_penalty == PR_DEFAULT_INSIDE_PENALTY) and
         (pa[0].outside_penalty == PR_DEFAULT_OUTSIDE_PENALTY)
     ):
         return 1
     return 0
 
 
-cdef int pdh_wrap_set_seq_args_globals(
+cdef inline int pdh_wrap_set_seq_args_globals(
         p3_global_settings* global_settings_data,
         seq_args_t* sequence_args_data,
         object kmer_lists_path,
         char* in_buffer,
 ) except -1:
     '''
     Creates a new p3_global_settings struct and initializes it with
@@ -1375,15 +1435,15 @@
         raise ValueError(err_msg_b.decode('utf8'))
     if fatal_parse_err.data != NULL:
         err_msg_b = <bytes> fatal_parse_err.data
         raise ValueError(err_msg_b.decode('utf8'))
     return 0
 
 
-cdef seq_lib* pdh_create_seq_lib(object seq_dict) except NULL:
+cdef inline seq_lib* pdh_create_seq_lib(object seq_dict) except NULL:
     '''
     Generates a library of sequences for mispriming checks.
     Input is a Python dictionary with <seq name: sequence> key value
     pairs. Returns NULL and sets the Python error string on failure.
 
     Args:
         seq_dict: Sequence disctionary in the format <seq name: sequence>
@@ -1436,15 +1496,15 @@
             destroy_seq_lib(sl)
             raise OSError(err_msg_b.decode('utf8'))
     reverse_complement_seq_lib(sl)
 
     return sl
 
 
-cdef object pdh_design_output_to_dict(
+cdef inline object pdh_design_output_to_dict(
         const p3_global_settings* global_settings_data,
         const seq_args_t* sequence_args_data,
         const p3retval *retval,
 ):
     '''
     Args:
         global_settings_data: primer3 p3_global_settings data pointer
@@ -1627,14 +1687,19 @@
     # Save the number of each type of oligo that was found
     output_dict['PRIMER_LEFT_NUM_RETURNED'] = print_fwd
     output_dict['PRIMER_RIGHT_NUM_RETURNED'] = print_rev
 
     output_dict[f'PRIMER_{int_oligo}_NUM_RETURNED'] = print_int
     output_dict['PRIMER_PAIR_NUM_RETURNED'] = num_pair
 
+    output_dict['PRIMER_PAIR'] = [None] * num_pair
+    output_dict['PRIMER_LEFT'] = [None] * print_fwd
+    output_dict['PRIMER_RIGHT'] = [None] * print_rev
+    output_dict[f'PRIMER_{int_oligo}'] = [None] * print_int
+
     # Start of the loop printing all pairs or primers or oligos
     for i in range(loop_max):
         # What needs to be printed the conditions for primer lists
         if retval[0].output_type == p3_output_type.primer_list:
             # Attach the selected primers to the pointers
             fwd = &(retval[0].fwd.oligo[i])
             rev = &(retval[0].rev.oligo[i])
@@ -1670,457 +1735,577 @@
             # Do hyb oligos have to be printed?
             if (global_settings_data[0].pick_internal_oligo == 1):
                 go_int = 1
             else:
                 go_int = 0
 
         # Print out the Pair Penalties
+        primer_pair_i = {}
+        primer_left_i = {}
+        primer_right_i = {}
+        primer_internal_i = {}
+
         if retval[0].output_type == p3_output_type.primer_pairs:
             temp_double = retval[0].best_pairs.pairs[i].pair_quality
             output_dict[f'PRIMER_PAIR_{i}_PENALTY'] = temp_double
-
+            primer_pair_i['PENALTY'] = temp_double
         # Print single primer penalty
         if go_fwd == 1:
             temp_double = fwd[0].quality
             output_dict[f'PRIMER_LEFT_{i}_PENALTY'] = temp_double
-
+            primer_left_i['PENALTY'] = temp_double
         if go_rev == 1:
             temp_double = rev[0].quality
             output_dict[f'PRIMER_RIGHT_{i}_PENALTY'] = temp_double
-
+            primer_right_i['PENALTY'] = temp_double
         if go_int == 1:
             temp_double = intl[0].quality
             output_dict[f'PRIMER_{int_oligo}_{i}_PENALTY'] = temp_double
+            primer_internal_i['PENALTY'] = temp_double
 
         # Print the oligo_problems
         if (go_fwd == 1) and p3_ol_has_any_problem(fwd):
             problem_b = <bytes> p3_get_ol_problem_string(fwd)
             output_dict[f'PRIMER_LEFT_{i}_PROBLEMS'] = problem_b
+            primer_left_i['PROBLEMS'] = problem_b
 
         if (go_rev == 1) and p3_ol_has_any_problem(rev):
             problem_b = <bytes> p3_get_ol_problem_string(rev)
             output_dict[f'PRIMER_RIGHT_{i}_PROBLEMS'] = problem_b
+            primer_right_i['PROBLEMS'] = problem_b
 
         if (go_int == 1) and p3_ol_has_any_problem(intl):
             problem_b = <bytes> p3_get_ol_problem_string(intl)
             output_dict[f'PRIMER_{int_oligo}_{i}_PROBLEMS'] = problem_b
-
+            primer_internal_i['PROBLEMS'] = problem_b
 
         # Print primer sequences.
         if go_fwd == 1:
             sqtemp_b = <bytes> pr_oligo_overhang_sequence(
                 sequence_args_data,
                 fwd,
             )
-            output_dict[f'PRIMER_LEFT_{i}_SEQUENCE'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_LEFT_{i}_SEQUENCE'] = sqtemp_str
+            primer_left_i['SEQUENCE'] = sqtemp_str
 
         if go_rev == 1:
             sqtemp_b = <bytes> pr_oligo_rev_c_overhang_sequence(
                 sequence_args_data,
                 rev,
             )
-            output_dict[f'PRIMER_RIGHT_{i}_SEQUENCE'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_RIGHT_{i}_SEQUENCE'] = sqtemp_str
+            primer_right_i['SEQUENCE'] = sqtemp_str
 
         if go_int == 1:
             sqtemp_b = <bytes> pr_oligo_sequence(sequence_args_data, intl)
-            output_dict[f'PRIMER_{int_oligo}_{i}_SEQUENCE'] = sqtemp_b.decode(
-                'utf8',
-            )
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_{int_oligo}_{i}_SEQUENCE'] = sqtemp_str
+            primer_internal_i['SEQUENCE'] = sqtemp_str
 
         # Print primer start and length
         if go_fwd == 1:
-            output_dict[f'PRIMER_LEFT_{i}'] = [
+            coord_list = [
                 fwd[0].start + incl_s + global_settings_data[0].first_base_index,
                 fwd[0].length,
             ]
+            output_dict[f'PRIMER_LEFT_{i}'] = coord_list
+            primer_left_i['COORDS'] = coord_list
+
         if go_rev == 1:
-            output_dict[f'PRIMER_RIGHT_{i}'] = [
+            coord_list = [
                 rev[0].start + incl_s + global_settings_data[0].first_base_index,
                 rev[0].length,
             ]
+            output_dict[f'PRIMER_RIGHT_{i}'] = coord_list
+            primer_right_i['COORDS'] = coord_list
+
         if go_int == 1:
-            output_dict[f'PRIMER_{int_oligo}_{i}'] = [
+            coord_list = [
                 (
                     intl[0].start +
                     incl_s +
                     global_settings_data[0].first_base_index
                 ),
                 intl[0].length,
             ]
+            output_dict[f'PRIMER_{int_oligo}_{i}'] = coord_list
+            primer_internal_i['COORDS'] = coord_list
 
         # Print primer Tm
         if go_fwd == 1:
             output_dict[f'PRIMER_LEFT_{i}_TM'] = fwd[0].temp
+            primer_left_i['TM'] = fwd[0].temp
         if go_rev == 1:
             output_dict[f'PRIMER_RIGHT_{i}_TM'] = rev[0].temp
+            primer_right_i['TM'] = rev[0].temp
         if go_int == 1:
             output_dict[f'PRIMER_{int_oligo}_{i}_TM'] = intl[0].temp
+            primer_internal_i['TM'] = intl[0].temp
 
         # Print fraction bound at melting temperature
         if (
             (global_settings_data[0].annealing_temp > 0.0) and
             (global_settings_data[0].salt_corrections != 2)
         ):
             if (go_fwd == 1) and (fwd[0].bound > 0.0):
                 output_dict[f'PRIMER_LEFT_{i}_BOUND'] = fwd[0].bound
+                primer_left_i['BOUND'] = fwd[0].bound
             if (go_rev == 1) and (rev[0].bound > 0.0):
                 output_dict[f'PRIMER_RIGHT_{i}_BOUND'] = rev[0].bound
+                primer_right_i['BOUND'] = rev[0].bound
             if (go_int == 1) and (intl[0].bound > 0.0):
                 output_dict[f'PRIMER_{int_oligo}_{i}_BOUND'] = intl[0].bound
+                primer_internal_i['BOUND'] = intl[0].bound
 
         # Print primer GC content
         if go_fwd == 1:
             output_dict[f'PRIMER_LEFT_{i}_GC_PERCENT'] = fwd[0].gc_content
+            primer_left_i['GC_PERCENT'] = fwd[0].gc_content
         if go_rev == 1:
             output_dict[f'PRIMER_RIGHT_{i}_GC_PERCENT'] = rev[0].gc_content
-
+            primer_right_i['GC_PERCENT'] = rev[0].gc_content
         if go_int == 1:
             output_dict[f'PRIMER_{int_oligo}_{i}_GC_PERCENT'] = intl[0].gc_content
-
+            primer_internal_i['GC_PERCENT'] = intl[0].gc_content
         # Print primer self_any
         if (
             (go_fwd == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 0)
         ):
             output_dict[f'PRIMER_LEFT_{i}_SELF_ANY'] = fwd[0].self_any
+            primer_left_i['SELF_ANY'] = fwd[0].self_any
         if (
             (go_rev == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 0)
         ):
             output_dict[f'PRIMER_RIGHT_{i}_SELF_ANY'] = rev[0].self_any
+            primer_right_i['SELF_ANY'] = rev[0].self_any
         if (
             (go_int == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 0)
         ):
             output_dict[f'PRIMER_{int_oligo}_{i}_SELF_ANY'] = intl[0].self_any
+            primer_internal_i['SELF_ANY'] = intl[0].self_any
 
         # Print primer self_any thermodynamical approach
         if (
             (go_fwd == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_LEFT_{i}_SELF_ANY_TH'] = fwd[0].self_any
+            primer_left_i['SELF_ANY_TH'] = fwd[0].self_any
         if (
             (go_rev == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_RIGHT_{i}_SELF_ANY_TH'] = rev[0].self_any
+            primer_right_i['SELF_ANY_TH'] = rev[0].self_any
         if (
             (go_int == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_{int_oligo}_{i}_SELF_ANY_TH'] = intl[0].self_any
+            primer_internal_i['SELF_ANY_TH'] = intl[0].self_any
 
         # Print primer secondary structures*/
         if (
             (go_fwd == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (fwd[0].self_any_struct != NULL)
         ):
             sqtemp_b = <bytes> fwd[0].self_any_struct
-            output_dict[f'PRIMER_LEFT_{i}_SELF_ANY_STUCT'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_LEFT_{i}_SELF_ANY_STUCT'] = sqtemp_str
+            primer_left_i['SELF_ANY_STUCT'] = sqtemp_str
         if (
             (go_rev == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (rev[0].self_any_struct != NULL)
         ):
             sqtemp_b = <bytes> rev[0].self_any_struct
-            output_dict[f'PRIMER_RIGHT_{i}_SELF_ANY_STUCT'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_RIGHT_{i}_SELF_ANY_STUCT'] = sqtemp_str
+            primer_right_i['SELF_ANY_STUCT'] = sqtemp_str
         if (
             (go_int == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (intl[0].self_any_struct != NULL)
         ):
             sqtemp_b = <bytes> intl[0].self_any_struct
-            output_dict[f'PRIMER_{int_oligo}_{i}_SELF_ANY_STUCT'] = sqtemp_b.decode('utf8')
-
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_{int_oligo}_{i}_SELF_ANY_STUCT'] = sqtemp_str
+            primer_internal_i['SELF_ANY_STUCT'] = sqtemp_str
 
         # Print primer self_end
         if (go_fwd == 1) and (global_settings_data[0].thermodynamic_oligo_alignment == 0):
             output_dict[f'PRIMER_LEFT_{i}_SELF_END'] = fwd[0].self_end
 
         if (go_rev == 1) and (global_settings_data[0].thermodynamic_oligo_alignment == 0):
             output_dict[f'PRIMER_RIGHT_{i}_SELF_END'] = rev[0].self_end
 
         if (go_int == 1) and (global_settings_data[0].thermodynamic_oligo_alignment == 0):
             output_dict[f'PRIMER_{int_oligo}_{i}_SELF_END'] = intl[0].self_end
 
         # Print primer self_end thermodynamical approach
         if (go_fwd == 1) and (global_settings_data[0].thermodynamic_oligo_alignment == 1):
             output_dict[f'PRIMER_LEFT_{i}_SELF_END_TH'] = fwd[0].self_end
+            primer_left_i['SELF_END_TH'] = fwd[0].self_end
         if (go_rev == 1) and (global_settings_data[0].thermodynamic_oligo_alignment == 1):
             output_dict[f'PRIMER_RIGHT_{i}_SELF_END_TH'] = rev[0].self_end
+            primer_right_i['SELF_END_TH'] = rev[0].self_end
         if (go_int == 1) and ((global_settings_data[0].thermodynamic_oligo_alignment == 1)):
             output_dict[f'PRIMER_{int_oligo}_{i}_SELF_END_TH'] = intl[0].self_end
+            primer_internal_i['SELF_END_TH'] = intl[0].self_end
 
         # Print primer secondary structures*/
         if (
             (go_fwd == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (fwd[0].self_end_struct != NULL)
         ):
             sqtemp_b = <bytes> fwd[0].self_end_struct
-            output_dict[f'PRIMER_LEFT_{i}_SELF_END_STUCT'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_LEFT_{i}_SELF_END_STUCT'] = sqtemp_str
+            primer_left_i['SELF_END_STUCT'] = sqtemp_str
         if (
             (go_rev == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (rev[0].self_end_struct != NULL)
         ):
             sqtemp_b = <bytes> rev[0].self_end_struct
-            output_dict[f'PRIMER_RIGHT_{i}_SELF_END_STUCT'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_RIGHT_{i}_SELF_END_STUCT'] = sqtemp_str
+            primer_right_i['SELF_END_STUCT'] = sqtemp_str
         if (
             (go_int == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (intl[0].self_end_struct != NULL)
         ):
             sqtemp_b = <bytes> intl[0].self_end_struct
-            output_dict[f'PRIMER_{int_oligo}_{i}_SELF_END_STUCT'] = sqtemp_b.decode('utf8')
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_{int_oligo}_{i}_SELF_END_STUCT'] = sqtemp_str
+            primer_internal_i['SELF_END_STUCT'] = sqtemp_str
 
         # Print primer hairpin
         if (
             (go_fwd == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_LEFT_{i}_HAIRPIN_TH'] = fwd[0].hairpin_th
+            primer_left_i['HAIRPIN_TH'] = fwd[0].hairpin_th
         if (
             (go_rev == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_RIGHT_{i}_HAIRPIN_TH'] = rev[0].hairpin_th
+            primer_right_i['HAIRPIN_TH'] = rev[0].hairpin_th
         if (
             (go_int == 1) and
             (global_settings_data[0].thermodynamic_oligo_alignment == 1)
         ):
             output_dict[f'PRIMER_{int_oligo}_{i}_HAIRPIN_TH'] = intl[0].hairpin_th
-
+            primer_internal_i['HAIRPIN_TH'] = intl[0].hairpin_th
         # Print primer secondary structures*/
         if (
             (go_fwd == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (fwd[0].hairpin_struct != NULL)
         ):
             sqtemp_b = <bytes> fwd[0].hairpin_struct
-            output_dict[f'PRIMER_LEFT_{i}_HAIRPIN_STUCT'] = sqtemp_b.decode('utf8')
-
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_LEFT_{i}_HAIRPIN_STUCT'] = sqtemp_str
+            primer_left_i['HAIRPIN_STUCT'] = fwd[0].hairpin_th
         if (
             (go_rev == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (rev[0].hairpin_struct != NULL)
         ):
             sqtemp_b = <bytes> rev[0].hairpin_struct
-            output_dict[f'PRIMER_RIGHT_{i}_HAIRPIN_STUCT'] = sqtemp_b.decode('utf8')
-
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_RIGHT_{i}_HAIRPIN_STUCT'] = sqtemp_str
+            primer_right_i['HAIRPIN_STUCT'] = rev[0].hairpin_th
         if (
             (go_int == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (intl[0].hairpin_struct != NULL)
         ):
             sqtemp_b = <bytes> intl[0].hairpin_struct
-            output_dict[f'PRIMER_{int_oligo}_{i}_HAIRPIN_STUCT'] = sqtemp_b.decode('utf8')
-
+            sqtemp_str = sqtemp_b.decode('utf8')
+            output_dict[f'PRIMER_{int_oligo}_{i}_HAIRPIN_STUCT'] = sqtemp_str
+            primer_internal_i['HAIRPIN_STUCT'] = intl[0].hairpin_th
         # Print out primer mispriming scores
         if seq_lib_num_seq(global_settings_data[0].p_args.repeat_lib) > 0:
             if go_fwd == 1:
                 sqtemp_b = <bytes> fwd[0].repeat_sim.name
                 output_dict[f'PRIMER_LEFT_{i}_LIBRARY_MISPRIMING'] = (
                     fwd[0].repeat_sim.score[fwd[0].repeat_sim.max],
                     sqtemp_b.decode('utf8'),
                 )
-
+                primer_left_i['LIBRARY_MISPRIMING'] = (
+                    fwd[0].repeat_sim.score[fwd[0].repeat_sim.max],
+                    sqtemp_b.decode('utf8'),
+                )
             if go_rev == 1:
                 sqtemp_b = <bytes> rev[0].repeat_sim.name
                 output_dict[f'PRIMER_RIGHT_{i}_LIBRARY_MISPRIMING'] = (
                     rev[0].repeat_sim.score[rev[0].repeat_sim.max],
                     sqtemp_b.decode('utf8'),
                 )
+                primer_right_i['LIBRARY_MISPRIMING'] = (
+                    rev[0].repeat_sim.score[rev[0].repeat_sim.max],
+                    sqtemp_b.decode('utf8'),
+                )
 
             if retval[0].output_type == p3_output_type.primer_pairs:
                 sqtemp_b = <bytes> retval[0].best_pairs.pairs[i].rep_name
                 output_dict[f'PRIMER_PAIR_{i}_LIBRARY_MISPRIMING'] = (
                     retval[0].best_pairs.pairs[i].repeat_sim,
                     sqtemp_b.decode('utf8'),
                 )
-
+                primer_pair_i['LIBRARY_MISPRIMING'] = (
+                    retval[0].best_pairs.pairs[i].repeat_sim,
+                    sqtemp_b.decode('utf8'),
+                )
         # Print out internal oligo mispriming scores
         if (
             (go_int == 1) and
             (seq_lib_num_seq(global_settings_data[0].o_args.repeat_lib) > 0)
         ):
             sqtemp_b = <bytes> intl[0].repeat_sim.name
             output_dict[f'PRIMER_{int_oligo}_{i}_LIBRARY_MISPRIMING'] = (
                 intl[0].repeat_sim.score[intl[0].repeat_sim.max],
                 sqtemp_b.decode('utf8'),
             )
+            primer_internal_i['LIBRARY_MISPRIMING'] = (
+                intl[0].repeat_sim.score[intl[0].repeat_sim.max],
+                sqtemp_b.decode('utf8'),
+            )
 
 
         # If a sequence quality was provided, print it*/
         if sequence_args_data[0].quality != NULL:
             if go_fwd == 1:
                 output_dict[f'PRIMER_LEFT_{i}_MIN_SEQ_QUALITY'] = fwd[0].seq_quality
+                primer_left_i['MIN_SEQ_QUALITY'] = fwd[0].seq_quality
             if go_rev == 1:
                 output_dict[f'PRIMER_RIGHT_{i}_MIN_SEQ_QUALITY'] = rev[0].seq_quality
+                primer_right_i['MIN_SEQ_QUALITY'] = rev[0].seq_quality
             if go_int == 1:
                 output_dict[f'PRIMER_{int_oligo}_{i}_MIN_SEQ_QUALITY'] = intl[0].seq_quality
+                primer_internal_i['MIN_SEQ_QUALITY'] = intl[0].seq_quality
 
         # Print position penalty, this is for backward compatibility
         if (
             not pr_default_position_penalties(global_settings_data) or
             not PR_START_CODON_POS_IS_NULL(sequence_args_data)
         ):
             if go_fwd == 1:
                 output_dict[f'PRIMER_LEFT_{i}_POSITION_PENALTY'] = fwd[0].position_penalty
+                primer_left_i['POSITION_PENALTY'] = fwd[0].position_penalty
             if go_rev == 1:
                 output_dict[f'PRIMER_RIGHT_{i}_POSITION_PENALTY'] = rev[0].position_penalty
+                primer_right_i['POSITION_PENALTY'] = rev[0].position_penalty
 
         # Print primer end stability
         if go_fwd == 1:
             output_dict[f'PRIMER_LEFT_{i}_END_STABILITY'] = fwd[0].end_stability
-
+            primer_left_i['END_STABILITY'] = fwd[0].end_stability
         if go_rev == 1:
             output_dict[f'PRIMER_RIGHT_{i}_END_STABILITY'] = rev[0].end_stability
-
+            primer_right_i['END_STABILITY'] = rev[0].end_stability
 
         # Print primer template mispriming
         if (
             (global_settings_data[0].thermodynamic_template_alignment == 0) and
             (go_fwd == 1) and
             (oligo_max_template_mispriming(fwd) != ALIGN_SCORE_UNDEF)
         ):
             output_dict[f'PRIMER_LEFT_{i}_TEMPLATE_MISPRIMING'] = \
                 oligo_max_template_mispriming(fwd)
+            primer_left_i['TEMPLATE_MISPRIMING'] = \
+                oligo_max_template_mispriming(fwd)
         if (
             (global_settings_data[0].thermodynamic_template_alignment == 0) and
             (go_rev == 1) and
             (oligo_max_template_mispriming(rev) != ALIGN_SCORE_UNDEF)
         ):
             output_dict[f'PRIMER_RIGHT_{i}_TEMPLATE_MISPRIMING'] = \
                 oligo_max_template_mispriming(rev)
-
+            primer_right_i['TEMPLATE_MISPRIMING'] = \
+                oligo_max_template_mispriming(rev)
 
         # Print primer template mispriming, thermodynamical approach*/
         if (
             (global_settings_data[0].thermodynamic_template_alignment == 0) and
             (go_fwd == 1) and
             (oligo_max_template_mispriming(fwd) != ALIGN_SCORE_UNDEF)
         ):
             output_dict[f'PRIMER_LEFT_{i}_TEMPLATE_MISPRIMING_TH'] = \
                 oligo_max_template_mispriming_thermod(fwd)
+            primer_left_i['TEMPLATE_MISPRIMING_TH'] = \
+                oligo_max_template_mispriming_thermod(fwd)
 
         if (
             (global_settings_data[0].thermodynamic_template_alignment == 0) and
             (go_rev == 1) and
             (oligo_max_template_mispriming(rev) != ALIGN_SCORE_UNDEF)
         ):
             output_dict[f'PRIMER_RIGHT_{i}_TEMPLATE_MISPRIMING_TH'] = \
                 oligo_max_template_mispriming_thermod(rev)
+            primer_right_i['TEMPLATE_MISPRIMING_TH'] = \
+                oligo_max_template_mispriming_thermod(rev)
 
         # Print primer secondary structures*/
         if (
             (go_fwd == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (oligo_max_template_mispriming_struct(fwd) != NULL)
         ):
             sqtemp_b = <bytes> oligo_max_template_mispriming_struct(fwd)
             output_dict[f'PRIMER_LEFT_{i}_TEMPLATE_MISPRIMING_STUCT'] = sqtemp_b.decode('utf8')
+            primer_left_i['TEMPLATE_MISPRIMING_STUCT'] = sqtemp_b.decode('utf8')
+
         if (
             (go_rev == 1) and
             (global_settings_data[0].show_secondary_structure_alignment == 1) and
             (oligo_max_template_mispriming_struct(rev) != NULL)
         ):
             sqtemp_b = <bytes> oligo_max_template_mispriming_struct(rev)
             output_dict[f'PRIMER_RIGHT_{i}_TEMPLATE_MISPRIMING_STUCT'] = sqtemp_b.decode('utf8')
+            primer_right_i['TEMPLATE_MISPRIMING_STUCT'] = sqtemp_b.decode('utf8')
 
         # Print the pair parameters*/
         if retval[0].output_type == p3_output_type.primer_pairs:
             if (go_int == 1) and (sequence_args_data[0].quality != NULL):
                 output_dict[f'PRIMER_{int_oligo}_{i}_MIN_SEQ_QUALITY'] = intl[0].seq_quality
+                primer_internal_i['MIN_SEQ_QUALITY'] = intl[0].seq_quality
+
             # Print pair comp_any
             if global_settings_data[0].thermodynamic_oligo_alignment == 0:
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_ANY'] = \
                     retval[0].best_pairs.pairs[i].compl_any
+                primer_pair_i['COMPL_ANY'] = \
+                    retval[0].best_pairs.pairs[i].compl_any
 
             if global_settings_data[0].thermodynamic_oligo_alignment == 1:
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_ANY_TH'] = \
                     retval[0].best_pairs.pairs[i].compl_any
+                primer_pair_i['COMPL_ANY_TH'] = \
+                    retval[0].best_pairs.pairs[i].compl_any
 
             # Print primer secondary structures */
             if (
                 (global_settings_data[0].show_secondary_structure_alignment == 1) and
                 (retval[0].best_pairs.pairs[i].compl_any_struct != NULL)
             ):
                 sqtemp_b = <bytes> retval[0].best_pairs.pairs[i].compl_any_struct
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_ANY_STUCT'] = sqtemp_b.decode('utf8')
+                primer_pair_i['COMPL_ANY_STUCT'] = sqtemp_b.decode('utf8')
 
             # Print pair comp_end
             if global_settings_data[0].thermodynamic_oligo_alignment == 0:
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_END'] = \
                     retval[0].best_pairs.pairs[i].compl_end
+                primer_pair_i['COMPL_END'] = \
+                    retval[0].best_pairs.pairs[i].compl_end
 
             if global_settings_data[0].thermodynamic_oligo_alignment == 1:
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_END_TH'] = \
                     retval[0].best_pairs.pairs[i].compl_end
+                primer_pair_i['COMPL_END_TH'] = \
+                    retval[0].best_pairs.pairs[i].compl_end
 
             # Print primer secondary structures*/
             if (
                 (global_settings_data[0].show_secondary_structure_alignment == 1) and
                 (retval[0].best_pairs.pairs[i].compl_end_struct != NULL)
             ):
                 sqtemp_b = <bytes> retval[0].best_pairs.pairs[i].compl_end_struct
                 output_dict[f'PRIMER_PAIR_{i}_COMPL_END_STUCT'] = sqtemp_b.decode('utf8')
+                primer_pair_i['COMPL_END_STUCT'] = sqtemp_b.decode('utf8')
 
             # Print product size
             product_size = retval[0].best_pairs.pairs[i].product_size
             if sequence_args_data[0].overhang_left != NULL:
                 product_size += strlen(sequence_args_data[0].overhang_left)
             if sequence_args_data[0].overhang_right != NULL:
                 product_size += strlen(sequence_args_data[0].overhang_right)
             output_dict[f'PRIMER_PAIR_{i}_PRODUCT_SIZE'] = product_size
-
+            primer_pair_i['PRODUCT_SIZE'] = product_size
 
             # Print the product Tm if a Tm range is defined
             if (
                 (global_settings_data[0].product_max_tm != PR_DEFAULT_PRODUCT_MAX_TM) or
                 (global_settings_data[0].product_min_tm != PR_DEFAULT_PRODUCT_MIN_TM)
             ):
                 output_dict[f'PRIMER_PAIR_{i}_PRODUCT_TM'] = \
                     retval[0].best_pairs.pairs[i].product_tm
+                primer_pair_i['PRODUCT_TM'] = \
+                    retval[0].best_pairs.pairs[i].product_tm
+
                 output_dict[f'PRIMER_PAIR_{i}_PRODUCT_TM_OLIGO_TM_DIFF'] = \
                     retval[0].best_pairs.pairs[i].product_tm_oligo_tm_diff
+                primer_pair_i['PRODUCT_TM_OLIGO_TM_DIFF'] = \
+                    retval[0].best_pairs.pairs[i].product_tm_oligo_tm_diff
+
                 output_dict[f'PRIMER_PAIR_{i}_T_OPT_A'] = retval[0].best_pairs.pairs[i].t_opt_a
+                primer_pair_i['T_OPT_A'] = retval[0].best_pairs.pairs[i].t_opt_a
             else:
                 output_dict[f'PRIMER_PAIR_{i}_PRODUCT_TM'] = \
                 retval[0].best_pairs.pairs[i].product_tm
+                primer_pair_i['PRODUCT_TM'] = \
+                    retval[0].best_pairs.pairs[i].product_tm
 
             # Print the primer pair template mispriming
             if (
                 (global_settings_data[0].thermodynamic_template_alignment == 0) and
                 (retval[0].best_pairs.pairs[i].template_mispriming != ALIGN_SCORE_UNDEF)
             ):
                 output_dict[f'PRIMER_PAIR_{i}_TEMPLATE_MISPRIMING'] = \
                     retval[0].best_pairs.pairs[i].template_mispriming
+                primer_pair_i['TEMPLATE_MISPRIMING'] = \
+                    retval[0].best_pairs.pairs[i].template_mispriming
+
             # Print the primer pair template mispriming. Thermodynamic approach.
             if (
                     (global_settings_data[0].thermodynamic_template_alignment == 1) and
                     (retval[0].best_pairs.pairs[i].template_mispriming != ALIGN_SCORE_UNDEF)
             ):
                 output_dict[f'PRIMER_PAIR_{i}_TEMPLATE_MISPRIMING_TH'] = \
                     retval[0].best_pairs.pairs[i].template_mispriming
+                primer_pair_i['TEMPLATE_MISPRIMING_TH'] = \
+                    retval[0].best_pairs.pairs[i].template_mispriming
 
             # Print primer secondary structures*/
             if (
                  (global_settings_data[0].show_secondary_structure_alignment == 1) and
                 (retval[0].best_pairs.pairs[i].template_mispriming_struct != NULL)
             ):
                 sqtemp_b = <bytes> retval[0].best_pairs.pairs[i].template_mispriming_struct
                 output_dict[f'PRIMER_PAIR_{i}_TEMPLATE_MISPRIMING_STUCT'] = \
                     sqtemp_b.decode('utf8')
+                primer_pair_i['TEMPLATE_MISPRIMING_STUCT'] = \
+                    sqtemp_b.decode('utf8')
         # End of print parameters of primer pairs
+
+        # Conditionally assign elements to output_dict
+        if primer_pair_i:
+            output_dict['PRIMER_PAIR'][i] = primer_pair_i
+        if primer_left_i:
+            output_dict['PRIMER_LEFT'][i] = primer_left_i
+        if primer_right_i:
+            output_dict['PRIMER_RIGHT'][i] = primer_right_i
+        if primer_internal_i:
+            output_dict['PRIMER_INTERNAL'][i] = primer_internal_i
     # End of the for big loop printing all data
     return output_dict
 
+
 class Singleton(type):
     _instances = {}  # type: ignore
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(
                 *args,
```

### Comparing `primer3-py-1.2.2/primer3_py.egg-info/PKG-INFO` & `primer3-py-2.0.0/primer3_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primer3-py
-Version: 1.2.2
+Version: 2.0.0
 Summary: Python bindings for Primer3
 Home-page: https://github.com/libnano/primer3-py
 Author: Ben Pruitt, Nick Conway
 Author-email: bpruittvt@gmail.com
 License: GPLv2
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: primer3-py Version: 1.2.2 Summary: Python bindings
+Metadata-Version: 2.1 Name: primer3-py Version: 2.0.0 Summary: Python bindings
 for Primer3 Home-page: https://github.com/libnano/primer3-py Author: Ben
 Pruitt, Nick Conway Author-email: bpruittvt@gmail.com License: GPLv2
 Classifier: Programming Language :: C Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 4 - Beta
```

### Comparing `primer3-py-1.2.2/primer3_py.egg-info/SOURCES.txt` & `primer3-py-2.0.0/primer3_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 examples/orthogonalprimers.py
 primer3/__init__.py
 primer3/argdefaults.py
 primer3/bindings.py
 primer3/p3helpers.h
 primer3/p3helpers.pyx
 primer3/thermoanalysis.pxd
+primer3/thermoanalysis.pxi
 primer3/thermoanalysis.pyx
 primer3/src/libprimer3/ABOUT.txt
 primer3/src/libprimer3/LICENSE.txt
 primer3/src/libprimer3/Makefile
 primer3/src/libprimer3/amplicontm.c
 primer3/src/libprimer3/amplicontm.h
 primer3/src/libprimer3/amplicontm_main.c
```

### Comparing `primer3-py-1.2.2/setup.py` & `primer3-py-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     LIBPRIMER3_THERMO_PARAMS_FPS +
     LIBPRIMER3_TEST_FPS +
     LIBPRIMER3_C_FPS_FLEX +
     LIBPRIMER3_C_EXTRA_FPS +
     LIBPRIMER3_H_FPS +
     KLIB_H_FPS +
     ['p3helpers.pyx', 'p3helpers.h'] +
-    ['thermoanalysis.pxd', 'thermoanalysis.pyx']
+    ['thermoanalysis.pxd', 'thermoanalysis.pxi', 'thermoanalysis.pyx']
 )
 
 # ~~~~~~~~~~~~~~~~~~~~~ Primer3 C library build helpers ~~~~~~~~~~~~~~~~~~~~~ #
 
 
 def p3Clean():
     '''
```

### Comparing `primer3-py-1.2.2/tests/_simulatedbindings.py` & `primer3-py-2.0.0/tests/_simulatedbindings.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/checkdatasets.py` & `primer3-py-2.0.0/tests/checkdatasets.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/long_seq_input` & `primer3-py-2.0.0/tests/input_files/long_seq_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/p3-tmpl-mispriming_input` & `primer3-py-2.0.0/tests/input_files/p3-tmpl-mispriming_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/p3_3_prime_0_input` & `primer3-py-2.0.0/tests/input_files/p3_3_prime_0_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/p3_3_prime_n_input` & `primer3-py-2.0.0/tests/input_files/p3_3_prime_n_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer1_input` & `primer3-py-2.0.0/tests/input_files/primer1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer1_th_input` & `primer3-py-2.0.0/tests/input_files/primer1_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer3_v1_1_4_default_settings_input` & `primer3-py-2.0.0/tests/input_files/primer3_v1_1_4_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer3web_v0_4_0_default_settings_input` & `primer3-py-2.0.0/tests/input_files/primer3web_v0_4_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer3web_v3_0_0_default_settings_input` & `primer3-py-2.0.0/tests/input_files/primer3web_v3_0_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer3web_v4_0_0_default_settings_input` & `primer3-py-2.0.0/tests/input_files/primer3web_v4_0_0_default_settings_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_all_settingsfiles_input` & `primer3-py-2.0.0/tests/input_files/primer_all_settingsfiles_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_annealing_temp_input` & `primer3-py-2.0.0/tests/input_files/primer_annealing_temp_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_boundary1_input` & `primer3-py-2.0.0/tests/input_files/primer_boundary1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_boundary_input` & `primer3-py-2.0.0/tests/input_files/primer_boundary_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_check_input` & `primer3-py-2.0.0/tests/input_files/primer_check_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_dmso_formamide_input` & `primer3-py-2.0.0/tests/input_files/primer_dmso_formamide_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_end_pathology_input` & `primer3-py-2.0.0/tests/input_files/primer_end_pathology_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_first_base_index_input` & `primer3-py-2.0.0/tests/input_files/primer_first_base_index_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_gc_end_input` & `primer3-py-2.0.0/tests/input_files/primer_gc_end_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_high_gc_load_set_input` & `primer3-py-2.0.0/tests/input_files/primer_high_gc_load_set_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_high_tm_load_set_input` & `primer3-py-2.0.0/tests/input_files/primer_high_tm_load_set_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_human_input` & `primer3-py-2.0.0/tests/input_files/primer_human_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_input` & `primer3-py-2.0.0/tests/input_files/primer_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_internal1_input` & `primer3-py-2.0.0/tests/input_files/primer_internal1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_internal_input` & `primer3-py-2.0.0/tests/input_files/primer_internal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_internal_position_input` & `primer3-py-2.0.0/tests/input_files/primer_internal_position_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_lib_amb_codes_input` & `primer3-py-2.0.0/tests/input_files/primer_lib_amb_codes_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_masker_input` & `primer3-py-2.0.0/tests/input_files/primer_masker_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_mispriming_boundary1_input` & `primer3-py-2.0.0/tests/input_files/primer_mispriming_boundary1_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_mispriming_boundary2_input` & `primer3-py-2.0.0/tests/input_files/primer_mispriming_boundary2_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_mispriming_input` & `primer3-py-2.0.0/tests/input_files/primer_mispriming_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_mispriming_long_lib_input` & `primer3-py-2.0.0/tests/input_files/primer_mispriming_long_lib_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_mispriming_th_input` & `primer3-py-2.0.0/tests/input_files/primer_mispriming_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_must_match_input` & `primer3-py-2.0.0/tests/input_files/primer_must_match_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_must_overlap_point_input` & `primer3-py-2.0.0/tests/input_files/primer_must_overlap_point_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_must_use_input` & `primer3-py-2.0.0/tests/input_files/primer_must_use_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_must_use_op_input` & `primer3-py-2.0.0/tests/input_files/primer_must_use_op_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_must_use_th_input` & `primer3-py-2.0.0/tests/input_files/primer_must_use_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_new_tasks_input` & `primer3-py-2.0.0/tests/input_files/primer_new_tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_new_tasks_th_input` & `primer3-py-2.0.0/tests/input_files/primer_new_tasks_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_num_best_input` & `primer3-py-2.0.0/tests/input_files/primer_num_best_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_obj_fn_input` & `primer3-py-2.0.0/tests/input_files/primer_obj_fn_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_ok_regions2_input` & `primer3-py-2.0.0/tests/input_files/primer_ok_regions2_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_ok_regions_input` & `primer3-py-2.0.0/tests/input_files/primer_ok_regions_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_overhang_input` & `primer3-py-2.0.0/tests/input_files/primer_overhang_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_overhang_th_input` & `primer3-py-2.0.0/tests/input_files/primer_overhang_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_overlap_junction_input` & `primer3-py-2.0.0/tests/input_files/primer_overlap_junction_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_poly_x_input` & `primer3-py-2.0.0/tests/input_files/primer_poly_x_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_position_penalty_input` & `primer3-py-2.0.0/tests/input_files/primer_position_penalty_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_quality_boundary_input` & `primer3-py-2.0.0/tests/input_files/primer_quality_boundary_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_rat_input` & `primer3-py-2.0.0/tests/input_files/primer_rat_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_renewed_tasks_input` & `primer3-py-2.0.0/tests/input_files/primer_renewed_tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_sec_struct_dpal_input` & `primer3-py-2.0.0/tests/input_files/primer_sec_struct_dpal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_sec_struct_thal_input` & `primer3-py-2.0.0/tests/input_files/primer_sec_struct_thal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_start_codon_input` & `primer3-py-2.0.0/tests/input_files/primer_start_codon_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_syntax_input` & `primer3-py-2.0.0/tests/input_files/primer_syntax_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_task_input` & `primer3-py-2.0.0/tests/input_files/primer_task_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_task_th_input` & `primer3-py-2.0.0/tests/input_files/primer_task_th_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_thal_args_input` & `primer3-py-2.0.0/tests/input_files/primer_thal_args_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_thal_max_seq_error_input` & `primer3-py-2.0.0/tests/input_files/primer_thal_max_seq_error_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_thermod_align_input` & `primer3-py-2.0.0/tests/input_files/primer_thermod_align_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_three_prime_distance_input` & `primer3-py-2.0.0/tests/input_files/primer_three_prime_distance_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_tm_lc_masking_input` & `primer3-py-2.0.0/tests/input_files/primer_tm_lc_masking_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/primer_windows_newlines_input` & `primer3-py-2.0.0/tests/input_files/primer_windows_newlines_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/test_left_to_right_of_right_input` & `primer3-py-2.0.0/tests/input_files/test_left_to_right_of_right_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/th-w-other-tasks_input` & `primer3-py-2.0.0/tests/input_files/th-w-other-tasks_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/thal_input` & `primer3-py-2.0.0/tests/input_files/thal_input`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/input_files/thal_output` & `primer3-py-2.0.0/tests/input_files/thal_output`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/test_argdefaults.py` & `primer3-py-2.0.0/tests/test_argdefaults.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/test_ntthal_io.py` & `primer3-py-2.0.0/tests/test_ntthal_io.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/test_p3helpers.py` & `primer3-py-2.0.0/tests/test_p3helpers.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/test_primerdesign.py` & `primer3-py-2.0.0/tests/test_primerdesign.py`

 * *Files 11% similar despite different names*

```diff
@@ -513,27 +513,101 @@
             global_args=global_args,
             mishyb_lib={
                 'SEQ1': 'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA',
             },
         )
         self.assertEqual(result['PRIMER_PAIR_NUM_RETURNED'], 5)
         self.assertEqual(result['PRIMER_LEFT_0'], [46, 21])
+        self.assertEqual(result['PRIMER_LEFT'][0]['COORDS'], [46, 21])
 
         bindings.design_primers(
             seq_args=seq_args,
             global_args=global_args,
             misprime_lib={
                 'SEQ1': 'CACCATGGAGCTCCTGATATTAAAGGCGAATGCCATT',
             },
             mishyb_lib={
                 'SEQ1': 'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA',
             },
         )
+
+        self.assertAlmostEqual(
+            result['PRIMER_PAIR_0_PENALTY'],
+            1.37323,
+            places=4,
+        )
+        self.assertAlmostEqual(
+            result['PRIMER_PAIR'][0]['PENALTY'],
+            1.37323,
+            places=4,
+        )
+        self.assertEqual(len(result['PRIMER_PAIR']), 5)
+
         self.assertEqual(result['PRIMER_PAIR_NUM_RETURNED'], 5)
         self.assertEqual(result['PRIMER_LEFT_0'], [46, 21])
+        self.assertEqual(result['PRIMER_LEFT'][0]['COORDS'], [46, 21])
+        self.assertEqual(len(result['PRIMER_LEFT']), 5)
+
+        self.assertEqual(result['PRIMER_RIGHT_0'], [132, 20])
+        self.assertEqual(result['PRIMER_RIGHT'][0]['COORDS'], [132, 20])
+        self.assertEqual(len(result['PRIMER_RIGHT']), 5)
+
+        self.assertEqual(result['PRIMER_INTERNAL_0'], [69, 24])
+        self.assertEqual(result['PRIMER_INTERNAL'][0]['COORDS'], [69, 24])
+        self.assertEqual(len(result['PRIMER_INTERNAL']), 5)
+
+    def test_PRIMER_SECONDARY_STRUCTURE_ALIGNMENT(self):
+        '''Ensure all result pointers are initialized to NULL.
+        '''
+        seq_args = {
+            'SEQUENCE_ID': 'MH1000',
+            'SEQUENCE_TEMPLATE': (
+                'GCTTGCATGCCTGCAGGTCGACTCTAGAGGATCCCCCTACATTTT'
+                'AGCATCAGTGAGTACAGCATGCTTACTGGAAGAGAGGGTCATGCA'
+                'ACAGATTAGGAGGTAAGTTTGCAAAGGCAGGCTAAGGAGGAGACG'
+                'CACTGAATGCCATGGTAAGAACTCTGGACATAAAAATATTGGAAG'
+                'TTGTTGAGCAAGTNAAAAAAATGTTTGGAAGTGTTACTTTAGCAA'
+                'TGGCAAGAATGATAGTATGGAATAGATTGGCAGAATGAAGGCAAA'
+                'ATGATTAGACATATTGCATTAAGGTAAAAAATGATAACTGAAGAA'
+                'TTATGTGCCACACTTATTAATAAGAAAGAATATGTGAACCTTGCA'
+                'GATGTTTCCCTCTAGTAG'
+            ),
+            'SEQUENCE_INCLUDED_REGION': [36, 342],
+        }
+        global_args = {
+            'PRIMER_SECONDARY_STRUCTURE_ALIGNMENT': 1,  # key parameter for test
+            'PRIMER_OPT_SIZE': 20,
+            'PRIMER_PICK_INTERNAL_OLIGO': 1,
+            'PRIMER_INTERNAL_MAX_SELF_END': 8,
+            'PRIMER_MIN_SIZE': 18,
+            'PRIMER_MAX_SIZE': 25,
+            'PRIMER_OPT_TM': 60.0,
+            'PRIMER_MIN_TM': 57.0,
+            'PRIMER_MAX_TM': 63.0,
+            'PRIMER_MIN_GC': 20.0,
+            'PRIMER_MAX_GC': 80.0,
+            'PRIMER_MAX_POLY_X': 100,
+            'PRIMER_INTERNAL_MAX_POLY_X': 100,
+            'PRIMER_SALT_MONOVALENT': 50.0,
+            'PRIMER_DNA_CONC': 50.0,
+            'PRIMER_MAX_NS_ACCEPTED': 0,
+            'PRIMER_MAX_SELF_ANY': 12,
+            'PRIMER_MAX_SELF_END': 8,
+            'PRIMER_PAIR_MAX_COMPL_ANY': 12,
+            'PRIMER_PAIR_MAX_COMPL_END': 8,
+            'PRIMER_PRODUCT_SIZE_RANGE': [
+                [75, 100], [100, 125], [125, 150],
+                [150, 175], [175, 200], [200, 225],
+            ],
+        }
+        # This should run without a segmentation fault.
+        bindings.design_primers(
+            seq_args=seq_args,
+            global_args=global_args,
+        )
 
 
 def suite():
     suite = unittest.TestSuite()
     suite.addTest(TestDesignBindings())
     return suite
```

### Comparing `primer3-py-1.2.2/tests/test_thermoanalysis.py` & `primer3-py-2.0.0/tests/test_thermoanalysis.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/test_threadsafe.py` & `primer3-py-2.0.0/tests/test_threadsafe.py`

 * *Files identical despite different names*

### Comparing `primer3-py-1.2.2/tests/wrappers.py` & `primer3-py-2.0.0/tests/wrappers.py`

 * *Files identical despite different names*

