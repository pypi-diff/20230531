# Comparing `tmp/google-cloud-dms-1.6.2.tar.gz` & `tmp/google-cloud-dms-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dms-1.6.2.tar", last modified: Mon Mar 27 15:00:34 2023, max compression
+gzip compressed data, was "google-cloud-dms-1.7.0.tar", last modified: Wed May 31 20:49:48 2023, max compression
```

## Comparing `google-cloud-dms-1.6.2.tar` & `google-cloud-dms-1.7.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.965376 google-cloud-dms-1.6.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4791 2023-03-27 15:00:34.965376 google-cloud-dms-1.6.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3887 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.953379 google-cloud-dms-1.6.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.953379 google-cloud-dms-1.6.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.957378 google-cloud-dms-1.6.2/google/cloud/clouddms/
--rw-rw-r--   0 root         (0)     1003     3381 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.957378 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/
--rw-rw-r--   0 root         (0)     1003     3219 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5147 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.957378 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/
--rw-rw-r--   0 root         (0)     1003      793 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    86935 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    98757 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/client.py
--rw-rw-r--   0 root         (0)     1003    11154 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1255 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13766 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31875 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32683 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/types/
--rw-rw-r--   0 root         (0)     1003     2901 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    23367 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/types/clouddms.py
--rw-rw-r--   0 root         (0)     1003    41690 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/google/cloud/clouddms_v1/types/clouddms_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/
--rw-r--r--   0 root         (0)     1003     4791 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1546 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:00:34.000000 google-cloud-dms-1.6.2/google_cloud_dms.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:00:34.965376 google-cloud-dms-1.6.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2910 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:00:34.961377 google-cloud-dms-1.6.2/tests/unit/gapic/clouddms_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/tests/unit/gapic/clouddms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   199637 2023-03-27 14:58:03.000000 google-cloud-dms-1.6.2/tests/unit/gapic/clouddms_v1/test_data_migration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4791 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3887 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.861137 google-cloud-dms-1.7.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.861137 google-cloud-dms-1.7.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms/
+-rw-rw-r--   0 root         (0)     1003     6922 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/
+-rw-rw-r--   0 root         (0)     1003     6736 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10619 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/
+-rw-rw-r--   0 root         (0)     1003      793 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   196914 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   213369 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    32059 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.865137 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1255 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25648 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    65408 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    66754 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/
+-rw-rw-r--   0 root         (0)     1003     6412 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53494 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms.py
+-rw-rw-r--   0 root         (0)     1003    68164 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms_resources.py
+-rw-rw-r--   0 root         (0)     1003    37330 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/conversionworkspace_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/
+-rw-r--r--   0 root         (0)     1003     4791 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1610 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:48.000000 google-cloud-dms-1.7.0/google_cloud_dms.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2957 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:48.869138 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   425567 2023-05-31 20:47:05.000000 google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/test_data_migration_service.py
```

### Comparing `google-cloud-dms-1.6.2/LICENSE` & `google-cloud-dms-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/MANIFEST.in` & `google-cloud-dms-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/PKG-INFO` & `google-cloud-dms-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dms
-Version: 1.6.2
+Version: 1.7.0
 Summary: Google Cloud Dms API client library
 Home-page: https://github.com/googleapis/python-dms
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dms-1.6.2/README.rst` & `google-cloud-dms-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms/gapic_version.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.2"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms_v1/gapic_version.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.2"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/__init__.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/__init__.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/google/cloud/clouddms_v1/types/clouddms_resources.py` & `google-cloud-dms-1.7.0/google/cloud/clouddms_v1/types/clouddms_resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,65 +22,103 @@
 from google.protobuf import wrappers_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.clouddms.v1",
     manifest={
+        "NetworkArchitecture",
         "DatabaseEngine",
         "DatabaseProvider",
         "SslConfig",
         "MySqlConnectionProfile",
         "PostgreSqlConnectionProfile",
+        "OracleConnectionProfile",
         "CloudSqlConnectionProfile",
+        "AlloyDbConnectionProfile",
         "SqlAclEntry",
         "SqlIpConfig",
         "CloudSqlSettings",
+        "AlloyDbSettings",
         "StaticIpConnectivity",
+        "PrivateServiceConnectConnectivity",
         "ReverseSshConnectivity",
         "VpcPeeringConnectivity",
+        "ForwardSshTunnelConnectivity",
+        "StaticServiceIpConnectivity",
+        "PrivateConnectivity",
         "DatabaseType",
         "MigrationJob",
+        "ConversionWorkspaceInfo",
         "ConnectionProfile",
         "MigrationJobVerificationError",
+        "PrivateConnection",
+        "VpcPeeringConfig",
     },
 )
 
 
