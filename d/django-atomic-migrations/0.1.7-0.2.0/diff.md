# Comparing `tmp/django-atomic-migrations-0.1.7.tar.gz` & `tmp/django-atomic-migrations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-atomic-migrations-0.1.7.tar", last modified: Tue May  4 07:09:41 2021, max compression
+gzip compressed data, was "django-atomic-migrations-0.2.0.tar", last modified: Wed May 31 07:39:49 2023, max compression
```

## Comparing `django-atomic-migrations-0.1.7.tar` & `django-atomic-migrations-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 07:09:41.582989 django-atomic-migrations-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     1552 2021-05-04 07:09:41.582989 django-atomic-migrations-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      803 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 07:09:41.578990 django-atomic-migrations-0.1.7/django_atomic_migrations/
--rw-r--r--   0 root         (0) root         (0)      989 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/django_atomic_migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 07:09:41.582989 django-atomic-migrations-0.1.7/django_atomic_migrations/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/django_atomic_migrations/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 07:09:41.582989 django-atomic-migrations-0.1.7/django_atomic_migrations/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/django_atomic_migrations/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      475 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/django_atomic_migrations/management/commands/add-migrations-constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 07:09:41.578990 django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2021-05-04 07:09:40.000000 django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2021-05-04 07:09:40.000000 django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-04 07:09:40.000000 django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-05-04 07:09:40.000000 django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-04 07:09:41.582989 django-atomic-migrations-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      707 2021-05-04 07:08:54.000000 django-atomic-migrations-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:39:49.824921 django-atomic-migrations-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-05-31 07:39:49.820922 django-atomic-migrations-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:39:49.812923 django-atomic-migrations-0.2.0/django_atomic_migrations/
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/django_atomic_migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:39:49.820922 django-atomic-migrations-0.2.0/django_atomic_migrations/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/django_atomic_migrations/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:39:49.820922 django-atomic-migrations-0.2.0/django_atomic_migrations/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/django_atomic_migrations/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/django_atomic_migrations/management/commands/add-migrations-constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:39:49.816922 django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-05-31 07:39:49.000000 django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-31 07:39:49.000000 django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 07:39:49.000000 django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-31 07:39:49.000000 django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 07:39:49.824921 django-atomic-migrations-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-31 07:39:03.000000 django-atomic-migrations-0.2.0/setup.py
```

### Comparing `django-atomic-migrations-0.1.7/PKG-INFO` & `django-atomic-migrations-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: django-atomic-migrations
-Version: 0.1.7
-Summary: Wraps migration step runs in transactions in Django
+Version: 0.2.0
+Summary: Adds unique constraint on Django's migration tracking model
 Home-page: https://github.com/rkojedzinszky/django-atomic-migrations
 Author: Richard Kojedzinszky
 Author-email: richard@kojedz.in
