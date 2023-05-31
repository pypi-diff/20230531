# Comparing `tmp/edsnlp-0.8.0.tar.gz` & `tmp/edsnlp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsnlp-0.8.0.tar", last modified: Thu May 25 07:54:46 2023, max compression
+gzip compressed data, was "edsnlp-0.8.1.tar", last modified: Wed May 31 11:42:33 2023, max compression
```

## Comparing `edsnlp-0.8.0.tar` & `edsnlp-0.8.1.tar`

### file list

```diff
@@ -1,485 +1,489 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.399655 edsnlp-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-25 07:54:19.000000 edsnlp-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-25 07:54:46.399655 edsnlp-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 07:54:19.000000 edsnlp-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-25 07:54:19.000000 edsnlp-0.8.0/demo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.283655 edsnlp-0.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-25 07:54:19.000000 edsnlp-0.8.0/docs/scripts/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/edsnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/conjugator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.319655 edsnlp-0.8.0/edsnlp/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20290 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/brat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/labeltool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.319655 edsnlp-0.8.0/edsnlp/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1214559 2023-05-25 07:54:43.000000 edsnlp-0.8.0/edsnlp/matchers/phrase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/simstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/matchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/patch_spacy_dot_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/context/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlinesmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/accents.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)  1054497 2023-05-25 07:54:45.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/sentences.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/terminology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/absolute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/current.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/false_positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/relative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/adicap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/AIDS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/CKD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/COPD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/dementia.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/base_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/sofa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/tnm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/family.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/negation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/terminations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/trainable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/crf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/pytorch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/processing/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.375655 edsnlp-0.8.0/edsnlp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/AVC.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)    95841 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/adicap.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   604577 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/cim10.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   136088 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/drugs.json
--rw-r--r--   0 runner    (1001) docker     (123)   200566 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/verbs.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/edsnlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/blocs.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/inclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/merge_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/span_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/edsnlp/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/viz/quick_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/edsnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/connectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/dates/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/dates/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/normalizer/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/sections/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/sentences/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/sentences/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/tokenizer/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-05-25 07:54:19.000000 edsnlp-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/adicap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/cim10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/conjugate_verbs.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:54:46.399655 edsnlp-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-25 07:54:19.000000 edsnlp-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_brat.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_labeltool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_omop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_phrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_simstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/core/
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_contextual_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_endlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_sentences.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_terminology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_consultation_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.387655 edsnlp-0.8.0/tests/pipelines/ner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/ner/disorders/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/AIDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/CKD.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/COPD.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/cerebrovascular_accident.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/congestive_heart_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/connective_tissue_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/dementia.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/hemiplegia.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/leukemia.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/liver_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/lymphoma.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/myocardial_infarction.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/peptic_ulcer_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/peripheral_vascular_disease.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/solid_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/tobacco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_adicap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_adicap_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_cim10.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_covid.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_drugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_tnm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_umls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/qualifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_negation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_reported_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/test_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/trainable/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/trainable/test_nested_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/trainable/test_span_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/processing/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_conjugator.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_quick_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.721783 edsnlp-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-31 11:42:12.000000 edsnlp-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-31 11:42:33.721783 edsnlp-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-31 11:42:12.000000 edsnlp-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.677783 edsnlp-0.8.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-31 11:42:12.000000 edsnlp-0.8.1/demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.665783 edsnlp-0.8.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.677783 edsnlp-0.8.1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 11:42:12.000000 edsnlp-0.8.1/docs/scripts/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.677783 edsnlp-0.8.1/edsnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/conjugator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.677783 edsnlp-0.8.1/edsnlp/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20290 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/connectors/brat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/connectors/labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/connectors/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1215942 2023-05-31 11:42:31.000000 edsnlp-0.8.1/edsnlp/matchers/phrase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/phrase.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/phrase.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/matchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/utils/offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/matchers/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/patch_spacy_dot_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/pipelines/core/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/context/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.681783 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/endlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/endlinesmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/endlines/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/matcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/matcher/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/accents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/lowercase/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/lowercase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/lowercase/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/pollution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/quotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.685783 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1055664 2023-05-31 11:42:32.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/sentences.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/sentences.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/sentences.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/sentences/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/core/terminology/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/terminology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/terminology/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/core/terminology/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/absolute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/false_positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/relative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.689783 edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/misc/reason/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/reason/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/reason/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/reason/reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/misc/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/sections/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/sections/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/sections/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/misc/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/tables/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/tables/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/misc/tables/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/covid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/covid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/covid/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/covid/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.693783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/AIDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/CKD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/COPD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.697783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/drugs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/drugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/drugs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/drugs/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/base_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.701783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/sofa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/tnm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/ner/umls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/umls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/umls/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/ner/umls/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/negation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.705783 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/pipelines/trainable/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/layers/crf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/pytorch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/processing/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.709783 edsnlp-0.8.1/edsnlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/resources/AVC.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    95841 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/resources/adicap.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   604577 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/resources/cim10.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   136088 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/resources/drugs.json
+-rw-r--r--   0 runner    (1001) docker     (123)   200566 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/resources/verbs.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/edsnlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/blocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/inclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/merge_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/span_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/edsnlp/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-31 11:42:12.000000 edsnlp-0.8.1/edsnlp/viz/quick_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.677783 edsnlp-0.8.1/edsnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 11:42:33.000000 edsnlp-0.8.1/edsnlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/connectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/dates/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/dates/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/normalizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/sections/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/sentences/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/sentences/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/tokenizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/notebooks/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 11:42:12.000000 edsnlp-0.8.1/notebooks/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-31 11:42:12.000000 edsnlp-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-31 11:42:12.000000 edsnlp-0.8.1/scripts/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 11:42:12.000000 edsnlp-0.8.1/scripts/cim10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-31 11:42:12.000000 edsnlp-0.8.1/scripts/conjugate_verbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 11:42:12.000000 edsnlp-0.8.1/scripts/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-31 11:42:12.000000 edsnlp-0.8.1/scripts/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:42:33.721783 edsnlp-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-31 11:42:12.000000 edsnlp-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/connectors/test_brat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/connectors/test_labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/connectors/test_omop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/matchers/test_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/matchers/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/matchers/test_simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.713783 edsnlp-0.8.1/tests/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.717783 edsnlp-0.8.1/tests/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_endlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_sentences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/core/test_terminology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.717783 edsnlp-0.8.1/tests/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_consultation_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/misc/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.717783 edsnlp-0.8.1/tests/pipelines/ner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.717783 edsnlp-0.8.1/tests/pipelines/ner/disorders/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/AIDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/CKD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/COPD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/peptic_ulcer_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/peripheral_vascular_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/disorders/tobacco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_adicap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_cim10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_covid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_drugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_tnm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/ner/test_umls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.721783 edsnlp-0.8.1/tests/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/test_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/test_negation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/qualifiers/test_reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.721783 edsnlp-0.8.1/tests/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/trainable/test_nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/pipelines/trainable/test_span_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.721783 edsnlp-0.8.1/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/processing/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/test_conjugator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/test_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:42:33.721783 edsnlp-0.8.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/utils/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/utils/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 11:42:12.000000 edsnlp-0.8.1/tests/utils/test_quick_examples.py
```

### Comparing `edsnlp-0.8.0/LICENSE` & `edsnlp-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/PKG-INFO` & `edsnlp-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsnlp
-Version: 0.8.0
+Version: 0.8.1
 Summary: A set of spaCy components to extract information from clinical notes written in French
 Author-email: Data Science - DSN APHP <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2021 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -50,15 +50,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.8.0
