# Comparing `tmp/lesscode_charts-0.0.2.tar.gz` & `tmp/lesscode_charts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.2.tar", last modified: Wed May 31 09:14:34 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.3.tar", last modified: Wed May 31 10:57:16 2023, max compression
```

## Comparing `lesscode_charts-0.0.2.tar` & `lesscode_charts-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.2/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.2/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.2/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.2/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.2/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.2/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     2106 2023-05-19 07:48:32.000000 lesscode_charts-0.0.2/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.2/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.2/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.2/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.2/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1911 2023-05-31 09:14:31.000000 lesscode_charts-0.0.2/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.2/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-31 09:14:31.000000 lesscode_charts-0.0.2/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-31 09:14:34.000000 lesscode_charts-0.0.2/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.2/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.3/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.3/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.3/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.3/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.3/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.3/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     2106 2023-05-19 07:48:32.000000 lesscode_charts-0.0.3/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.3/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1437 2023-05-19 03:41:10.000000 lesscode_charts-0.0.3/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.3/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.3/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 10:57:13.000000 lesscode_charts-0.0.3/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.3/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-05-31 10:57:13.000000 lesscode_charts-0.0.3/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-05-31 10:57:16.000000 lesscode_charts-0.0.3/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.3/setup.py
```

### Comparing `lesscode_charts-0.0.2/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.3/lesscode_charts/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/histogram_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/histogram_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/pie_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/pyramid_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/sankey_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/sankey_chart.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,40 @@
 class SankeyChart:
     @staticmethod
     def sankey(data: List[dict], title: str = "", data_key="id", parent_key="parent_id", **kwargs):
         """
         :param parent_key: 父级key
         :param data_key: 数据key
         :param title: 图题
-        :param data: 数据,示例：[{"id":"INB133001","title":"感知设备与服务","value":"value1","parent_id":"INB1330","depth":2},
-                                {"id":"INB1330","title":"感知设备","value":"value2","parent_id":None,"depth":1}]
+        :param data: 数据,示例：[{"id": "INB133001", "config": {"title": "感知设备与服务", "value": "value1", "depth": 2}, "parent_id": "INB1330"},
+                                {"id": "INB1330", "config": {"title": "感知设备", "value": "value2", "depth": 1}, "parent_id": None}]
         :return:
         """
         data_list = []
         link_list = []
         data_map = {item.get(data_key): item for item in data if item.get(data_key)}
         tmp = dict()
         for item in data:
             tmp.setdefault(item.get(parent_key), []).append(item)
         for parent_id, children in tmp.items():
             if parent_id:
                 for child in children:
-                    link_list.append(
-                        {"source": data_map.get(parent_id, {}).get(data_key), "target": child.get(data_key),
-                         "value": child.get("value")})
+                    link_info = {"source": data_map.get(parent_id, {}).get(data_key), "target": child.get(data_key)}
+                    value = child.get("config", {}).get("value")
+                    if value is not None:
+                        link_info.update({"value": value})
+                    link_list.append(link_info)
         for item in data:
             name = item.pop(data_key)
-            label = item.pop("title")
-            depth = item.pop("depth")
-            value = item.pop("value", name)
-            other = item.pop("other", {})
+            config = item.pop("config", {})
             info = {
-                "name": name,
-                "label": label,
-                "value": value,
-                "depth": depth
+                "name": name
             }
-            if other:
-                info.update(other)
+            if config:
+                info.update(config)
             data_list.append(info)
         result = {
             "series": [
                 {
                     "name": title,
                     "data": data_list,
                     "links": link_list
```

### Comparing `lesscode_charts-0.0.2/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.3/lesscode_charts/v1/table_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.3/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.2/setup.py` & `lesscode_charts-0.0.3/setup.py`

 * *Files identical despite different names*

