# Comparing `tmp/google-cloud-dialogflow-2.9.0.tar.gz` & `tmp/google-cloud-dialogflow-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google-cloud-dialogflow-2.9.0.tar", last modified: Thu Sep 30 23:36:59 2021, max compression
+gzip compressed data, was "dist/google-cloud-dialogflow-2.9.1.tar", last modified: Tue Oct  5 10:22:32 2021, max compression
```

## Comparing `google-cloud-dialogflow-2.9.0.tar` & `google-cloud-dialogflow-2.9.1.tar`

### file list

```diff
@@ -1,454 +1,456 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.552462 google-cloud-dialogflow-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4110 2021-09-30 23:36:59.552462 google-cloud-dialogflow-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3285 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/docs/
--rw-rw-r--   0 root         (0)     1003    12417 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/docs/conf.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.464462 google-cloud-dialogflow-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.468462 google-cloud-dialogflow-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow/
--rw-rw-r--   0 root         (0)     1003    22551 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow/__init__.py
--rw-rw-r--   0 root         (0)     1003       84 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/
--rw-rw-r--   0 root         (0)     1003    16763 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    25544 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       84 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/
--rw-rw-r--   0 root         (0)     1003      737 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/__init__.py
--rw-rw-r--   0 root         (0)     1003    39220 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/async_client.py
--rw-rw-r--   0 root         (0)     1003    48557 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/client.py
--rw-rw-r--   0 root         (0)     1003     5655 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.476462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10382 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25155 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25693 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.480462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/__init__.py
--rw-rw-r--   0 root         (0)     1003    16076 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/async_client.py
--rw-rw-r--   0 root         (0)     1003    24241 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/client.py
--rw-rw-r--   0 root         (0)     1003     5943 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.480462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7509 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12775 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13096 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.480462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/__init__.py
--rw-rw-r--   0 root         (0)     1003    30448 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/async_client.py
--rw-rw-r--   0 root         (0)     1003    39582 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/client.py
--rw-rw-r--   0 root         (0)     1003     5697 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.480462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8853 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16830 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17254 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.480462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/
--rw-rw-r--   0 root         (0)     1003      793 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/__init__.py
--rw-rw-r--   0 root         (0)     1003    26384 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/async_client.py
--rw-rw-r--   0 root         (0)     1003    37365 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/client.py
--rw-rw-r--   0 root         (0)     1003     6295 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.484462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9371 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17537 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17931 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.484462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/__init__.py
--rw-rw-r--   0 root         (0)     1003    26260 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/async_client.py
--rw-rw-r--   0 root         (0)     1003    36060 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/client.py
--rw-rw-r--   0 root         (0)     1003    10947 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.484462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8758 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17499 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17909 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.484462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/
--rw-rw-r--   0 root         (0)     1003      749 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/__init__.py
--rw-rw-r--   0 root         (0)     1003    33109 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/async_client.py
--rw-rw-r--   0 root         (0)     1003    42129 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/client.py
--rw-rw-r--   0 root         (0)     1003     5742 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.484462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/
--rw-rw-r--   0 root         (0)     1003     1149 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9226 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19710 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20216 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.488462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/
--rw-rw-r--   0 root         (0)     1003      757 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54344 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/async_client.py
--rw-rw-r--   0 root         (0)     1003    64202 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/client.py
--rw-rw-r--   0 root         (0)     1003     5853 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.488462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/
--rw-rw-r--   0 root         (0)     1003     1167 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11304 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26891 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27482 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.488462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    24762 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    34519 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003    10949 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.488462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9089 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17975 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18434 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.488462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/__init__.py
--rw-rw-r--   0 root         (0)     1003    15173 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/async_client.py
--rw-rw-r--   0 root         (0)     1003    23269 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.492462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7347 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12541 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12875 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.492462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/
--rw-rw-r--   0 root         (0)     1003      741 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/__init__.py
--rw-rw-r--   0 root         (0)     1003    38924 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/async_client.py
--rw-rw-r--   0 root         (0)     1003    48581 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/client.py
--rw-rw-r--   0 root         (0)     1003     5652 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.492462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/
--rw-rw-r--   0 root         (0)     1003     1131 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9613 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20528 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21042 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.492462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/
--rw-rw-r--   0 root         (0)     1003      769 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/__init__.py
--rw-rw-r--   0 root         (0)     1003    25766 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/async_client.py
--rw-rw-r--   0 root         (0)     1003    34634 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/client.py
--rw-rw-r--   0 root         (0)     1003     5988 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.492462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9013 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16354 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16756 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.496462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/__init__.py
--rw-rw-r--   0 root         (0)     1003    32465 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/async_client.py
--rw-rw-r--   0 root         (0)     1003    43485 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/client.py
--rw-rw-r--   0 root         (0)     1003     5877 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.496462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10026 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18864 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19353 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.496462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/
--rw-rw-r--   0 root         (0)     1003      785 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/__init__.py
--rw-rw-r--   0 root         (0)     1003    28589 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/async_client.py
--rw-rw-r--   0 root         (0)     1003    37742 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/client.py
--rw-rw-r--   0 root         (0)     1003     6226 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.496462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9308 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17834 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18217 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.496462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/__init__.py
--rw-rw-r--   0 root         (0)     1003    18095 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/async_client.py
--rw-rw-r--   0 root         (0)     1003    27042 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.500462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7843 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13439 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13769 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.500462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    26222 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    35057 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/client.py
--rw-rw-r--   0 root         (0)     1003     5697 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.500462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8458 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15954 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16356 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.504462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/
--rw-rw-r--   0 root         (0)     1003    10438 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12939 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/agent.py
--rw-rw-r--   0 root         (0)     1003    11430 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/answer_record.py
--rw-rw-r--   0 root         (0)     1003    16586 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/audio_config.py
--rw-rw-r--   0 root         (0)     1003    10027 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/context.py
--rw-rw-r--   0 root         (0)     1003    12686 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation.py
--rw-rw-r--   0 root         (0)     1003     2306 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation_event.py
--rw-rw-r--   0 root         (0)     1003    29356 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation_profile.py
--rw-rw-r--   0 root         (0)     1003    11236 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/document.py
--rw-rw-r--   0 root         (0)     1003    17376 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/entity_type.py
--rw-rw-r--   0 root         (0)     1003    14509 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/environment.py
--rw-rw-r--   0 root         (0)     1003     6177 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/fulfillment.py
--rw-rw-r--   0 root         (0)     1003      731 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/gcs.py
--rw-rw-r--   0 root         (0)     1003     1912 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/human_agent_assistant_event.py
--rw-rw-r--   0 root         (0)     1003    53898 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/intent.py
--rw-rw-r--   0 root         (0)     1003     6608 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/knowledge_base.py
--rw-rw-r--   0 root         (0)     1003    26677 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/participant.py
--rw-rw-r--   0 root         (0)     1003    35935 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/session.py
--rw-rw-r--   0 root         (0)     1003     8810 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/session_entity_type.py
--rw-rw-r--   0 root         (0)     1003     2735 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/validation_result.py
--rw-rw-r--   0 root         (0)     1003     7431 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/version.py
--rw-rw-r--   0 root         (0)     1003     8773 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/webhook.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.504462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/
--rw-rw-r--   0 root         (0)     1003    18456 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    27112 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       84 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.504462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.504462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/
--rw-rw-r--   0 root         (0)     1003      737 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/__init__.py
--rw-rw-r--   0 root         (0)     1003    39771 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/async_client.py
--rw-rw-r--   0 root         (0)     1003    49108 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/client.py
--rw-rw-r--   0 root         (0)     1003     5700 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.508462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10397 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25259 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25797 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.508462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/__init__.py
--rw-rw-r--   0 root         (0)     1003    19712 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/async_client.py
--rw-rw-r--   0 root         (0)     1003    28071 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/client.py
--rw-rw-r--   0 root         (0)     1003     5988 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.508462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7934 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13953 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14310 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.508462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/__init__.py
--rw-rw-r--   0 root         (0)     1003    32318 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/async_client.py
--rw-rw-r--   0 root         (0)     1003    41452 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/client.py
--rw-rw-r--   0 root         (0)     1003     5742 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.508462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8863 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16879 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17303 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.512462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/
--rw-rw-r--   0 root         (0)     1003      793 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/__init__.py
--rw-rw-r--   0 root         (0)     1003    26742 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/async_client.py
--rw-rw-r--   0 root         (0)     1003    38255 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/client.py
--rw-rw-r--   0 root         (0)     1003     6340 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.512462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9381 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17587 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17981 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.512462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/
--rw-rw-r--   0 root         (0)     1003      765 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/__init__.py
--rw-rw-r--   0 root         (0)     1003    29473 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/async_client.py
--rw-rw-r--   0 root         (0)     1003    39497 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/client.py
--rw-rw-r--   0 root         (0)     1003    11037 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.512462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9293 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18881 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19313 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.512462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/
--rw-rw-r--   0 root         (0)     1003      749 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/__init__.py
--rw-rw-r--   0 root         (0)     1003    37401 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/async_client.py
--rw-rw-r--   0 root         (0)     1003    46587 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/client.py
--rw-rw-r--   0 root         (0)     1003     5787 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.516462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/
--rw-rw-r--   0 root         (0)     1003     1149 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9639 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22507 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23049 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.516462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/
--rw-rw-r--   0 root         (0)     1003      757 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/__init__.py
--rw-rw-r--   0 root         (0)     1003    56014 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/async_client.py
--rw-rw-r--   0 root         (0)     1003    65871 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/client.py
--rw-rw-r--   0 root         (0)     1003     5898 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.516462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/
--rw-rw-r--   0 root         (0)     1003     1167 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11314 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26961 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27552 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.516462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/__init__.py
--rw-rw-r--   0 root         (0)     1003    24857 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/async_client.py
--rw-rw-r--   0 root         (0)     1003    34614 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/client.py
--rw-rw-r--   0 root         (0)     1003    11034 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.520462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9094 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17977 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18436 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.520462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/__init__.py
--rw-rw-r--   0 root         (0)     1003    15340 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/async_client.py
--rw-rw-r--   0 root         (0)     1003    23436 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.520462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7357 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12566 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12900 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.520462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/
--rw-rw-r--   0 root         (0)     1003      741 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/__init__.py
--rw-rw-r--   0 root         (0)     1003    39763 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/async_client.py
--rw-rw-r--   0 root         (0)     1003    49420 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/client.py
--rw-rw-r--   0 root         (0)     1003     5697 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.520462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/
--rw-rw-r--   0 root         (0)     1003     1131 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9623 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20587 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21101 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.524462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/
--rw-rw-r--   0 root         (0)     1003      769 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/__init__.py
--rw-rw-r--   0 root         (0)     1003    26478 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/async_client.py
--rw-rw-r--   0 root         (0)     1003    35346 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/client.py
--rw-rw-r--   0 root         (0)     1003     6033 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.524462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9023 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17001 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17403 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.524462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/
--rw-rw-r--   0 root         (0)     1003      761 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/__init__.py
--rw-rw-r--   0 root         (0)     1003    42818 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/async_client.py
--rw-rw-r--   0 root         (0)     1003    54984 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/client.py
--rw-rw-r--   0 root         (0)     1003    11016 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.524462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11496 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24652 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25225 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.524462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/
--rw-rw-r--   0 root         (0)     1003      785 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/__init__.py
--rw-rw-r--   0 root         (0)     1003    30171 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/async_client.py
--rw-rw-r--   0 root         (0)     1003    39324 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/client.py
--rw-rw-r--   0 root         (0)     1003     6271 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.528462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9318 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17874 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18257 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.528462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/__init__.py
--rw-rw-r--   0 root         (0)     1003    18925 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/async_client.py
--rw-rw-r--   0 root         (0)     1003    28423 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.528462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7853 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13459 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13789 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.528462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/
--rw-rw-r--   0 root         (0)     1003      745 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    26336 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    35171 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/client.py
--rw-rw-r--   0 root         (0)     1003     5742 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.528462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8468 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15998 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16400 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.536462 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/
--rw-rw-r--   0 root         (0)     1003    11617 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14275 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/agent.py
--rw-rw-r--   0 root         (0)     1003    12859 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/answer_record.py
--rw-rw-r--   0 root         (0)     1003    17739 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/audio_config.py
--rw-rw-r--   0 root         (0)     1003    12057 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/context.py
--rw-rw-r--   0 root         (0)     1003    14938 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation.py
--rw-rw-r--   0 root         (0)     1003     2318 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation_event.py
--rw-rw-r--   0 root         (0)     1003    30047 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation_profile.py
--rw-rw-r--   0 root         (0)     1003    16280 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/document.py
--rw-rw-r--   0 root         (0)     1003    18594 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/entity_type.py
--rw-rw-r--   0 root         (0)     1003    14381 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/environment.py
--rw-rw-r--   0 root         (0)     1003     6222 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/fulfillment.py
--rw-rw-r--   0 root         (0)     1003     1639 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/gcs.py
--rw-rw-r--   0 root         (0)     1003     2478 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/human_agent_assistant_event.py
--rw-rw-r--   0 root         (0)     1003    74410 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/intent.py
--rw-rw-r--   0 root         (0)     1003     7845 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/knowledge_base.py
--rw-rw-r--   0 root         (0)     1003    49904 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/participant.py
--rw-rw-r--   0 root         (0)     1003    44383 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/session.py
--rw-rw-r--   0 root         (0)     1003    10692 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/session_entity_type.py
--rw-rw-r--   0 root         (0)     1003     2750 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/validation_result.py
--rw-rw-r--   0 root         (0)     1003     7486 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/version.py
--rw-rw-r--   0 root         (0)     1003    10096 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/webhook.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.536462 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/
--rw-r--r--   0 root         (0)     1003     4110 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    22578 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       75 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       42 2021-09-30 23:36:59.000000 google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.472462 google-cloud-dialogflow-2.9.0/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.540462 google-cloud-dialogflow-2.9.0/samples/snippets/
--rw-rw-r--   0 root         (0)     1003     1732 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/answer_record_management.py
--rw-rw-r--   0 root         (0)     1003     3803 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/answer_record_management_test.py
--rw-rw-r--   0 root         (0)     1003     3424 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/conversation_management.py
--rw-rw-r--   0 root         (0)     1003     7929 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/conversation_profile_management.py
--rw-rw-r--   0 root         (0)     1003     2426 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/conversation_profile_management_test.py
--rw-rw-r--   0 root         (0)     1003     2259 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/create_document_test.py
--rw-rw-r--   0 root         (0)     1003     1530 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/create_knowledge_base_test.py
--rw-rw-r--   0 root         (0)     1003     3594 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_audio.py
--rw-rw-r--   0 root         (0)     1003     1261 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_audio_test.py
--rw-rw-r--   0 root         (0)     1003     4144 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_knowledge.py
--rw-rw-r--   0 root         (0)     1003     1091 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_knowledge_test.py
--rw-rw-r--   0 root         (0)     1003     4402 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_stream.py
--rw-rw-r--   0 root         (0)     1003     1124 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_stream_test.py
--rw-rw-r--   0 root         (0)     1003     3041 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts.py
--rw-rw-r--   0 root         (0)     1003     1119 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_test.py
--rw-rw-r--   0 root         (0)     1003     3228 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_with_location.py
--rw-rw-r--   0 root         (0)     1003     1231 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_with_location_test.py
--rw-rw-r--   0 root         (0)     1003     3986 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_sentiment_analysis.py
--rw-rw-r--   0 root         (0)     1003     1191 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_sentiment_analysis_test.py
--rw-rw-r--   0 root         (0)     1003     3620 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_texttospeech_response.py
--rw-rw-r--   0 root         (0)     1003     1217 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_texttospeech_response_test.py
--rw-rw-r--   0 root         (0)     1003     8721 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/document_management.py
--rw-rw-r--   0 root         (0)     1003     5613 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/intent_management.py
--rw-rw-r--   0 root         (0)     1003     1877 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/intent_management_test.py
--rw-rw-r--   0 root         (0)     1003     4872 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/knowledge_base_management.py
--rw-rw-r--   0 root         (0)     1003     8499 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/noxfile.py
--rw-rw-r--   0 root         (0)     1003     4681 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/participant_management.py
--rw-rw-r--   0 root         (0)     1003     5913 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/participant_management_test.py
--rw-rw-r--   0 root         (0)     1003     1137 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/set_agent.py
--rw-rw-r--   0 root         (0)     1003     1013 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/set_agent_test.py
--rw-rw-r--   0 root         (0)     1003     1191 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/update_intent.py
--rw-rw-r--   0 root         (0)     1003     1777 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/update_intent_test.py
--rw-rw-r--   0 root         (0)     1003     1328 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/webhook.py
--rw-rw-r--   0 root         (0)     1003      632 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/samples/snippets/webhook_test.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.544462 google-cloud-dialogflow-2.9.0/scripts/
--rw-rw-r--   0 root         (0)     1003    11364 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/scripts/fixup_dialogflow_v2_keywords.py
--rw-rw-r--   0 root         (0)     1003    11921 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/scripts/fixup_dialogflow_v2beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2021-09-30 23:36:59.552462 google-cloud-dialogflow-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2446 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.544462 google-cloud-dialogflow-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.544462 google-cloud-dialogflow-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.544462 google-cloud-dialogflow-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.548462 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   111019 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_agents.py
--rw-rw-r--   0 root         (0)     1003    65202 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_answer_records.py
--rw-rw-r--   0 root         (0)     1003    91754 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_contexts.py
--rw-rw-r--   0 root         (0)     1003    99766 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_conversation_profiles.py
--rw-rw-r--   0 root         (0)     1003    98776 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_conversations.py
--rw-rw-r--   0 root         (0)     1003    95986 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_documents.py
--rw-rw-r--   0 root         (0)     1003   134235 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_entity_types.py
--rw-rw-r--   0 root         (0)     1003    91232 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_environments.py
--rw-rw-r--   0 root         (0)     1003    58157 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_fulfillments.py
--rw-rw-r--   0 root         (0)     1003   113372 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_intents.py
--rw-rw-r--   0 root         (0)     1003    91723 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_knowledge_bases.py
--rw-rw-r--   0 root         (0)     1003   110783 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_participants.py
--rw-rw-r--   0 root         (0)     1003    96064 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_session_entity_types.py
--rw-rw-r--   0 root         (0)     1003    54465 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_sessions.py
--rw-rw-r--   0 root         (0)     1003    85768 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_versions.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 23:36:59.552462 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   111084 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_agents.py
--rw-rw-r--   0 root         (0)     1003    70825 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_answer_records.py
--rw-rw-r--   0 root         (0)     1003    91814 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_contexts.py
--rw-rw-r--   0 root         (0)     1003   102075 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_conversation_profiles.py
--rw-rw-r--   0 root         (0)     1003   107190 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_conversations.py
--rw-rw-r--   0 root         (0)     1003   101301 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_documents.py
--rw-rw-r--   0 root         (0)     1003   134759 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_entity_types.py
--rw-rw-r--   0 root         (0)     1003    91306 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_environments.py
--rw-rw-r--   0 root         (0)     1003    58221 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_fulfillments.py
--rw-rw-r--   0 root         (0)     1003   113857 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_intents.py
--rw-rw-r--   0 root         (0)     1003    91792 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_knowledge_bases.py
--rw-rw-r--   0 root         (0)     1003   137017 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_participants.py
--rw-rw-r--   0 root         (0)     1003    96129 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_session_entity_types.py
--rw-rw-r--   0 root         (0)     1003    55330 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_sessions.py
--rw-rw-r--   0 root         (0)     1003    85828 2021-09-30 23:33:41.000000 google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.930727 google-cloud-dialogflow-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4110 2021-10-05 10:22:32.930727 google-cloud-dialogflow-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3285 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.842727 google-cloud-dialogflow-2.9.1/docs/
+-rw-rw-r--   0 root         (0)     1003    12417 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/docs/conf.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.834727 google-cloud-dialogflow-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.838727 google-cloud-dialogflow-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.842727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow/
+-rw-rw-r--   0 root         (0)     1003    22551 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow/__init__.py
+-rw-rw-r--   0 root         (0)     1003       84 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.846727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/
+-rw-rw-r--   0 root         (0)     1003    16763 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25544 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       84 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.846727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.846727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/
+-rw-rw-r--   0 root         (0)     1003      737 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39220 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48557 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/client.py
+-rw-rw-r--   0 root         (0)     1003     5655 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.846727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10382 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25155 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25693 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.846727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16076 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24241 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/client.py
+-rw-rw-r--   0 root         (0)     1003     5943 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.850727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7509 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12775 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13096 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.850727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30448 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39582 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/client.py
+-rw-rw-r--   0 root         (0)     1003     5697 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.850727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8853 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16830 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17254 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.850727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/
+-rw-rw-r--   0 root         (0)     1003      793 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26384 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37365 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/client.py
+-rw-rw-r--   0 root         (0)     1003     6295 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.854727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9371 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17537 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17931 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.854727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26260 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36060 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/client.py
+-rw-rw-r--   0 root         (0)     1003    10947 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.854727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8758 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17499 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17909 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.854727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/
+-rw-rw-r--   0 root         (0)     1003      749 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33109 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42129 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/client.py
+-rw-rw-r--   0 root         (0)     1003     5742 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.854727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/
+-rw-rw-r--   0 root         (0)     1003     1149 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9226 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19710 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20216 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.858727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/
+-rw-rw-r--   0 root         (0)     1003      757 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54344 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64202 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/client.py
+-rw-rw-r--   0 root         (0)     1003     5853 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.858727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/
+-rw-rw-r--   0 root         (0)     1003     1167 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11304 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26891 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27482 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.858727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24762 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34519 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003    10949 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.858727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9089 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17975 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18434 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.862727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15173 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23269 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.862727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7347 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12541 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12875 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.862727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/
+-rw-rw-r--   0 root         (0)     1003      741 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38924 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48581 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/client.py
+-rw-rw-r--   0 root         (0)     1003     5652 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.862727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/
+-rw-rw-r--   0 root         (0)     1003     1131 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9613 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20528 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21042 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.866727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/
+-rw-rw-r--   0 root         (0)     1003      769 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25766 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34634 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/client.py
+-rw-rw-r--   0 root         (0)     1003     5988 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.866727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9013 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16354 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16756 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.866727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32465 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43485 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/client.py
+-rw-rw-r--   0 root         (0)     1003     5877 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.866727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10026 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18864 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19353 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.866727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/
+-rw-rw-r--   0 root         (0)     1003      785 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28589 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37742 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/client.py
+-rw-rw-r--   0 root         (0)     1003     6226 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.870727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9308 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17834 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18217 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.870727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18095 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27042 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.870727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7843 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13439 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13769 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.870727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26222 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    35057 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/client.py
+-rw-rw-r--   0 root         (0)     1003     5697 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.874727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8458 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15954 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16356 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.878727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/
+-rw-rw-r--   0 root         (0)     1003    10438 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12939 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/agent.py
+-rw-rw-r--   0 root         (0)     1003    11430 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/answer_record.py
+-rw-rw-r--   0 root         (0)     1003    16586 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/audio_config.py
+-rw-rw-r--   0 root         (0)     1003    10027 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/context.py
+-rw-rw-r--   0 root         (0)     1003    12686 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation.py
+-rw-rw-r--   0 root         (0)     1003     2306 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation_event.py
+-rw-rw-r--   0 root         (0)     1003    29356 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation_profile.py
+-rw-rw-r--   0 root         (0)     1003    11236 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/document.py
+-rw-rw-r--   0 root         (0)     1003    17376 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/entity_type.py
+-rw-rw-r--   0 root         (0)     1003    14509 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/environment.py
+-rw-rw-r--   0 root         (0)     1003     6177 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/fulfillment.py
+-rw-rw-r--   0 root         (0)     1003      731 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/gcs.py
+-rw-rw-r--   0 root         (0)     1003     1912 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/human_agent_assistant_event.py
+-rw-rw-r--   0 root         (0)     1003    53898 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/intent.py
+-rw-rw-r--   0 root         (0)     1003     6608 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/knowledge_base.py
+-rw-rw-r--   0 root         (0)     1003    26677 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/participant.py
+-rw-rw-r--   0 root         (0)     1003    35935 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/session.py
+-rw-rw-r--   0 root         (0)     1003     8810 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/session_entity_type.py
+-rw-rw-r--   0 root         (0)     1003     2735 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/validation_result.py
+-rw-rw-r--   0 root         (0)     1003     7431 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/version.py
+-rw-rw-r--   0 root         (0)     1003     8773 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/webhook.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.878727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/
+-rw-rw-r--   0 root         (0)     1003    18456 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27112 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       84 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.878727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.878727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/
+-rw-rw-r--   0 root         (0)     1003      737 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39771 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    49108 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/client.py
+-rw-rw-r--   0 root         (0)     1003     5700 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.878727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10397 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25259 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25797 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.882727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19712 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28071 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/client.py
+-rw-rw-r--   0 root         (0)     1003     5988 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.882727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7934 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13953 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14310 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.882727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32318 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41452 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/client.py
+-rw-rw-r--   0 root         (0)     1003     5742 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.882727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8863 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16879 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17303 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.886727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/
+-rw-rw-r--   0 root         (0)     1003      793 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26742 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/async_client.py
+-rw-rw-r--   0 root         (0)     1003    38255 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/client.py
+-rw-rw-r--   0 root         (0)     1003     6340 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.886727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9381 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17587 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17981 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.886727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/
+-rw-rw-r--   0 root         (0)     1003      765 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29473 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39497 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/client.py
+-rw-rw-r--   0 root         (0)     1003    11037 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.886727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9293 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18881 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19313 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.890727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/
+-rw-rw-r--   0 root         (0)     1003      749 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37401 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46587 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/client.py
+-rw-rw-r--   0 root         (0)     1003     5787 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.890727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/
+-rw-rw-r--   0 root         (0)     1003     1149 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9639 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22507 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23049 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.890727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/
+-rw-rw-r--   0 root         (0)     1003      757 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56014 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/async_client.py
+-rw-rw-r--   0 root         (0)     1003    65871 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/client.py
+-rw-rw-r--   0 root         (0)     1003     5898 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.890727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/
+-rw-rw-r--   0 root         (0)     1003     1167 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11314 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26961 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27552 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.890727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24857 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34614 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/client.py
+-rw-rw-r--   0 root         (0)     1003    11034 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.894727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9094 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17977 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18436 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.894727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15340 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23436 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.894727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7357 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12566 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12900 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.894727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/
+-rw-rw-r--   0 root         (0)     1003      741 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39763 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/async_client.py
+-rw-rw-r--   0 root         (0)     1003    49420 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/client.py
+-rw-rw-r--   0 root         (0)     1003     5697 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.898727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/
+-rw-rw-r--   0 root         (0)     1003     1131 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9623 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20587 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21101 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.898727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/
+-rw-rw-r--   0 root         (0)     1003      769 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26478 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/async_client.py
+-rw-rw-r--   0 root         (0)     1003    35346 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/client.py
+-rw-rw-r--   0 root         (0)     1003     6033 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.898727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9023 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17001 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17403 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.898727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/
+-rw-rw-r--   0 root         (0)     1003      761 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42818 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/async_client.py
+-rw-rw-r--   0 root         (0)     1003    54984 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/client.py
+-rw-rw-r--   0 root         (0)     1003    11016 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.898727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11496 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24652 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25225 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.902727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/
+-rw-rw-r--   0 root         (0)     1003      785 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30171 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39324 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/client.py
+-rw-rw-r--   0 root         (0)     1003     6271 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.902727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9318 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17874 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18257 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.902727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18925 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28423 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.902727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7853 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13459 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13789 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.906727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/
+-rw-rw-r--   0 root         (0)     1003      745 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26336 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    35171 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/client.py
+-rw-rw-r--   0 root         (0)     1003     5742 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.906727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8468 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15998 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16400 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.910727 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/
+-rw-rw-r--   0 root         (0)     1003    11617 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14275 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/agent.py
+-rw-rw-r--   0 root         (0)     1003    12859 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/answer_record.py
+-rw-rw-r--   0 root         (0)     1003    17739 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/audio_config.py
+-rw-rw-r--   0 root         (0)     1003    12057 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/context.py
+-rw-rw-r--   0 root         (0)     1003    14938 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation.py
+-rw-rw-r--   0 root         (0)     1003     2318 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation_event.py
+-rw-rw-r--   0 root         (0)     1003    30047 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation_profile.py
+-rw-rw-r--   0 root         (0)     1003    16280 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/document.py
+-rw-rw-r--   0 root         (0)     1003    18594 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/entity_type.py
+-rw-rw-r--   0 root         (0)     1003    14381 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/environment.py
+-rw-rw-r--   0 root         (0)     1003     6222 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/fulfillment.py
+-rw-rw-r--   0 root         (0)     1003     1639 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/gcs.py
+-rw-rw-r--   0 root         (0)     1003     2478 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/human_agent_assistant_event.py
+-rw-rw-r--   0 root         (0)     1003    74410 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/intent.py
+-rw-rw-r--   0 root         (0)     1003     7845 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/knowledge_base.py
+-rw-rw-r--   0 root         (0)     1003    49904 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/participant.py
+-rw-rw-r--   0 root         (0)     1003    44383 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/session.py
+-rw-rw-r--   0 root         (0)     1003    10692 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/session_entity_type.py
+-rw-rw-r--   0 root         (0)     1003     2750 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/validation_result.py
+-rw-rw-r--   0 root         (0)     1003     7486 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/version.py
+-rw-rw-r--   0 root         (0)     1003    10096 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/webhook.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.910727 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/
+-rw-r--r--   0 root         (0)     1003     4110 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    22667 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       75 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       42 2021-10-05 10:22:32.000000 google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.842727 google-cloud-dialogflow-2.9.1/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.918727 google-cloud-dialogflow-2.9.1/samples/snippets/
+-rw-rw-r--   0 root         (0)     1003     1658 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/answer_record_management.py
+-rw-rw-r--   0 root         (0)     1003     3690 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/answer_record_management_test.py
+-rw-rw-r--   0 root         (0)     1003     3359 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/conversation_management.py
+-rw-rw-r--   0 root         (0)     1003     7550 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/conversation_profile_management.py
+-rw-rw-r--   0 root         (0)     1003     2414 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/conversation_profile_management_test.py
+-rw-rw-r--   0 root         (0)     1003     2143 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/create_document_test.py
+-rw-rw-r--   0 root         (0)     1003     1530 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/create_knowledge_base_test.py
+-rw-rw-r--   0 root         (0)     1003     3578 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_audio.py
+-rw-rw-r--   0 root         (0)     1003     1261 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_audio_test.py
+-rw-rw-r--   0 root         (0)     1003     4144 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_knowledge.py
+-rw-rw-r--   0 root         (0)     1003     1091 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_knowledge_test.py
+-rw-rw-r--   0 root         (0)     1003     4402 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_stream.py
+-rw-rw-r--   0 root         (0)     1003     1124 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_stream_test.py
+-rw-rw-r--   0 root         (0)     1003     3041 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts.py
+-rw-rw-r--   0 root         (0)     1003     1119 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_test.py
+-rw-rw-r--   0 root         (0)     1003     3228 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_with_location.py
+-rw-rw-r--   0 root         (0)     1003     1231 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_with_location_test.py
+-rw-rw-r--   0 root         (0)     1003     3986 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_sentiment_analysis.py
+-rw-rw-r--   0 root         (0)     1003     1191 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_sentiment_analysis_test.py
+-rw-rw-r--   0 root         (0)     1003     3620 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_texttospeech_response.py
+-rw-rw-r--   0 root         (0)     1003     1217 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_texttospeech_response_test.py
+-rw-rw-r--   0 root         (0)     1003     8660 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/document_management.py
+-rw-rw-r--   0 root         (0)     1003     5613 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/intent_management.py
+-rw-rw-r--   0 root         (0)     1003     1877 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/intent_management_test.py
+-rw-rw-r--   0 root         (0)     1003     4830 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/knowledge_base_management.py
+-rw-rw-r--   0 root         (0)     1003     1569 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/list_training_phrases.py
+-rw-rw-r--   0 root         (0)     1003      969 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/list_training_phrases_test.py
+-rw-rw-r--   0 root         (0)     1003     8499 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/noxfile.py
+-rw-rw-r--   0 root         (0)     1003     4681 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/participant_management.py
+-rw-rw-r--   0 root         (0)     1003     5619 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/participant_management_test.py
+-rw-rw-r--   0 root         (0)     1003     1137 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/set_agent.py
+-rw-rw-r--   0 root         (0)     1003     1013 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/set_agent_test.py
+-rw-rw-r--   0 root         (0)     1003     1193 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/update_intent.py
+-rw-rw-r--   0 root         (0)     1003     1776 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/update_intent_test.py
+-rw-rw-r--   0 root         (0)     1003     1328 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/webhook.py
+-rw-rw-r--   0 root         (0)     1003      632 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/samples/snippets/webhook_test.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.918727 google-cloud-dialogflow-2.9.1/scripts/
+-rw-rw-r--   0 root         (0)     1003    11364 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/scripts/fixup_dialogflow_v2_keywords.py
+-rw-rw-r--   0 root         (0)     1003    11921 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/scripts/fixup_dialogflow_v2beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2021-10-05 10:22:32.930727 google-cloud-dialogflow-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2446 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.918727 google-cloud-dialogflow-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.918727 google-cloud-dialogflow-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.922727 google-cloud-dialogflow-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.926727 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111019 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_agents.py
+-rw-rw-r--   0 root         (0)     1003    65202 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_answer_records.py
+-rw-rw-r--   0 root         (0)     1003    91754 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_contexts.py
+-rw-rw-r--   0 root         (0)     1003    99766 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_conversation_profiles.py
+-rw-rw-r--   0 root         (0)     1003    98776 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_conversations.py
+-rw-rw-r--   0 root         (0)     1003    95986 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_documents.py
+-rw-rw-r--   0 root         (0)     1003   134235 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_entity_types.py
+-rw-rw-r--   0 root         (0)     1003    91232 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    58157 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_fulfillments.py
+-rw-rw-r--   0 root         (0)     1003   113372 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_intents.py
+-rw-rw-r--   0 root         (0)     1003    91723 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_knowledge_bases.py
+-rw-rw-r--   0 root         (0)     1003   110783 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_participants.py
+-rw-rw-r--   0 root         (0)     1003    96064 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_session_entity_types.py
+-rw-rw-r--   0 root         (0)     1003    54465 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_sessions.py
+-rw-rw-r--   0 root         (0)     1003    85768 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-05 10:22:32.930727 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   111084 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_agents.py
+-rw-rw-r--   0 root         (0)     1003    70825 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_answer_records.py
+-rw-rw-r--   0 root         (0)     1003    91814 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_contexts.py
+-rw-rw-r--   0 root         (0)     1003   102075 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_conversation_profiles.py
+-rw-rw-r--   0 root         (0)     1003   107190 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_conversations.py
+-rw-rw-r--   0 root         (0)     1003   101301 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_documents.py
+-rw-rw-r--   0 root         (0)     1003   134759 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_entity_types.py
+-rw-rw-r--   0 root         (0)     1003    91306 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_environments.py
+-rw-rw-r--   0 root         (0)     1003    58221 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_fulfillments.py
+-rw-rw-r--   0 root         (0)     1003   113857 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_intents.py
+-rw-rw-r--   0 root         (0)     1003    91792 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_knowledge_bases.py
+-rw-rw-r--   0 root         (0)     1003   137017 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_participants.py
+-rw-rw-r--   0 root         (0)     1003    96129 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_session_entity_types.py
+-rw-rw-r--   0 root         (0)     1003    55330 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_sessions.py
+-rw-rw-r--   0 root         (0)     1003    85828 2021-10-05 10:19:54.000000 google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_versions.py
```

### Comparing `google-cloud-dialogflow-2.9.0/LICENSE` & `google-cloud-dialogflow-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/MANIFEST.in` & `google-cloud-dialogflow-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/PKG-INFO` & `google-cloud-dialogflow-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dialogflow
-Version: 2.9.0
+Version: 2.9.1
 Summary: Client library for the Dialogflow API
 Home-page: https://github.com/googleapis/dialogflow-python-client-v2
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dialogflow-2.9.0/README.rst` & `google-cloud-dialogflow-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/docs/conf.py` & `google-cloud-dialogflow-2.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/gapic_metadata.json` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/agents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/agents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/answer_records/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/answer_records/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/contexts/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/contexts/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversation_profiles/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/conversations/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/conversations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/documents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/documents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/entity_types/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/entity_types/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/environments/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/environments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/fulfillments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/intents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/intents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/knowledge_bases/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/participants/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/participants/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/session_entity_types/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/sessions/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/sessions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/services/versions/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/services/versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/agent.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/agent.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/answer_record.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/answer_record.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/audio_config.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/audio_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/context.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/context.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation_event.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/conversation_profile.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/conversation_profile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/document.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/entity_type.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/entity_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/environment.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/environment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/fulfillment.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/fulfillment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/gcs.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/gcs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/human_agent_assistant_event.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/human_agent_assistant_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/intent.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/intent.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/knowledge_base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/participant.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/participant.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/session.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/session.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/session_entity_type.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/session_entity_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/validation_result.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/validation_result.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/version.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2/types/webhook.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2/types/webhook.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/gapic_metadata.json` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/agents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/answer_records/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/contexts/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversation_profiles/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/conversations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/documents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/entity_types/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/environments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/fulfillments/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/intents/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/knowledge_bases/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/participants/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/session_entity_types/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/sessions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/async_client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/client.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/pagers.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc_asyncio.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/services/versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/__init__.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/agent.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/agent.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/answer_record.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/answer_record.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/audio_config.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/audio_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/context.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/context.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation_event.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/conversation_profile.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/conversation_profile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/document.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/entity_type.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/entity_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/environment.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/environment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/fulfillment.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/fulfillment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/gcs.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/gcs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/human_agent_assistant_event.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/human_agent_assistant_event.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/intent.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/intent.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/knowledge_base.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/participant.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/participant.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/session.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/session.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/session_entity_type.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/session_entity_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/validation_result.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/validation_result.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/version.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google/cloud/dialogflow_v2beta1/types/webhook.py` & `google-cloud-dialogflow-2.9.1/google/cloud/dialogflow_v2beta1/types/webhook.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/PKG-INFO` & `google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dialogflow
-Version: 2.9.0
+Version: 2.9.1
 Summary: Client library for the Dialogflow API
 Home-page: https://github.com/googleapis/dialogflow-python-client-v2
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dialogflow-2.9.0/google_cloud_dialogflow.egg-info/SOURCES.txt` & `google-cloud-dialogflow-2.9.1/google_cloud_dialogflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,16 @@
 samples/snippets/detect_intent_with_sentiment_analysis_test.py
 samples/snippets/detect_intent_with_texttospeech_response.py
 samples/snippets/detect_intent_with_texttospeech_response_test.py
 samples/snippets/document_management.py
 samples/snippets/intent_management.py
 samples/snippets/intent_management_test.py
 samples/snippets/knowledge_base_management.py