+pip install edsnlp==0.8.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.8.0/README.md` & `edsnlp-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.8.0
+pip install edsnlp==0.8.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.8.0/demo/app.py` & `edsnlp-0.8.1/demo/app.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/docs/scripts/plugin.py` & `edsnlp-0.8.1/docs/scripts/plugin.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/conjugator.py` & `edsnlp-0.8.1/edsnlp/conjugator.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/connectors/brat.py` & `edsnlp-0.8.1/edsnlp/connectors/brat.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/connectors/labeltool.py` & `edsnlp-0.8.1/edsnlp/connectors/labeltool.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/connectors/omop.py` & `edsnlp-0.8.1/edsnlp/connectors/omop.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/language.py` & `edsnlp-0.8.1/edsnlp/language.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/matchers/phrase.cpp` & `edsnlp-0.8.1/edsnlp/matchers/phrase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.matchers.phrase",
         "sources": [
             "edsnlp/matchers/phrase.pyx"
         ]
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,16 +102,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1233,195 +1237,195 @@
 /* "typedefs.pxd":11
  * ctypedef uint64_t flags_t
  * ctypedef uint16_t len_t
  * ctypedef uint16_t tag_t             # <<<<<<<<<<<<<<
  */
 typedef uint16_t __pyx_t_5spacy_8typedefs_tag_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -2286,42 +2290,42 @@
   std::vector<int>  first_head;
   std::vector<int>  first_tail;
   std::unordered_set<int>  *roots;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *node_map;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *edge_map;
 };
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3814,30 +3818,30 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
@@ -4199,18 +4203,18 @@
 static PyObject *__Pyx_Generator_Next(PyObject *self);
 static int __pyx_Generator_init(void);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static void __pyx_f_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_find_matches(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, struct __pyx_obj_5spacy_6tokens_3doc_Doc *__pyx_v_doc, int __pyx_v_start_idx, int __pyx_v_end_idx, std::vector<struct __pyx_t_5spacy_7structs_SpanC>  *__pyx_v_matches); /* proto*/
 static CYTHON_INLINE struct __pyx_obj_5spacy_6tokens_4span_Span *__pyx_f_5spacy_6tokens_4span_4Span_cinit(struct __pyx_obj_5spacy_6tokens_3doc_Doc *__pyx_v_doc, struct __pyx_t_5spacy_7structs_SpanC __pyx_v_span); /* proto*/
 static CYTHON_INLINE struct __pyx_obj_5spacy_6lexeme_Lexeme *__pyx_f_5spacy_6lexeme_6Lexeme_from_ptr(struct __pyx_t_5spacy_7structs_LexemeC *__pyx_v_lex, struct __pyx_obj_5spacy_5vocab_Vocab *__pyx_v_vocab); /* proto*/