+class NetworkArchitecture(proto.Enum):
+    r"""
+
+    Values:
+        NETWORK_ARCHITECTURE_UNSPECIFIED (0):
+            No description available.
+        NETWORK_ARCHITECTURE_OLD_CSQL_PRODUCER (1):
+            Instance is in Cloud SQL's old producer
+            network architecture.
+        NETWORK_ARCHITECTURE_NEW_CSQL_PRODUCER (2):
+            Instance is in Cloud SQL's new producer
+            network architecture.
+    """
+    NETWORK_ARCHITECTURE_UNSPECIFIED = 0
+    NETWORK_ARCHITECTURE_OLD_CSQL_PRODUCER = 1
+    NETWORK_ARCHITECTURE_NEW_CSQL_PRODUCER = 2
+
+
 class DatabaseEngine(proto.Enum):
     r"""The database engine types.
 
     Values:
         DATABASE_ENGINE_UNSPECIFIED (0):
             The source database engine of the migration
             job is unknown.
         MYSQL (1):
             The source engine is MySQL.
         POSTGRESQL (2):
             The source engine is PostgreSQL.
+        ORACLE (4):
+            The source engine is Oracle.
     """
     DATABASE_ENGINE_UNSPECIFIED = 0
     MYSQL = 1
     POSTGRESQL = 2
+    ORACLE = 4
 
 
 class DatabaseProvider(proto.Enum):
     r"""The database providers.
 
     Values:
         DATABASE_PROVIDER_UNSPECIFIED (0):
             The database provider is unknown.
         CLOUDSQL (1):
             CloudSQL runs the database.
         RDS (2):
             RDS runs the database.
+        AURORA (3):
+            Amazon Aurora.
+        ALLOYDB (4):
+            AlloyDB.
     """
     DATABASE_PROVIDER_UNSPECIFIED = 0
     CLOUDSQL = 1
     RDS = 2
+    AURORA = 3
+    ALLOYDB = 4
 
 
 class SslConfig(proto.Message):
     r"""SSL configuration information.
 
     Attributes:
         type_ (google.cloud.clouddms_v1.types.SslConfig.SslType):
@@ -205,14 +243,21 @@
     )
 
 
 class PostgreSqlConnectionProfile(proto.Message):
     r"""Specifies connection parameters required specifically for
     PostgreSQL databases.
 
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
     Attributes:
         host (str):
             Required. The IP or hostname of the source
             PostgreSQL database.
         port (int):
             Required. The network port of the source
             PostgreSQL database.
@@ -234,14 +279,27 @@
         ssl (google.cloud.clouddms_v1.types.SslConfig):
             SSL configuration for the destination to
             connect to the source database.
         cloud_sql_id (str):
             If the source is a Cloud SQL database, use
             this field to provide the Cloud SQL instance ID
             of the source.
+        network_architecture (google.cloud.clouddms_v1.types.NetworkArchitecture):
+            Output only. If the source is a Cloud SQL
+            database, this field indicates the network
+            architecture it's associated with.
+        static_ip_connectivity (google.cloud.clouddms_v1.types.StaticIpConnectivity):
+            Static ip connectivity data (default, no
+            additional details needed).
+
+            This field is a member of `oneof`_ ``connectivity``.
+        private_service_connect_connectivity (google.cloud.clouddms_v1.types.PrivateServiceConnectConnectivity):
+            Private service connect connectivity.
+
+            This field is a member of `oneof`_ ``connectivity``.
     """
 
     host: str = proto.Field(
         proto.STRING,
         number=1,
     )
     port: int = proto.Field(
@@ -265,14 +323,127 @@
         number=6,
         message="SslConfig",
     )
     cloud_sql_id: str = proto.Field(
         proto.STRING,
         number=7,
     )
+    network_architecture: "NetworkArchitecture" = proto.Field(
+        proto.ENUM,
+        number=8,
+        enum="NetworkArchitecture",
+    )
+    static_ip_connectivity: "StaticIpConnectivity" = proto.Field(
+        proto.MESSAGE,
+        number=100,
+        oneof="connectivity",
+        message="StaticIpConnectivity",
+    )
+    private_service_connect_connectivity: "PrivateServiceConnectConnectivity" = (
+        proto.Field(
+            proto.MESSAGE,
+            number=101,
+            oneof="connectivity",
+            message="PrivateServiceConnectConnectivity",
+        )
+    )
+
+
+class OracleConnectionProfile(proto.Message):
+    r"""Specifies connection parameters required specifically for
+    Oracle databases.
+
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        host (str):
+            Required. The IP or hostname of the source
+            Oracle database.
+        port (int):
+            Required. The network port of the source
+            Oracle database.
+        username (str):
+            Required. The username that Database
+            Migration Service will use to connect to the
+            database. The value is encrypted when stored in
+            Database Migration Service.
+        password (str):
+            Required. Input only. The password for the
+            user that Database Migration Service will be
+            using to connect to the database. This field is
+            not returned on request, and the value is
+            encrypted when stored in Database Migration
+            Service.
+        password_set (bool):
+            Output only. Indicates whether a new password
+            is included in the request.
+        database_service (str):
+            Required. Database service for the Oracle
+            connection.
+        static_service_ip_connectivity (google.cloud.clouddms_v1.types.StaticServiceIpConnectivity):
+            Static Service IP connectivity.
+
+            This field is a member of `oneof`_ ``connectivity``.
+        forward_ssh_connectivity (google.cloud.clouddms_v1.types.ForwardSshTunnelConnectivity):
+            Forward SSH tunnel connectivity.
+
+            This field is a member of `oneof`_ ``connectivity``.
+        private_connectivity (google.cloud.clouddms_v1.types.PrivateConnectivity):
+            Private connectivity.
+
+            This field is a member of `oneof`_ ``connectivity``.
+    """
+
+    host: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    port: int = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    username: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    password: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    password_set: bool = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
+    database_service: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    static_service_ip_connectivity: "StaticServiceIpConnectivity" = proto.Field(
+        proto.MESSAGE,
+        number=100,
+        oneof="connectivity",
+        message="StaticServiceIpConnectivity",
+    )
+    forward_ssh_connectivity: "ForwardSshTunnelConnectivity" = proto.Field(
+        proto.MESSAGE,
+        number=101,
+        oneof="connectivity",
+        message="ForwardSshTunnelConnectivity",
+    )
+    private_connectivity: "PrivateConnectivity" = proto.Field(
+        proto.MESSAGE,
+        number=102,
+        oneof="connectivity",
+        message="PrivateConnectivity",
+    )
 
 
 class CloudSqlConnectionProfile(proto.Message):
     r"""Specifies required connection parameters, and, optionally,
     the parameters required to create a Cloud SQL destination
     database instance.
 