+samples/snippets/list_training_phrases.py
+samples/snippets/list_training_phrases_test.py
 samples/snippets/noxfile.py
 samples/snippets/participant_management.py
 samples/snippets/participant_management_test.py
 samples/snippets/set_agent.py
 samples/snippets/set_agent_test.py
 samples/snippets/update_intent.py
 samples/snippets/update_intent_test.py
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/answer_record_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/answer_record_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,22 @@
     Args:
         project_id: The GCP project linked with the conversation profile.
         answer_record_id: The answer record id returned along with the
         suggestion.
         is_clicked: whether the answer record is clicked."""
 
     client = dialogflow.AnswerRecordsClient()
-    answer_record_path = client.answer_record_path(project_id,
-                                                   answer_record_id)
+    answer_record_path = client.answer_record_path(project_id, answer_record_id)
 
     response = client.update_answer_record(
         answer_record={
-            'name': answer_record_path,
-            'answer_feedback': {
-                'clicked': is_clicked
-            }
+            "name": answer_record_path,
+            "answer_feedback": {"clicked": is_clicked},
         },
-        update_mask={'paths': ['answer_feedback']})
-    print('AnswerRecord Name: {}'.format(response.name))
-    print('Clicked: {}'.format(response.answer_feedback.clicked))
+        update_mask={"paths": ["answer_feedback"]},
+    )
+    print("AnswerRecord Name: {}".format(response.name))
+    print("Clicked: {}".format(response.answer_feedback.clicked))
     return response
 
 
 # [END dialogflow_update_answer_record]
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/answer_record_management_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/answer_record_management_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,83 +15,91 @@
 import os
 
 import answer_record_management
 import conversation_management
 import conversation_profile_management
 import participant_management
 
-PROJECT_ID = os.getenv('GOOGLE_CLOUD_PROJECT')
-SMART_REPLY_MODEL = os.getenv('SMART_REPLY_MODEL')
-SMART_REPLY_ALLOWLIST = os.getenv('SMART_REPLY_ALLOWLIST')
-CONVERSATION_PROFILE_DISPLAY_NAME = 'sample code profile for smart reply'
+PROJECT_ID = os.getenv("GOOGLE_CLOUD_PROJECT")
+SMART_REPLY_MODEL = os.getenv("SMART_REPLY_MODEL")
+SMART_REPLY_ALLOWLIST = os.getenv("SMART_REPLY_ALLOWLIST")
+CONVERSATION_PROFILE_DISPLAY_NAME = "sample code profile for smart reply"
 
 
 def test_smart_reply(capsys):
     """Test smart reply feature.
     """
 
     # Create conversation profile.
     conversation_profile_management.create_conversation_profile_smart_reply(
         project_id=PROJECT_ID,
         display_name=CONVERSATION_PROFILE_DISPLAY_NAME,
         smart_reply_allowlist_name=SMART_REPLY_ALLOWLIST,
-        smart_reply_model_name=SMART_REPLY_MODEL)
+        smart_reply_model_name=SMART_REPLY_MODEL,
+    )
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
-    conversation_profile_id = out.split('conversationProfiles/')[1].rstrip()
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
+    conversation_profile_id = out.split("conversationProfiles/")[1].rstrip()
 
     # Create conversation.
     conversation_management.create_conversation(
-        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id)
+        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id
+    )
 
     out, _ = capsys.readouterr()
-    conversation_id = out.split('conversations/')[1].rstrip()
+    conversation_id = out.split("conversations/")[1].rstrip()
 
     # Create end user participant.
-    participant_management.create_participant(project_id=PROJECT_ID,
-                                              conversation_id=conversation_id,
-                                              role='END_USER')
+    participant_management.create_participant(
+        project_id=PROJECT_ID, conversation_id=conversation_id, role="END_USER"
+    )
     out, _ = capsys.readouterr()
-    end_user_id = out.split('participants/')[1].rstrip()
+    end_user_id = out.split("participants/")[1].rstrip()
 
     # Create human agent participant.
-    participant_management.create_participant(project_id=PROJECT_ID,
-                                              conversation_id=conversation_id,
-                                              role='HUMAN_AGENT')
+    participant_management.create_participant(
+        project_id=PROJECT_ID, conversation_id=conversation_id, role="HUMAN_AGENT"
+    )
     out, _ = capsys.readouterr()
-    human_agent_id = out.split('participants/')[1].rstrip()
+    human_agent_id = out.split("participants/")[1].rstrip()
 
     # AnalyzeContent
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=human_agent_id,
-        text='Hi, how are you?')
+        text="Hi, how are you?",
+    )
     out, _ = capsys.readouterr()
-    assert 'What would you like to know?' in out
+    assert "What would you like to know?" in out
 
     response = participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=end_user_id,
-        text='I am doing well, just want to check')
+        text="I am doing well, just want to check",
+    )
     out, _ = capsys.readouterr()
-    assert 'Sounds good.' in out
+    assert "Sounds good." in out
     # Update AnswerRecord.
-    answer_record_id = response.human_agent_suggestion_results[
-        0].suggest_smart_replies_response.smart_reply_answers[
-            0].answer_record.split('answerRecords/')[1].rstrip()
+    answer_record_id = (
+        response.human_agent_suggestion_results[0]
+        .suggest_smart_replies_response.smart_reply_answers[0]
+        .answer_record.split("answerRecords/")[1]
+        .rstrip()
+    )
     answer_record_management.update_answer_record(
-        project_id=PROJECT_ID,
-        answer_record_id=answer_record_id,
-        is_clicked=True)
+        project_id=PROJECT_ID, answer_record_id=answer_record_id, is_clicked=True
+    )
     out, _ = capsys.readouterr()
-    assert 'Clicked: True' in out
+    assert "Clicked: True" in out
 
     # Complete conversation.
     conversation_management.complete_conversation(
-        project_id=PROJECT_ID, conversation_id=conversation_id)
+        project_id=PROJECT_ID, conversation_id=conversation_id
+    )
 
     # Delete conversation profile.
     conversation_profile_management.delete_conversation_profile(
-        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id)
+        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id
+    )
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/conversation_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/conversation_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,25 @@
         project_id:  The GCP project linked with the conversation.
         conversation_profile_id: The conversation profile id used to create
         conversation."""
 
     client = dialogflow.ConversationsClient()
     conversation_profile_client = dialogflow.ConversationProfilesClient()
     project_path = client.common_project_path(project_id)
