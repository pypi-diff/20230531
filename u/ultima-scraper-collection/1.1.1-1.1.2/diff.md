# Comparing `tmp/ultima_scraper_collection-1.1.1.tar.gz` & `tmp/ultima_scraper_collection-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-1.1.1.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-1.1.2.tar", max compression
```

## Comparing `ultima_scraper_collection-1.1.1.tar` & `ultima_scraper_collection-1.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      788 2023-05-22 11:06:28.657966 ultima_scraper_collection-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.1/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     5640 2023-05-14 03:41:28.928194 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    10564 2023-05-22 04:57:37.439982 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/legacy_code.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    27937 2023-05-22 04:54:03.366424 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     7080 2023-05-22 08:09:26.097930 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    17837 2023-05-22 07:44:05.266486 ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.1/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      788 2023-05-31 21:42:12.599928 ultima_scraper_collection-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.2/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5641 2023-05-31 12:09:04.884552 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    10728 2023-05-31 18:34:23.965718 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/legacy_code.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    27937 2023-05-22 04:54:03.366424 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7080 2023-05-22 08:09:26.097930 ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    18213 2023-05-31 11:19:09.143046 ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.2/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.2/PKG-INFO
```

### Comparing `ultima_scraper_collection-1.1.1/pyproject.toml` & `ultima_scraper_collection-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
```

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
 from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
+from ultima_scraper_renamer.reformat import ReformatManager
+
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
-from ultima_scraper_renamer.reformat import ReformatManager
 
 
 class OnlyFansDataScraper(StreamlinedDatascraper):
     def __init__(self, api: OnlyFansAPI, option_manager: OptionManager) -> None:
         self.api = api
         self.option_manager = option_manager
         StreamlinedDatascraper.__init__(self, self)
```

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/download_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import copy
 from pathlib import Path
+from urllib.parse import urlparse
 
 import ffmpeg
 from aiohttp import ClientResponse
 from ultima_scraper_api.helpers import main_helper
 from ultima_scraper_api.managers.session_manager import SessionManager
 from ultima_scraper_renamer.reformat import ReformatManager
 
@@ -94,14 +95,20 @@
         if not db_content or not download_item.id:
             return
         db_media = db_content.find_media(download_item.id)
         if not db_media:
             return
         if not download_item.urls:
             return
+        matches = ["us", "uk", "ca", "ca2", "de"]
+        p_url = urlparse(download_item.urls[0])
+
+        subdomain = p_url.hostname.split(".")[0]
+        if any(subdomain in nm for nm in matches):
+            return
         download_item.__db_item__ = db_media
 
         authed = self.session_manager.auth
         authed_drm = authed.drm
 
         async with self.session_manager.semaphore:
             while attempt < self.session_manager.max_attempts + 1:
@@ -165,19 +172,16 @@
                     timestamp = db_media.created_at.timestamp()
                     await main_helper.format_file(
                         download_path, timestamp, self.reformat
                     )
                     db_media.size = final_size
                     db_media.downloaded = True
                     break
-                except asyncio.TimeoutError as e:
-                    pass
-                except Exception as e:
-                    print(e)
-                    pass
+                except asyncio.TimeoutError as _e:
+                    continue
 
     async def writer(
         self,
         result: ClientResponse,
         download_item: MediaMetadata,
         encrypted: bool = True,
     ):
```

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/legacy_code.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/legacy_code.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/managers/option_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-1.1.2/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 from sqlalchemy.exc import OperationalError
 from tqdm.asyncio import tqdm_asyncio
+from ultima_scraper_renamer import renamer
+
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
-from ultima_scraper_renamer import renamer
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
 subscription_types = ultima_scraper_api.subscription_types
 
@@ -182,14 +183,19 @@
                     pass
                 case "Highlights":
                     pass
                 case "MassMessages":
                     pass
                 case _:
                     raise Exception(f"{content_type} is an invalid choice")
+        # Adding paid content and removing duplicates by id
+        if isinstance(user, ultima_scraper_api.onlyfans_classes.user_model.create_user):
+            for paid_content in await user.get_paid_contents(content_type):
+                temp_master_set.append(paid_content)
+            temp_master_set = list({getattr(obj,"id"): obj for obj in temp_master_set}.values())
         await self.process_scraped_content(
             temp_master_set, content_type, user, metadata_manager
         )
         current_job.done = True
 
     async def process_scraped_content(
         self,
```

### Comparing `ultima_scraper_collection-1.1.1/PKG-INFO` & `ultima_scraper_collection-1.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

