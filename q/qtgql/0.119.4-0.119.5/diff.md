# Comparing `tmp/qtgql-0.119.4.tar.gz` & `tmp/qtgql-0.119.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.4.tar", max compression
+gzip compressed data, was "qtgql-0.119.5.tar", max compression
```

## Comparing `qtgql-0.119.4.tar` & `qtgql-0.119.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-30 11:23:46.511797 qtgql-0.119.4/LICENSE
--rw-r--r--   0        0        0     1805 2023-05-30 11:23:46.511797 qtgql-0.119.4/README.md
--rw-r--r--   0        0        0     4424 2023-05-30 11:24:04.336475 qtgql-0.119.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    12381 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3655 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2159 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      420 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17749 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10322 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     2998 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     4633 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     2086 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 11:12:45.006711 qtgql-0.119.5/LICENSE
+-rw-r--r--   0        0        0     1805 2023-05-31 11:12:45.006711 qtgql-0.119.5/README.md
+-rw-r--r--   0        0        0     4424 2023-05-31 11:13:08.919134 qtgql-0.119.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1761 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    12381 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3655 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2159 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      420 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17783 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10604 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     3047 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     4633 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3479 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-31 11:12:45.018711 qtgql-0.119.5/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.5/PKG-INFO
```

### Comparing `qtgql-0.119.4/LICENSE` & `qtgql-0.119.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/README.md` & `qtgql-0.119.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
 [Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
 - [x] object types, for each field there is a corresponding `Q_PROPERTY`
-- [ ] enums
+- [x] enums
 - [ ] custom scalars
 - [ ] Unions
 - [ ] interfaces
 - [ ] Garbage collection
 - [ ] Type-safe operation handlers
   - [x] Query.
   - [ ] Mutations.
```

### Comparing `qtgql-0.119.4/pyproject.toml` & `qtgql-0.119.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.4"
+version = "0.119.5"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.119.4/qtgqlcodegen/cli.py` & `qtgql-0.119.5/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.5/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.5/qtgqlcodegen/compiler/operation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.5/qtgqlcodegen/compiler/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/config.py` & `qtgql-0.119.5/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.5/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/introspection.py` & `qtgql-0.119.5/qtgqlcodegen/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,16 +336,16 @@
 
         if definition := self._enums_def_map.get(name, None):
             return definition
 
         ret = QtGqlEnumDefinition(
             name=name,
             members=[
-                EnumValue(name=name, description=val.description or "")
-                for name, val in enum.values.items()
+                EnumValue(name=enum.value, index=index, description=enum.description or "")
+                for index, enum in enumerate(enum.values.values())
             ],
         )
 
         self._enums_def_map[name] = ret
         return ret
 
     def parse_schema_concretes(self) -> None:
```

### Comparing `qtgql-0.119.4/qtgqlcodegen/objecttype.py` & `qtgql-0.119.5/qtgqlcodegen/objecttype.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 class QtGqlVariableDefinition(Generic[T], QtGqlBaseTypedNode):
     default_value: Optional[T] = UNSET
 
     def json_repr(self, attr_name: Optional[str] = None) -> str:
         if not attr_name:
             attr_name = self.name
         if self.type.is_input_object_type:
-            raise NotImplementedError
+            return f"{attr_name}.to_json()"
         elif self.type.is_builtin_scalar:
             return f"{attr_name}.value()"
-        elif self.type.is_enum:
-            raise NotImplementedError
+        elif enum_def := self.type.is_enum:
+            return f"Enums::{enum_def.map_name}[{attr_name}]"
         elif self.is_custom_scalar:
             raise NotImplementedError
 
         raise NotImplementedError(f"{self.type} is not supported as an input type ATM")
 
 
 @define(slots=False)
@@ -101,15 +101,15 @@
             # this would just generate the model without data.
             return "{}"
 
         if self.type.is_custom_scalar:
             return "{}"
 
         if enum_def := self.type.is_enum:
-            raise NotImplementedError
+            return f"{enum_def.namespaced_name}(0)"
 
         raise NotImplementedError
 
     @cached_property
     def fget_annotation(self) -> str:
         """This annotates the value that is QML-compatible."""
         if custom_scalar := self.type.is_custom_scalar:
@@ -207,22 +207,31 @@
 
 
 @define
 class EnumValue:
     """encapsulates enumValues from introspection, maps to an Enum member."""
 
     name: str
+    index: int
     description: str = ""
 
 
-@define
+@define(slots=False)
 class QtGqlEnumDefinition:
     name: str
     members: list[EnumValue]
 
+    @cached_property
+    def map_name(self) -> str:
+        return f"{self.name}EnumMap"
+
+    @cached_property
+    def namespaced_name(self) -> str:
+        return f"Enums::{self.name}"
+
 
 EnumMap = dict[str, "QtGqlEnumDefinition"]
 
 
 def freeze(self, key, value):  # pragma: no cover
     raise PermissionError("setattr called on frozen type")
 
@@ -312,16 +321,16 @@
 
         # int, str, float etc...
         if builtin_scalar := t_self.is_builtin_scalar:
             return builtin_scalar.tp
 
         if scalar := t_self.is_custom_scalar:
             return scalar.type_name
-        if gql_enum := t_self.is_enum:
-            return gql_enum.name
+        if enum_def := t_self.is_enum:
+            return enum_def.namespaced_name
         if model_of := t_self.is_model:
             # map of instances based on operation hash.
             return f"QMap<QUuid, QList<{model_of.member_type}>>"
         if object_def := t_self.is_object_type or t_self.is_interface:
             return f"std::shared_ptr<{object_def.name}>"
         if q_object_def := t_self.is_queried_object_type:
             return f"{q_object_def.name}"
```

### Comparing `qtgql-0.119.4/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.5/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.5/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.5/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 {% endif %}
 {% elif f.type.is_builtin_scalar -%}
 👉 assign_to 👈 = data.value("👉f.name👈").👉 f.type.is_builtin_scalar.from_json_convertor 👈;
 {% elif f.is_custom_scalar -%}
 👉 assign_to 👈 = 👉 f.is_custom_scalar.type_name 👈();
 👉 assign_to 👈.deserialize(data.value("👉f.name👈"));
 {% elif f.type.is_enum -%}
-👉 assign_to 👈 = 👉f.type.is_enum.name👈[field_data];
+👉 assign_to 👈 = Enums::👉f.type.is_enum.map_name👈::by_name(data.value("👉f.name👈").toString());
 {% elif f.type.is_union -%}
 type_name = field_data['__typename']
 choice = inner_config.choices[type_name]
 👉 assign_to 👈 = __TYPE_MAP__[type_name].from_dict(parent, field_data, choice, metadata);
 {% endif -%}
 };
 {%- endmacro %}