-    conversation_profile_path = (
-        conversation_profile_client.conversation_profile_path(
-            project_id, conversation_profile_id))
-    conversation = {'conversation_profile': conversation_profile_path}
-    response = client.create_conversation(parent=project_path,
-                                          conversation=conversation)
-
-    print('Life Cycle State: {}'.format(response.lifecycle_state))
-    print('Conversation Profile Name: {}'.format(
-        response.conversation_profile))
-    print('Name: {}'.format(response.name))
+    conversation_profile_path = conversation_profile_client.conversation_profile_path(
+        project_id, conversation_profile_id
+    )
+    conversation = {"conversation_profile": conversation_profile_path}
+    response = client.create_conversation(
+        parent=project_path, conversation=conversation
+    )
+
+    print("Life Cycle State: {}".format(response.lifecycle_state))
+    print("Conversation Profile Name: {}".format(response.conversation_profile))
+    print("Name: {}".format(response.name))
     return response
 
 
 # [END dialogflow_create_conversation]
 
 
 # [START dialogflow_get_conversation]
@@ -57,18 +57,17 @@
         conversation_id: Id of the conversation."""
 
     client = dialogflow.ConversationsClient()
     conversation_path = client.conversation_path(project_id, conversation_id)
 
     response = client.get_conversation(name=conversation_path)
 
-    print('Life Cycle State: {}'.format(response.lifecycle_state))
-    print('Conversation Profile Name: {}'.format(
-        response.conversation_profile))
-    print('Name: {}'.format(response.name))
+    print("Life Cycle State: {}".format(response.lifecycle_state))
+    print("Conversation Profile Name: {}".format(response.conversation_profile))
+    print("Name: {}".format(response.name))
     return response
 
 
 # [END dialogflow_get_conversation]
 
 
 # [START dialogflow_complete_conversation]
@@ -78,16 +77,15 @@
     Args:
         project_id: The GCP project linked with the conversation.
         conversation_id: Id of the conversation."""
 
     client = dialogflow.ConversationsClient()
     conversation_path = client.conversation_path(project_id, conversation_id)
     conversation = client.complete_conversation(name=conversation_path)
