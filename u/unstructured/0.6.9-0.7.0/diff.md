# Comparing `tmp/unstructured-0.6.9.tar.gz` & `tmp/unstructured-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.9.tar", last modified: Wed May 24 22:34:42 2023, max compression
+gzip compressed data, was "unstructured-0.7.0.tar", last modified: Wed May 31 20:15:02 2023, max compression
```

## Comparing `unstructured-0.6.9.tar` & `unstructured-0.7.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-24 22:34:33.000000 unstructured-0.6.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 22:34:33.000000 unstructured-0.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-24 22:34:42.407830 unstructured-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-24 22:34:33.000000 unstructured-0.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 22:34:33.000000 unstructured-0.6.9/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 22:34:42.407830 unstructured-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-24 22:34:33.000000 unstructured-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-24 22:34:33.000000 unstructured-0.6.9/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.391830 unstructured-0.6.9/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.399830 unstructured-0.6.9/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.403830 unstructured-0.6.9/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.407830 unstructured-0.6.9/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-24 22:34:33.000000 unstructured-0.6.9/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:34:42.395830 unstructured-0.6.9/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 22:34:42.000000 unstructured-0.6.9/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.575583 unstructured-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-31 20:14:52.000000 unstructured-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 20:14:52.000000 unstructured-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-31 20:15:02.575583 unstructured-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-31 20:14:52.000000 unstructured-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-31 20:15:02.575583 unstructured-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-31 20:14:52.000000 unstructured-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.571583 unstructured-0.7.0/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.571583 unstructured-0.7.0/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.575583 unstructured-0.7.0/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.9/LICENSE.md` & `unstructured-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/PKG-INFO` & `unstructured-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.9
+Version: 0.7.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -32,26 +32,14 @@
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
-        <h2 align="center">
-          <p>Announcement!!!</p>
-        </h2>
-        <div align="center">
-          <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
-        
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
-        We'd love to hear your feedback, let us know how it goes in our <a
-          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
-           community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
-        <p><img src="easy.gif"></p></p>
-        </div>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -62,15 +50,18 @@
           elements.
         - :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
           sentence
           fragments.
         - :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
           and data labeling.
         
-        <br></br>
+        Unstructured also provides the capabilities from `unstructured` as an API.
+        Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
+        to get started making API calls.
+        You’ll also find instructions there about how to host your own version of the API.
         
         ## :eight_pointed_black_star: Quick Start
         
         Use the following instructions to get up and running with `unstructured` and test your
         installation. NOTE: We do not currently support python 3.11, please use an older version.
         
         - Install the Python SDK with `pip install "unstructured[local-inference]"`
@@ -91,22 +82,42 @@
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
-        And if you installed with `local-inference`, you should be able to run this as well:
+        The following table shows the document types the `unstructured` library currently supports.
+        `partition` will recognize each of these document types and route the document to the
+        appropriate partitioning function. If you already know your document type, you can use
+        the partitioning function listed in the table directly.
+        See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
+        about the library.
+        
+        | Document Type | Partition Function | Strategies | Table Support | Options |
+        | --- | --- | --- | --- | --- |
+        | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
+        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
+        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+        | EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+        | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
+        | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
+        | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+        | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+        | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
+        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+        | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+        | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
-        ```python
-        from unstructured.partition.auto import partition
         
-        elements = partition("example-docs/layout-parser-paper.pdf")
-        print("\n\n".join([str(el) for el in elements]))
-        ```
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
         NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
@@ -186,32 +197,29 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        
-        You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
-        and **PNG** documents with one line of code!
+        You can parse over a dozen document types with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
         The easiest way to parse a document in unstructured is to use the `partition` brick. If you
         use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
         file-specific partitioning brick.
         If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
         instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
         `partition` will always apply the default arguments. If you need