```

### Comparing `qtgql-0.119.4/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.5/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.5/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,48 @@
 
 #include <qtgql/bases/bases.hpp>
 {% for dep in context.dependencies -%}
 👉 dep 👈
 {% endfor %}
 
 namespace 👉 context.config.env_name 👈{
+{% if context.enums %}
+// ---------- Enums ----------
 
-// ----------- Object Types -----------
+class Enums{
+    Q_GADGET
+
+public:
+{% for enum in context.enums %}
+enum 👉enum.name👈{
+{% for member in enum.members -%}
+👉member.name👈 = 👉member.index👈,
+{% endfor %}
+};
+Q_ENUM(👉enum.name👈)
+struct 👉enum.map_name👈{
+Q_GADGET
+public:
+inline static const std::vector<std::pair<QString, 👉enum.name👈>> members = {
+        {% for member in enum.members -%}
+        {"👉member.name👈", 👉enum.name👈::👉member.name👈},
+        {% endfor %}
+};
+    GraphQLEnum_MACRO(👉enum.name👈)
+};
+
+{% endfor %}
+};
+{% endif %}
+
+// ---------- Object Types ----------
 {% for type in context.types %}
 {%- set base_class -%}{% if type.has_id_field %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
 class 👉 type.name 👈 : public qtgql::bases::👉 base_class 👈{
+Q_OBJECT
 protected:
 static auto & INST_STORE() {
     static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 
 👉 macros.concrete_type_fields(type) 👈
@@ -57,8 +86,36 @@
 void loose(const qtgql::bases::OperationMetadata &metadata){throw "not implemented";};
 void update(const QJsonObject &data,
             const qtgql::bases::SelectionsConfig &selections){throw "not implemented";};
 
 };
 {% endfor %}
 
+// ----------------------------------------- INPUT OBJECTS -----------------------------------------
+
+{% for type in context.input_objects %}
+/*
+ * 👉 type.docstring 👈
+ */
+
+struct 👉type.name👈: QObject{
+{% for f in type.fields %}
+👉f.annotation👈 m_👉f.name👈;
+{% endfor -%}
+
+👉type.name👈(QObject* parent, {% for f in type.fields %} 👉f.name👈: 👉f.annotation👈 {% endfor %}): QObject::QObject(parent){
+    {% for f in type.fields %}
+    m_👉f.name👈 = 👉f.name👈;
+    {% endfor -%}
+};
+QJsonObject to_json(){
+    ret = {}
+    {% for f in type.fields %}{% set attr_name %}self.👉f.name👈{% endset %}
+    if 👉attr_name👈:
+    ret['👉f.name👈'] = 👉f.json_repr(attr_name)👈
+    {% endfor %}
+    return ret
+};
+}
+{% endfor %}
+
 }
```

### Comparing `qtgql-0.119.4/qtgqlcodegen/utils.py` & `qtgql-0.119.5/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.4/PKG-INFO` & `qtgql-0.119.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.4
+Version: 0.119.5
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -38,15 +38,15 @@
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
 [Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
 - [x] object types, for each field there is a corresponding `Q_PROPERTY`
-- [ ] enums
+- [x] enums
 - [ ] custom scalars
 - [ ] Unions
 - [ ] interfaces
 - [ ] Garbage collection
 - [ ] Type-safe operation handlers
   - [x] Query.
   - [ ] Mutations.
```

