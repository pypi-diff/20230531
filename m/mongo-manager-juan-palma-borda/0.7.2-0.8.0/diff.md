# Comparing `tmp/mongo-manager-juan-palma-borda-0.7.2.tar.gz` & `tmp/mongo-manager-juan-palma-borda-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-manager-juan-palma-borda-0.7.2.tar", last modified: Thu Mar 30 10:45:18 2023, max compression
+gzip compressed data, was "mongo-manager-juan-palma-borda-0.8.0.tar", last modified: Tue May 30 10:37:10 2023, max compression
```

## Comparing `mongo-manager-juan-palma-borda-0.7.2.tar` & `mongo-manager-juan-palma-borda-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.918344 mongo-manager-juan-palma-borda-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.918344 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.918344 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/entity/objeto_mongo_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/mongo_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/mongo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/patrones/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/patrones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/patrones/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-30 10:44:56.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/repository/repository_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:45:18.922344 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-30 10:45:18.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-30 10:45:18.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:45:18.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 10:45:18.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 10:45:18.000000 mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.243249 mongo-manager-juan-palma-borda-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-30 10:37:10.243249 mongo-manager-juan-palma-borda-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 10:37:10.243249 mongo-manager-juan-palma-borda-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/aggregations/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/entity/objeto_mongo_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/mongo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/mongo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/patrones/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/patrones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/patrones/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.239249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-30 10:36:51.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/repository/repository_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:37:10.243249 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-30 10:37:10.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 10:37:10.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:37:10.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 10:37:10.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 10:37:10.000000 mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/top_level.txt
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/LICENSE` & `mongo-manager-juan-palma-borda-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.7.2/LICENSE.txt` & `mongo-manager-juan-palma-borda-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.7.2/PKG-INFO` & `mongo-manager-juan-palma-borda-0.8.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: mongo-manager-juan-palma-borda
-Version: 0.7.2
-Summary: Libreria para manejar objetos almacenados en MongoDB, usando la referencia de los CRUDRepository de SpringBoot
-Home-page: https://github.com/muerterauda/mongo_manager
-Author: Juan Palma Borda
-Author-email: juanpalmaborda@hotmail.com
-Project-URL: Bug Tracker, https://github.com/muerterauda/mongo_manager/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
-# Mongo Manager (0.7.2)
+# Mongo Manager (0.8.0)
 
 Libreria para el manejo de Objetos almacenados en base de datos MongoDB
 
 ## Clases
 
 ### MongoManager
 
@@ -29,21 +13,42 @@
 
 Clase abstracta en la que se representa un objeto mongo predefinido,
 su constructor recibe un object _id haciendo referencia al '_id' del
 objeto Mongo y **kwargs con los argumentos desechados por el
 constructor concreto de tu clase. Es recomendable llamar al contructor 
 padre para establecer los atributos.
 
+### Objetos internos
+
+En caso de tener objetos interno dentro del objeto principal es necesario
+reescribir las funciones internas get_dict y generar_object_from_dict de 
+forma que el objeto se transforme y destransforme en un diccionario.
+
+En caso de que el objeto o la lista de objetos internos hereden de la clase ObjetoMongoAbstract
+se puede modificar el metodo get_attr_nested_objects de la siguiente manera
+*{nombre_atributo: clase_atributo(aunque sea una lista)}* y automaticamente se instanciaran y desinstanciaran
+solos.
+
 ### RepositoryBase
 
 Repositorio base de mongo, recibe como parametros en el constructor,
 la coleccion a la que se hace referencia y el objeto al que va a convertir
 los resultados de las query que se realicen.
 
-## Ejemplo 
+En caso de querer usar una coleccion no perteneciente a la base de datos instanciada,
+se puede pasar el atributo *connection_collection* que debe ser una instancia de la conexion 
+MongoClient para la coleccion a tratar por el repositorio.
+
+### Aggregates
+
+Todavia no se han implementado ninguna clase que las trate a fondo, pero se pueden
+usar la mayoria de las *stages* y *operators* definidos en mongo_utils. Una vez definida la clase o 
+clases para tratar los Aggregates se compenetrara con estas funciones.
+
+## Ejemplo 1
 
 En este ejemplo veremos el uso de la libreria definiendo un objeto <i>Book</i> 
 que hereda de ObjetoMongoAbstract y para el que implementa un <i>RepositoryBook</i>
  para poder manejar el objeto de manera más comoda.
 
     class Book(ObjetoMongoAbstract):
             def __init__(self, name, id_mongo=None, **kwargs):
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/setup.cfg` & `mongo-manager-juan-palma-borda-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongo-manager-juan-palma-borda
-version = 0.7.2
+version = 0.8.0
 author = Juan Palma Borda
 author_email = juanpalmaborda@hotmail.com
 description = Libreria para manejar objetos almacenados en MongoDB, usando la referencia de los CRUDRepository de SpringBoot
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/muerterauda/mongo_manager
 project_urls =
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/setup.py` & `mongo-manager-juan-palma-borda-0.8.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongo-manager-juan-palma-borda",
-    version="0.7.2",
+    version="0.8.0",
     author='Juan Palma Borda',
     author_email='juanpalmaborda@hotmail.com',
     description='Libreria para manejar objetos almacenados en MongoDB, '
                 'usando la referencia de los CRUDRepository de SpringBoot',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url = "https://github.com/muerterauda/mongo_manager",