@@ -7517,15 +7521,15 @@
   __Pyx_WriteUnraisable("edsnlp.matchers.phrase.make_spanstruct", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7536,29 +7540,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[2], 735, 0, __PYX_ERR(2, 735, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7570,15 +7574,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7589,29 +7593,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[2], 738, 0, __PYX_ERR(2, 738, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7623,15 +7627,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7642,29 +7646,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[2], 741, 0, __PYX_ERR(2, 741, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7676,15 +7680,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7695,29 +7699,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[2], 744, 0, __PYX_ERR(2, 744, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7729,15 +7733,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7748,29 +7752,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[2], 747, 0, __PYX_ERR(2, 747, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7782,15 +7786,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7801,60 +7805,60 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[2], 750, 0, __PYX_ERR(2, 750, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7865,15 +7869,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7882,33 +7886,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[2], 929, 0, __PYX_ERR(2, 929, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7917,15 +7921,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7937,66 +7941,66 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[2], 933, 0, __PYX_ERR(2, 933, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -8007,15 +8011,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8033,15 +8037,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[2], 941, 0, __PYX_ERR(2, 941, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8049,53 +8053,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -8103,30 +8107,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8142,15 +8146,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8168,15 +8172,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[2], 947, 0, __PYX_ERR(2, 947, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8184,53 +8188,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -8238,30 +8242,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8277,15 +8281,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8303,15 +8307,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[2], 953, 0, __PYX_ERR(2, 953, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8319,53 +8323,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -8373,30 +8377,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8412,15 +8416,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8430,25 +8434,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[2], 967, 0, __PYX_ERR(2, 967, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8458,15 +8462,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8476,25 +8480,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[2], 982, 0, __PYX_ERR(2, 982, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8504,15 +8508,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8520,25 +8524,25 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[2], 997, 1, __PYX_ERR(2, 997, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8547,15 +8551,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8563,25 +8567,25 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[2], 1007, 1, __PYX_ERR(2, 1007, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8590,15 +8594,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8606,23 +8610,23 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[2], 1014, 1, __PYX_ERR(2, 1014, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -24223,15 +24227,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns *__pyx_freelist_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns[8];
 static int __pyx_freecount_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns = 0;
 
@@ -24348,15 +24352,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr *__pyx_freelist_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr = 0;
 
@@ -24461,15 +24465,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -24653,15 +24657,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -24775,15 +24779,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -25039,15 +25043,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -25188,15 +25192,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -25463,26 +25467,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_map cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_self_c_map_cannot_be_converted_t); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 951, __pyx_L1_error)
@@ -25833,17 +25837,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_t_1 = PyImport_ImportModule("spacy.matcher.phrasematcher"); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher = __Pyx_ImportType(__pyx_t_1, "spacy.matcher.phrasematcher", "PhraseMatcher", sizeof(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.matcher.phrasematcher", "PhraseMatcher", sizeof(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher = (struct __pyx_vtabstruct_5spacy_7matcher_13phrasematcher_PhraseMatcher*)__Pyx_GetVtable(__pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_6edsnlp_8matchers_6phrase_EDSPhraseMatcher = &__pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher;
   __pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.__pyx_base = *__pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher;
   __pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.__pyx_base.find_matches = (void (*)(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher *, struct __pyx_obj_5spacy_6tokens_3doc_Doc *, int, int, std::vector<struct __pyx_t_5spacy_7structs_SpanC>  *))__pyx_f_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_find_matches;
   __pyx_type_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.tp_base = __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher;
   if (PyType_Ready(&__pyx_type_6edsnlp_8matchers_6phrase_EDSPhraseMatcher) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
@@ -25948,147 +25950,90 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("cymem.cymem"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyMalloc),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(6, 4, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_PyMalloc),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(6, 4, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyMalloc = (struct __pyx_vtabstruct_5cymem_5cymem_PyMalloc*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyMalloc->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyMalloc)) __PYX_ERR(6, 4, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyFree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(6, 10, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_PyFree),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(6, 10, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyFree = (struct __pyx_vtabstruct_5cymem_5cymem_PyFree*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyFree->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyFree)) __PYX_ERR(6, 10, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Pool),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(6, 16, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_Pool),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(6, 16, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_Pool = (struct __pyx_vtabstruct_5cymem_5cymem_Pool*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_Pool->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_Pool)) __PYX_ERR(6, 16, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Address),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(6, 28, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_Address),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(6, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("preshed.maps"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
+  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType_0_29_35(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_7preshed_4maps_PreshMap),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMap = (struct __pyx_vtabstruct_7preshed_4maps_PreshMap*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMap->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMap)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMapArray),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
+  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType_0_29_35(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_7preshed_4maps_PreshMapArray),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMapArray = (struct __pyx_vtabstruct_7preshed_4maps_PreshMapArray*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMapArray->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMapArray)) __PYX_ERR(7, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(8, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.strings"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7strings_StringStore),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(9, 22, __pyx_L1_error)
+  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_7strings_StringStore),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(9, 22, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7strings_StringStore = (struct __pyx_vtabstruct_5spacy_7strings_StringStore*)__Pyx_GetVtable(__pyx_ptype_5spacy_7strings_StringStore->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7strings_StringStore)) __PYX_ERR(9, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.morphology"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_10morphology_Morphology),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_10morphology_Morphology),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(10, 11, __pyx_L1_error)
   __pyx_vtabptr_5spacy_10morphology_Morphology = (struct __pyx_vtabstruct_5spacy_10morphology_Morphology*)__Pyx_GetVtable(__pyx_ptype_5spacy_10morphology_Morphology->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_10morphology_Morphology)) __PYX_ERR(10, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_5vocab_Vocab),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(11, 26, __pyx_L1_error)
+  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_5vocab_Vocab),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(11, 26, __pyx_L1_error)
   __pyx_vtabptr_5spacy_5vocab_Vocab = (struct __pyx_vtabstruct_5spacy_5vocab_Vocab*)__Pyx_GetVtable(__pyx_ptype_5spacy_5vocab_Vocab->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_5vocab_Vocab)) __PYX_ERR(11, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.doc"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_3doc_Doc),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(12, 37, __pyx_L1_error)
+  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6tokens_3doc_Doc),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(12, 37, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_3doc_Doc = (struct __pyx_vtabstruct_5spacy_6tokens_3doc_Doc*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_3doc_Doc->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_3doc_Doc)) __PYX_ERR(12, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.span"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_4span_Span = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.span", "Span", sizeof(struct __pyx_obj_5spacy_6tokens_4span_Span), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_4span_Span),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6tokens_4span_Span) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_5spacy_6tokens_4span_Span = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.tokens.span", "Span", sizeof(struct __pyx_obj_5spacy_6tokens_4span_Span), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6tokens_4span_Span),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6tokens_4span_Span) __PYX_ERR(3, 8, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_4span_Span = (struct __pyx_vtabstruct_5spacy_6tokens_4span_Span*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_4span_Span->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_4span_Span)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6lexeme_Lexeme),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6lexeme_Lexeme),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(4, 15, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6lexeme_Lexeme = (struct __pyx_vtabstruct_5spacy_6lexeme_Lexeme*)__Pyx_GetVtable(__pyx_ptype_5spacy_6lexeme_Lexeme->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6lexeme_Lexeme)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_5token_Token),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(5, 14, __pyx_L1_error)
+  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6tokens_5token_Token),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(5, 14, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_5token_Token = (struct __pyx_vtabstruct_5spacy_6tokens_5token_Token*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_5token_Token->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_5token_Token)) __PYX_ERR(5, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -26101,24 +26046,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_5vocab_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_5vocab_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_6lexeme_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "OOV_RANK", (void **)&__pyx_vp_5spacy_6lexeme_OOV_RANK, "__pyx_t_5spacy_8typedefs_attr_t") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_6lexeme_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "OOV_RANK", (void **)&__pyx_vp_5spacy_6lexeme_OOV_RANK, "__pyx_t_5spacy_8typedefs_attr_t") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "MISSING_DEP", (void **)&__pyx_vp_5spacy_6tokens_5token_MISSING_DEP, "int") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "MISSING_DEP", (void **)&__pyx_vp_5spacy_6tokens_5token_MISSING_DEP, "int") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -26130,23 +26075,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("preshed.maps"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "map_get", (void (**)(void))&__pyx_f_7preshed_4maps_map_get, "void *(struct __pyx_t_7preshed_4maps_MapStruct const *, __pyx_t_7preshed_4maps_key_t const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "map_set", (void (**)(void))&__pyx_f_7preshed_4maps_map_set, "void (struct __pyx_obj_5cymem_5cymem_Pool *, struct __pyx_t_7preshed_4maps_MapStruct *, __pyx_t_7preshed_4maps_key_t, void *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "map_init", (void (**)(void))&__pyx_f_7preshed_4maps_map_init, "void (struct __pyx_obj_5cymem_5cymem_Pool *, struct __pyx_t_7preshed_4maps_MapStruct *, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "map_iter", (void (**)(void))&__pyx_f_7preshed_4maps_map_iter, "int (struct __pyx_t_7preshed_4maps_MapStruct const *, int *, __pyx_t_7preshed_4maps_key_t *, void **)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "map_clear", (void (**)(void))&__pyx_f_7preshed_4maps_map_clear, "void *(struct __pyx_t_7preshed_4maps_MapStruct *, __pyx_t_7preshed_4maps_key_t const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "map_get", (void (**)(void))&__pyx_f_7preshed_4maps_map_get, "void *(struct __pyx_t_7preshed_4maps_MapStruct const *, __pyx_t_7preshed_4maps_key_t const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "map_set", (void (**)(void))&__pyx_f_7preshed_4maps_map_set, "void (struct __pyx_obj_5cymem_5cymem_Pool *, struct __pyx_t_7preshed_4maps_MapStruct *, __pyx_t_7preshed_4maps_key_t, void *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "map_init", (void (**)(void))&__pyx_f_7preshed_4maps_map_init, "void (struct __pyx_obj_5cymem_5cymem_Pool *, struct __pyx_t_7preshed_4maps_MapStruct *, size_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "map_iter", (void (**)(void))&__pyx_f_7preshed_4maps_map_iter, "int (struct __pyx_t_7preshed_4maps_MapStruct const *, int *, __pyx_t_7preshed_4maps_key_t *, void **)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "map_clear", (void (**)(void))&__pyx_f_7preshed_4maps_map_clear, "void *(struct __pyx_t_7preshed_4maps_MapStruct *, __pyx_t_7preshed_4maps_key_t const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("murmurhash.mrmr"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "hash64", (void (**)(void))&__pyx_f_10murmurhash_4mrmr_hash64, "uint64_t (void *, int, uint64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "hash64", (void (**)(void))&__pyx_f_10murmurhash_4mrmr_hash64, "uint64_t (void *, int, uint64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -28648,18 +28593,18 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -28705,22 +28650,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -29622,15 +29567,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -30093,15 +30038,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -30289,15 +30234,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -30523,15 +30468,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -31792,15 +31737,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
@@ -31845,17 +31793,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-#ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -31894,17 +31842,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `edsnlp-0.8.0/edsnlp/matchers/regex.py` & `edsnlp-0.8.1/edsnlp/matchers/regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/matchers/simstring.py` & `edsnlp-0.8.1/edsnlp/matchers/simstring.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/matchers/utils/offset.py` & `edsnlp-0.8.1/edsnlp/matchers/utils/offset.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/matchers/utils/text.py` & `edsnlp-0.8.1/edsnlp/matchers/utils/text.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/patch_spacy_dot_components.py` & `edsnlp-0.8.1/edsnlp/patch_spacy_dot_components.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/base.py` & `edsnlp-0.8.1/edsnlp/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/context/context.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/context/context.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/models.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/contextual_matcher/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlines.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/endlines/endlines.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlinesmodel.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/endlines/endlinesmodel.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/functional.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/endlines/functional.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/matcher/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/matcher/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/matcher/matcher.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/__init__.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/accents.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/accents.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/accents/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/lowercase/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/normalizer.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/pollution/pollution.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/quotes/quotes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/spaces.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/normalizer/spaces/spaces.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/sentences/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/sentences.cpp` & `edsnlp-0.8.1/edsnlp/pipelines/core/sentences/sentences.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.pipelines.core.sentences.sentences",
         "sources": [
             "edsnlp/pipelines/core/sentences/sentences.pyx"
         ]
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,16 +102,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1163,195 +1167,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1479,42 +1483,42 @@
  * ctypedef void* (*malloc_t)(size_t n)
  * ctypedef void (*free_t)(void *p)             # <<<<<<<<<<<<<<
  * 
  * cdef class PyMalloc:
  */
 typedef void (*__pyx_t_5cymem_5cymem_free_t)(void *);
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3419,30 +3423,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -3664,18 +3668,18 @@
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* VoidPtrImport.proto */
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig);
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static void __pyx_f_6edsnlp_9pipelines_4core_9sentences_9sentences_17SentenceSegmenter_process(struct __pyx_obj_6edsnlp_9pipelines_4core_9sentences_9sentences_SentenceSegmenter *__pyx_v_self, struct __pyx_obj_5spacy_6tokens_3doc_Doc *__pyx_v_doc); /* proto*/
 static CYTHON_INLINE struct __pyx_obj_5spacy_6lexeme_Lexeme *__pyx_f_5spacy_6lexeme_6Lexeme_from_ptr(struct __pyx_t_5spacy_7structs_LexemeC *__pyx_v_lex, struct __pyx_obj_5spacy_5vocab_Vocab *__pyx_v_vocab); /* proto*/
 static CYTHON_INLINE void __pyx_f_5spacy_6lexeme_6Lexeme_set_struct_attr(struct __pyx_t_5spacy_7structs_LexemeC *__pyx_v_lex, enum __pyx_t_5spacy_5attrs_attr_id_t __pyx_v_name, __pyx_t_5spacy_8typedefs_attr_t __pyx_v_value); /* proto*/
@@ -5884,15 +5888,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5901,29 +5905,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5934,15 +5938,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5951,29 +5955,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5984,15 +5988,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6001,29 +6005,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6034,15 +6038,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6051,29 +6055,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6084,15 +6088,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6101,29 +6105,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6134,212 +6138,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6355,15 +6359,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6371,53 +6375,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -6425,30 +6429,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6463,15 +6467,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6487,15 +6491,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6503,53 +6507,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -6557,30 +6561,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6595,15 +6599,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6619,15 +6623,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6635,53 +6639,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -6689,30 +6693,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6727,176 +6731,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22109,15 +22113,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -22301,15 +22305,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -22423,15 +22427,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -22687,15 +22691,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -22836,15 +22840,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -23059,26 +23063,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x80392e3, 0x56d5ac8, 0x70dfbb1) = (capitalized_shapes_hash, endline_hash, excluded_hash, ignore_excluded, newline_hash, punct_chars_hash))" % __pyx_checksum)
  */
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_134451939, __pyx_int_91052744, __pyx_int_118356913); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-1pz4ptgf/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 951, __pyx_L1_error)
@@ -23498,140 +23502,85 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("cymem.cymem"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyMalloc),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(5, 4, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_PyMalloc),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(5, 4, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyMalloc = (struct __pyx_vtabstruct_5cymem_5cymem_PyMalloc*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyMalloc->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyMalloc)) __PYX_ERR(5, 4, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyFree),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(5, 10, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_PyFree),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyFree = (struct __pyx_vtabstruct_5cymem_5cymem_PyFree*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyFree->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyFree)) __PYX_ERR(5, 10, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Pool),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(5, 16, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_Pool),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(5, 16, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_Pool = (struct __pyx_vtabstruct_5cymem_5cymem_Pool*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_Pool->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_Pool)) __PYX_ERR(5, 16, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Address),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(5, 28, __pyx_L1_error)
+  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType_0_29_35(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5cymem_5cymem_Address),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(5, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("preshed.maps"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMap),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
+  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType_0_29_35(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_7preshed_4maps_PreshMap),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMap = (struct __pyx_vtabstruct_7preshed_4maps_PreshMap*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMap->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMap)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMapArray),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
+  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType_0_29_35(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_7preshed_4maps_PreshMapArray),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMapArray = (struct __pyx_vtabstruct_7preshed_4maps_PreshMapArray*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMapArray->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMapArray)) __PYX_ERR(7, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.strings"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7strings_StringStore),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(8, 22, __pyx_L1_error)
+  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_7strings_StringStore),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(8, 22, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7strings_StringStore = (struct __pyx_vtabstruct_5spacy_7strings_StringStore*)__Pyx_GetVtable(__pyx_ptype_5spacy_7strings_StringStore->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7strings_StringStore)) __PYX_ERR(8, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.morphology"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_10morphology_Morphology),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(9, 11, __pyx_L1_error)
+  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_10morphology_Morphology),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(9, 11, __pyx_L1_error)
   __pyx_vtabptr_5spacy_10morphology_Morphology = (struct __pyx_vtabstruct_5spacy_10morphology_Morphology*)__Pyx_GetVtable(__pyx_ptype_5spacy_10morphology_Morphology->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_10morphology_Morphology)) __PYX_ERR(9, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_5vocab_Vocab),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(10, 26, __pyx_L1_error)
+  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_5vocab_Vocab),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(10, 26, __pyx_L1_error)
   __pyx_vtabptr_5spacy_5vocab_Vocab = (struct __pyx_vtabstruct_5spacy_5vocab_Vocab*)__Pyx_GetVtable(__pyx_ptype_5spacy_5vocab_Vocab->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_5vocab_Vocab)) __PYX_ERR(10, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.doc"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_3doc_Doc),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(11, 37, __pyx_L1_error)
+  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6tokens_3doc_Doc),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(11, 37, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_3doc_Doc = (struct __pyx_vtabstruct_5spacy_6tokens_3doc_Doc*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_3doc_Doc->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_3doc_Doc)) __PYX_ERR(11, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6lexeme_Lexeme),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6lexeme_Lexeme),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(3, 15, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6lexeme_Lexeme = (struct __pyx_vtabstruct_5spacy_6lexeme_Lexeme*)__Pyx_GetVtable(__pyx_ptype_5spacy_6lexeme_Lexeme->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6lexeme_Lexeme)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_5token_Token),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(4, 14, __pyx_L1_error)
+  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType_0_29_35(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_5spacy_6tokens_5token_Token),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(4, 14, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_5token_Token = (struct __pyx_vtabstruct_5spacy_6tokens_5token_Token*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_5token_Token->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_5token_Token)) __PYX_ERR(4, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -23644,24 +23593,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_5vocab_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_5vocab_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_6lexeme_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "OOV_RANK", (void **)&__pyx_vp_5spacy_6lexeme_OOV_RANK, "__pyx_t_5spacy_8typedefs_attr_t") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "EMPTY_LEXEME", (void **)&__pyx_vp_5spacy_6lexeme_EMPTY_LEXEME, "struct __pyx_t_5spacy_7structs_LexemeC") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "OOV_RANK", (void **)&__pyx_vp_5spacy_6lexeme_OOV_RANK, "__pyx_t_5spacy_8typedefs_attr_t") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportVoidPtr(__pyx_t_1, "MISSING_DEP", (void **)&__pyx_vp_5spacy_6tokens_5token_MISSING_DEP, "int") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_0_29_35(__pyx_t_1, "MISSING_DEP", (void **)&__pyx_vp_5spacy_6tokens_5token_MISSING_DEP, "int") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -23673,15 +23622,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("murmurhash.mrmr"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "hash64", (void (**)(void))&__pyx_f_10murmurhash_4mrmr_hash64, "uint64_t (void *, int, uint64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "hash64", (void (**)(void))&__pyx_f_10murmurhash_4mrmr_hash64, "uint64_t (void *, int, uint64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -25925,18 +25874,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -25982,22 +25931,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -26773,15 +26722,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26969,15 +26918,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27203,15 +27152,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27636,15 +27585,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27811,17 +27760,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* VoidPtrImport */
-#ifndef __PYX_HAVE_RT_ImportVoidPtr
-#define __PYX_HAVE_RT_ImportVoidPtr
-static int __Pyx_ImportVoidPtr(PyObject *module, const char *name, void **p, const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+#define __PYX_HAVE_RT_ImportVoidPtr_0_29_35
+static int __Pyx_ImportVoidPtr_0_29_35(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
     if (!d)
         goto bad;
     cobj = PyDict_GetItemString(d, name);
     if (!cobj) {
@@ -27860,17 +27809,17 @@
 bad:
     Py_XDECREF(d);
     return -1;
 }
 #endif
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/terms.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/sentences/terms.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/terminology/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/terminology/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/core/terminology/terminology.py` & `edsnlp-0.8.1/edsnlp/pipelines/core/terminology/terminology.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/factories.py` & `edsnlp-0.8.1/edsnlp/pipelines/factories.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/consultation_dates/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/dates.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/models.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/absolute.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/absolute.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/days.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/months.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/atomic/time.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/relative.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/dates/patterns/relative.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/measurements.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/measurements/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/reason/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/reason/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/reason.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/reason/reason.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/sections/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/sections/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/sections.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/sections/sections.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/tables/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/tables/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/misc/tables/tables.py` & `edsnlp-0.8.1/edsnlp/pipelines/misc/tables/tables.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/adicap.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/adicap/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/cim10/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/covid/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/covid/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/AIDS.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/AIDS.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/AIDS/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/CKD.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/CKD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/CKD/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/COPD.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/COPD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/COPD/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/base.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/base.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/dementia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/diabetes/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/leukemia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/terms.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/disorders/terms.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/drugs/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/base_score.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/base_score.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/charlson/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/elstonellis/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/sofa.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/sofa/sofa.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/models.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/tnm.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/scores/tnm/tnm.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/umls/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/umls/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/ner/umls/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/ner/umls/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/base.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/base.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/family.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/family.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/family/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/history.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/history/history.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/hypothesis/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/negation.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/negation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/negation/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py` & `edsnlp-0.8.1/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/terminations.py` & `edsnlp-0.8.1/edsnlp/pipelines/terminations.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/crf.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/layers/crf.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/nested_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/pytorch_wrapper.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/factory.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/utils.py` & `edsnlp-0.8.1/edsnlp/pipelines/trainable/span_qualifier/utils.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/processing/distributed.py` & `edsnlp-0.8.1/edsnlp/processing/distributed.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/processing/helpers.py` & `edsnlp-0.8.1/edsnlp/processing/helpers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/processing/parallel.py` & `edsnlp-0.8.1/edsnlp/processing/parallel.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/processing/simple.py` & `edsnlp-0.8.1/edsnlp/processing/simple.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/processing/wrapper.py` & `edsnlp-0.8.1/edsnlp/processing/wrapper.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/resources/AVC.csv.gz` & `edsnlp-0.8.1/edsnlp/resources/AVC.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/resources/adicap.json.gz` & `edsnlp-0.8.1/edsnlp/resources/adicap.json.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/resources/cim10.csv.gz` & `edsnlp-0.8.1/edsnlp/resources/cim10.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/resources/drugs.json` & `edsnlp-0.8.1/edsnlp/resources/drugs.json`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/resources/verbs.csv.gz` & `edsnlp-0.8.1/edsnlp/resources/verbs.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/blocs.py` & `edsnlp-0.8.1/edsnlp/utils/blocs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/colors.py` & `edsnlp-0.8.1/edsnlp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/deprecation.py` & `edsnlp-0.8.1/edsnlp/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/examples.py` & `edsnlp-0.8.1/edsnlp/utils/examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/filter.py` & `edsnlp-0.8.1/edsnlp/utils/filter.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/inclusion.py` & `edsnlp-0.8.1/edsnlp/utils/inclusion.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/merge_configs.py` & `edsnlp-0.8.1/edsnlp/utils/merge_configs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/numbers.py` & `edsnlp-0.8.1/edsnlp/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/regex.py` & `edsnlp-0.8.1/edsnlp/utils/regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/resources.py` & `edsnlp-0.8.1/edsnlp/utils/resources.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/span_getters.py` & `edsnlp-0.8.1/edsnlp/utils/span_getters.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/utils/training.py` & `edsnlp-0.8.1/edsnlp/utils/training.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp/viz/quick_examples.py` & `edsnlp-0.8.1/edsnlp/viz/quick_examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp.egg-info/PKG-INFO` & `edsnlp-0.8.1/edsnlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsnlp
-Version: 0.8.0
+Version: 0.8.1
 Summary: A set of spaCy components to extract information from clinical notes written in French
 Author-email: Data Science - DSN APHP <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2021 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -50,15 +50,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.8.0
+pip install edsnlp==0.8.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.8.0/edsnlp.egg-info/SOURCES.txt` & `edsnlp-0.8.1/edsnlp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 edsnlp.egg-info/top_level.txt
 edsnlp/connectors/__init__.py
 edsnlp/connectors/brat.py
 edsnlp/connectors/labeltool.py
 edsnlp/connectors/omop.py
 edsnlp/matchers/__init__.py
 edsnlp/matchers/phrase.cpp
+edsnlp/matchers/phrase.pxd
+edsnlp/matchers/phrase.pyx
 edsnlp/matchers/regex.py
 edsnlp/matchers/simstring.py
 edsnlp/matchers/utils/__init__.py
 edsnlp/matchers/utils/offset.py
 edsnlp/matchers/utils/text.py
 edsnlp/pipelines/__init__.py
 edsnlp/pipelines/base.py
@@ -66,14 +68,16 @@
 edsnlp/pipelines/core/normalizer/quotes/quotes.py
 edsnlp/pipelines/core/normalizer/spaces/__init__.py
 edsnlp/pipelines/core/normalizer/spaces/factory.py
 edsnlp/pipelines/core/normalizer/spaces/spaces.py
 edsnlp/pipelines/core/sentences/__init__.py
 edsnlp/pipelines/core/sentences/factory.py
 edsnlp/pipelines/core/sentences/sentences.cpp
+edsnlp/pipelines/core/sentences/sentences.pxd
+edsnlp/pipelines/core/sentences/sentences.pyx
 edsnlp/pipelines/core/sentences/terms.py
 edsnlp/pipelines/core/terminology/__init__.py
 edsnlp/pipelines/core/terminology/factory.py
 edsnlp/pipelines/core/terminology/terminology.py
 edsnlp/pipelines/misc/__init__.py
 edsnlp/pipelines/misc/consultation_dates/__init__.py
 edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
```

### Comparing `edsnlp-0.8.0/edsnlp.egg-info/entry_points.txt` & `edsnlp-0.8.1/edsnlp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/edsnlp.egg-info/requires.txt` & `edsnlp-0.8.1/edsnlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/pyproject.toml` & `edsnlp-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 "Bug Tracker" = "https://github.com/aphp/edsnlp/issues"
 
 [tool.setuptools.dynamic]
 version = { attr = "edsnlp.__version__" }
 
 [tool.setuptools.package-data]
 "edsnlp" = [
-    "*.pyx",
-    "*.pxd",
-    "*.pxi",
+    "**/*.pyx",
+    "**/*.pxd",
+    "**/*.pxi",
     "resources/*.csv",
     "resources/*.json",
     "resources/*.csv.gz",
     "resources/*.json.gz",
 ]
 
 [tool.setuptools.packages.find]
```

### Comparing `edsnlp-0.8.0/scripts/adicap.py` & `edsnlp-0.8.1/scripts/adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/scripts/cim10.py` & `edsnlp-0.8.1/scripts/cim10.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/scripts/conjugate_verbs.py` & `edsnlp-0.8.1/scripts/conjugate_verbs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/scripts/serve.py` & `edsnlp-0.8.1/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/setup.py` & `edsnlp-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/conftest.py` & `edsnlp-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/connectors/test_brat.py` & `edsnlp-0.8.1/tests/connectors/test_brat.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/connectors/test_omop.py` & `edsnlp-0.8.1/tests/connectors/test_omop.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/matchers/test_phrase.py` & `edsnlp-0.8.1/tests/matchers/test_phrase.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/matchers/test_regex.py` & `edsnlp-0.8.1/tests/matchers/test_regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/matchers/test_simstring.py` & `edsnlp-0.8.1/tests/matchers/test_simstring.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_contextual_matcher.py` & `edsnlp-0.8.1/tests/pipelines/core/test_contextual_matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_endlines.py` & `edsnlp-0.8.1/tests/pipelines/core/test_endlines.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_matcher.py` & `edsnlp-0.8.1/tests/pipelines/core/test_matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_normalisation.py` & `edsnlp-0.8.1/tests/pipelines/core/test_normalisation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_sentences.py` & `edsnlp-0.8.1/tests/pipelines/core/test_sentences.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/core/test_terminology.py` & `edsnlp-0.8.1/tests/pipelines/core/test_terminology.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_consultation_date.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_consultation_date.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_dates.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_measurements.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_measurements.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_reason.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_reason.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_sections.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_sections.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/misc/test_tables.py` & `edsnlp-0.8.1/tests/pipelines/misc/test_tables.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/CKD.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/CKD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/COPD.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/COPD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/alcohol.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/alcohol.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/diabetes.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/diabetes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/peripheral_vascular_disease.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/peripheral_vascular_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/solid_tumor.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/solid_tumor.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/test_all.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/test_all.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/disorders/tobacco.py` & `edsnlp-0.8.1/tests/pipelines/ner/disorders/tobacco.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_adicap.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_adicap_decoder.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_adicap_decoder.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_cim10.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_cim10.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_drugs.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_drugs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_score.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_score.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_tnm.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_tnm.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/ner/test_umls.py` & `edsnlp-0.8.1/tests/pipelines/ner/test_umls.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/qualifiers/test_family.py` & `edsnlp-0.8.1/tests/pipelines/qualifiers/test_family.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/qualifiers/test_history.py` & `edsnlp-0.8.1/tests/pipelines/qualifiers/test_history.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/qualifiers/test_hypothesis.py` & `edsnlp-0.8.1/tests/pipelines/qualifiers/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/qualifiers/test_negation.py` & `edsnlp-0.8.1/tests/pipelines/qualifiers/test_negation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/qualifiers/test_reported_speech.py` & `edsnlp-0.8.1/tests/pipelines/qualifiers/test_reported_speech.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/trainable/test_nested_ner.py` & `edsnlp-0.8.1/tests/pipelines/trainable/test_nested_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/pipelines/trainable/test_span_classifier.py` & `edsnlp-0.8.1/tests/pipelines/trainable/test_span_classifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/processing/test_processing.py` & `edsnlp-0.8.1/tests/processing/test_processing.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/test_conjugator.py` & `edsnlp-0.8.1/tests/test_conjugator.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/test_language.py` & `edsnlp-0.8.1/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/utils/test_examples.py` & `edsnlp-0.8.1/tests/utils/test_examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/utils/test_filter.py` & `edsnlp-0.8.1/tests/utils/test_filter.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.8.0/tests/utils/test_quick_examples.py` & `edsnlp-0.8.1/tests/utils/test_quick_examples.py`

 * *Files identical despite different names*