-    print('Completed Conversation.')
-    print('Life Cycle State: {}'.format(conversation.lifecycle_state))
-    print('Conversation Profile Name: {}'.format(
-        conversation.conversation_profile))
-    print('Name: {}'.format(conversation.name))
+    print("Completed Conversation.")
+    print("Life Cycle State: {}".format(conversation.lifecycle_state))
+    print("Conversation Profile Name: {}".format(conversation.conversation_profile))
+    print("Name: {}".format(conversation.name))
     return conversation
 
 
 # [END dialogflow_complete_conversation]
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/conversation_profile_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/conversation_profile_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,159 +25,143 @@
 
     Args: project_id: The GCP project linked with the conversation profile."""
 
     client = dialogflow.ConversationProfilesClient()
     project_path = client.common_project_path(project_id)
     response = client.list_conversation_profiles(parent=project_path)
     for conversation_profile in response:
-        print('Display Name: {}'.format(conversation_profile.display_name))
-        print('Name: {}'.format(conversation_profile.name))
+        print("Display Name: {}".format(conversation_profile.display_name))
+        print("Name: {}".format(conversation_profile.name))
     return response
 
 
 # [END dialogflow_list_conversation_profiles]
 
 
 # [START dialogflow_create_conversation_profile_article_faq]
 def create_conversation_profile_article_faq(
-        project_id,
-        display_name,
-        article_suggestion_knowledge_base_id=None,
-        faq_knowledge_base_id=None):
+    project_id,
+    display_name,
+    article_suggestion_knowledge_base_id=None,
+    faq_knowledge_base_id=None,
+):
     """Creates a conversation profile with given values
 
     Args: project_id:  The GCP project linked with the conversation profile.
         display_name: The display name for the conversation profile to be
         created.
         article_suggestion_knowledge_base_id: knowledge base id for article
         suggestion.
         faq_knowledge_base_id: knowledge base id for faq."""
 
     client = dialogflow.ConversationProfilesClient()
     project_path = client.common_project_path(project_id)
 
     conversation_profile = {
-        'display_name': display_name,
-        'human_agent_assistant_config': {
-            'human_agent_suggestion_config': {
-                'feature_configs': []
-            }
+        "display_name": display_name,
+        "human_agent_assistant_config": {
+            "human_agent_suggestion_config": {"feature_configs": []}
         },
-        'language_code': 'en-US'
+        "language_code": "en-US",
     }
 
     if article_suggestion_knowledge_base_id is not None:
         as_kb_path = dialogflow.KnowledgeBasesClient.knowledge_base_path(
-            project_id, article_suggestion_knowledge_base_id)
+            project_id, article_suggestion_knowledge_base_id
+        )
         feature_config = {
-            'suggestion_feature': {
-                'type_': 'ARTICLE_SUGGESTION'
-            },
-            'suggestion_trigger_settings': {
-                'no_small_talk': True,
-                'only_end_user': True,
-            },
-            'query_config': {
-                'knowledge_base_query_source': {
-                    'knowledge_bases': [as_kb_path]
-                },
-                'max_results': 3
+            "suggestion_feature": {"type_": "ARTICLE_SUGGESTION"},
+            "suggestion_trigger_settings": {
+                "no_small_talk": True,
+                "only_end_user": True,
+            },
+            "query_config": {
+                "knowledge_base_query_source": {"knowledge_bases": [as_kb_path]},
+                "max_results": 3,
             },
         }
-        conversation_profile['human_agent_assistant_config'][
-            'human_agent_suggestion_config']['feature_configs'].append(
-                feature_config)
+        conversation_profile["human_agent_assistant_config"][
+            "human_agent_suggestion_config"
+        ]["feature_configs"].append(feature_config)
     if faq_knowledge_base_id is not None:
         faq_kb_path = dialogflow.KnowledgeBasesClient.knowledge_base_path(
-            project_id, faq_knowledge_base_id)
+            project_id, faq_knowledge_base_id
+        )
         feature_config = {
-            'suggestion_feature': {
-                'type_': 'FAQ'
-            },
-            'suggestion_trigger_settings': {
-                'no_small_talk': True,
-                'only_end_user': True,
-            },
-            'query_config': {
-                'knowledge_base_query_source': {
-                    'knowledge_bases': [faq_kb_path]
-                },
-                'max_results': 3
+            "suggestion_feature": {"type_": "FAQ"},
+            "suggestion_trigger_settings": {
+                "no_small_talk": True,
+                "only_end_user": True,
+            },
+            "query_config": {
+                "knowledge_base_query_source": {"knowledge_bases": [faq_kb_path]},
+                "max_results": 3,
             },
         }
-        conversation_profile['human_agent_assistant_config'][
-            'human_agent_suggestion_config']['feature_configs'].append(
-                feature_config)
+        conversation_profile["human_agent_assistant_config"][
+            "human_agent_suggestion_config"
+        ]["feature_configs"].append(feature_config)
 
     response = client.create_conversation_profile(
-        parent=project_path, conversation_profile=conversation_profile)
+        parent=project_path, conversation_profile=conversation_profile
+    )
 
-    print('Conversation Profile created:')
-    print('Display Name: {}'.format(response.display_name))
+    print("Conversation Profile created:")
+    print("Display Name: {}".format(response.display_name))
     # Put Name is the last to make it easier to retrieve.
-    print('Name: {}'.format(response.name))
+    print("Name: {}".format(response.name))
     return response
 
 
 # [END dialogflow_create_conversation_profile_article_faq]
 
 
 # [START dialogflow_create_conversation_profile_smart_reply]
-def create_conversation_profile_smart_reply(project_id, display_name,
-                                            smart_reply_allowlist_name,
-                                            smart_reply_model_name):
+def create_conversation_profile_smart_reply(
+    project_id, display_name, smart_reply_allowlist_name, smart_reply_model_name
+):
     """Creates a conversation profile with given values for smart reply
 
     Args: project_id:  The GCP project linked with the conversation profile.
         display_name: The display name for the conversation profile to be
         created.
         smart_reply_allowlist_name: document name for smart reply allowlist.
         smart_reply_model_name: conversation model name for smart reply."""
 
     client = dialogflow.ConversationProfilesClient()
     project_path = client.common_project_path(project_id)
 
     conversation_profile = {
-        'display_name': display_name,
-        'human_agent_assistant_config': {
-            'human_agent_suggestion_config': {
-                'feature_configs': []
-            }
+        "display_name": display_name,
+        "human_agent_assistant_config": {
+            "human_agent_suggestion_config": {"feature_configs": []}
         },
-        'language_code': 'en-US'
+        "language_code": "en-US",
     }
     feature_config = {
-        'suggestion_feature': {
-            'type_': 'SMART_REPLY'
+        "suggestion_feature": {"type_": "SMART_REPLY"},
+        "suggestion_trigger_settings": {"no_small_talk": True, "only_end_user": True, },
+        "query_config": {
+            "document_query_source": {"documents": [smart_reply_allowlist_name]},
+            "max_results": 3,
         },
-        'suggestion_trigger_settings': {
-            'no_small_talk': True,
-            'only_end_user': True,
-        },
-        'query_config': {
-            'document_query_source': {
-                'documents': [smart_reply_allowlist_name]
-            },
-            'max_results': 3
-        },
-        'conversation_model_config': {
-            'model': smart_reply_model_name
-        }
+        "conversation_model_config": {"model": smart_reply_model_name},
     }
-    conversation_profile['human_agent_assistant_config'][
-        'human_agent_suggestion_config']['feature_configs'].append(
-            feature_config)
+    conversation_profile["human_agent_assistant_config"][
+        "human_agent_suggestion_config"
+    ]["feature_configs"].append(feature_config)
 
     response = client.create_conversation_profile(
-        parent=project_path, conversation_profile=conversation_profile)
+        parent=project_path, conversation_profile=conversation_profile
+    )
 
-    print('Conversation Profile created:')
-    print('Display Name: {}'.format(response.display_name))
+    print("Conversation Profile created:")
+    print("Display Name: {}".format(response.display_name))
     # Put Name is the last to make it easier to retrieve.
-    print('Name: {}'.format(response.name))
+    print("Name: {}".format(response.name))
     return response
 
 
 # [END dialogflow_create_conversation_profile_smart_reply]
 
 
 # [START dialogflow_get_conversation_profile]
@@ -185,21 +169,22 @@
     """Gets a specific conversation profile.
 
     Args: project_id: The GCP project linked with the conversation profile.
         conversation_profile_id: Id of the conversation profile."""
 
     client = dialogflow.ConversationProfilesClient()
     conversation_profile_path = client.conversation_profile_path(
-        project_id, conversation_profile_id)
+        project_id, conversation_profile_id
+    )
 
     response = client.get_conversation_profile(name=conversation_profile_path)
 
-    print('Got conversation profile:')
-    print('Display Name: {}'.format(response.display_name))
-    print('Name: {}'.format(response.name))
+    print("Got conversation profile:")
+    print("Display Name: {}".format(response.display_name))
+    print("Name: {}".format(response.name))
     return response
 
 
 # [END dialogflow_get_conversation_profile]
 
 
 # [START dialogflow_delete_conversation_profile]
@@ -207,15 +192,16 @@
     """Deletes a specific conversation profile.
 
     Args: project_id: The GCP project linked with the conversation profile.
         conversation_profile_id: Id of the conversation profile."""
 
     client = dialogflow.ConversationProfilesClient()
     conversation_profile_path = client.conversation_profile_path(
-        project_id, conversation_profile_id)
+        project_id, conversation_profile_id
+    )
 
     client.delete_conversation_profile(name=conversation_profile_path)
 
-    print('Conversation Profile deleted.')
+    print("Conversation Profile deleted.")
 
 
 # [END dialogflow_delete_conversation_profile]
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/conversation_profile_management_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/conversation_profile_management_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,54 +14,54 @@
 
 from __future__ import absolute_import
 
 import os
 
 import conversation_profile_management
 
-PROJECT_ID = os.getenv('GOOGLE_CLOUD_PROJECT')
+PROJECT_ID = os.getenv("GOOGLE_CLOUD_PROJECT")
 
-CONVERSATION_PROFILE_DISPLAY_NAME = 'fake_conversation_profile_name'
+CONVERSATION_PROFILE_DISPLAY_NAME = "fake_conversation_profile_name"
 
 
 def test_create_conversation_profile(capsys):
     # Check the conversation profile does not yet exists.
     conversation_profile_management.list_conversation_profiles(PROJECT_ID)
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(
-        CONVERSATION_PROFILE_DISPLAY_NAME) not in out
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) not in out
 
     # Create a conversation profile.
     conversation_profile_management.create_conversation_profile_article_faq(
-        project_id=PROJECT_ID, display_name=CONVERSATION_PROFILE_DISPLAY_NAME,
-        article_suggestion_knowledge_base_id='abc')
+        project_id=PROJECT_ID,
+        display_name=CONVERSATION_PROFILE_DISPLAY_NAME,
+        article_suggestion_knowledge_base_id="abc",
+    )
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(
-        CONVERSATION_PROFILE_DISPLAY_NAME) in out
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
 
-    conversation_profile_id = out.split('conversationProfiles/')[1].rstrip()
+    conversation_profile_id = out.split("conversationProfiles/")[1].rstrip()
 
     # List conversation profiles.
     conversation_profile_management.list_conversation_profiles(PROJECT_ID)
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(
-        CONVERSATION_PROFILE_DISPLAY_NAME) in out
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
 
     # Get the conversation profile.
     conversation_profile_management.get_conversation_profile(
-        PROJECT_ID, conversation_profile_id)
+        PROJECT_ID, conversation_profile_id
+    )
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
 
     # Delete the conversation profile.
     conversation_profile_management.delete_conversation_profile(
-        PROJECT_ID, conversation_profile_id)
+        PROJECT_ID, conversation_profile_id
+    )
 
     # Verify the conversation profile is deleted.
     conversation_profile_management.list_conversation_profiles(PROJECT_ID)
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(
-        CONVERSATION_PROFILE_DISPLAY_NAME) not in out
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) not in out
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/create_document_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/create_document_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,26 +31,28 @@
 
 @pytest.fixture(scope="function", autouse=True)
 def setup_teardown():
     # Create a knowledge base to use in document management
     client = dialogflow.KnowledgeBasesClient()
     project_path = client.common_project_path(PROJECT_ID)
     knowledge_base = dialogflow.KnowledgeBase(display_name=KNOWLEDGE_BASE_NAME)
-    response = client.create_knowledge_base(parent=project_path,
-                                            knowledge_base=knowledge_base)
-    pytest.KNOWLEDGE_BASE_ID = response.name.split(
-        "/knowledgeBases/")[1].split("\n")[0]
+    response = client.create_knowledge_base(
+        parent=project_path, knowledge_base=knowledge_base
+    )
+    pytest.KNOWLEDGE_BASE_ID = response.name.split("/knowledgeBases/")[1].split("\n")[0]
 
     yield
 
     # Delete the created knowledge base
-    knowledge_base_path = client.knowledge_base_path(PROJECT_ID,
-                                                     pytest.KNOWLEDGE_BASE_ID)
-    request = dialogflow.DeleteKnowledgeBaseRequest(name=knowledge_base_path,
-                                                    force=True)
+    knowledge_base_path = client.knowledge_base_path(
+        PROJECT_ID, pytest.KNOWLEDGE_BASE_ID
+    )
+    request = dialogflow.DeleteKnowledgeBaseRequest(
+        name=knowledge_base_path, force=True
+    )
     client.delete_knowledge_base(request=request)
 
 
 @pytest.mark.flaky(max_runs=3, min_passes=1)
 def test_create_document(capsys):
     document_management.create_document(
         PROJECT_ID,
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/create_knowledge_base_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/create_knowledge_base_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_audio.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,15 @@
         audio_encoding=audio_encoding,
         language_code=language_code,
         sample_rate_hertz=sample_rate_hertz,
     )
     query_input = dialogflow.QueryInput(audio_config=audio_config)
 
     request = dialogflow.DetectIntentRequest(
-        session=session,
-        query_input=query_input,
-        input_audio=input_audio,
+        session=session, query_input=query_input, input_audio=input_audio,
     )
     response = session_client.detect_intent(request=request)
 
     print("=" * 20)
     print("Query text: {}".format(response.query_result.query_text))
     print(
         "Detected intent: {} (confidence: {})\n".format(
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_audio_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_audio_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_knowledge.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_knowledge.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_knowledge_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_knowledge_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_stream.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_stream.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_stream_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_stream_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_with_location.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_with_location.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_texts_with_location_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_texts_with_location_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_sentiment_analysis.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_sentiment_analysis_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_sentiment_analysis_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_texttospeech_response.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_texttospeech_response.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/detect_intent_with_texttospeech_response_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/detect_intent_with_texttospeech_response_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/document_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/document_management.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,189 +32,217 @@
   --knowledge-base-id knowledge_base_id \
   delete --document-id DOCUMENT_ID
 """
 
 import argparse
 
 
