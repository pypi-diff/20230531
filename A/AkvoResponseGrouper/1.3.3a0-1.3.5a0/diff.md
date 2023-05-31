# Comparing `tmp/AkvoResponseGrouper-1.3.3a0.tar.gz` & `tmp/AkvoResponseGrouper-1.3.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoResponseGrouper-1.3.3a0.tar", last modified: Mon May 22 14:15:01 2023, max compression
+gzip compressed data, was "AkvoResponseGrouper-1.3.5a0.tar", last modified: Wed May 31 13:58:44 2023, max compression
```

## Comparing `AkvoResponseGrouper-1.3.3a0.tar` & `AkvoResponseGrouper-1.3.5a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.648979 AkvoResponseGrouper-1.3.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-22 14:15:01.648979 AkvoResponseGrouper-1.3.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 14:15:01.648979 AkvoResponseGrouper-1.3.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.640978 AkvoResponseGrouper-1.3.3a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.644978 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.644978 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/checker_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/response_grouper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.648979 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.644978 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 14:15:01.000000 AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:15:01.648979 AkvoResponseGrouper-1.3.3a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/tests/test_category_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/tests/test_category_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-22 14:14:43.000000 AkvoResponseGrouper-1.3.3a0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 13:58:44.904362 AkvoResponseGrouper-1.3.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.896362 AkvoResponseGrouper-1.3.5a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/checker_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/response_grouper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 13:58:44.000000 AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:58:44.900362 AkvoResponseGrouper-1.3.5a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/tests/test_category_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/tests/test_category_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-31 13:58:27.000000 AkvoResponseGrouper-1.3.5a0/tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.3.3a0/LICENSE` & `AkvoResponseGrouper-1.3.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/PKG-INFO` & `AkvoResponseGrouper-1.3.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.3a0
+Version: 1.3.5a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.3a0/README.md` & `AkvoResponseGrouper-1.3.5a0/README.md`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/setup.py` & `AkvoResponseGrouper-1.3.5a0/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/checker.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,16 +141,17 @@
 
 
 def check_config(file_config: str, info: bool = True):
     with open(file_config) as f:
         data = f.read()
         data = json.loads(data)
     errors = []
-    items = []
+    duplicates = []
     for config in data:
+        items = []
         qs = []
         cname = config.get("name")
         errors += find_errors_in_config(config=config, name=cname)
 
         if "form" in config and "categories" in config:
             for c in config["categories"]:
                 find_errors_in_questions(
@@ -159,14 +160,15 @@
                 qs = get_all_questions(config=c, form=config["form"], qs=qs)
                 items.append(
                     {
                         "form": config["form"],
                         "questions": qs,
                     }
                 )
-    duplicates = get_potential_duplicates(items=items)
+        # move duplicates check inside each config
+        duplicates += get_potential_duplicates(items=items)
     questions = [i["questions"] for i in items]
     errors = get_error_messages(errors=errors)
     if info:
         for error in errors:
             print(error, "\n=============================")
     return errors, questions, duplicates
```

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/checker_db.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/checker_db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/generate_schema.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/generate_schema.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/cli/migrate.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/db.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/models.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/models.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/routes.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/routes.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/conftest.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     group_by_category_output,
     get_intersection,
     generate_data_as_json_file,
     get_valid_list,
     flatten_list,
     validate_number,
     get_counted_category,
+    transform_categories_to_df,
 )
 
 """
 A test case for utils with pytest
 """
 
 
@@ -148,7 +149,23 @@
     ]
     df = pd.DataFrame(categories)
     grouped = get_counted_category(df=df)
     assert grouped == [
         {"category": "Basic", "count": 1, "form": 1, "name": "Water"},
         {"category": "Limited", "count": 1, "form": 1, "name": "Water"},
     ]
+
+
+def test_empty_transform_categories_to_df():
+    categories = [
+        {
+            "form": 1,
+            "data": 6,
+            "name": "Water",
+            "opt": {"567800083": ["Underconstruction"]},
+        }
+    ]
+    df = transform_categories_to_df(categories=categories)
+
+    # Assert that the column is empty
+    column = ["id", "data", "form", "name", "category"]
+    assert df[column].empty
```

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/utils.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,31 +109,37 @@
         if sorted(conditions) == sorted(validator):
             category = c["name"]
     if sorted(valid) == sorted(validator):
         category = c["name"]
     return category
 
 
-def get_category(opt: dict, file_path: str = "./.category.json"):
+def get_category(data: dict, file_path: str = "./.category.json"):
+    name = data["name"]
+    opt = data["opt"]
     with open(f"{file_path}") as config_file:
         configs = json.load(config_file)
     category = False
+    # filter config with data name (e.g. water == water)
+    configs = list(filter(
+        lambda x: x["name"].lower() == name.lower(), configs
+    ))
     for config in configs:
         for c in config["categories"]:
             category = get_valid_list(opt, c, category)
     return category
 
 
 def transform_categories_to_df(
     categories: list, file_path: str = "./.category.json"
 ):
     df = pd.DataFrame(categories)
     results = df.to_dict("records")
     for d in results:
-        d.update({"category": get_category(opt=d["opt"], file_path=file_path)})
+        d.update({"category": get_category(data=d, file_path=file_path)})
     res = pd.DataFrame(results)
     if list(res) != ["id", "data", "form", "name", "opt", "category"]:
         return pd.DataFrame(
             columns=[
                 "id",
                 "data",
                 "form",
```

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper/views.py` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper/views.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/PKG-INFO` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.3a0
+Version: 1.3.5a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.3a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt` & `AkvoResponseGrouper-1.3.5a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/tests/test_category_checker.py` & `AkvoResponseGrouper-1.3.5a0/tests/test_category_checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.3a0/tests/test_category_data_frame.py` & `AkvoResponseGrouper-1.3.5a0/tests/test_category_data_frame.py`

 * *Files identical despite different names*