@@ -285,14 +456,20 @@
             destination Cloud SQL database.
         private_ip (str):
             Output only. The Cloud SQL database
             instance's private IP.
         public_ip (str):
             Output only. The Cloud SQL database
             instance's public IP.
+        additional_public_ip (str):
+            Output only. The Cloud SQL database
+            instance's additional (outgoing) public IP. Used
+            when the Cloud SQL database availability type is
+            REGIONAL (i.e. multiple zones / highly
+            available).
     """
 
     cloud_sql_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
     settings: "CloudSqlSettings" = proto.Field(
@@ -304,14 +481,42 @@
         proto.STRING,
         number=3,
     )
     public_ip: str = proto.Field(
         proto.STRING,
         number=4,
     )
+    additional_public_ip: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+
+
+class AlloyDbConnectionProfile(proto.Message):
+    r"""Specifies required connection parameters, and the parameters
+    required to create an AlloyDB destination cluster.
+
+    Attributes:
+        cluster_id (str):
+            Required. The AlloyDB cluster ID that this
+            connection profile is associated with.
+        settings (google.cloud.clouddms_v1.types.AlloyDbSettings):
+            Immutable. Metadata used to create the
+            destination AlloyDB cluster.
+    """
+
+    cluster_id: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    settings: "AlloyDbSettings" = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message="AlloyDbSettings",
+    )
 
 
 class SqlAclEntry(proto.Message):
     r"""An entry for an Access Control list.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -369,14 +574,25 @@
             Whether the instance should be assigned an
             IPv4 address or not.
         private_network (str):
             The resource link for the VPC network from which the Cloud
             SQL instance is accessible for private IP. For example,
             ``projects/myProject/global/networks/default``. This setting
             can be updated, but it cannot be removed after it is set.
+        allocated_ip_range (str):
+            Optional. The name of the allocated IP
+            address range for the private IP Cloud SQL
+            instance. This name refers to an already
+            allocated IP range address. If set, the instance
+            IP address will be created in the allocated
+            range. Note that this IP address range can't be
+            modified after the instance is created. If you
+            change the VPC when configuring connectivity
+            settings for the migration job, this field is
+            not relevant.
         require_ssl (google.protobuf.wrappers_pb2.BoolValue):
             Whether SSL connections over IP should be
             enforced or not.
         authorized_networks (MutableSequence[google.cloud.clouddms_v1.types.SqlAclEntry]):
             The list of external networks that are allowed to connect to
             the instance using the IP. See
             https://en.wikipedia.org/wiki/CIDR_notation#CIDR_notation,
@@ -388,14 +604,18 @@
         number=1,
         message=wrappers_pb2.BoolValue,
     )
     private_network: str = proto.Field(
         proto.STRING,
         number=2,
     )