-KNOWLEDGE_TYPES = ['KNOWLEDGE_TYPE_UNSPECIFIED', 'FAQ', 'EXTRACTIVE_QA', 'ARTICLE_SUGGESTION']
+KNOWLEDGE_TYPES = [
+    "KNOWLEDGE_TYPE_UNSPECIFIED",
+    "FAQ",
+    "EXTRACTIVE_QA",
+    "ARTICLE_SUGGESTION",
+]
 
 
 # [START dialogflow_list_document]
 def list_documents(project_id, knowledge_base_id):
     """Lists the Documents belonging to a Knowledge base.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.DocumentsClient()
     knowledge_base_path = dialogflow.KnowledgeBasesClient.knowledge_base_path(
-        project_id, knowledge_base_id)
+        project_id, knowledge_base_id
+    )
 
-    print('Documents for Knowledge Id: {}'.format(knowledge_base_id))
+    print("Documents for Knowledge Id: {}".format(knowledge_base_id))
     response = client.list_documents(parent=knowledge_base_path)
     for document in response:
-        print(' - Display Name: {}'.format(document.display_name))
-        print(' - Knowledge ID: {}'.format(document.name))
-        print(' - MIME Type: {}'.format(document.mime_type))
-        print(' - Knowledge Types:')
+        print(" - Display Name: {}".format(document.display_name))
+        print(" - Knowledge ID: {}".format(document.name))
+        print(" - MIME Type: {}".format(document.mime_type))
+        print(" - Knowledge Types:")
         for knowledge_type in document.knowledge_types:
-            print('    - {}'.format(KNOWLEDGE_TYPES[knowledge_type]))
-        print(' - Source: {}\n'.format(document.content_uri))
+            print("    - {}".format(KNOWLEDGE_TYPES[knowledge_type]))
+        print(" - Source: {}\n".format(document.content_uri))
     return response
+
+
 # [END dialogflow_list_document]
 
 
 # [START dialogflow_create_document]]
-def create_document(project_id, knowledge_base_id, display_name, mime_type,
-                    knowledge_type, content_uri):
+def create_document(
+    project_id, knowledge_base_id, display_name, mime_type, knowledge_type, content_uri
+):
     """Creates a Document.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base.
         display_name: The display name of the Document.
         mime_type: The mime_type of the Document. e.g. text/csv, text/html,
             text/plain, text/pdf etc.
         knowledge_type: The Knowledge type of the Document. e.g. FAQ,
             EXTRACTIVE_QA.
         content_uri: Uri of the document, e.g. gs://path/mydoc.csv,
             http://mypage.com/faq.html."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.DocumentsClient()
     knowledge_base_path = dialogflow.KnowledgeBasesClient.knowledge_base_path(
-        project_id, knowledge_base_id)
+        project_id, knowledge_base_id
+    )
 
     document = dialogflow.Document(
-        display_name=display_name, mime_type=mime_type,
-        content_uri=content_uri)
+        display_name=display_name, mime_type=mime_type, content_uri=content_uri
+    )
 
     document.knowledge_types.append(
         getattr(dialogflow.Document.KnowledgeType, knowledge_type)
     )
 
     response = client.create_document(parent=knowledge_base_path, document=document)
