# Comparing `tmp/lndb-0.45a4.tar.gz` & `tmp/lndb-0.46a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.45a4.tar", last modified: Sun May 28 13:56:11 2023, max compression
+gzip compressed data, was "lndb-0.46a1.tar", last modified: Wed May 31 20:34:07 2023, max compression
```

## Comparing `lndb-0.45a4.tar` & `lndb-0.46a1.tar`

### file list

```diff
@@ -1,78 +1,166 @@
--rw-r--r--   0        0        0     3804 2023-05-28 13:55:44.139985 lndb-0.45a4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.45a4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.45a4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.45a4/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.45a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.45a4/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.45a4/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.45a4/docs/api.md
--rw-r--r--   0        0        0    49540 2023-05-28 13:55:52.645402 lndb-0.45a4/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.45a4/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.45a4/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8795 2023-05-26 18:42:19.597992 lndb-0.45a4/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.45a4/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.45a4/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.45a4/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2589 2023-05-27 05:58:01.864810 lndb-0.45a4/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.45a4/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     8540 2023-05-27 09:10:15.195959 lndb-0.45a4/docs/guide/00-index.ipynb
--rw-r--r--   0        0        0     5025 2023-05-26 16:29:38.650577 lndb-0.45a4/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11082 2023-05-26 16:29:38.651219 lndb-0.45a4/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6639 2023-05-26 16:29:38.651368 lndb-0.45a4/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     7616 2023-05-26 16:29:38.651991 lndb-0.45a4/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-05-26 16:29:38.652557 lndb-0.45a4/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     3331 2023-05-24 18:12:34.768903 lndb-0.45a4/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.45a4/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.45a4/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-05-28 13:55:46.522109 lndb-0.45a4/lndb/__init__.py
--rw-r--r--   0        0        0     5268 2023-05-24 18:12:34.769088 lndb-0.45a4/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.45a4/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.45a4/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-05-28 13:55:44.140489 lndb-0.45a4/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.45a4/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.45a4/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-24 17:57:29.952669 lndb-0.45a4/lndb/_info.py
--rw-r--r--   0        0        0     6247 2023-05-26 16:29:38.653812 lndb-0.45a4/lndb/_init_instance.py
--rw-r--r--   0        0        0     6661 2023-05-26 16:29:38.653964 lndb-0.45a4/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.45a4/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.45a4/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-24 17:08:25.124000 lndb-0.45a4/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7611 2023-05-27 05:58:01.865831 lndb-0.45a4/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.45a4/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-24 17:25:24.780147 lndb-0.45a4/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.45a4/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-05-24 18:12:34.769186 lndb-0.45a4/lndb/_notebook.py
--rw-r--r--   0        0        0      803 2023-04-28 18:11:00.215484 lndb-0.45a4/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.45a4/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.45a4/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.45a4/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.45a4/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.45a4/lndb/_settings_store.py
--rw-r--r--   0        0        0     3905 2023-05-12 07:21:12.821554 lndb-0.45a4/lndb/_setup_user.py
--rw-r--r--   0        0        0      456 2023-05-26 16:29:43.073569 lndb-0.45a4/lndb/dev/__init__.py
--rw-r--r--   0        0        0     3886 2023-05-26 16:39:31.260401 lndb-0.45a4/lndb/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-05-26 16:40:04.945302 lndb-0.45a4/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.45a4/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.45a4/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.45a4/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-28 18:11:00.215703 lndb-0.45a4/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.45a4/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.45a4/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.45a4/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.45a4/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2710 2023-05-26 16:29:38.655499 lndb-0.45a4/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     4466 2023-05-26 16:29:38.655928 lndb-0.45a4/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.45a4/lndb/dev/_storage.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.45a4/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.45a4/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.45a4/lndb/test/_env.py
--rw-r--r--   0        0        0     3913 2023-05-26 16:40:53.833999 lndb-0.45a4/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.45a4/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      254 2023-05-26 16:43:38.785220 lndb-0.45a4/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.45a4/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.45a4/noxfile.py
--rw-r--r--   0        0        0     1356 2023-05-28 13:55:44.140652 lndb-0.45a4/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.45a4/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.45a4/tests/test_init_instance.py
--rw-r--r--   0        0        0      379 2023-05-12 07:21:08.563165 lndb-0.45a4/tests/test_notebooks.py
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 lndb-0.45a4/PKG-INFO
+-rw-r--r--   0        0        0     3302 2023-05-31 19:23:44.380632 lndb-0.46a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lndb-0.46a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lndb-0.46a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lndb-0.46a1/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lndb-0.46a1/.gitmodules
+-rw-r--r--   0        0        0     1777 2023-05-26 12:29:21.559703 lndb-0.46a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lndb-0.46a1/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-26 12:29:21.559893 lndb-0.46a1/README.md
+-rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lndb-0.46a1/docs/api.md
+-rw-r--r--   0        0        0    49975 2023-05-31 19:34:44.890833 lndb-0.46a1/docs/changelog.md
+-rw-r--r--   0        0        0     5329 2023-05-31 19:23:44.381276 lndb-0.46a1/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3499 2023-05-31 19:23:44.381656 lndb-0.46a1/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     6321 2023-05-31 19:23:44.382018 lndb-0.46a1/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-05-26 12:29:21.560682 lndb-0.46a1/docs/faq/index.md
+-rw-r--r--   0        0        0     1226 2023-05-31 19:23:44.382327 lndb-0.46a1/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3305 2023-05-31 19:23:44.382618 lndb-0.46a1/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2767 2023-05-31 19:23:44.382879 lndb-0.46a1/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2117 2023-05-31 19:23:44.383107 lndb-0.46a1/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     8809 2023-05-31 19:23:44.383467 lndb-0.46a1/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5025 2023-05-30 16:37:06.807599 lndb-0.46a1/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0     8060 2023-05-31 19:23:44.383804 lndb-0.46a1/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     4330 2023-05-31 19:23:44.384142 lndb-0.46a1/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6096 2023-05-31 19:23:44.384468 lndb-0.46a1/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3263 2023-05-31 19:23:44.384744 lndb-0.46a1/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lndb-0.46a1/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lndb-0.46a1/docs/index.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lndb-0.46a1/docs/test_notebooks.py
+-rw-r--r--   0        0        0      118 2023-05-26 12:29:21.561849 lndb-0.46a1/lamin-project.yaml
+-rw-r--r--   0        0        0     2799 2023-05-31 20:33:33.891779 lndb-0.46a1/lndb/__init__.py
+-rw-r--r--   0        0        0     5268 2023-05-26 12:29:21.562165 lndb-0.46a1/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-05-26 12:29:21.562276 lndb-0.46a1/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1606 2023-05-31 19:23:44.385426 lndb-0.46a1/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-30 12:40:09.059428 lndb-0.46a1/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-05-26 12:29:21.562518 lndb-0.46a1/lndb/_close.py
+-rw-r--r--   0        0        0     2182 2023-05-31 19:23:44.386369 lndb-0.46a1/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-05-26 12:29:21.562660 lndb-0.46a1/lndb/_info.py
+-rw-r--r--   0        0        0     7253 2023-05-31 19:23:44.386693 lndb-0.46a1/lndb/_init_instance.py
+-rw-r--r--   0        0        0     7282 2023-05-31 19:23:44.387007 lndb-0.46a1/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-05-26 12:29:21.562943 lndb-0.46a1/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-26 12:29:21.563011 lndb-0.46a1/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-05-26 12:29:21.563098 lndb-0.46a1/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7611 2023-05-26 12:29:21.563211 lndb-0.46a1/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-05-26 12:29:21.563296 lndb-0.46a1/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-05-26 12:29:21.563363 lndb-0.46a1/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-05-26 12:29:21.563464 lndb-0.46a1/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-05-26 12:29:21.563537 lndb-0.46a1/lndb/_notebook.py
+-rw-r--r--   0        0        0      803 2023-05-26 12:29:21.563604 lndb-0.46a1/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-05-26 12:29:21.563675 lndb-0.46a1/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-05-26 12:29:21.563744 lndb-0.46a1/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-05-26 12:29:21.563814 lndb-0.46a1/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-05-26 12:29:21.563877 lndb-0.46a1/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-05-26 12:29:21.563934 lndb-0.46a1/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3488 2023-05-31 19:23:44.387337 lndb-0.46a1/lndb/_setup_user.py
+-rw-r--r--   0        0        0      456 2023-05-28 13:35:53.148657 lndb-0.46a1/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-28 13:35:53.148822 lndb-0.46a1/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-05-26 12:29:21.564290 lndb-0.46a1/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-05-26 12:29:21.564389 lndb-0.46a1/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0     1693 2023-05-31 19:23:44.387585 lndb-0.46a1/lndb/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-05-26 12:29:21.564469 lndb-0.46a1/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-05-26 12:29:21.564557 lndb-0.46a1/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     9126 2023-05-31 19:23:44.387900 lndb-0.46a1/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-05-31 19:23:44.388155 lndb-0.46a1/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-05-26 12:29:21.564796 lndb-0.46a1/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-05-26 12:29:21.564870 lndb-0.46a1/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-05-31 19:23:44.388369 lndb-0.46a1/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2710 2023-05-26 12:29:21.565003 lndb-0.46a1/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     5052 2023-05-31 19:23:44.388665 lndb-0.46a1/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5536 2023-05-31 19:23:44.388940 lndb-0.46a1/lndb/dev/_storage.py
+-rw-r--r--   0        0        0     2536 2023-05-26 12:29:21.565324 lndb-0.46a1/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-05-26 12:29:21.565431 lndb-0.46a1/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-26 12:29:21.565498 lndb-0.46a1/lndb/test/_env.py
+-rw-r--r--   0        0        0     3913 2023-05-28 13:35:53.149022 lndb-0.46a1/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-05-26 12:29:21.565658 lndb-0.46a1/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      254 2023-05-28 13:35:53.149174 lndb-0.46a1/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-05-26 12:29:21.565795 lndb-0.46a1/lndb/test/nox.py
+-rw-r--r--   0        0        0     2802 2023-05-31 19:24:00.352440 lndb-0.46a1/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lndb-0.46a1/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lndb-0.46a1/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lndb-0.46a1/lnschema-core/.gitignore
+-rw-r--r--   0        0        0       73 2023-05-30 14:21:30.384608 lndb-0.46a1/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lndb-0.46a1/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lndb-0.46a1/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lndb-0.46a1/lnschema-core/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.384908 lndb-0.46a1/lnschema-core/django_project/__init__.py
+-rw-r--r--   0        0        0      404 2023-05-30 14:21:30.384975 lndb-0.46a1/lnschema-core/django_project/asgi.py
+-rw-r--r--   0        0        0     3572 2023-05-30 14:21:30.385044 lndb-0.46a1/lnschema-core/django_project/settings.py
+-rw-r--r--   0        0        0      770 2023-05-30 14:21:30.385110 lndb-0.46a1/lnschema-core/django_project/urls.py
+-rw-r--r--   0        0        0      404 2023-05-30 14:21:30.385276 lndb-0.46a1/lnschema-core/django_project/wsgi.py
+-rw-r--r--   0        0        0    24348 2023-05-31 19:31:21.507267 lndb-0.46a1/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-05-31 12:00:39.299258 lndb-0.46a1/lnschema-core/docs/guide/0-core-schema.ipynb
+-rw-r--r--   0        0        0     8386 2023-05-31 12:00:39.320747 lndb-0.46a1/lnschema-core/docs/guide/1-data-validation.ipynb
+-rw-r--r--   0        0        0       68 2023-05-30 14:21:30.385923 lndb-0.46a1/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lndb-0.46a1/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lndb-0.46a1/lnschema-core/lamin-project.yaml
+drwxr-xr-x   0        0        0        0 2023-05-30 14:21:30.386114 lndb-0.46a1/lnschema-core/lndb/
+-rw-r--r--   0        0        0      869 2023-05-31 19:30:02.377807 lndb-0.46a1/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0    24667 2023-05-31 19:24:00.353470 lndb-0.46a1/lnschema-core/lnschema_core/_core.py
+-rw-r--r--   0        0        0     1514 2023-05-30 14:21:30.386812 lndb-0.46a1/lnschema-core/lnschema_core/_link.py
+-rw-r--r--   0        0        0      228 2023-05-30 14:21:30.386885 lndb-0.46a1/lnschema-core/lnschema_core/_timestamps.py
+-rw-r--r--   0        0        0      923 2023-05-31 19:24:00.353681 lndb-0.46a1/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      331 2023-05-31 19:24:00.354019 lndb-0.46a1/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0      100 2023-05-30 14:21:30.387077 lndb-0.46a1/lnschema-core/lnschema_core/apps.py
+-rw-r--r--   0        0        0      313 2023-05-30 14:21:30.387173 lndb-0.46a1/lnschema-core/lnschema_core/dev/__init__.py
+-rw-r--r--   0        0        0     2477 2023-05-30 14:21:30.387427 lndb-0.46a1/lnschema-core/lnschema_core/dev/_id.py
+-rw-r--r--   0        0        0     1075 2023-05-30 14:21:30.387523 lndb-0.46a1/lnschema-core/lnschema_core/dev/_versions.py
+-rw-r--r--   0        0        0      579 2023-05-30 14:21:30.387597 lndb-0.46a1/lnschema-core/lnschema_core/dev/id.py
+-rw-r--r--   0        0        0    14699 2023-05-30 14:21:30.387708 lndb-0.46a1/lnschema-core/lnschema_core/dev/sqlmodel.py
+-rw-r--r--   0        0        0      227 2023-05-30 14:21:30.387777 lndb-0.46a1/lnschema-core/lnschema_core/link.py
+-rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.387839 lndb-0.46a1/lnschema-core/lnschema_core/manage.py
+-rw-r--r--   0        0        0     9699 2023-05-31 19:24:00.354344 lndb-0.46a1/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lndb-0.46a1/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0     3694 2023-05-30 14:21:30.388217 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
+-rw-r--r--   0        0        0     6580 2023-05-30 14:21:30.388467 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
+-rw-r--r--   0        0        0     2073 2023-05-30 14:21:30.388554 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
+-rw-r--r--   0        0        0     4358 2023-05-30 14:21:30.388622 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
+-rw-r--r--   0        0        0     3333 2023-05-30 14:21:30.388701 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
+-rw-r--r--   0        0        0      817 2023-05-30 14:21:30.388767 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
+-rw-r--r--   0        0        0      536 2023-05-30 14:21:30.388831 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
+-rw-r--r--   0        0        0      976 2023-05-30 14:21:30.388893 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
+-rw-r--r--   0        0        0     6332 2023-05-30 14:21:30.388963 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
+-rw-r--r--   0        0        0     2886 2023-05-30 14:21:30.389027 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
+-rw-r--r--   0        0        0      762 2023-05-30 14:21:30.389088 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
+-rw-r--r--   0        0        0      668 2023-05-30 14:21:30.389149 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
+-rw-r--r--   0        0        0     1082 2023-05-30 14:21:30.389209 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py
+-rw-r--r--   0        0        0     1725 2023-05-30 14:21:30.389276 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py
+-rw-r--r--   0        0        0      613 2023-05-30 14:21:30.389356 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py
+-rw-r--r--   0        0        0      646 2023-05-30 14:21:30.389424 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py
+-rw-r--r--   0        0        0     3507 2023-05-30 14:21:30.389485 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py
+-rw-r--r--   0        0        0     2344 2023-05-30 14:21:30.389548 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py
+-rw-r--r--   0        0        0     8560 2023-05-30 14:21:30.389626 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py
+-rw-r--r--   0        0        0     4792 2023-05-30 14:21:30.389844 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py
+-rw-r--r--   0        0        0     4603 2023-05-30 14:21:30.389927 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py
+-rw-r--r--   0        0        0     1209 2023-05-30 14:21:30.390122 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py
+-rw-r--r--   0        0        0     2202 2023-05-30 14:21:30.390229 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py
+-rw-r--r--   0        0        0     1098 2023-05-30 14:21:30.390300 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py
+-rw-r--r--   0        0        0     1229 2023-05-30 14:21:30.390371 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py
+-rw-r--r--   0        0        0     3580 2023-05-30 14:21:30.390448 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py
+-rw-r--r--   0        0        0      593 2023-05-30 14:21:30.390525 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py
+-rw-r--r--   0        0        0      973 2023-05-30 14:21:30.390584 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py
+-rw-r--r--   0        0        0     1120 2023-05-30 14:21:30.390641 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py
+-rw-r--r--   0        0        0     1067 2023-05-30 14:21:30.390699 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py
+-rw-r--r--   0        0        0     1712 2023-05-30 14:21:30.390788 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py
+-rw-r--r--   0        0        0      483 2023-05-30 14:21:30.390866 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-23-3dd9f8d41861-v0_28_3.py
+-rw-r--r--   0        0        0      581 2023-05-30 14:21:30.390932 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py
+-rw-r--r--   0        0        0      778 2023-05-30 14:21:30.390997 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py
+-rw-r--r--   0        0        0     5367 2023-05-30 14:21:30.391066 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py
+-rw-r--r--   0        0        0     6957 2023-05-30 14:21:30.391136 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py
+-rw-r--r--   0        0        0     1658 2023-05-30 14:21:30.391214 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py
+-rw-r--r--   0        0        0      780 2023-05-30 14:21:30.391283 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py
+-rw-r--r--   0        0        0     4440 2023-05-30 14:21:30.391353 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py
+-rw-r--r--   0        0        0     3782 2023-05-30 14:21:30.391419 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py
+-rw-r--r--   0        0        0     8841 2023-05-30 14:21:30.391507 lndb-0.46a1/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py
+-rw-r--r--   0        0        0    16439 2023-05-31 19:24:00.354775 lndb-0.46a1/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      205 2023-05-30 14:21:30.391658 lndb-0.46a1/lnschema-core/lnschema_core/types.py
+-rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.391734 lndb-0.46a1/lnschema-core/manage.py
+-rw-r--r--   0        0        0     1260 2023-05-31 19:24:00.355143 lndb-0.46a1/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      945 2023-05-31 19:24:00.355513 lndb-0.46a1/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-05-30 14:21:30.392094 lndb-0.46a1/lnschema-core/tests/test_migrations.py
+-rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lndb-0.46a1/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2297 2023-05-31 20:04:49.370954 lndb-0.46a1/noxfile.py
+-rw-r--r--   0        0        0     1289 2023-05-31 20:11:41.676020 lndb-0.46a1/pyproject.toml
+-rw-r--r--   0        0        0      645 2023-05-31 19:23:44.389708 lndb-0.46a1/tests/test_bionty.py
+-rw-r--r--   0        0        0     2900 2023-05-31 19:23:44.389984 lndb-0.46a1/tests/test_init_instance.py
+-rw-r--r--   0        0        0      659 2023-05-31 19:23:44.390213 lndb-0.46a1/tests/test_load_instance.py
+-rw-r--r--   0        0        0      231 2023-05-31 19:23:44.390411 lndb-0.46a1/tests/test_set_storage.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 lndb-0.46a1/PKG-INFO
```

### Comparing `lndb-0.45a4/.github/workflows/build.yml` & `lndb-0.46a1/lnschema-core/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,83 @@
 name: build
 
 on:
   push:
-    branches: [main, staging]
+    branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
   build:
     runs-on: ubuntu-22.04
     env:
       GITHUB_EVENT_NAME: ${{ github.event_name }}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
-    timeout-minutes: 20
+    timeout-minutes: 15
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
+          submodules: recursive
           fetch-depth: 0
       - name: Checkout lndocs
         uses: actions/checkout@v3
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
-      - name: Setup Python
-        uses: actions/setup-python@v4
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
-      - name: Cache nox
-        uses: actions/cache@v3
-        with:
-          path: .nox
-          key: nox-${{ runner.os }}
-      - name: Cache pre-commit
+      - name: cache pre-commit
         uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
-      - name: Cache postgres
+      - name: cache postgres
         id: cache-postgres
         uses: actions/cache@v3
         with:
           path: ~/postgres.tar
           key: cache-postgres-0
-      - name: Cache postgres miss
+      - name: cache postgres miss
         if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
-      - name: Cache postgres use
+      - name: cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
-      - name: Install Python dependencies
+      - name: install Python deps
         run: |
           python -m pip install -U pip
-          pip install lamindb>=0.41a3
-      - name: Install apt-get dependencies
+          pip install laminci
+      - name: install apt-get deps
         run: |
           sudo apt-get -y install graphviz
-          sudo apt-get install sqlite3-tools=3.37.2-2
           sudo apt-get install libpq-dev
-      - name: Lint
-        run: |
-          nox -s lint
       - name: Configure AWS