+    allocated_ip_range: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
     require_ssl: wrappers_pb2.BoolValue = proto.Field(
         proto.MESSAGE,
         number=3,
         message=wrappers_pb2.BoolValue,
     )
     authorized_networks: MutableSequence["SqlAclEntry"] = proto.RepeatedField(
         proto.MESSAGE,
@@ -461,27 +681,42 @@
             The type of storage: ``PD_SSD`` (default) or ``PD_HDD``.
         data_disk_size_gb (google.protobuf.wrappers_pb2.Int64Value):
             The storage capacity available to the
             database, in GB. The minimum (and default) size
             is 10GB.
         zone (str):
             The Google Cloud Platform zone where your
-            Cloud SQL datdabse instance is located.
+            Cloud SQL database instance is located.
+        secondary_zone (str):
+            Optional. The Google Cloud Platform zone
+            where the failover Cloud SQL database instance
+            is located. Used when the Cloud SQL database
+            availability type is REGIONAL (i.e. multiple
+            zones / highly available).
         source_id (str):
             The Database Migration Service source connection profile ID,
             in the format:
             ``projects/my_project_name/locations/us-central1/connectionProfiles/connection_profile_ID``
         root_password (str):
             Input only. Initial root password.
         root_password_set (bool):
             Output only. Indicates If this connection
             profile root password is stored.
         collation (str):
             The Cloud SQL default instance level
             collation.
+        cmek_key_name (str):
+            The KMS key name used for the csql instance.
+        availability_type (google.cloud.clouddms_v1.types.CloudSqlSettings.SqlAvailabilityType):
+            Optional. Availability type. Potential values:
+
+            -  ``ZONAL``: The instance serves data from only one zone.
+               Outages in that zone affect data availability.
+            -  ``REGIONAL``: The instance can serve data from more than
+               one zone in a region (it is highly available).
     """
 
     class SqlActivationPolicy(proto.Enum):
         r"""Specifies when the instance should be activated.
 
         Values:
             SQL_ACTIVATION_POLICY_UNSPECIFIED (0):
@@ -528,24 +763,42 @@
                 PostgreSQL 10.
             MYSQL_8_0 (6):
                 MySQL 8.0.
             POSTGRES_12 (7):
                 PostgreSQL 12.
             POSTGRES_13 (8):
                 PostgreSQL 13.
+            POSTGRES_14 (17):
+                PostgreSQL 14.
         """
         SQL_DATABASE_VERSION_UNSPECIFIED = 0
         MYSQL_5_6 = 1
         MYSQL_5_7 = 2
         POSTGRES_9_6 = 3
         POSTGRES_11 = 4
         POSTGRES_10 = 5
         MYSQL_8_0 = 6
         POSTGRES_12 = 7
         POSTGRES_13 = 8
+        POSTGRES_14 = 17
+
+    class SqlAvailabilityType(proto.Enum):
+        r"""The availability type of the given Cloud SQL instance.
+
+        Values:
+            SQL_AVAILABILITY_TYPE_UNSPECIFIED (0):
+                This is an unknown Availability type.
+            ZONAL (1):
+                Zonal availablility instance.
+            REGIONAL (2):
+                Regional availability instance.
+        """
+        SQL_AVAILABILITY_TYPE_UNSPECIFIED = 0
+        ZONAL = 1
+        REGIONAL = 2
 
     database_version: SqlDatabaseVersion = proto.Field(
         proto.ENUM,
         number=1,
         enum=SqlDatabaseVersion,
     )
     user_labels: MutableMapping[str, str] = proto.MapField(
@@ -592,14 +845,18 @@
         number=10,
         message=wrappers_pb2.Int64Value,
     )
     zone: str = proto.Field(
         proto.STRING,
         number=11,
     )
+    secondary_zone: str = proto.Field(
+        proto.STRING,
+        number=18,
+    )
     source_id: str = proto.Field(
         proto.STRING,
         number=12,
     )
     root_password: str = proto.Field(
         proto.STRING,
         number=13,
@@ -608,24 +865,214 @@
         proto.BOOL,
         number=14,
     )
     collation: str = proto.Field(
         proto.STRING,
         number=15,
     )
+    cmek_key_name: str = proto.Field(
+        proto.STRING,
+        number=16,
+    )
+    availability_type: SqlAvailabilityType = proto.Field(
+        proto.ENUM,
+        number=17,
+        enum=SqlAvailabilityType,
+    )
+
+
+class AlloyDbSettings(proto.Message):
+    r"""Settings for creating an AlloyDB cluster.
+
+    Attributes:
+        initial_user (google.cloud.clouddms_v1.types.AlloyDbSettings.UserPassword):
+            Required. Input only. Initial user to setup
+            during cluster creation. Required.
+        vpc_network (str):
+            Required. The resource link for the VPC network in which
+            cluster resources are created and from which they are
+            accessible via Private IP. The network must belong to the
+            same project as the cluster. It is specified in the form:
+            "projects/{project_number}/global/networks/{network_id}".
+            This is required to create a cluster.
+        labels (MutableMapping[str, str]):
+            Labels for the AlloyDB cluster created by
+            DMS. An object containing a list of 'key',
+            'value' pairs.
+        primary_instance_settings (google.cloud.clouddms_v1.types.AlloyDbSettings.PrimaryInstanceSettings):
+
+        encryption_config (google.cloud.clouddms_v1.types.AlloyDbSettings.EncryptionConfig):
+            Optional. The encryption config can be
+            specified to encrypt the data disks and other
+            persistent data resources of a cluster with a
+            customer-managed encryption key (CMEK). When
+            this field is not specified, the cluster will
+            then use default encryption scheme to protect
+            the user data.
+    """
+
+    class UserPassword(proto.Message):
+        r"""The username/password for a database user. Used for
+        specifying initial users at cluster creation time.
+
+        Attributes:
+            user (str):
+                The database username.
+            password (str):
+                The initial password for the user.
+            password_set (bool):
+                Output only. Indicates if the initial_user.password field
+                has been set.
+        """
+
+        user: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        password: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+        password_set: bool = proto.Field(
+            proto.BOOL,
+            number=3,
+        )
+
+    class PrimaryInstanceSettings(proto.Message):
+        r"""Settings for the cluster's primary instance
+
+        Attributes:
+            id (str):
+                Required. The ID of the AlloyDB primary instance. The ID
+                must satisfy the regex expression "[a-z0-9-]+".
+            machine_config (google.cloud.clouddms_v1.types.AlloyDbSettings.PrimaryInstanceSettings.MachineConfig):
+                Configuration for the machines that host the
+                underlying database engine.
+            database_flags (MutableMapping[str, str]):
+                Database flags to pass to AlloyDB when DMS is
+                creating the AlloyDB cluster and instances. See
+                the AlloyDB documentation for how these can be
+                used.
+            labels (MutableMapping[str, str]):
+                Labels for the AlloyDB primary instance
+                created by DMS. An object containing a list of
+                'key', 'value' pairs.
+            private_ip (str):
+                Output only. The private IP address for the
+                Instance. This is the connection endpoint for an
+                end-user application.
+        """
+
+        class MachineConfig(proto.Message):
+            r"""MachineConfig describes the configuration of a machine.
+
+            Attributes:
+                cpu_count (int):
+                    The number of CPU's in the VM instance.
+            """
+
+            cpu_count: int = proto.Field(
+                proto.INT32,
+                number=1,
+            )
+
+        id: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        machine_config: "AlloyDbSettings.PrimaryInstanceSettings.MachineConfig" = (
+            proto.Field(
+                proto.MESSAGE,
+                number=2,
+                message="AlloyDbSettings.PrimaryInstanceSettings.MachineConfig",
+            )
+        )
+        database_flags: MutableMapping[str, str] = proto.MapField(
+            proto.STRING,
+            proto.STRING,
+            number=6,
+        )
+        labels: MutableMapping[str, str] = proto.MapField(
+            proto.STRING,
+            proto.STRING,
+            number=7,
+        )
+        private_ip: str = proto.Field(
+            proto.STRING,
+            number=8,
+        )
+
+    class EncryptionConfig(proto.Message):
+        r"""EncryptionConfig describes the encryption config of a cluster
+        that is encrypted with a CMEK (customer-managed encryption key).
+
+        Attributes:
+            kms_key_name (str):
+                The fully-qualified resource name of the KMS key. Each Cloud
+                KMS key is regionalized and has the following format:
+                projects/[PROJECT]/locations/[REGION]/keyRings/[RING]/cryptoKeys/[KEY_NAME]
+        """
+
+        kms_key_name: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+
+    initial_user: UserPassword = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=UserPassword,
+    )
+    vpc_network: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=3,
+    )
+    primary_instance_settings: PrimaryInstanceSettings = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message=PrimaryInstanceSettings,
+    )
+    encryption_config: EncryptionConfig = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message=EncryptionConfig,
+    )
 
 
 class StaticIpConnectivity(proto.Message):
     r"""The source database will allow incoming connections from the
-    destination database's public IP. You can retrieve the Cloud SQL
-    instance's public IP from the Cloud SQL console or using Cloud
-    SQL APIs. No additional configuration is required.
+    public IP of the destination database. You can retrieve the
+    public IP of the Cloud SQL instance from the Cloud SQL console
+    or using Cloud SQL APIs. No additional configuration is
+    required.
+
+    """
+
 
+class PrivateServiceConnectConnectivity(proto.Message):
+    r"""Private Service Connect connectivity
+    (https://cloud.google.com/vpc/docs/private-service-connect#service-attachments)
+
+    Attributes:
+        service_attachment (str):
+            Required. A service attachment that exposes a database, and
+            has the following format:
+            projects/{project}/regions/{region}/serviceAttachments/{service_attachment_name}
     """
 
+    service_attachment: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
 
 class ReverseSshConnectivity(proto.Message):
     r"""The details needed to configure a reverse SSH tunnel between
     the source and destination databases. These details will be used
     when calling the generateSshScript method (see
     https://cloud.google.com/database-migration/docs/reference/rest/v1/projects.locations.migrationJobs/generateSshScript)
     to produce the script that will help set up the reverse SSH
@@ -681,14 +1128,84 @@
 
     vpc: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
+class ForwardSshTunnelConnectivity(proto.Message):
+    r"""Forward SSH Tunnel connectivity.
+
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        hostname (str):
+            Required. Hostname for the SSH tunnel.
+        username (str):
+            Required. Username for the SSH tunnel.
+        port (int):
+            Port for the SSH tunnel, default value is 22.
+        password (str):
+            Input only. SSH password.
+
+            This field is a member of `oneof`_ ``authentication_method``.
+        private_key (str):
+            Input only. SSH private key.
+
+            This field is a member of `oneof`_ ``authentication_method``.
+    """
+
+    hostname: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    username: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    port: int = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    password: str = proto.Field(
+        proto.STRING,
+        number=100,
+        oneof="authentication_method",
+    )
+    private_key: str = proto.Field(
+        proto.STRING,
+        number=101,
+        oneof="authentication_method",
+    )
+
+
+class StaticServiceIpConnectivity(proto.Message):
+    r"""Static IP address connectivity configured on service project."""
+
+
+class PrivateConnectivity(proto.Message):
+    r"""Private Connectivity.
+
+    Attributes:
+        private_connection (str):
+            Required. The resource name (URI) of the
+            private connection.
+    """
+
+    private_connection: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
 class DatabaseType(proto.Message):
     r"""A message defining the database engine and provider.
 
     Attributes:
         provider (google.cloud.clouddms_v1.types.DatabaseProvider):
             The database provider.
         engine (google.cloud.clouddms_v1.types.DatabaseEngine):
@@ -717,15 +1234,15 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             The name (URI) of this migration job
             resource, in the form of:
-            projects/{project}/locations/{location}/instances/{instance}.
+            projects/{project}/locations/{location}/migrationJobs/{migrationJob}.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the migration
             job resource was created. A timestamp in RFC3339
             UTC "Zulu" format, accurate to nanoseconds.
             Example: "2014-10-02T15:01:23.045123456Z".
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the migration
@@ -746,15 +1263,19 @@
             The current migration job state.
         phase (google.cloud.clouddms_v1.types.MigrationJob.Phase):
             Output only. The current migration job phase.
         type_ (google.cloud.clouddms_v1.types.MigrationJob.Type):
             Required. The migration job type.
         dump_path (str):
             The path to the dump file in Google Cloud Storage, in the
-            format: (gs://[BUCKET_NAME]/[OBJECT_NAME]).
+            format: (gs://[BUCKET_NAME]/[OBJECT_NAME]). This field and
+            the "dump_flags" field are mutually exclusive.
+        dump_flags (google.cloud.clouddms_v1.types.MigrationJob.DumpFlags):
+            The initial dump flags. This field and the "dump_path" field
+            are mutually exclusive.
         source (str):
             Required. The resource name (URI) of the
             source connection profile.
         destination (str):
             Required. The resource name (URI) of the
             destination connection profile.
         reverse_ssh_connectivity (google.cloud.clouddms_v1.types.ReverseSshConnectivity):
@@ -785,14 +1306,38 @@
             source.
         destination_database (google.cloud.clouddms_v1.types.DatabaseType):
             The database engine type and provider of the
             destination.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. If the migration job is
             completed, the time when it was completed.
+        conversion_workspace (google.cloud.clouddms_v1.types.ConversionWorkspaceInfo):
+            The conversion workspace used by the
+            migration.
+        filter (str):
+            This field can be used to select the entities
+            to migrate as part of the migration job. It uses
+            AIP-160 notation to select a subset of the
+            entities configured on the associated
+            conversion-workspace. This field should not be
+            set on migration-jobs that are not associated
+            with a conversion workspace.
+        cmek_key_name (str):
+            The CMEK (customer-managed encryption key) fully qualified
+            key name used for the migration job. This field supports all
+            migration jobs types except for:
+
+            -  Mysql to Mysql (use the cmek field in the cloudsql
+               connection profile instead).
+            -  PostrgeSQL to PostgreSQL (use the cmek field in the
+               cloudsql connection profile instead).
+            -  PostgreSQL to AlloyDB (use the kms_key_name field in the
+               alloydb connection profile instead). Each Cloud CMEK key
+               has the following format:
+               projects/[PROJECT]/locations/[REGION]/keyRings/[RING]/cryptoKeys/[KEY_NAME]
     """
 
     class State(proto.Enum):
         r"""The current migration job states.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -884,14 +1429,47 @@
             CONTINUOUS (2):
                 The migration job is a continuous migration.
         """
         TYPE_UNSPECIFIED = 0
         ONE_TIME = 1
         CONTINUOUS = 2
 
+    class DumpFlag(proto.Message):
+        r"""Dump flag definition.
+
+        Attributes:
+            name (str):
+                The name of the flag
+            value (str):
+                The value of the flag.
+        """
+
+        name: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        value: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+
+    class DumpFlags(proto.Message):
+        r"""Dump flags definition.
+
+        Attributes:
+            dump_flags (MutableSequence[google.cloud.clouddms_v1.types.MigrationJob.DumpFlag]):
+                The flags for the initial dump.
+        """
+
+        dump_flags: MutableSequence["MigrationJob.DumpFlag"] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=1,
+            message="MigrationJob.DumpFlag",
+        )
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
@@ -926,14 +1504,19 @@
         number=8,
         enum=Type,
     )
     dump_path: str = proto.Field(
         proto.STRING,
         number=9,
     )
+    dump_flags: DumpFlags = proto.Field(
+        proto.MESSAGE,
+        number=17,
+        message=DumpFlags,
+    )
     source: str = proto.Field(
         proto.STRING,
         number=10,
     )
     destination: str = proto.Field(
         proto.STRING,
         number=11,
@@ -977,14 +1560,48 @@
         message="DatabaseType",
     )
     end_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=16,
         message=timestamp_pb2.Timestamp,
     )
