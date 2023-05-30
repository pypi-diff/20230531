# Comparing `tmp/fastapi_cookiecutter-0.0.1-py2-none-any.whl.zip` & `tmp/fastapi_cookiecutter-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,113 @@
-Zip file size: 1222 bytes, number of entries: 4
--rw-r--r--  2.0 unx      330 b- defN 20-Nov-25 18:07 fastapi_cookiecutter-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Nov-25 18:07 fastapi_cookiecutter-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 20-Nov-25 18:07 fastapi_cookiecutter-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      348 b- defN 20-Nov-25 18:07 fastapi_cookiecutter-0.0.1.dist-info/RECORD
-4 files, 771 bytes uncompressed, 536 bytes compressed:  30.5%
+Zip file size: 77930 bytes, number of entries: 111
+-rw-r--r--  2.0 unx      896 b- defN 80-Jan-01 00:00 cookiecutter.json
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fastapi_cookiecutter/__init__.py
+-rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 fastapi_cookiecutter/main.py
+-rw-r--r--  2.0 unx     1718 b- defN 80-Jan-01 00:00 hooks/post_gen_project.py
+-rw-r--r--  2.0 unx      805 b- defN 80-Jan-01 00:00 hooks/pre_gen_project.py
+-rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.coveragerc
+-rw-r--r--  2.0 unx     2810 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.github/workflows/build.yml
+-rw-r--r--  2.0 unx     1475 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.github/workflows/sphinx.yml
+-rw-r--r--  2.0 unx     2584 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.github/workflows/test.yml
+-rw-r--r--  2.0 unx      558 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--  2.0 unx     3136 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/.gitlab-ci.yml
+-rw-r--r--  2.0 unx     5814 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--  2.0 unx     1316 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/LICENSES/2-Clause BSD
+-rw-r--r--  2.0 unx     1507 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/LICENSES/3-Clause BSD
+-rw-r--r--  2.0 unx      600 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/LICENSES/APACHE
+-rw-r--r--  2.0 unx      700 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/LICENSES/GPL
+-rw-r--r--  2.0 unx     1096 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/LICENSES/MIT
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--  2.0 unx     1442 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/Makefile
+-rw-r--r--  2.0 unx     4229 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/README.rst
+-rw-r--r--  2.0 unx     4446 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/bitbucket-pipelines.yml
+-rw-r--r--  2.0 unx      412 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/Dockerfile
+-rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/Dockerfile.local
+-rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/compose_hooks/post_build.sh
+-rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/compose_hooks/pre_build.sh
+-rw-r--r--  2.0 unx     1844 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/docker-compose.yml
+-rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker/init.sql
+-rwxr-xr-x  2.0 unx      350 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docker-compose.sh
+-rw-r--r--  2.0 unx      584 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--  2.0 unx      755 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/make.bat
+-rwxr-xr-x  2.0 unx       30 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/01_about.rst
+-rwxr-xr-x  2.0 unx     6118 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/02_usage.rst
+-rwxr-xr-x  2.0 unx     3114 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/03_source.rst
+-rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/04_authors.rst
+-rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/05_contributing.rst
+-rwxr-xr-x  2.0 unx     5942 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/conf.py
+-rwxr-xr-x  2.0 unx      471 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/docs/source/index.rst
+-rw-r--r--  2.0 unx      280 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/requirements/base.txt
+-rw-r--r--  2.0 unx      119 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/requirements/dev.txt
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/requirements/doc.txt
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/scripts/.keep
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/scripts/prestart.sh
+-rw-r--r--  2.0 unx      644 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--  2.0 unx     2198 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/setup.py
+-rw-r--r--  2.0 unx     2183 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/resources/.keep
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_api/__init__.py
+-rw-r--r--  2.0 unx     5299 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_api/test_auth.py
+-rw-r--r--  2.0 unx      247 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_api/test_base.py
+-rw-r--r--  2.0 unx     1098 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_application.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_configs/__init__.py
+-rw-r--r--  2.0 unx     4418 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_configs/test_base.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_db/__init__.py
+-rw-r--r--  2.0 unx      572 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_db/test_base.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_db/test_models/__init__.py
+-rw-r--r--  2.0 unx     2209 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_db/test_models/test_auth.py
+-rw-r--r--  2.0 unx      811 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_db/test_session.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_events/__init__.py
+-rw-r--r--  2.0 unx      610 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_events/test_base.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_middlewares/__init__.py
+-rw-r--r--  2.0 unx     1337 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_middlewares/test_logging.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_schemas/__init__.py
+-rw-r--r--  2.0 unx     2867 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_schemas/test_auth.py
+-rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_schemas/test_base.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_logging/__init__.py
+-rw-r--r--  2.0 unx     5190 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_colorformatter.py
+-rw-r--r--  2.0 unx     2195 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_helper.py
+-rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_standardformatter.py
+-rw-r--r--  2.0 unx     6305 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_security.py
+-rw-r--r--  2.0 unx     1194 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/tests/test_utils/test_storage.py
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/__init__.py
+-rw-r--r--  2.0 unx      537 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/__init__.py
+-rw-r--r--  2.0 unx     3600 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/auth.py
+-rw-r--r--  2.0 unx      504 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/base.py
+-rw-r--r--  2.0 unx     3360 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/application.py
+-rw-r--r--  2.0 unx     1200 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/__init__.py
+-rw-r--r--  2.0 unx     5891 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/base.py
+-rw-r--r--  2.0 unx      119 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/dev.py
+-rw-r--r--  2.0 unx     1060 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/prod.py
+-rw-r--r--  2.0 unx      969 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/test.py
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/constants.py
+-rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/__init__.py
+-rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/base.py
+-rw-r--r--  2.0 unx       80 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/models/__init__.py
+-rw-r--r--  2.0 unx     3552 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/models/auth.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/queries/__init__.py
+-rw-r--r--  2.0 unx      981 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/session.py
+-rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/events/__init__.py
+-rw-r--r--  2.0 unx      759 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/events/base.py
+-rw-r--r--  2.0 unx      205 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/globals.py
+-rw-r--r--  2.0 unx       30 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/middlewares/__init__.py
+-rw-r--r--  2.0 unx     1079 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/middlewares/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/__init__.py
+-rw-r--r--  2.0 unx     2528 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/auth.py
+-rw-r--r--  2.0 unx      232 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/base.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/services/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/__init__.py
+-rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/errors.py
+-rw-r--r--  2.0 unx     5546 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/logging.py
+-rw-r--r--  2.0 unx     3383 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/security.py
+-rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/storage.py
+-rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/version.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/.keep
+-rw-r--r--  2.0 unx      318 b- defN 80-Jan-01 00:00 {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11236 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12836 b- defN 16-Jan-01 00:00 fastapi_cookiecutter-0.1.0.dist-info/RECORD
+111 files, 161603 bytes uncompressed, 56098 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,13 +1,334 @@
-Filename: fastapi_cookiecutter-0.0.1.dist-info/METADATA
+Filename: cookiecutter.json
 Comment: 
 
-Filename: fastapi_cookiecutter-0.0.1.dist-info/WHEEL
+Filename: fastapi_cookiecutter/__init__.py
 Comment: 
 
-Filename: fastapi_cookiecutter-0.0.1.dist-info/top_level.txt
+Filename: fastapi_cookiecutter/main.py
 Comment: 
 
-Filename: fastapi_cookiecutter-0.0.1.dist-info/RECORD
+Filename: hooks/post_gen_project.py
+Comment: 
+
+Filename: hooks/pre_gen_project.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.coveragerc
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.github/workflows/build.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.github/workflows/sphinx.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.github/workflows/test.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.gitignore
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/.gitlab-ci.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/CONTRIBUTING.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/LICENSES/2-Clause BSD
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/LICENSES/3-Clause BSD
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/LICENSES/APACHE
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/LICENSES/GPL
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/LICENSES/MIT
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/MANIFEST.in
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/Makefile
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/README.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/bitbucket-pipelines.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/Dockerfile
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/Dockerfile.local
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/compose_hooks/post_build.sh
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/compose_hooks/pre_build.sh
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/docker-compose.yml
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker/init.sql
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docker-compose.sh
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/Makefile
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/make.bat
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/01_about.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/02_usage.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/03_source.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/04_authors.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/05_contributing.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/conf.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/docs/source/index.rst
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/requirements/base.txt
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/requirements/dev.txt
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/requirements/doc.txt
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/scripts/.keep
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/scripts/prestart.sh
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/setup.cfg
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/setup.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/conftest.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/resources/.keep
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_api/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_api/test_auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_api/test_base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_application.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_configs/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_configs/test_base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_db/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_db/test_base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_db/test_models/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_db/test_models/test_auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_db/test_session.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_events/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_events/test_base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_middlewares/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_middlewares/test_logging.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_schemas/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_schemas/test_auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_schemas/test_base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_logging/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_colorformatter.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_helper.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_logging/test_standardformatter.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_security.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/tests/test_utils/test_storage.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/api/base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/application.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/dev.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/prod.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/configs/test.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/constants.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/models/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/models/auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/queries/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/db/session.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/events/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/events/base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/globals.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/middlewares/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/middlewares/logging.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/auth.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/schemas/base.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/services/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/__init__.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/errors.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/logging.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/security.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/utils/storage.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/app/version.py
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/.keep
+Comment: 
+
+Filename: {{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
+Comment: 
+
+Filename: fastapi_cookiecutter-0.1.0.dist-info/LICENSE
+Comment: 
+
+Filename: fastapi_cookiecutter-0.1.0.dist-info/METADATA
+Comment: 
+
+Filename: fastapi_cookiecutter-0.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: fastapi_cookiecutter-0.1.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: fastapi_cookiecutter-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

