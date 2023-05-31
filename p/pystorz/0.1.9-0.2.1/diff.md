# Comparing `tmp/pystorz-0.1.9.tar.gz` & `tmp/pystorz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.1.9.tar", last modified: Mon May  1 22:03:25 2023, max compression
+gzip compressed data, was "dist/pystorz-0.2.1.tar", last modified: Wed May 31 04:18:32 2023, max compression
```

## Comparing `pystorz-0.1.9.tar` & `pystorz-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.124302 pystorz-0.1.9/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.9/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-01 22:03:25.123921 pystorz-0.1.9/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.1.9/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.112924 pystorz-0.1.9/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.9/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.114022 pystorz-0.1.9/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.9/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      334 2023-04-29 21:02:22.000000 pystorz-0.1.9/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.115462 pystorz-0.1.9/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.9/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.9/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     6231 2023-04-29 19:33:35.000000 pystorz-0.1.9/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.117802 pystorz-0.1.9/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.9/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.9/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.1.9/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.9/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.9/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.118292 pystorz-0.1.9/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.9/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)    11623 2023-05-01 21:54:00.000000 pystorz-0.1.9/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.121893 pystorz-0.1.9/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.9/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.1.9/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4437 2023-04-27 06:31:29.000000 pystorz-0.1.9/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2997 2023-04-29 20:57:56.000000 pystorz-0.1.9/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.1.9/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-01 22:03:25.113732 pystorz-0.1.9/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-01 22:03:25.000000 pystorz-0.1.9/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-05-01 22:03:25.000000 pystorz-0.1.9/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-05-01 22:03:25.000000 pystorz-0.1.9/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-05-01 22:03:25.000000 pystorz-0.1.9/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-05-01 22:03:25.000000 pystorz-0.1.9/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-05-01 22:03:25.124370 pystorz-0.1.9/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-05-01 21:54:26.000000 pystorz-0.1.9/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.632314 pystorz-0.2.1/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.2.1/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-31 04:18:32.632111 pystorz-0.2.1/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.2.1/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.627784 pystorz-0.2.1/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.2.1/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.628843 pystorz-0.2.1/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.2.1/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      334 2023-04-29 21:02:22.000000 pystorz-0.2.1/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.629597 pystorz-0.2.1/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.2.1/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.2.1/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.2.1/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.630790 pystorz-0.2.1/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.2.1/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.2.1/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.2.1/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.2.1/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.2.1/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.631080 pystorz-0.2.1/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.2.1/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15702 2023-05-31 04:07:15.000000 pystorz-0.2.1/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.631872 pystorz-0.2.1/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.2.1/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.2.1/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     8681 2023-05-30 20:25:45.000000 pystorz-0.2.1/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2997 2023-05-30 20:27:50.000000 pystorz-0.2.1/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.2.1/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.628555 pystorz-0.2.1/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-05-31 04:18:32.632365 pystorz-0.2.1/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-05-31 04:08:02.000000 pystorz-0.2.1/setup.py
```

### Comparing `pystorz-0.1.9/LICENSE` & `pystorz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/PKG-INFO` & `pystorz-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.9/README.md` & `pystorz-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/mgen/builder.py` & `pystorz-0.2.1/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/mgen/loader.py` & `pystorz-0.2.1/pystorz/mgen/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,17 @@
             return "dict"
         if self.IsArray():
             return "list"
         if self.type == "string":
             return "str"
         return self.type
 
+    def ComplexTypeValueDefault(self):
+        return complexTypeValueDefault(self.type)
+
     def StrippedDefault(self):
         return typeDefault(self.StrippedType())
 
 
 class Struct:
     def __init__(self, name, implements="", properties=[]):
         self.name = name
@@ -112,76 +115,91 @@
                 resources.append(Resource(m["name"], ext, intr, pkey))
                 continue
 
             raise Exception("unknown kind: {}".format(m["kind"]))
 
     errors = validate_model(structs, resources)
     if len(errors) > 0:
-        raise Exception('''model validation failed:
-    {}'''.format('''
-    '''.join(errors)))
+        raise Exception(
+            """model validation failed:
+    {}""".format(
+                """
+    """.join(
+                    errors
+                )
+            )
+        )
 
     return structs, resources
 
 
 def validate_model(structs, resources):
     errors = []
-    known_types = [
-        "string",
-        "int",
-        "float",
-        "bool",
-        "datetime"
-    ]
+    known_types = ["string", "int", "float", "bool", "datetime"]
 
     for s in structs:
         known_types.append(s.name)
 
     for s in structs:
         for p in s.properties:
             if p.IsArray():
                 elem_type = p.type[2:]
                 if elem_type not in known_types:
-                    errors.append("struct {} property {}: unknown type: {}".format(
-                        s.name, p.name, elem_type))
+                    errors.append(
+                        "struct {} property {}: unknown type: {}".format(
+                            s.name, p.name, elem_type
+                        )
+                    )
                 continue
 
             if p.IsMap():
                 # map[int]string
                 key_type = p.type[4:].split("]")[0]
                 val_type = p.type[4:].split("]")[1]
                 if key_type not in known_types:
-                    errors.append("struct {} property {}: unknown type: {}".format(
-                        s.name, p.name, elem_type))
+                    errors.append(
+                        "struct {} property {}: unknown type: {}".format(
+                            s.name, p.name, elem_type
+                        )
+                    )
                 if val_type not in known_types:
-                    errors.append("struct {} property {}: unknown type: {}".format(
-                        s.name, p.name, elem_type))
+                    errors.append(
+                        "struct {} property {}: unknown type: {}".format(
+                            s.name, p.name, elem_type
+                        )
+                    )
                 continue
-            
+
             if p.type not in known_types:
-                errors.append("struct {} property {}: unknown type: {}".format(
-                    s.name, p.name, p.type))
+                errors.append(
+                    "struct {} property {}: unknown type: {}".format(
+                        s.name, p.name, p.type
+                    )
+                )
 
     for r in resources:
         if r.external is None and r.internal is None:
             errors.append("resource {} has no internal and external".format(r.name))
             continue
 
         if r.external is not None:
             if r.external not in known_types:
-                errors.append("resource {} external: unknown type: {}".format(
-                    r.name, r.external))
+                errors.append(
+                    "resource {} external: unknown type: {}".format(r.name, r.external)
+                )
 
         if r.internal is not None:
             if r.internal not in known_types:
-                errors.append("resource {} internal: unknown type: {}".format(
-                    r.name, r.internal))
+                errors.append(
+                    "resource {} internal: unknown type: {}".format(r.name, r.internal)
+                )
 
     return errors
 
+
 def read_model(path: str):
     log.debug(f"reading model from {path}")
 
     with open(path, "r") as f:
         data = yaml.safe_load(f)
     return data
 
@@ -225,7 +243,23 @@
         return "0"
     if tp == "float":
         return "0.0"
     if tp == "datetime":
         return '"0001-01-01T00:00:00.000000Z"'
 
     return f"{tp}Factory()"
+
+
+def complexTypeValueDefault(tp: str) -> str:
+    log.debug(f"typeValueDefault: {tp}")
+
+    if tp.startswith("[]"):
+        return typeDefault(tp[2:])
+
+    if tp.startswith("map"):
+        closing_bracket_index = tp.find("]")
+        if closing_bracket_index == -1:
+            raise Exception("invalid map type: {}".format(tp))
+
+        return typeDefault(tp[closing_bracket_index + 1 :])
+
+    raise Exception("unknown type: {}".format(tp))
```

### Comparing `pystorz-0.1.9/pystorz/mgen/templates/structure.py` & `pystorz-0.2.1/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.2.1/pystorz/mgen/templates/unmarshall.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,27 +48,27 @@
 			
 			{% for prop in data.properties %}
 			if key == "{{prop.json}}":
 				{% if prop.IsArray() %}
 				res = {{ prop.default }}
 
 				for rw in rawValue:
-					ud = {{prop.StrippedDefault()}}
+					ud = {{ prop.ComplexTypeValueDefault() }}
 					if hasattr(ud, "FromDict"):
 						ud.FromDict(rw)
 					else:
 						ud = rw
 					res.append(ud)
 
 				self.{{prop.name}}_ = res
 				{% elif prop.IsMap() %}
 				res = {{ prop.default }}
 				
 				for rk, rw in rawValue.items():
-					ud = {{prop.StrippedDefault()}}
+					ud = {{prop.ComplexTypeValueDefault()}}
 					if hasattr(ud, "FromDict"):
 						ud.FromDict(rw)
 					else:
 						ud = rw
 					res[rk] = ud
 
 				self.{{prop.name}}_ = res
```

### Comparing `pystorz-0.1.9/pystorz/mgen/test.py` & `pystorz-0.2.1/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/mgen/utils.py` & `pystorz-0.2.1/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/sql/store.py` & `pystorz-0.2.1/pystorz/sql/store.py`

 * *Files 21% similar despite different names*

```diff
@@ -98,23 +98,25 @@
             raise Exception(constants.ErrNoSuchObject)
 
         if existing.PrimaryKey() != obj.PrimaryKey():
             # log.info("primary key changed from {} to {}".format(
             #     existing.PrimaryKey(), obj.PrimaryKey())
             # )
 