+    conversion_workspace: "ConversionWorkspaceInfo" = proto.Field(
+        proto.MESSAGE,
+        number=18,
+        message="ConversionWorkspaceInfo",
+    )
+    filter: str = proto.Field(
+        proto.STRING,
+        number=20,
+    )
+    cmek_key_name: str = proto.Field(
+        proto.STRING,
+        number=21,
+    )
+
+
+class ConversionWorkspaceInfo(proto.Message):
+    r"""A conversion workspace's version.
+
+    Attributes:
+        name (str):
+            The resource name (URI) of the conversion
+            workspace.
+        commit_id (str):
+            The commit ID of the conversion workspace.
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    commit_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 class ConnectionProfile(proto.Message):
     r"""A connection profile definition.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -993,15 +1610,15 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             The name of this connection profile resource
             in the form of
-            projects/{project}/locations/{location}/instances/{instance}.
+            projects/{project}/locations/{location}/connectionProfiles/{connectionProfile}.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the resource
             was created. A timestamp in RFC3339 UTC "Zulu"
             format, accurate to nanoseconds. Example:
             "2014-10-02T15:01:23.045123456Z".
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the resource
@@ -1025,18 +1642,26 @@
             A MySQL database connection profile.
 
             This field is a member of `oneof`_ ``connection_profile``.
         postgresql (google.cloud.clouddms_v1.types.PostgreSqlConnectionProfile):
             A PostgreSQL database connection profile.
 
             This field is a member of `oneof`_ ``connection_profile``.
