# Comparing `tmp/pddl-0.2.0.tar.gz` & `tmp/pddl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-0.2.0.tar", last modified: Fri Dec 23 04:07:39 2022, max compression
+gzip compressed data, was "pddl-0.3.1.tar", last modified: Wed May 31 14:41:11 2023, max compression
```

## Comparing `pddl-0.2.0.tar` & `pddl-0.3.1.tar`

### file list

```diff
@@ -1,716 +1,740 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.203492 pddl-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-23 04:07:18.000000 pddl-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-23 04:07:18.000000 pddl-0.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-23 04:07:18.000000 pddl-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-23 04:07:18.000000 pddl-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-23 04:07:18.000000 pddl-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2022-12-23 04:07:39.203492 pddl-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-23 04:07:18.000000 pddl-0.2.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2022-12-23 04:07:18.000000 pddl-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.075491 pddl-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-23 04:07:18.000000 pddl-0.2.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-23 04:07:18.000000 pddl-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-23 04:07:18.000000 pddl-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-23 04:07:18.000000 pddl-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-23 04:07:18.000000 pddl-0.2.0/docs/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.079491 pddl-0.2.0/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.079491 pddl-0.2.0/pddl/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/helpers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/helpers/cache_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.079491 pddl-0.2.0/pddl/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/logic/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.083491 pddl-0.2.0/pddl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/common.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/domain.lark
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/problem.lark
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2022-12-23 04:07:18.000000 pddl-0.2.0/pddl/parser/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.079491 pddl-0.2.0/pddl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32224 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 04:07:38.000000 pddl-0.2.0/pddl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-23 04:07:39.000000 pddl-0.2.0/pddl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      735 2022-12-23 04:07:39.203492 pddl-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2022-12-23 04:07:18.000000 pddl-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.083491 pddl-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.083491 pddl-0.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.083491 pddl-0.2.0/tests/fixtures/code_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/code_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/code_objects/blocksworld_fond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/code_objects/blocksworld_ipc08.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/code_objects/triangle_tireworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.071491 pddl-0.2.0/tests/fixtures/pddl_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.087491 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      740 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p08.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.087491 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      738 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    47814 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   101062 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   207558 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p11.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.095491 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/domain.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p01.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p02.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p03.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      277 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p04.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      305 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p05.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p06.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p07.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p08.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      305 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p09.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p10.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p11.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p12.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p13.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p14.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p15.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p16.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p17.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p18.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p19.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p20.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      615 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p21.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p22.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p23.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      615 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p24.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      615 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p25.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p26.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      615 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p27.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p28.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p29.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p30.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.095491 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld_fond/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld_fond/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/blocksworld_fond/p01.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.099491 pddl-0.2.0/tests/fixtures/pddl_files/doors/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2430 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/doors/p15.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.103491 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p16.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p17.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p18.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p19.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p20.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p21.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p22.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p23.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p24.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p25.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p26.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p27.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p28.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p29.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p30.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p31.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p32.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p33.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p34.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11582 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p35.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p36.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p37.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p38.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p39.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p40.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.107491 pddl-0.2.0/tests/fixtures/pddl_files/elevators/
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      419 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/elevators/p15.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.127491 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d01.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1029 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d02.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d03.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d04.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d05.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d06.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d07.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d08.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2399 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d09.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3105 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d10.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d11.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1737 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d12.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d13.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d14.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3855 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d15.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d16.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1755 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d17.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d18.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3141 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d19.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3873 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d20.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d21.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d22.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d23.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d24.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3159 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d25.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d26.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d27.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     5433 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d28.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d29.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d30.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2471 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d31.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d32.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3909 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d33.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4667 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d34.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     5451 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d35.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     6261 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d36.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d37.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d38.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2489 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d39.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3195 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d40.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3927 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d41.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4685 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d42.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     5469 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d43.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     6279 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d44.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     7115 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d45.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d46.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d47.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d48.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3215 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d49.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d50.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4705 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d51.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     5489 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d52.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     6299 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d53.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d54.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     8020 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d55.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p01.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p02.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      150 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p03.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      154 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p04.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      170 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p05.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p06.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p07.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      190 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p08.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p09.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p10.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p11.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p12.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      226 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p13.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p14.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      258 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p15.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p16.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      230 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p17.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      246 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p18.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p19.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p20.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      294 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p21.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p22.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      250 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p23.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      266 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p24.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p25.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p26.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p27.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p28.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p29.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      270 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p30.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      286 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p31.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p32.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      318 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p33.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      334 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p34.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p35.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p36.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p37.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      290 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p38.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p39.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p40.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p41.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p42.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p43.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p44.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      402 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p45.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      296 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p46.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p47.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      328 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p48.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p49.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p50.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      376 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p51.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      392 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p52.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      408 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p53.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p54.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/p55.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.147491 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/domain.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p01.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      542 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p02.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p03.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      758 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p04.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      867 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p05.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p06.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p07.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p08.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p09.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p10.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p100.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3284 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p101.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3366 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p102.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p103.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p104.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p105.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p106.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3575 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p107.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4599 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p108.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3026 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p109.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p11.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4051 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p110.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p12.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p13.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p14.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      978 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p15.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p16.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p17.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p18.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p19.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p20.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p31.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      905 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p32.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      932 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p33.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p34.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p35.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p36.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p37.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p38.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p39.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1760 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p40.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      768 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p41.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p42.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)      988 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p43.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p44.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1205 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p45.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p46.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p47.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1680 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p48.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p49.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p50.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p51.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p52.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p53.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p54.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p55.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p56.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1481 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p57.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2202 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p58.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p59.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p60.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p61.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1415 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p62.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p63.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p64.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2107 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p65.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1837 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p66.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p67.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p68.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2512 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p69.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p70.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1776 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p71.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p72.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p73.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p74.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p75.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p76.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2046 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p77.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2338 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p78.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p79.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p80.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2163 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p81.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1944 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p82.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1878 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p83.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2319 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p84.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p85.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p86.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p87.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2543 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p88.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3191 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p89.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3055 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p90.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p91.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3358 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p92.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3365 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p93.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p94.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2665 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p95.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3596 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p96.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     4047 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p97.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p98.pddl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p99.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.159491 pddl-0.2.0/tests/fixtures/pddl_files/islands/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      967 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p16.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p17.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p18.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p19.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p20.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p21.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p22.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p23.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p24.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p25.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p26.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p27.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p28.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p29.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p30.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p31.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p32.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p33.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p34.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p35.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p36.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p37.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p38.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p39.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p40.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p41.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p42.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p43.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p44.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p45.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p46.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p47.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p48.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p49.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p50.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p51.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p52.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p53.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p54.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p55.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p56.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p57.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p58.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p59.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/islands/p60.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.167491 pddl-0.2.0/tests/fixtures/pddl_files/miner/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3064 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p06.pddll
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p16.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p17.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p18.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p19.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p20.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p21.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p22.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p23.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p24.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p25.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p26.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p27.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p28.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p29.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p30.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p31.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p32.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p33.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p34.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p35.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p36.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p37.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p38.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p39.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p40.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p41.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p42.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p43.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p44.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p45.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p46.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p47.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p48.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p49.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p50.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/miner/p51.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.171491 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p09.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.171491 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1983 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p11.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.175491 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p15.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.187492 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      922 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      922 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      938 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      934 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      930 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p16.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p17.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p18.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p19.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p20.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p21.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p22.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p23.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p24.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p25.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p26.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p27.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p28.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p29.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p30.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p31.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p32.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p33.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-23 04:07:18.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p34.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p35.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p36.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p37.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p38.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p39.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p40.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p41.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p42.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p43.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p44.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p45.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p46.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p47.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p48.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p49.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p50.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p51.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p52.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p53.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p54.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p55.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p56.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p57.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p58.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p59.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p60.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p61.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p62.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p63.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p64.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p65.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p66.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p67.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p68.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p69.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p70.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p71.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p72.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p73.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p74.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p75.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.199492 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      419 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      901 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    20000 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    31109 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    35364 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p16.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    39895 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p17.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    44702 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p18.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    49785 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p19.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    55144 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p20.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    60779 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p21.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    66690 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p22.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    72877 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p23.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    79340 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p24.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    86079 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p25.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    93093 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p26.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   100384 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p27.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   107951 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p28.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   115794 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p29.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   123913 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p30.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   132308 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p31.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   140979 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p32.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   149926 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p33.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   159149 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p34.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   168648 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p35.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   178423 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p36.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   188474 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p37.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   198801 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p38.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   209404 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p39.pddl
--rw-r--r--   0 runner    (1001) docker     (123)   220283 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p40.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.203492 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p01.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      536 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p02.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      538 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p03.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      542 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p04.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p05.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p06.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p07.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      885 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p08.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      893 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p09.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p10.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p11.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p12.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p13.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p14.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p15.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.203492 pddl-0.2.0/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_docs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_docs/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 04:07:39.203492 pddl-0.2.0/tests/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_helpers/test_cache_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-23 04:07:19.000000 pddl-0.2.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.840979 pddl-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-31 14:40:58.000000 pddl-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 14:40:58.000000 pddl-0.3.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 14:40:58.000000 pddl-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 14:40:58.000000 pddl-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 14:40:58.000000 pddl-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-31 14:41:11.840979 pddl-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-31 14:40:58.000000 pddl-0.3.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-31 14:40:58.000000 pddl-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.628973 pddl-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 14:40:58.000000 pddl-0.3.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 14:40:58.000000 pddl-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 14:40:58.000000 pddl-0.3.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:40:58.000000 pddl-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 14:40:58.000000 pddl-0.3.1/docs/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.632973 pddl-0.3.1/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.632973 pddl-0.3.1/pddl/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/helpers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/helpers/cache_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.636973 pddl-0.3.1/pddl/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/logic/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.636973 pddl-0.3.1/pddl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/common.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/domain.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/problem.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-31 14:40:58.000000 pddl-0.3.1/pddl/parser/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.632973 pddl-0.3.1/pddl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33968 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 14:41:11.000000 pddl-0.3.1/pddl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 14:41:11.840979 pddl-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-31 14:40:58.000000 pddl-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.640973 pddl-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.644973 pddl-0.3.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.644973 pddl-0.3.1/tests/fixtures/code_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/code_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/code_objects/blocksworld_fond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/code_objects/blocksworld_ipc08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/code_objects/triangle_tireworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.624972 pddl-0.3.1/tests/fixtures/pddl_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.648973 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p08.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.652973 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    47814 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   101062 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   207558 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p11.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.664974 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/domain.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p01.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p02.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p03.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p04.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      305 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p05.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p06.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p07.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p08.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      305 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p09.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p10.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p11.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p12.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p13.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p14.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p15.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p16.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p17.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p18.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p19.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p20.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      615 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p21.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p22.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p23.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      615 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p24.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      615 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p25.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p26.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      615 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p27.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p28.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p29.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p30.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.664974 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld_fond/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld_fond/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/blocksworld_fond/p01.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.672974 pddl-0.3.1/tests/fixtures/pddl_files/doors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2430 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/doors/p15.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.688974 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p20.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p21.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p22.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p23.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p24.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p25.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p26.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p27.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p28.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p29.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p30.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p31.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p32.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p33.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p34.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p35.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p36.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p37.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p38.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p39.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p40.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.696975 pddl-0.3.1/tests/fixtures/pddl_files/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/elevators/p15.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.724976 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d01.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1029 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d02.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d03.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d04.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d05.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d06.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d07.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d08.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2399 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d09.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3105 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d10.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d11.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1737 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d12.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d13.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d14.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3855 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d15.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d16.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1755 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d17.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d18.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3141 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d19.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3873 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d20.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4631 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d21.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d22.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d23.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d24.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3159 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d25.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d26.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d27.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5433 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d28.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d29.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d30.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2471 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d31.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d32.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3909 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d33.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4667 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d34.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5451 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d35.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6261 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d36.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d37.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d38.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2489 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d39.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3195 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d40.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3927 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d41.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4685 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d42.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5469 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d43.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6279 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d44.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7115 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d45.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d46.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d47.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d48.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3215 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d49.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d50.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4705 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d51.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5489 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d52.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6299 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d53.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d54.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8020 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d55.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p01.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p02.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p03.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p04.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p05.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p06.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p07.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p08.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p09.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p10.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p11.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p12.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      226 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p13.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p14.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      258 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p15.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p16.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p17.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p18.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p19.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p20.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      294 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p21.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p22.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p23.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p24.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p25.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p26.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p27.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p28.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p29.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p30.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p31.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p32.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p33.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      334 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p34.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p35.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p36.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p37.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p38.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p39.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p40.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p41.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p42.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p43.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p44.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p45.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      296 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p46.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p47.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      328 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p48.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p49.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p50.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      376 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p51.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      392 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p52.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p53.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p54.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/p55.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.748977 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/domain.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p01.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      542 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p02.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p03.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      758 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p04.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p05.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p06.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p07.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p08.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p09.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p10.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p100.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3284 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p101.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3366 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p102.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p103.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p104.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p105.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p106.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3575 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p107.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4599 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p108.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3026 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p109.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p11.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4051 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p110.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p12.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p13.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p14.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p15.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p16.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p17.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p18.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p19.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p20.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p31.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      905 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p32.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      932 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p33.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p34.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p35.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p36.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p37.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p38.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p39.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1760 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p40.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      768 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p41.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p42.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p43.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p44.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1205 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p45.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p46.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p47.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1680 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p48.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p49.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p50.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p51.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p52.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p53.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p54.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p55.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1566 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p56.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1481 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p57.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2202 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p58.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p59.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p60.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p61.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1415 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p62.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p63.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p64.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2107 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p65.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1837 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p66.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p67.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p68.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2512 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p69.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p70.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1776 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p71.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p72.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p73.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p74.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p75.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p76.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2046 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p77.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2338 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p78.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p79.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p80.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2163 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p81.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1944 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p82.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1878 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p83.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2319 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p84.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p85.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p86.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p87.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2543 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p88.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3191 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p89.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3055 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p90.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p91.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3358 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p92.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3365 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p93.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p94.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2665 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p95.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3596 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p96.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4047 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p97.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p98.pddl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p99.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.764977 pddl-0.3.1/tests/fixtures/pddl_files/islands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p20.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p21.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p22.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p23.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p24.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p25.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p26.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p27.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p28.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p29.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p30.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p31.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p32.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p33.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p34.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p35.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p36.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p37.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p38.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p39.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p40.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p41.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p42.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p43.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p44.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p45.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p46.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p47.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p48.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p49.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p50.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p51.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p52.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p53.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p54.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p55.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p56.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p57.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p58.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p59.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/islands/p60.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.772977 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    22797 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    22773 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    38512 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    38500 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    50837 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    50843 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    50829 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    75786 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    66594 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    66663 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   121920 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   121892 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   121954 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   117556 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   117531 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   117605 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   175158 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   175170 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   175215 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p20.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.788978 pddl-0.3.1/tests/fixtures/pddl_files/miner/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3064 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p06.pddll
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p20.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p21.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p22.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p23.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p24.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p25.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p26.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p27.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p28.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p29.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p30.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p31.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p32.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p33.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p34.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p35.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p36.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p37.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p38.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p39.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p40.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p41.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p42.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p43.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p44.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p45.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p46.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p47.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p48.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p49.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p50.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/miner/p51.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.788978 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p09.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.792978 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1983 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p11.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.796978 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p15.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.816979 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2872 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p20.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p21.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p22.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p23.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p24.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p25.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p26.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p27.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p28.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p29.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p30.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p31.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p32.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p33.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p34.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p35.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p36.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p37.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p38.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p39.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p40.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p41.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p42.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p43.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p44.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p45.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p46.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p47.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p48.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p49.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p50.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p51.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p52.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p53.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p54.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p55.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p56.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p57.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p58.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p59.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p60.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p61.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p62.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p63.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p64.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p65.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p66.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p67.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p68.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p69.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p70.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p71.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p72.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p73.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p74.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p75.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.832979 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    31109 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    35364 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p16.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    39895 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p17.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    44702 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p18.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    49785 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p19.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    55144 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p20.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    60779 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p21.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    66690 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p22.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    72877 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p23.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    79340 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p24.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    86079 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p25.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    93093 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p26.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   100384 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p27.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   107951 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p28.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   115794 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p29.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   123913 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p30.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   132308 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p31.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   140979 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p32.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   149926 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p33.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   159149 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p34.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   168648 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p35.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   178423 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p36.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   188474 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p37.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   198801 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p38.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   209404 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p39.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)   220283 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p40.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.836979 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p01.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p02.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p03.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p04.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p05.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p06.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p07.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p08.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p09.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p10.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p11.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p12.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p13.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p14.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p15.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.840979 pddl-0.3.1/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_docs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_docs/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:41:11.840979 pddl-0.3.1/tests/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_helpers/test_cache_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 14:40:58.000000 pddl-0.3.1/tests/test_types.py
```

### Comparing `pddl-0.2.0/LICENSE` & `pddl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/PKG-INFO` & `pddl-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: pddl
-Version: 0.2.0
+Version: 0.3.1
 Summary: PDDL parser
 Home-page: https://github.com/AI-Planning/pddl.git
