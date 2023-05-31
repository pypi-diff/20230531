# Comparing `tmp/docker-recipe-1.0.0.tar.gz` & `tmp/docker-recipe-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-recipe-1.0.0.tar", last modified: Tue May 30 11:10:32 2023, max compression
+gzip compressed data, was "docker-recipe-2.0.0.tar", last modified: Wed May 31 10:05:38 2023, max compression
```

## Comparing `docker-recipe-1.0.0.tar` & `docker-recipe-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-30 11:10:32.289110 docker-recipe-1.0.0/
--rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-1.0.0/LICENSE.md
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-30 11:10:32.288975 docker-recipe-1.0.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-1.0.0/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-30 11:10:32.287807 docker-recipe-1.0.0/docker_recipe/
--rw-r--r--   0 steve      (501) staff       (20)       23 2023-05-28 14:22:01.000000 docker-recipe-1.0.0/docker_recipe/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     1019 2023-05-29 21:40:33.000000 docker-recipe-1.0.0/docker_recipe/cli.py
--rw-r--r--   0 steve      (501) staff       (20)      314 2023-05-30 11:10:17.000000 docker-recipe-1.0.0/docker_recipe/data_structure.py
--rw-r--r--   0 steve      (501) staff       (20)      158 2023-05-29 21:39:21.000000 docker-recipe-1.0.0/docker_recipe/filters.py
--rw-r--r--   0 steve      (501) staff       (20)     1085 2023-05-29 21:40:12.000000 docker-recipe-1.0.0/docker_recipe/main.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-30 11:10:32.288803 docker-recipe-1.0.0/docker_recipe.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      379 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2023-05-30 11:10:32.000000 docker-recipe-1.0.0/docker_recipe.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-30 11:10:32.289145 docker-recipe-1.0.0/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-30 11:10:29.000000 docker-recipe-1.0.0/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-31 10:05:38.426602 docker-recipe-2.0.0/
+-rw-r--r--   0 steve      (501) staff       (20)    34893 2023-05-27 23:05:54.000000 docker-recipe-2.0.0/LICENSE.md
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-31 10:05:38.426462 docker-recipe-2.0.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      461 2023-05-27 23:05:54.000000 docker-recipe-2.0.0/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-31 10:05:38.425291 docker-recipe-2.0.0/docker_recipe/
+-rw-r--r--   0 steve      (501) staff       (20)       23 2023-05-28 14:22:01.000000 docker-recipe-2.0.0/docker_recipe/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      692 2023-05-31 09:26:49.000000 docker-recipe-2.0.0/docker_recipe/cli.py
+-rw-r--r--   0 steve      (501) staff       (20)      314 2023-05-30 11:10:17.000000 docker-recipe-2.0.0/docker_recipe/data_structure.py
+-rw-r--r--   0 steve      (501) staff       (20)      158 2023-05-29 21:39:21.000000 docker-recipe-2.0.0/docker_recipe/filters.py
+-rw-r--r--   0 steve      (501) staff       (20)     1060 2023-05-31 09:53:28.000000 docker-recipe-2.0.0/docker_recipe/main.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-31 10:05:38.426248 docker-recipe-2.0.0/docker_recipe.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      919 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      379 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       53 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)       43 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-05-31 10:05:38.000000 docker-recipe-2.0.0/docker_recipe.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-31 10:05:38.426645 docker-recipe-2.0.0/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-05-31 09:44:59.000000 docker-recipe-2.0.0/setup.py
```

### Comparing `docker-recipe-1.0.0/LICENSE.md` & `docker-recipe-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docker-recipe-1.0.0/PKG-INFO` & `docker-recipe-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 1.0.0
+Version: 2.0.0
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-1.0.0/docker_recipe/main.py` & `docker-recipe-2.0.0/docker_recipe/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 
     return output if output.endswith("\n") else output + "\n"
 
 
 def main():
     args = parser.parse_args()
 
-    with open(args.gitlab_ci_output_file, 'w+') as f_gitlab_ci:
-        f_gitlab_ci.write(render_file(args.gitlab_ci_template,
+    with open(args.output, 'w+') as f_gitlab_ci:
+        f_gitlab_ci.write(render_file(args.template,
                                       load_recipe(args.docker_recipe)))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `docker-recipe-1.0.0/docker_recipe.egg-info/PKG-INFO` & `docker-recipe-2.0.0/docker_recipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-recipe
-Version: 1.0.0
+Version: 2.0.0
 Summary: A way to cook multiple Dockerfiles
 Home-page: https://github.com/stephanmeijer/docker-recipe
 Author: Stephan Meijer
 Author-email: me@stephanmeijer.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `docker-recipe-1.0.0/setup.py` & `docker-recipe-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="docker-recipe",
-    version="1.0.0",
+    version="2.0.0",
     packages=find_packages(),
     install_requires=[
         'pydantic~=1.10.8',
         'PyYaml~=6.0',
         'Jinja2~=3.1.2',
     ],
     author="Stephan Meijer",
```

