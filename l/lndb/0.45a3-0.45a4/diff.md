# Comparing `tmp/lndb-0.45a3.tar.gz` & `tmp/lndb-0.45a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.45a3.tar", last modified: Sun May 28 12:53:45 2023, max compression
+gzip compressed data, was "lndb-0.45a4.tar", last modified: Sun May 28 13:56:11 2023, max compression
```

## Comparing `lndb-0.45a3.tar` & `lndb-0.45a4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     3804 2023-05-27 08:31:20.462437 lndb-0.45a3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.45a3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.45a3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.45a3/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.45a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.45a3/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.45a3/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.45a3/docs/api.md
--rw-r--r--   0        0        0    49387 2023-05-28 12:53:18.343383 lndb-0.45a3/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.45a3/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.45a3/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8795 2023-05-26 18:42:19.597992 lndb-0.45a3/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.45a3/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.45a3/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.45a3/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2589 2023-05-27 05:58:01.864810 lndb-0.45a3/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.45a3/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     8540 2023-05-27 09:10:15.195959 lndb-0.45a3/docs/guide/00-index.ipynb
--rw-r--r--   0        0        0     5025 2023-05-26 16:29:38.650577 lndb-0.45a3/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11082 2023-05-26 16:29:38.651219 lndb-0.45a3/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6639 2023-05-26 16:29:38.651368 lndb-0.45a3/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     7616 2023-05-26 16:29:38.651991 lndb-0.45a3/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-05-26 16:29:38.652557 lndb-0.45a3/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     3331 2023-05-24 18:12:34.768903 lndb-0.45a3/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.45a3/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.45a3/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-05-28 12:53:10.436966 lndb-0.45a3/lndb/__init__.py
--rw-r--r--   0        0        0     5268 2023-05-24 18:12:34.769088 lndb-0.45a3/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.45a3/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.45a3/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-05-28 12:52:47.657543 lndb-0.45a3/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.45a3/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.45a3/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-24 17:57:29.952669 lndb-0.45a3/lndb/_info.py
--rw-r--r--   0        0        0     6247 2023-05-26 16:29:38.653812 lndb-0.45a3/lndb/_init_instance.py
--rw-r--r--   0        0        0     6661 2023-05-26 16:29:38.653964 lndb-0.45a3/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.45a3/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.45a3/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-24 17:08:25.124000 lndb-0.45a3/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7611 2023-05-27 05:58:01.865831 lndb-0.45a3/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.45a3/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-24 17:25:24.780147 lndb-0.45a3/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.45a3/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-05-24 18:12:34.769186 lndb-0.45a3/lndb/_notebook.py
--rw-r--r--   0        0        0      803 2023-04-28 18:11:00.215484 lndb-0.45a3/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.45a3/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.45a3/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.45a3/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.45a3/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.45a3/lndb/_settings_store.py
--rw-r--r--   0        0        0     3905 2023-05-12 07:21:12.821554 lndb-0.45a3/lndb/_setup_user.py
--rw-r--r--   0        0        0      456 2023-05-26 16:29:43.073569 lndb-0.45a3/lndb/dev/__init__.py
--rw-r--r--   0        0        0     3886 2023-05-26 16:39:31.260401 lndb-0.45a3/lndb/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-05-26 16:40:04.945302 lndb-0.45a3/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.45a3/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.45a3/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.45a3/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-28 18:11:00.215703 lndb-0.45a3/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.45a3/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.45a3/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.45a3/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.45a3/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2710 2023-05-26 16:29:38.655499 lndb-0.45a3/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     4466 2023-05-26 16:29:38.655928 lndb-0.45a3/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.45a3/lndb/dev/_storage.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.45a3/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.45a3/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.45a3/lndb/test/_env.py
--rw-r--r--   0        0        0     3913 2023-05-26 16:40:53.833999 lndb-0.45a3/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.45a3/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      254 2023-05-26 16:43:38.785220 lndb-0.45a3/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.45a3/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.45a3/noxfile.py
--rw-r--r--   0        0        0     1318 2023-05-28 12:52:50.543577 lndb-0.45a3/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.45a3/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.45a3/tests/test_init_instance.py
--rw-r--r--   0        0        0      379 2023-05-12 07:21:08.563165 lndb-0.45a3/tests/test_notebooks.py
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 lndb-0.45a3/PKG-INFO
+-rw-r--r--   0        0        0     3804 2023-05-28 13:55:44.139985 lndb-0.45a4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.45a4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.45a4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.45a4/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.45a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.45a4/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.45a4/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.45a4/docs/api.md
+-rw-r--r--   0        0        0    49540 2023-05-28 13:55:52.645402 lndb-0.45a4/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.45a4/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.45a4/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8795 2023-05-26 18:42:19.597992 lndb-0.45a4/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.45a4/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.45a4/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.45a4/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2589 2023-05-27 05:58:01.864810 lndb-0.45a4/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.45a4/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     8540 2023-05-27 09:10:15.195959 lndb-0.45a4/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5025 2023-05-26 16:29:38.650577 lndb-0.45a4/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11082 2023-05-26 16:29:38.651219 lndb-0.45a4/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6639 2023-05-26 16:29:38.651368 lndb-0.45a4/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     7616 2023-05-26 16:29:38.651991 lndb-0.45a4/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-05-26 16:29:38.652557 lndb-0.45a4/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-05-24 18:12:34.768903 lndb-0.45a4/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.45a4/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.45a4/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-05-28 13:55:46.522109 lndb-0.45a4/lndb/__init__.py
+-rw-r--r--   0        0        0     5268 2023-05-24 18:12:34.769088 lndb-0.45a4/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.45a4/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.45a4/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-28 13:55:44.140489 lndb-0.45a4/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.45a4/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.45a4/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-24 17:57:29.952669 lndb-0.45a4/lndb/_info.py
+-rw-r--r--   0        0        0     6247 2023-05-26 16:29:38.653812 lndb-0.45a4/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6661 2023-05-26 16:29:38.653964 lndb-0.45a4/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.45a4/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.45a4/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-24 17:08:25.124000 lndb-0.45a4/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7611 2023-05-27 05:58:01.865831 lndb-0.45a4/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.45a4/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-24 17:25:24.780147 lndb-0.45a4/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.45a4/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-05-24 18:12:34.769186 lndb-0.45a4/lndb/_notebook.py
+-rw-r--r--   0        0        0      803 2023-04-28 18:11:00.215484 lndb-0.45a4/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.45a4/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.45a4/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.45a4/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.45a4/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.45a4/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3905 2023-05-12 07:21:12.821554 lndb-0.45a4/lndb/_setup_user.py
+-rw-r--r--   0        0        0      456 2023-05-26 16:29:43.073569 lndb-0.45a4/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-26 16:39:31.260401 lndb-0.45a4/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-05-26 16:40:04.945302 lndb-0.45a4/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.45a4/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.45a4/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.45a4/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-28 18:11:00.215703 lndb-0.45a4/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.45a4/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.45a4/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.45a4/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.45a4/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2710 2023-05-26 16:29:38.655499 lndb-0.45a4/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     4466 2023-05-26 16:29:38.655928 lndb-0.45a4/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.45a4/lndb/dev/_storage.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.45a4/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.45a4/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.45a4/lndb/test/_env.py
+-rw-r--r--   0        0        0     3913 2023-05-26 16:40:53.833999 lndb-0.45a4/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.45a4/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:43:38.785220 lndb-0.45a4/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.45a4/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.45a4/noxfile.py
+-rw-r--r--   0        0        0     1356 2023-05-28 13:55:44.140652 lndb-0.45a4/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.45a4/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.45a4/tests/test_init_instance.py
+-rw-r--r--   0        0        0      379 2023-05-12 07:21:08.563165 lndb-0.45a4/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 lndb-0.45a4/PKG-INFO
```

### Comparing `lndb-0.45a3/.github/workflows/build.yml` & `lndb-0.45a4/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
       - name: Install Python dependencies
         run: |
           python -m pip install -U pip
