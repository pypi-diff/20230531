# Comparing `tmp/podman-4.5.0.tar.gz` & `tmp/podman-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podman-4.5.0.tar", last modified: Thu Apr 27 14:43:27 2023, max compression
+gzip compressed data, was "podman-4.5.1.tar", last modified: Wed May 31 15:45:46 2023, max compression
```

## Comparing `podman-4.5.0.tar` & `podman-4.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.561593 podman-4.5.0/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.5.0/LICENSE
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-04-27 14:43:27.561593 podman-4.5.0/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.5.0/README.md
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.557593 podman-4.5.0/podman/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.5.0/podman/__init__.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.558593 podman-4.5.0/podman/api/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/adapter_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/cached_property.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/client.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/http_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3270 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/parse_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9974 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/ssh.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/tar_utils.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109033 2023-04-27 13:32:41.000000 podman-4.5.0/podman/api/typing_extensions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5976 2022-10-19 21:26:36.000000 podman-4.5.0/podman/api/uds.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8640 2023-04-27 13:32:41.000000 podman-4.5.0/podman/client.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.560593 podman-4.5.0/podman/domain/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3720 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/config.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    18880 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/containers.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    31505 2023-04-27 13:32:41.000000 podman-4.5.0/podman/domain/containers_create.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5405 2023-02-07 13:10:19.000000 podman-4.5.0/podman/domain/containers_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-02-07 13:10:19.000000 podman-4.5.0/podman/domain/containers_run.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/events.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/images.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/images_build.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14363 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/images_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/ipam.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/manifests.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/networks.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6920 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/networks_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/pods.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5465 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/pods_manager.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/registry_data.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/secrets.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.5.0/podman/domain/system.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-02-09 13:04:40.000000 podman-4.5.0/podman/domain/volumes.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.560593 podman-4.5.0/podman/errors/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.5.0/podman/errors/__init__.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.5.0/podman/errors/exceptions.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.5.0/podman/tlsconfig.py
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-04-27 13:33:53.000000 podman-4.5.0/podman/version.py
-drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-04-27 14:43:27.557593 podman-4.5.0/podman.egg-info/
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/PKG-INFO
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/SOURCES.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/dependency_links.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)       84 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/requires.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-04-27 14:43:27.000000 podman-4.5.0/podman.egg-info/top_level.txt
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      662 2023-04-27 13:32:41.000000 podman-4.5.0/pyproject.toml
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1313 2023-04-27 14:43:27.561593 podman-4.5.0/setup.cfg
--rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.5.0/setup.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.201281 podman-4.5.1/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    11357 2022-10-19 21:26:36.000000 podman-4.5.1/LICENSE
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-05-31 15:45:46.201281 podman-4.5.1/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1745 2022-10-19 21:26:36.000000 podman-4.5.1/README.md
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.194281 podman-4.5.1/podman/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      277 2022-10-19 21:26:36.000000 podman-4.5.1/podman/__init__.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.197281 podman-4.5.1/podman/api/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1980 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/adapter_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      256 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/cached_property.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14670 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/client.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2918 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/http_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3270 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/parse_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     9974 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/ssh.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3845 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/tar_utils.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)   109033 2023-04-27 13:32:41.000000 podman-4.5.1/podman/api/typing_extensions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5976 2022-10-19 21:26:36.000000 podman-4.5.1/podman/api/uds.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8640 2023-04-27 13:32:41.000000 podman-4.5.1/podman/client.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.200281 podman-4.5.1/podman/domain/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        0 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3720 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/config.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    18880 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/containers.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    31505 2023-04-27 13:32:41.000000 podman-4.5.1/podman/domain/containers_create.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5405 2023-02-07 13:10:19.000000 podman-4.5.1/podman/domain/containers_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3305 2023-02-07 13:10:19.000000 podman-4.5.1/podman/domain/containers_run.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1724 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/events.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3699 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/images.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     8616 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/images_build.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)    14363 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/images_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1697 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/ipam.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3968 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     7485 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/manifests.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4882 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/networks.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     6920 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/networks_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     3451 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/pods.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     5465 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/pods_manager.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2936 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/registry_data.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4026 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/secrets.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2931 2022-10-19 21:26:36.000000 podman-4.5.1/podman/domain/system.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4969 2023-02-09 13:04:40.000000 podman-4.5.1/podman/domain/volumes.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.200281 podman-4.5.1/podman/errors/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2710 2022-10-19 21:26:36.000000 podman-4.5.1/podman/errors/__init__.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     4045 2022-10-19 21:26:36.000000 podman-4.5.1/podman/errors/exceptions.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      894 2022-10-19 21:26:36.000000 podman-4.5.1/podman/tlsconfig.py
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       82 2023-05-31 15:05:01.000000 podman-4.5.1/podman/version.py
+drwxr-xr-x   0 umohnani  (1000) umohnani  (1000)        0 2023-05-31 15:45:46.195281 podman-4.5.1/podman.egg-info/
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     2884 2023-05-31 15:45:45.000000 podman-4.5.1/podman.egg-info/PKG-INFO
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1155 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/SOURCES.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        1 2023-05-31 15:45:45.000000 podman-4.5.1/podman.egg-info/dependency_links.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)       91 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/requires.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)        7 2023-05-31 15:45:46.000000 podman-4.5.1/podman.egg-info/top_level.txt
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      662 2023-04-27 13:32:41.000000 podman-4.5.1/pyproject.toml
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)     1323 2023-05-31 15:45:46.201281 podman-4.5.1/setup.cfg
+-rw-r--r--   0 umohnani  (1000) umohnani  (1000)      611 2022-10-19 21:26:36.000000 podman-4.5.1/setup.py
```

### Comparing `podman-4.5.0/LICENSE` & `podman-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/PKG-INFO` & `podman-4.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.5.0
+Version: 4.5.1
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
```

### Comparing `podman-4.5.0/README.md` & `podman-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/__init__.py` & `podman-4.5.1/podman/api/__init__.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/adapter_utils.py` & `podman-4.5.1/podman/api/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/client.py` & `podman-4.5.1/podman/api/client.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/http_utils.py` & `podman-4.5.1/podman/api/http_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/parse_utils.py` & `podman-4.5.1/podman/api/parse_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/ssh.py` & `podman-4.5.1/podman/api/ssh.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/tar_utils.py` & `podman-4.5.1/podman/api/tar_utils.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/typing_extensions.py` & `podman-4.5.1/podman/api/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/api/uds.py` & `podman-4.5.1/podman/api/uds.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/client.py` & `podman-4.5.1/podman/client.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/config.py` & `podman-4.5.1/podman/domain/config.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/containers.py` & `podman-4.5.1/podman/domain/containers.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/containers_create.py` & `podman-4.5.1/podman/domain/containers_create.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/containers_manager.py` & `podman-4.5.1/podman/domain/containers_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/containers_run.py` & `podman-4.5.1/podman/domain/containers_run.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/events.py` & `podman-4.5.1/podman/domain/events.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/images.py` & `podman-4.5.1/podman/domain/images.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/images_build.py` & `podman-4.5.1/podman/domain/images_build.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/images_manager.py` & `podman-4.5.1/podman/domain/images_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/ipam.py` & `podman-4.5.1/podman/domain/ipam.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/manager.py` & `podman-4.5.1/podman/domain/manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/manifests.py` & `podman-4.5.1/podman/domain/manifests.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/networks.py` & `podman-4.5.1/podman/domain/networks.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/networks_manager.py` & `podman-4.5.1/podman/domain/networks_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/pods.py` & `podman-4.5.1/podman/domain/pods.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/pods_manager.py` & `podman-4.5.1/podman/domain/pods_manager.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/registry_data.py` & `podman-4.5.1/podman/domain/registry_data.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/secrets.py` & `podman-4.5.1/podman/domain/secrets.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/system.py` & `podman-4.5.1/podman/domain/system.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/domain/volumes.py` & `podman-4.5.1/podman/domain/volumes.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/errors/__init__.py` & `podman-4.5.1/podman/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/errors/exceptions.py` & `podman-4.5.1/podman/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman/tlsconfig.py` & `podman-4.5.1/podman/tlsconfig.py`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/podman.egg-info/PKG-INFO` & `podman-4.5.1/podman.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podman
-Version: 4.5.0
+Version: 4.5.1
 Summary: Bindings for Podman RESTful API
 Home-page: https://github.com/containers/podman-py
 Author: Brent Baude, Jhon Honce
 Author-email: jhonce@redhat.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/containers/podman-py/issues
 Project-URL: Libpod API, https://docs.podman.io/en/latest/_static/api.html
```

### Comparing `podman-4.5.0/podman.egg-info/SOURCES.txt` & `podman-4.5.1/podman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/pyproject.toml` & `podman-4.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `podman-4.5.0/setup.cfg` & `podman-4.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = podman
-version = 4.5.0
+version = 4.5.1
 author = Brent Baude, Jhon Honce
 author_email = jhonce@redhat.com
 description = Bindings for Podman RESTful API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/containers/podman-py
 license = Apache-2.0
@@ -32,15 +32,15 @@
 include_package_data = True
 python_requires = >=3.6
 test_suite = 
 install_requires = 
 	pyxdg >=0.26
 	requests >=2.24
 	tomli>=1.2.3; python_version<'3.11'
-	urllib3 >=1.26.5
+	urllib3 >= 1.26.5, < 2.0.0
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 formats = gztar
```

### Comparing `podman-4.5.0/setup.py` & `podman-4.5.1/setup.py`

 * *Files identical despite different names*

