# Comparing `tmp/pypendency-0.4.0.tar.gz` & `tmp/pypendency-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypendency-0.4.0.tar", last modified: Thu May 25 07:25:02 2023, max compression
+gzip compressed data, was "dist/pypendency-0.5.0.tar", last modified: Wed May 31 15:37:23 2023, max compression
```

## Comparing `pypendency-0.4.0.tar` & `pypendency-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 07:25:02.000000 pypendency-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-25 07:24:49.000000 pypendency-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:25:02.000000 pypendency-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 07:24:49.000000 pypendency-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/on_container_resolved_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/types/python_loadable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-31 15:37:23.000000 pypendency-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-31 15:37:13.000000 pypendency-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:37:23.000000 pypendency-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-31 15:37:13.000000 pypendency-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/pypendency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/pypendency/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/loaders/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/loaders/py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/on_container_resolved_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/pypendency/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 15:37:13.000000 pypendency-0.5.0/src/pypendency/types/python_loadable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/pypendency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-31 15:37:22.000000 pypendency-0.5.0/src/pypendency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 15:37:23.000000 pypendency-0.5.0/src/pypendency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:37:22.000000 pypendency-0.5.0/src/pypendency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 15:37:22.000000 pypendency-0.5.0/src/pypendency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 15:37:22.000000 pypendency-0.5.0/src/pypendency.egg-info/top_level.txt
```

### Comparing `pypendency-0.4.0/PKG-INFO` & `pypendency-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.4.0
+Version: 0.5.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Fever - Platform Squad
 Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