-License: UNKNOWN
-Description: # Django Atomic Migrations
-        
-        [![Build Status](https://drone.srv.kojedz.in/api/badges/krichy/django-atomic-migrations/status.svg)](https://drone.srv.kojedz.in/krichy/django-atomic-migrations)
-        
-        This small package ensures that Django's migration tracking model has an
-        unique index for applied migrations, and also ensures that migrations
-        steps are applied in transactions. This is known to work with
-        PostgreSQL.
-        
-        ## Usage
-        
-        Install the package:
-        ```bash
-        $ pip install django-atomic-migrations
-        ```
-        Then, add the application to `INSTALLED_APPS` in your Django project:
-        ```
-        INSTALLED_APPS = [
-        	...
-        	'django_atomic_migrations.AtomicMigrations',
-        	...
-        ]
-        ```
-        
-        If your project's database already exists, you should run
-        ```bash
-        $ python manage.py add-migrations-constraint
-        ```
-        to create the missing unique constraint.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Atomic Migrations
+
+[![Build Status](https://drone.srv.kojedz.in/api/badges/krichy/django-atomic-migrations/status.svg)](https://drone.srv.kojedz.in/krichy/django-atomic-migrations)
+
+This small package ensures that Django's migration tracking model has an
+unique index for applied migrations.
+
+[Django ticket](https://code.djangoproject.com/ticket/34610)
+
+## Usage
+
+Install the package:
+```bash
+$ pip install django-atomic-migrations
+```
+Then, add the application to `INSTALLED_APPS` in your Django project:
+```
+INSTALLED_APPS = [
+	...
+	'django_atomic_migrations.AtomicMigrations',
+	...
+]
+```
+
+If your project's database already exists, you should run
+```bash
+$ python manage.py add-migrations-constraint
+```
+to create the missing unique constraint.
```

### Comparing `django-atomic-migrations-0.1.7/README.md` & `django-atomic-migrations-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Django Atomic Migrations
 
 [![Build Status](https://drone.srv.kojedz.in/api/badges/krichy/django-atomic-migrations/status.svg)](https://drone.srv.kojedz.in/krichy/django-atomic-migrations)
 
 This small package ensures that Django's migration tracking model has an
-unique index for applied migrations, and also ensures that migrations
-steps are applied in transactions. This is known to work with
-PostgreSQL.
+unique index for applied migrations.
+
+[Django ticket](https://code.djangoproject.com/ticket/34610)
 
 ## Usage
 
 Install the package:
 ```bash
 $ pip install django-atomic-migrations
 ```
```

### Comparing `django-atomic-migrations-0.1.7/django_atomic_migrations.egg-info/PKG-INFO` & `django-atomic-migrations-0.2.0/django_atomic_migrations.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: django-atomic-migrations
-Version: 0.1.7
-Summary: Wraps migration step runs in transactions in Django
+Version: 0.2.0
+Summary: Adds unique constraint on Django's migration tracking model
 Home-page: https://github.com/rkojedzinszky/django-atomic-migrations
 Author: Richard Kojedzinszky
 Author-email: richard@kojedz.in
-License: UNKNOWN
-Description: # Django Atomic Migrations
-        
-        [![Build Status](https://drone.srv.kojedz.in/api/badges/krichy/django-atomic-migrations/status.svg)](https://drone.srv.kojedz.in/krichy/django-atomic-migrations)
-        
-        This small package ensures that Django's migration tracking model has an
-        unique index for applied migrations, and also ensures that migrations
-        steps are applied in transactions. This is known to work with
-        PostgreSQL.
-        
-        ## Usage
-        
-        Install the package:
-        ```bash
-        $ pip install django-atomic-migrations
-        ```
-        Then, add the application to `INSTALLED_APPS` in your Django project:
-        ```
-        INSTALLED_APPS = [
-        	...
-        	'django_atomic_migrations.AtomicMigrations',
-        	...
-        ]
-        ```
-        
-        If your project's database already exists, you should run
-        ```bash
-        $ python manage.py add-migrations-constraint
-        ```
-        to create the missing unique constraint.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Atomic Migrations
+
+[![Build Status](https://drone.srv.kojedz.in/api/badges/krichy/django-atomic-migrations/status.svg)](https://drone.srv.kojedz.in/krichy/django-atomic-migrations)
+
+This small package ensures that Django's migration tracking model has an
+unique index for applied migrations.
+
+[Django ticket](https://code.djangoproject.com/ticket/34610)
+
+## Usage
+
+Install the package:
+```bash
+$ pip install django-atomic-migrations
+```
+Then, add the application to `INSTALLED_APPS` in your Django project:
+```
+INSTALLED_APPS = [
+	...
+	'django_atomic_migrations.AtomicMigrations',
+	...
+]
+```
+
+If your project's database already exists, you should run
+```bash
+$ python manage.py add-migrations-constraint
+```
+to create the missing unique constraint.
```

### Comparing `django-atomic-migrations-0.1.7/setup.py` & `django-atomic-migrations-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-atomic-migrations",
-    version='0.1.7',
+    version='0.2.0',
     author="Richard Kojedzinszky",
     author_email="richard@kojedz.in",
-    description="Wraps migration step runs in transactions in Django",
+    description="Adds unique constraint on Django's migration tracking model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rkojedzinszky/django-atomic-migrations",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

