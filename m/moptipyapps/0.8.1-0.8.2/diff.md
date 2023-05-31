# Comparing `tmp/moptipyapps-0.8.1.tar.gz` & `tmp/moptipyapps-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moptipyapps-0.8.1.tar", last modified: Sat May 27 09:03:38 2023, max compression
+gzip compressed data, was "moptipyapps-0.8.2.tar", last modified: Wed May 31 04:04:22 2023, max compression
```

## Comparing `moptipyapps-0.8.1.tar` & `moptipyapps-0.8.2.tar`

### file list

```diff
@@ -1,34 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.138771 moptipyapps-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-05-27 09:03:38.138771 moptipyapps-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.134771 moptipyapps-0.8.1/moptipyapps/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.134771 moptipyapps-0.8.1/moptipyapps/binpacking2d/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/bin_count_and_last_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    18957 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/ibl_encoding_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/ibl_encoding_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/make_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/packing_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/binpacking2d/plot_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.138771 moptipyapps-0.8.1/moptipyapps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/tests/on_binpacking2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/moptipyapps/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.134771 moptipyapps-0.8.1/moptipyapps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-05-27 09:03:38.000000 moptipyapps-0.8.1/moptipyapps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-27 09:03:38.000000 moptipyapps-0.8.1/moptipyapps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:38.000000 moptipyapps-0.8.1/moptipyapps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:37.000000 moptipyapps-0.8.1/moptipyapps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-27 09:03:38.000000 moptipyapps-0.8.1/moptipyapps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-27 09:03:38.000000 moptipyapps-0.8.1/moptipyapps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-27 09:03:38.138771 moptipyapps-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:38.138771 moptipyapps-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/tests/test_examples_in_examples_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-05-27 08:58:11.000000 moptipyapps-0.8.1/tests/test_links_in_documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.488881 moptipyapps-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-05-31 04:04:22.488881 moptipyapps-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.460881 moptipyapps-0.8.2/moptipyapps/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.460881 moptipyapps-0.8.2/moptipyapps/binpacking2d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   191757 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/2dpacklib.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/bin_count_and_last_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/ibl_encoding_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22954 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/ibl_encoding_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/make_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/packing_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/binpacking2d/plot_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.460881 moptipyapps-0.8.2/moptipyapps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tests/on_binpacking2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.464881 moptipyapps-0.8.2/moptipyapps/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/known_optima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tour_length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.488881 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/a280.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/a280.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ali535.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/att48.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/att48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/att532.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/bayg29.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/bayg29.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/bays29.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/bays29.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/berlin52.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/berlin52.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/bier127.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/br17.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/brazil58.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/brg180.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    98436 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/brg180.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/burma14.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ch130.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ch130.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ch150.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ch150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/d1291.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    47015 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/d1655.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/d198.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/d493.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/d657.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/dantzig42.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil101.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil101.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil51.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil51.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil76.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/eil76.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/fl1400.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    44754 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/fl1577.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/fl417.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/fri26.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/fri26.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ft53.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ft70.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   360799 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv170.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv33.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv35.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv38.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv44.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv47.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    38312 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv55.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    51562 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv64.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    60649 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ftv70.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gil262.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr120.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    30909 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr120.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr137.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr17.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr202.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr202.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr21.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr229.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr24.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr24.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr431.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr48.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr666.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr666.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr96.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/gr96.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/hk48.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    81561 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kro124p.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroA100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroA100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroA150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroA200.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroB100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroB150.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroB200.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroC100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroC100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroD100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroD100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/kroE100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/lin105.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/lin105.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/lin318.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/nrw1379.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/p43.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/p654.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    33047 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pcb1173.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pcb442.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pcb442.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr1002.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr1002.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr107.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr124.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr136.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr144.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr152.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr226.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr264.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr299.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr439.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr76.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/pr76.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rat195.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rat575.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rat783.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rat99.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)   423944 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rbg323.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   520701 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rbg358.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   659477 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rbg403.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)   797126 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rbg443.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rd100.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rd100.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rd400.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rl1304.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    37385 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rl1323.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    53799 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/rl1889.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ry48p.atsp
+-rw-r--r--   0 runner    (1001) docker     (123)  2162350 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/si1032.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    62351 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/si175.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)   579782 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/si535.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/st70.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/st70.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/swiss42.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ts225.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/tsp225.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/tsp225.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    29768 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u1060.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    40548 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u1432.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u159.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    51713 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u1817.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u574.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/u724.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ulysses16.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ulysses16.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ulysses22.opt.tour
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/ulysses22.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/vm1084.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)    49714 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/tsp/tsplib/vm1748.tsp
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/moptipyapps/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.460881 moptipyapps-0.8.2/moptipyapps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 04:04:22.000000 moptipyapps-0.8.2/moptipyapps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-31 04:04:22.488881 moptipyapps-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:04:22.488881 moptipyapps-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/tests/test_examples_in_examples_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-05-31 03:56:49.000000 moptipyapps-0.8.2/tests/test_links_in_documentation.py
```

### Comparing `moptipyapps-0.8.1/PKG-INFO` & `moptipyapps-0.8.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moptipyapps
-Version: 0.8.1
+Version: 0.8.2
 Summary: Applications of Metaheuristic Optimization in Python.
 Home-page: https://thomasweise.github.io/moptipy
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -40,14 +40,15 @@
 
 # moptipyapps: Applications of Metaheuristic Optimization in Python
 
 - [Introduction](https://thomasweise.github.io/moptipyapps/index.html#introduction)
 - [Installation](https://thomasweise.github.io/moptipyapps/index.html#installation)
 - [Applications](https://thomasweise.github.io/moptipyapps/index.html#applications)
   - [Two-Dimensional Bin Packing Problem](https://thomasweise.github.io/moptipyapps/index.html#two-dimensional-bin-packing-problem)
+  - [Traveling Salesperson Problem (TSP)](https://thomasweise.github.io/moptipyapps/index.html#the-traveling-salesperson-problem-tsp)
 - [Unit Tests and Static Analysis](https://thomasweise.github.io/moptipyapps/index.html#unit-tests-and-static-analysis)
 - [License](https://thomasweise.github.io/moptipyapps/index.html#license)
 - [Contact](https://thomasweise.github.io/moptipyapps/index.html#contact)
 
 
 ## 1. Introduction
 
@@ -87,19 +88,20 @@
 
 All dependencies for using and running `moptipyapps` are listed at [here](https://thomasweise.github.io/moptipyapps/requirements.html).
 The additional dependencies for a [full `make` build](https://thomasweise.github.io/moptipyapps/Makefile.html), including unit tests, static analysis, and the generation of documentation are listed [here](https://thomasweise.github.io/moptipyapps/requirements-dev.html).
 
 
 ## 3. Applications
 
-Here we list the applications.
+Here we list the applications of [`moptipy`](https://thomasweise.github.io/moptipy).
 
 
 ### 3.1. Two-Dimensional Bin Packing Problem
 
+In the package [`moptipyapps.binpacking2d`](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d), we provide tools for experimenting and playing around with the two-dimensional bin packing problem.
 Bin packing is a classical domain from Operations Research.
 The goal is to pack objects into containers, the so-called bins.
 We address [two-dimensional rectangular bin packing](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 We provide the bin packing [instances](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.instance) from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) as [resources](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#moptipyapps.binpacking2d.instance.Instance.from_resource) together with [this package](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 Each such instances defines a set of `n_different_items` objects `Oi` with `i` from `1..n_different_objects`.
 Each object `Oi` is a rectangle with a given width and height.
 The object occur is a given multiplicity `repetitions(O_i)`, i.e., either only once or multiple times.
@@ -114,15 +116,44 @@
 [The first one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_1) closes bins as soon as one object cannot be placed into them.
 [The second one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_2) tries to put each object in the earliest possible bin.
 While the former one is faster, the latter one leads to better packings.
 
 We can then apply a black-box metaheuristic to search in the space of these signed permutations with repetitions.
 The objective function would be some measure consistent with the goal of minimizing the number of bins used.
 
-The encodings were originally implemented by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student of the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+*Examples:*
+
+- [plot a packing chart](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_plot.html)
+- [apply a randomized local search to one 2D bin packing instance](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_rls.html)
+- [measure the runtime of the different encodings for the 2D bin packing problem](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_timing.html)
+
+Important work on this code has been contributed by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+
+
+### 3.2. The Traveling Salesperson Problem (TSP)
+
+In the package [`moptipyapps.tsp`](https://thomasweise.github.io/moptipyapps/moptipyapps.tsp.html#module-moptipyapps.tsp), we provide tools to run experiments and play around with the Traveling Salesperson Problem (TSP) .
+A TSP instance is defined as a fully-connected graph with `n_cities` nodes.
+Each edge in  the graph has a weight, which identifies the distance between the nodes.
+The goal is to find the *shortest* tour that visits every single node in the graph exactly once and then returns back to its starting node.
+Then nodes are usually called cities.
+A tour can be represented in path representation, which means that it is stored as a permutation of the numbers `0` to `n_cities-1`.
+The number at index `k` identifies that `k`-th city to visit.
+So the first number in the permutation identifies the first city, the second number the second city,
+and so on.
+The length of the tour can be computed by summing up the distances from the `k`-th city to the `k+1`-st city, for `k` in `0..n_cities-2` and then adding the distance from the last city to the first city.
+
+We use the TSP instances from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/), the maybe most important benchmark set for the TSP.
+110 of these instances are included as resources in this package.
+
+*Examples:*
+
+- [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
+
+Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
@@ -197,15 +228,15 @@
 
 
 ## 5. License
 
 [`moptipyapps`](https://thomasweise.github.io/moptipyapps) is a library for implementing, using, and experimenting with metaheuristic optimization algorithms.
 Our project is developed for scientific, educational, and industrial applications.
 
-Copyright (C) 2021-2022  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
+Copyright (C) 2023  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
 
 Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/moptipyapps/index.html#contact)) holds the copyright of this package *except* for the data of the benchmark sets we imported from other sources.
 `moptipyapps` is provided to the public as open source software under the [GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007](https://thomasweise.github.io/moptipyapps/LICENSE.html).
 Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/moptipyapps/index.html#contact) below).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
@@ -217,14 +248,16 @@
 
 
 ### 5.1. Exceptions
 
 - The included benchmark instance data of the [two-dimensional bin packing](https://thomasweise.github.io/moptipyapps/index.html#two-dimensional-bin-packing-problem) is taken from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib).
   It has been stored in a more size-efficient way and some unnecessary information has been stripped from it (as we really only need the raw bin packing data).
   Nevertheless, the copyright of the original data lies with the authors [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) or the original authors of the datasets used by them.
+- The included benchmark instances for the [Traveling Salesperson Problem](https://thomasweise.github.io/moptipyapps/index.html#the-traveling-salesperson-problem-tsp) are taken from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/).
+  The copyright of the original data lies with Gerhard Reinelt, the original author of TSPLib, or the original authors of the datasets used by him.
 
 
 ## 6. Contact
 
 If you have any questions or suggestions, please contact
 Prof. Dr. [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授) of the
 Institute of Applied Optimization (应用优化研究所, [IAO](http://iao.hfuu.edu.cn)) of the
```

### Comparing `moptipyapps-0.8.1/README.md` & `moptipyapps-0.8.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # moptipyapps: Applications of Metaheuristic Optimization in Python
 
 - [Introduction](#1-introduction)
 - [Installation](#2-installation)
 - [Applications](#3-applications)
   - [Two-Dimensional Bin Packing Problem](#31-two-dimensional-bin-packing-problem)
+  - [Traveling Salesperson Problem (TSP)](#32-the-traveling-salesperson-problem-tsp)
 - [Unit Tests and Static Analysis](#4-unit-tests-and-static-analysis)
 - [License](#5-license)
 - [Contact](#6-contact)
 
 
 ## 1. Introduction
 
@@ -53,19 +54,20 @@
 
 All dependencies for using and running `moptipyapps` are listed at [here](https://thomasweise.github.io/moptipyapps/requirements.html).
 The additional dependencies for a [full `make` build](https://thomasweise.github.io/moptipyapps/Makefile.html), including unit tests, static analysis, and the generation of documentation are listed [here](https://thomasweise.github.io/moptipyapps/requirements-dev.html).
 
 
 ## 3. Applications
 
-Here we list the applications.
+Here we list the applications of [`moptipy`](https://thomasweise.github.io/moptipy).
 
 
 ### 3.1. Two-Dimensional Bin Packing Problem
 
+In the package [`moptipyapps.binpacking2d`](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d), we provide tools for experimenting and playing around with the two-dimensional bin packing problem.
 Bin packing is a classical domain from Operations Research.
 The goal is to pack objects into containers, the so-called bins.
 We address [two-dimensional rectangular bin packing](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 We provide the bin packing [instances](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.instance) from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) as [resources](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#moptipyapps.binpacking2d.instance.Instance.from_resource) together with [this package](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 Each such instances defines a set of `n_different_items` objects `Oi` with `i` from `1..n_different_objects`.
 Each object `Oi` is a rectangle with a given width and height.
 The object occur is a given multiplicity `repetitions(O_i)`, i.e., either only once or multiple times.
@@ -80,15 +82,44 @@
 [The first one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_1) closes bins as soon as one object cannot be placed into them.
 [The second one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_2) tries to put each object in the earliest possible bin.
 While the former one is faster, the latter one leads to better packings.
 
 We can then apply a black-box metaheuristic to search in the space of these signed permutations with repetitions.
 The objective function would be some measure consistent with the goal of minimizing the number of bins used.
 
-The encodings were originally implemented by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student of the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+*Examples:*
+
+- [plot a packing chart](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_plot.html)
+- [apply a randomized local search to one 2D bin packing instance](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_rls.html)
+- [measure the runtime of the different encodings for the 2D bin packing problem](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_timing.html)
+
+Important work on this code has been contributed by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+
+
+### 3.2. The Traveling Salesperson Problem (TSP)
+
+In the package [`moptipyapps.tsp`](https://thomasweise.github.io/moptipyapps/moptipyapps.tsp.html#module-moptipyapps.tsp), we provide tools to run experiments and play around with the Traveling Salesperson Problem (TSP) .
+A TSP instance is defined as a fully-connected graph with `n_cities` nodes.
+Each edge in  the graph has a weight, which identifies the distance between the nodes.
+The goal is to find the *shortest* tour that visits every single node in the graph exactly once and then returns back to its starting node.
+Then nodes are usually called cities.
+A tour can be represented in path representation, which means that it is stored as a permutation of the numbers `0` to `n_cities-1`.
+The number at index `k` identifies that `k`-th city to visit.
+So the first number in the permutation identifies the first city, the second number the second city,
+and so on.
+The length of the tour can be computed by summing up the distances from the `k`-th city to the `k+1`-st city, for `k` in `0..n_cities-2` and then adding the distance from the last city to the first city.
+
+We use the TSP instances from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/), the maybe most important benchmark set for the TSP.
+110 of these instances are included as resources in this package.
+
+*Examples:*
+
+- [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
+
+Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
@@ -163,15 +194,15 @@
 
 
 ## 5. License
 
 [`moptipyapps`](https://thomasweise.github.io/moptipyapps) is a library for implementing, using, and experimenting with metaheuristic optimization algorithms.
 Our project is developed for scientific, educational, and industrial applications.
 
-Copyright (C) 2021-2022  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
+Copyright (C) 2023  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
 
 Dr. Thomas Weise (see [Contact](#6-contact)) holds the copyright of this package *except* for the data of the benchmark sets we imported from other sources.
 `moptipyapps` is provided to the public as open source software under the [GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007](https://thomasweise.github.io/moptipyapps/LICENSE.html).
 Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](#6-contact) below).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
@@ -183,14 +214,16 @@
 
 
 ### 5.1. Exceptions
 
 - The included benchmark instance data of the [two-dimensional bin packing](#31-two-dimensional-bin-packing-problem) is taken from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib).
   It has been stored in a more size-efficient way and some unnecessary information has been stripped from it (as we really only need the raw bin packing data).
   Nevertheless, the copyright of the original data lies with the authors [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) or the original authors of the datasets used by them.
+- The included benchmark instances for the [Traveling Salesperson Problem](#32-the-traveling-salesperson-problem-tsp) are taken from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/).
+  The copyright of the original data lies with Gerhard Reinelt, the original author of TSPLib, or the original authors of the datasets used by him.
 
 
 ## 6. Contact
 
 If you have any questions or suggestions, please contact
 Prof. Dr. [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授) of the 
 Institute of Applied Optimization (应用优化研究所, [IAO](http://iao.hfuu.edu.cn)) of the
```

### Comparing `moptipyapps-0.8.1/moptipyapps/__init__.py` & `moptipyapps-0.8.2/moptipyapps/__init__.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/__init__.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,8 +25,15 @@
 - :mod:`~moptipyapps.binpacking2d.bin_count_and_last_empty` provides an
   objective function that tries to minimize the number of bins and pushes
   towards decreasing the number of objects in the very last bin used.
 - :mod:`~moptipyapps.binpacking2d.make_instances` offers a method to download
   the two-dimensional bin packing instances from the original sources in the \
 [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib)
   format.
+
+Important initial work on this code has been contributed by Mr. Rui ZHAO
+(赵睿), <zr1329142665@163.com> a Master's student at the Institute of Applied
+Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of
+Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University
+(合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of
+Prof. Dr. Thomas Weise (汤卫思教授).
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/bin_count_and_last_empty.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/bin_count_and_last_empty.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/ibl_encoding_1.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/ibl_encoding_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
 This is different from the second variant of this encoding implemented in file
 :mod:`moptipyapps.binpacking2d.ibl_encoding_2`, which always checks
 all the bins, starting at bin `1`, when placing any object. That other
 encoding variant therefore must always consider all bins and is thus slower,
 but tends to yield better packings.
 
-This procedure has originally been developed an implemented by Mr. Rui ZHAO
-(赵睿), <zr1329142665@163.com> a Master's student of the Institute of Applied
+This procedure has originally been developed and implemented by Mr. Rui ZHAO
+(赵睿), <zr1329142665@163.com> a Master's student at the Institute of Applied
 Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of
 Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University
 (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of
 Prof. Dr. Thomas Weise (汤卫思教授).
 
 1. Dequan Liu and Hongfei Teng. An Improved BL-Algorithm for Genetic Algorithm
    of the Orthogonal Packing of Rectangles. European Journal of Operational
```

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/ibl_encoding_2.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/ibl_encoding_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 put in there. Now within these two indices, there also might be objects that
 we placed into other bins. But for a very little overhead (remembering two
 values per bin), we have a certain chance to speed up the process in several
 situations. For instance, the worst case from above, that each object occupies
 exactly one bin by itself becomes easier because we would only look at one
 already placed object per bin.
 
-This procedure has originally been developed an implemented by Mr. Rui ZHAO
-(赵睿), <zr1329142665@163.com>, a Master's student of the Institute of Applied
+This procedure has originally been developed and implemented by Mr. Rui ZHAO
+(赵睿), <zr1329142665@163.com>, a Master's student at the Institute of Applied
 Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of
 Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University
 (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of
 Prof. Dr. Thomas Weise (汤卫思教授).
 
 1. Dequan Liu and Hongfei Teng. An Improved BL-Algorithm for Genetic Algorithm
    of the Orthogonal Packing of Rectangles. European Journal of Operational
```

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/instance.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 (via :meth:`Instance.to_compact_str`). This library ships with a set of
 pre-defined instances as resource which can be obtained via
 :meth:`Instance.from_resource` and listed via
 :meth:`Instance.list_resources`.
 
 We provide the instances of the sets `A` [3], `BENG` [4], and `CLASS` [5].
 
+Initial work on this code has been contributed by Mr. Rui ZHAO (赵睿),
+<zr1329142665@163.com> a Master's student at the Institute of Applied
+Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of
+Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University
+(合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of
+Prof. Dr. Thomas Weise (汤卫思教授).
+
 1. Manuel Iori, Vinícius Loti de Lima, Silvano Martello, and Michele Monaci.
    *2DPackLib*.
    https://site.unibo.it/operations-research/en/research/2dpacklib
 2. Manuel Iori, Vinícius Loti de Lima, Silvano Martello, and Michele
    Monaci. 2DPackLib: A Two-Dimensional Cutting and Packing Library.
    *Optimization Letters* 16(2):471-480. March 2022.
    https://doi.org/10.1007/s11590-021-01808-y
@@ -326,19 +333,20 @@
         for i in range(n_different_items):
             obj[i, :] = matrix[i]
 
         #: the name of the instance
         obj.name = use_name
         #: the number of different items
         obj.n_different_items = n_different_items
-        #: the number of jobs == self.shape[0]
+        #: the total number of items, i.e., the number of different items
+        #: multiplied with their repetition counts
         obj.n_items = n_items
-        #: the number of machines == self.shape[1]
+        #: the height of the bins
         obj.bin_height = bin_height
-        #: the lower bound of the makespan of this JSSP instance
+        #: the width of the bins
         obj.bin_width = bin_width
 
 # We need as least as many bins such that their area is big enough
 # for the total area of the items.
         bin_area: int = bin_height * bin_width
         min_size: int = item_area // bin_area
         if (min_size * bin_area) < item_area:
@@ -509,17 +517,17 @@
         logger.key_value(BIN_WIDTH, self.bin_width)
         logger.key_value(BIN_HEIGHT, self.bin_height)
         logger.key_value(npu.KEY_NUMPY_TYPE, self.dtype.char)
 
     @staticmethod
     def list_resources() -> tuple[str, ...]:
         """
-        Get an iterable of all the instances available as resource.
+        Get a tuple of all the instances available as resource.
 
-        :return: the iterable with the instance names
+        :return: the tuple with the instance names
 
         >>> len(list(Instance.list_resources()))
         553
         """
         return _INSTANCES
 
     @staticmethod
```

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/make_instances.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/make_instances.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/packing.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/packing.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/packing_space.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/packing_space.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/binpacking2d/plot_packing.py` & `moptipyapps-0.8.2/moptipyapps/binpacking2d/plot_packing.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps/tests/on_binpacking2d.py` & `moptipyapps-0.8.2/moptipyapps/tests/on_binpacking2d.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/moptipyapps.egg-info/PKG-INFO` & `moptipyapps-0.8.2/moptipyapps.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moptipyapps
-Version: 0.8.1
+Version: 0.8.2
 Summary: Applications of Metaheuristic Optimization in Python.
 Home-page: https://thomasweise.github.io/moptipy
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -40,14 +40,15 @@
 
 # moptipyapps: Applications of Metaheuristic Optimization in Python
 
 - [Introduction](https://thomasweise.github.io/moptipyapps/index.html#introduction)
 - [Installation](https://thomasweise.github.io/moptipyapps/index.html#installation)
 - [Applications](https://thomasweise.github.io/moptipyapps/index.html#applications)
   - [Two-Dimensional Bin Packing Problem](https://thomasweise.github.io/moptipyapps/index.html#two-dimensional-bin-packing-problem)
+  - [Traveling Salesperson Problem (TSP)](https://thomasweise.github.io/moptipyapps/index.html#the-traveling-salesperson-problem-tsp)
 - [Unit Tests and Static Analysis](https://thomasweise.github.io/moptipyapps/index.html#unit-tests-and-static-analysis)
 - [License](https://thomasweise.github.io/moptipyapps/index.html#license)
 - [Contact](https://thomasweise.github.io/moptipyapps/index.html#contact)
 
 
 ## 1. Introduction
 
@@ -87,19 +88,20 @@
 
 All dependencies for using and running `moptipyapps` are listed at [here](https://thomasweise.github.io/moptipyapps/requirements.html).
 The additional dependencies for a [full `make` build](https://thomasweise.github.io/moptipyapps/Makefile.html), including unit tests, static analysis, and the generation of documentation are listed [here](https://thomasweise.github.io/moptipyapps/requirements-dev.html).
 
 
 ## 3. Applications
 
-Here we list the applications.
+Here we list the applications of [`moptipy`](https://thomasweise.github.io/moptipy).
 
 
 ### 3.1. Two-Dimensional Bin Packing Problem
 
+In the package [`moptipyapps.binpacking2d`](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d), we provide tools for experimenting and playing around with the two-dimensional bin packing problem.
 Bin packing is a classical domain from Operations Research.
 The goal is to pack objects into containers, the so-called bins.
 We address [two-dimensional rectangular bin packing](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 We provide the bin packing [instances](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.instance) from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) as [resources](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#moptipyapps.binpacking2d.instance.Instance.from_resource) together with [this package](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d).
 Each such instances defines a set of `n_different_items` objects `Oi` with `i` from `1..n_different_objects`.
 Each object `Oi` is a rectangle with a given width and height.
 The object occur is a given multiplicity `repetitions(O_i)`, i.e., either only once or multiple times.
@@ -114,15 +116,44 @@
 [The first one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_1) closes bins as soon as one object cannot be placed into them.
 [The second one](https://thomasweise.github.io/moptipyapps/moptipyapps.binpacking2d.html#module-moptipyapps.binpacking2d.ibl_encoding_2) tries to put each object in the earliest possible bin.
 While the former one is faster, the latter one leads to better packings.
 
 We can then apply a black-box metaheuristic to search in the space of these signed permutations with repetitions.
 The objective function would be some measure consistent with the goal of minimizing the number of bins used.
 
-The encodings were originally implemented by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student of the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+*Examples:*
+
+- [plot a packing chart](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_plot.html)
+- [apply a randomized local search to one 2D bin packing instance](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_rls.html)
+- [measure the runtime of the different encodings for the 2D bin packing problem](https://thomasweise.github.io/moptipyapps/examples/binpacking2d_timing.html)
+
+Important work on this code has been contributed by Mr. Rui ZHAO (赵睿), <zr1329142665@163.com>, a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授), who then refined the implementations.
+
+
+### 3.2. The Traveling Salesperson Problem (TSP)
+
+In the package [`moptipyapps.tsp`](https://thomasweise.github.io/moptipyapps/moptipyapps.tsp.html#module-moptipyapps.tsp), we provide tools to run experiments and play around with the Traveling Salesperson Problem (TSP) .
+A TSP instance is defined as a fully-connected graph with `n_cities` nodes.
+Each edge in  the graph has a weight, which identifies the distance between the nodes.
+The goal is to find the *shortest* tour that visits every single node in the graph exactly once and then returns back to its starting node.
+Then nodes are usually called cities.
+A tour can be represented in path representation, which means that it is stored as a permutation of the numbers `0` to `n_cities-1`.
+The number at index `k` identifies that `k`-th city to visit.
+So the first number in the permutation identifies the first city, the second number the second city,
+and so on.
+The length of the tour can be computed by summing up the distances from the `k`-th city to the `k+1`-st city, for `k` in `0..n_cities-2` and then adding the distance from the last city to the first city.
+
+We use the TSP instances from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/), the maybe most important benchmark set for the TSP.
+110 of these instances are included as resources in this package.
+
+*Examples:*
+
+- [apply a randomized local search to one TSP instance](https://thomasweise.github.io/moptipyapps/examples/tsp_rls.html)
+
+Important work on this code has been contributed by Mr. Tianyu LIANG (梁天宇), <liangty@stu.hfuu.edu.cn> a Master's student at the Institute of Applied Optimization (应用优化研究所, http://iao.hfuu.edu.cn) of the School of Artificial Intelligence and Big Data (人工智能与大数据学院) at Hefei  University (合肥学院) in Hefei, Anhui, China (中国安徽省合肥市) under the supervision of Prof. Dr. Thomas Weise (汤卫思教授).
 
 
 ## 4. Unit Tests and Static Analysis
 
 When developing and applying randomized algorithms, proper testing and checking of the source code is of utmost importance.
 If we apply a randomized metaheuristic to an optimization problem, then we usually do not which solution quality we can achieve.
 Therefore, we can usually not know whether we have implemented the algorithm correctly.
@@ -197,15 +228,15 @@
 
 
 ## 5. License
 
 [`moptipyapps`](https://thomasweise.github.io/moptipyapps) is a library for implementing, using, and experimenting with metaheuristic optimization algorithms.
 Our project is developed for scientific, educational, and industrial applications.
 
-Copyright (C) 2021-2022  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
+Copyright (C) 2023  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
 
 Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/moptipyapps/index.html#contact)) holds the copyright of this package *except* for the data of the benchmark sets we imported from other sources.
 `moptipyapps` is provided to the public as open source software under the [GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007](https://thomasweise.github.io/moptipyapps/LICENSE.html).
 Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/moptipyapps/index.html#contact) below).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
@@ -217,14 +248,16 @@
 
 
 ### 5.1. Exceptions
 
 - The included benchmark instance data of the [two-dimensional bin packing](https://thomasweise.github.io/moptipyapps/index.html#two-dimensional-bin-packing-problem) is taken from [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib).
   It has been stored in a more size-efficient way and some unnecessary information has been stripped from it (as we really only need the raw bin packing data).
   Nevertheless, the copyright of the original data lies with the authors [2DPackLib](https://site.unibo.it/operations-research/en/research/2dpacklib) or the original authors of the datasets used by them.
+- The included benchmark instances for the [Traveling Salesperson Problem](https://thomasweise.github.io/moptipyapps/index.html#the-traveling-salesperson-problem-tsp) are taken from [TSPLib](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/).
+  The copyright of the original data lies with Gerhard Reinelt, the original author of TSPLib, or the original authors of the datasets used by him.
 
 
 ## 6. Contact
 
 If you have any questions or suggestions, please contact
 Prof. Dr. [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授) of the
 Institute of Applied Optimization (应用优化研究所, [IAO](http://iao.hfuu.edu.cn)) of the
```

### Comparing `moptipyapps-0.8.1/setup.cfg` & `moptipyapps-0.8.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 	urllib3 >= 1.26.16
 packages = find:
 python_requires = >= 3.10
 zip_safe = False
 
 [options.package_data]
 moptipyapps = py.typed
-moptipyapps.problems.binpacking2d = *.txt
+moptipyapps.binpacking2d = *.txt
+moptipyapps.tsp.tsplib = *.tsp, *.atsp, *.opt.tour
 
 [options.packages.find]
 exclude = 
 	.coverage*
 	.github*
 	.mypy_cache*
 	.pytest_cache*
```

### Comparing `moptipyapps-0.8.1/setup.py` & `moptipyapps-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/tests/test_examples_in_examples_directory.py` & `moptipyapps-0.8.2/tests/test_examples_in_examples_directory.py`

 * *Files identical despite different names*

### Comparing `moptipyapps-0.8.1/tests/test_links_in_documentation.py` & `moptipyapps-0.8.2/tests/test_links_in_documentation.py`

 * *Files identical despite different names*

