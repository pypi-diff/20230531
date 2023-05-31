# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.902.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.902.tar", last modified: Tue May 30 00:29:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.903.tar", last modified: Wed May 31 02:18:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.902.tar` & `tencentcloud-sdk-python-redis-3.0.903.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    87184 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297481 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-30 00:29:55.000000 tencentcloud-sdk-python-redis-3.0.902/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:29:56.000000 tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    87184 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297533 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:18:02.000000 tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.902/README.rst` & `tencentcloud-sdk-python-redis-3.0.903/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.902/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.903/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1248,23 +1248,23 @@
 class DelayDistribution(AbstractModel):
     """延时分布详情
 
     """
 
     def __init__(self):
         r"""
-        :param Ladder: 分布阶梯，延时和Ladder值的对应关系：
-[0ms,1ms]: 1；
-[1ms,5ms]: 5；
-[5ms,10ms]: 10；
-[10ms,50ms]: 50；
-[50ms,200ms]: 200；
-[200ms,∞]: -1。
+        :param Ladder: 指延时分布阶梯，其与延时区间的对应关系如下所示。
+- 1：[0ms,1ms]。
+- 5： [1ms,5ms]。
+- 10： [5ms,10ms]。
+- 50： [10ms,50ms]。
+- 200：[50ms,200ms]。
+- -1： [200ms,∞]。
         :type Ladder: int
-        :param Size: 延时处于当前分布阶梯的命令数量，个。
+        :param Size: 延时处于当前分布阶梯的命令数量，单位：个。
         :type Size: int
         :param Updatetime: 修改时间。
         :type Updatetime: int
         """
         self.Ladder = None
         self.Size = None
         self.Updatetime = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.902/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.903/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.902'
+__version__ = '3.0.903'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.902/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.902/setup.py` & `tencentcloud-sdk-python-redis-3.0.903/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.902/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.903/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.902
+Version: 3.0.903
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