-        advanced features, use a document-specific brick. The `partition` brick currently works for
-        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+        advanced features, use a document-specific brick.
+        See the table above for a full list of document types supported in the library.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -244,145 +252,17 @@
         
         Introduction
         
         Deep Learning(DL)-based approaches are the state-of-the-art for a wide range of document image analysis (DIA) tasks
         including document image classiﬁcation [11,
         ```
         
-        ### HTML Parsing
-        
-        You can parse an HTML document using the following workflow:
-        
-        ```python
-        from unstructured.partition.html import partition_html
-        
-        elements = partition_html("example-docs/example-10k.html")
-        print("\n\n".join([str(el) for el in elements[:5]]))
-        ```
-        
-        The print statement will show the following text:
-        ```
-        UNITED STATES
-        
-        SECURITIES AND EXCHANGE COMMISSION
-        
-        Washington, D.C. 20549
-        
-        FORM 10-K
-        
-        ANNUAL REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-        ```
-        
-        And `elements` will be a list of elements in the HTML document, similar to the following:
-        
-        ```python
-        [<unstructured.documents.elements.Title at 0x169cbe820>,
-         <unstructured.documents.elements.NarrativeText at 0x169cbe8e0>,
-         <unstructured.documents.elements.NarrativeText at 0x169cbe3a0>]
-        ```
-        
-        ### PDF Parsing
-        
-        You can use the following workflow to parse PDF documents.
-        
-        ```python
-        from unstructured.partition.pdf import partition_pdf
-        
-        elements = partition_pdf("example-docs/layout-parser-paper.pdf")
-        ```
-        
-        The output will look the same as the example from the document parsing section above.
-        
-        
-        ### E-mail Parsing
-        
-        The `partition_email` function within `unstructured` is helpful for parsing `.eml` files. Common
-        e-mail clients such as Microsoft Outlook and Gmail support exporting e-mails as `.eml` files.
-        `partition_email` accepts filenames, file-like object, and raw text as input. The following
-        three snippets for parsing `.eml` files are equivalent:
-        
-        ```python
-        from unstructured.partition.email import partition_email
-        
-        elements = partition_email(filename="example-docs/fake-email.eml")
-        
-        with open("example-docs/fake-email.eml", "r") as f:
-          elements = partition_email(file=f)
-        
-        with open("example-docs/fake-email.eml", "r") as f:
-          text = f.read()
-        elements = partition_email(text=text)
-        ```
-        
-        The `elements` output will look like the following:
-        
-        ```python
-        [<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-        <unstructured.documents.html.HTMLTitle at 0x106877970>,
-        <unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-        <unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-        ```
-        
-        Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-        output, which looks like:
-        
-        ```python
-        This is a test email to use for unit tests.
-        
-        Important points:
-        
-        Roses are red
-        
-        Violets are blue
-        ```
-        
-        ### Text Document Parsing
-        
-        The `partition_text` function within `unstructured` can be used to parse simple
-        text files into elements.
-        
-        `partition_text` accepts filenames, file-like object, and raw text as input. The following three snippets are for parsing text files:
-        
-        ```python
-        from unstructured.partition.text import partition_text
-        
-        elements = partition_text(filename="example-docs/fake-text.txt")
-        
-        with open("example-docs/fake-text.txt", "r") as f:
-          elements = partition_text(file=f)
-        
-        with open("example-docs/fake-text.txt", "r") as f:
-          text = f.read()
-        elements = partition_text(text=text)
-        ```
-        
-        The `elements` output will look like the following:
-        
-        ```python
-        [<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-        <unstructured.documents.html.HTMLTitle at 0x106877970>,
-        <unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-        <unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-        ```
-        
-        Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-        output, which looks like:
-        
-        ```python
-        This is a test document to use for unit tests.
-        
-        Important points:
-        
-        Hamburgers are delicious
-        
-        Dogs are the best
-        
-        I love fuzzy blankets
-        ```
-        
+        See the [partitioning](https://unstructured-io.github.io/unstructured/bricks.html#partitioning)
+        section in our documentation for a full list of options and instructions on how to use
+        file-specific partitioning functions.
         
         ## :guardsman: Security Policy
         
         See our [security policy](https://github.com/Unstructured-IO/unstructured/security/policy) for
         information on how to report security vulnerabilities.
         
         ## :books: Learn more
@@ -400,14 +280,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -15,90 +15,107 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
-                          ***** Announcement!!! *****
-We're excited to announce the public release of the unstructured.io hosted API!
- Now you can leverage Unstructured with a simple API call to render clean text
-     in JSON format out of your images, documents, powerpoints, and more.
- Checkout the readme here to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. Unstructured
-data just got easier! We'd love to hear your feedback, let us know how it goes
-  in our community_slack. And stay tuned for improvements to both quality and
-                      performance over the coming months!
-                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
 broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
 boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
 that format data for downstream tasks, such as ML inference and data labeling.
-## :eight_pointed_black_star: Quick Start Use the following instructions to get
-up and running with `unstructured` and test your installation. NOTE: We do not
+Unstructured also provides the capabilities from `unstructured` as an API.
+Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
+unstructured-api) to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. ## :
+eight_pointed_black_star: Quick Start Use the following instructions to get up
+and running with `unstructured` and test your installation. NOTE: We do not
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
 facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
 should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` And if you installed with `local-inference`, you should be able
-to run this as well: ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") print
-("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
-using the docker image The following instructions are intended to help you get
-up and running using Docker to interact with `unstructured`. See [here](https:/
-/docs.docker.com/get-docker/) if you don't already have docker installed on
-your machine. NOTE: we build multi-platform images to support both x86_64 and
-Apple silicon hardware. `docker pull` should download the corresponding image
-for your architecture, but you can specify with `--platform` (e.g. `--platform
-linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
-tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
-the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
-with `latest`. To leverage this, `docker pull` from our image repository.
-```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
-pulled, you can create a container from this image and shell to it. ```bash #
-create the container docker run -dt --name unstructured quay.io/unstructured-
-io/unstructured:latest # this will drop you into a bash shell where the Docker
-image is running docker exec -it unstructured bash ``` You can also build your
-own Docker image. If you only plan on parsing one type of data you can speed up
-building the image by commenting out some of the packages/requirements
-necessary for other data types. See Dockerfile to know which lines are
-necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+elements])) ``` The following table shows the document types the `unstructured`
+library currently supports. `partition` will recognize each of these document
+types and route the document to the appropriate partitioning function. If you
+already know your document type, you can use the partitioning function listed
+in the table directly. See our [documentation page](https://unstructured-
+io.github.io/unstructured/) for more details about the library. | Document Type
+| Partition Function | Strategies | Table Support | Options | | --- | --- | --
+- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
+E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
+`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
+N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
+| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
+`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
+Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
+Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
+(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
+Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
+Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
+:dizzy: Instructions for using the docker image The following instructions are
+intended to help you get up and running using Docker to interact with
+`unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
+already have docker installed on your machine. NOTE: we build multi-platform
+images to support both x86_64 and Apple silicon hardware. `docker pull` should
+download the corresponding image for your architecture, but you can specify
+with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
+images for all pushes to `main`. We tag each image with the corresponding short
+commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`).
+We also tag the most recent image with `latest`. To leverage this, `docker
+pull` from our image repository. ```bash docker pull quay.io/unstructured-io/
+unstructured:latest ``` Once pulled, you can create a container from this image
+and shell to it. ```bash # create the container docker run -dt --name
+unstructured quay.io/unstructured-io/unstructured:latest # this will drop you
+into a bash shell where the Docker image is running docker exec -it
+unstructured bash ``` You can also build your own Docker image. If you only
+plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
@@ -110,33 +127,30 @@
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
-documents with one line of code!
+show how to get started with the `unstructured` library. You can parse over a
+dozen document types with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
-document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
-`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
-import partition elements = partition("example-docs/layout-parser-paper.pdf")
-``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+document-specific brick. See the table above for a full list of document types
+supported in the library. ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
+`print("\n\n".join([str(el) for el in elements]))` to get a string
 representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
 Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
 0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
 Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
 analysis (DIA) have been primarily driven by the application of neural
 networks. Ideally, research outcomes could be easily deployed in production and
 extended for further investigation. However, various factors like loosely
@@ -156,75 +170,30 @@
 both pre-trained models and full document digiti- zation pipelines. We
 demonstrate that LayoutParser is helpful for both lightweight and large-scale
 digitization pipelines in real-word use cases. The library is publicly
 available at https://layout-parser.github.io Keywords: Document Image Analysis
 Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
 library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
 state-of-the-art for a wide range of document image analysis (DIA) tasks
-including document image classiï¬cation [11, ``` ### HTML Parsing You can
-parse an HTML document using the following workflow: ```python from
-unstructured.partition.html import partition_html elements = partition_html
-("example-docs/example-10k.html") print("\n\n".join([str(el) for el in elements
-[:5]])) ``` The print statement will show the following text: ``` UNITED STATES
-SECURITIES AND EXCHANGE COMMISSION Washington, D.C. 20549 FORM 10-K ANNUAL
-REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-``` And `elements` will be a list of elements in the HTML document, similar to
-the following: ```python [
-documents.elements.Title at 0x169cbe820>,
-documents.elements.NarrativeText at 0x169cbe8e0>,
-documents.elements.NarrativeText at 0x169cbe3a0>] ``` ### PDF Parsing You can
-use the following workflow to parse PDF documents. ```python from
-unstructured.partition.pdf import partition_pdf elements = partition_pdf
-("example-docs/layout-parser-paper.pdf") ``` The output will look the same as
-the example from the document parsing section above. ### E-mail Parsing The
-`partition_email` function within `unstructured` is helpful for parsing `.eml`
-files. Common e-mail clients such as Microsoft Outlook and Gmail support
-exporting e-mails as `.eml` files. `partition_email` accepts filenames, file-
-like object, and raw text as input. The following three snippets for parsing
-`.eml` files are equivalent: ```python from unstructured.partition.email import
-partition_email elements = partition_email(filename="example-docs/fake-
-email.eml") with open("example-docs/fake-email.eml", "r") as f: elements =
-partition_email(file=f) with open("example-docs/fake-email.eml", "r") as f:
-text = f.read() elements = partition_email(text=text) ``` The `elements` output
-will look like the following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test email to use for unit tests. Important
-points: Roses are red Violets are blue ``` ### Text Document Parsing The
-`partition_text` function within `unstructured` can be used to parse simple
-text files into elements. `partition_text` accepts filenames, file-like object,
-and raw text as input. The following three snippets are for parsing text files:
-```python from unstructured.partition.text import partition_text elements =
-partition_text(filename="example-docs/fake-text.txt") with open("example-docs/
-fake-text.txt", "r") as f: elements = partition_text(file=f) with open
-("example-docs/fake-text.txt", "r") as f: text = f.read() elements =
-partition_text(text=text) ``` The `elements` output will look like the
-following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test document to use for unit tests. Important
-points: Hamburgers are delicious Dogs are the best I love fuzzy blankets ``` ##
-:guardsman: Security Policy See our [security policy](https://github.com/
-Unstructured-IO/unstructured/security/policy) for information on how to report
-security vulnerabilities. ## :books: Learn more | Section | Description | |-|-
-| | [Company Website](https://unstructured.io) | Unstructured.io product and
-company info | | [Documentation](https://unstructured-io.github.io/
-unstructured) | Full API documentation | | [Batch Processing](Ingest.md) |
-Ingesting batches of documents through Unstructured | Keywords: NLP PDF HTML CV
-XML parsing preprocessing Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
-text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
-slack Provides-Extra: wikipedia Provides-Extra: google-drive
+including document image classiï¬cation [11, ``` See the [partitioning](https:
+//unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
+our documentation for a full list of options and instructions on how to use
+file-specific partitioning functions. ## :guardsman: Security Policy See our
+[security policy](https://github.com/Unstructured-IO/unstructured/security/
+policy) for information on how to report security vulnerabilities. ## :books:
+Learn more | Section | Description | |-|-| | [Company Website](https://
+unstructured.io) | Unstructured.io product and company info | | [Documentation]
+(https://unstructured-io.github.io/unstructured) | Full API documentation | |
+[Batch Processing](Ingest.md) | Ingesting batches of documents through
+Unstructured | Keywords: NLP PDF HTML CV XML parsing preprocessing Platform:
+UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
+Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
+discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
+Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
```

### Comparing `unstructured-0.6.9/README.md` & `unstructured-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,14 @@
   href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
     <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
   </a>
   <a href="https://www.linkedin.com/company/unstructuredio/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </div>
-<h2 align="center">
-  <p>Announcement!!!</p>
-</h2>
-<div align="center">
-  <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
-
-<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
-We'd love to hear your feedback, let us know how it goes in our <a
-  href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
-   community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
-<p><img src="easy.gif"></p></p>
-</div>
 
 <h3 align="center">
   <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
 </h3>
 
 The `unstructured` library provides open-source components for pre-processing text documents
 such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -54,15 +42,18 @@
   elements.
 - :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
   sentence
   fragments.
 - :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
   and data labeling.
 
-<br></br>
+Unstructured also provides the capabilities from `unstructured` as an API.
+Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
+to get started making API calls.
+You’ll also find instructions there about how to host your own version of the API.
 
 ## :eight_pointed_black_star: Quick Start
 
 Use the following instructions to get up and running with `unstructured` and test your
 installation. NOTE: We do not currently support python 3.11, please use an older version.
 
 - Install the Python SDK with `pip install "unstructured[local-inference]"`
@@ -83,22 +74,42 @@
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition(filename="example-docs/fake-email.eml")
 print("\n\n".join([str(el) for el in elements]))
 ```
 
-And if you installed with `local-inference`, you should be able to run this as well:
+The following table shows the document types the `unstructured` library currently supports.
+`partition` will recognize each of these document types and route the document to the
+appropriate partitioning function. If you already know your document type, you can use
+the partitioning function listed in the table directly.
+See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
+about the library.
+
+| Document Type | Partition Function | Strategies | Table Support | Options |
+| --- | --- | --- | --- | --- |
+| CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
+| E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
+| E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+| EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+| Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
+| HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
+| Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+| Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+| Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
+| PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+| Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+| Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+| Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+| Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+| Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+| XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
 
-```python
-from unstructured.partition.auto import partition
 
-elements = partition("example-docs/layout-parser-paper.pdf")
-print("\n\n".join([str(el) for el in elements]))
-```
 
 ## :dizzy: Instructions for using the docker image
 
 The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
 See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
 
 NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
@@ -178,32 +189,29 @@
 you can also uninstall the hooks with `pre-commit uninstall`.
 
 ## :clap: Quick Tour
 
 You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
 
 The following examples show how to get started with the `unstructured` library.
-
-You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
-and **PNG** documents with one line of code!
+You can parse over a dozen document types with one line of code!
 <br></br>
 See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
 of the features in the library.
 
 ### Document Parsing
 
 The easiest way to parse a document in unstructured is to use the `partition` brick. If you
 use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
 file-specific partitioning brick.
 If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
 instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
 `partition` will always apply the default arguments. If you need
-advanced features, use a document-specific brick. The `partition` brick currently works for
-`.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+advanced features, use a document-specific brick.
+See the table above for a full list of document types supported in the library.
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition("example-docs/layout-parser-paper.pdf")
 ```
 
@@ -236,145 +244,17 @@
 
 Introduction
 
 Deep Learning(DL)-based approaches are the state-of-the-art for a wide range of document image analysis (DIA) tasks
 including document image classiﬁcation [11,
 ```
 
-### HTML Parsing
-
-You can parse an HTML document using the following workflow:
-
-```python
-from unstructured.partition.html import partition_html
-
-elements = partition_html("example-docs/example-10k.html")
-print("\n\n".join([str(el) for el in elements[:5]]))
-```
-
-The print statement will show the following text:
-```
-UNITED STATES
-
-SECURITIES AND EXCHANGE COMMISSION
-
-Washington, D.C. 20549
-
-FORM 10-K
-
-ANNUAL REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-```
-
-And `elements` will be a list of elements in the HTML document, similar to the following:
-
-```python
-[<unstructured.documents.elements.Title at 0x169cbe820>,
- <unstructured.documents.elements.NarrativeText at 0x169cbe8e0>,
- <unstructured.documents.elements.NarrativeText at 0x169cbe3a0>]
-```
-
-### PDF Parsing
-
-You can use the following workflow to parse PDF documents.
-
-```python
-from unstructured.partition.pdf import partition_pdf
-
-elements = partition_pdf("example-docs/layout-parser-paper.pdf")
-```
-
-The output will look the same as the example from the document parsing section above.
-
-
-### E-mail Parsing
-
-The `partition_email` function within `unstructured` is helpful for parsing `.eml` files. Common
-e-mail clients such as Microsoft Outlook and Gmail support exporting e-mails as `.eml` files.
-`partition_email` accepts filenames, file-like object, and raw text as input. The following
-three snippets for parsing `.eml` files are equivalent:
-
-```python
-from unstructured.partition.email import partition_email
-
-elements = partition_email(filename="example-docs/fake-email.eml")
-
-with open("example-docs/fake-email.eml", "r") as f:
-  elements = partition_email(file=f)
-
-with open("example-docs/fake-email.eml", "r") as f:
-  text = f.read()
-elements = partition_email(text=text)
-```
-
-The `elements` output will look like the following:
-
-```python
-[<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-<unstructured.documents.html.HTMLTitle at 0x106877970>,
-<unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-<unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-```
-
-Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-output, which looks like:
-
-```python
-This is a test email to use for unit tests.
-
-Important points:
-
-Roses are red
-
-Violets are blue
-```
-
-### Text Document Parsing
-
-The `partition_text` function within `unstructured` can be used to parse simple
-text files into elements.
-
-`partition_text` accepts filenames, file-like object, and raw text as input. The following three snippets are for parsing text files:
-
-```python
-from unstructured.partition.text import partition_text
-
-elements = partition_text(filename="example-docs/fake-text.txt")
-
-with open("example-docs/fake-text.txt", "r") as f:
-  elements = partition_text(file=f)
-
-with open("example-docs/fake-text.txt", "r") as f:
-  text = f.read()
-elements = partition_text(text=text)
-```
-
-The `elements` output will look like the following:
-
-```python
-[<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-<unstructured.documents.html.HTMLTitle at 0x106877970>,
-<unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-<unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-```
-
-Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-output, which looks like:
-
-```python
-This is a test document to use for unit tests.
-
-Important points:
-
-Hamburgers are delicious
-
-Dogs are the best
-
-I love fuzzy blankets
-```
-
+See the [partitioning](https://unstructured-io.github.io/unstructured/bricks.html#partitioning)
+section in our documentation for a full list of options and instructions on how to use
+file-specific partitioning functions.
 
 ## :guardsman: Security Policy
 
 See our [security policy](https://github.com/Unstructured-IO/unstructured/security/policy) for
 information on how to report security vulnerabilities.
 
 ## :books: Learn more
```

#### html2text {}

```diff
@@ -11,90 +11,107 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
-                          ***** Announcement!!! *****
-We're excited to announce the public release of the unstructured.io hosted API!
- Now you can leverage Unstructured with a simple API call to render clean text
-     in JSON format out of your images, documents, powerpoints, and more.
- Checkout the readme here to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. Unstructured
-data just got easier! We'd love to hear your feedback, let us know how it goes
-  in our community_slack. And stay tuned for improvements to both quality and
-                      performance over the coming months!
-                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
 broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
 boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
 that format data for downstream tasks, such as ML inference and data labeling.
-## :eight_pointed_black_star: Quick Start Use the following instructions to get
-up and running with `unstructured` and test your installation. NOTE: We do not
+Unstructured also provides the capabilities from `unstructured` as an API.
+Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
+unstructured-api) to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. ## :
+eight_pointed_black_star: Quick Start Use the following instructions to get up
+and running with `unstructured` and test your installation. NOTE: We do not
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
 facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
 should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` And if you installed with `local-inference`, you should be able
-to run this as well: ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") print
-("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
-using the docker image The following instructions are intended to help you get
-up and running using Docker to interact with `unstructured`. See [here](https:/
-/docs.docker.com/get-docker/) if you don't already have docker installed on
-your machine. NOTE: we build multi-platform images to support both x86_64 and
-Apple silicon hardware. `docker pull` should download the corresponding image
-for your architecture, but you can specify with `--platform` (e.g. `--platform
-linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
-tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
-the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
-with `latest`. To leverage this, `docker pull` from our image repository.
-```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
-pulled, you can create a container from this image and shell to it. ```bash #
-create the container docker run -dt --name unstructured quay.io/unstructured-
-io/unstructured:latest # this will drop you into a bash shell where the Docker
-image is running docker exec -it unstructured bash ``` You can also build your
-own Docker image. If you only plan on parsing one type of data you can speed up
-building the image by commenting out some of the packages/requirements
-necessary for other data types. See Dockerfile to know which lines are
-necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+elements])) ``` The following table shows the document types the `unstructured`
+library currently supports. `partition` will recognize each of these document
+types and route the document to the appropriate partitioning function. If you
+already know your document type, you can use the partitioning function listed
+in the table directly. See our [documentation page](https://unstructured-
+io.github.io/unstructured/) for more details about the library. | Document Type
+| Partition Function | Strategies | Table Support | Options | | --- | --- | --
+- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
+E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
+`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
+N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
+| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
+`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
+Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
+Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
+(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
+Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
+Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
+:dizzy: Instructions for using the docker image The following instructions are
+intended to help you get up and running using Docker to interact with
+`unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
+already have docker installed on your machine. NOTE: we build multi-platform
+images to support both x86_64 and Apple silicon hardware. `docker pull` should
+download the corresponding image for your architecture, but you can specify
+with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
+images for all pushes to `main`. We tag each image with the corresponding short
+commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`).
+We also tag the most recent image with `latest`. To leverage this, `docker
+pull` from our image repository. ```bash docker pull quay.io/unstructured-io/
+unstructured:latest ``` Once pulled, you can create a container from this image
+and shell to it. ```bash # create the container docker run -dt --name
+unstructured quay.io/unstructured-io/unstructured:latest # this will drop you
+into a bash shell where the Docker image is running docker exec -it
+unstructured bash ``` You can also build your own Docker image. If you only
+plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
@@ -106,33 +123,30 @@
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
-documents with one line of code!
+show how to get started with the `unstructured` library. You can parse over a
+dozen document types with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
-document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
-`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
-import partition elements = partition("example-docs/layout-parser-paper.pdf")
-``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+document-specific brick. See the table above for a full list of document types
+supported in the library. ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
+`print("\n\n".join([str(el) for el in elements]))` to get a string
 representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
 Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
 0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
 Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
 analysis (DIA) have been primarily driven by the application of neural
 networks. Ideally, research outcomes could be easily deployed in production and
 extended for further investigation. However, various factors like loosely
@@ -152,63 +166,18 @@
 both pre-trained models and full document digiti- zation pipelines. We
 demonstrate that LayoutParser is helpful for both lightweight and large-scale
 digitization pipelines in real-word use cases. The library is publicly
 available at https://layout-parser.github.io Keywords: Document Image Analysis
 Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
 library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
 state-of-the-art for a wide range of document image analysis (DIA) tasks
-including document image classiï¬cation [11, ``` ### HTML Parsing You can
-parse an HTML document using the following workflow: ```python from
-unstructured.partition.html import partition_html elements = partition_html
-("example-docs/example-10k.html") print("\n\n".join([str(el) for el in elements
-[:5]])) ``` The print statement will show the following text: ``` UNITED STATES
-SECURITIES AND EXCHANGE COMMISSION Washington, D.C. 20549 FORM 10-K ANNUAL
-REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-``` And `elements` will be a list of elements in the HTML document, similar to
-the following: ```python [
-documents.elements.Title at 0x169cbe820>,
-documents.elements.NarrativeText at 0x169cbe8e0>,
-documents.elements.NarrativeText at 0x169cbe3a0>] ``` ### PDF Parsing You can
-use the following workflow to parse PDF documents. ```python from
-unstructured.partition.pdf import partition_pdf elements = partition_pdf
-("example-docs/layout-parser-paper.pdf") ``` The output will look the same as
-the example from the document parsing section above. ### E-mail Parsing The
-`partition_email` function within `unstructured` is helpful for parsing `.eml`
-files. Common e-mail clients such as Microsoft Outlook and Gmail support
-exporting e-mails as `.eml` files. `partition_email` accepts filenames, file-
-like object, and raw text as input. The following three snippets for parsing
-`.eml` files are equivalent: ```python from unstructured.partition.email import
-partition_email elements = partition_email(filename="example-docs/fake-
-email.eml") with open("example-docs/fake-email.eml", "r") as f: elements =
-partition_email(file=f) with open("example-docs/fake-email.eml", "r") as f:
-text = f.read() elements = partition_email(text=text) ``` The `elements` output
-will look like the following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test email to use for unit tests. Important
-points: Roses are red Violets are blue ``` ### Text Document Parsing The
-`partition_text` function within `unstructured` can be used to parse simple
-text files into elements. `partition_text` accepts filenames, file-like object,
-and raw text as input. The following three snippets are for parsing text files:
-```python from unstructured.partition.text import partition_text elements =
-partition_text(filename="example-docs/fake-text.txt") with open("example-docs/
-fake-text.txt", "r") as f: elements = partition_text(file=f) with open
-("example-docs/fake-text.txt", "r") as f: text = f.read() elements =
-partition_text(text=text) ``` The `elements` output will look like the
-following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test document to use for unit tests. Important
-points: Hamburgers are delicious Dogs are the best I love fuzzy blankets ``` ##
-:guardsman: Security Policy See our [security policy](https://github.com/
-Unstructured-IO/unstructured/security/policy) for information on how to report
-security vulnerabilities. ## :books: Learn more | Section | Description | |-|-
-| | [Company Website](https://unstructured.io) | Unstructured.io product and
-company info | | [Documentation](https://unstructured-io.github.io/
-unstructured) | Full API documentation | | [Batch Processing](Ingest.md) |
-Ingesting batches of documents through Unstructured |
+including document image classiï¬cation [11, ``` See the [partitioning](https:
+//unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
+our documentation for a full list of options and instructions on how to use
+file-specific partitioning functions. ## :guardsman: Security Policy See our
+[security policy](https://github.com/Unstructured-IO/unstructured/security/
+policy) for information on how to report security vulnerabilities. ## :books:
+Learn more | Section | Description | |-|-| | [Company Website](https://
+unstructured.io) | Unstructured.io product and company info | | [Documentation]
+(https://unstructured-io.github.io/unstructured) | Full API documentation | |
+[Batch Processing](Ingest.md) | Ingesting batches of documents through
+Unstructured |
```

### Comparing `unstructured-0.6.9/setup.py` & `unstructured-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     author="Unstructured Technologies",
     author_email="devops@unstructuredai.io",
     license="Apache-2.0",
     packages=find_packages(),
     version=__version__,
```

### Comparing `unstructured-0.6.9/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.0/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.0/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/test_unstructured/test_utils.py` & `unstructured-0.7.0/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/cleaners/core.py` & `unstructured-0.7.0/unstructured/cleaners/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 def replace_mime_encodings(text: str, encoding: str = "utf-8") -> str:
     """Replaces MIME encodings with their equivalent characters in the specified encoding.
 
     Example
     -------
     5 w=E2=80-99s -> 5 w’s
     """
-    return quopri.decodestring(text.encode()).decode(encoding)
+    return quopri.decodestring(text.encode(encoding)).decode(encoding)
 
 
 def clean_prefix(text: str, pattern: str, ignore_case: bool = False, strip: bool = True) -> str:
     """Removes prefixes from a string according to the specified pattern. Strips leading
     whitespace if the strip parameter is set to True.
 
     Input
```

### Comparing `unstructured-0.6.9/unstructured/cleaners/extract.py` & `unstructured-0.7.0/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/cleaners/translate.py` & `unstructured-0.7.0/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/documents/base.py` & `unstructured-0.7.0/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/documents/elements.py` & `unstructured-0.7.0/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/documents/email_elements.py` & `unstructured-0.7.0/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/documents/html.py` & `unstructured-0.7.0/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/documents/xml.py` & `unstructured-0.7.0/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/file_utils/encoding.py` & `unstructured-0.7.0/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/file_utils/exploration.py` & `unstructured-0.7.0/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.0/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/file_utils/filetype.py` & `unstructured-0.7.0/unstructured/file_utils/filetype.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import zipfile
 from enum import Enum
 from functools import wraps
 from typing import IO, Callable, List, Optional
 
 from unstructured.documents.elements import Element, PageBreak
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
-from unstructured.partition.common import _add_element_metadata, exactly_one
+from unstructured.partition.common import (
+    _add_element_metadata,
+    _remove_element_metadata,
+    exactly_one,
+)
 
 try:
     import magic
 
     LIBMAGIC_AVAILABLE = True
 except ImportError:  # pragma: nocover
     LIBMAGIC_AVAILABLE = False  # pragma: nocover
@@ -133,14 +137,15 @@
 EXT_TO_FILETYPE = {
     ".pdf": FileType.PDF,
     ".docx": FileType.DOCX,
     ".jpg": FileType.JPG,
     ".jpeg": FileType.JPG,
     ".txt": FileType.TXT,
     ".text": FileType.TXT,
+    ".log": FileType.TXT,
     ".eml": FileType.EML,
     ".xml": FileType.XML,
     ".htm": FileType.HTML,
     ".html": FileType.HTML,
     ".md": FileType.MD,
     ".xlsx": FileType.XLSX,
     ".pptx": FileType.PPTX,
@@ -204,14 +209,18 @@
 
     # NOTE(crag): for older versions of the OS libmagic package, such as is currently
     # installed on the Unstructured docker image, .json files resolve to "text/plain"
     # rather than "application/json". this corrects for that case.
     if mime_type == "text/plain" and extension == ".json":
         return FileType.JSON
 
+    # NOTE(Crag): older magic lib does not differentiate between xls and doc
+    if mime_type == "application/msword" and extension == ".xls":
+        return FileType.XLS
+
     elif mime_type.endswith("xml"):
         if extension and (extension == ".html" or extension == ".htm"):
             return FileType.HTML
         else:
             return FileType.XML
 
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
@@ -371,12 +380,14 @@
                 }
                 return _add_element_metadata(
                     elements,
                     filetype=FILETYPE_TO_MIMETYPE[filetype],
                     **metadata_kwargs,  # type: ignore
                 )
             else:
-                return elements
+                return _remove_element_metadata(
+                    elements,
+                )
 
         return wrapper
 
     return decorator
```

### Comparing `unstructured-0.6.9/unstructured/file_utils/metadata.py` & `unstructured-0.7.0/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/azure.py` & `unstructured-0.7.0/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.0/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/discord.py` & `unstructured-0.7.0/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.0/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/git.py` & `unstructured-0.7.0/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/github.py` & `unstructured-0.7.0/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.0/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.0/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/local.py` & `unstructured-0.7.0/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.0/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/s3.py` & `unstructured-0.7.0/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/slack.py` & `unstructured-0.7.0/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.0/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.0/unstructured/ingest/doc_processor/generalized.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Process aribritrary files with the Unstructured library"""
 
 from typing import Any, Dict, List, Optional
 
-from unstructured_inference.models.detectron2 import MODEL_TYPES
+from unstructured_inference.models.base import get_model
 
 from unstructured.ingest.interfaces import BaseIngestDoc as IngestDoc
 from unstructured.ingest.logger import logger
 
 
 def initialize():
-    """Download models (avoids subprocesses all doing the same)"""
-    # Accessing this dictionary triggers standard model downloads for pdf processing.
-    # There will be a better way to do this, see
-    # https://github.com/Unstructured-IO/unstructured-inference/issues/55
-    MODEL_TYPES[None]["model_path"]
-    MODEL_TYPES[None]["config_path"]
+    """Download default model (avoids subprocesses all doing the same)"""
+
+    get_model()
 
 
 def process_document(doc: "IngestDoc", **partition_kwargs) -> Optional[List[Dict[str, Any]]]:
     """Process any IngestDoc-like class of document with choosen Unstructured's partition logic.
 
     Parameters
     ----------
```

### Comparing `unstructured-0.6.9/unstructured/ingest/interfaces.py` & `unstructured-0.7.0/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/ingest/main.py` & `unstructured-0.7.0/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/nlp/english-words.txt` & `unstructured-0.7.0/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/nlp/english_words.py` & `unstructured-0.7.0/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/nlp/patterns.py` & `unstructured-0.7.0/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/nlp/tokenize.py` & `unstructured-0.7.0/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/__init__.py` & `unstructured-0.7.0/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/api.py` & `unstructured-0.7.0/unstructured/partition/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,21 @@
             response = requests.post(
                 api_url,
                 headers=headers,
                 data=data,
                 files=files,  # type: ignore
             )
     elif file is not None:
-        _filename = file_filename or ""
+        if file_filename is None:
+            raise ValueError(
+                "If file is specified in partition_via_api, "
+                "file_filename must be specified as well.",
+            )
         files = [
-            ("files", (_filename, file, content_type)),  # type: ignore
+            ("files", (file_filename, file, content_type)),  # type: ignore
         ]
         response = requests.post(api_url, headers=headers, data=data, files=files)  # type: ignore
 
     if response.status_code == 200:
         return partition_json(text=response.text)
     else:
         raise ValueError(
```

### Comparing `unstructured-0.6.9/unstructured/partition/auto.py` & `unstructured-0.7.0/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         elements = partition_pptx(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
         )
     elif filetype == FileType.JSON:
         elements = partition_json(filename=filename, file=file)
-    elif filetype == FileType.XLSX:
+    elif (filetype == FileType.XLSX) or (filetype == FileType.XLS):
         elements = partition_xlsx(filename=filename, file=file)
     elif filetype == FileType.CSV:
         elements = partition_csv(filename=filename, file=file)
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
```

### Comparing `unstructured-0.6.9/unstructured/partition/common.py` & `unstructured-0.7.0/unstructured/partition/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import subprocess
 from io import BytesIO
 from tempfile import SpooledTemporaryFile
 from typing import BinaryIO, List, Optional, Tuple, Union
 
+from docx import table as docxtable
+from tabulate import tabulate
+
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
     ElementMetadata,
     ListItem,
     PageBreak,
@@ -80,14 +83,19 @@
     page_number: int = 1
     for layout_element in layout_elements:
         element = normalize_layout_element(layout_element)
         if hasattr(layout_element, "text_as_html"):
             text_as_html: Optional[str] = layout_element.text_as_html
         else:
             text_as_html = None
+        # NOTE(robinson) - defer to the page number that's already in the metadata
+        # if it's available
+        if hasattr(element, "metadata"):
+            page_number = element.metadata.page_number or page_number
+
         metadata = ElementMetadata(
             filename=filename,
             filetype=filetype,
             url=url,
             page_number=page_number,
             text_as_html=text_as_html,
         )
@@ -101,14 +109,34 @@
                 elements.append(element)
         else:
             element.metadata = metadata.merge(element.metadata)
             elements.append(element)
     return elements
 
 
+def _remove_element_metadata(
+    layout_elements,
+) -> List[Element]:
+    """Removes document metadata from the document element. Document metadata includes information
+    like the filename, source url, and page number."""
+    # Init an empty list of elements to write to
+    elements: List[Element] = []
+    metadata = ElementMetadata()
+    for layout_element in layout_elements:
+        element = normalize_layout_element(layout_element)
+        if isinstance(element, list):
+            for _element in element:
+                _element.metadata = metadata
+            elements.extend(element)
+        else:
+            element.metadata = metadata
+            elements.append(element)
+    return elements
+
+
 def convert_office_doc(input_filename: str, output_directory: str, target_format: str):
     """Converts a .doc file to a .docx file using the libreoffice CLI."""
     # NOTE(robinson) - In the future can also include win32com client as a fallback for windows
     # users who do not have LibreOffice installed
     # ref: https://stackoverflow.com/questions/38468442/
     #       multiple-doc-to-docx-file-conversion-using-python
     try:
@@ -156,7 +184,26 @@
     if isinstance(file_obj, SpooledTemporaryFile):
         file_obj.seek(0)
         contents = file_obj.read()
         return BytesIO(contents)
     else:
         # Return the original file object if it's not a SpooledTemporaryFile
         return file_obj
+
+
+def convert_ms_office_table_to_text(table: docxtable.Table, as_html: bool = True):
+    """
+    Convert a table object from a Word document to an HTML table string using the tabulate library.
+
+    Args:
+        table (Table): A Table object.
+        as_html (bool): Whether to return the table as an HTML string (True) or a
+            plain text string (False)
+
+    Returns:
+        str: An table string representation of the input table.
+    """
+    fmt = "html" if as_html else "plain"
+    rows = list(table.rows)
+    headers = [cell.text for cell in rows[0].cells]
+    data = [[cell.text for cell in row.cells] for row in rows[1:]]
+    return tabulate(data, headers=headers, tablefmt=fmt)
```

### Comparing `unstructured-0.6.9/unstructured/partition/csv.py` & `unstructured-0.7.0/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/doc.py` & `unstructured-0.7.0/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/docx.py` & `unstructured-0.7.0/unstructured/partition/docx.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import docx
 import pypandoc
 from docx.oxml.shared import qn
 from docx.text.paragraph import Paragraph
 from docx.text.run import Run
-from tabulate import tabulate
 
 from unstructured.cleaners.core import clean_bullets
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Table,
     Text,
     Title,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    convert_ms_office_table_to_text,
+    exactly_one,
+    spooled_to_bytes_io_if_needed,
+)
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
 
@@ -129,16 +132,16 @@
     metadata_filename = metadata_filename or filename
     elements: List[Element] = []
     table_index = 0
 
     for element_item in document.element.body:
         if element_item.tag.endswith("tbl"):
             table = document.tables[table_index]
-            html_table = _convert_table_to_text(table, as_html=True)
-            text_table = _convert_table_to_text(table, as_html=False)
+            html_table = convert_ms_office_table_to_text(table, as_html=True)
+            text_table = convert_ms_office_table_to_text(table, as_html=False)
             element = Table(text_table)
             if element is not None:
                 element.metadata = ElementMetadata(
                     text_as_html=html_table,
                     filename=metadata_filename,
                 )
                 elements.append(element)
@@ -149,32 +152,14 @@
             if para_element is not None:
                 para_element.metadata = ElementMetadata(filename=metadata_filename)
                 elements.append(para_element)
 
     return elements
 
 
-def _convert_table_to_text(table, as_html):
-    """
-    Convert a table object from a Word document to an HTML table string using the tabulate library.
-
-    Args:
-        table (Table): A Table object.
-        as_html (bool): Whether to return the table as an HTML string (True) or a
-            plain text string (False)
-
-    Returns:
-        str: An table string representation of the input table.
-    """
-    fmt = "html" if as_html else "plain"
-    headers = [cell.text for cell in table.rows[0].cells]
-    data = [[cell.text for cell in row.cells] for row in table.rows[1:]]
-    return tabulate(data, headers=headers, tablefmt=fmt)
-
-
 def _paragraph_to_element(paragraph: docx.text.paragraph.Paragraph) -> Optional[Text]:
     """Converts a docx Paragraph object into the appropriate unstructured document element.
     If the paragraph style is "Normal" or unknown, we try to predict the element type from the
     raw text."""
     text = paragraph.text
     style_name = paragraph.style and paragraph.style.name  # .style can be None
```

### Comparing `unstructured-0.6.9/unstructured/partition/email.py` & `unstructured-0.7.0/unstructured/partition/email.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import email
 import re
 import sys
 from email.message import Message
 from functools import partial
 from typing import IO, Dict, List, Optional, Tuple, Union
 
+from unstructured.file_utils.encoding import read_txt_file
 from unstructured.partition.common import exactly_one
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
     from typing import Final
 
@@ -201,40 +202,32 @@
         The string representation of the .eml document.
     content_source
         default: "text/html"
         other: "text/plain"
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     """
-    if not encoding:
-        encoding = "utf-8"
-
     if content_source not in VALID_CONTENT_SOURCES:
         raise ValueError(
             f"{content_source} is not a valid value for content_source. "
             f"Valid content sources are: {VALID_CONTENT_SOURCES}",
         )
 
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text)
 
     if filename is not None:
-        with open(filename) as f:
-            msg = email.message_from_file(f)
+        encoding, file_text = read_txt_file(filename=filename, encoding=encoding)
+        msg = email.message_from_string(file_text)
 
     elif file is not None:
-        file_content = file.read()
-        if isinstance(file_content, bytes):
-            file_text = file_content.decode(encoding)
-        else:
-            file_text = file_content
-
+        encoding, file_text = read_txt_file(file=file, encoding=encoding)
         msg = email.message_from_string(file_text)
 
     elif text is not None:
         _text: str = str(text)
         msg = email.message_from_string(_text)
 
     content_map: Dict[str, str] = {}
@@ -254,21 +247,27 @@
         # NOTE(robinson) - In the .eml files, the HTML content gets stored in a format that
         # looks like the following, resulting in extraneous "=" characters in the output if
         # you don't clean it up
         # <ul> =
         #    <li>Item 1</li>=
         #    <li>Item 2<li>=
         # </ul>
+        if not encoding:
+            encoding = "utf-8"
         list_content = content.split("=\n")
         content = "".join(list_content)
         elements = partition_html(text=content, include_metadata=False)
         for element in elements:
             if isinstance(element, Text):
                 _replace_mime_encodings = partial(replace_mime_encodings, encoding=encoding)
-                element.apply(_replace_mime_encodings)
+                try:
+                    element.apply(_replace_mime_encodings)
+                except UnicodeDecodeError:
+                    # If decoding fails, try decoding with default encoding (utf-8)
+                    element.apply(replace_mime_encodings)
     elif content_source == "text/plain":
         list_content = split_by_paragraph(content)
         elements = partition_text(text=content)
 
     for idx, element in enumerate(elements):
         indices = has_embedded_image(element)
         if (isinstance(element, (NarrativeText, Title))) and indices:
```

### Comparing `unstructured-0.6.9/unstructured/partition/epub.py` & `unstructured-0.7.0/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/html.py` & `unstructured-0.7.0/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/image.py` & `unstructured-0.7.0/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/json.py` & `unstructured-0.7.0/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/md.py` & `unstructured-0.7.0/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/msg.py` & `unstructured-0.7.0/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/odt.py` & `unstructured-0.7.0/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/pdf.py` & `unstructured-0.7.0/unstructured/partition/pdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -275,20 +275,20 @@
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
         height = page.height
 
         text_segments = []
         for obj in page:
-            # NOTE(robinson) - "Figure" is an example of an object type that does
-            # not have a get_text method
             x1, y2, x2, y1 = obj.bbox
             y1 = height - y1
             y2 = height - y2
 
+            # NOTE(robinson) - "Figure" is an example of an object type that does
+            # not have a get_text method
             if not hasattr(obj, "get_text"):
                 continue
             _text = obj.get_text()
             _text = re.sub(PARAGRAPH_PATTERN, " ", _text)
             _text = clean_extra_whitespace(_text)
             if _text.strip():
                 text_segments.append(_text)
```

### Comparing `unstructured-0.6.9/unstructured/partition/ppt.py` & `unstructured-0.7.0/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/pptx.py` & `unstructured-0.7.0/unstructured/partition/pptx.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     PageBreak,
+    Table,
     Text,
     Title,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    convert_ms_office_table_to_text,
+    exactly_one,
+    spooled_to_bytes_io_if_needed,
+)
 from unstructured.partition.text_type import (
     is_possible_narrative_text,
     is_possible_title,
 )
 
 OPENXML_SCHEMA_NAME = "{http://schemas.openxmlformats.org/drawingml/2006/main}"
 
@@ -59,18 +64,25 @@
     metadata_filename = metadata_filename or filename
     metadata = ElementMetadata(filename=metadata_filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
         metadata.page_number = i + 1
 
         for shape in _order_shapes(slide.shapes):
-            # NOTE(robinson) - we don't deal with tables yet, but so future humans can find
-            # it again, here are docs on how to deal with tables. The check for tables should
-            # be `if shape.has_table`
-            # ref: https://python-pptx.readthedocs.io/en/latest/user/table.html#adding-a-table
+            if shape.has_table:
+                table: pptx.table.Table = shape.table
+                html_table = convert_ms_office_table_to_text(table, as_html=True)
+                text_table = convert_ms_office_table_to_text(table, as_html=False)
+                if (text_table := text_table.strip()) != "":
+                    metadata = ElementMetadata(
+                        filename=metadata_filename,
+                        text_as_html=html_table,
+                    )
+                    elements.append(Table(text=text_table, metadata=metadata))
+                continue
             if not shape.has_text_frame:
                 continue
             # NOTE(robinson) - avoid processing shapes that are not on the actual slide
             if shape.top < 0 or shape.left < 0:
                 continue
             for paragraph in shape.text_frame.paragraphs:
                 text = paragraph.text
```

### Comparing `unstructured-0.6.9/unstructured/partition/rtf.py` & `unstructured-0.7.0/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/strategies.py` & `unstructured-0.7.0/unstructured/partition/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
 ):
     """Determines what strategy to use for processing PDFs or images, accounting for fallback
     logic if some dependencies are not available."""
     pytesseract_installed = dependency_exists("pytesseract")
-    detectron2_installed = dependency_exists("detectron2")
+    unstructured_inference_installed = dependency_exists("unstructured_inference")
 
     if is_image:
         validate_strategy(strategy, "image")
         pdf_text_extractable = False
     else:
         validate_strategy(strategy, "pdf")
         pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
@@ -88,33 +88,35 @@
                 pdf_text_extractable=pdf_text_extractable,
                 infer_table_structure=infer_table_structure,
             )
 
     if file is not None:
         file.seek(0)  # type: ignore
 
-    if all([not detectron2_installed, not pytesseract_installed, not pdf_text_extractable]):
+    if all(
+        [not unstructured_inference_installed, not pytesseract_installed, not pdf_text_extractable],
+    ):
         raise ValueError(
-            "detectron2 is not installed, pytesseract is not installed "
+            "unstructured_inference is not installed, pytesseract is not installed "
             "and the text of the PDF is not extractable. "
-            "To process this file, install detectron2, install pytesseract, "
+            "To process this file, install unstructured_inference, install pytesseract, "
             "or remove copy protection from the PDF.",
         )
 
     if strategy == "fast" and not pdf_text_extractable:
         logger.warning(
             "PDF text is not extractable. Cannot use the fast partitioning "
             "strategy. Falling back to partitioning with the ocr_only strategy.",
         )
         # NOTE(robinson) - fallback to ocr_only here because it is faster than hi_res
         return "ocr_only"
 
-    elif strategy == "hi_res" and not detectron2_installed:
+    elif strategy == "hi_res" and not unstructured_inference_installed:
         logger.warning(
-            "detectron2 is not installed. Cannot use the hi_res partitioning "
+            "unstructured_inference is not installed. Cannot use the hi_res partitioning "
             "strategy. Falling back to partitioning with another strategy.",
         )
         # NOTE(robinson) - fallback to ocr_only if possible because it is the most
         # similar to hi_res
         if pytesseract_installed:
             logger.warning("Falling back to partitioning with ocr_only.")
             return "ocr_only"
```

### Comparing `unstructured-0.6.9/unstructured/partition/text.py` & `unstructured-0.7.0/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/text_type.py` & `unstructured-0.7.0/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/xlsx.py` & `unstructured-0.7.0/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/partition/xml.py` & `unstructured-0.7.0/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/argilla.py` & `unstructured-0.7.0/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/base.py` & `unstructured-0.7.0/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/baseplate.py` & `unstructured-0.7.0/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/datasaur.py` & `unstructured-0.7.0/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/huggingface.py` & `unstructured-0.7.0/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/label_box.py` & `unstructured-0.7.0/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/label_studio.py` & `unstructured-0.7.0/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/staging/prodigy.py` & `unstructured-0.7.0/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured/utils.py` & `unstructured-0.7.0/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.9/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.0/unstructured.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.9
+Version: 0.7.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -32,26 +32,14 @@
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
-        <h2 align="center">
-          <p>Announcement!!!</p>
-        </h2>
-        <div align="center">
-          <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
-        
-        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier!
-        We'd love to hear your feedback, let us know how it goes in our <a
-          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
-           community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
-        <p><img src="easy.gif"></p></p>
-        </div>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -62,15 +50,18 @@
           elements.
         - :broom: ***Cleaning bricks*** that remove unwanted text from documents, such as boilerplate and
           sentence
           fragments.
         - :performing_arts: ***Staging bricks*** that format data for downstream tasks, such as ML inference
           and data labeling.
         
-        <br></br>
+        Unstructured also provides the capabilities from `unstructured` as an API.
+        Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/unstructured-api)
+        to get started making API calls.
+        You’ll also find instructions there about how to host your own version of the API.
         
         ## :eight_pointed_black_star: Quick Start
         
         Use the following instructions to get up and running with `unstructured` and test your
         installation. NOTE: We do not currently support python 3.11, please use an older version.
         
         - Install the Python SDK with `pip install "unstructured[local-inference]"`
@@ -91,22 +82,42 @@
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
-        And if you installed with `local-inference`, you should be able to run this as well:
+        The following table shows the document types the `unstructured` library currently supports.
+        `partition` will recognize each of these document types and route the document to the
+        appropriate partitioning function. If you already know your document type, you can use
+        the partitioning function listed in the table directly.
+        See our [documentation page](https://unstructured-io.github.io/unstructured/) for more details
+        about the library.
+        
+        | Document Type | Partition Function | Strategies | Table Support | Options |
+        | --- | --- | --- | --- | --- |
+        | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
+        | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
+        | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
+        | EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+        | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
+        | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
+        | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+        | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+        | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
+        | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
+        | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
+        | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+        | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+        | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
-        ```python
-        from unstructured.partition.auto import partition
         
-        elements = partition("example-docs/layout-parser-paper.pdf")
-        print("\n\n".join([str(el) for el in elements]))
-        ```
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
         NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
@@ -186,32 +197,29 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        
-        You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
-        and **PNG** documents with one line of code!
+        You can parse over a dozen document types with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
         The easiest way to parse a document in unstructured is to use the `partition` brick. If you
         use `partition` brick, `unstructured` will detect the file type and route it to the appropriate
         file-specific partitioning brick.
         If you are using the `partition` brick, you may need to install additional parameters via `pip install unstructured[local-inference]`. Ensure you first install `libmagic` using the
         instructions outlined [here](https://unstructured-io.github.io/unstructured/installing.html#filetype-detection)
         `partition` will always apply the default arguments. If you need
-        advanced features, use a document-specific brick. The `partition` brick currently works for
-        `.txt`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`, `.html`, and `.pdf` documents.
+        advanced features, use a document-specific brick.
+        See the table above for a full list of document types supported in the library.
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition("example-docs/layout-parser-paper.pdf")
         ```
         
@@ -244,145 +252,17 @@
         
         Introduction
         
         Deep Learning(DL)-based approaches are the state-of-the-art for a wide range of document image analysis (DIA) tasks
         including document image classiﬁcation [11,
         ```
         
-        ### HTML Parsing
-        
-        You can parse an HTML document using the following workflow:
-        
-        ```python
-        from unstructured.partition.html import partition_html
-        
-        elements = partition_html("example-docs/example-10k.html")
-        print("\n\n".join([str(el) for el in elements[:5]]))
-        ```
-        
-        The print statement will show the following text:
-        ```
-        UNITED STATES
-        
-        SECURITIES AND EXCHANGE COMMISSION
-        
-        Washington, D.C. 20549
-        
-        FORM 10-K
-        
-        ANNUAL REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-        ```
-        
-        And `elements` will be a list of elements in the HTML document, similar to the following:
-        
-        ```python
-        [<unstructured.documents.elements.Title at 0x169cbe820>,
-         <unstructured.documents.elements.NarrativeText at 0x169cbe8e0>,
-         <unstructured.documents.elements.NarrativeText at 0x169cbe3a0>]
-        ```
-        
-        ### PDF Parsing
-        
-        You can use the following workflow to parse PDF documents.
-        
-        ```python
-        from unstructured.partition.pdf import partition_pdf
-        
-        elements = partition_pdf("example-docs/layout-parser-paper.pdf")
-        ```
-        
-        The output will look the same as the example from the document parsing section above.
-        
-        
-        ### E-mail Parsing
-        
-        The `partition_email` function within `unstructured` is helpful for parsing `.eml` files. Common
-        e-mail clients such as Microsoft Outlook and Gmail support exporting e-mails as `.eml` files.
-        `partition_email` accepts filenames, file-like object, and raw text as input. The following
-        three snippets for parsing `.eml` files are equivalent:
-        
-        ```python
-        from unstructured.partition.email import partition_email
-        
-        elements = partition_email(filename="example-docs/fake-email.eml")
-        
-        with open("example-docs/fake-email.eml", "r") as f:
-          elements = partition_email(file=f)
-        
-        with open("example-docs/fake-email.eml", "r") as f:
-          text = f.read()
-        elements = partition_email(text=text)
-        ```
-        
-        The `elements` output will look like the following:
-        
-        ```python
-        [<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-        <unstructured.documents.html.HTMLTitle at 0x106877970>,
-        <unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-        <unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-        ```
-        
-        Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-        output, which looks like:
-        
-        ```python
-        This is a test email to use for unit tests.
-        
-        Important points:
-        
-        Roses are red
-        
-        Violets are blue
-        ```
-        
-        ### Text Document Parsing
-        
-        The `partition_text` function within `unstructured` can be used to parse simple
-        text files into elements.
-        
-        `partition_text` accepts filenames, file-like object, and raw text as input. The following three snippets are for parsing text files:
-        
-        ```python
-        from unstructured.partition.text import partition_text
-        
-        elements = partition_text(filename="example-docs/fake-text.txt")
-        
-        with open("example-docs/fake-text.txt", "r") as f:
-          elements = partition_text(file=f)
-        
-        with open("example-docs/fake-text.txt", "r") as f:
-          text = f.read()
-        elements = partition_text(text=text)
-        ```
-        
-        The `elements` output will look like the following:
-        
-        ```python
-        [<unstructured.documents.html.HTMLNarrativeText at 0x13ab14370>,
-        <unstructured.documents.html.HTMLTitle at 0x106877970>,
-        <unstructured.documents.html.HTMLListItem at 0x1068776a0>,
-        <unstructured.documents.html.HTMLListItem at 0x13fe4b0a0>]
-        ```
-        
-        Run `print("\n\n".join([str(el) for el in elements]))` to get a string representation of the
-        output, which looks like:
-        
-        ```python
-        This is a test document to use for unit tests.
-        
-        Important points:
-        
-        Hamburgers are delicious
-        
-        Dogs are the best
-        
-        I love fuzzy blankets
-        ```
-        
+        See the [partitioning](https://unstructured-io.github.io/unstructured/bricks.html#partitioning)
+        section in our documentation for a full list of options and instructions on how to use
+        file-specific partitioning functions.
         
         ## :guardsman: Security Policy
         
         See our [security policy](https://github.com/Unstructured-IO/unstructured/security/policy) for
         information on how to report security vulnerabilities.
         
         ## :books: Learn more
@@ -400,14 +280,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -15,90 +15,107 @@
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
 [![Downloads](https://static.pepy.tech/badge/unstructured)](https://pepy.tech/
       project/unstructured) [![Downloads](https://static.pepy.tech/badge/
          unstructured/month)](https://pepy.tech/project/unstructured)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
-                          ***** Announcement!!! *****
-We're excited to announce the public release of the unstructured.io hosted API!
- Now you can leverage Unstructured with a simple API call to render clean text
-     in JSON format out of your images, documents, powerpoints, and more.
- Checkout the readme here to get started making API calls. Youâll also find
-instructions there about how to host your own version of the API. Unstructured
-data just got easier! We'd love to hear your feedback, let us know how it goes
-  in our community_slack. And stay tuned for improvements to both quality and
-                      performance over the coming months!
-                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
 broom: ***Cleaning bricks*** that remove unwanted text from documents, such as
 boilerplate and sentence fragments. - :performing_arts: ***Staging bricks***
 that format data for downstream tasks, such as ML inference and data labeling.
-## :eight_pointed_black_star: Quick Start Use the following instructions to get
-up and running with `unstructured` and test your installation. NOTE: We do not
+Unstructured also provides the capabilities from `unstructured` as an API.
+Checkout the [`unstructured-api` repo](https://github.com/Unstructured-IO/
+unstructured-api) to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. ## :
+eight_pointed_black_star: Quick Start Use the following instructions to get up
+and running with `unstructured` and test your installation. NOTE: We do not
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
 facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
 should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` And if you installed with `local-inference`, you should be able
-to run this as well: ```python from unstructured.partition.auto import
-partition elements = partition("example-docs/layout-parser-paper.pdf") print
-("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
-using the docker image The following instructions are intended to help you get
-up and running using Docker to interact with `unstructured`. See [here](https:/
-/docs.docker.com/get-docker/) if you don't already have docker installed on
-your machine. NOTE: we build multi-platform images to support both x86_64 and
-Apple silicon hardware. `docker pull` should download the corresponding image
-for your architecture, but you can specify with `--platform` (e.g. `--platform
-linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
-tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
-the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
-with `latest`. To leverage this, `docker pull` from our image repository.
-```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
-pulled, you can create a container from this image and shell to it. ```bash #
-create the container docker run -dt --name unstructured quay.io/unstructured-
-io/unstructured:latest # this will drop you into a bash shell where the Docker
-image is running docker exec -it unstructured bash ``` You can also build your
-own Docker image. If you only plan on parsing one type of data you can speed up
-building the image by commenting out some of the packages/requirements
-necessary for other data types. See Dockerfile to know which lines are
-necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+elements])) ``` The following table shows the document types the `unstructured`
+library currently supports. `partition` will recognize each of these document
+types and route the document to the appropriate partitioning function. If you
+already know your document type, you can use the partitioning function listed
+in the table directly. See our [documentation page](https://unstructured-
+io.github.io/unstructured/) for more details about the library. | Document Type
+| Partition Function | Strategies | Table Support | Options | | --- | --- | --
+- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
+E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
+`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
+N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
+| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
+`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
+Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
+Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
+(`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
+Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
+Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
+:dizzy: Instructions for using the docker image The following instructions are
+intended to help you get up and running using Docker to interact with
+`unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
+already have docker installed on your machine. NOTE: we build multi-platform
+images to support both x86_64 and Apple silicon hardware. `docker pull` should
+download the corresponding image for your architecture, but you can specify
+with `--platform` (e.g. `--platform linux/amd64`) if needed. We build Docker
+images for all pushes to `main`. We tag each image with the corresponding short
+commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`).
+We also tag the most recent image with `latest`. To leverage this, `docker
+pull` from our image repository. ```bash docker pull quay.io/unstructured-io/
+unstructured:latest ``` Once pulled, you can create a container from this image
+and shell to it. ```bash # create the container docker run -dt --name
+unstructured quay.io/unstructured-io/unstructured:latest # this will drop you
+into a bash shell where the Docker image is running docker exec -it
+unstructured bash ``` You can also build your own Docker image. If you only
+plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
@@ -110,33 +127,30 @@
 changes should be applied, and `make tidy` to apply them. If using the optional
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
-show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
-documents with one line of code!
+show how to get started with the `unstructured` library. You can parse over a
+dozen document types with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
 `libmagic` using the instructions outlined [here](https://unstructured-
 io.github.io/unstructured/installing.html#filetype-detection) `partition` will
 always apply the default arguments. If you need advanced features, use a
-document-specific brick. The `partition` brick currently works for `.txt`,
-`.doc`, `.docx`, `.ppt`, `.pptx`, `.xlsx`, `.jpg`, `.png`, `.eml`, `.msg`,
-`.html`, and `.pdf` documents. ```python from unstructured.partition.auto
-import partition elements = partition("example-docs/layout-parser-paper.pdf")
-``` Run `print("\n\n".join([str(el) for el in elements]))` to get a string
+document-specific brick. See the table above for a full list of document types
+supported in the library. ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") ``` Run
+`print("\n\n".join([str(el) for el in elements]))` to get a string
 representation of the output, which looks like: ``` LayoutParser : A Uniï¬ed
 Toolkit for Deep Learning Based Document Image Analysis Zejiang Shen 1 ( (cid:
 0) ), Ruochen Zhang 2 , Melissa Dell 3 , Benjamin Charles Germain Lee 4 , Jacob
 Carlson 3 , and Weining Li 5 Abstract. Recent advances in document image
 analysis (DIA) have been primarily driven by the application of neural
 networks. Ideally, research outcomes could be easily deployed in production and
 extended for further investigation. However, various factors like loosely
@@ -156,75 +170,30 @@
 both pre-trained models and full document digiti- zation pipelines. We
 demonstrate that LayoutParser is helpful for both lightweight and large-scale
 digitization pipelines in real-word use cases. The library is publicly
 available at https://layout-parser.github.io Keywords: Document Image Analysis
 Â· Deep Learning Â· Layout Analysis Â· Character Recognition Â· Open Source
 library Â· Toolkit. Introduction Deep Learning(DL)-based approaches are the
 state-of-the-art for a wide range of document image analysis (DIA) tasks
-including document image classiï¬cation [11, ``` ### HTML Parsing You can
-parse an HTML document using the following workflow: ```python from
-unstructured.partition.html import partition_html elements = partition_html
-("example-docs/example-10k.html") print("\n\n".join([str(el) for el in elements
-[:5]])) ``` The print statement will show the following text: ``` UNITED STATES
-SECURITIES AND EXCHANGE COMMISSION Washington, D.C. 20549 FORM 10-K ANNUAL
-REPORT PURSUANT TO SECTION 13 OR 15(d) OF THE SECURITIES EXCHANGE ACT OF 1934
-``` And `elements` will be a list of elements in the HTML document, similar to
-the following: ```python [
-documents.elements.Title at 0x169cbe820>,
-documents.elements.NarrativeText at 0x169cbe8e0>,
-documents.elements.NarrativeText at 0x169cbe3a0>] ``` ### PDF Parsing You can
-use the following workflow to parse PDF documents. ```python from
-unstructured.partition.pdf import partition_pdf elements = partition_pdf
-("example-docs/layout-parser-paper.pdf") ``` The output will look the same as
-the example from the document parsing section above. ### E-mail Parsing The
-`partition_email` function within `unstructured` is helpful for parsing `.eml`
-files. Common e-mail clients such as Microsoft Outlook and Gmail support
-exporting e-mails as `.eml` files. `partition_email` accepts filenames, file-
-like object, and raw text as input. The following three snippets for parsing
-`.eml` files are equivalent: ```python from unstructured.partition.email import
-partition_email elements = partition_email(filename="example-docs/fake-
-email.eml") with open("example-docs/fake-email.eml", "r") as f: elements =
-partition_email(file=f) with open("example-docs/fake-email.eml", "r") as f:
-text = f.read() elements = partition_email(text=text) ``` The `elements` output
-will look like the following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test email to use for unit tests. Important
-points: Roses are red Violets are blue ``` ### Text Document Parsing The
-`partition_text` function within `unstructured` can be used to parse simple
-text files into elements. `partition_text` accepts filenames, file-like object,
-and raw text as input. The following three snippets are for parsing text files:
-```python from unstructured.partition.text import partition_text elements =
-partition_text(filename="example-docs/fake-text.txt") with open("example-docs/
-fake-text.txt", "r") as f: elements = partition_text(file=f) with open
-("example-docs/fake-text.txt", "r") as f: text = f.read() elements =
-partition_text(text=text) ``` The `elements` output will look like the
-following: ```python [
-documents.html.HTMLNarrativeText at 0x13ab14370>,
-documents.html.HTMLTitle at 0x106877970>,
-documents.html.HTMLListItem at 0x1068776a0>,
-documents.html.HTMLListItem at 0x13fe4b0a0>] ``` Run `print("\n\n".join([str
-(el) for el in elements]))` to get a string representation of the output, which
-looks like: ```python This is a test document to use for unit tests. Important
-points: Hamburgers are delicious Dogs are the best I love fuzzy blankets ``` ##
-:guardsman: Security Policy See our [security policy](https://github.com/
-Unstructured-IO/unstructured/security/policy) for information on how to report
-security vulnerabilities. ## :books: Learn more | Section | Description | |-|-
-| | [Company Website](https://unstructured.io) | Unstructured.io product and
-company info | | [Documentation](https://unstructured-io.github.io/
-unstructured) | Full API documentation | | [Batch Processing](Ingest.md) |
-Ingesting batches of documents through Unstructured | Keywords: NLP PDF HTML CV
-XML parsing preprocessing Platform: UNKNOWN Classifier: Development Status :: 4
-- Beta Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
-text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
-Provides-Extra: s3 Provides-Extra: azure Provides-Extra: discord Provides-
-Extra: github Provides-Extra: gitlab Provides-Extra: reddit Provides-Extra:
-slack Provides-Extra: wikipedia Provides-Extra: google-drive
+including document image classiï¬cation [11, ``` See the [partitioning](https:
+//unstructured-io.github.io/unstructured/bricks.html#partitioning) section in
+our documentation for a full list of options and instructions on how to use
+file-specific partitioning functions. ## :guardsman: Security Policy See our
+[security policy](https://github.com/Unstructured-IO/unstructured/security/
+policy) for information on how to report security vulnerabilities. ## :books:
+Learn more | Section | Description | |-|-| | [Company Website](https://
+unstructured.io) | Unstructured.io product and company info | | [Documentation]
+(https://unstructured-io.github.io/unstructured) | Full API documentation | |
+[Batch Processing](Ingest.md) | Ingesting batches of documents through
+Unstructured | Keywords: NLP PDF HTML CV XML parsing preprocessing Platform:
+UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
+Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
+discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
+Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
```

### Comparing `unstructured-0.6.9/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.0/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