-            if existing.Metadata().Identity().Path() != obj.Metadata().Identity().Path():
+            if (
+                existing.Metadata().Identity().Path()
+                != obj.Metadata().Identity().Path()
+            ):
                 raise Exception(constants.ErrObjectIdentityMismatch)
-            
+
             # see if there is an object with the new primary key value
             target_identity = store.ObjectIdentity(
-                "{}/{}".format(
-                    existing.Metadata().Kind().lower(), obj.PrimaryKey())
+                "{}/{}".format(existing.Metadata().Kind().lower(), obj.PrimaryKey())
             )
-            
+
             target = None
             try:
                 target = self.Get(target_identity)
             except Exception as e:
                 pass
 
             if target is not None:
@@ -157,29 +159,48 @@
     def Delete(self, identity, *opt):
         log.info("delete {}".format(identity.Path()))
         copt = options.CommonOptionHolderFactory()
 
         for o in opt:
             o.ApplyFunction()(copt)
 
-        existing = self.Get(identity)
-        if existing is None:
-            raise Exception(constants.ErrNoSuchObject)
+        existing = None
+        if copt.filter is None:
+            existing = self.Get(identity)
+            if existing is None:
+                raise Exception(constants.ErrNoSuchObject)
 
         self.TestConnection()
 
         try:
             # Start a transaction
             self.DB.execute("BEGIN")
             cursor = self.DB.cursor()
 
-            self._removeIdentity(cursor, existing.Metadata().Identity().Path())
-            self._removeObject(
-                cursor, existing.PrimaryKey(), existing.Metadata().Kind()
-            )
+            if copt.filter is None:
+                self._removeIdentity(cursor, existing.Metadata().Identity().Path())
+                self._removeObject(
+                    cursor, existing.PrimaryKey(), existing.Metadata().Kind()
+                )
+            else:
+                clause = self._buildFilterClause(copt, identity)
+                keys = self._getObjectKeys(
+                    cursor,
+                    identity.Type(),
+                    clause)
+                
+                self._removeObjects(
+                    cursor,
+                    identity.Type(),
+                    clause)
+                
+                self._removeIdentities(
+                    cursor,
+                    identity.Type(),
+                    keys)
 
             self.DB.commit()
         except Exception as e:
             self.DB.rollback()
             raise e
 
     def Get(self, identity, *opt):
@@ -192,15 +213,15 @@
         self.TestConnection()
 
         cursor = self.DB.cursor()
 
         if identity.IsId():
             pkey, typ = self._getIdentity(cursor, identity.Path())
             return self._getObject(cursor, pkey, typ)
-        
+
         return self._getObject(cursor, identity.Key(), identity.Type())
 
     def List(self, identity, *opt):
         log.info("list {}".format(identity))
 
         if len(identity.Key()) > 0:
             raise Exception(constants.ErrInvalidPath)
@@ -214,32 +235,15 @@
         cursor = self.DB.cursor()
 
         query = """SELECT Object FROM Objects 
         WHERE Type = '{}'""".format(
             identity.Type()
         )
 
-        # pkey filter
-        if copt.key_filter is not None:
-            query += """
-            AND Pkey IN ('{}')""".format(
-                "', '".join(copt.key_filter)
-            )
-
-        # prop filter
-        if copt.prop_filter is not None:
-            obj = self.Schema.ObjectForKind(identity.Type())
-            if obj is None:
-                raise Exception(constants.ErrNoSuchObject)
-            if utils.object_path(obj, copt.prop_filter.key) is None:
-                raise Exception(constants.ErrInvalidFilter)
-            query = query + " AND json_extract(Object, '$.{}') = {}".format(
-                copt.prop_filter.key,
-                copt.prop_filter.value
-            )
+        query += self._buildFilterClause(copt, identity)
 
         if copt.order_by is not None and len(copt.order_by) > 0:
             query += """
             ORDER BY json_extract(Object, '$.{}')""".format(
                 copt.order_by
             )
             if copt.order_incremental is None or copt.order_incremental:
@@ -372,14 +376,53 @@
     def _removeObject(self, cursor, pkey, typ):
         query = """DELETE FROM Objects
         WHERE Pkey = '{}' AND Type = '{}'""".format(
             pkey, typ.lower()
         )
 
         self._do_query(cursor, query)