-        uses: aws-actions/configure-aws-credentials@v2
+        uses: aws-actions/configure-aws-credentials@v1
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
-      - name: Configure Google Cloud
-        id: "auth"
-        uses: "google-github-actions/auth@v0"
-        with:
-          credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
-      - name: "Set up Cloud SDK"
-        uses: "google-github-actions/setup-gcloud@v0"
-      - name: Build
-        run: |
-          nox -s build --python ${{ matrix.python-version }}
-        env:
-          GITHUB_EVENT_NAME: ${{ github.event_name }}
-          SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
-          SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
+      # - run: nox -s lint
+      - run: nox -s install
+      - run: nox -s build
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
-      - name: Read lamin-project.yaml
-        if: matrix.python-version == '3.9'
-        id: lamin-project
-        uses: CumulusDS/get-yaml-paths-action@v0.1.0
-        with:
-          file: lamin-project.yaml
-          project_slug: project_slug
       - name: Deploy docs
         if: matrix.python-version == '3.9'
         id: netlify
         uses: nwtgck/actions-netlify@v1.2
         with:
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
```

### Comparing `lndb-0.45a4/.github/workflows/latest-changes.yml` & `lndb-0.46a1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/.gitignore` & `lndb-0.46a1/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/.pre-commit-config.yaml` & `lndb-0.46a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/LICENSE` & `lndb-0.46a1/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/docs/changelog.md` & `lndb-0.46a1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Add Django backend | [388](https://github.com/laminlabs/lndb/pull/388) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.46a1
+♻️ Refactor CI | [387](https://github.com/laminlabs/lndb/pull/387) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 | 0.45.0
+🐛 Unlock on uncaught exceptions in ipython | [386](https://github.com/laminlabs/lndb/pull/386) | [Koncopd](https://github.com/Koncopd) | 2023-05-30 |
 ⬆️ Upgrade to lnhub-rest 0.9.8 | [384](https://github.com/laminlabs/lndb/pull/384) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a4
 ⬆️ Upgrade lnhub-rest to 0.9.7 | [383](https://github.com/laminlabs/lndb/pull/383) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a3
 📝 Add setup overview from lamindb | [382](https://github.com/laminlabs/lndb/pull/382) | [falexwolf](https://github.com/falexwolf) | 2023-05-27 |
 🔥 Remove schema modules logic from `setup_schema` | [381](https://github.com/laminlabs/lndb/pull/381) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.45a2
 🏗️ Remove SQL-level schema modules | [380](https://github.com/laminlabs/lndb/pull/380) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.45a1
 ✨ Add track command to CLI | [378](https://github.com/laminlabs/lndb/pull/378) | [Koncopd](https://github.com/Koncopd) | 2023-05-23 |
 📝 Improve migration docs | [379](https://github.com/laminlabs/lndb/pull/379) | [Zethson](https://github.com/Zethson) | 2023-05-22 |
```

### Comparing `lndb-0.45a4/docs/faq/check-synchronization.ipynb` & `lndb-0.46a1/docs/faq/check-synchronization.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876612103174603%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 4: {'source': ['init(\\n', '    "*

 * *            'storage="s3://lndb-setup-ci",\\n\', \'    name=instance_name,\\n\', \')\']}, 5: '*

 * *            "{'attachments': OrderedDict()}, 10: {'attachments': OrderedDict()}, 13: "*

 * *            "{'attachments': OrderedDict()}, 16: {'attachments': OrderedDict()}, insert: [(1, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', '6e685a68'), "*

 * *            "('metadata', OrderedDict()), ('outputs', […]*

```diff
@@ -1,20 +1,35 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "404d7543",
             "metadata": {},
             "source": [
                 "# Check synchronization of local and cloud sqlite databases"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "6e685a68",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import lndb\n",
+                "\n",
+                "group = \"django\" if lndb._USE_DJANGO else \"sqlalchemy\"\n",
+                "instance_name = f\"lamindb-setup-ci-{group}\"\n",
+                "!lamin delete {instance_name}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "f906c3b7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lndb import login, init, settings, delete\n",
                 "import os"
             ]
@@ -32,18 +47,22 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b651f6da",
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"s3://lndb-setup-ci\")"
+                "init(\n",
+                "    storage=\"s3://lndb-setup-ci\",\n",
+                "    name=instance_name,\n",
+                ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "9256886a",
             "metadata": {},
             "source": [
                 "Get the paths to the cloud and local sqlite databases."
             ]
         },
@@ -84,14 +103,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "cache_file"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "26d8bd48",
             "metadata": {},
             "source": [
                 "Delete the local sqlite database file."
             ]
         },
@@ -112,14 +132,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert not cache_file.exists()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "27bd0aac",
             "metadata": {},
             "source": [
                 "Access to the session restores the local version of sqlite database by downloading it from the cloud."
             ]
         },
@@ -140,14 +161,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert cache_file.exists()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "dc5f6ac8",
             "metadata": {},
             "source": [
                 "If the local sqlite database is older than the cloud one, the cloud database replaces the local sqlite database file."
             ]
         },
@@ -236,15 +258,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
     },
```

### Comparing `lndb-0.45a4/docs/faq/clone.ipynb` & `lndb-0.46a1/docs/faq/clone.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768518518518519%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: {'source': "*

 * *            "{insert: [(0, 'import lndb\\n')]}}, 3: {'attachments': OrderedDict()}, 4: {'source': "*

 * *            '[\'if not lndb._USE_DJANGO:\\n\', \'    init(storage="s3://lamin-site-assets")\']}, '*

 * *            "5: {'source': ['if not lndb._USE_DJANGO:\\n', '    clone_test()']}, 6: "*

 * *            "{'attachments': OrderedDict()}, 8: {'attachments': OrderedDict()}, 9: {'source': ['if "*

 * *            "not lndb._USE […]*

```diff
@@ -1,61 +1,68 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Clone a shallow copy of an instance for testing"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The function `clone_test` demonstrated below clones a shallow copy (last 20 rows of each table) of the current instance and returns the connection url to the test instance clone.\n",
                 "\n",
                 "Alternatively, one can pass an `InstanceSettings` object."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import lndb\n",
                 "from lndb import init, settings\n",
                 "from lndb.dev._clone import clone_test"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## A remote SQLite instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"s3://lamin-site-assets\")"
+                "if not lndb._USE_DJANGO:\n",
+                "    init(storage=\"s3://lamin-site-assets\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "clone_test()"
+                "if not lndb._USE_DJANGO:\n",
+                "    clone_test()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Clean up the test instance."
             ]
         },
         {
@@ -64,39 +71,33 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "!rm -r lamin-site-assets_test"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Alternative way of calling `clone_test`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "isettings = settings.instance"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "clone_test(isettings)"
+                "if not lndb._USE_DJANGO:\n",
+                "    clone_test(settings.instance)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Clean up the test instance."
             ]
         },
         {
@@ -105,14 +106,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "!rm -r lamin-site-assets_test"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## A postgres instance"
             ]
         },
         {
@@ -130,14 +132,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# clone_test()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Clean up:"
             ]
         },
         {
```

### Comparing `lndb-0.45a4/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.46a1/docs/guide/00-index.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9249395419301415%*

 * *Differences: {"'cells'": "{0: {'source': ['# Guide']}, 1: {'cell_type': 'markdown', 'source': {insert: [(0, "*

 * *            "'Set up a LaminDB instance either using the CLI (`lamin`) or the Python API "*

 * *            "({mod}`docs:lamindb.setup`).\\n'), (2, '```{toctree}\\n'), (3, ':maxdepth: 1\\n'), "*

 * *            "(4, ':hidden:\\n'), (5, '\\n'), (6, 'setup-user\\n'), (7, 'init-instance\\n'), (8, "*

 * *            "'load-instance\\n'), (9, 'set-storage\\n'), (10, 'schema-modules\\n'), (11, "*

 * *            "'migrate\\n'), (12, '``` […]*

```diff
@@ -1,377 +1,385 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Edge cases for login, init, load"
+                "# Guide"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import lamindb.setup as lnsetup\n",
-                "from lamindb.setup import settings\n",
-                "from lndb.dev._settings_store import (\n",
-                "    current_instance_settings_file,\n",
-                "    current_user_settings_file,\n",
-                "    get_settings_file_name_prefix,\n",
-                "    settings_dir,\n",
-                ")\n",
-                "from laminci.db import setup_local_test_postgres\n",
-                "from lndb.dev._settings_store import instance_settings_file\n",
-                "import nbproject\n",
-                "import pytest\n",
-                "import os\n",
+                "Set up a LaminDB instance either using the CLI (`lamin`) or the Python API ({mod}`docs:lamindb.setup`).\n",
+                "\n",
+                "```{toctree}\n",
+                ":maxdepth: 1\n",
+                ":hidden:\n",
                 "\n",
-                "nbproject.header()"
+                "setup-user\n",
+                "init-instance\n",
+                "load-instance\n",
+                "set-storage\n",
+                "schema-modules\n",
+                "migrate\n",
+                "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Log in with in-sufficient information"
+                "If you use the CLI, you can access help like so:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with pytest.raises(TypeError):\n",
-                "    lnsetup.login()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "If we add an email or handle it looks up the password from the stored env file (`lamin login testuser1@lamin.ai`):"
+                "!lamin -h"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lnsetup.login(\"testuser1@lamin.ai\")"
+                "!lamin init -h"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now, let's start with a fresh environment without any user profiles stored."
+                "## Sign up and log in"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "(\n",
-                "    settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1@lamin.ai.env\"\n",
-                ").unlink()\n",
-                "(settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1.env\").unlink()\n",
-                "current_user_settings_file().unlink()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "If we try to login with a handle at first login, this will error:"
+                "# in case an instance is open\n",
+                "!lamin close"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with pytest.raises(RuntimeError):\n",
-                "    lnsetup.login(\"testuser1\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\")"
+                "import lamindb as ln"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If we try to login without password, this will error:"
+                "```{code}\n",
+                "\n",
+                "ln.setup.signup(\"testuser1@lamin.ai\")  # CLI: lamin signup testuser1@lamin.ai\n",
+                "```\n",
+                "This will generate a password and cache both email and password in your `~/.lamin` directory. \n",
+                "\n",
+                "\ud83d\udce7 You will also receive a confirmation email with a link to choose your user handle and complete the sign-up!"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "with pytest.raises(RuntimeError):\n",
-                "    lnsetup.login(\"testuser1@lamin.ai\")"
+                "You can log in with either email or handle:"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If we try login with a wrong password, this will error:"
+                "```\n",
+                "ln.setup.login(\"testuser1@lamin.ai\")  # CLI: lamin login testuser1@lamin.ai\n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = lnsetup.login(\"testuser1@lamin.ai\", password=\"hello\")\n",
-                "assert result == \"could-not-login\""
+                "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Hence, we need to login once with email and password:"
+                "If you don't have a cached password in your environment, you need to pass it to the `login()` function:\n",
+                "```{code}\n",
+                "ln.setup.login(\"<email>\", password=\"<password>\")  # CLI: lamin login <email> --password <password>\n",
+                "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "result = lnsetup.login(\n",
-                "    \"testuser1@lamin.ai\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
-                ")\n",
-                "assert result is None"
+                "## Init an instance"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "And now we can have the convenient login just with the handle."
+                "The most common arguments for `lamin init` are the following:\n",
+                "\n",
+                "- `storage`: a storage location\n",
+                "    - local storage: path to a local directory\n",
+                "    - cloud storage: `s3://my-bucket` or `gs://my-bucket`\n",
+                "- `db` (optional): a SQL database URI\n",
+                "    - if not passed, the instance will use a SQLite database    \n",
+                "- `schema` (optional): schema modules\n",
+                "    - any instance uses the core schema module\n",
+                "    - there are 2 public schema modules:\n",
+                "        - [`bionty`](https://lamin.ai/docs/lnschema-bionty): biological entities\n",
+                "        - [`lamin1`](https://lamin.ai/docs/lnschema-lamin1): Lamin's sample biolab schema\n",
+                "    - [contact us](https://lamin.ai/contact) to learn about customized enterprise schema modules"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "result = lnsetup.login(\"testuser1\")\n",
-                "assert result is None"
+                "### Examples"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Configuration with insufficient information"
+                "#### Local storage + SQLite"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If you are only interested in tracking files and their transformations, init your local SQLite instance via:\n",
+                "\n",
+                "```\n",
+                "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata\n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "current_user_settings_file().unlink()"
+                "ln.setup.init(storage=\"./mydata\")\n",
+                "# ln.setup.init(\n",
+                "#     storage=\"./mydata\", schema=\"bionty,lamin1\"\n",
+                "# )  # CLI: lamin init --storage mydata --schema bionty,lamin1"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We'd also get an error about not being logged in if we try to init an instance without it being set:"
+                "#### Cloud storage (S3) + SQLite"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "with pytest.raises(RuntimeError):\n",
-                "    lnsetup.init(storage=\"mydata\")"
+                "```\n",
+                "ln.setup.init(storage=\"s3://<bucket_name>\", schema=\"bionty,lamin1\")  # CLI: lamin init --storage s3://<bucket_name> --schema bionty,lamin1\n",
+                "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let's log in again."
+                "#### Cloud storage (GCP) + Postgres"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "result = lnsetup.login(\"testuser1\")\n",
-                "assert result is None"
+                "```\n",
+                "ln.setup.init(storage=\"gs://<bucket_name>\", db=\"postgresql://<user>:<pwd>@<hostname>:<port>/<dbname>\", schema=\"bionty,lamin1\")  # CLI: lamin init --storage gs://<bucket_name> --db postgresql://<user>:<pwd>@<hostname>:<port>/<dbname> --schema bionty,lamin1\n",
+                "```\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let's now try to init without providing storage (`lamin init`):"
+                "## Load an instance"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "with pytest.raises(TypeError):\n",
-                "    lnsetup.init()"
+                "Load your own instance:\n",
+                "```\n",
+                "ln.setup.load(\"<instance_name>\")  # CLI: lamin load <instance_name>\n",
+                "````"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "However, if we set a location (`lamin init --storage \"mydata\"`)"
+                "Load somebody else's instance:\n",
+                "```\n",
+                "ln.setup.load(f\"{account_handle}/{instance_name}\")  # CLI: lamin load <account_handle/instance_name>\n",
+                "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "lnsetup.init(storage=\"mydata\")"
+                "## Get info"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Local instances can not be loaded via the hub"
+                "Settings persist in `~/.lamin/` and can be accessed via {class}`docs:`lamindb.setup.settings`."
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "It's not possible to load an instance from the hub if it has a local component, say, local storage."
+                "ln.setup.info()  # CLI: lamin info"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lnsetup.init(storage=\"local_storage_instance\")\n",
-                "instance_settings_file(\"local_storage_instance\", \"testuser1\").unlink()"
+                "ln.setup.settings.user"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert lnsetup.load(\"local_storage_instance\") == \"instance-not-reachable\""
+                "ln.setup.settings.instance"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "It's not possible to load an instance from the hub if it's using a local db."
+                "```{note}\n",
+                "\n",
+                "The user who creates an instance is its owner. Ownership can be transferred in the hub.\n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pgurl = setup_local_test_postgres(\"pgtest_remote_storage\")"
+                "ln.setup.settings.instance.owner"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lnsetup.init(\n",
-                "    storage=\"s3://lndb-setup-ci-pgtest-remote\", db=pgurl, name=\"pgtest_remote_storage\"\n",
-                ")\n",
-                "instance_settings_file(\"pgtest_remote_storage\", \"testuser1\").unlink()"
+                "ln.setup.settings.instance.identifier"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert lnsetup.load(\"pgtest_remote_storage\") == \"instance-not-reachable\""
+                "ln.setup.settings.instance.db"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "!docker stop pgtest_remote_storage && docker rm pgtest_remote_storage"
+                "ln.setup.settings.storage.root"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Invalid command"
+                "## Delete an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!lamin invalid"
+                "ln.setup.delete(\"mydata\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -385,26 +393,16 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.15"
         },
-        "nbproject": {
-            "id": "vLOmzd6d4Jow",
-            "parent": null,
-            "pypackage": null,
-            "time_init": "2023-01-20T15:25:50.335298+00:00",
-            "user_handle": "falexwolf",
-            "user_id": "FBa7SHjn",
-            "user_name": "Alex Wolf",
-            "version": "0"
-        },
         "vscode": {
             "interpreter": {
-                "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lndb-0.45a4/docs/faq/manage-migrations.ipynb` & `lndb-0.46a1/docs/faq/manage-migrations.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'attachments': OrderedDict()}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Manage migrations"
             ]
         },
         {
@@ -13,14 +14,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lndb"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Running the following on the CLI\n",
                 "```\n",
                 "lamin migrate generate\n",
                 "```\n",
```

### Comparing `lndb-0.45a4/docs/faq/switch-environment.ipynb` & `lndb-0.46a1/docs/faq/switch-environment.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951554232804233%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'source': {insert: [(3, "*

 * *            "'user_access_token_prod = settings.user.access_token\\n'), (4, '!lamin delete "*

 * *            "mydata_prod')], delete: [3]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Test switch environment"
@@ -28,15 +29,16 @@
             "id": "a9cbc2b8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "login(\"testuser1@lamin.ai\")\n",
                 "init(storage=\"mydata_prod\")\n",
                 "\n",
-                "user_access_token_prod = settings.user.access_token"
+                "user_access_token_prod = settings.user.access_token\n",
+                "!lamin delete mydata_prod"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a5e8a0a6",
             "metadata": {},
@@ -127,15 +129,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
             }
         }
     },
```

### Comparing `lndb-0.45a4/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.46a1/docs/faq/test-migrations-e2e.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703705%*

 * *Differences: {"'cells'": "{4: {'source': ['if not lndb._USE_DJANGO:\\n', '    "*

 * *            'lndb.test.migrate_clone(storage="s3://lamin-site-assets")\']}, 5: {\'source\': [\'if '*

 * *            'not lndb._USE_DJANGO:\\n\', \'    lndb.delete("lamin-site-assets_test")\']}, 6: '*

 * *            "{'source': ['if not lndb._USE_DJANGO:\\n', '    "*

 * *            'lndb.test.migrate_clones("lnschema_core", n_instances=1, dialect_name="sqlite")\']}, '*

 * *            "8: {'source': ['if not lndb._USE_DJANGO:\\n', '    lndb.test.migrate_clone […]*

```diff
@@ -42,39 +42,42 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2fe506c7-9788-4f04-8d12-a5a855a81db0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lndb.test.migrate_clone(storage=\"s3://lamin-site-assets\")"
+                "if not lndb._USE_DJANGO:\n",
+                "    lndb.test.migrate_clone(storage=\"s3://lamin-site-assets\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8f16a4b4-e165-4df3-af1b-592796b9bca5",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "lndb.delete(\"lamin-site-assets_test\")"
+                "if not lndb._USE_DJANGO:\n",
+                "    lndb.delete(\"lamin-site-assets_test\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f1f43b5a-59ca-419a-8ed1-9672f2ff2025",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lndb.test.migrate_clones(\"lnschema_core\", n_instances=1, dialect_name=\"sqlite\")"
+                "if not lndb._USE_DJANGO:\n",
+                "    lndb.test.migrate_clones(\"lnschema_core\", n_instances=1, dialect_name=\"sqlite\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e53c8996-73a1-4c5f-b54f-4ea9ea117702",
             "metadata": {},
@@ -85,17 +88,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd10731f-5667-4550-99db-90fb47e92c32",
             "metadata": {},
             "outputs": [],
             "source": [
-                "lndb.test.migrate_clone(\n",
-                "    db=\"postgresql://batman:robin@35.222.187.204:5432/lamindata\", schema=\"bionty,lamin1\"\n",
-                ")"
+                "if not lndb._USE_DJANGO:\n",
+                "    lndb.test.migrate_clone(\n",
+                "        db=\"postgresql://batman:robin@35.222.187.204:5432/lamindata\",\n",
+                "        schema=\"bionty,lamin1\",\n",
+                "    )"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "py39",
             "language": "python",
```

### Comparing `lndb-0.45a4/docs/faq/test-migrations-unit.ipynb` & `lndb-0.46a1/docs/faq/test-migrations-unit.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}}"}*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "558d9dfc-e367-4406-b8df-c67647385e76",
             "metadata": {},
             "source": [
                 "# Test migrations unit"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "4330bc99-65c0-491d-a750-f59d86278b98",
             "metadata": {},
             "source": [
                 "Let us first mimic what happens inside a noxfile in a schema module. We set up a reference instance:"
             ]
         },
```

### Comparing `lndb-0.45a4/docs/guide/00-index.ipynb` & `lndb-0.46a1/lnschema-core/docs/guide/1-data-validation.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9069437741312741%*

 * *Differences: {"'cells'": "{0: {'source': ['# Data validation with ORMs']}, 1: {'source': {insert: [(0, 'LaminDB "*

 * *            'implements data validation at the ORM level by fully integrating the SQLModel ORM '*

 * *            'with pydantic type checking.\\n\'), (2, "Let\'s take a look at data validation '*

 * *            'behavior in LaminDB.")], delete: [12, 11, 10, 9, 8, 7, 6, 4, 3, 2, 1, 0]}}, 2: '*

 * *            "{'source': ['import lamindb as ln\\n', 'import lamindb.schema as lns\\n', 'import "*

 * *            "pytest\\n', 'fro […]*

```diff
@@ -1,369 +1,323 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Guide"
+                "# Data validation with ORMs"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Set up a LaminDB instance either using the CLI (`lamin`) or the Python API ({mod}`docs:lamindb.setup`).\n",
+                "LaminDB implements data validation at the ORM level by fully integrating the SQLModel ORM with pydantic type checking.\n",
                 "\n",
-                "```{toctree}\n",
-                ":maxdepth: 1\n",
-                ":hidden:\n",
-                "\n",
-                "setup-user\n",
-                "init-instance\n",
-                "load-instance\n",
-                "set-storage\n",
-                "schema-modules\n",
-                "migrate\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "If you use the CLI, you can access help like so:"
+                "Let's take a look at data validation behavior in LaminDB."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!lamin -h"
+                "import lamindb as ln\n",
+                "import lamindb.schema as lns\n",
+                "import pytest\n",
+                "from pydantic import ValidationError"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!lamin init -h"
+                "## Missing required field"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Sign up and log in"
+                "Let's create a `User` instance without the required `email` and `handle` fields."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln"
+                "with pytest.raises(ValidationError) as e:\n",
+                "    exception = e\n",
+                "    user_missing = lns.User(id=\"123\")\n",
+                "print(exception.exconly())"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "```{code}\n",
-                "\n",
-                "ln.setup.signup(\"testuser1@lamin.ai\")  # CLI: lamin signup testuser1@lamin.ai\n",
-                "```\n",
-                "This will generate a password and cache both email and password in your `~/.lamin` directory. \n",
-                "\n",
-                "\ud83d\udce7 You will also receive a confirmation email with a link to choose your user handle and complete the sign-up!"
+                "## Field type error"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You can log in with either email or handle:"
+                "Let's create a `Transform` instance with the wrong type for the optional field `name`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1@lamin.ai\")  # CLI: lamin login testuser1@lamin.ai"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "If you don't have a cached password in your environment, you need to pass it to the `login()` function:\n",
-                "```{code}\n",
-                "ln.setup.login(\"<email>\", password=\"<password>\")  # CLI: lamin login <email> --password <password>\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Init an instance"
+                "from datetime import datetime\n",
+                "\n",
+                "with pytest.raises(ValidationError) as e:\n",
+                "    exception = e\n",
+                "    invalid_transform = ln.Transform(name=datetime.now())\n",
+                "print(exception.exconly())"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The most common arguments for `lamin init` are the following:\n",
-                "\n",
-                "- `storage`: a storage location\n",
-                "    - local storage: path to a local directory\n",
-                "    - cloud storage: `s3://my-bucket` or `gs://my-bucket`\n",
-                "- `db` (optional): a SQL database URI\n",
-                "    - if not passed, the instance will use a SQLite database    \n",
-                "- `schema` (optional): schema modules\n",
-                "    - any instance uses the core schema module\n",
-                "    - there are 2 public schema modules:\n",
-                "        - [`bionty`](https://lamin.ai/docs/lnschema-bionty): biological entities\n",
-                "        - [`lamin1`](https://lamin.ai/docs/lnschema-lamin1): Lamin's sample biolab schema\n",
-                "    - [contact us](https://lamin.ai/contact) to learn about customized enterprise schema modules"
+                "## Invalid categorical"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Examples"
+                "Let's pass an invalid categorical to the `type` field in `Usage`, which only accepts the values 'ingest', 'insert', 'select', 'update', 'delete', 'load', and 'link'."
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "#### Local storage + SQLite"
+                "from lnschema_core._core import SQLModel\n",
+                "from lnschema_core._types import Usage as UsageType\n",
+                "from sqlmodel import Field"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "If you are only interested in tracking files and their transformations, init your local SQLite instance via:\n",
-                "\n",
-                "```\n",
-                "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata\n",
-                "```"
+                "class Usage(SQLModel, table=True):  # type: ignore\n",
+                "    id: str = Field(default=None, primary_key=True)\n",
+                "    type: UsageType = Field(nullable=False, index=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(\n",
-                "    storage=\"./mydata\", schema=\"bionty,lamin1\"\n",
-                ")  # CLI: lamin init --storage mydata --schema bionty,lamin1"
+                "assert Usage(type=\"ingest\")"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "#### Cloud storage (S3) + SQLite"
+                "with pytest.raises(ValidationError) as e:\n",
+                "    exception = e\n",
+                "    invalid_usage = Usage(type=\"invalid categorical\")\n",
+                "print(exception.exconly())"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "```\n",
-                "ln.setup.init(storage=\"s3://<bucket_name>\", schema=\"bionty,lamin1\")  # CLI: lamin init --storage s3://<bucket_name> --schema bionty,lamin1\n",
-                "```"
+                "## Special cases"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Cloud storage (GCP) + Postgres"
+                "Data validation with the LaminDB ORM mirrors the standard Pydantic behavior, including variable casting (see example #1 below) and extra field behaviors (see example #2 below). These can be changed through Pydantic's configuration.\n",
+                "\n",
+                "The only difference in behavior between LaminDB and Pydantic is strict type checking for `Relationship` fields (see example #3 below), which is implemented in LaminDB."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "```\n",
-                "ln.setup.init(storage=\"gs://<bucket_name>\", db=\"postgresql://<user>:<pwd>@<hostname>:<port>/<dbname>\", schema=\"bionty,lamin1\")  # CLI: lamin init --storage gs://<bucket_name> --db postgresql://<user>:<pwd>@<hostname>:<port>/<dbname> --schema bionty,lamin1\n",
-                "```\n"
+                "### Argument casting"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Load an instance"
+                "LaminDB mirrors Pydantic's default behavior of casting input variables to conform to field types (see details in [Pydantic's documentation](https://docs.pydantic.dev/usage/models/#data-conversion)).\n",
+                "\n",
+                "Let's take a look at the default behavior by creating transform instances with `int` and `bool` inputs to the `name` field, which is string-typed in the schema."
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Load your own instance:\n",
-                "```\n",
-                "ln.setup.load(\"<instance_name>\")  # CLI: lamin load <instance_name>\n",
-                "````"
+                "# Name (int) is cast to str\n",
+                "transform_name_int_to_str = ln.Transform(name=1)\n",
+                "type(transform_name_int_to_str.name)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Load somebody else's instance:\n",
-                "```\n",
-                "ln.setup.load(f\"{account_handle}/{instance_name}\")  # CLI: lamin load <account_handle/instance_name>\n",
-                "```"
+                "# Name (bool) is cast to str\n",
+                "transform_name_bool_to_str = ln.Transform(name=True)\n",
+                "type(transform_name_int_to_str.name)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "## Get info"
+                "### Extra fields"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Settings persist in `~/.lamin/` and can be accessed via {class}`docs:`lamindb.setup.settings`."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.info()  # CLI: lamin info"
+                "LaminDB also mirror's Pydantic default behavior of accepting extra fields not defined in the schema."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.user"
+                "# No error is raised for the extra field\n",
+                "transform = ln.Transform(name=\"Test\", extra_field=\"This field is not defined in the schema\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "ln.setup.settings.instance.name"
+                "### Strict type checking for relationships"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "```{note}\n",
+                "Differently from Pydantic, LaminDB enforces strict type checking for `Relationship` fields.\n",
                 "\n",
-                "The user who creates an instance is its owner. Ownership can be transferred in the hub.\n",
-                "```"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.owner"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.identifier"
+                "Below is a simple example of Pydantic's lenient type checking for `Relationship` fields. Rather than enforcing the `Car` type in the `Wheel.car` field, it only enforces type-checking on the attributes of the input object."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.instance.db"
+                "from sqlmodel import SQLModel, Field, Relationship\n",
+                "from typing import Optional, List\n",
+                "\n",
+                "\n",
+                "class Car(SQLModel, table=False):\n",
+                "    id: str = Field(primary_key=True, default=None)\n",
+                "    name: str\n",
+                "\n",
+                "    wheels: List[\"Wheel\"] = Relationship()\n",
+                "\n",
+                "\n",
+                "class Wheel(SQLModel, table=False):\n",
+                "    id: str = Field(primary_key=True, default=None)\n",
+                "    name: str\n",
+                "\n",
+                "    car: Optional[\"Car\"] = Relationship()\n",
+                "\n",
+                "\n",
+                "class Bird(SQLModel, table=False):\n",
+                "    id: str = Field(primary_key=True, default=None)\n",
+                "    name: str"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.storage.root"
+                "# Pydantic does not raise a validation error for wrong type in the car field\n",
+                "wheel = Wheel(name=\"Test Wheel\", car=Bird(name=\"Test\"))"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Delete an instance"
+                "LaminDB, on the other hand, enforces strict type checking for `Relationships`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.delete(\"mydata\")"
+                "with pytest.raises(TypeError) as e:\n",
+                "    exception = e\n",
+                "    run = lns.Run(name=\"Test Run\", transform=Bird(name=\"This is not a Transform\"))\n",
+                "print(exception.exconly())"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -375,18 +329,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
-            }
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lndb-0.45a4/docs/guide/01-setup-user.ipynb` & `lndb-0.46a1/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/docs/guide/02-init-instance.ipynb` & `lndb-0.46a1/docs/guide/02-init-instance.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95281333463618%*

 * *Differences: {"'cells'": "{0: {'source': ['# Init & delete an instance']}, 2: {'source': ['import lamindb as "*

 * *            "ln']}, 10: {'source': ['If you want to register the instance on the hub at lamin.ai, "*

 * *            "use {func}`lamindb.setup.register`.']}, 11: {'source': ['from pathlib import "*

 * *            "Path\\n', '\\n', 'assert ln.setup.settings.instance.storage.is_cloud == False\\n', "*

 * *            "'assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\\n', "*

 * *            '\'assert ln.setup […]*

```diff
@@ -3,26 +3,37 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Init an instance"
+                "# Init & delete an instance"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
+            "source": [
+                "!lamin close"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln\n",
-                "from laminci.db import setup_local_test_postgres\n",
-                "from pathlib import Path"
+                "import lamindb as ln"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -56,23 +67,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!lamin delete mydata"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -86,23 +88,33 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.settings.instance"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If you want to register the instance on the hub at lamin.ai, use {func}`lamindb.setup.register`."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
+                "from pathlib import Path\n",
+                "\n",
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.name == \"mydata\"\n",
                 "assert ln.setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
                 "assert ln.setup.settings.storage.cache_dir is None\n",
                 "assert ln.setup.settings.storage.id is not None\n",
                 "assert (\n",
@@ -112,358 +124,237 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If you want to register it on the hub at lamin.ai, call:\n",
-                "```\n",
-                "ln.setup.register()\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Postgres"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "pgurl = setup_local_test_postgres()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "A connection string for postgres looks like this:"
+                "Assume we accidentally `init` an existing instance, it will be loaded:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pgurl"
+                "ln.setup.init(storage=\"mydata\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let us call init:"
+                "To delete an instance, call:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"./mydatapg\", db=pgurl)"
+                "ln.setup.delete(\"mydata\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.instance.name == \"pgtest\"\n",
-                "assert ln.setup.settings.instance.storage.is_cloud == False\n",
-                "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
-                "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
-                "assert ln.setup.settings.instance.db == pgurl\n",
-                "assert ln.setup.settings.storage.id is not None\n",
-                "assert (\n",
-                "    ln.setup.settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"mydatapg\").absolute().as_posix()\n",
-                ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None\n",
+                "from lndb.dev._settings_store import instance_settings_file\n",
                 "\n",
-                "!lamin delete pgtest\n",
-                "!docker stop pgtest && docker rm pgtest"
+                "settings_file = instance_settings_file(\"mydata\", \"testuser1\")\n",
+                "assert settings_file.exists() == False"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Custom instance name"
+                "### Postgres"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
-            "outputs": [],
             "source": [
-                "pgurl = setup_local_test_postgres()"
+                "```\n",
+                "from laminci.db import setup_local_test_postgres\n",
+                "pgurl = setup_local_test_postgres()\n",
+                "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
+                "A connection string for postgres looks like this:\n",
+                "```\n",
+                "'postgresql://postgres:pwd@0.0.0.0:5432/pgtest'\n",
+                "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(\n",
-                "    storage=\"./mystorage\", name=\"mydata2\", db=pgurl\n",
-                ")  # CLI: lamin init --storage ./mystorage --name \"mydata\" --db ..."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
             "source": [
-                "assert ln.setup.settings.instance.name == \"mydata2\"\n",
-                "assert ln.setup.settings.instance.storage.is_cloud == False\n",
-                "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
-                "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
-                "assert ln.setup.settings.instance.db == pgurl\n",
-                "assert ln.setup.settings.storage.id is not None\n",
-                "assert (\n",
-                "    ln.setup.settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"mystorage\").absolute().as_posix()\n",
-                ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None\n",
-                "\n",
-                "!lamin delete mydata2\n",
-                "!docker stop pgtest && docker rm pgtest"
+                "You can call init like so:"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Configure with cloud storage"
+                "```\n",
+                "ln.setup.init(storage=\"./mydatapg\", db='postgresql://postgres:pwd@0.0.0.0:5432/pgtest')  # CLI: lamin init --storage ./mystorage --db 'postgresql://postgres:pwd@0.0.0.0:5432/pgtest'\n",
+                "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### AWS"
+                "Your instance name will then be `pgtest`!"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You need to have access to AWS S3 via `awscli configure`."
+                "### Custom instance name"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let us look at the special case of an sqlite instance:"
+                "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
+                "```\n",
                 "ln.setup.init(\n",
-                "    storage=\"s3://lndb-setup-ci\"\n",
-                ")  # CLI: lamin init --storage \"s3://lndb-setup-ci\""
+                "    storage=\"./mystorage\", name=\"mydata2\", db=pgurl\n",
+                ")  # CLI: lamin init --storage ./mystorage --name \"mydata\" --db ...\n",
+                "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.setup.settings.instance"
+                "## Configure with cloud storage"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.setup.settings.instance._sqlite_file"
+                "### AWS"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance._sqlite_file_local"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
             "source": [
-                "# test\n",
-                "assert ln.setup.settings.storage.is_cloud == True\n",
-                "assert str(ln.setup.settings.storage.root) == \"s3://lndb-setup-ci/\"\n",
-                "assert ln.setup.settings.storage.region == \"us-east-1\"\n",
-                "assert (\n",
-                "    str(ln.setup.settings.instance._sqlite_file)\n",
-                "    == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
-                ")\n",
-                "assert ln.setup.settings.storage.id is not None\n",
-                "\n",
-                "# do the same for an S3 bucket in Europe\n",
-                "ln.setup.init(storage=\"s3://lndb-setup-ci-eu-central-1\", name=\"lndb-setup-ci-europe\")\n",
-                "assert ln.setup.settings.storage.region == \"eu-central-1\"\n",
-                "assert ln.setup.settings.instance.name == \"lndb-setup-ci-europe\"\n",
-                "assert (\n",
-                "    str(ln.setup.settings.instance._sqlite_file)\n",
-                "    == \"s3://lndb-setup-ci-eu-central-1/lndb-setup-ci-europe.lndb\"\n",
-                ")\n",
-                "assert ln.setup.settings.storage.id is not None\n",
-                "ln.setup.delete(\"lndb-setup-ci-europe\")"
+                "You need to have access to AWS S3 via `awscli configure`."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### GCP"
+                "Let us look at the special case of an sqlite instance:"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You need to authenticate for Google Clod.\n",
-                "\n",
-                "* Either, set the environment variable `export GOOGLE_APPLICATION_CREDENTIALS=<HOME-DIR>/.lndb/<GOOGLE CLOUD PROJECT>.json`.\n",
-                "* Alternatively, if you set up the `gcloud` CLI, log in with `gcloud auth application-default login`.\n"
+                "```\n",
+                "ln.setup.init(\n",
+                "    storage=\"s3://lndb-setup-ci\"\n",
+                ")  # CLI: lamin init --storage \"s3://lndb-setup-ci\"\n",
+                "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"gs://lndb-setup-ci-us\")"
+                "Under the hood, for an SQLite instance, LaminDB then keeps track of a cloud & and a synched local SQLite file:"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "ln.setup.delete(\"lndb-setup-ci-us\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# this should move up in this guide\n",
-                "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")\n",
-                "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)\n",
-                "ln.setup.register()"
+                "```\n",
+                "ln.setup.settings.instance._sqlite_file\n",
+                "ln.setup.settings.instance._sqlite_file_local\n",
+                "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Re-initialize an existing instance"
+                "### GCP"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Assume we accidentally `init` an existing instance, it will be loaded:"
+                "You need to authenticate for Google Clod.\n",
+                "\n",
+                "* Either, set the environment variable `export GOOGLE_APPLICATION_CREDENTIALS=<HOME-DIR>/.lndb/<GOOGLE CLOUD PROJECT>.json`.\n",
+                "* Alternatively, if you set up the `gcloud` CLI, log in with `gcloud auth application-default login`.\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "assert ln.setup.init(storage=\"mydata\") == \"migrate-unnecessary\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
             "source": [
-                "assert type(ln.setup.settings.storage.id)"
+                "```\n",
+                "ln.setup.init(storage=\"gs://lndb-setup-ci-us\")  # CLI: lamin init --storage \"gs://lndb-setup-ci-us\"\n",
+                "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.45a4/docs/guide/03-load-instance.ipynb` & `lndb-0.46a1/docs/faq/edge-cases-login-init.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7814463458994709%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, 'source': ['# Edge cases for login & "*

 * *            "init'], delete: ['id']}, 1: {delete: ['id']}, 2: {'source': {insert: [(0, 'import "*

 * *            "lamindb.setup as lnsetup\\n'), (2, 'from lndb.dev._settings_store import (\\n'), (3, "*

 * *            "'    current_instance_settings_file,\\n'), (4, '    current_user_settings_file,\\n'), "*

 * *            "(5, '    get_settings_file_name_prefix,\\n'), (6, '    settings_dir,\\n'), (7, "*

 * *            "')\\n'), (8, […]*

```diff
@@ -1,275 +1,263 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "source": [
-                "# Load & close an instance"
+                "# Edge cases for login & init"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "!lamin close"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "import pytest\n",
-                "import lamindb as ln\n",
+                "import lamindb.setup as lnsetup\n",
                 "from lamindb.setup import settings\n",
-                "from lndb.dev._settings_store import instance_settings_file"
+                "from lndb.dev._settings_store import (\n",
+                "    current_instance_settings_file,\n",
+                "    current_user_settings_file,\n",
+                "    get_settings_file_name_prefix,\n",
+                "    settings_dir,\n",
+                ")\n",
+                "from laminci.db import setup_local_test_postgres\n",
+                "from lndb.dev._settings_store import instance_settings_file\n",
+                "import pytest\n",
+                "import os"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "1be836bb",
             "metadata": {},
             "source": [
-                "## Load your own instance by name"
+                "## Log in with in-sufficient information"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "with pytest.raises(TypeError):\n",
+                "    lnsetup.login()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "a5c94e19",
             "metadata": {},
             "source": [
-                "If the user is the instance owner, just load the instance by name:"
+                "If we add an email or handle it looks up the password from the stored env file (`lamin login testuser1@lamin.ai`):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e7ecc665",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")  # CLI: lamin load mydata"
+                "lnsetup.login(\"testuser1@lamin.ai\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2276e0be",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "assert settings.instance.storage.is_cloud == False\n",
-                "assert settings.instance.name == \"mydata\"\n",
-                "assert (\n",
-                "    settings.instance.storage.root.as_posix() == Path(\"./mydata\").resolve().as_posix()\n",
-                ")\n",
-                "assert settings.instance.storage.cache_dir is None\n",
-                "assert (\n",
-                "    settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "Now, let's start with a fresh environment without any user profiles stored."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ac0d2b30",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# assume we move the storage location\n",
-                "!mv mydata mydata_new_loc\n",
-                "with pytest.raises(\n",
-                "    RuntimeError\n",
-                "):  # triggers because it does not find the SQLite file anymore\n",
-                "    ln.setup.load(\"mydata\")\n",
-                "# now account for the new storage location\n",
-                "ln.setup.load(\"mydata\", storage=\"./mydata_new_loc\")\n",
-                "assert (\n",
-                "    settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
-                ")\n",
-                "assert settings.instance.storage.cache_dir is None\n",
-                "assert (\n",
-                "    settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "(\n",
+                "    settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1@lamin.ai.env\"\n",
+                ").unlink()\n",
+                "(settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1.env\").unlink()\n",
+                "current_user_settings_file().unlink()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If we try to login with a handle at first login, this will error:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4f179b5b",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# another test case, this time with a manually configured instance name\n",
-                "ln.setup.load(\"pgtest-registered\")\n",
-                "assert settings.instance.storage.is_cloud == True\n",
-                "assert settings.instance.name == \"pgtest-registered\"\n",
-                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
+                "with pytest.raises(RuntimeError):\n",
+                "    lnsetup.login(\"testuser1\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "3f47a1d4",
             "metadata": {},
             "source": [
-                "This also works for remote instances:"
+                "If we try to login without password, this will error:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7c9698f9",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# ensure that the locally cached env file is deleted\n",
-                "instance_settings_file(\"lndb-setup-ci\", \"testuser1\").unlink()"
+                "with pytest.raises(RuntimeError):\n",
+                "    lnsetup.login(\"testuser1@lamin.ai\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If we try login with a wrong password, this will error:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "089a3832",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"lndb-setup-ci\")  # lamin load lndb-setup-ci"
+                "result = lnsetup.login(\"testuser1@lamin.ai\", password=\"hello\")\n",
+                "assert result == \"could-not-login\""
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Hence, we need to login once with email and password:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1ebd784f",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert settings.instance.storage.is_cloud == True\n",
-                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
-                "assert (\n",
-                "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
-                ")"
+                "result = lnsetup.login(\n",
+                "    \"testuser1@lamin.ai\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
+                ")\n",
+                "assert result is None"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "914af9a6",
             "metadata": {},
             "source": [
-                "## Load an instance from another owner"
+                "And now we can have the convenient login just with the handle."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "result = lnsetup.login(\"testuser1\")\n",
+                "assert result is None"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "65ab467e",
             "metadata": {},
             "source": [
-                "If you have the permission, you can load an instance from another owner. "
+                "## Configuration with insufficient information"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"testuser1/mydata\")  # lamin load \"testuser1/mydata\""
+                "current_user_settings_file().unlink()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "0986a5f3",
             "metadata": {},
             "source": [
-                "Load an instance from wrong owner."
+                "We'd also get an error about not being logged in if we try to init an instance without it being set:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bc3568ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
+                "with pytest.raises(Exception):\n",
+                "    lnsetup.init(storage=\"mydata\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "e3701120",
             "metadata": {},
             "source": [
-                "## Close an instance"
+                "Let's log in again."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e54d8cd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.close()"
+                "result = lnsetup.login(\"testuser1\")\n",
+                "assert result is None"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's now try to init without providing storage (`lamin init`):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "12db83b9-9d14-4575-876a-3d640a1c1e10",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# clean up\n",
-                "!lamin delete pgtest-registered\n",
-                "!docker stop pgtest-registered && docker rm pgtest-registered"
+                "with pytest.raises(TypeError):\n",
+                "    lnsetup.init()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -283,16 +271,26 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.15"
         },
+        "nbproject": {
+            "id": "vLOmzd6d4Jow",
+            "parent": null,
+            "pypackage": null,
+            "time_init": "2023-01-20T15:25:50.335298+00:00",
+            "user_handle": "falexwolf",
+            "user_id": "FBa7SHjn",
+            "user_name": "Alex Wolf",
+            "version": "0"
+        },
         "vscode": {
             "interpreter": {
-                "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
+                "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `lndb-0.45a4/docs/guide/04-set-storage.ipynb` & `lndb-0.46a1/docs/guide/04-set-storage.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9404083508403361%*

 * *Differences: {"'cells'": "{0: {'source': ['# Set storage']}, 1: {'id': '6422b64e', 'metadata': {replace: "*

 * *            "OrderedDict([('tags', ['hide-cell'])])}, 'source': ['!lamin close\\n', '!lamin delete "*

 * *            "pgtest']}, 2: {'id': '33c2bb76-d61f-4866-87e2-780e61600022', 'source': ['import "*

 * *            "lamindb as ln']}, 4: {'source': {insert: [(2, '!docker stop pgtest && docker rm "*

 * *            'pgtest\\n\')]}}, 5: {\'source\': [\'ln.setup.init(storage="./storage1", '*

 * *            "db=pgurl)']}, 15: {'source' […]*

```diff
@@ -4,54 +4,40 @@
             "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Get info, set storage & delete an instance"
+                "# Set storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import lamindb as ln"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "fe33eb9b",
-            "metadata": {},
-            "source": [
-                "## Get info"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "00a97004",
-            "metadata": {},
+            "id": "6422b64e",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")"
+                "!lamin close\n",
+                "!lamin delete pgtest"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6f127d1",
+            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.info()  # CLI: lamin info"
+                "import lamindb as ln"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "a7cf42fb",
             "metadata": {},
@@ -68,25 +54,36 @@
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "import laminci\n",
                 "\n",
+                "!docker stop pgtest && docker rm pgtest\n",
                 "pgurl = laminci.db.setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d6b0bd5e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
+                "ln.setup.init(storage=\"./storage1\", db=pgurl)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "63392da0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.settings.storage.root"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e6638f44",
             "metadata": {},
@@ -103,14 +100,24 @@
             "source": [
                 "ln.setup.set.storage(\"./storage_2\")  # CLI: lamin set --storage ./storage_2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "47b1f038",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.settings.storage.root"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "8e481aa0",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
@@ -136,14 +143,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.set.storage(\"s3://lndb-setup-ci\")  # lamin set --storage s3://lndb-setup-ci"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "af069899",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.settings.storage.root"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "id": "859a972e",
             "metadata": {},
             "source": [
                 "See an overview:"
             ]
@@ -151,15 +168,21 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "146192a7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.select(ln.Storage).df()"
+                "import lndb\n",
+                "import pandas as pd\n",
+                "\n",
+                "if lndb._USE_DJANGO:\n",
+                "    display(pd.DataFrame(ln.Storage.objects.all().values()))\n",
+                "else:\n",
+                "    print(ln.select(ln.Storage).df())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d2934990",
             "metadata": {
@@ -226,127 +249,23 @@
                 "tags": []
             },
             "source": [
                 "### Currently not possible: setting storage for SQLite instance"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "49309f3a-199f-40bc-b318-a396ebcaafec",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.login(\"testuser1\")\n",
-                "ln.setup.load(\"mydata\")"
-            ]
-        },
-        {
             "attachments": {},
             "cell_type": "markdown",
             "id": "6ccb6573",
             "metadata": {},
             "source": [
-                "If you try to set the storage for an sqlite instance, an error message is returned:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e4f2545f",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "675739c6",
-            "metadata": {},
-            "source": [
-                "## Delete an instance"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "cceb345b",
-            "metadata": {},
-            "source": [
-                "### With local default storage"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "562024da",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(storage=\"mydata-delete\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e7d4860a",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.delete(\"mydata-delete\")  # CLI: lamin delete mydata"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "5d558511",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "from lndb.dev._settings_store import instance_settings_file\n",
-                "\n",
-                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")\n",
-                "assert settings_file.exists() == False"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "83d675b0",
-            "metadata": {},
-            "source": [
-                "### With remote default storage"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "dccb27bf",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(storage=\"s3://lndb-setup-delete-ci\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "fde88024",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.delete(\"lndb-setup-delete-ci\")"
+                "If you try to set the storage for an sqlite instance, an error message is returned:\n",
+                "```\n",
+                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\"\n",
+                "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -358,15 +277,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
```

### Comparing `lndb-0.45a4/docs/guide/05-schema-modules.ipynb` & `lndb-0.46a1/docs/guide/05-schema-modules.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9526851851851852%*

 * *Differences: {"'cells'": "{1: {'source': ['!lamin close\\n', '!lamin delete mydata2']}, 2: {'source': ['import "*

 * *            "lamindb as ln']}, 3: {'source': {insert: [(2, 'The `lamin1` module is an example for "*

 * *            'a configurable in-house schema that tracks lab operations: '*

 * *            "https://github.com/laminlabs/lnschema-lamin1\\n'), (3, '\\n'), (4, 'You can configure "*

 * *            "an arbitrary number of schema modules.')], delete: [2]}}, 4: {'source': ['import "*

 * *            "lndb\\n', '\\n', 'if not lnd […]*

```diff
@@ -7,102 +7,68 @@
             "source": [
                 "# Configure schema modules"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import lamindb as ln"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Core schema module"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The core schema module is part of any LaminDB instance and tracks data lineage."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "You can find the code here: https://github.com/laminlabs/lnschema-core"
+                "!lamin close\n",
+                "!lamin delete mydata2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.schema.draw()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Schema modules `bionty` & `lamin1`"
+                "import lamindb as ln"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `bionty` schema module maps fundamental biological entities: https://github.com/laminlabs/lnschema-bionty\n",
                 "\n",
-                "The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1"
+                "The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1\n",
+                "\n",
+                "You can configure an arbitrary number of schema modules."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(\n",
-                "    storage=\"mydata2\", schema=\"bionty,lamin1\"\n",
-                ")  # CLI: lamin init --storage mydata2 --schema bionty,lamin1"
+                "import lndb\n",
+                "\n",
+                "if not lndb._USE_DJANGO:\n",
+                "    ln.setup.init(\n",
+                "        storage=\"mydata2\", schema=\"bionty,lamin1\"\n",
+                "    )  # CLI: lamin init --storage mydata2 --schema bionty,lamin1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.schema.draw()"
+                "if not lndb._USE_DJANGO:\n",
+                "    ln.setup.schema.draw()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -124,36 +90,38 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "load_bionty_versions(ln.setup.settings.instance, display=True)"
+                "if not lndb._USE_DJANGO:\n",
+                "    load_bionty_versions(ln.setup.settings.instance, display=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "# clean up\n",
-                "ln.setup.delete(\"mydata2\")\n",
-                "# test with postgres\n",
-                "from laminci.db import setup_local_test_postgres\n",
+                "if not lndb._USE_DJANGO:\n",
+                "    # clean up\n",
+                "    ln.setup.delete(\"mydata2\")\n",
+                "    # test with postgres\n",
+                "    from laminci.db import setup_local_test_postgres\n",
                 "\n",
-                "pgurl = setup_local_test_postgres()\n",
-                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)\n",
-                "!docker stop pgtest && docker rm pgtest\n",
-                "ln.setup.delete(\"pgtest\")"
+                "    pgurl = setup_local_test_postgres()\n",
+                "    ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)\n",
+                "    !docker stop pgtest && docker rm pgtest\n",
+                "    ln.setup.delete(\"pgtest\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.45a4/docs/guide/migrate.md` & `lndb-0.46a1/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/__init__.py` & `lndb-0.46a1/lndb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,16 +47,23 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.45a4"  # denote a release candidate for 0.1.0 with 0.1rc1
+import os
 
+__version__ = "0.46a1"  # denote a release candidate for 0.1.0 with 0.1rc1
+_USE_DJANGO = os.getenv("LAMINDB_USE_DJANGO") is not None
+# _USE_DJANGO = True
+if _USE_DJANGO:
+    print("using django backend")
+
+import builtins
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
 from ._delete import delete  # noqa
@@ -67,27 +74,49 @@
 from ._register_instance import register  # noqa
 from ._schema import schema  # noqa
 from ._set import set, set_storage  # noqa
 from ._settings import settings  # noqa
 from ._setup_user import login, signup  # noqa
 
 
-# unlock and clear even if an uncaught exception happens
-def _clear_on_exception(typ, value, traceback):
+# unlock and clear on uncaught exception
+def _clear_on_exception():
     from .dev._exclusion import _locker
 
     if _locker is not None:
         try:
             _locker._clear()
         except:
             pass
-    sys.__excepthook__(typ, value, traceback)
 
 
-sys.excepthook = _clear_on_exception
+_is_ipython = getattr(builtins, "__IPYTHON__", False)
+if _is_ipython:
+    try:
+        from IPython import get_ipython
+
+        ipython = get_ipython()
+    except:
+        _is_ipython = False
+# unlock and clear even if an uncaught exception happens in an ipython session
+if _is_ipython:
+
+    def _clear_on_exception_ipython(self, etype, value, tb, tb_offset=None):
+        _clear_on_exception()
+        return self.showtraceback()
+
+    ipython.set_custom_exc((BaseException,), _clear_on_exception_ipython)
+# unlock and clear even if an uncaught exception happens in a script
+else:
+
+    def _clear_on_exception_script(typ, value, traceback):
+        _clear_on_exception()
+        sys.__excepthook__(typ, value, traceback)
+
+    sys.excepthook = _clear_on_exception_script
 
 # hide the supabase error in a thread on windows
 if _os_name == "nt":
     if sys.version_info.minor > 7:
         import threading
 
         _original_excepthook = threading.excepthook
```

### Comparing `lndb-0.45a4/lndb/__main__.py` & `lndb-0.46a1/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_check_instance_setup.py` & `lndb-0.46a1/lndb/_check_instance_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from lamin_logger import logger
 
+from . import _USE_DJANGO
 from .dev._settings_store import current_instance_settings_file
 
 
 def check_instance_setup(from_lamindb: bool = False):
     if current_instance_settings_file().exists():
         try:
             # attempt loading the settings file
             from .dev._settings_load import load_instance_settings
 
             load_instance_settings()
 
+            if _USE_DJANGO:
+                from .dev._django import IS_SETUP
+
+                if not IS_SETUP:
+                    return False
+
             # if importing from lamindb, also ensure migrations are correct
-            if from_lamindb:
+            if from_lamindb and not _USE_DJANGO:
                 # attempt accessing settings and migrating the instance
                 from . import settings
                 from ._migrate import check_deploy_migration
 
                 check_deploy_migration(
                     usettings=settings.user, isettings=settings.instance
                 )
```

### Comparing `lndb-0.45a4/lndb/_close.py` & `lndb-0.46a1/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_delete.py` & `lndb-0.46a1/lndb/_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 def delete(instance_name: str):
     """Delete an instance."""
     instance_identifier = f"{settings.user.handle}/{instance_name}"
     logger.info(f"Deleting instance {instance_identifier}")
     settings_file = instance_settings_file(instance_name, settings.user.handle)
     if not settings_file.exists():
-        raise RuntimeError(
-            "Instance settings do not exist locally. Did you provide a wrong instance"
-            " name? Could you try loading it?"
+        logger.warning(
+            "Could not delete as instance settings do not exist locally. Did you"
+            " provide a wrong instance name? Could you try loading it?"
         )
+        return None
     isettings = load_instance_settings(settings_file)
 
     delete_settings(settings_file)
     if settings._instance_exists:
         if instance_identifier == settings.instance.identifier:
             current_settings_file = current_instance_settings_file()
             logger.info(
```

### Comparing `lndb-0.45a4/lndb/_init_instance.py` & `lndb-0.46a1/lndb/_init_instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,35 +10,61 @@
     get_storage_region,
     validate_storage_root_arg,
 )
 from pydantic import PostgresDsn
 
 from lndb.dev.upath import UPath
 
+from . import _USE_DJANGO
 from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
 from .dev._db import insert_if_not_exists, upsert
 from .dev._docs import doc_args
 from .dev._setup_knowledge import write_bionty_versions
 from .dev._setup_schema import load_schema, setup_schema
 from .dev._storage import Storage
 
 
 def register(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
-    upsert.user(usettings.email, usettings.id, usettings.handle, usettings.name)
-    insert_if_not_exists.storage(isettings.storage)
+    if _USE_DJANGO:
+        from lnschema_core.models import Storage, User
+
+        user, created = User.objects.update_or_create(
+            id=usettings.get_id_as_int(),
+            defaults=dict(
+                handle=usettings.handle,
+                name=usettings.name,
+                email=usettings.email,
+            ),
+        )
+        storage, created = Storage.objects.update_or_create(
+            root=isettings.storage.root_as_str,
+            defaults=dict(
+                root=isettings.storage.root_as_str,
+                region=isettings.storage.region,
+            ),
+        )
+        if created:
+            logger.success(
+                f"Added storage root {storage.id}:  {isettings.storage.root_as_str}"
+            )
+    else:
+        upsert.user(usettings.email, usettings.id, usettings.handle, usettings.name)
+        insert_if_not_exists.storage(isettings.storage)
 
 
 def reload_lamindb(isettings: InstanceSettings):
     # only touch lamindb if we're operating from lamindb
     if "lamindb" in sys.modules:
         import lamindb
+        import lnschema_core
 
+        importlib.reload(lnschema_core)
         importlib.reload(lamindb)
     else:
         # only log if we're outside lamindb
         # lamindb itself logs upon import!
         logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
 
 
@@ -78,14 +104,15 @@
 def init(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
     schema: Optional[str] = None,
     _migrate: bool = False,  # not user-facing
+    _test: bool = False,
 ) -> Optional[str]:
     """Creating and loading a LaminDB instance.
 
     Args:
         storage: {}
         name: {}
         db: {}
@@ -96,15 +123,17 @@
 
     schema = validate_schema_arg(schema)
     validate_storage_root_arg(str(storage))
     validate_db_arg(db)
 
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # test whether instance exists by trying to load it
-    message = load(f"{owner}/{name_str}", _log_error_message=False, migrate=_migrate)
+    message = load(
+        f"{owner}/{name_str}", _log_error_message=False, migrate=_migrate, _test=_test
+    )
     if message != "instance-not-reachable":
         return message
 
     isettings = InstanceSettings(
         owner=owner,
         name=name_str,
         storage_root=storage,
@@ -132,20 +161,26 @@
             db=db,
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Creating instance on hub failed:\n{result}")
-        logger.success(f"Registered instance on hub: https://lamin.ai/{owner}/{name}")
+        logger.success(
+            f"Registered instance on hub: https://lamin.ai/{owner}/{name_str}"
+        )
     else:
         logger.info(
             "Not registering instance on hub, if you want, call `lamin register`"
         )
 
+    if _test:
+        isettings._persist()
+        return None
+
     # this does not yet setup a setup for a new database
     persist_settings_load_schema(isettings)
 
     message = None
     if not isettings._is_db_setup(mute=True)[0]:
         setup_schema(isettings, settings.user)
         register(isettings, settings.user)
```

### Comparing `lndb-0.45a4/lndb/_load_instance.py` & `lndb-0.46a1/lndb/_load_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from lamin_logger import logger
 from lnhub_rest.core.instance._load_instance import (
     load_instance as load_instance_from_hub,
 )
 
 from lndb.dev.upath import UPath
 
+from . import _USE_DJANGO
 from ._settings import InstanceSettings, settings
+from .dev._django import setup_django
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 from .dev._storage import StorageSettings
 
 
 def load(
     identifier: str,
     *,
     migrate: Optional[bool] = None,
     storage: Optional[Union[str, Path, UPath]] = None,
     _log_error_message: bool = True,
     _access_token: Optional[str] = None,
+    _test: bool = False,
 ) -> Optional[str]:
     """Load existing instance.
 
     Args:
         identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
         storage: `Optional[PathLike] = None` - Load the instance with an
@@ -67,32 +70,44 @@
                     " cache. Check whether instance exists and you have access:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
                 )
             return "instance-not-reachable"
 
     if storage is not None:
         update_isettings_with_storage(isettings, storage)
-
-    if not isettings.storage.root.exists():
-        raise RuntimeError(
-            f"Storage root does not exist: {isettings.storage.root}\n"
-            "Please amend by passing --storage <my-storage-root>"
-        )
+    if _test:
+        isettings._persist()  # this is to test the settings
+        return None
 
     check, msg = isettings._is_db_setup()
     if not check:
         if _log_error_message:
             raise RuntimeError(msg)
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
 
+    if _USE_DJANGO:
+        setup_django(isettings)
+    else:
+        from ._init_instance import persist_settings_load_schema
+
+        persist_settings_load_schema(isettings)
+    if storage is not None and isettings.dialect == "sqlite":
+        update_storage(isettings)
+
+    if not isettings.storage.root.exists():
+        raise RuntimeError(
+            f"Storage root does not exist: {isettings.storage.root}\n"
+            "Please amend by passing --storage <my-storage-root>"
+        )
+
     message = load_from_isettings(isettings, migrate)
     if not message == "migrate-failed":
         os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
     return message
 
 
 def get_owner_name_from_identifier(identifier: str):
@@ -111,68 +126,77 @@
         name = identifier
     return owner, name
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
     migrate: Optional[bool] = None,
-):
+) -> Optional[str]:
     from ._init_instance import persist_settings_load_schema, register, reload_lamindb
     from ._migrate import check_deploy_migration
     from .dev._setup_knowledge import load_bionty_versions
 
     persist_settings_load_schema(isettings)
-    message = check_deploy_migration(
-        usettings=settings.user, isettings=isettings, attempt_deploy=migrate
-    )
-    if message == "migrate-failed":
-        return message
+    message = None
+    if not _USE_DJANGO:
+        message = check_deploy_migration(
+            usettings=settings.user, isettings=isettings, attempt_deploy=migrate
+        )
+        if message == "migrate-failed":
+            return message
     register(isettings, settings.user)
     load_bionty_versions(isettings)
     reload_lamindb(isettings)
     return message
 
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
-    isettings._persist()  # this is temporary for import of lnschema_core
     ssettings = StorageSettings(storage, instance_settings=isettings)
     if ssettings.is_cloud:
         try:  # triggering ssettings.id makes a lookup in the storage table
             logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
         except RuntimeError:
             raise RuntimeError(
                 "Storage not registered!\n"
                 "Load instance without the `storage` arg and register storage root: "
                 f"`lamin set storage --storage {storage}`"
             )
     else:
         # local storage
         # assumption is you want to merely update the storage location
+        isettings._storage = ssettings  # need this here already
+    # update isettings in place
+    isettings._storage = ssettings
+
+
+# this is different from register!
+def update_storage(isettings: InstanceSettings):
+    if _USE_DJANGO:
+        from lnschema_core.models import Storage
+
+        storages = Storage.objects.all()
+        if len(storages) != 1:
+            raise RuntimeError("Can't identify which storage location to update")
+        storage = storages[0]
+        storage.root = isettings.storage.root_as_str
+        storage.save()
+    else:
         from lnschema_core import Storage
 
-        isettings._storage = ssettings  # need this here already
-        if isettings.dialect == "sqlite":
-            isettings._engine = sqm.create_engine(isettings.db)
+        isettings._engine = sqm.create_engine(isettings.db)
+        with sqm.Session(isettings.engine) as session:
+            storage = session.exec(
+                sqm.select(Storage).where(Storage.root == isettings.storage.root_as_str)
+            ).one_or_none()
+        if storage is None:
             with sqm.Session(isettings.engine) as session:
-                storage = session.exec(
-                    sqm.select(Storage).where(Storage.root == ssettings.root_as_str)
-                ).one_or_none()
-            if storage is None:
-                with sqm.Session(isettings.engine) as session:
-                    storage_record = session.exec(sqm.select(Storage)).one()
-                    storage_record.root = ssettings.root_as_str
-                    session.add(storage_record)
-                    session.commit()
-                    session.refresh(storage_record)
-                logger.success(
-                    f"Updated storage root {storage_record.id} to"
-                    f" {ssettings.root_as_str}"
-                )
-        else:
-            raise RuntimeError(
-                "Cannot currently not update local storage of sqlite upon load. Use"
-                " `lamin set --storage`"
+                storage_record = session.exec(sqm.select(Storage)).one()
+                storage_record.root = isettings.storage.root_as_str
+                session.add(storage_record)
+                session.commit()
+                session.refresh(storage_record)
+            logger.success(
+                f"Updated storage root {storage_record.id} to"
+                f" {isettings.storage.root_as_str}"
             )
-    # update isettings in place
-    isettings._storage = ssettings
```

### Comparing `lndb-0.45a4/lndb/_migrate/alembic.ini` & `lndb-0.46a1/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_migrate/core.py` & `lndb-0.46a1/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_migrate/deploy.py` & `lndb-0.46a1/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_migrate/env.py` & `lndb-0.46a1/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_migrate/utils.py` & `lndb-0.46a1/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_notebook.py` & `lndb-0.46a1/lndb/_notebook.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_register_instance.py` & `lndb-0.46a1/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_schema.py` & `lndb-0.46a1/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_set.py` & `lndb-0.46a1/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_settings.py` & `lndb-0.46a1/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/_setup_user.py` & `lndb-0.46a1/lndb/_setup_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 from lamin_logger import logger
 from lnhub_rest.core.account._signup_signin import sign_in_hub, sign_up_hub
 
 from ._settings import settings
-from .dev._db import upsert
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
 
 
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
@@ -96,21 +95,8 @@
     user_settings.id = user_id
     user_settings.handle = user_handle
     user_settings.name = user_name
     user_settings.access_token = access_token
     save_user_settings(user_settings)
 
     settings._user_settings = None
-
-    # register login of user in instance db
-    if settings._instance_exists:
-        if not settings.instance._is_db_reachable():
-            logger.info("Consider closing the instance: `lamin close`")
-            return None
-        upsert.user(
-            settings.user.email,
-            settings.user.id,
-            settings.user.handle,
-            settings.user.name,
-        )
-
     return None
```

### Comparing `lndb-0.45a4/lndb/dev/_clone.py` & `lndb-0.46a1/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_db.py` & `lndb-0.46a1/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_deprecated.py` & `lndb-0.46a1/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_exclusion.py` & `lndb-0.46a1/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_settings_instance.py` & `lndb-0.46a1/lndb/dev/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,21 +222,28 @@
                     False,
                     f"SQLite file {self._sqlite_file} does not exist! It should be in"
                     f" the storage root: {self.storage.root}",
                 )
             else:
                 return False, f"Connection {self.db} not reachable"
 
-        with self.engine.connect() as conn:
+        engine = sqm.create_engine(self.db)
+        with engine.connect() as conn:
             try:  # cannot import lnschema_core here, need to use plain SQL
-                result = conn.execute(sa.text("select * from version_yvzi")).first()
+                result = conn.execute(
+                    sa.text("select * from lnschema_core_user")
+                ).first()
             except Exception as e:
                 return False, f"Your DB is not initialized: {e}"
             if result is None:
-                return False, "Your DB is not initialized: version_yvzi has no row"
+                return (
+                    False,
+                    "Your DB is not initialized: lnschema_core_user has no row",
+                )
+        self._engine = engine
         return True, ""
 
     def _is_db_reachable(self, mute: bool = False) -> bool:
         if self.dialect == "sqlite":
             if not self._sqlite_file.exists():
                 if not mute:
                     logger.warning(f"SQLite file {self._sqlite_file} does not exist")
```

### Comparing `lndb-0.45a4/lndb/dev/_settings_load.py` & `lndb-0.46a1/lndb/dev/_settings_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,11 @@
 
 
 def setup_user_from_store(store: UserSettingsStore) -> UserSettings:
     settings = UserSettings()
     settings.email = store.email
     settings.password = store.password if store.password != "null" else None
     settings.access_token = store.access_token
-    settings.id = store.id if store.id != "null" else None
+    settings.id = store.id
     settings.handle = store.handle if store.handle != "null" else None
     settings.name = store.name if store.name != "null" else None
     return settings
```

### Comparing `lndb-0.45a4/lndb/dev/_settings_save.py` & `lndb-0.46a1/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_settings_store.py` & `lndb-0.46a1/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_settings_user.py` & `lndb-0.46a1/lndb/dev/_settings_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from base64 import b64decode
 from dataclasses import dataclass
 from typing import Union
 
 
 class user_description:
     email = """User email."""
     password = """User password."""
@@ -16,22 +17,25 @@
 
     email: str = None  # type: ignore
     """User email."""
     password: Union[str, None] = None
     """User password."""
     access_token: Union[str, None] = None
     """User access token."""
-    id: Union[str, None] = None
+    id: str = "null"
     """User ID."""
     handle: Union[str, None] = None
     "Unique handle."
     name: Union[str, None] = None
     "Full name."
 
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current user: {self.handle}"
         attrs = ["handle", "email", "id"]
         for attr in attrs:
             value = getattr(self, attr)
             representation += f"\n- {attr}: {value}"
         return representation
+
+    def get_id_as_int(self) -> int:
+        return int.from_bytes(b64decode(self.id), "big")
```

### Comparing `lndb-0.45a4/lndb/dev/_setup_knowledge.py` & `lndb-0.46a1/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/dev/_setup_schema.py` & `lndb-0.46a1/lndb/dev/_setup_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import sqlmodel as sqm
 from importlib_metadata import requires as importlib_requires
 from importlib_metadata import version as get_pip_version
 from lamin_logger import logger
 from lnhub_rest._assets._schemas import get_schema_module_name
 from packaging.requirements import Requirement
 
+from .. import _USE_DJANGO
 from ._db import insert
+from ._django import setup_django
 from ._settings_instance import InstanceSettings
 from ._settings_user import UserSettings
 
 
 def check_schema_version_and_import(schema_name) -> ModuleType:
     def check_version(module_version):
         schema_module_name = get_schema_module_name(schema_name)
@@ -53,53 +55,71 @@
         raise import_error
 
     check_version(module_version)
     return module
 
 
 def load_schema(isettings: InstanceSettings):
+    if _USE_DJANGO:
+        setup_django(isettings)
+
     schema_names = ["core"] + list(isettings.schema)
     msg = "Loading schema modules: "
     for schema_name in schema_names:
         module = check_schema_version_and_import(schema_name)
         msg += f"{schema_name}=={module.__version__} "
     return msg, schema_names
 
 
 def setup_schema(isettings: InstanceSettings, usettings: UserSettings):
     msg, schema_names = load_schema(isettings)
     logger.info(f"{msg}")
 
-    sqm.SQLModel.metadata.create_all(isettings.engine)
+    if not _USE_DJANGO:
+        sqm.SQLModel.metadata.create_all(isettings.engine)
 
-    # we could try to also retrieve the user name here at some point
-    insert.user(
-        email=usettings.email,
-        user_id=usettings.id,
-        handle=usettings.handle,
-        name=usettings.name,
-    )
+        # we could try to also retrieve the user name here at some point
+        insert.user(
+            email=usettings.email,
+            user_id=usettings.id,
+            handle=usettings.handle,
+            name=usettings.name,
+        )
 
-    for schema_name in schema_names:
-        schema_module = importlib.import_module(get_schema_module_name(schema_name))
-        insert.version(
-            schema_module=schema_module,
-            user_id=usettings.id,  # type: ignore
-            cloud_sqlite=False,
+    else:
+        from lnschema_core.models import User
+
+        user = User(
+            id=usettings.get_id_as_int(),
+            email=usettings.email,
+            handle=usettings.handle,
+            name=usettings.name,
         )
-        # this is the only time we need manipulate the migration table
-        # in all other cases alembic is going to to do this for us
-        schema_id, migration = schema_module._schema_id, schema_module._migration
-        if migration is not None:
-            table_loc = (
-                schema_module.dev if hasattr(schema_module, "dev") else schema_module
+        user.save()
+
+    if not _USE_DJANGO:
+        for schema_name in schema_names:
+            schema_module = importlib.import_module(get_schema_module_name(schema_name))
+            insert.version(
+                schema_module=schema_module,
+                user_id=usettings.id,  # type: ignore
+                cloud_sqlite=False,
             )
-            migration_table = getattr(table_loc, f"migration_{schema_id}")
-            # we purposefully do not use isettings.session(), here, as we do *not*
-            # want to update the local sqlite file from the cloud while looping over
-            # schema modules
-            # in fact, a synchronization issue led to loss of version information,
-            # because the old cloud sqlite file overwrote the newer local file
-            with sqm.Session(isettings.engine) as session:
-                session.add(migration_table(version_num=migration))
-                session.commit()
-    isettings._update_cloud_sqlite_file()
+            # this is the only time we need manipulate the migration table
+            # in all other cases alembic is going to to do this for us
+            schema_id, migration = schema_module._schema_id, schema_module._migration
+            if migration is not None:
+                table_loc = (
+                    schema_module.dev
+                    if hasattr(schema_module, "dev")
+                    else schema_module
+                )
+                migration_table = getattr(table_loc, f"migration_{schema_id}")
+                # we purposefully do not use isettings.session(), here, as we do *not*
+                # want to update the local sqlite file from the cloud while looping over
+                # schema modules
+                # in fact, a synchronization issue led to loss of version information,
+                # because the old cloud sqlite file overwrote the newer local file
+                with sqm.Session(isettings.engine) as session:
+                    session.add(migration_table(version_num=migration))
+                    session.commit()
+        isettings._update_cloud_sqlite_file()
```

### Comparing `lndb-0.45a4/lndb/dev/_storage.py` & `lndb-0.46a1/lndb/dev/_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from pathlib import Path
 from typing import Literal, Optional, Union
 
 import sqlmodel as sqm
 from appdirs import AppDirs
 
+from .. import _USE_DJANGO
 from .upath import UPath
 
 DIRS = AppDirs("lamindb", "laminlabs")
 
 
 class StorageSettings:
     """Manage cloud or local storage settings."""
@@ -46,26 +47,31 @@
             storage_root = Path(storage).resolve()
         return storage_root
 
     @property
     def id(self) -> str:
         """Storage id."""
         if self._id is None:
-            from lnschema_core import Storage
+            if not _USE_DJANGO:
+                from lnschema_core import Storage
 
-            with sqm.Session(self._instance_settings.engine) as session:
-                # needs to have been registered before!
-                storage = session.exec(
-                    sqm.select(Storage).where(Storage.root == self.root_as_str)
-                ).one_or_none()
-            if storage is None:
-                raise RuntimeError(
-                    f"{self.root_as_str} wasn't registered in the db! "
-                    "Check ln.select(ln.Storage).all()"
-                )
+                with sqm.Session(self._instance_settings.engine) as session:
+                    # needs to have been registered before!
+                    storage = session.exec(
+                        sqm.select(Storage).where(Storage.root == self.root_as_str)
+                    ).one_or_none()
+                if storage is None:
+                    raise RuntimeError(
+                        f"{self.root_as_str} wasn't registered in the db! "
+                        "Check ln.select(ln.Storage).all()"
+                    )
+            else:
+                from lnschema_core.models import Storage
+
+                storage = Storage.objects.get(root=self.root_as_str)
             self._id = storage.id
         return self._id
 
     @property
     def root(self) -> Union[Path, UPath]:
         """Root storage location."""
         return self._root
```

### Comparing `lndb-0.45a4/lndb/dev/upath.py` & `lndb-0.46a1/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/test/_migrations_e2e.py` & `lndb-0.46a1/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/lndb/test/_migrations_unit.py` & `lndb-0.46a1/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a4/pyproject.toml` & `lndb-0.46a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
     "lnhub_rest==0.9.8",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
-    "lnschema_core>=0.34a2",
+    "lnschema_core>=0.35a1",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
-    "sqlmodel>=0.0.8",
     "psycopg2-binary",
     "appdirs",
     "python-dotenv",
     "erdiagram",
     "alembic",
     "natsort",
     "pandas",
@@ -30,21 +29,20 @@
     "universal_pathlib"
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lndb"
 
 [project.optional-dependencies]
-dev = [
-    "pre-commit",
-    "nox",
+django = [
+    "django",
 ]
 test = [
-    "lnschema_lamin1",
-    "lamindb[bionty,lamin1]>=0.41a3",
+    "pre-commit",
+    "nox",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
     "nbproject",
 ]
 
 [project.scripts]
```

### Comparing `lndb-0.45a4/PKG-INFO` & `lndb-0.46a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.45a4
+Version: 0.46a1
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.8
 Requires-Dist: laminci>=0.3.0
-Requires-Dist: lnschema_core>=0.34a2
+Requires-Dist: lnschema_core>=0.35a1
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
-Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
 Requires-Dist: appdirs
 Requires-Dist: python-dotenv
 Requires-Dist: erdiagram
 Requires-Dist: alembic
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
-Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: nox ; extra == "dev"
-Requires-Dist: lnschema_lamin1 ; extra == "test"
-Requires-Dist: lamindb[bionty,lamin1]>=0.41a3 ; extra == "test"
+Requires-Dist: django ; extra == "django"
+Requires-Dist: pre-commit ; extra == "test"
+Requires-Dist: nox ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb
-Provides-Extra: dev
+Provides-Extra: django
 Provides-Extra: test
 
 # lndb: Setup LaminDB
 
 - Stable user docs: [lamin.ai/docs/setup/](https://lamin.ai/docs/setup/)
 - Latest developer docs: [netlify](https://lndb-htry.netlify.app/docs/lndb/)
```

