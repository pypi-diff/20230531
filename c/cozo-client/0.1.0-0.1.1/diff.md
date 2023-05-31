# Comparing `tmp/cozo_client-0.1.0.tar.gz` & `tmp/cozo_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozo_client-0.1.0.tar", last modified: Tue May 30 06:47:46 2023, max compression
+gzip compressed data, was "cozo_client-0.1.1.tar", last modified: Wed May 31 08:51:04 2023, max compression
```

## Comparing `cozo_client-0.1.0.tar` & `cozo_client-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-30 06:47:46.944797 cozo_client-0.1.0/
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-30 06:47:46.944672 cozo_client-0.1.0/PKG-INFO
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-30 06:47:46.943343 cozo_client-0.1.0/cozo_client/
--rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.0/cozo_client/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.0/cozo_client/_builder.py
--rw-r--r--   0 zh217      (501) staff       (20)    21781 2023-05-30 06:32:38.000000 cozo_client-0.1.0/cozo_client/_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-30 06:47:46.944503 cozo_client-0.1.0/cozo_client.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-30 06:47:46.000000 cozo_client-0.1.0/cozo_client.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      268 2023-05-30 06:47:46.000000 cozo_client-0.1.0/cozo_client.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-30 06:47:46.000000 cozo_client-0.1.0/cozo_client.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       32 2023-05-30 06:47:46.000000 cozo_client-0.1.0/cozo_client.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)       12 2023-05-30 06:47:46.000000 cozo_client-0.1.0/cozo_client.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)      520 2023-05-30 06:44:09.000000 cozo_client-0.1.0/pyproject.toml
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-30 06:47:46.944835 cozo_client-0.1.0/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.0/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.006130 cozo_client-0.1.1/
+-rw-r--r--   0 zh217      (501) staff       (20)     3098 2023-05-30 06:46:54.000000 cozo_client-0.1.1/.gitignore
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-31 08:51:04.005982 cozo_client-0.1.1/PKG-INFO
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.005055 cozo_client-0.1.1/cozo_client/
+-rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.1/cozo_client/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.1/cozo_client/_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    22427 2023-05-31 08:19:07.000000 cozo_client-0.1.1/cozo_client/_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.005782 cozo_client-0.1.1/cozo_client.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      296 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       41 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       12 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      535 2023-05-31 08:08:04.000000 cozo_client-0.1.1/pyproject.toml
+-rw-r--r--   0 zh217      (501) staff       (20)       40 2023-05-31 08:07:55.000000 cozo_client-0.1.1/requirements.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-31 08:51:04.006177 cozo_client-0.1.1/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.1/setup.py
```

### Comparing `cozo_client-0.1.0/cozo_client/_builder.py` & `cozo_client-0.1.1/cozo_client/_builder.py`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.0/cozo_client/_client.py` & `cozo_client-0.1.1/cozo_client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,36 @@
                 for k, v in row.to_dict().items():
                     if k not in ('ids', 'id'):
                         new_row[k] = v[i]
                 yield new_row
 
         return self.flatmap(generic_unbatch)
 
+    def save_as_spreadsheet(self, filename: str):
+        from openpyxl import Workbook
+        from openpyxl.styles import Font
+
+        wb = Workbook()
+        ws = wb.active
+        ws.append(self.headers)
+        for row in self.rows:
+            nr = []
+            for v in row:
+                if isinstance(v, str) or isinstance(v, int) or isinstance(v, float):
+                    nr.append(v)
+                else:
+                    nr.append(json.dumps(v, ensure_ascii=False))
+            ws.append(nr)
+
+        bold_font = Font(bold=True)
+        for cell in ws["1:1"]:
+            cell.font = bold_font
+
+        wb.save(filename)
+
 
 class CozoRow(BaseModel):
     headers: list[str]
     row: list[Any]
 
     def _repr_html_(self):
         html_str = ["<table>", "<tbody>"]
```

