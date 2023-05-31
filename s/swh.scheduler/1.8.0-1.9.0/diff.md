# Comparing `tmp/swh.scheduler-1.8.0.tar.gz` & `tmp/swh.scheduler-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.scheduler-1.8.0.tar", last modified: Fri Mar 31 10:39:43 2023, max compression
+gzip compressed data, was "dist/swh.scheduler-1.9.0.tar", last modified: Wed May 31 08:19:27 2023, max compression
```

## Comparing `swh.scheduler-1.8.0.tar` & `swh.scheduler-1.9.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/LICENSE.Celery
--rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/data/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/data/elastic-template.json
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/data/update-index-settings.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/docs/simulator.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/requirements-journal.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/requirements-simulator.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/sql/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/sql/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/
--rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/backend.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/pika_listener.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13193 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/celery_backend/runner.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     2912 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7154 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7250 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12950 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/task.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7052 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/
--rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/origin_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/origins.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/simulator/task_scheduler.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    14494 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/40-func.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/50-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/02.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/03.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/04.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/05.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/06.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/07.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/08.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/09.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/10.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/11.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/12.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/13.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/14.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/15.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/16.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/17.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/18.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/19.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/20.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/23.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/24.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/25.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/26.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/27.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/28.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/29.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/30-bis.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/30.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/31.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/32.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/33.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/task.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh/scheduler/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/data/logging-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_celery_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24126 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5009 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3937 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5687 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8573 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)    61026 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5366 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3536 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/swh/scheduler/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4195 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-31 10:39:43.000000 swh.scheduler-1.8.0/swh.scheduler.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-03-31 10:39:41.000000 swh.scheduler-1.8.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/LICENSE.Celery
+-rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/elastic-template.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/update-index-settings.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/simulator.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-journal.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-simulator.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/sql/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/backend.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/pika_listener.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13193 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/runner.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2912 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5302 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7154 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7250 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12950 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7052 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/origin_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/origins.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/task_scheduler.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    14494 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/40-func.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/50-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/02.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/03.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/04.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/05.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/06.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/07.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/08.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/09.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/10.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/11.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/12.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/13.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/14.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/15.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/16.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/17.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/18.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/19.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/20.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/23.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/24.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/25.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/26.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/27.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/28.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/29.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30-bis.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/31.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/32.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/33.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/task.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/logging-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_celery_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24126 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5586 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3937 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5687 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8573 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    61026 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5366 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3536 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4195 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/tox.ini
```

### Comparing `swh.scheduler-1.8.0/.pre-commit-config.yaml` & `swh.scheduler-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/CODE_OF_CONDUCT.md` & `swh.scheduler-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/LICENSE` & `swh.scheduler-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/LICENSE.Celery` & `swh.scheduler-1.9.0/LICENSE.Celery`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/PKG-INFO` & `swh.scheduler-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.8.0
+Version: 1.9.0
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.8.0/conftest.py` & `swh.scheduler-1.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/data/README.md` & `swh.scheduler-1.9.0/data/README.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/data/elastic-template.json` & `swh.scheduler-1.9.0/data/elastic-template.json`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/docs/cli.rst` & `swh.scheduler-1.9.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/docs/index.rst` & `swh.scheduler-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/docs/simulator.rst` & `swh.scheduler-1.9.0/docs/simulator.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/mypy.ini` & `swh.scheduler-1.9.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/setup.py` & `swh.scheduler-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/sql/Makefile` & `swh.scheduler-1.9.0/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/__init__.py` & `swh.scheduler-1.9.0/swh/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/api/client.py` & `swh.scheduler-1.9.0/swh/scheduler/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/api/serializers.py` & `swh.scheduler-1.9.0/swh/scheduler/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/api/server.py` & `swh.scheduler-1.9.0/swh/scheduler/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/backend.py` & `swh.scheduler-1.9.0/swh/scheduler/backend.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/celery_backend/config.py` & `swh.scheduler-1.9.0/swh/scheduler/celery_backend/config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/celery_backend/pika_listener.py` & `swh.scheduler-1.9.0/swh/scheduler/celery_backend/pika_listener.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/celery_backend/recurrent_visits.py` & `swh.scheduler-1.9.0/swh/scheduler/celery_backend/recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/celery_backend/runner.py` & `swh.scheduler-1.9.0/swh/scheduler/celery_backend/runner.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/__init__.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/add_forge_now.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/add_forge_now.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     from datetime import timedelta
 
     from swh.scheduler.utils import utcnow
 
     for listing_type, task_type in task_types.items():
         now = utcnow()
-        next_run = now if listing_type == "full" else now + timedelta(days=1)
+        next_run = now + timedelta(days=1) if listing_type == "incremental" else now
         task_add(
             scheduler,
             task_type_name=task_type["type"],
             args=args,
             kw=kw,
             policy=policy,
             next_run=next_run,
@@ -121,23 +121,29 @@
     help="Limit origins to those listed from lister with provided name",
 )
 @click.option(
     "--lister-instance-name",
     default=None,
     help="Limit origins to those listed from lister with instance name",
 )
+@click.option(
+    "--queue-name-prefix",
+    default="add_forge_now",
+    help='Prefix queue to use when scheduling tasks. Default to "add_forge_now".',
+)
 @click.pass_context
 def schedule_first_visits_cli(
     ctx,
     visit_type_names: List[str],
     lister_name: Optional[str] = None,
     lister_instance_name: Optional[str] = None,
+    queue_name_prefix: str = "add_forge_now",
 ):
     """Send next origin visits of VISIT_TYPE_NAME(S) loader to celery, filling the
-    associated add_forge_now queue(s).
+    associated "prefixed" add_forge_now queue(s).
 
     """
     from .utils import get_task_type, send_to_celery
 
     scheduler = ctx.obj["scheduler"]
     preset = ctx.obj["preset"]
 