```

### Comparing `pypendency-0.4.0/README.md` & `pypendency-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pypendency-0.4.0/setup.py` & `pypendency-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as readme:
     README = readme.read()
 
 
 setup(
     name='pypendency',
-    version='0.4.0',
+    version='0.5.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     author='Fever - Platform Squad',
     author_email='platform@feverup.com',
     description='A dependency injection tool for python',
     long_description=README,
     long_description_content_type='text/markdown',
```

### Comparing `pypendency-0.4.0/src/pypendency/builder.py` & `pypendency-0.5.0/src/pypendency/builder.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.4.0/src/pypendency/container.py` & `pypendency-0.5.0/src/pypendency/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,47 +69,23 @@
             raise exceptions.ServiceAlreadyDefined(identifier)
 
         self._service_mapping.update({identifier: service})
         if tags is not None:
             for tag in tags:
                 self.__add_service_to_tag_group(tag, identifier)
 
+    def has(self, identifier: str) -> bool:
+        return identifier in self._service_mapping
+
     def get(self, identifier: str) -> Optional[object]:
         if self.is_resolved() is False:
             self.resolve()
 
         return self._do_get(identifier)
 
-    def get_by_tag(self, tag: Tag) -> Set[object]:
-        if self.is_resolved() is False:
-            self.resolve()
-
-        if tag not in self._tags_mapping:
-            raise exceptions.TagNotFoundInContainer(tag.identifier)
-
-        return set([self._do_get(service) for service in self._tags_mapping[tag]])
-
-    def get_by_tag_name(self, tag_identifier: str, tag_value: Optional[object] = Tag.UNSET_VALUE) -> Set[object]:
-        if self.is_resolved() is False:
-            self.resolve()
-
-        services = set()
-        for tag, tagged_services in self._tags_mapping.items():
-            if tag.identifier == tag_identifier and (tag_value == Tag.UNSET_VALUE or tag.value == tag_value):
-                for tagged_service in tagged_services:
-                    services.add(self._do_get(tagged_service))
-
-        return services
-
-    def get_service_tags(self, service_identifier: str) -> Set[Tag]:
-        if self.is_resolved() is False:
-            self.resolve()
-
-        return {tag for tag, services in self._tags_mapping.items() if service_identifier in services}
-
     def _do_get(self, identifier: str) -> Optional[object]:
         empty = object()
 
         service = self._service_mapping.get(identifier, empty)
 
         if service is empty:
             raise exceptions.ServiceNotFoundInContainer(identifier)
@@ -145,9 +121,58 @@
             raise exceptions.ServiceNotFoundFromFullyQualifiedName(fully_qualified_name)
 
         try:
             return klass(*args, **kwargs)
         except TypeError as e:
             raise exceptions.ServiceInstantiationFailed(fully_qualified_name) from e
 
-    def has(self, identifier: str) -> bool:
-        return identifier in self._service_mapping
+    def get_by_tag(self, tag: Tag) -> Set[object]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        if tag not in self._tags_mapping:
+            raise exceptions.TagNotFoundInContainer(tag.identifier)
+
+        return set([self._do_get(service) for service in self._tags_mapping[tag]])
+
+    def get_by_tag_name(self, tag_identifier: str, tag_value: Optional[object] = Tag.UNSET_VALUE) -> Set[object]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        services = set()
+        for tag, tagged_services in self._tags_mapping.items():
+            if tag.identifier == tag_identifier and (tag_value == Tag.UNSET_VALUE or tag.value == tag_value):
+                for tagged_service in tagged_services:
+                    services.add(self._do_get(tagged_service))
+
+        return services
+
+    def get_services_identifiers_by_tag_name(self, tag_identifier: str,
+                                             tag_value: Optional[object] = Tag.UNSET_VALUE) -> Set[str]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        if tag_value != Tag.UNSET_VALUE:
+            return self._do_get_services_identifiers_by_tag(Tag(identifier=tag_identifier, value=tag_value))
+
+        identifiers: Set[str] = set()
+        for tag, tagged_services in self._tags_mapping.items():
+            if tag.identifier == tag_identifier:
+                for service in tagged_services:
+                    identifiers.add(service)
+
+        if len(identifiers) == 0:
+            raise exceptions.TagNotFoundInContainer(tag_identifier)
+
+        return identifiers
+
+    def _do_get_services_identifiers_by_tag(self, tag: Tag) -> Set[str]:
+        if tag not in self._tags_mapping:
+            raise exceptions.TagNotFoundInContainer(tag.identifier)
+
+        return set(self._tags_mapping[tag])
+
+    def get_service_tags(self, service_identifier: str) -> Set[Tag]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        return {tag for tag, services in self._tags_mapping.items() if service_identifier in services}
```

### Comparing `pypendency-0.4.0/src/pypendency/exceptions.py` & `pypendency-0.5.0/src/pypendency/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Union
+
+from pypendency.definition import Definition
 from pypendency.tag import Tag
 
 
 class ContainerAlreadyResolved(Exception):
     def __init__(self):
         super().__init__("Container already resolved can't be resolved again")
 
@@ -30,21 +33,23 @@
 class ServiceNotFoundFromFullyQualifiedName(Exception):
     def __init__(self, fully_qualified_name: str):
         self.fully_qualified_name = fully_qualified_name
         super().__init__(
             f"Container can't locate any class in {fully_qualified_name}"
         )
 
+
 class ServiceInstantiationFailed(Exception):
     def __init__(self, service_fqn: str) -> None:
         self.service_fqn = service_fqn
         super().__init__(f"Type {service_fqn} cannot be instantiated by the container")
 
 
 class TagNotFoundInContainer(Exception):
     def __init__(self, tag_identifier: str) -> None:
         self.tag_identifier = tag_identifier
         super().__init__(f"The tag '{tag_identifier}' does not exist in the container")
 
+
 class PypendencyCallbackException(Exception):
     def __init__(self) -> None:
         super().__init__(f"Exception on_resolved_callback")
```

### Comparing `pypendency-0.4.0/src/pypendency/loaders/exceptions.py` & `pypendency-0.5.0/src/pypendency/loaders/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.4.0/src/pypendency/loaders/py_loader.py` & `pypendency-0.5.0/src/pypendency/loaders/py_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.4.0/src/pypendency/loaders/yaml_loader.py` & `pypendency-0.5.0/src/pypendency/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.4.0/src/pypendency.egg-info/PKG-INFO` & `pypendency-0.5.0/src/pypendency.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.4.0
+Version: 0.5.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Fever - Platform Squad
 Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
```

### Comparing `pypendency-0.4.0/src/pypendency.egg-info/SOURCES.txt` & `pypendency-0.5.0/src/pypendency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