-    print('Waiting for results...')
+    print("Waiting for results...")
     document = response.result(timeout=120)
-    print('Created Document:')
-    print(' - Display Name: {}'.format(document.display_name))
-    print(' - Knowledge ID: {}'.format(document.name))
-    print(' - MIME Type: {}'.format(document.mime_type))
-    print(' - Knowledge Types:')
+    print("Created Document:")
+    print(" - Display Name: {}".format(document.display_name))
+    print(" - Knowledge ID: {}".format(document.name))
+    print(" - MIME Type: {}".format(document.mime_type))
+    print(" - Knowledge Types:")
     for knowledge_type in document.knowledge_types:
-        print('    - {}'.format(KNOWLEDGE_TYPES[knowledge_type]))
-    print(' - Source: {}\n'.format(document.content_uri))
+        print("    - {}".format(KNOWLEDGE_TYPES[knowledge_type]))
+    print(" - Source: {}\n".format(document.content_uri))
+
+
 # [END dialogflow_create_document]
 
 
 # [START dialogflow_get_document]]
 def get_document(project_id, knowledge_base_id, document_id):
     """Gets a Document.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base.
         document_id: Id of the Document."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.DocumentsClient()
-    document_path = client.document_path(project_id, knowledge_base_id,
-                                         document_id)
+    document_path = client.document_path(project_id, knowledge_base_id, document_id)
 
     response = client.get_document(name=document_path)
-    print('Got Document:')
-    print(' - Display Name: {}'.format(response.display_name))
-    print(' - Knowledge ID: {}'.format(response.name))
-    print(' - MIME Type: {}'.format(response.mime_type))
-    print(' - Knowledge Types:')
+    print("Got Document:")
+    print(" - Display Name: {}".format(response.display_name))
+    print(" - Knowledge ID: {}".format(response.name))
+    print(" - MIME Type: {}".format(response.mime_type))
+    print(" - Knowledge Types:")
     for knowledge_type in response.knowledge_types:
-        print('    - {}'.format(KNOWLEDGE_TYPES[knowledge_type]))
-    print(' - Source: {}\n'.format(response.content_uri))
+        print("    - {}".format(KNOWLEDGE_TYPES[knowledge_type]))
+    print(" - Source: {}\n".format(response.content_uri))
     return response
+
+
 # [END dialogflow_get_document]]
 
 
 # [START dialogflow_delete_document]]
 def delete_document(project_id, knowledge_base_id, document_id):
     """Deletes a Document.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base.
         document_id: Id of the Document."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.DocumentsClient()