@@ -145,15 +151,15 @@
     unknown_task_types = []
     for visit_type_name in visit_type_names:
         task_type = get_task_type(scheduler, visit_type_name)
         if not task_type:
             unknown_task_types.append(visit_type_name)
             continue
         queue_name = task_type["backend_name"]
-        visit_type_to_queue[visit_type_name] = f"add_forge_now:{queue_name}"
+        visit_type_to_queue[visit_type_name] = f"{queue_name_prefix}:{queue_name}"
 
     if unknown_task_types:
         raise ValueError(f"Unknown task types {','.join(unknown_task_types)}.")
 
     send_to_celery(
         scheduler,
         visit_type_to_queue=visit_type_to_queue,
```

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/admin.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/celery_monitor.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/journal.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/origin.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/origin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/simulator.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/task.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/task.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/task_type.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/task_type.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/test_cli_utils.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/cli/utils.py` & `swh.scheduler-1.9.0/swh/scheduler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/interface.py` & `swh.scheduler-1.9.0/swh/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/journal_client.py` & `swh.scheduler-1.9.0/swh/scheduler/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/model.py` & `swh.scheduler-1.9.0/swh/scheduler/model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/pytest_plugin.py` & `swh.scheduler-1.9.0/swh/scheduler/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/simulator/__init__.py` & `swh.scheduler-1.9.0/swh/scheduler/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/simulator/common.py` & `swh.scheduler-1.9.0/swh/scheduler/simulator/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/simulator/origin_scheduler.py` & `swh.scheduler-1.9.0/swh/scheduler/simulator/origin_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/simulator/origins.py` & `swh.scheduler-1.9.0/swh/scheduler/simulator/origins.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/simulator/task_scheduler.py` & `swh.scheduler-1.9.0/swh/scheduler/simulator/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/30-schema.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/40-func.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/40-func.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/50-data.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/50-data.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/60-indexes.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/02.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/02.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/03.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/03.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/04.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/04.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/05.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/05.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/06.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/06.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/07.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/07.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/08.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/08.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/09.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/09.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/10.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/10.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/11.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/11.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/12.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/12.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/13.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/13.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/14.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/14.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/15.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/15.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/16.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/16.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/19.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/19.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/23.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/23.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/25.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/25.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/26.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/26.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/27.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/27.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/28.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/28.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/29.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/29.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/30.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/31.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/31.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/32.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/32.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/sql/upgrades/33.sql` & `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/33.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/task.py` & `swh.scheduler-1.9.0/swh/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/common.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/conftest.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/data/logging-config.yaml` & `swh.scheduler-1.9.0/swh/scheduler/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/tasks.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_api_client.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_celery_tasks.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_celery_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_add_forge_now.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_add_forge_now.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 @pytest.mark.parametrize(
     "cmd_args, subcmd_args",
     [
         ([], []),
         ([], ["--lister-name", "github", "--lister-instance-name", "github"]),
         (["--preset", "staging"], []),
+        ([], ["--queue-name-prefix", "add_forge_now_slow"]),
     ],
 )
 def test_schedule_first_visits_cli(
     mocker,
     swh_scheduler,
     swh_scheduler_celery_app,
     listed_origins_by_type,
@@ -88,14 +89,27 @@
     expected_tasks = {
         (TASK_TYPES[origin.visit_type]["backend_name"], origin.url)
         for origin in listed_origins_by_type[visit_type]
     }
 
     assert scheduled_tasks == expected_tasks
 
+    # Ensure the scheduling happens on the right queue
+    queue_name = send_task.call_args[1]["queue"]
+    queue_name_prefix, queue_name_suffix = queue_name.split(":")
+
+    try:
+        arg_index = subcmd_args.index("--queue-name-prefix")
+        expected_queue_name_prefix = subcmd_args[arg_index + 1]
+    except ValueError:
+        expected_queue_name_prefix = "add_forge_now"
+
+    assert queue_name_prefix == expected_queue_name_prefix
+    assert queue_name_suffix == "swh.loader.git.tasks.UpdateGitRepository"
+
 
 def _create_task_type(
     swh_scheduler: SchedulerInterface, lister_name: str, listing_type: str = "full"
 ) -> Dict:
     task_type = {
         "type": lister_task_type(lister_name, listing_type),  # only relevant bit
         "description": f"{listing_type} listing",
```

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_celery_monitor.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_journal.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_origin.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_origin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_task_type.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_task_type.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_cli_utils.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_common.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_config.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_init.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_journal_client.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_model.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_recurrent_visits.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_scheduler.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_server.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_simulator.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/tests/test_utils.py` & `swh.scheduler-1.9.0/swh/scheduler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh/scheduler/utils.py` & `swh.scheduler-1.9.0/swh/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/swh.scheduler.egg-info/PKG-INFO` & `swh.scheduler-1.9.0/swh.scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.8.0
+Version: 1.9.0
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.8.0/swh.scheduler.egg-info/SOURCES.txt` & `swh.scheduler-1.9.0/swh.scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.8.0/tox.ini` & `swh.scheduler-1.9.0/tox.ini`

 * *Files identical despite different names*