+    
+    def _getObjectKeys(self, cursor, typ, clause):
+        query = """SELECT Pkey FROM Objects
+        WHERE Type = '{}' {}""".format(
+            typ.lower(),
+            clause,
+        )
+
+        self._do_query(cursor, query)
+        rows = cursor.fetchall()
+        res = []
+        for row in rows:
+            res.append(row[0])
+        return res
+
+    def _removeIdentities(self, cursor, typ, keys):
+        batch_size = 100
+        for i in range(0, len(keys), batch_size):
+            batch = keys[i:i+batch_size]
+            clause = "Pkey IN ({})".format(
+                ",".join(["'{}'".format(k) for k in batch])
+            )
+
+            query = """DELETE FROM IdIndex
+                WHERE Type = '{}' AND {}""".format(
+                    typ.lower(),
+                    clause,
+                )
+
+            self._do_query(cursor, query)
+
+    def _removeObjects(self, cursor, typ, clause):
+        query = """DELETE FROM Objects
+        WHERE Type = '{}' {}""".format(
+            typ.lower(),
+            clause,
+        )
+
+        self._do_query(cursor, query)
 
     def _parseObjectRow(self, data, typ):
         return utils.unmarshal_object(data, self.Schema, typ)
 
     def _parseObjectRows(self, rows, typ):
         res = []
         for row in rows:
@@ -387,7 +430,93 @@
             res.append(self._parseObjectRow(data, typ))
         return res
 
     def _do_query(self, cursor, query):
         log.debug("running query: {}".format(query))
 
         cursor.execute(query)
+
+    def _buildFilterClause(self, copt, identity):
+        if copt.filter is None:
+            return ""
+
+        sample = self.Schema.ObjectForKind(identity.Type())
+        if sample is None:
+            raise Exception(constants.ErrNoSuchObject)
+
+        return """
+            AND ({})
+            """.format(
+            self._convertFilter(copt.filter, sample)
+        )
+
+    def _convertFilter(self, filterSetting, sample):
+        if isinstance(filterSetting, options._ListDeleteOption):
+            copt = options.CommonOptionHolderFactory()
+            filterSetting.ApplyFunction()(copt)
+            filterSetting = copt.filter
+
+        if isinstance(filterSetting, options.AndSetting):
+            return "( {} )".format(
+                " AND ".join(
+                    [self._convertFilter(f, sample) for f in filterSetting.filters]
+                )
+            )
+
+        if isinstance(filterSetting, options.OrSetting):
+            return "( {} )".format(
+                " OR ".join(
+                    [self._convertFilter(f, sample) for f in filterSetting.filters]
+                )
+            )
+
+        if isinstance(filterSetting, options.NotSetting):
+            return "( NOT {} )".format(
+                self._convertFilter(filterSetting.filter, sample)
+            )
+
+        if utils.object_path(sample, filterSetting.key) is None:
+            raise Exception(constants.ErrInvalidFilter)
+
+        if isinstance(filterSetting, options.InSetting):
+
+            def convert_value(v):
+                # return "'{}'".format(v)
+                if isinstance(v, str):
+                    return "'{}'".format(v)
+                elif isinstance(v, bool):
+                    return str(v).lower()
+                else:
+                    return str(v)
+
+            values = ", ".join([convert_value(v) for v in filterSetting.values])
+
+            return " json_extract(Object, '$.{}') IN ({})".format(
+                filterSetting.key, values
+            )
+
+        if isinstance(filterSetting, options.EqSetting):
+            return " json_extract(Object, '$.{}') = {} ".format(
+                filterSetting.key, filterSetting.value
+            )
+
+        if isinstance(filterSetting, options.LtSetting):
+            return " json_extract(Object, '$.{}') < {} ".format(
+                filterSetting.key, filterSetting.value
+            )
+
+        if isinstance(filterSetting, options.GtSetting):
+            return " json_extract(Object, '$.{}') > {} ".format(
+                filterSetting.key, filterSetting.value
+            )
+
+        if isinstance(filterSetting, options.LteSetting):
+            return " json_extract(Object, '$.{}') <= {} ".format(
+                filterSetting.key, filterSetting.value
+            )
+
+        if isinstance(filterSetting, options.GteSetting):
+            return " json_extract(Object, '$.{}') >= {} ".format(
+                filterSetting.key, filterSetting.value
+            )
+
+        raise Exception(constants.ErrInvalidFilter)
```

### Comparing `pystorz-0.1.9/pystorz/store/meta.py` & `pystorz-0.2.1/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/store/store.py` & `pystorz-0.2.1/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz/store/utils.py` & `pystorz-0.2.1/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/pystorz.egg-info/PKG-INFO` & `pystorz-0.2.1/pystorz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.1.9/pystorz.egg-info/SOURCES.txt` & `pystorz-0.2.1/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.1.9/setup.py` & `pystorz-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.1.9',
+    version='0.2.1',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