-Author: Marco Favorito, Francesco Fuggitti
-Author-email: marco.favorito@gmail.com, fuggitti@diag.uniroma1.it, christian.muise@queensu.ca
+Author: Marco Favorito, Francesco Fuggitti, Christian Muise
+Author-email: marco.favorito@gmail.com, francesco.fuggitti@gmail.com, christian.muise@queensu.ca
 License: MIT License
 Keywords: pddl
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <b>pddl</b>
 </h1>
 
@@ -135,15 +139,15 @@
 ```output
 (define (domain my_domain)
     (:requirements :strips :typing)
     (:types type_1)
     (:constants a b c)
     (:predicates (p1 ?x - type_1 ?y - type_1 ?z - type_1)  (p2 ?x - type_1 ?y - type_1))
     (:action action-1
-        :parameters (?x - type_1 ?y - type_1 ?z - type_1 )
+        :parameters (?x - type_1 ?y - type_1 ?z - type_1)
         :precondition (and (p1 ?x ?y ?z) (not (p2 ?y ?z)))
         :effect (p2 ?y ?z)
     )
 )
 ```
 
 As well as a PDDL problem:
@@ -233,14 +237,15 @@
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
 ## Authors
 
 - [Marco Favorito](https://marcofavorito.me)
 - [Francesco Fuggitti](https://francescofuggitti.github.io)
+- [Christian Muise](http://www.haz.ca/)
 
 ## License
 
 `pddl` is released under the MIT License.
 
 Copyright (c) 2021-2022 WhiteMech
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: pddl Version: 0.2.0 Summary: PDDL parser Home-page:
+Metadata-Version: 2.1 Name: pddl Version: 0.3.1 Summary: PDDL parser Home-page:
 https://github.com/AI-Planning/pddl.git Author: Marco Favorito, Francesco
-Fuggitti Author-email: marco.favorito@gmail.com, fuggitti@diag.uniroma1.it,
-christian.muise@queensu.ca License: MIT License Keywords: pddl Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
+Fuggitti, Christian Muise Author-email: marco.favorito@gmail.com,
+francesco.fuggitti@gmail.com, christian.muise@queensu.ca License: MIT License
+Keywords: pddl Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Education Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE
                               ****** pddl ******
 [PyPI] [PyPI_-_Python_Version] [PyPI - Status] [PyPI - Implementation] [PyPI -
                                 Wheel] [GitHub]
                         [test] [lint] [docs] [codecov]
                                     [black]
 `pddl` aims to be an unquestionable and complete parser for PDDL 3.1. ##
 Install - from PyPI: ``` pip install pddl ``` - from source (`main` branch):
@@ -28,15 +31,15 @@
 & ~p2(y, z), effect=p2(y, z) ) # define the domain object. requirements =
 [Requirements.STRIPS, Requirements.TYPING] domain = Domain("my_domain",
 requirements=requirements, types=["type_1"], constants=[a, b, c], predicates=
 [p1, p2], actions=[a1]) print(domain_to_string(domain)) ``` that gives:
 ```output (define (domain my_domain) (:requirements :strips :typing) (:types
 type_1) (:constants a b c) (:predicates (p1 ?x - type_1 ?y - type_1 ?z -
 type_1) (p2 ?x - type_1 ?y - type_1)) (:action action-1 :parameters (?x -
-type_1 ?y - type_1 ?z - type_1 ) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
+type_1 ?y - type_1 ?z - type_1) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
 ?z))) :effect (p2 ?y ?z) ) ) ``` As well as a PDDL problem: ```python problem =
 Problem( "problem-1", domain=domain, requirements=requirements, objects=[a, b,
 c], init=[p1(a, b, c), ~p2(b, c)], goal=p2(b, c) ) print(problem_to_string
 (problem)) ``` Output: ```output (define (problem problem-1) (:domain
 my_domain) (:requirements :strips :typing) (:objects a - type_1 b - type_1 c -
 type_1) (:init (not (p2 b c)) (p1 a b c)) (:goal (p2 b c)) ) ``` Example
 parsing: ```python from pddl import parse_domain, parse_problem domain =
