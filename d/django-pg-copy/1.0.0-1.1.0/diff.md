# Comparing `tmp/django-pg-copy-1.0.0.tar.gz` & `tmp/django-pg-copy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-pg-copy-1.0.0.tar", last modified: Tue Aug 30 14:22:47 2022, max compression
+gzip compressed data, was "/var/www-dev/tallen/django-pg-copy/dist/.tmp-n_c0cs54/django-pg-copy-1.1.0.tar", last modified: Wed May 31 14:42:54 2023, max compression
```

## Comparing `django-pg-copy-1.0.0.tar` & `django-pg-copy-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.315385 django-pg-copy-1.0.0/
--rw-------   0 tallen   (86646) wrds     (60359)      581 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/.gitignore
--rw-------   0 tallen   (86646) wrds     (60359)     1539 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/LICENSE
--rw-------   0 tallen   (86646) wrds     (60359)     8947 2022-08-30 14:22:47.315385 django-pg-copy-1.0.0/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)     7028 2022-08-30 14:18:39.000000 django-pg-copy-1.0.0/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.314385 django-pg-copy-1.0.0/django_pg_copy.egg-info/
--rw-------   0 tallen   (86646) wrds     (60359)     8947 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)      504 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/not-zip-safe
--rw-------   0 tallen   (86646) wrds     (60359)       13 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/requires.txt
--rw-------   0 tallen   (86646) wrds     (60359)        8 2022-08-30 14:22:47.000000 django-pg-copy-1.0.0/django_pg_copy.egg-info/top_level.txt
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.314385 django-pg-copy-1.0.0/pg_copy/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)       88 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/apps.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.315385 django-pg-copy-1.0.0/pg_copy/management/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/management/__init__.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.315385 django-pg-copy-1.0.0/pg_copy/management/commands/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/management/commands/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)     3835 2022-08-30 14:04:56.000000 django-pg-copy-1.0.0/pg_copy/management/commands/pg_backup.py
--rw-------   0 tallen   (86646) wrds     (60359)     5267 2022-08-30 14:04:52.000000 django-pg-copy-1.0.0/pg_copy/management/commands/pg_restore.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2022-08-30 14:22:47.315385 django-pg-copy-1.0.0/pg_copy/migrations/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/migrations/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)      235 2022-01-19 22:06:47.000000 django-pg-copy-1.0.0/pg_copy/settings.py
--rw-------   0 tallen   (86646) wrds     (60359)       38 2022-08-30 14:22:47.316385 django-pg-copy-1.0.0/setup.cfg
--rw-------   0 tallen   (86646) wrds     (60359)     1248 2022-08-30 14:14:12.000000 django-pg-copy-1.0.0/setup.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.213532 django-pg-copy-1.1.0/
+-rw-------   0 tallen   (86646) wrds     (60359)      581 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/.gitignore
+-rw-------   0 tallen   (86646) wrds     (60359)     1539 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/LICENSE
+-rw-------   0 tallen   (86646) wrds     (60359)     8355 2023-05-31 14:42:54.213532 django-pg-copy-1.1.0/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)     7143 2023-05-31 14:21:15.000000 django-pg-copy-1.1.0/README.md
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.211532 django-pg-copy-1.1.0/django_pg_copy.egg-info/
+-rw-------   0 tallen   (86646) wrds     (60359)     8355 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/django_pg_copy.egg-info/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)      493 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/django_pg_copy.egg-info/SOURCES.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/django_pg_copy.egg-info/dependency_links.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       13 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/django_pg_copy.egg-info/requires.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        8 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/django_pg_copy.egg-info/top_level.txt
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.212532 django-pg-copy-1.1.0/pg_copy/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)      160 2023-05-31 14:42:54.000000 django-pg-copy-1.1.0/pg_copy/_version.py
+-rw-------   0 tallen   (86646) wrds     (60359)       88 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/apps.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.212532 django-pg-copy-1.1.0/pg_copy/management/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/management/__init__.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.212532 django-pg-copy-1.1.0/pg_copy/management/commands/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/management/commands/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)     4072 2023-05-31 14:18:06.000000 django-pg-copy-1.1.0/pg_copy/management/commands/pg_backup.py
+-rw-------   0 tallen   (86646) wrds     (60359)     5557 2023-05-31 14:17:33.000000 django-pg-copy-1.1.0/pg_copy/management/commands/pg_restore.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-05-31 14:42:54.213532 django-pg-copy-1.1.0/pg_copy/migrations/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/migrations/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)      235 2022-01-19 22:06:47.000000 django-pg-copy-1.1.0/pg_copy/settings.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1381 2023-05-31 14:29:06.000000 django-pg-copy-1.1.0/pyproject.toml
+-rw-------   0 tallen   (86646) wrds     (60359)       38 2023-05-31 14:42:54.213532 django-pg-copy-1.1.0/setup.cfg
```

### Comparing `django-pg-copy-1.0.0/.gitignore` & `django-pg-copy-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django-pg-copy-1.0.0/LICENSE` & `django-pg-copy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pg-copy-1.0.0/PKG-INFO` & `django-pg-copy-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,154 @@
 Metadata-Version: 2.1
 Name: django-pg-copy