-    document_path = client.document_path(project_id, knowledge_base_id,
-                                         document_id)
+    document_path = client.document_path(project_id, knowledge_base_id, document_id)
 
     response = client.delete_document(name=document_path)
-    print('operation running:\n {}'.format(response.operation))
-    print('Waiting for results...')
-    print('Done.\n {}'.format(response.result()))
+    print("operation running:\n {}".format(response.operation))
+    print("Waiting for results...")
+    print("Done.\n {}".format(response.result()))
+
+
 # [END dialogflow_delete_document]]
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument(
-        '--project-id', help='Project id.  Required.', required=True)
+        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
+    )
+    parser.add_argument("--project-id", help="Project id.  Required.", required=True)
     parser.add_argument(
-        '--knowledge-base-id',
-        help='The id of the Knowledge Base that the Document belongs to',
-        required=True)
+        "--knowledge-base-id",
+        help="The id of the Knowledge Base that the Document belongs to",
+        required=True,
+    )
 
-    subparsers = parser.add_subparsers(dest='command')
+    subparsers = parser.add_subparsers(dest="command")
 
     list_parser = subparsers.add_parser(
-        'list',
-        help='List all Documents that belong to a certain Knowledge base.')
+        "list", help="List all Documents that belong to a certain Knowledge base."
+    )
 
     create_parser = subparsers.add_parser(
-        'create', help='Create a Document for a certain Knowledge base.')
+        "create", help="Create a Document for a certain Knowledge base."
+    )
     create_parser.add_argument(
-        '--display-name',
-        help='A name of the Document, mainly used for display purpose, '
-             'can not be used to identify the Document.',
-        default=str(''))
+        "--display-name",
+        help="A name of the Document, mainly used for display purpose, "
+        "can not be used to identify the Document.",
+        default=str(""),
+    )
     create_parser.add_argument(
-        '--mime-type',
-        help='The mime-type of the Document, e.g. text/csv, text/html, '
-             'text/plain, text/pdf etc. ',
-        required=True)
+        "--mime-type",
+        help="The mime-type of the Document, e.g. text/csv, text/html, "
+        "text/plain, text/pdf etc. ",
+        required=True,
+    )
     create_parser.add_argument(
-        '--knowledge-type',
-        help='The knowledge-type of the Document, e.g. FAQ, EXTRACTIVE_QA.',
-        required=True)
+        "--knowledge-type",
+        help="The knowledge-type of the Document, e.g. FAQ, EXTRACTIVE_QA.",
+        required=True,
+    )
     create_parser.add_argument(
-        '--content-uri',
-        help='The uri of the Document, e.g. gs://path/mydoc.csv, '
-             'http://mypage.com/faq.html',
-        required=True)
+        "--content-uri",
+        help="The uri of the Document, e.g. gs://path/mydoc.csv, "
+        "http://mypage.com/faq.html",
+        required=True,
+    )
 
     get_parser = subparsers.add_parser(
-        'get', help='Get a Document by its id and the Knowledge base id.')
+        "get", help="Get a Document by its id and the Knowledge base id."
+    )
     get_parser.add_argument(
-        '--document-id', help='The id of the Document', required=True)
+        "--document-id", help="The id of the Document", required=True
+    )
 
     delete_parser = subparsers.add_parser(
-        'delete', help='Delete a Document by its id and the Knowledge base'
-                       'id.')
+        "delete", help="Delete a Document by its id and the Knowledge base" "id."
+    )
     delete_parser.add_argument(
-        '--document-id',
-        help='The id of the Document you want to delete',
-        required=True)
+        "--document-id", help="The id of the Document you want to delete", required=True
+    )
 
     args = parser.parse_args()
 
-    if args.command == 'list':
+    if args.command == "list":
         list_documents(args.project_id, args.knowledge_base_id)
-    elif args.command == 'create':
-        create_document(args.project_id, args.knowledge_base_id,
-                        args.display_name, args.mime_type, args.knowledge_type,
-                        args.content_uri)
-    elif args.command == 'get':
+    elif args.command == "create":
+        create_document(
+            args.project_id,
+            args.knowledge_base_id,
+            args.display_name,
+            args.mime_type,
+            args.knowledge_type,
+            args.content_uri,
+        )
+    elif args.command == "get":
         get_document(args.project_id, args.knowledge_base_id, args.document_id)
-    elif args.command == 'delete':
-        delete_document(args.project_id, args.knowledge_base_id,
-                        args.document_id)
+    elif args.command == "delete":
+        delete_document(args.project_id, args.knowledge_base_id, args.document_id)
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/intent_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/intent_management.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/intent_management_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/intent_management_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/knowledge_base_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/knowledge_base_management.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,104 +35,110 @@
 def create_knowledge_base(project_id, display_name):
     """Creates a Knowledge base.
 
     Args:
         project_id: The GCP project linked with the agent.
         display_name: The display name of the Knowledge base."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.KnowledgeBasesClient()
     project_path = client.common_project_path(project_id)
 
-    knowledge_base = dialogflow.KnowledgeBase(
-        display_name=display_name)
+    knowledge_base = dialogflow.KnowledgeBase(display_name=display_name)
 
     response = client.create_knowledge_base(
-        parent=project_path,
-        knowledge_base=knowledge_base
+        parent=project_path, knowledge_base=knowledge_base
     )
 
-    print('Knowledge Base created:\n')
-    print('Display Name: {}\n'.format(response.display_name))
-    print('Knowledge ID: {}\n'.format(response.name))
+    print("Knowledge Base created:\n")
+    print("Display Name: {}\n".format(response.display_name))
+    print("Knowledge ID: {}\n".format(response.name))
+
+
 # [END dialogflow_create_knowledge_base]
 
 
 # [START dialogflow_get_knowledge_base]
 def get_knowledge_base(project_id, knowledge_base_id):
     """Gets a specific Knowledge base.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.KnowledgeBasesClient()
-    knowledge_base_path = client.knowledge_base_path(
-        project_id, knowledge_base_id)
+    knowledge_base_path = client.knowledge_base_path(project_id, knowledge_base_id)
 
     response = client.get_knowledge_base(name=knowledge_base_path)
 
-    print('Got Knowledge Base:')
-    print(' - Display Name: {}'.format(response.display_name))
-    print(' - Knowledge ID: {}'.format(response.name))
+    print("Got Knowledge Base:")
+    print(" - Display Name: {}".format(response.display_name))
+    print(" - Knowledge ID: {}".format(response.name))
     return response
+
+
 # [END dialogflow_get_knowledge_base]
 
 
 # [START dialogflow_delete_knowledge_base]
 def delete_knowledge_base(project_id, knowledge_base_id):
     """Deletes a specific Knowledge base.
 
     Args:
         project_id: The GCP project linked with the agent.
         knowledge_base_id: Id of the Knowledge base."""
     from google.cloud import dialogflow_v2beta1 as dialogflow
+
     client = dialogflow.KnowledgeBasesClient()
-    knowledge_base_path = client.knowledge_base_path(
-        project_id, knowledge_base_id)
+    knowledge_base_path = client.knowledge_base_path(project_id, knowledge_base_id)
 
     client.delete_knowledge_base(name=knowledge_base_path)
 
-    print('Knowledge Base deleted.')
+    print("Knowledge Base deleted.")
+
+
 # [END dialogflow_delete_knowledge_base]
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument(
-        '--project-id', help='Project/agent id.', required=True)
+        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
+    )
+    parser.add_argument("--project-id", help="Project/agent id.", required=True)
 
-    subparsers = parser.add_subparsers(dest='command')
+    subparsers = parser.add_subparsers(dest="command")
 
     list_parser = subparsers.add_parser(
-        'list', help='List all Knowledge bases that belong to the project.')
+        "list", help="List all Knowledge bases that belong to the project."
+    )
 
-    create_parser = subparsers.add_parser(
-        'create', help='Create a new Knowledge base.')
+    create_parser = subparsers.add_parser("create", help="Create a new Knowledge base.")
     create_parser.add_argument(
-        '--display-name',
-        help='A name of the Knowledge base, used for display purpose, '
-             'can not be used to identify the Knowledge base.',
-        default=str(''))
+        "--display-name",
+        help="A name of the Knowledge base, used for display purpose, "
+        "can not be used to identify the Knowledge base.",
+        default=str(""),
+    )
 
-    get_parser = subparsers.add_parser(
-        'get', help='Get a Knowledge base by its id.')
+    get_parser = subparsers.add_parser("get", help="Get a Knowledge base by its id.")
     get_parser.add_argument(
-        '--knowledge-base-id', help='The id of the Knowledge base.',
-        required=True)
+        "--knowledge-base-id", help="The id of the Knowledge base.", required=True
+    )
 
     delete_parser = subparsers.add_parser(
-        'delete', help='Delete a Knowledge base by its id.')
+        "delete", help="Delete a Knowledge base by its id."
+    )
     delete_parser.add_argument(
-        '--knowledge-base-id',
-        help='The id of the Knowledge base you want to delete.',
-        required=True)
+        "--knowledge-base-id",
+        help="The id of the Knowledge base you want to delete.",
+        required=True,
+    )
 
     args = parser.parse_args()
 