@@ -59,17 +62,17 @@
 fork.readthedocs.io/en/latest/) - Clone the repository: `git clone https://
 github.com/AI-Planning/pddl.git && cd pddl` - Install development dependencies:
 `pipenv shell --python 3.7 && pipenv install --dev` ## Tests To run tests:
 `tox` To run only the code tests: `tox -e py37` To run only the code style
 checks: `tox -e flake8` ## Docs To build the docs: `mkdocs build` To view
 documentation in a browser: `mkdocs serve` and then go to [http://localhost:
 8000](http://localhost:8000) ## Authors - [Marco Favorito](https://
-marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io)
-## License `pddl` is released under the MIT License. Copyright (c) 2021-2022
-WhiteMech ## Acknowledgements The `pddl` project is partially supported by the
-ERC Advanced Grant WhiteMech (No. 834228), the EU ICT-48 2020 project TAILOR
-(No. 952215), the PRIN project RIPER (No. 20203FFYLK), and the JPMorgan AI
-Faculty Research Award "Resilience-based Generalized Planning and Strategic
-Reasoning". # Change Log ## 0.1.0 (2021-06-21) The first official release of
-pddl. Main features: * Specify PDDL domains and problems programmatically. *
-Parsing for PDDL domains and problems. ## 0.0.1 (2020-07-30) * First commit on
-the package.
+marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io) -
+[Christian Muise](http://www.haz.ca/) ## License `pddl` is released under the
+MIT License. Copyright (c) 2021-2022 WhiteMech ## Acknowledgements The `pddl`
+project is partially supported by the ERC Advanced Grant WhiteMech (No.
+834228), the EU ICT-48 2020 project TAILOR (No. 952215), the PRIN project RIPER
+(No. 20203FFYLK), and the JPMorgan AI Faculty Research Award "Resilience-based
+Generalized Planning and Strategic Reasoning". # Change Log ## 0.1.0 (2021-06-
+21) The first official release of pddl. Main features: * Specify PDDL domains
+and problems programmatically. * Parsing for PDDL domains and problems. ##
+0.0.1 (2020-07-30) * First commit on the package.
```

### Comparing `pddl-0.2.0/README.md` & `pddl-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 ```output
 (define (domain my_domain)
     (:requirements :strips :typing)
     (:types type_1)
     (:constants a b c)
     (:predicates (p1 ?x - type_1 ?y - type_1 ?z - type_1)  (p2 ?x - type_1 ?y - type_1))
     (:action action-1
-        :parameters (?x - type_1 ?y - type_1 ?z - type_1 )
+        :parameters (?x - type_1 ?y - type_1 ?z - type_1)
         :precondition (and (p1 ?x ?y ?z) (not (p2 ?y ?z)))
         :effect (p2 ?y ?z)
     )
 )
 ```
 
 As well as a PDDL problem:
@@ -214,14 +214,15 @@
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
 ## Authors
 
 - [Marco Favorito](https://marcofavorito.me)
 - [Francesco Fuggitti](https://francescofuggitti.github.io)
+- [Christian Muise](http://www.haz.ca/)
 
 ## License
 
 `pddl` is released under the MIT License.
 
 Copyright (c) 2021-2022 WhiteMech
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 & ~p2(y, z), effect=p2(y, z) ) # define the domain object. requirements =
 [Requirements.STRIPS, Requirements.TYPING] domain = Domain("my_domain",
 requirements=requirements, types=["type_1"], constants=[a, b, c], predicates=
 [p1, p2], actions=[a1]) print(domain_to_string(domain)) ``` that gives:
 ```output (define (domain my_domain) (:requirements :strips :typing) (:types
 type_1) (:constants a b c) (:predicates (p1 ?x - type_1 ?y - type_1 ?z -
 type_1) (p2 ?x - type_1 ?y - type_1)) (:action action-1 :parameters (?x -
-type_1 ?y - type_1 ?z - type_1 ) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
+type_1 ?y - type_1 ?z - type_1) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
 ?z))) :effect (p2 ?y ?z) ) ) ``` As well as a PDDL problem: ```python problem =
 Problem( "problem-1", domain=domain, requirements=requirements, objects=[a, b,
 c], init=[p1(a, b, c), ~p2(b, c)], goal=p2(b, c) ) print(problem_to_string
 (problem)) ``` Output: ```output (define (problem problem-1) (:domain
 my_domain) (:requirements :strips :typing) (:objects a - type_1 b - type_1 c -
 type_1) (:init (not (p2 b c)) (p1 a b c)) (:goal (p2 b c)) ) ``` Example
 parsing: ```python from pddl import parse_domain, parse_problem domain =
@@ -50,14 +50,14 @@
 fork.readthedocs.io/en/latest/) - Clone the repository: `git clone https://
 github.com/AI-Planning/pddl.git && cd pddl` - Install development dependencies:
 `pipenv shell --python 3.7 && pipenv install --dev` ## Tests To run tests:
 `tox` To run only the code tests: `tox -e py37` To run only the code style
 checks: `tox -e flake8` ## Docs To build the docs: `mkdocs build` To view
 documentation in a browser: `mkdocs serve` and then go to [http://localhost:
 8000](http://localhost:8000) ## Authors - [Marco Favorito](https://
-marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io)
-## License `pddl` is released under the MIT License. Copyright (c) 2021-2022
-WhiteMech ## Acknowledgements The `pddl` project is partially supported by the
-ERC Advanced Grant WhiteMech (No. 834228), the EU ICT-48 2020 project TAILOR
-(No. 952215), the PRIN project RIPER (No. 20203FFYLK), and the JPMorgan AI
-Faculty Research Award "Resilience-based Generalized Planning and Strategic
-Reasoning".
+marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io) -
+[Christian Muise](http://www.haz.ca/) ## License `pddl` is released under the
+MIT License. Copyright (c) 2021-2022 WhiteMech ## Acknowledgements The `pddl`
+project is partially supported by the ERC Advanced Grant WhiteMech (No.
+834228), the EU ICT-48 2020 project TAILOR (No. 952215), the PRIN project RIPER
+(No. 20203FFYLK), and the JPMorgan AI Faculty Research Award "Resilience-based
+Generalized Planning and Strategic Reasoning".
```

### Comparing `pddl-0.2.0/pddl/__init__.py` & `pddl-0.3.1/pddl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -23,14 +22,15 @@
     __url__,
     __version__,
 )
 from .helpers.base import _get_current_path
 
 _ROOT_PATH = _get_current_path()
 
+
 # Simple helpers
 def parse_domain(fn):
     from pddl.parser.domain import DomainParser
 
     with open(fn, "r") as f:
         dtext = f.read()
     return DomainParser()(dtext)
```

### Comparing `pddl-0.2.0/pddl/__main__.py` & `pddl-0.3.1/pddl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/__version__.py` & `pddl-0.3.1/pddl/__version__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -12,14 +11,14 @@
 #
 
 """Package metadata declaration."""
 
 __title__ = "pddl"
 __description__ = "PDDL parser"
 __url__ = "https://github.com/AI-Planning/pddl.git"
-__version__ = "0.2.0"
-__author__ = "Marco Favorito, Francesco Fuggitti"
+__version__ = "0.3.1"
+__author__ = "Marco Favorito, Francesco Fuggitti, Christian Muise"
 __author_email__ = (
-    "marco.favorito@gmail.com, fuggitti@diag.uniroma1.it, christian.muise@queensu.ca"
+    "marco.favorito@gmail.com, francesco.fuggitti@gmail.com, christian.muise@queensu.ca"
 )
 __license__ = "MIT License"
 __copyright__ = "2021-2022 WhiteMech"
```

### Comparing `pddl-0.2.0/pddl/core.py` & `pddl-0.3.1/pddl/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/custom_types.py` & `pddl-0.3.1/pddl/custom_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/exceptions.py` & `pddl-0.3.1/pddl/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/formatter.py` & `pddl-0.3.1/pddl/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -40,15 +39,15 @@
             result += f"({p.name})"
         else:
             result += f"({p.name}"
             for t in p.terms:
                 result += (
                     f" ?{t.name} - {' '.join(t.type_tags)}"
                     if t.type_tags
-                    else f"?{t.name}"
+                    else f" ?{t.name}"
                 )
             result += ") "
         result += " "
     return result.strip()
 
 
 def _print_objects_with_types(objects: Collection):