+        oracle (google.cloud.clouddms_v1.types.OracleConnectionProfile):
+            An Oracle database connection profile.
+
+            This field is a member of `oneof`_ ``connection_profile``.
         cloudsql (google.cloud.clouddms_v1.types.CloudSqlConnectionProfile):
             A CloudSQL database connection profile.
 
             This field is a member of `oneof`_ ``connection_profile``.
+        alloydb (google.cloud.clouddms_v1.types.AlloyDbConnectionProfile):
+            An AlloyDB cluster connection profile.
+
+            This field is a member of `oneof`_ ``connection_profile``.
         error (google.rpc.status_pb2.Status):
             Output only. The error details in case of
             state FAILED.
         provider (google.cloud.clouddms_v1.types.DatabaseProvider):
             The database provider.
     """
 
@@ -1110,20 +1735,32 @@
     )
     postgresql: "PostgreSqlConnectionProfile" = proto.Field(
         proto.MESSAGE,
         number=101,
         oneof="connection_profile",
         message="PostgreSqlConnectionProfile",
     )
+    oracle: "OracleConnectionProfile" = proto.Field(
+        proto.MESSAGE,
+        number=104,
+        oneof="connection_profile",
+        message="OracleConnectionProfile",
+    )
     cloudsql: "CloudSqlConnectionProfile" = proto.Field(
         proto.MESSAGE,
         number=102,
         oneof="connection_profile",
         message="CloudSqlConnectionProfile",
     )
+    alloydb: "AlloyDbConnectionProfile" = proto.Field(
+        proto.MESSAGE,
+        number=105,
+        oneof="connection_profile",
+        message="AlloyDbConnectionProfile",
+    )
     error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=7,
         message=status_pb2.Status,
     )
     provider: "DatabaseProvider" = proto.Field(
         proto.ENUM,
@@ -1201,14 +1838,28 @@
                 The table definition is not support due to
                 missing primary key or replica identity.
             UNSUPPORTED_DEFINER (19):
                 The definer is not supported.
             CANT_RESTART_RUNNING_MIGRATION (21):
                 Migration is already running at the time of
                 restart request.
+            TABLES_WITH_LIMITED_SUPPORT (24):
+                The source has tables with limited support.
+                E.g. PostgreSQL tables without primary keys.
+            UNSUPPORTED_DATABASE_LOCALE (25):
+                The source uses an unsupported locale.
+            UNSUPPORTED_DATABASE_FDW_CONFIG (26):
+                The source uses an unsupported Foreign Data
+                Wrapper configuration.
+            ERROR_RDBMS (27):
+                There was an underlying RDBMS error.
+            SOURCE_SIZE_EXCEEDS_THRESHOLD (28):
+                The source DB size in Bytes exceeds a certain
+                threshold. The migration might require an
+                increase of quota, or might not be supported.
         """
         ERROR_CODE_UNSPECIFIED = 0
         CONNECTION_FAILURE = 1
         AUTHENTICATION_FAILURE = 2
         INVALID_CONNECTION_PROFILE_CONFIG = 3
         VERSION_INCOMPATIBILITY = 4
         CONNECTION_PROFILE_TYPES_INCOMPATIBILITY = 5