-    if args.command == 'create':
+    if args.command == "create":
         create_knowledge_base(args.project_id, args.display_name)
-    elif args.command == 'get':
+    elif args.command == "get":
         get_knowledge_base(args.project_id, args.knowledge_base_id)
-    elif args.command == 'delete':
+    elif args.command == "delete":
         delete_knowledge_base(args.project_id, args.knowledge_base_id)
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/noxfile.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/noxfile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/participant_management.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/participant_management.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/participant_management_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/participant_management_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,129 +16,140 @@
 
 import conversation_management
 import conversation_profile_management
 import document_management
 import knowledge_base_management
 import participant_management
 
-PROJECT_ID = os.getenv('GOOGLE_CLOUD_PROJECT')
-KNOWLEDGE_BASE_DISPLAY_NAME = 'fake_KNOWLEDGE_BASE_DISPLAY_NAME'
-DOCUMENT_DISPLAY_NAME = 'Cancel an order'
-CONVERSATION_PROFILE_DISPLAY_NAME = 'fake_conversation_profile'
+PROJECT_ID = os.getenv("GOOGLE_CLOUD_PROJECT")
+KNOWLEDGE_BASE_DISPLAY_NAME = "fake_KNOWLEDGE_BASE_DISPLAY_NAME"
+DOCUMENT_DISPLAY_NAME = "Cancel an order"
+CONVERSATION_PROFILE_DISPLAY_NAME = "fake_conversation_profile"
 
 
 def test_analyze_content_text(capsys):
     """Test analyze content api with text only messages.
     """
     # Create knowledge base.
     knowledge_base_management.create_knowledge_base(
-        PROJECT_ID, KNOWLEDGE_BASE_DISPLAY_NAME)
+        PROJECT_ID, KNOWLEDGE_BASE_DISPLAY_NAME
+    )
     out, _ = capsys.readouterr()
-    knowledge_base_id = out.split('knowledgeBases/')[1].rstrip()
+    knowledge_base_id = out.split("knowledgeBases/")[1].rstrip()
     # Get the knowledge base
     knowledge_base_management.get_knowledge_base(PROJECT_ID, knowledge_base_id)
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(KNOWLEDGE_BASE_DISPLAY_NAME) in out
+    assert "Display Name: {}".format(KNOWLEDGE_BASE_DISPLAY_NAME) in out
 
     # Create documents. Note that you should get read permission of bucket gs://cloud-samples-data/dialogflow/participant_test.html
     # via Pantheon for service account (google application credential account) from here:
     # https://support.google.com/googleshopping/answer/9116497
-    document_management.create_document(PROJECT_ID, knowledge_base_id,
-                                        DOCUMENT_DISPLAY_NAME, 'text/html',
-                                        'ARTICLE_SUGGESTION',
-                                        'gs://cloud-samples-data/dialogflow/participant_test.html')
+    document_management.create_document(
+        PROJECT_ID,
+        knowledge_base_id,
+        DOCUMENT_DISPLAY_NAME,
+        "text/html",
+        "ARTICLE_SUGGESTION",
+        "gs://cloud-samples-data/dialogflow/participant_test.html",
+    )
     out, _ = capsys.readouterr()
-    document_id = out.split('documents/')[1].split(' - MIME Type:')[0].rstrip()
+    document_id = out.split("documents/")[1].split(" - MIME Type:")[0].rstrip()
 
     # Get the Document
-    document_management.get_document(PROJECT_ID, knowledge_base_id,
-                                     document_id)
+    document_management.get_document(PROJECT_ID, knowledge_base_id, document_id)
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(DOCUMENT_DISPLAY_NAME) in out
+    assert "Display Name: {}".format(DOCUMENT_DISPLAY_NAME) in out
 
     # Create conversation profile.
     conversation_profile_management.create_conversation_profile_article_faq(
         project_id=PROJECT_ID,
         display_name=CONVERSATION_PROFILE_DISPLAY_NAME,
-        article_suggestion_knowledge_base_id=knowledge_base_id)
+        article_suggestion_knowledge_base_id=knowledge_base_id,
+    )
 
     out, _ = capsys.readouterr()
-    assert 'Display Name: {}'.format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
-    conversation_profile_id = out.split('conversationProfiles/')[1].rstrip()
+    assert "Display Name: {}".format(CONVERSATION_PROFILE_DISPLAY_NAME) in out
+    conversation_profile_id = out.split("conversationProfiles/")[1].rstrip()
 
     # Create conversation.
     conversation_management.create_conversation(
-        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id)
+        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id
+    )
 
     out, _ = capsys.readouterr()
-    conversation_id = out.split('conversations/')[1].rstrip()
+    conversation_id = out.split("conversations/")[1].rstrip()
 
     # Create end user participant.
-    participant_management.create_participant(project_id=PROJECT_ID,
-                                              conversation_id=conversation_id,
-                                              role='END_USER')
+    participant_management.create_participant(
+        project_id=PROJECT_ID, conversation_id=conversation_id, role="END_USER"
+    )
     out, _ = capsys.readouterr()
-    end_user_id = out.split('participants/')[1].rstrip()
+    end_user_id = out.split("participants/")[1].rstrip()
 
     # Create human agent participant.
-    participant_management.create_participant(project_id=PROJECT_ID,
-                                              conversation_id=conversation_id,
-                                              role='HUMAN_AGENT')
+    participant_management.create_participant(
+        project_id=PROJECT_ID, conversation_id=conversation_id, role="HUMAN_AGENT"
+    )
     out, _ = capsys.readouterr()
-    human_agent_id = out.split('participants/')[1].rstrip()
+    human_agent_id = out.split("participants/")[1].rstrip()
 
     # AnalyzeContent
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=human_agent_id,
-        text='Hi, how are you?')
+        text="Hi, how are you?",
+    )
     out, _ = capsys.readouterr()
 
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=end_user_id,
-        text='Hi, I am doing well, how about you?')
+        text="Hi, I am doing well, how about you?",
+    )
     out, _ = capsys.readouterr()
 
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=human_agent_id,
-        text='Great. How can I help you?')
+        text="Great. How can I help you?",
+    )
     out, _ = capsys.readouterr()
 
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=end_user_id,
-        text='So I ordered something, but I do not like it.')
+        text="So I ordered something, but I do not like it.",
+    )
     out, _ = capsys.readouterr()
 
     participant_management.analyze_content_text(
         project_id=PROJECT_ID,
         conversation_id=conversation_id,
         participant_id=end_user_id,
-        text='Thinking if I can cancel that order')
+        text="Thinking if I can cancel that order",
+    )
     suggestion_out, _ = capsys.readouterr()
     # Currently suggestion_out won't contain the suggestion we want since it
     # takes time for document to be ready to serve.
     # assert 'Cancel an order' in suggestion_out
 
     # Complete conversation.
     conversation_management.complete_conversation(
-        project_id=PROJECT_ID, conversation_id=conversation_id)
+        project_id=PROJECT_ID, conversation_id=conversation_id
+    )
 
     # Delete conversation profile.
     conversation_profile_management.delete_conversation_profile(
-        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id)
+        project_id=PROJECT_ID, conversation_profile_id=conversation_profile_id
+    )
 
     # Delete document.
-    document_management.delete_document(PROJECT_ID, knowledge_base_id,
-                                        document_id)
+    document_management.delete_document(PROJECT_ID, knowledge_base_id, document_id)
 
     # Delete the Knowledge Base.
-    knowledge_base_management.delete_knowledge_base(PROJECT_ID,
-                                                    knowledge_base_id)
+    knowledge_base_management.delete_knowledge_base(PROJECT_ID, knowledge_base_id)
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/set_agent.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/set_agent.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/set_agent_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/set_agent_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/update_intent.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/update_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,10 @@
     intent_name = intents_client.intent_path(project_id, intent_id)
     intent = intents_client.get_intent(request={"name": intent_name})
 
     intent.display_name = display_name
     update_mask = field_mask_pb2.FieldMask(paths=["display_name"])
     response = intents_client.update_intent(intent=intent, update_mask=update_mask)
     return response
+
+
 # [END dialogflow_es_update_intent]
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/update_intent_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/update_intent_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     parent = AgentsClient.agent_path(project_id)
 
     intent = Intent()
 
     intent.display_name = "fake_intent"
 
-    intents = intents_client.create_intent(request={"parent": parent,  "intent": intent})
+    intents = intents_client.create_intent(request={"parent": parent, "intent": intent})
 
     return intents.name.split("/")[4]
 
 
 @pytest.fixture(scope="function", autouse=True)
 def setup_teardown():
     pytest.INTENT_ID = create_intent(project_id=PROJECT_ID)
```

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/webhook.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/webhook.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/samples/snippets/webhook_test.py` & `google-cloud-dialogflow-2.9.1/samples/snippets/webhook_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/scripts/fixup_dialogflow_v2_keywords.py` & `google-cloud-dialogflow-2.9.1/scripts/fixup_dialogflow_v2_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/scripts/fixup_dialogflow_v2beta1_keywords.py` & `google-cloud-dialogflow-2.9.1/scripts/fixup_dialogflow_v2beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/setup.py` & `google-cloud-dialogflow-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import io
 import os
 
 import setuptools
 
 name = "dialogflow"
 description = "Client library for the Dialogflow API"
-version = "2.9.0"
+version = "2.9.1"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.26.0, <3.0.0dev",
     "proto-plus >= 1.10.0",
```

### Comparing `google-cloud-dialogflow-2.9.0/tests/__init__.py` & `google-cloud-dialogflow-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/__init__.py` & `google-cloud-dialogflow-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/__init__.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_agents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_agents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_answer_records.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_answer_records.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_contexts.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_contexts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_conversation_profiles.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_conversation_profiles.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_conversations.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_conversations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_documents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_documents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_entity_types.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_entity_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_environments.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_environments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_fulfillments.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_fulfillments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_intents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_intents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_knowledge_bases.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_participants.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_participants.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_session_entity_types.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_session_entity_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_sessions.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_sessions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2/test_versions.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2/test_versions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/__init__.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_agents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_agents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_answer_records.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_answer_records.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_contexts.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_contexts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_conversation_profiles.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_conversation_profiles.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_conversations.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_conversations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_documents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_documents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_entity_types.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_entity_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_environments.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_environments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_fulfillments.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_fulfillments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_intents.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_intents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_knowledge_bases.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_participants.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_participants.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_session_entity_types.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_session_entity_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_sessions.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_sessions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dialogflow-2.9.0/tests/unit/gapic/dialogflow_v2beta1/test_versions.py` & `google-cloud-dialogflow-2.9.1/tests/unit/gapic/dialogflow_v2beta1/test_versions.py`

 * *Files identical despite different names*