```

### Comparing `pddl-0.2.0/pddl/helpers/base.py` & `pddl-0.3.1/pddl/helpers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -22,16 +21,22 @@
     """Get the path to the file where the function is called."""
     import inspect
     import os
 
     return Path(os.path.dirname(inspect.getfile(inspect.currentframe()))).parent  # type: ignore
 
 
-def assert_(condition: bool, message: str = ""):
-    """User-defined assert."""
+def assert_(condition: bool, message: str = "") -> None:
+    """
+    User-defined assert.
+
+    This function is useful to avoid the use of the built-in assert statement, which is removed
+        when the code is compiled in optimized mode. For more information, see
+        https://bandit.readthedocs.io/en/1.7.5/plugins/b101_assert_used.html
+    """
     if not condition:
         raise AssertionError(message)
 
 
 def ensure(arg: Optional[Any], default: Any):
     """Ensure an object is not None, or return a default."""
     return arg if arg is not None else default
@@ -89,15 +94,15 @@
     """Return a list of parameters along with types if available."""
     result = ""
     for p in parameters:
         if p.type_tags:
             result += f"?{p.name} - {' '.join(map(str, p.type_tags))} "
         else:
             result += str(p) + " "
-    return result
+    return result.strip()
 
 
 class RegexConstrainedString(str):
     """
     A string that is constrained by a regex.
 
     The default behaviour is to match anything.
```

### Comparing `pddl-0.2.0/pddl/helpers/cache_hash.py` & `pddl-0.3.1/pddl/helpers/cache_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/logic/base.py` & `pddl-0.3.1/pddl/logic/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/logic/effects.py` & `pddl-0.3.1/pddl/logic/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 #
 
 """This modules implements PDDL effects."""
 import functools
 from typing import AbstractSet, Collection, Generic, Optional, Sequence, TypeVar, Union
 
-from pddl.helpers.base import ensure_set
+from pddl.helpers.base import _typed_parameters, ensure_set
 from pddl.helpers.cache_hash import cache_hash
 from pddl.logic import Variable
 from pddl.logic.base import Atomic, Formula, Not, OneOf
 from pddl.parser.symbols import Symbols
 
 EffectType = TypeVar("EffectType")
 
@@ -137,15 +136,15 @@
     @property
     def variables(self) -> AbstractSet[Variable]:
         """Get the variables."""
         return self._variables
 
     def __str__(self) -> str:
         """Get the string representation."""
-        return f"({Symbols.FORALL.value} ({' '.join(map(str, self.variables))}) {self.effect})"
+        return f"({Symbols.FORALL.value} ({_typed_parameters(self.variables)}) {self.effect})"
 
     def __repr__(self) -> str:
         """Get an unambiguous string representation."""
         return f"{type(self).__name__}({self.variables}, {self.effect})"
 
     def __eq__(self, other) -> bool:
         """Compare with another object."""
```

### Comparing `pddl-0.2.0/pddl/logic/helpers.py` & `pddl-0.3.1/pddl/logic/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/logic/predicates.py` & `pddl-0.3.1/pddl/logic/predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -124,19 +123,19 @@
 
     def __hash__(self) -> int:
         """Get the hash."""
         return hash((EqualTo, self.left, self.right))
 
     def __str__(self) -> str:
         """Get the string representation."""
-        return f"({Symbols.EQUAL} {self.left} {self.right})"
+        return f"({Symbols.EQUAL.value} {self.left} {self.right})"
 
     def __repr__(self) -> str:
         """Get the string representation."""
-        return f"{type(self).__name__}({self.left}, {self.right})"
+        return f"{type(self).__name__}({repr(self.left)}, {repr(self.right)})"
 
 
 @cache_hash
 @functools.total_ordering
 class DerivedPredicate(Atomic):
     """A class for a Derived Predicates in PDDL."""
```

### Comparing `pddl-0.2.0/pddl/logic/terms.py` & `pddl-0.3.1/pddl/logic/terms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -111,12 +110,16 @@
 
     def __repr__(self):
         """Get a unique representation of the object."""
         return f"Variable({self.name})"
 
     def __eq__(self, other) -> bool:
         """Compare with another object."""
-        return isinstance(other, Variable) and self.name == other.name
+        return (
+            isinstance(other, Variable)
+            and self.name == other.name
+            and self.type_tags == other.type_tags
+        )
 
     def __hash__(self) -> int:
         """Get the hash."""
         return hash((Variable, self._name))
```

### Comparing `pddl-0.2.0/pddl/parser/__init__.py` & `pddl-0.3.1/pddl/parser/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/pddl/parser/common.lark` & `pddl-0.3.1/pddl/parser/common.lark`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/pddl/parser/domain.lark` & `pddl-0.3.1/pddl/parser/domain.lark`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/pddl/parser/domain.py` & `pddl-0.3.1/pddl/parser/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 #
 
 """Implementation of the PDDL domain parser."""
+import sys
 from typing import Dict, Set
 
 from lark import Lark, ParseError, Transformer
 
 from pddl.core import Action, Domain, Requirements
 from pddl.exceptions import PDDLMissingRequirementError
 from pddl.helpers.base import assert_, safe_get, safe_index
@@ -51,24 +51,25 @@
 
     def start(self, args):
         """Entry point."""
         return args[0]
 
     def domain(self, args):
         """Process the 'domain' rule."""
+        args = [arg for arg in args if arg is not None]
         kwargs = {}
         actions = []
         derived_predicates = []
         for arg in args[2:-1]:
             if isinstance(arg, Action):
                 actions.append(arg)
             elif isinstance(arg, DerivedPredicate):
                 derived_predicates.append(arg)
             else:
-                assert isinstance(arg, dict)
+                assert_(isinstance(arg, dict))
                 kwargs.update(arg)
         kwargs.update(actions=actions, derived_predicates=derived_predicates)
         return Domain(**kwargs)
 
     def domain_def(self, args):
         """Process the 'domain_def' rule."""
         return dict(name=args[2])
@@ -222,15 +223,16 @@
         raise ValueError("case not recognized")
 
     def c_effect(self, args):
         """Process the 'c_effect' rule."""
         if len(args) == 1:
             return args[0]
         if args[1] == Symbols.FORALL.value:
-            return Forall(effect=args[-2], variables=args[3])
+            variables = [Variable(name, tags) for name, tags in args[3].items()]
+            return Forall(effect=args[-2], variables=variables)
         if args[1] == Symbols.WHEN.value:
             return When(args[2], args[3])
         if args[1] == Symbols.ONEOF.value:
             if not bool({Requirements.NON_DETERMINISTIC} & self._extended_requirements):
                 raise PDDLMissingRequirementError(Requirements.NON_DETERMINISTIC)
             return OneOf(*args[2:-1])
         raise ValueError()
@@ -243,15 +245,15 @@
             return Not(args[2])
 
     def cond_effect(self, args):
         """Process the 'cond_effect' rule."""
         if len(args) >= 3 and args[1] == Symbols.AND.value:
             p_effects = args[2:-1]
             return And(*p_effects)
-        assert len(args) == 1
+        assert_(len(args) == 1)
         return args[0]
 
     def atomic_formula_term(self, args):
         """Process the 'atomic_formula_term' rule."""
 
         def constant_or_variable(t):
             # Case where the term is a free variable (bug) or comes from a parent quantifier
@@ -345,10 +347,12 @@
         self._transformer = DomainTransformer()
         self._parser = Lark(
             _domain_parser_lark, parser="lalr", import_paths=[PARSERS_DIRECTORY]
         )
 
     def __call__(self, text):
         """Call."""
+        sys.tracebacklimit = 0  # noqa
         tree = self._parser.parse(text)
+        sys.tracebacklimit = None  # noqa
         formula = self._transformer.transform(tree)
         return formula
```

### Comparing `pddl-0.2.0/pddl/parser/problem.lark` & `pddl-0.3.1/pddl/parser/problem.lark`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/pddl/parser/problem.py` & `pddl-0.3.1/pddl/parser/problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 #
 
 """Implementation of the PDDL problem parser."""
+import sys
 from typing import Dict
 
 from lark import Lark, ParseError, Transformer
 
 from pddl.core import Problem, Requirements
+from pddl.helpers.base import assert_
 from pddl.logic.base import And, Not
 from pddl.logic.predicates import EqualTo, Predicate
 from pddl.logic.terms import Constant
 from pddl.parser import PARSERS_DIRECTORY, PROBLEM_GRAMMAR_FILE
 from pddl.parser.domain import DomainTransformer
 from pddl.parser.symbols import Symbols
 
@@ -37,14 +38,19 @@
 
     def start(self, args):
         """Process the rule 'start'."""
         return args[0]
 
     def problem(self, args):
         """Process the 'problem' rule."""
+        args = [arg for arg in args if arg is not None]
+        assert_(
+            (args[0].value + args[1].value + args[-1].value == "(define)"),
+            "Problem should start with '(define' and close with ')'",
+        )
         return Problem(**dict(args[2:-1]))
 
     def problem_def(self, args):
         """Process the 'problem_def' rule."""
         return "name", args[2]
 
     def problem_domain(self, args):
@@ -73,15 +79,15 @@
         :param args: the argument of this grammar rule
         :return: a typed list (name)
         """
         return self._domain_transformer._typed_list_x(args)
 
     def domain__type_def(self, names):
         """Process a domain type def."""