+    url="https://github.com/muerterauda/mongo_manager",
     project_urls={
         "Bug Tracker": "https://github.com/muerterauda/mongo_manager/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/entity/objeto_mongo_abstract.py` & `mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/entity/objeto_mongo_abstract.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,22 @@
         @return: dict with object variables, similar to vars(object)
         """
         d = vars(self).copy()
         if not id_mongo:
             d.pop('_id')
         elif id_as_string and self._id is not None:
             d['_id'] = str(self._id)
+        for x, y in self.get_attr_nested_objects().items():
+            obj = d.get(x, None)
+            if obj is None:
+                continue
+            if type(obj) is list:
+                d[x] = y.generar_list_dicts_from_list_objects(d[x], False, False)
+            else:
+                d[x] = d[x].get_dict(False, False)
         return d
 
     def get_dict_no_id(self) -> dict:
         """
         Fachade for get_dict(id_mongo=False). Return all variables from this object, similar to vars(object) with exception for _id
         @return: dict with object variables, similar to vars(object)
         """
@@ -58,16 +66,32 @@
         return json.dumps(ObjetoMongoAbstract.generar_list_dicts_from_list_objects(objetos, id_mongo=id_mongo,
                                                                                    id_as_string=True))
 
     @classmethod
     def generar_object_from_dict(cls, dictionary):
         if dictionary is None:
             return None
+        for x, y in cls.get_attr_nested_objects().items():
+            obj = dictionary.get(x, None)
+            if obj is None:
+                continue
+            if type(obj) is list:
+                dictionary[x] = y.generar_objects_from_list_dicts(obj)
+            else:
+                dictionary[x] = y.generar_object_from_dict(obj)
         return cls(**dictionary)
 
     @classmethod
     def generar_objects_from_list_dicts(cls, dictionaries: list | Cursor):
         return [cls.generar_object_from_dict(dictionary) for dictionary in dictionaries]
 
     @staticmethod
     def generar_list_dicts_from_list_objects(lista_objetos: list, id_mongo=True, id_as_string=False):
         return [c.get_dict(id_mongo=id_mongo, id_as_string=id_as_string) for c in lista_objetos]
+
+    @staticmethod
+    def get_attr_nested_objects() -> dict:
+        """
+        Attributes which are objects of the class ObjetoMongoAbstract, all of them. Overrides parents methods.
+        @return: dict format {name_attr: class_attr}
+        """
+        return {}
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/mongo_manager.py` & `mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/mongo_manager.py`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/patrones/singleton.py` & `mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/patrones/singleton.py`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager/repository/repository_base.py` & `mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager/repository/repository_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from bson import ObjectId
 
 T_O = TypeVar('T_O', bound=ObjetoMongoAbstract)
 
 
 class RepositoryBase(Generic[T_O], metaclass=SingletonMeta):
 
-    def __init__(self, collection, clase: Type[T_O]) -> None:
+    def __init__(self, collection, clase: Type[T_O], connection_collection=None) -> None:
         __metaclass__ = SingletonMeta
-        from ..mongo_manager import _mongo_manager_gl as mongo_manager_gl
-        self.__collection = mongo_manager_gl.collection(collection)
+        if connection_collection is None:
+            from ..mongo_manager import _mongo_manager_gl as mongo_manager_gl
+            connection_collection = mongo_manager_gl.collection(collection)
+        self.__collection = connection_collection
         self.__clase = clase
 
     @property
     def collection(self) -> pymongo.collection.Collection:
         """
         @return: Pymongo collection | Coleccion Pymongo
         """
```

### Comparing `mongo-manager-juan-palma-borda-0.7.2/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt` & `mongo-manager-juan-palma-borda-0.8.0/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/mongo_manager/__init__.py
 src/mongo_manager/mongo_manager.py
 src/mongo_manager/mongo_utils.py
+src/mongo_manager/aggregations/__init__.py
+src/mongo_manager/aggregations/aggregation.py
 src/mongo_manager/entity/__init__.py
 src/mongo_manager/entity/objeto_mongo_abstract.py
 src/mongo_manager/patrones/__init__.py
 src/mongo_manager/patrones/singleton.py
 src/mongo_manager/repository/__init__.py
 src/mongo_manager/repository/repository_base.py
 src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO
```