-          pip install lamindb==0.41a3
+          pip install lamindb>=0.41a3
       - name: Install apt-get dependencies
         run: |
           sudo apt-get -y install graphviz
           sudo apt-get install sqlite3-tools=3.37.2-2
           sudo apt-get install libpq-dev
       - name: Lint
         run: |
```

### Comparing `lndb-0.45a3/.github/workflows/latest-changes.yml` & `lndb-0.45a4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/.gitignore` & `lndb-0.45a4/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/.pre-commit-config.yaml` & `lndb-0.45a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/LICENSE` & `lndb-0.45a4/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/changelog.md` & `lndb-0.45a4/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade to lnhub-rest 0.9.8 | [384](https://github.com/laminlabs/lndb/pull/384) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a4
 ⬆️ Upgrade lnhub-rest to 0.9.7 | [383](https://github.com/laminlabs/lndb/pull/383) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a3
 📝 Add setup overview from lamindb | [382](https://github.com/laminlabs/lndb/pull/382) | [falexwolf](https://github.com/falexwolf) | 2023-05-27 |
 🔥 Remove schema modules logic from `setup_schema` | [381](https://github.com/laminlabs/lndb/pull/381) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.45a2
 🏗️ Remove SQL-level schema modules | [380](https://github.com/laminlabs/lndb/pull/380) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.45a1
 ✨ Add track command to CLI | [378](https://github.com/laminlabs/lndb/pull/378) | [Koncopd](https://github.com/Koncopd) | 2023-05-23 |
 📝 Improve migration docs | [379](https://github.com/laminlabs/lndb/pull/379) | [Zethson](https://github.com/Zethson) | 2023-05-22 |
 🔊 Use lamin_logger in test_notebooks.py | [376](https://github.com/laminlabs/lndb/pull/376) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
```

### Comparing `lndb-0.45a3/docs/faq/check-synchronization.ipynb` & `lndb-0.45a4/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/clone.ipynb` & `lndb-0.45a4/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.45a4/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/manage-migrations.ipynb` & `lndb-0.45a4/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/switch-environment.ipynb` & `lndb-0.45a4/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.45a4/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/faq/test-migrations-unit.ipynb` & `lndb-0.45a4/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/00-index.ipynb` & `lndb-0.45a4/docs/guide/00-index.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/01-setup-user.ipynb` & `lndb-0.45a4/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/02-init-instance.ipynb` & `lndb-0.45a4/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/03-load-instance.ipynb` & `lndb-0.45a4/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/04-set-storage.ipynb` & `lndb-0.45a4/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/05-schema-modules.ipynb` & `lndb-0.45a4/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/docs/guide/migrate.md` & `lndb-0.45a4/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/__init__.py` & `lndb-0.45a4/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.45a3"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.45a4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.45a3/lndb/__main__.py` & `lndb-0.45a4/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_check_instance_setup.py` & `lndb-0.45a4/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_close.py` & `lndb-0.45a4/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_delete.py` & `lndb-0.45a4/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_init_instance.py` & `lndb-0.45a4/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_load_instance.py` & `lndb-0.45a4/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_migrate/alembic.ini` & `lndb-0.45a4/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_migrate/core.py` & `lndb-0.45a4/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_migrate/deploy.py` & `lndb-0.45a4/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_migrate/env.py` & `lndb-0.45a4/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_migrate/utils.py` & `lndb-0.45a4/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_notebook.py` & `lndb-0.45a4/lndb/_notebook.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_register_instance.py` & `lndb-0.45a4/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_schema.py` & `lndb-0.45a4/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_set.py` & `lndb-0.45a4/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_settings.py` & `lndb-0.45a4/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/_setup_user.py` & `lndb-0.45a4/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_clone.py` & `lndb-0.45a4/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_db.py` & `lndb-0.45a4/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_deprecated.py` & `lndb-0.45a4/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_exclusion.py` & `lndb-0.45a4/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_settings_instance.py` & `lndb-0.45a4/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_settings_load.py` & `lndb-0.45a4/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_settings_save.py` & `lndb-0.45a4/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_settings_store.py` & `lndb-0.45a4/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_settings_user.py` & `lndb-0.45a4/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_setup_knowledge.py` & `lndb-0.45a4/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_setup_schema.py` & `lndb-0.45a4/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/_storage.py` & `lndb-0.45a4/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/dev/upath.py` & `lndb-0.45a4/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/test/_migrations_e2e.py` & `lndb-0.45a4/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/lndb/test/_migrations_unit.py` & `lndb-0.45a4/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/noxfile.py` & `lndb-0.45a4/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/pyproject.toml` & `lndb-0.45a4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.7",
+    "lnhub_rest==0.9.8",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.34a2",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "sqlmodel>=0.0.8",
@@ -36,14 +36,15 @@
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
     "lnschema_lamin1",
+    "lamindb[bionty,lamin1]>=0.41a3",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
     "nbproject",
 ]
 
 [project.scripts]
```

### Comparing `lndb-0.45a3/tests/test_bionty.py` & `lndb-0.45a4/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/tests/test_init_instance.py` & `lndb-0.45a4/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a3/PKG-INFO` & `lndb-0.45a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.45a3
+Version: 0.45a4
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.7
+Requires-Dist: lnhub_rest==0.9.8
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.34a2
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
 Requires-Dist: appdirs
@@ -18,14 +18,15 @@
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: lnschema_lamin1 ; extra == "test"
+Requires-Dist: lamindb[bionty,lamin1]>=0.41a3 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb
 Provides-Extra: dev
 Provides-Extra: test
```