-        assert len(names) == 1
+        assert_(len(names) == 1)
         return str(names[0])
 
     def init(self, args):
         """Process the 'init' rule."""
         return "init", args[2:-1]
 
     def literal_name(self, args):
@@ -136,10 +142,12 @@
         self._transformer = ProblemTransformer()
         self._parser = Lark(
             _problem_parser_lark, parser="lalr", import_paths=[PARSERS_DIRECTORY]
         )
 
     def __call__(self, text):
         """Call."""
+        sys.tracebacklimit = 0  # noqa
         tree = self._parser.parse(text)
+        sys.tracebacklimit = None  # noqa
         formula = self._transformer.transform(tree)
         return formula
```

### Comparing `pddl-0.2.0/pddl/parser/symbols.py` & `pddl-0.3.1/pddl/parser/symbols.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -48,15 +47,15 @@
     EFFECT = ":effect"
     ROUND_BRACKET_LEFT = "("
     ROUND_BRACKET_RIGHT = ")"
     TYPE_SEP = "-"
     EQUAL = "="
 
 
-ALL_SYMBOLS = {v.value for v in Symbols}  # type: Set[str]
+ALL_SYMBOLS: Set[str] = {v.value for v in Symbols}
 
 
 class RequirementSymbols(Enum):
     """A set of requirements that can be used in PDDL."""
 
     STRIPS = ":strips"
     TYPING = ":typing"
@@ -72,8 +71,8 @@
     NON_DETERMINISTIC = ":non-deterministic"
 
     def strip(self) -> str:
         """Strip the leading colon."""
         return self.value[1:]
 
 
-ALL_REQUIREMENTS = {v.value for v in RequirementSymbols}  # type: Set[str]
+ALL_REQUIREMENTS: Set[str] = {v.value for v in RequirementSymbols}
```

### Comparing `pddl-0.2.0/pddl.egg-info/PKG-INFO` & `pddl-0.3.1/pddl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: pddl
-Version: 0.2.0
+Version: 0.3.1
 Summary: PDDL parser
 Home-page: https://github.com/AI-Planning/pddl.git
-Author: Marco Favorito, Francesco Fuggitti
-Author-email: marco.favorito@gmail.com, fuggitti@diag.uniroma1.it, christian.muise@queensu.ca
+Author: Marco Favorito, Francesco Fuggitti, Christian Muise
+Author-email: marco.favorito@gmail.com, francesco.fuggitti@gmail.com, christian.muise@queensu.ca
 License: MIT License
 Keywords: pddl
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <b>pddl</b>
 </h1>
 
@@ -135,15 +139,15 @@
 ```output
 (define (domain my_domain)
     (:requirements :strips :typing)
     (:types type_1)
     (:constants a b c)
     (:predicates (p1 ?x - type_1 ?y - type_1 ?z - type_1)  (p2 ?x - type_1 ?y - type_1))
     (:action action-1
-        :parameters (?x - type_1 ?y - type_1 ?z - type_1 )
+        :parameters (?x - type_1 ?y - type_1 ?z - type_1)
         :precondition (and (p1 ?x ?y ?z) (not (p2 ?y ?z)))
         :effect (p2 ?y ?z)
     )
 )
 ```
 
 As well as a PDDL problem:
@@ -233,14 +237,15 @@
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
 ## Authors
 
 - [Marco Favorito](https://marcofavorito.me)
 - [Francesco Fuggitti](https://francescofuggitti.github.io)
+- [Christian Muise](http://www.haz.ca/)
 
 ## License
 
 `pddl` is released under the MIT License.
 
 Copyright (c) 2021-2022 WhiteMech
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 2.1 Name: pddl Version: 0.2.0 Summary: PDDL parser Home-page:
+Metadata-Version: 2.1 Name: pddl Version: 0.3.1 Summary: PDDL parser Home-page:
 https://github.com/AI-Planning/pddl.git Author: Marco Favorito, Francesco
-Fuggitti Author-email: marco.favorito@gmail.com, fuggitti@diag.uniroma1.it,
-christian.muise@queensu.ca License: MIT License Keywords: pddl Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
+Fuggitti, Christian Muise Author-email: marco.favorito@gmail.com,
+francesco.fuggitti@gmail.com, christian.muise@queensu.ca License: MIT License
+Keywords: pddl Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Education Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE
                               ****** pddl ******
 [PyPI] [PyPI_-_Python_Version] [PyPI - Status] [PyPI - Implementation] [PyPI -
                                 Wheel] [GitHub]
                         [test] [lint] [docs] [codecov]
                                     [black]
 `pddl` aims to be an unquestionable and complete parser for PDDL 3.1. ##
 Install - from PyPI: ``` pip install pddl ``` - from source (`main` branch):
@@ -28,15 +31,15 @@
 & ~p2(y, z), effect=p2(y, z) ) # define the domain object. requirements =
 [Requirements.STRIPS, Requirements.TYPING] domain = Domain("my_domain",
 requirements=requirements, types=["type_1"], constants=[a, b, c], predicates=
 [p1, p2], actions=[a1]) print(domain_to_string(domain)) ``` that gives:
 ```output (define (domain my_domain) (:requirements :strips :typing) (:types
 type_1) (:constants a b c) (:predicates (p1 ?x - type_1 ?y - type_1 ?z -
 type_1) (p2 ?x - type_1 ?y - type_1)) (:action action-1 :parameters (?x -
-type_1 ?y - type_1 ?z - type_1 ) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
+type_1 ?y - type_1 ?z - type_1) :precondition (and (p1 ?x ?y ?z) (not (p2 ?y
 ?z))) :effect (p2 ?y ?z) ) ) ``` As well as a PDDL problem: ```python problem =
 Problem( "problem-1", domain=domain, requirements=requirements, objects=[a, b,
 c], init=[p1(a, b, c), ~p2(b, c)], goal=p2(b, c) ) print(problem_to_string
 (problem)) ``` Output: ```output (define (problem problem-1) (:domain
 my_domain) (:requirements :strips :typing) (:objects a - type_1 b - type_1 c -
 type_1) (:init (not (p2 b c)) (p1 a b c)) (:goal (p2 b c)) ) ``` Example
 parsing: ```python from pddl import parse_domain, parse_problem domain =
@@ -59,17 +62,17 @@
 fork.readthedocs.io/en/latest/) - Clone the repository: `git clone https://
 github.com/AI-Planning/pddl.git && cd pddl` - Install development dependencies:
 `pipenv shell --python 3.7 && pipenv install --dev` ## Tests To run tests:
 `tox` To run only the code tests: `tox -e py37` To run only the code style
 checks: `tox -e flake8` ## Docs To build the docs: `mkdocs build` To view
 documentation in a browser: `mkdocs serve` and then go to [http://localhost:
 8000](http://localhost:8000) ## Authors - [Marco Favorito](https://
-marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io)
-## License `pddl` is released under the MIT License. Copyright (c) 2021-2022
-WhiteMech ## Acknowledgements The `pddl` project is partially supported by the
-ERC Advanced Grant WhiteMech (No. 834228), the EU ICT-48 2020 project TAILOR
-(No. 952215), the PRIN project RIPER (No. 20203FFYLK), and the JPMorgan AI
-Faculty Research Award "Resilience-based Generalized Planning and Strategic
-Reasoning". # Change Log ## 0.1.0 (2021-06-21) The first official release of
-pddl. Main features: * Specify PDDL domains and problems programmatically. *
-Parsing for PDDL domains and problems. ## 0.0.1 (2020-07-30) * First commit on
-the package.
+marcofavorito.me) - [Francesco Fuggitti](https://francescofuggitti.github.io) -
+[Christian Muise](http://www.haz.ca/) ## License `pddl` is released under the
+MIT License. Copyright (c) 2021-2022 WhiteMech ## Acknowledgements The `pddl`
+project is partially supported by the ERC Advanced Grant WhiteMech (No.
+834228), the EU ICT-48 2020 project TAILOR (No. 952215), the PRIN project RIPER
+(No. 20203FFYLK), and the JPMorgan AI Faculty Research Award "Resilience-based
+Generalized Planning and Strategic Reasoning". # Change Log ## 0.1.0 (2021-06-
+21) The first official release of pddl. Main features: * Specify PDDL domains
+and problems programmatically. * Parsing for PDDL domains and problems. ##
+0.0.1 (2020-07-30) * First commit on the package.
```

### Comparing `pddl-0.2.0/pddl.egg-info/SOURCES.txt` & `pddl-0.3.1/pddl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 pddl/parser/symbols.py
 tests/__init__.py
 tests/conftest.py
 tests/test_action.py
 tests/test_actions.py
 tests/test_cli.py
 tests/test_domain.py
+tests/test_formatter.py
 tests/test_parser.py
 tests/test_predicate.py
 tests/test_problem.py
 tests/test_types.py
 tests/fixtures/__init__.py
 tests/fixtures/code_objects/__init__.py
 tests/fixtures/code_objects/blocksworld_fond.py
@@ -452,14 +453,36 @@
 tests/fixtures/pddl_files/islands/p54.pddl
 tests/fixtures/pddl_files/islands/p55.pddl
 tests/fixtures/pddl_files/islands/p56.pddl
 tests/fixtures/pddl_files/islands/p57.pddl
 tests/fixtures/pddl_files/islands/p58.pddl
 tests/fixtures/pddl_files/islands/p59.pddl
 tests/fixtures/pddl_files/islands/p60.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/README.md
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/domain.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p01.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p02.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p03.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p04.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p05.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p06.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p07.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p08.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p09.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p10.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p11.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p12.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p13.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p14.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p15.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p16.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p17.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p18.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p19.pddl
+tests/fixtures/pddl_files/maintenance-sequential-satisficing-ipc2014/p20.pddl
 tests/fixtures/pddl_files/miner/domain.pddl
 tests/fixtures/pddl_files/miner/p01.pddl
 tests/fixtures/pddl_files/miner/p02.pddl
 tests/fixtures/pddl_files/miner/p03.pddl
 tests/fixtures/pddl_files/miner/p04.pddl
 tests/fixtures/pddl_files/miner/p05.pddl
 tests/fixtures/pddl_files/miner/p06.pddll
```

### Comparing `pddl-0.2.0/setup.cfg` & `pddl-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/setup.py` & `pddl-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -48,15 +47,19 @@
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
+    python_requires='>=3.7',
     install_requires=install_requires,
     license=about["__license__"],
     include_package_data=True,
     data_files=[
         ("pddl/parser", glob.glob("pddl/parser/*.lark")),
     ],
     keywords='pddl',
```

### Comparing `pddl-0.2.0/tests/conftest.py` & `pddl-0.3.1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -47,14 +46,15 @@
     "blocksworld_fond",
     "doors",
     # "earth_observation",
     "elevators",
     # "faults-ipc08",
     # "first-responders-ipc08",
     "islands",
+    "maintenance-sequential-satisficing-ipc2014",
     "miner",
     "rovers_fond",
     "spiky-tireworld",
     "tireworld",
     "tireworld-truck",
     "triangle-tireworld",
     "zenotravel",
```

### Comparing `pddl-0.2.0/tests/fixtures/code_objects/blocksworld_fond.py` & `pddl-0.3.1/tests/fixtures/code_objects/blocksworld_fond.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/fixtures/code_objects/blocksworld_ipc08.py` & `pddl-0.3.1/tests/fixtures/code_objects/blocksworld_ipc08.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/fixtures/code_objects/triangle_tireworld.py` & `pddl-0.3.1/tests/fixtures/code_objects/triangle_tireworld.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/acrobatics/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/acrobatics/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/beam-walk/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/beam-walk/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld-ipc08/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld-ipc08/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/blocksworld_fond/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/blocksworld_fond/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/doors/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/doors/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/earth_observation/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/earth_observation/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/elevators/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/elevators/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d41.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d41.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d42.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d42.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d43.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d43.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d44.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d44.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d45.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d45.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d46.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d46.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d47.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d47.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d48.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d48.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d49.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d49.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d50.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d50.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d51.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d51.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d52.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d52.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d53.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d53.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d54.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d54.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/faults-ipc08/d55.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/faults-ipc08/d55.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p100.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p100.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p101.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p101.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p102.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p102.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p103.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p103.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p104.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p104.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p105.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p105.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p106.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p106.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p107.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p107.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p108.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p108.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p109.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p109.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p110.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p110.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p41.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p41.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p42.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p42.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p43.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p43.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p44.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p44.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p45.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p45.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p46.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p46.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p47.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p47.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p48.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p48.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p49.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p49.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p50.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p50.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p51.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p51.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p52.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p52.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p53.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p53.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p54.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p54.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p55.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p55.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p56.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p56.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p57.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p57.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p58.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p58.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p59.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p59.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p60.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p60.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p61.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p61.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p62.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p62.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p63.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p63.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p64.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p64.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p65.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p65.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p66.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p66.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p67.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p67.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p68.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p68.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p69.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p69.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p70.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p70.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p71.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p71.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p72.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p72.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p73.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p73.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p74.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p74.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p75.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p75.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p76.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p76.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p77.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p77.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p78.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p78.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p79.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p79.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p80.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p80.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p81.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p81.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p82.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p82.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p83.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p83.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p84.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p84.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p85.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p85.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p86.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p86.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p87.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p87.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p88.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p88.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p89.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p89.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p90.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p90.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p91.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p91.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p92.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p92.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p93.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p93.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p94.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p94.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p95.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p95.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p96.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p96.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p97.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p97.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p98.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p98.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/first-responders-ipc08/p99.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/first-responders-ipc08/p99.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p41.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p41.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p42.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p42.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p43.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p43.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p44.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p44.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p45.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p45.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p46.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p46.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p47.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p47.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p48.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p48.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p49.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p49.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p50.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p50.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p51.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p51.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p52.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p52.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p53.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p53.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p54.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p54.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p55.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p55.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p56.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p56.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p57.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p57.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p58.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p58.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p59.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p59.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/islands/p60.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/islands/p60.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p06.pddll` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p06.pddll`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p41.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p41.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p42.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p42.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p43.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p43.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p44.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p44.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p45.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p45.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p46.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p46.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p47.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p47.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p48.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p48.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p49.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p49.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p50.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p50.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/miner/p51.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/miner/p51.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/rovers_fond/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/rovers_fond/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/spiky-tireworld/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/spiky-tireworld/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p41.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p41.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p42.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p42.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p43.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p43.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p44.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p44.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p45.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p45.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p46.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p46.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p47.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p47.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p48.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p48.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p49.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p49.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p50.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p50.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p51.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p51.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p52.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p52.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p53.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p53.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p54.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p54.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p55.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p55.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p56.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p56.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p57.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p57.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p58.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p58.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p59.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p59.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p60.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p60.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p61.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p61.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p62.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p62.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p63.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p63.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p64.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p64.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p65.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p65.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p66.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p66.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p67.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p67.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p68.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p68.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p69.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p69.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p70.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p70.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p71.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p71.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p72.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p72.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p73.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p73.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p74.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p74.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/tireworld-truck/p75.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/tireworld-truck/p75.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p16.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p16.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p17.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p17.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p18.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p18.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p19.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p19.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p20.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p20.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p21.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p21.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p22.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p22.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p23.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p23.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p24.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p24.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p25.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p25.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p26.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p26.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p27.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p27.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p28.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p28.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p29.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p29.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p30.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p30.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p31.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p31.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p32.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p32.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p33.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p33.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p34.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p34.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p35.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p35.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p36.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p36.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p37.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p37.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p38.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p38.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p39.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p39.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/triangle-tireworld/p40.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/triangle-tireworld/p40.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/domain.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/domain.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p01.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p01.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p02.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p02.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p03.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p03.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p04.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p04.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p05.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p05.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p06.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p06.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p07.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p07.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p08.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p08.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p09.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p09.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p10.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p10.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p11.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p11.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p12.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p12.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p13.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p13.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p14.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p14.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/fixtures/pddl_files/zenotravel/p15.pddl` & `pddl-0.3.1/tests/fixtures/pddl_files/zenotravel/p15.pddl`

 * *Files identical despite different names*

### Comparing `pddl-0.2.0/tests/test_action.py` & `pddl-0.3.1/tests/test_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_actions.py` & `pddl-0.3.1/tests/test_actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_cli.py` & `pddl-0.3.1/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_docs/base.py` & `pddl-0.3.1/tests/test_docs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
@@ -19,15 +18,15 @@
 
 import mistune
 import pytest
 
 MISTUNE_BLOCK_CODE_ID = "block_code"
 
 
-def compile_and_exec(code: str, locals_dict: Dict = None) -> Dict:
+def compile_and_exec(code: str, locals_dict: Optional[Dict] = None) -> Dict:
     """
     Compile and exec the code.
 
     :param code: the code to execute.
     :param locals_dict: the dictionary of local variables.
     :return: the dictionary of locals.
     """
```

### Comparing `pddl-0.2.0/tests/test_docs/test_readme.py` & `pddl-0.3.1/tests/test_docs/test_readme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_domain.py` & `pddl-0.3.1/tests/test_domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_helpers/test_cache_hash.py` & `pddl-0.3.1/tests/test_helpers/test_cache_hash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 #
 
 """Test the cache hash class decorator."""
-import pickle
+import pickle  # nosec
 
 from pddl.helpers.cache_hash import cache_hash
 
 
 @cache_hash
 class MyHashable:
     """A test class to test 'Hashable' metaclass."""
@@ -41,10 +40,10 @@
     h1 = hash(obj)
     h2 = hash(obj)
     assert h1 == h2
 
     assert hasattr(obj, "__hash")
     assert obj.__hash == h1 == h2
 
-    dumped_obj = pickle.dumps(obj)
-    actual_obj = pickle.loads(dumped_obj)
+    dumped_obj = pickle.dumps(obj)  # nosec
+    actual_obj = pickle.loads(dumped_obj)  # nosec
     assert not hasattr(actual_obj, "__hash")
```

### Comparing `pddl-0.2.0/tests/test_parser.py` & `pddl-0.3.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_predicate.py` & `pddl-0.3.1/tests/test_predicate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 #
 
 """This module contains tests for PDDL predicates."""
 from pddl.core import Predicate
 from pddl.logic.helpers import variables
+from pddl.logic.predicates import EqualTo
 
 
 class TestPredicateSimpleInitialisation:
     """Test simple predicate initialisation."""
 
-    def setup(self):
+    def setup_method(self):
         """Set up the tests."""
         self.a, self.b = variables("a b")
         self.predicate = Predicate("P", self.a, self.b)
 
     def test_name(self):
         """Test name getter."""
         assert self.predicate.name == "P"
@@ -31,7 +31,37 @@
     def test_variables(self):
         """Test terms getter."""
         assert self.predicate.terms == (self.a, self.b)
 
     def test_arity(self):
         """Test arity property."""
         assert self.predicate.arity == 2
+
+
+class TestEqualToPredicate:
+    """Test the eaual to predicate."""
+
+    def setup_method(self):
+        """Set up the tests."""
+        self.left, self.right = variables("l r")
+        self.equal_to = EqualTo(self.left, self.right)
+
+    def test_left(self):
+        """Test left getter."""
+        assert self.equal_to.left == self.left
+
+    def test_right(self):
+        """Test right getter."""
+        assert self.equal_to.right == self.right
+
+    def test_to_equal(self):
+        """Test to equal."""
+        other = EqualTo(self.left, self.right)
+        assert self.equal_to == other
+
+    def test_to_str(self):
+        """Test to string."""
+        assert str(self.equal_to) == f"(= {str(self.left)} {str(self.right)})"
+
+    def test_to_repr(self):
+        """Test to repr."""
+        assert repr(self.equal_to) == f"EqualTo({repr(self.left)}, {repr(self.right)})"
```

### Comparing `pddl-0.2.0/tests/test_problem.py` & `pddl-0.3.1/tests/test_problem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

### Comparing `pddl-0.2.0/tests/test_types.py` & `pddl-0.3.1/tests/test_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 WhiteMech
+# Copyright 2021-2023 WhiteMech
 #
 # ------------------------------
 #
 # This file is part of pddl.
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
```