-Version: 1.0.0
-Summary: UNKNOWN
-Home-page: https://github.com/FlipperPA/django-pg-copy
-Author: Tim Allen
-Author-email: tallen@wharton.upenn.edu
-License: UNKNOWN
-Description: # Django PostgreSQL Copy
-        
-        The package `django-pg-copy` provides Django management commands for backing up and restoring PostgreSQL databases. These were developed for copying production databases to development, to allow developers to share images with one another, or bring local development databases up to date. It can also be handy for creating different local databases for different branches, and for only creating one migration after tweaking models to get them the way they need to be.
-        
-        We also use it with Jenkins to automatically back up production, and restore to a staging database environment, so we can test new migrations repeatedly to ensure they'll work when we run them in production.
-        
-        ## Installation
-        
-        `pip install django-pg-copy`
-        
-        Then add `'pg_copy',` to your `INSTALLED_APPS` list. It is recommended that it is used in all environments (development, production) so that you can use it against different instances of your database.
-        
-        ## Settings
-        
-        `PG_COPY_BACKUP_PATH = 'db_backup'`
-        
-        By default, PostgreSQL backups will be stored in a directory called `db_backup` where you run the command. This setting will override that location.
-        
-        It is also recommended to add this path to your `.gitignore` file, if the path falls under your version control repository.
-        
-        ## Parameters
-        
-        * `--database`: The database defined in the DATABASES settings to backup from or restore to.
-        * `--db-override`: A value to override the db argument sent to psql.
-        * `--host-override`: A value to override the host argument sent to psql.
-        * `--pg-home`: The path to the PostgreSQL installation, if it is not on your path.
-        * `--file`, `-f`: The filename to backup to, or restore from.
-        * `--jobs`, `-j`: The number of parallel jobs to run. This can *drastically* increase the speed of the backup and restore. When backing up, this must use the `--directory` option. *Be careful!* This will also create multiple database connections and can slow your database down.
-        * `--directory`, `-d`: Restore from a directory. Overrides `--file` when used.
-        * `--ignore-table`, `-i`: Excludes the table completely during the backup file creation. Can pass multiple tables: `-i bigtable1 -i bigtable2`
-        * `--exclude-table-data`, `-e`: Excludes the table data during the backup file creation. Can pass multiple tables: `-e bigtable1 -e bigtable2`
-        * `--no-confirm`: Restores the database without confirmation: be careful! (**pg_restore** only)
-        
-        ## Example Commands
-        
-        `python manage.py pg_backup`
-        
-        This command will create a backup file in the directory `./db_backup/` (or the directory you specified with `PG_COPY_BACKUP_PATH`) called `[timestamp].sqlc` using the `default` settings from `DATABASES` using the default Django settings file resolved by `manage.py`.
-        
-        `python manage.py pg_backup --settings=config.settings.production --database=default --filename=my_backup.sqlc`
-        
-        This command will create a backup in the same directory as `manage.py` called `my_backup.sqlc` using the `default` settings from `DATABASES` using the Django settings file located at `config/settings/production.py`.
-        
-        `python manage.py pg_backup --directory=/tmp/pg_backup --jobs=8`
-        
-        This command will create a backup directory at `/tmp/backup` use 8 parallel jobs and database connections.
-        
-        `python manage.py pg_backup -i bigtable1 -i bigtable2`
-        
-        This will do the same as the previous command, but omit the tables named `bigtable1` and `bigtable2`.
-        
-        `python manage.py pg_backup -e bigtable1 -e bigtable2`
-        
-        This will do the same as the previous command, but include the table structure without any data for the tables named `bigtable1` and `bigtable2`.
-        
-        `python manage.py pg_restore`
-        
-        This command will provide a list of backup files in `PG_COPY_BACKUP_PATH` that can be restored. After selecting a backup file, it will confirm that the user wants to overwrite the destination database by showing which server and database will be overwritten from the settings. Here's what it will look like:
-        
-        ```bash
-        (venv) [django-project]$ ./manage.py pg_restore
-        There are 8 backup files in '/var/dev/username/django-project/db_backup'. Which would you like to restore?
-        1: 2020-05-27-13-33-38.sqlc
-        2: 2020-05-10-09-07-45.sqlc
-        3: 2020-05-11-13-05-49.sqlc
-        4: 2020-07-14-15-21-22.sqlc
-        5: 2020-05-15-08-31-59.sqlc
-        6: 2020-06-11-13-11-00.sqlc
-        7: 2020-06-02-13-28-09.sqlc
-        8: 2020-05-27-14-54-15.sqlc
-        Enter number of the file to restore: 4
-        About to restore 'django_project_db' on host 'localhost' from the file:
-        '/var/dev/username/django-project/db_backup/2020-07-14-15-21-22.sqlc'.
-        THIS WILL OVERWRITE THE DATABASE.
-        Type "yes" to start the restore [no]: yes
-        ```
-        
-        `python manage.py pg_restore --filename=my_file.sqlc --no-confirm`
-        
-        This command will read the file `my_file.sqlc` and **skip confirmation** that the user wants to overwrite the destination database.
-        
-        `python manage.py pg_restore --directory=/tmp/pg_backup --jobs=8`
-        
-        This command will restore from the directory `/tmp/pg_backup` using 8 parallel jobs and database connections.
-        
-        ## Known Issues
-        
-        #### Errors Displayed During `pg_restore`
-        
-        When restoring, PostgreSQL's `pg_restore` command may output some warnings and erorrs. I haven't figured out a command line option to make these warnings disappear, but they can likely be ignored if you read them. Here is an example of what these errors may look like:
-        
-        ```bash
-        pg_restore: [archiver (db)] Error while PROCESSING TOC:
-        pg_restore: [archiver (db)] Error from TOC entry 1; 3079 13792 EXTENSION plpgsql
-        pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of extension plpgsql
-            Command was: DROP EXTENSION IF EXISTS plpgsql;
-        
-        pg_restore: [archiver (db)] Error from TOC entry 6; 2615 2200 SCHEMA public postgres
-        pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of schema public
-            Command was: DROP SCHEMA IF EXISTS public;
-        
-        pg_restore: [archiver (db)] could not execute query: ERROR:  schema "public" already exists
-            Command was: CREATE SCHEMA public;
-        ```
-        
-        These may be errors from extensions that aren't used, or warnings about default schemata that already exist.
-        
-        ## Release Notes
-        
-        [Release notes are available on GitHub](https://github.com/FlipperPA/django-pg-copy/releases).
-        ## Maintainer
-        
-        * [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
-        
-        This package is maintained by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our package users.
-        
-        ## Contributors
-        
-        * Alex Malek (https://github.com/amalek215)
-        * Noel Victor (https://github.com/noeldvictor)
-        * Ryan Sullivan (https://github.com/rgs258)
-        
-Platform: UNKNOWN
+Version: 1.1.0
+Summary: Django management command to backup and restore PostgreSQL databases using the DATABASES settings.
+Author-email: Tim Allen <tallen@wharton.upenn.edu>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/FlipperPA/django-pg-copy
+Project-URL: Repository, https://github.com/FlipperPA/django-pg-copy
+Project-URL: Documentation, https://github.com/FlipperPA/django-pg-copy
+Keywords: postgres,postgresql,backup,restore,database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django PostgreSQL Copy
+
+The package `django-pg-copy` provides Django management commands for backing up and restoring PostgreSQL databases. These were developed for copying production databases to development, to allow developers to share images with one another, or bring local development databases up to date. It can also be handy for creating different local databases for different branches, and for only creating one migration after tweaking models to get them the way they need to be.
+
+We also use it with Jenkins to automatically back up production, and restore to a staging database environment, so we can test new migrations repeatedly to ensure they'll work when we run them in production.
+
+## Installation
+
+`pip install django-pg-copy`
+
+Then add `'pg_copy',` to your `INSTALLED_APPS` list. It is recommended that it is used in all environments (development, production) so that you can use it against different instances of your database.
+
+## Settings
+
+`PG_COPY_BACKUP_PATH = 'db_backup'`
+
+By default, PostgreSQL backups will be stored in a directory called `db_backup` where you run the command. This setting will override that location.
+
+It is also recommended to add this path to your `.gitignore` file, if the path falls under your version control repository.
+
+## Parameters
+
+* `--database`: The database defined in the DATABASES settings to backup from or restore to.
+* `--db-override`: A value to override the db argument sent to psql.
+* `--host-override`: A value to override the host argument sent to psql.
+* `--pg-home`: The path to the PostgreSQL installation, if it is not on your path.
+* `--file`, `-f`: The filename to backup to, or restore from.
+* `--jobs`, `-j`: The number of parallel jobs to run. This can *drastically* increase the speed of the backup and restore. When backing up, this must use the `--directory` option. *Be careful!* This will also create multiple database connections and can slow your database down.
+* `--directory`, `-d`: Restore from a directory. Overrides `--file` when used.
+
+### Backup Only Parameters for `pg_backup`
+
+* `--ignore-table`, `-i`: Excludes the table completely during the backup process. Can pass multiple tables: `-i bigtable1 -i bigtable2`
+* `--exclude-table-data`, `-e`: Excludes the table data during the backup process. Can pass multiple tables: `-e bigtable1 -e bigtable2`
+
+### Restore Only Parameters for `pg_restore`
+
+* `--no-confirm`: Restores the database without confirmation: be careful! DON'T OVERWRITE YOUR PROD DATABASE! (Ask me how I know.)
+
+## Example Commands
+
+`python manage.py pg_backup`
+
+This command will create a backup file in the directory `./db_backup/` (or the directory you specified with `PG_COPY_BACKUP_PATH`) called `[timestamp].sqlc` using the `default` settings from `DATABASES` using the default Django settings file resolved by `manage.py`.
+
+`python manage.py pg_backup --settings=config.settings.production --database=default --filename=my_backup.sqlc`
+
+This command will create a backup in the same directory as `manage.py` called `my_backup.sqlc` using the `default` settings from `DATABASES` using the Django settings file located at `config/settings/production.py`.
+
+`python manage.py pg_backup --directory=/tmp/pg_backup --jobs=8`
+
+This command will create a backup directory at `/tmp/backup` use 8 parallel jobs and database connections.
+
+`python manage.py pg_backup -i bigtable1 -i bigtable2`
+
+This will do the same as the previous command, but omit the tables named `bigtable1` and `bigtable2`.
+
+`python manage.py pg_backup -e bigtable1 -e bigtable2`
+
+This will do the same as the previous command, but include the table structure without any data for the tables named `bigtable1` and `bigtable2`.
+
+`python manage.py pg_restore`
+
+This command will provide a list of backup files in `PG_COPY_BACKUP_PATH` that can be restored. After selecting a backup file, it will confirm that the user wants to overwrite the destination database by showing which server and database will be overwritten from the settings. Here's what it will look like:
+
+```bash
+(venv) [django-project]$ ./manage.py pg_restore
+There are 8 backup files in '/var/dev/username/django-project/db_backup'. Which would you like to restore?
+1: 2020-05-27-13-33-38.sqlc
+2: 2020-05-10-09-07-45.sqlc
+3: 2020-05-11-13-05-49.sqlc
+4: 2020-07-14-15-21-22.sqlc
+5: 2020-05-15-08-31-59.sqlc
+6: 2020-06-11-13-11-00.sqlc
+7: 2020-06-02-13-28-09.sqlc
+8: 2020-05-27-14-54-15.sqlc
+Enter number of the file to restore: 4
+About to restore 'django_project_db' on host 'localhost' from the file:
+'/var/dev/username/django-project/db_backup/2020-07-14-15-21-22.sqlc'.
+THIS WILL OVERWRITE THE DATABASE.
+Type "yes" to start the restore [no]: yes
+```
+
+`python manage.py pg_restore --filename=my_file.sqlc --no-confirm`
+
+This command will read the file `my_file.sqlc` and **skip confirmation** that the user wants to overwrite the destination database.
+
+`python manage.py pg_restore --directory=/tmp/pg_backup --jobs=8`
+
+This command will restore from the directory `/tmp/pg_backup` using 8 parallel jobs and database connections.
+
+## Known Issues
+
+#### Errors Displayed During `pg_restore`
+
+When restoring, PostgreSQL's `pg_restore` command may output some warnings and erorrs. I haven't figured out a command line option to make these warnings disappear, but they can likely be ignored if you read them. Here is an example of what these errors may look like:
+
+```bash
+pg_restore: [archiver (db)] Error while PROCESSING TOC:
+pg_restore: [archiver (db)] Error from TOC entry 1; 3079 13792 EXTENSION plpgsql
+pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of extension plpgsql
+    Command was: DROP EXTENSION IF EXISTS plpgsql;
+
+pg_restore: [archiver (db)] Error from TOC entry 6; 2615 2200 SCHEMA public postgres
+pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of schema public
+    Command was: DROP SCHEMA IF EXISTS public;
+
+pg_restore: [archiver (db)] could not execute query: ERROR:  schema "public" already exists
+    Command was: CREATE SCHEMA public;
+```
+
+These may be errors from extensions that aren't used, or warnings about default schemata that already exist.
+
+## Release Notes
+
+[Release notes are available on GitHub](https://github.com/FlipperPA/django-pg-copy/releases).
+## Maintainer
+
+* [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
+
+This package is maintained by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our package users.
+
+## Contributors
+
+* Alex Malek (https://github.com/amalek215)
+* Noel Victor (https://github.com/noeldvictor)
+* Ryan Sullivan (https://github.com/rgs258)
```

### Comparing `django-pg-copy-1.0.0/README.md` & `django-pg-copy-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,23 @@
 * `--database`: The database defined in the DATABASES settings to backup from or restore to.
 * `--db-override`: A value to override the db argument sent to psql.
 * `--host-override`: A value to override the host argument sent to psql.
 * `--pg-home`: The path to the PostgreSQL installation, if it is not on your path.
 * `--file`, `-f`: The filename to backup to, or restore from.
 * `--jobs`, `-j`: The number of parallel jobs to run. This can *drastically* increase the speed of the backup and restore. When backing up, this must use the `--directory` option. *Be careful!* This will also create multiple database connections and can slow your database down.
 * `--directory`, `-d`: Restore from a directory. Overrides `--file` when used.
-* `--ignore-table`, `-i`: Excludes the table completely during the backup file creation. Can pass multiple tables: `-i bigtable1 -i bigtable2`
-* `--exclude-table-data`, `-e`: Excludes the table data during the backup file creation. Can pass multiple tables: `-e bigtable1 -e bigtable2`
-* `--no-confirm`: Restores the database without confirmation: be careful! (**pg_restore** only)
+
+### Backup Only Parameters for `pg_backup`
+
+* `--ignore-table`, `-i`: Excludes the table completely during the backup process. Can pass multiple tables: `-i bigtable1 -i bigtable2`
+* `--exclude-table-data`, `-e`: Excludes the table data during the backup process. Can pass multiple tables: `-e bigtable1 -e bigtable2`
+
+### Restore Only Parameters for `pg_restore`
+
+* `--no-confirm`: Restores the database without confirmation: be careful! DON'T OVERWRITE YOUR PROD DATABASE! (Ask me how I know.)
 
 ## Example Commands
 
 `python manage.py pg_backup`
 
 This command will create a backup file in the directory `./db_backup/` (or the directory you specified with `PG_COPY_BACKUP_PATH`) called `[timestamp].sqlc` using the `default` settings from `DATABASES` using the default Django settings file resolved by `manage.py`.
```

### Comparing `django-pg-copy-1.0.0/django_pg_copy.egg-info/PKG-INFO` & `django-pg-copy-1.1.0/django_pg_copy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,154 @@
 Metadata-Version: 2.1
 Name: django-pg-copy
-Version: 1.0.0
-Summary: UNKNOWN
-Home-page: https://github.com/FlipperPA/django-pg-copy
-Author: Tim Allen
-Author-email: tallen@wharton.upenn.edu
-License: UNKNOWN
-Description: # Django PostgreSQL Copy
-        
-        The package `django-pg-copy` provides Django management commands for backing up and restoring PostgreSQL databases. These were developed for copying production databases to development, to allow developers to share images with one another, or bring local development databases up to date. It can also be handy for creating different local databases for different branches, and for only creating one migration after tweaking models to get them the way they need to be.
-        
-        We also use it with Jenkins to automatically back up production, and restore to a staging database environment, so we can test new migrations repeatedly to ensure they'll work when we run them in production.
-        
-        ## Installation
-        
-        `pip install django-pg-copy`
-        
-        Then add `'pg_copy',` to your `INSTALLED_APPS` list. It is recommended that it is used in all environments (development, production) so that you can use it against different instances of your database.
-        
-        ## Settings
-        
-        `PG_COPY_BACKUP_PATH = 'db_backup'`
-        
-        By default, PostgreSQL backups will be stored in a directory called `db_backup` where you run the command. This setting will override that location.
-        
-        It is also recommended to add this path to your `.gitignore` file, if the path falls under your version control repository.
-        
-        ## Parameters
-        
-        * `--database`: The database defined in the DATABASES settings to backup from or restore to.
-        * `--db-override`: A value to override the db argument sent to psql.
-        * `--host-override`: A value to override the host argument sent to psql.
-        * `--pg-home`: The path to the PostgreSQL installation, if it is not on your path.
-        * `--file`, `-f`: The filename to backup to, or restore from.
-        * `--jobs`, `-j`: The number of parallel jobs to run. This can *drastically* increase the speed of the backup and restore. When backing up, this must use the `--directory` option. *Be careful!* This will also create multiple database connections and can slow your database down.
-        * `--directory`, `-d`: Restore from a directory. Overrides `--file` when used.
-        * `--ignore-table`, `-i`: Excludes the table completely during the backup file creation. Can pass multiple tables: `-i bigtable1 -i bigtable2`
-        * `--exclude-table-data`, `-e`: Excludes the table data during the backup file creation. Can pass multiple tables: `-e bigtable1 -e bigtable2`
-        * `--no-confirm`: Restores the database without confirmation: be careful! (**pg_restore** only)
-        
-        ## Example Commands
-        
-        `python manage.py pg_backup`
-        
-        This command will create a backup file in the directory `./db_backup/` (or the directory you specified with `PG_COPY_BACKUP_PATH`) called `[timestamp].sqlc` using the `default` settings from `DATABASES` using the default Django settings file resolved by `manage.py`.
-        
-        `python manage.py pg_backup --settings=config.settings.production --database=default --filename=my_backup.sqlc`
-        
-        This command will create a backup in the same directory as `manage.py` called `my_backup.sqlc` using the `default` settings from `DATABASES` using the Django settings file located at `config/settings/production.py`.
-        
-        `python manage.py pg_backup --directory=/tmp/pg_backup --jobs=8`
-        
-        This command will create a backup directory at `/tmp/backup` use 8 parallel jobs and database connections.
-        
-        `python manage.py pg_backup -i bigtable1 -i bigtable2`
-        
-        This will do the same as the previous command, but omit the tables named `bigtable1` and `bigtable2`.
-        
-        `python manage.py pg_backup -e bigtable1 -e bigtable2`
-        
-        This will do the same as the previous command, but include the table structure without any data for the tables named `bigtable1` and `bigtable2`.
-        
-        `python manage.py pg_restore`
-        
-        This command will provide a list of backup files in `PG_COPY_BACKUP_PATH` that can be restored. After selecting a backup file, it will confirm that the user wants to overwrite the destination database by showing which server and database will be overwritten from the settings. Here's what it will look like:
-        
-        ```bash
-        (venv) [django-project]$ ./manage.py pg_restore
-        There are 8 backup files in '/var/dev/username/django-project/db_backup'. Which would you like to restore?
-        1: 2020-05-27-13-33-38.sqlc
-        2: 2020-05-10-09-07-45.sqlc
-        3: 2020-05-11-13-05-49.sqlc
-        4: 2020-07-14-15-21-22.sqlc
-        5: 2020-05-15-08-31-59.sqlc
-        6: 2020-06-11-13-11-00.sqlc
-        7: 2020-06-02-13-28-09.sqlc
-        8: 2020-05-27-14-54-15.sqlc
-        Enter number of the file to restore: 4
-        About to restore 'django_project_db' on host 'localhost' from the file:
-        '/var/dev/username/django-project/db_backup/2020-07-14-15-21-22.sqlc'.
-        THIS WILL OVERWRITE THE DATABASE.
-        Type "yes" to start the restore [no]: yes
-        ```
-        
-        `python manage.py pg_restore --filename=my_file.sqlc --no-confirm`
-        
-        This command will read the file `my_file.sqlc` and **skip confirmation** that the user wants to overwrite the destination database.
-        
-        `python manage.py pg_restore --directory=/tmp/pg_backup --jobs=8`
-        
-        This command will restore from the directory `/tmp/pg_backup` using 8 parallel jobs and database connections.
-        
-        ## Known Issues
-        
-        #### Errors Displayed During `pg_restore`
-        
-        When restoring, PostgreSQL's `pg_restore` command may output some warnings and erorrs. I haven't figured out a command line option to make these warnings disappear, but they can likely be ignored if you read them. Here is an example of what these errors may look like:
-        
-        ```bash
-        pg_restore: [archiver (db)] Error while PROCESSING TOC:
-        pg_restore: [archiver (db)] Error from TOC entry 1; 3079 13792 EXTENSION plpgsql
-        pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of extension plpgsql
-            Command was: DROP EXTENSION IF EXISTS plpgsql;
-        
-        pg_restore: [archiver (db)] Error from TOC entry 6; 2615 2200 SCHEMA public postgres
-        pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of schema public
-            Command was: DROP SCHEMA IF EXISTS public;
-        
-        pg_restore: [archiver (db)] could not execute query: ERROR:  schema "public" already exists
-            Command was: CREATE SCHEMA public;
-        ```
-        
-        These may be errors from extensions that aren't used, or warnings about default schemata that already exist.
-        
-        ## Release Notes
-        
-        [Release notes are available on GitHub](https://github.com/FlipperPA/django-pg-copy/releases).
-        ## Maintainer
-        
-        * [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
-        
-        This package is maintained by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our package users.
-        
-        ## Contributors
-        
-        * Alex Malek (https://github.com/amalek215)
-        * Noel Victor (https://github.com/noeldvictor)
-        * Ryan Sullivan (https://github.com/rgs258)
-        
-Platform: UNKNOWN
+Version: 1.1.0
+Summary: Django management command to backup and restore PostgreSQL databases using the DATABASES settings.
+Author-email: Tim Allen <tallen@wharton.upenn.edu>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/FlipperPA/django-pg-copy
+Project-URL: Repository, https://github.com/FlipperPA/django-pg-copy
+Project-URL: Documentation, https://github.com/FlipperPA/django-pg-copy
+Keywords: postgres,postgresql,backup,restore,database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django PostgreSQL Copy
+
+The package `django-pg-copy` provides Django management commands for backing up and restoring PostgreSQL databases. These were developed for copying production databases to development, to allow developers to share images with one another, or bring local development databases up to date. It can also be handy for creating different local databases for different branches, and for only creating one migration after tweaking models to get them the way they need to be.
+
+We also use it with Jenkins to automatically back up production, and restore to a staging database environment, so we can test new migrations repeatedly to ensure they'll work when we run them in production.
+
+## Installation
+
+`pip install django-pg-copy`
+
+Then add `'pg_copy',` to your `INSTALLED_APPS` list. It is recommended that it is used in all environments (development, production) so that you can use it against different instances of your database.
+
+## Settings
+
+`PG_COPY_BACKUP_PATH = 'db_backup'`
+
+By default, PostgreSQL backups will be stored in a directory called `db_backup` where you run the command. This setting will override that location.
+
+It is also recommended to add this path to your `.gitignore` file, if the path falls under your version control repository.
+
+## Parameters
+
+* `--database`: The database defined in the DATABASES settings to backup from or restore to.
+* `--db-override`: A value to override the db argument sent to psql.
+* `--host-override`: A value to override the host argument sent to psql.
+* `--pg-home`: The path to the PostgreSQL installation, if it is not on your path.
+* `--file`, `-f`: The filename to backup to, or restore from.
+* `--jobs`, `-j`: The number of parallel jobs to run. This can *drastically* increase the speed of the backup and restore. When backing up, this must use the `--directory` option. *Be careful!* This will also create multiple database connections and can slow your database down.
+* `--directory`, `-d`: Restore from a directory. Overrides `--file` when used.
+
+### Backup Only Parameters for `pg_backup`
+
+* `--ignore-table`, `-i`: Excludes the table completely during the backup process. Can pass multiple tables: `-i bigtable1 -i bigtable2`
+* `--exclude-table-data`, `-e`: Excludes the table data during the backup process. Can pass multiple tables: `-e bigtable1 -e bigtable2`
+
+### Restore Only Parameters for `pg_restore`
+
+* `--no-confirm`: Restores the database without confirmation: be careful! DON'T OVERWRITE YOUR PROD DATABASE! (Ask me how I know.)
+
+## Example Commands
+
+`python manage.py pg_backup`
+
+This command will create a backup file in the directory `./db_backup/` (or the directory you specified with `PG_COPY_BACKUP_PATH`) called `[timestamp].sqlc` using the `default` settings from `DATABASES` using the default Django settings file resolved by `manage.py`.
+
+`python manage.py pg_backup --settings=config.settings.production --database=default --filename=my_backup.sqlc`
+
+This command will create a backup in the same directory as `manage.py` called `my_backup.sqlc` using the `default` settings from `DATABASES` using the Django settings file located at `config/settings/production.py`.
+
+`python manage.py pg_backup --directory=/tmp/pg_backup --jobs=8`
+
+This command will create a backup directory at `/tmp/backup` use 8 parallel jobs and database connections.
+
+`python manage.py pg_backup -i bigtable1 -i bigtable2`
+
+This will do the same as the previous command, but omit the tables named `bigtable1` and `bigtable2`.
+
+`python manage.py pg_backup -e bigtable1 -e bigtable2`
+
+This will do the same as the previous command, but include the table structure without any data for the tables named `bigtable1` and `bigtable2`.
+
+`python manage.py pg_restore`
+
+This command will provide a list of backup files in `PG_COPY_BACKUP_PATH` that can be restored. After selecting a backup file, it will confirm that the user wants to overwrite the destination database by showing which server and database will be overwritten from the settings. Here's what it will look like:
+
+```bash
+(venv) [django-project]$ ./manage.py pg_restore
+There are 8 backup files in '/var/dev/username/django-project/db_backup'. Which would you like to restore?
+1: 2020-05-27-13-33-38.sqlc
+2: 2020-05-10-09-07-45.sqlc
+3: 2020-05-11-13-05-49.sqlc
+4: 2020-07-14-15-21-22.sqlc
+5: 2020-05-15-08-31-59.sqlc
+6: 2020-06-11-13-11-00.sqlc
+7: 2020-06-02-13-28-09.sqlc
+8: 2020-05-27-14-54-15.sqlc
+Enter number of the file to restore: 4
+About to restore 'django_project_db' on host 'localhost' from the file:
+'/var/dev/username/django-project/db_backup/2020-07-14-15-21-22.sqlc'.
+THIS WILL OVERWRITE THE DATABASE.
+Type "yes" to start the restore [no]: yes
+```
+
+`python manage.py pg_restore --filename=my_file.sqlc --no-confirm`
+
+This command will read the file `my_file.sqlc` and **skip confirmation** that the user wants to overwrite the destination database.
+
+`python manage.py pg_restore --directory=/tmp/pg_backup --jobs=8`
+
+This command will restore from the directory `/tmp/pg_backup` using 8 parallel jobs and database connections.
+
+## Known Issues
+
+#### Errors Displayed During `pg_restore`
+
+When restoring, PostgreSQL's `pg_restore` command may output some warnings and erorrs. I haven't figured out a command line option to make these warnings disappear, but they can likely be ignored if you read them. Here is an example of what these errors may look like:
+
+```bash
+pg_restore: [archiver (db)] Error while PROCESSING TOC:
+pg_restore: [archiver (db)] Error from TOC entry 1; 3079 13792 EXTENSION plpgsql
+pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of extension plpgsql
+    Command was: DROP EXTENSION IF EXISTS plpgsql;
+
+pg_restore: [archiver (db)] Error from TOC entry 6; 2615 2200 SCHEMA public postgres
+pg_restore: [archiver (db)] could not execute query: ERROR:  must be owner of schema public
+    Command was: DROP SCHEMA IF EXISTS public;
+
+pg_restore: [archiver (db)] could not execute query: ERROR:  schema "public" already exists
+    Command was: CREATE SCHEMA public;
+```
+
+These may be errors from extensions that aren't used, or warnings about default schemata that already exist.
+
+## Release Notes
+
+[Release notes are available on GitHub](https://github.com/FlipperPA/django-pg-copy/releases).
+## Maintainer
+
+* [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
+
+This package is maintained by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our package users.
+
+## Contributors
+
+* Alex Malek (https://github.com/amalek215)
+* Noel Victor (https://github.com/noeldvictor)
+* Ryan Sullivan (https://github.com/rgs258)
```

### Comparing `django-pg-copy-1.0.0/pg_copy/management/commands/pg_backup.py` & `django-pg-copy-1.1.0/pg_copy/management/commands/pg_backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 @click.option(
     "--host-override",
     "host_override",
     default=None,
     help="A value to override the host argument sent to psql.",
 )
 @click.option(
+    "--port-override",
+    "port_override",
+    default=None,
+    help="A value to override the port argument sent to psql.",
+)
+@click.option(
     "--pg-home",
     "pg_home",
     default=None,
     help="The path to the PostgreSQL installation, if it is not on your path.",
 )
 @click.option(
     "--file",
@@ -80,27 +86,29 @@
     ),
     help="The directory to backup to when the --jobs parameter is used.",
 )
 def command(
     database,
     db_override,
     host_override,
+    port_override,
     pg_home,
     filename,
     ignore_table,
     exclude_table_data,
     jobs,
     directory,
 ):
     """
     Django management command to make a backup of a PostgreSQL database.
     """
 
     db = db_override or settings.DATABASES[database]["NAME"]
     host = host_override or settings.DATABASES[database]["HOST"]
+    port = port_override or settings.DATABASES[database]["PORT"]
     pg_dump = os.path.join(pg_home, "bin", "pg_dump") if pg_home else "pg_dump"
 
     ignore_table_cmd = ""
     for table in ignore_table:
         ignore_table_cmd = " -T {table}{ignore_table_cmd}".format(
             table=table,
             ignore_table_cmd=ignore_table_cmd,
@@ -126,15 +134,15 @@
     backup_path = get_backup_path()
     if not os.path.exists(backup_path):
         os.makedirs(backup_path)
 
     os.environ["PGPASSWORD"] = settings.DATABASES[database]["PASSWORD"]
     try:
         backup_command = (
-            f"""{pg_dump} {backup} -c -O -x -h {host} """
+            f"""{pg_dump} {backup} -c -O -x -h {host} -p {port} """
             f"""-U {settings.DATABASES[database]["USER"]} """
             f"{ignore_table_cmd} {exclude_table_cmd} {db}"
         )
 
         print(backup_command)
         subprocess.check_output(
             backup_command,
```

### Comparing `django-pg-copy-1.0.0/pg_copy/management/commands/pg_restore.py` & `django-pg-copy-1.1.0/pg_copy/management/commands/pg_restore.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 @click.option(
     "--host-override",
     "host_override",
     default=None,
     help="A value to override the host argument sent to psql.",
 )
 @click.option(
+    "--port-override",
+    "port_override",
+    default=None,
+    help="A value to override the port argument sent to psql.",
+)
+@click.option(
     "--pg-home",
     "pg_home",
     default=None,
     help="The path to the PostgreSQL installation, if it is not on your path.",
 )
 @click.option(
     "--file",
@@ -57,22 +63,31 @@
 @click.option(
     "--no-confirm",
     "no_confirm",
     is_flag=True,
     help="Restores the database without confirmation: be careful!",
 )
 def command(
-    database, db_override, host_override, pg_home, filename, jobs, directory, no_confirm
+    database,
+    db_override,
+    host_override,
+    port_override,
+    pg_home,
+    filename,
+    jobs,
+    directory,
+    no_confirm,
 ):
     """
     Django management command to restore a PostgreSQL database.
     """
 
     db = db_override or settings.DATABASES[database]["NAME"]
     host = host_override or settings.DATABASES[database]["HOST"]
+    port = port_override or settings.DATABASES[database]["PORT"]
     psql = os.path.join(pg_home, "bin", "psql") if pg_home else "psql"
     pg_restore = os.path.join(pg_home, "bin", "pg_restore") if pg_home else "pg_restore"
 
     if directory:
         if not os.path.isdir(directory):
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), directory)
 
@@ -124,44 +139,44 @@
         restore = f"--format=custom {filename}"
 
     if no_confirm:
         confirm = "yes"
     else:
         if directory:
             message = (
-                f"About to restore '{db}' on host '{host}' from the directory:\n"
+                f"About to restore '{db}' on host '{host}:{port}' from the directory:\n"
                 f"'{directory}'\n"
             )
         else:
             message = (
-                f"About to restore '{db}' on host '{host}' from the file:\n"
+                f"About to restore '{db}' on host '{host}:{port}' from the file:\n"
                 f"'{filename}'\n"
             )
 
         click.secho(
             f"{message}THIS WILL OVERWRITE THE DATABASE.",
             fg="red",
             bold=True,
         )
 
-        confirm = click.prompt('Type "yes" to start the restore', default="no")
+        confirm = click.prompt("Type 'yes' to start the restore", default="no")
 
     if confirm == "yes":
         os.environ["PGPASSWORD"] = settings.DATABASES[database]["PASSWORD"]
 
         try:
             subprocess.check_output(
                 f'{psql} -h {host} -U {settings.DATABASES[database]["USER"]} -d {db} '
-                f'-c "DROP OWNED BY {settings.DATABASES[database]["USER"]};"',
+                f'-p {port} -c "DROP OWNED BY {settings.DATABASES[database]["USER"]};"',
                 shell=True,
             )
 
             subprocess.check_output(
                 f"{pg_restore} -c -O -x --if-exists -h {host} -d {db} --jobs {jobs} "
-                f"""-U {settings.DATABASES[database]["USER"]} {restore}""",
+                f"""-p {port} -U {settings.DATABASES[database]["USER"]} {restore}""",
                 shell=True,
             )
             click.secho("The database has been restored.", fg="green")
         except subprocess.CalledProcessError as e:
             print(e)
             sys.exit(e.returncode)
         finally:
```