@@ -1222,14 +1873,19 @@
         UNSUPPORTED_EXTENSIONS = 14
         UNSUPPORTED_MIGRATION_TYPE = 15
         INVALID_RDS_LOGICAL_REPLICATION = 16
         UNSUPPORTED_GTID_MODE = 17
         UNSUPPORTED_TABLE_DEFINITION = 18
         UNSUPPORTED_DEFINER = 19
         CANT_RESTART_RUNNING_MIGRATION = 21
+        TABLES_WITH_LIMITED_SUPPORT = 24
+        UNSUPPORTED_DATABASE_LOCALE = 25
+        UNSUPPORTED_DATABASE_FDW_CONFIG = 26
+        ERROR_RDBMS = 27
+        SOURCE_SIZE_EXCEEDS_THRESHOLD = 28
 
     error_code: ErrorCode = proto.Field(
         proto.ENUM,
         number=1,
         enum=ErrorCode,
     )
     error_message: str = proto.Field(
@@ -1238,8 +1894,139 @@
     )
     error_detail_message: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
+class PrivateConnection(proto.Message):
+    r"""The PrivateConnection resource is used to establish private
+    connectivity with the customer's network.
+
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        name (str):
+            The name of the resource.
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The create time of the resource.
+        update_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The last update time of the
+            resource.
+        labels (MutableMapping[str, str]):
+            The resource labels for private connections to use to
+            annotate any related underlying resources such as Compute
+            Engine VMs. An object containing a list of "key": "value"
+            pairs.
+
+            Example:
+            ``{ "name": "wrench", "mass": "1.3kg", "count": "3" }``.
+        display_name (str):
+            The private connection display name.
+        state (google.cloud.clouddms_v1.types.PrivateConnection.State):
+            Output only. The state of the private
+            connection.
+        error (google.rpc.status_pb2.Status):
+            Output only. The error details in case of
+            state FAILED.
+        vpc_peering_config (google.cloud.clouddms_v1.types.VpcPeeringConfig):
+            VPC peering configuration.
+
+            This field is a member of `oneof`_ ``connectivity``.
+    """
+
+    class State(proto.Enum):
+        r"""Private Connection state.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                No description available.
+            CREATING (1):
+                The private connection is in creation state -
+                creating resources.
+            CREATED (2):
+                The private connection has been created with
+                all of its resources.
+            FAILED (3):
+                The private connection creation has failed.
+            DELETING (4):
+                The private connection is being deleted.
+            FAILED_TO_DELETE (5):
+                Delete request has failed, resource is in
+                invalid state.
+            DELETED (6):
+                The private connection has been deleted.
+        """
+        STATE_UNSPECIFIED = 0
+        CREATING = 1
+        CREATED = 2
+        FAILED = 3
+        DELETING = 4
+        FAILED_TO_DELETE = 5
+        DELETED = 6
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    update_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=timestamp_pb2.Timestamp,
+    )
+    labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=4,
+    )
+    display_name: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    state: State = proto.Field(
+        proto.ENUM,
+        number=6,
+        enum=State,
+    )
+    error: status_pb2.Status = proto.Field(
+        proto.MESSAGE,
+        number=7,
+        message=status_pb2.Status,
+    )
+    vpc_peering_config: "VpcPeeringConfig" = proto.Field(
+        proto.MESSAGE,
+        number=100,
+        oneof="connectivity",
+        message="VpcPeeringConfig",
+    )
+
+
+class VpcPeeringConfig(proto.Message):
+    r"""The VPC peering configuration is used to create VPC peering
+    with the consumer's VPC.
+
+    Attributes:
+        vpc_name (str):
+            Required. Fully qualified name of the VPC
+            that Database Migration Service will peer to.
+        subnet (str):
+            Required. A free subnet for peering. (CIDR of
+            /29)
+    """
+
+    vpc_name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    subnet: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dms-1.6.2/google_cloud_dms.egg-info/PKG-INFO` & `google-cloud-dms-1.7.0/google_cloud_dms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dms
-Version: 1.6.2
+Version: 1.7.0
 Summary: Google Cloud Dms API client library
 Home-page: https://github.com/googleapis/python-dms
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dms-1.6.2/google_cloud_dms.egg-info/SOURCES.txt` & `google-cloud-dms-1.7.0/google_cloud_dms.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 google/cloud/clouddms_v1/services/data_migration_service/transports/__init__.py
 google/cloud/clouddms_v1/services/data_migration_service/transports/base.py
 google/cloud/clouddms_v1/services/data_migration_service/transports/grpc.py
 google/cloud/clouddms_v1/services/data_migration_service/transports/grpc_asyncio.py
 google/cloud/clouddms_v1/types/__init__.py
 google/cloud/clouddms_v1/types/clouddms.py
 google/cloud/clouddms_v1/types/clouddms_resources.py
+google/cloud/clouddms_v1/types/conversionworkspace_resources.py
 google_cloud_dms.egg-info/PKG-INFO
 google_cloud_dms.egg-info/SOURCES.txt
 google_cloud_dms.egg-info/dependency_links.txt
 google_cloud_dms.egg-info/namespace_packages.txt
 google_cloud_dms.egg-info/not-zip-safe
 google_cloud_dms.egg-info/requires.txt
 google_cloud_dms.egg-info/top_level.txt
```

### Comparing `google-cloud-dms-1.6.2/setup.py` & `google-cloud-dms-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
 url = "https://github.com/googleapis/python-dms"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `google-cloud-dms-1.6.2/tests/__init__.py` & `google-cloud-dms-1.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/tests/unit/__init__.py` & `google-cloud-dms-1.7.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/tests/unit/gapic/__init__.py` & `google-cloud-dms-1.7.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dms-1.6.2/tests/unit/gapic/clouddms_v1/__init__.py` & `google-cloud-dms-1.7.0/tests/unit/gapic/clouddms_v1/__init__.py`

 * *Files identical despite different names*

