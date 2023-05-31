# Comparing `tmp/goodai-ltm-0.1.0.tar.gz` & `tmp/goodai-ltm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.1.0.tar", last modified: Mon May 22 19:01:56 2023, max compression
+gzip compressed data, was "goodai-ltm-0.2.0.tar", last modified: Wed May 31 12:50:18 2023, max compression
```

## Comparing `goodai-ltm-0.1.0.tar` & `goodai-ltm-0.2.0.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.808776 goodai-ltm-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2008 2023-05-22 19:01:56.807776 goodai-ltm-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    15729 2023-05-22 19:01:10.000000 goodai-ltm-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.684777 goodai-ltm-0.1.0/goodai/
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.704779 goodai-ltm-0.1.0/goodai/helpers/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/helpers/collections_helper.py
--rw-rw-rw-   0        0        0     3257 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/json_helper.py
--rw-rw-rw-   0        0        0     1473 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/helpers/sched_opt.py
--rw-rw-rw-   0        0        0     3911 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.708777 goodai-ltm-0.1.0/goodai/ltm/
--rw-rw-rw-   0        0        0       34 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.710777 goodai-ltm-0.1.0/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.714777 goodai-ltm-0.1.0/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     1996 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/names/__init__.py
--rw-rw-rw-   0        0        0   183119 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/names/wikidata-names.json
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.732776 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      485 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     3036 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      331 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    11554 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1857 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa_tok_entry.py
--rw-rw-rw-   0        0        0     8159 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/sharc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.734777 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-05-08 20:37:32.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
--rw-rw-rw-   0        0        0     7168 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wiki.py
--rw-rw-rw-   0        0        0     7229 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wikianswers.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.749780 goodai-ltm-0.1.0/goodai/ltm/embeddings/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/__init__.py
--rw-rw-rw-   0        0        0     2600 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/auto.py
--rw-rw-rw-   0        0        0     1726 2023-05-03 22:03:18.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/base.py
--rw-rw-rw-   0        0        0     1554 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/contrast_classifier.py
--rw-rw-rw-   0        0        0     5994 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/default.py
--rw-rw-rw-   0        0        0     1515 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     3116 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/openai_emb.py
--rw-rw-rw-   0        0        0     2610 2023-05-03 22:03:18.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/st_emb.py
--rw-rw-rw-   0        0        0     5962 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/embeddings/trainable.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.763775 goodai-ltm-0.1.0/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     1589 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/auto.py
--rw-rw-rw-   0        0        0     4796 2023-05-18 14:51:26.000000 goodai-ltm-0.1.0/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     2716 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/metrics.py
--rw-rw-rw-   0        0        0     2158 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/msmarco.py
--rw-rw-rw-   0        0        0     1708 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/qp_ds.py
--rw-rw-rw-   0        0        0     1901 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/qrecc.py
--rw-rw-rw-   0        0        0     2072 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/strategy_qa.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.765776 goodai-ltm-0.1.0/goodai/ltm/eval/tests/
--rw-rw-rw-   0        0        0     1420 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/eval/tests/test_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.779776 goodai-ltm-0.1.0/goodai/ltm/mem/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.1.0/goodai/ltm/mem/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/auto.py
--rw-rw-rw-   0        0        0     2609 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/base.py
--rw-rw-rw-   0        0        0     1239 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk.py
--rw-rw-rw-   0        0        0      679 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk_mixin.py
--rw-rw-rw-   0        0        0    10596 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/chunk_queue.py
--rw-rw-rw-   0        0        0      995 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/config.py
--rw-rw-rw-   0        0        0     7939 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/default.py
--rw-rw-rw-   0        0        0    10980 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/mem_foundation.py
--rw-rw-rw-   0        0        0    13064 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/mem/rewrite_model.py
--rw-rw-rw-   0        0        0     3454 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/mem/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.782777 goodai-ltm-0.1.0/goodai/ltm/mem/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/__init__.py
--rw-rw-rw-   0        0        0     3091 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/test_chunk_queue.py
--rw-rw-rw-   0        0        0     2747 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/mem/tests/test_mem.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.793775 goodai-ltm-0.1.0/goodai/ltm/reranking/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/__init__.py
--rw-rw-rw-   0        0        0     2003 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/auto.py
--rw-rw-rw-   0        0        0     1248 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/base.py
--rw-rw-rw-   0        0        0    10135 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/default.py
--rw-rw-rw-   0        0        0     1857 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/emb.py
--rw-rw-rw-   0        0        0      706 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/prob_model.py
--rw-rw-rw-   0        0        0      672 2023-05-22 19:01:03.000000 goodai-ltm-0.1.0/goodai/ltm/reranking/st_ce.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.794776 goodai-ltm-0.1.0/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.799776 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7420 2023-05-03 13:13:46.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/em_trainer.py
--rw-rw-rw-   0        0        0     7635 2023-05-08 20:37:32.000000 goodai-ltm-0.1.0/goodai/ltm/training/query_passage/qppm_trainer.py
--rw-rw-rw-   0        0        0       23 2023-05-18 14:51:26.000000 goodai-ltm-0.1.0/goodai/ltm/version.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.801778 goodai-ltm-0.1.0/goodai/modules/
--rw-rw-rw-   0        0        0     1647 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/goodai/modules/loss.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:01:56.806776 goodai-ltm-0.1.0/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0     2008 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2554 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 19:01:56.000000 goodai-ltm-0.1.0/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 19:01:56.808776 goodai-ltm-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-05-11 14:39:36.000000 goodai-ltm-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.707733 goodai-ltm-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2008 2023-05-31 12:50:18.706732 goodai-ltm-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15811 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.589092 goodai-ltm-0.2.0/goodai/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.604091 goodai-ltm-0.2.0/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3257 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     1473 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/helpers/sched_opt.py
+-rw-rw-rw-   0        0        0     3911 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.607095 goodai-ltm-0.2.0/goodai/ltm/
+-rw-rw-rw-   0        0        0       34 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.608092 goodai-ltm-0.2.0/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.612091 goodai-ltm-0.2.0/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/names/__init__.py
+-rw-rw-rw-   0        0        0   183119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/names/wikidata-names.json
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.630514 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     3036 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11554 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa_tok_entry.py
+-rw-rw-rw-   0        0        0     8159 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/sharc.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.633132 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2632 2023-05-08 20:37:32.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     7168 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wiki.py
+-rw-rw-rw-   0        0        0     7229 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wikianswers.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.647171 goodai-ltm-0.2.0/goodai/ltm/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     3212 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/auto.py
+-rw-rw-rw-   0        0        0     1726 2023-05-03 22:03:18.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/base.py
+-rw-rw-rw-   0        0        0     1554 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5994 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/default.py
+-rw-rw-rw-   0        0        0     1515 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     3116 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/openai_emb.py
+-rw-rw-rw-   0        0        0     2610 2023-05-03 22:03:18.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/st_emb.py
+-rw-rw-rw-   0        0        0     5989 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/trainable.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.661172 goodai-ltm-0.2.0/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     1589 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4796 2023-05-18 14:51:26.000000 goodai-ltm-0.2.0/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     2158 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/msmarco.py
+-rw-rw-rw-   0        0        0     1708 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/qp_ds.py
+-rw-rw-rw-   0        0        0     1901 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.662171 goodai-ltm-0.2.0/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/tests/test_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.676734 goodai-ltm-0.2.0/goodai/ltm/mem/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/mem/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/auto.py
+-rw-rw-rw-   0        0        0     6012 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/base.py
+-rw-rw-rw-   0        0        0     1678 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/chunk.py
+-rw-rw-rw-   0        0        0    24198 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/chunk_queue.py
+-rw-rw-rw-   0        0        0     4635 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/config.py
+-rw-rw-rw-   0        0        0    10212 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/default.py
+-rw-rw-rw-   0        0        0    17984 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/mem_foundation.py
+-rw-rw-rw-   0        0        0    13064 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/mem/rewrite_model.py
+-rw-rw-rw-   0        0        0     3465 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.679732 goodai-ltm-0.2.0/goodai/ltm/mem/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/__init__.py
+-rw-rw-rw-   0        0        0    13906 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_chunk_queue.py
+-rw-rw-rw-   0        0        0    16882 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_mem.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.690733 goodai-ltm-0.2.0/goodai/ltm/reranking/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/auto.py
+-rw-rw-rw-   0        0        0     1248 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/base.py
+-rw-rw-rw-   0        0        0    10135 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/default.py
+-rw-rw-rw-   0        0        0     2219 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/emb.py
+-rw-rw-rw-   0        0        0      706 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/prob_model.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/st_ce.py
+-rw-rw-rw-   0        0        0     6952 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/stanford.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.691733 goodai-ltm-0.2.0/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.696732 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7420 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/em_trainer.py
+-rw-rw-rw-   0        0        0     7635 2023-05-08 20:37:32.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/qppm_trainer.py
+-rw-rw-rw-   0        0        0       23 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/version.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.698733 goodai-ltm-0.2.0/goodai/modules/
+-rw-rw-rw-   0        0        0     1647 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/modules/loss.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.700732 goodai-ltm-0.2.0/goodai/text_gen/
+-rw-rw-rw-   0        0        0      158 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/text_gen/base.py
+-rw-rw-rw-   0        0        0     1860 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/text_gen/openai_tg.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.705732 goodai-ltm-0.2.0/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:50:18.707733 goodai-ltm-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/setup.py
```

### Comparing `goodai-ltm-0.1.0/LICENSE` & `goodai-ltm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/PKG-INFO` & `goodai-ltm-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodai-ltm
-Version: 0.1.0
+Version: 0.2.0
 Summary: A text memory meant to be used with conversational language models.
 Home-page: https://github.com/GoodAI/goodai-ltm
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## GoodAI-LTM
```

### Comparing `goodai-ltm-0.1.0/README.md` & `goodai-ltm-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 The following code snippet creates an instance of LTM, loads in some text and then retrieves the most relevant text chunks given a query:
 
     from goodai.ltm.mem.auto import AutoTextMemory
     mem = AutoTextMemory.create()
     mem.add_text("Lorem ipsum dolor sit amet, consectetur adipiscing elit\n")
     mem.add_text("Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore\n",
-                 metadata={'timestamp': time.time(), 'type': 'generic'})
+                 metadata={'title': 'My document', 'tags': ['latin']})
     r_memories = mem.retrieve(query='dolorem eum fugiat quo voluptas nulla pariatur?', k=3)
 
 ## Loading a text memory instance
 
 A default memory instance can be created as follows:
 
     from goodai.ltm.mem.auto import AutoTextMemory
@@ -102,27 +102,28 @@
 
 Internally, the memory will chunk and index the text
 automatically.
 
 Text can be associated with an arbitrary metadata dictionary, such as:
 
     mem.add_text("Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore\n",
-                 metadata={'timestamp': time.time(), 'type': 'generic'})
+                 metadata={'title': 'My document', 'tags': ['latin']})
 
 Internally, the memory concatenates text stored using add_text with any text previously sent to the memory.
 
 To retrieve a list of passages associated with a query,
 call the `retrieve` method:
 
     r_memories = mem.retrieve(query='dolorem eum fugiat quo voluptas nulla pariatur?', k=3)
 
 The `retrieve` method returns a list of objects of type `RetrievedMemory`, containing
 the following properties:
 
 * `passage`: The text of the memory. This corresponds to text found in a matching chunk, but it may be expanded using text from adjacent chunks.
+* `timestamp`: The time (seconds since Epoch) when the retrieved chunk was created. 
 * `distance`: Calculated distance between the query and the chunk passage.
 * `confidence`: If a query-passage matching model is available, this is the probability assigned by the model.
 * `metadata`: Metadata associated with the retrieved text, if any.
 
 ## How it works
 
 For a slightly more detailed view of how the memory works, let us revisit the storage and retrieval of text passages.
```

### Comparing `goodai-ltm-0.1.0/goodai/helpers/file_helper.py` & `goodai-ltm-0.2.0/goodai/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/helpers/sched_opt.py` & `goodai-ltm-0.2.0/goodai/helpers/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/helpers/tokenizer_helper.py` & `goodai-ltm-0.2.0/goodai/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/cloud.py` & `goodai-ltm-0.2.0/goodai/ltm/data/cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 
 class CloudStorage:
     def __init__(self, bucket_name: str):
         self.bucket_name = bucket_name
         aws_key_id = os.environ.get('AWS_ACCESS_KEY_ID')
         if aws_key_id is None:
-            raise SystemError('AWS_ACCESS_KEY_ID needs to be set')
+            raise RuntimeError('AWS_ACCESS_KEY_ID needs to be set')
         aws_secret_key = os.environ.get('AWS_SECRET_ACCESS_KEY')
         if aws_secret_key is None:
-            raise SystemError('AWS_SECRET_ACCESS_KEY needs to be set')
+            raise RuntimeError('AWS_SECRET_ACCESS_KEY needs to be set')
         self.client = boto3.client(
             's3',
             aws_access_key_id=aws_key_id,
             aws_secret_access_key=aws_secret_key,
         )
 
     def put_object(self, key: str, obj: Dict[str, Any]):
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.2.0/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/names/wikidata-names.json` & `goodai-ltm-0.2.0/goodai/ltm/data/names/wikidata-names.json`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/dataset.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/sharc.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/sharc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wiki.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/data/query_passage/wikianswers.py` & `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wikianswers.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/auto.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pickle
 from typing import Union
+from weakref import WeakValueDictionary
 
 import torch
 
 from goodai.helpers.file_helper import open_url_as_file, unpickle_downloaded_url
 from goodai.ltm.embeddings.openai_emb import OpenAIEmbeddingModel
 from goodai.ltm.embeddings.st_emb import SentenceTransformerEmbeddingModel
 from goodai.ltm.embeddings.trainable import TrainableEmbeddingModel
@@ -22,14 +23,25 @@
 
 class AutoTextEmbeddingModel:
     """
     Factory class for text embedding models.
     """
 
     @staticmethod
+    def shared_pretrained(name: str, device: Union[str, torch.device] = None):
+        if device is None:
+            device = torch.device('cuda:0') if torch.cuda.is_available() else torch.device('cpu')
+        key = f'{name}|{device}'
+        model = AutoTextEmbeddingModel.model_cache.get(key)
+        if model is None:
+            model = AutoTextEmbeddingModel.from_pretrained(name, device)
+            AutoTextEmbeddingModel.model_cache[key] = model
+        return model
+
+    @staticmethod
     def from_pretrained(name: str, device: Union[str, torch.device] = None, **kwargs) -> BaseTextEmbeddingModel:
         """
         Makes a pretrained embedding model from a descriptor (name).
 
         The name has the format <model_type>:<model_name>, for example "st:sentence-transformers/all-distilroberta-v1",
         where model_type is 'st' for Hugging Face Sentence Transformers or 'openai' for Open AI text embeddings.
 
@@ -56,7 +68,10 @@
         model_name = name[colon_idx + 1:]
         if model_type == 'st':
             return SentenceTransformerEmbeddingModel(model_name, device=device, **kwargs)
         elif model_type == 'openai':
             return OpenAIEmbeddingModel(model_name, device=device, **kwargs)
         else:
             raise ValueError(f'Unknown model type: {model_type}')
+
+
+AutoTextEmbeddingModel.model_cache = WeakValueDictionary()
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/base.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/contrast_classifier.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/default.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/emb_qp_prob_model.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/emb_qp_prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/openai_emb.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/openai_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/st_emb.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/st_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/embeddings/trainable.py` & `goodai-ltm-0.2.0/goodai/ltm/embeddings/trainable.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
                           show_progress_bar: bool = False,
                           convert_to_tensor: bool = False,
                           return_token_lengths: bool = False,
                           detach_tensors: bool = True,
                           device: Union[str, torch.device] = None):
         device = device if device else self.get_device()
         t = self.tokenizer
-        rng = range(0, len(sentences), batch_size)
+        s_count = len(sentences)
+        rng = range(0, s_count, batch_size)
         if show_progress_bar:
             rng = tqdm(rng, desc='Embeddings', unit='batch')
         keys_list = []
         for b0 in rng:
             b_sentences = sentences[b0:b0 + batch_size]
             input_ids_list = [t.encode(s, add_special_tokens=add_special_tokens) for s in b_sentences]
             model_inputs = get_model_inputs(input_ids_list, self.pad_token_id,
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/auto.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/mem.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/mem.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/msmarco.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/msmarco.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/qp_ds.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/qp_ds.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/qrecc.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/qrecc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/strategy_qa.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/strategy_qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/eval/tests/test_metrics.py` & `goodai-ltm-0.2.0/goodai/ltm/eval/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/mem/auto.py` & `goodai-ltm-0.2.0/goodai/ltm/mem/auto.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import weakref
 
 import torch
 from typing import Union, Optional
 from transformers import AutoTokenizer, PreTrainedTokenizer
 from goodai.ltm.embeddings.auto import AutoTextEmbeddingModel
 from goodai.ltm.embeddings.base import BaseTextEmbeddingModel
-from goodai.ltm.mem.base import BaseTextMemory
+from goodai.ltm.mem.base import BaseTextMemory, BaseReranker, BaseImportanceModel
 from goodai.ltm.mem.config import TextMemoryConfig
 from goodai.ltm.mem.default import DefaultTextMemory
 from goodai.ltm.mem.mem_foundation import VectorDbType
 from goodai.ltm.mem.rewrite_model import BaseRewriteModel
+from goodai.ltm.reranking.auto import AutoTextMatchingModel
 from goodai.ltm.reranking.base import BaseTextMatchingModel
 
-_default_emb_model_wr: Optional[weakref.ref] = None
 _default_tokenizer_wr: Optional[weakref.ref] = None
 
 
 class MemType(enum.Enum):
     TRANSIENT_CHUNK_EMB = 0
 
 
@@ -27,30 +27,35 @@
     Factory class for text memory.
     """
 
     @staticmethod
     def create(mem_type: MemType = MemType.TRANSIENT_CHUNK_EMB,
                vector_db_type: VectorDbType = VectorDbType.SIMPLE,
                tokenizer: PreTrainedTokenizer = None,
-               emb_model: BaseTextEmbeddingModel = None,
-               matching_model: BaseTextMatchingModel = None,
+               emb_model: Union[BaseTextEmbeddingModel, Optional[str]] = None,
+               matching_model: Union[BaseTextMatchingModel, Optional[str]] = None,
                query_rewrite_model: BaseRewriteModel = None,
                memory_rewrite_model: BaseRewriteModel = None,
+               reranker: BaseReranker = None,
+               importance_model: BaseImportanceModel = None,
                device: Union[torch.device, str] = None,
                config: TextMemoryConfig = None
                ) -> BaseTextMemory:
         """
         Creates a memory instance.
         :param mem_type: Reserved parameter.
         :param vector_db_type: The type of vector database. Default is VectorDbType.SIMPLE.
         :param tokenizer: A chunking tokenizer. It should be a tokenizer that preserves whitespace and casing.
         :param emb_model: The embedding model.
         :param matching_model: An optional query-passage matching model.
         :param query_rewrite_model: The query rewrite model.
         :param memory_rewrite_model: The memory rewrite model.
+        :param reranker: A custom reranker.
+        :param importance_model: A model that assigns an importance value to stored memories.
+        It may be required by some rerankers.
         :param device: The Pytorch device.
         :param config: The memory configuration.
         :return: An instance of BaseTextMemory.
         """
         if tokenizer is None:
             global _default_tokenizer_wr
 
@@ -60,21 +65,20 @@
                 tokenizer = AutoTokenizer.from_pretrained('distilroberta-base')
                 # Suppress length warning
                 tokenizer.model_max_length = sys.maxsize
                 _default_tokenizer_wr = weakref.ref(tokenizer)
         if device is None:
             device = torch.device('cuda:0') if torch.cuda.is_available() else torch.device('cpu')
         if emb_model is None:
-            global _default_emb_model_wr
-
-            if _default_emb_model_wr:
-                emb_model = _default_emb_model_wr()
-            if emb_model is None:
-                emb_model = AutoTextEmbeddingModel.from_pretrained('em-distilroberta-p1-01',
-                                                                   device=device)
-                _default_emb_model_wr = weakref.ref(emb_model)
+            emb_model = 'em-distilroberta-p1-01'
+        if isinstance(emb_model, str):
+            emb_model = AutoTextEmbeddingModel.shared_pretrained(emb_model)
+        if isinstance(matching_model, str):
+            matching_model = AutoTextMatchingModel.shared_pretrained(matching_model)
         if config is None:
             config = TextMemoryConfig()
         return DefaultTextMemory(vector_db_type, tokenizer, emb_model, matching_model,
                                  device=device, config=config,
                                  query_rewrite_model=query_rewrite_model,
-                                 memory_rewrite_model=memory_rewrite_model)
+                                 memory_rewrite_model=memory_rewrite_model,
+                                 reranker=reranker,
+                                 importance_model=importance_model)
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/mem/chunk.py` & `goodai-ltm-0.2.0/goodai/ltm/mem/chunk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+import time
 from typing import Any, Optional
 
+TextKeyType = int
+
 
 class Chunk:
-    def __init__(self, index: int, capacity: int, from_token_seq_id: int, metadata: Optional[dict]):
+    def __init__(self, chunk_id: int, capacity: int, from_token_seq_id: int, metadata: Optional[dict],
+                 importance: Optional[float], timestamp: float):
+        self.importance = importance
         self.metadata = metadata
-        self.index = index
+        self.chunk_id = chunk_id
         self.capacity = capacity
         self.from_token_seq_id = from_token_seq_id
         self.to_token_seq_id = from_token_seq_id
         self.indexed: bool = False
+        self.timestamp: float = timestamp
+        self.associated_keys = []
 
     def __len__(self):
         return self.to_token_seq_id - self.from_token_seq_id
 
     def get_room(self):
         return self.capacity - len(self)
 
@@ -25,12 +32,19 @@
         self.to_token_seq_id = to_token_seq_id
 
     def extend_by(self, num_tokens: int):
         if len(self) + num_tokens > self.capacity:
             raise ValueError(f'capacity={self.capacity} would be exceeded')
         self.to_token_seq_id += num_tokens
 
+    def shift(self, offset: int):
+        self.from_token_seq_id += offset
+        self.to_token_seq_id += offset
+
     def is_indexed(self) -> bool:
         return self.indexed
 
     def set_indexed(self, mode: bool):
         self.indexed = mode
+
+    def add_key(self, text_key: TextKeyType):
+        self.associated_keys.append(text_key)
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/mem/default.py` & `goodai-ltm-0.2.0/goodai/ltm/mem/default.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-import gc
-from typing import List, Union, Any, Callable, Set, Optional, Tuple
+import math
+from typing import List, Union, Any, Optional, Tuple, Callable
 import numpy as np
 import torch
 from faiss import Index
 from tqdm import tqdm
 from transformers import PreTrainedTokenizer
 
 from goodai.helpers.tokenizer_helper import get_pad_token_id, get_sentence_punctuation_ids
 from goodai.ltm.embeddings.base import BaseTextEmbeddingModel
-from goodai.ltm.mem.base import RetrievedMemory
-from goodai.ltm.mem.chunk import Chunk
+from goodai.ltm.mem.base import BaseReranker, BaseImportanceModel
+from goodai.ltm.mem.chunk import Chunk, TextKeyType
 from goodai.ltm.mem.rewrite_model import BaseRewriteModel
 from goodai.ltm.reranking.base import BaseTextMatchingModel
-from goodai.ltm.mem.chunk_queue import ChunkQueue, BaseChunkQueue
+from goodai.ltm.mem.chunk_queue import ChunkQueue, PassageInfo, ChunkExpansionOptions
 from goodai.ltm.mem.config import TextMemoryConfig
 from goodai.ltm.mem.mem_foundation import BaseTextMemoryFoundation, VectorDbType
 from goodai.ltm.mem.simple_vector_db import SimpleVectorDb
 
 _vector_db_type = Union[Index, SimpleVectorDb]
 
 
 class DefaultTextMemory(BaseTextMemoryFoundation):
     def __init__(self, vector_db_type: VectorDbType, tokenizer: PreTrainedTokenizer,
                  emb_model: BaseTextEmbeddingModel, matching_model: Optional[BaseTextMatchingModel],
                  device: torch.device, config: TextMemoryConfig,
-                 chunk_queue_fn: Callable[[], BaseChunkQueue] = None,
                  query_rewrite_model: Optional[BaseRewriteModel] = None,
-                 memory_rewrite_model: Optional[BaseRewriteModel] = None
+                 memory_rewrite_model: Optional[BaseRewriteModel] = None,
+                 reranker: Optional[BaseReranker] = None,
+                 importance_model: Optional[BaseImportanceModel] = None,
                  ):
-        if chunk_queue_fn is None:
-            def chunk_queue_fn():
-                return ChunkQueue(config.queue_capacity, config.chunk_capacity)
-
+        cc = config.chunk_capacity
+        cof = config.chunk_overlap_fraction
+        if cof < 0 or cof > 0.5:
+            raise ValueError(f'Invalid chunk overlap fraction: {cof}')
+        ciao = cc - math.ceil(cc * cof)
+        self.chunk_queue = ChunkQueue(config.queue_capacity, cc, ciao)
         self.config = config
         self.device = device
         self.emb_model = emb_model
         self.matching_model = matching_model
         self.chunk_tokenizer = tokenizer
         self.bucket_capacity = config.chunk_capacity
         self.pad_token_id = get_pad_token_id(self.chunk_tokenizer)
         self.punctuation_ids = get_sentence_punctuation_ids(self.chunk_tokenizer, include_line_break=False)
-        self.chunk_queue: BaseChunkQueue = chunk_queue_fn()
-        has_matching_model = self.matching_model is not None
         self.query_rewrite_model = query_rewrite_model
         self.memory_rewrite_model = memory_rewrite_model
+        self.importance_model = importance_model
+        self.reranker = reranker
+        self.ce_options = ChunkExpansionOptions.from_config(tokenizer, config.chunk_expansion_config)
+        has_matching_model = self.matching_model is not None
         super().__init__(vector_db_type, self.chunk_tokenizer, has_matching_model,
                          self.emb_model.get_num_storage_embeddings(),
-                         self.emb_model.get_embedding_dim(), config.reranking_k_factor,
-                         config.max_query_length, device)
+                         self.emb_model.get_embedding_dim(),
+                         config.chunk_capacity,
+                         config.reranking_k_factor, config.max_query_length,
+                         query_rewrite_model, reranker,
+                         config.chunk_overlap_fraction, config.redundancy_overlap_threshold,
+                         self.ce_options, device)
+
+    def has_importance_model(self) -> bool:
+        return self.importance_model is not None
 
     def get_tokenizer(self):
         return self.chunk_tokenizer
 
     def get_queue_capacity(self):
         return self.chunk_queue.get_capacity()
 
@@ -64,49 +76,81 @@
             return None
         return chunk.metadata
 
     def get_chunk_text(self, chunk: Chunk) -> str:
         token_ids = self.chunk_queue.get_chunk_token_ids(chunk)
         return self.chunk_tokenizer.decode(token_ids, skip_special_tokens=True)
 
-    def retrieve_multiple(self, queries: List[str], k: int = 1, rewrite: bool = False,
-                          show_progress_bar: bool = False, **kwargs) -> List[List[RetrievedMemory]]:
-        if rewrite and not self.query_rewrite_model:
-            raise ValueError("For query rewriting, a rewriting model must be provided")
-        if rewrite and self.query_rewrite_model:
-            queries = [self.query_rewrite_model.rewrite_query(q) for q in queries]
-        return super().retrieve_multiple(queries, k, rewrite, show_progress_bar, **kwargs)
+    def get_complete_passage(self, chunk: Chunk) -> PassageInfo:
+        return self.chunk_queue.get_complete_passage(chunk, self.ce_options)
 
-    def retrieve_chunk_sequences(self, chunk_ids: List[int]):
-        return self.chunk_queue.retrieve_chunk_sequences(chunk_ids)
+    def get_chunk(self, chunk_id: int) -> Chunk:
+        return self.chunk_queue.get_chunk(chunk_id)
 
-    def retrieve_complete_sequences(self, chunk_ids: List[int], punctuation_ids: Set[int]):
-        return self.chunk_queue.retrieve_complete_sequences(chunk_ids, punctuation_ids)
+    def retrieve_chunk_sequences(self, chunks: List[Chunk]):
+        return self.chunk_queue.retrieve_chunk_sequences_given_chunks(chunks)
 
     def get_retrieval_key_for_text(self, queries: List[str], show_progress_bar: bool = False) -> torch.Tensor:
         return self.emb_model.encode_queries(queries, convert_to_tensor=True, show_progress_bar=show_progress_bar)
 
     def predict_match(self, sentences: List[Tuple[str, str]], show_progress_bar: bool = False,
                       batch_size: int = 32) -> List[float]:
         return self.matching_model.predict(sentences, show_progress_bar=show_progress_bar,
                                            batch_size=batch_size)
 
-    def add_text(self, text: str, metadata: Optional[Any] = None, rewrite: bool = False,
-                 rewrite_context: Optional[str] = None, show_progress_bar: bool = False):
+    def _replace_or_add_text(self, cq_fn: Callable, text: str, metadata: Optional[Any] = None, rewrite: bool = False,
+                             rewrite_context: Optional[str] = None, show_progress_bar: bool = False,
+                             timestamp: Optional[float] = None, text_key: TextKeyType = None):
         if rewrite and not self.memory_rewrite_model:
             raise ValueError("For memory rewriting, a rewriting model must be provided")
         if rewrite and self.memory_rewrite_model:
             text = self.memory_rewrite_model.rewrite_memory(text, rewrite_context)
-
+        importance = None
+        if self.importance_model:
+            importance = self.importance_model.get_importance(text)
         token_ids = self.chunk_tokenizer.encode(text, add_special_tokens=False)
-        removed_buckets = self.chunk_queue.add_sequence(token_ids, metadata)
+        cq_params = dict(
+            new_token_ids=token_ids,
+            metadata=metadata,
+            importance=importance,
+            timestamp=timestamp,
+        )
+        if text_key is not None:
+            cq_params['text_key'] = text_key
+        removed_chunks, text_key = cq_fn(**cq_params)
         self._ensure_keys_added(show_progress_bar=show_progress_bar)
-        removed_indexes = [rb.index for rb in removed_buckets]
-        if len(removed_indexes) > 0:
-            self.vector_db.remove_ids(np.array(removed_indexes).astype(np.int64))
+        removed_chunk_ids = [rb.chunk_id for rb in removed_chunks]
+        if len(removed_chunk_ids) > 0:
+            self.vector_db.remove_ids(np.array(removed_chunk_ids).astype(np.int64))
+        return text_key
+
+    def add_text(self, text: str, metadata: Optional[dict] = None, rewrite: bool = False,
+                 rewrite_context: Optional[str] = None, show_progress_bar: bool = False,
+                 timestamp: Optional[float] = None) -> TextKeyType:
+        return self._replace_or_add_text(self.chunk_queue.add_sequence,
+                                         text=text, metadata=metadata, rewrite=rewrite,
+                                         rewrite_context=rewrite_context, show_progress_bar=show_progress_bar,
+                                         timestamp=timestamp)
+
+    def replace_text(self, text_key: TextKeyType, text: str, metadata: Optional[dict] = None,
+                     rewrite: bool = False, rewrite_context: Optional[str] = None,
+                     show_progress_bar: bool = False, timestamp: Optional[float] = None) -> TextKeyType:
+        return self._replace_or_add_text(self.chunk_queue.replace_sequence,
+                                         text=text, metadata=metadata, rewrite=rewrite,
+                                         rewrite_context=rewrite_context, show_progress_bar=show_progress_bar,
+                                         timestamp=timestamp, text_key=text_key)
+
+    def delete_text(self, text_key: TextKeyType, show_progress_bar: bool = False) -> TextKeyType:
+        return self.replace_text(text_key, "", show_progress_bar=show_progress_bar)
+
+    def add_separator(self):
+        self.chunk_queue.add_separator(self.pad_token_id)
+
+    def is_empty(self) -> bool:
+        return len(self.chunk_queue.token_ids) == 0
 
     def retrieve_all_text(self) -> str:
         token_ids = self.chunk_queue.get_latest_token_ids(max_num_tokens=None)
         return self.chunk_tokenizer.decode(token_ids, skip_special_tokens=True)
 
     def retrieve_all_chunks(self) -> List[str]:
         chunk_list = self.chunk_queue.get_chunk_sequences()
@@ -126,29 +170,26 @@
             rng = tqdm(rng, desc='Storage', unit='batch')
         for i in rng:
             token_id_batch = token_id_matrix[i:i + batch_size]
             text_batch = self.chunk_tokenizer.batch_decode(token_id_batch, skip_special_tokens=True)
             sk_batch = emb_model.encode_corpus(text_batch, convert_to_tensor=True,
                                                show_progress_bar=False, batch_size=batch_size)
             if sk_batch.size(0) != len(text_batch):
-                raise SystemError(f'Number of storage embeddings returned by embedding model is {sk_batch.size(0)}, '
-                                  f'while the number of encoded texts is {len(text_batch)}')
+                raise RuntimeError(f'Number of storage embeddings returned by embedding model is {sk_batch.size(0)}, '
+                                   f'while the number of encoded texts is {len(text_batch)}')
             sk_list.append(sk_batch.detach())
-            if num_sequences > batch_size:
-                del sk_batch
-                gc.collect()
         if len(sk_list) > 0:
             sk_all = torch.cat(sk_list)
             num_chunks, num_sk = sk_all.size(0), sk_all.size(1),
             sk_all = sk_all.view(num_chunks * num_sk, -1)
             sk_all_np = sk_all.cpu().numpy().astype(np.float32)
             b_indexes = []
             for chunk in picked_chunks:
                 if chunk.is_at_capacity():
                     chunk.set_indexed(True)
-                b_indexes.extend([chunk.index] * num_sk)
+                b_indexes.extend([chunk.chunk_id] * num_sk)
             b_indexes_np = np.array(b_indexes).astype(np.int64)
             self.vector_db.add_with_ids(sk_all_np, b_indexes_np)
 
     def clear(self):
         self.chunk_queue.flush()
         self.vector_db.reset()
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/mem/rewrite_model.py` & `goodai-ltm-0.2.0/goodai/ltm/mem/rewrite_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/mem/simple_vector_db.py` & `goodai-ltm-0.2.0/goodai/ltm/mem/simple_vector_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         placeholder_ids = -np.ones((batch_size, k), dtype=np.int64)
         if self.all_vectors is None:
             return placeholder_dist, placeholder_ids,
         # vectors: (n, emb_size,)
         # all_vectors: (m, emb_size,)
         diff_sq = (vectors[:, None, :] - self.all_vectors[None, :, :]) ** 2
         # diff_sq: (n, m, emb_size,)
-        mean_diff_sq = np.mean(diff_sq, axis=2)
+        all_sq_distances = np.sum(diff_sq, axis=2)
         # mean_diff_sq: (n, m,)
-        sort_indexes = np.argsort(mean_diff_sq, axis=1)
+        sort_indexes = np.argsort(all_sq_distances, axis=1)
         # sort_indexes: (n, m,)
         select_indexes = sort_indexes[:, :k]
         flat_select_indexes = select_indexes.flatten()
         flat_result_ids = self.all_ids[flat_select_indexes]
         # result_indexes: (n, k,)
         result_size, num_result_ids = select_indexes.shape
         result_range = np.arange(0, result_size)
         rep_range = np.repeat(result_range, num_result_ids)
-        result_distances = mean_diff_sq[rep_range, flat_select_indexes]
+        result_distances = all_sq_distances[rep_range, flat_select_indexes]
         result_distances = np.reshape(result_distances, select_indexes.shape)
         result_ids = np.reshape(flat_result_ids, select_indexes.shape)
         placeholder_dist[:, :result_distances.shape[1]] = result_distances
         placeholder_ids[:, :result_ids.shape[1]] = result_ids
         return placeholder_dist, placeholder_ids,
 
     def add_with_ids(self, vectors: np.ndarray, ids: np.ndarray):
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/reranking/auto.py` & `goodai-ltm-0.2.0/goodai/ltm/reranking/auto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pickle
 from typing import Union
+from weakref import WeakValueDictionary
+
 import torch
 
-from goodai.helpers.file_helper import open_url_as_file, unpickle_downloaded_url
+from goodai.helpers.file_helper import unpickle_downloaded_url
 from goodai.ltm.embeddings.auto import AutoTextEmbeddingModel
 from goodai.ltm.reranking.base import BaseTextMatchingModel
 from goodai.ltm.reranking.default import DefaultRerankingCrossEncoder
 from goodai.ltm.reranking.emb import EmbeddingBasedMatchingModel
 from goodai.ltm.reranking.st_ce import SentenceTransformerTextMatchingModel
 
 _default_dist_param = 0.75
@@ -18,14 +20,25 @@
 
 class AutoTextMatchingModel:
     """
     Factory class for text matching models.
     """
 
     @staticmethod
+    def shared_pretrained(name: str, device: Union[str, torch.device] = None):
+        if device is None:
+            device = torch.device('cuda:0') if torch.cuda.is_available() else torch.device('cpu')
+        key = f'{name}|{device}'
+        model = AutoTextMatchingModel.model_cache.get(key)
+        if model is None:
+            model = AutoTextMatchingModel.from_pretrained(name, device)
+            AutoTextMatchingModel.model_cache[key] = model
+        return model
+
+    @staticmethod
     def from_pretrained(name: str, device: Union[torch.device, str] = None) -> BaseTextMatchingModel:
         if device is None:
             device = torch.device('cuda:0') if torch.cuda.is_available() else torch.device('cpu')
         name = name.strip()
         colon_idx = name.find(':')
         if colon_idx == -1:
             url = _pretrained_map.get(name)
@@ -38,11 +51,14 @@
             model.eval()
             return model
         model_type = name[:colon_idx]
         model_name = name[colon_idx + 1:]
         if model_type == 'st':
             return SentenceTransformerTextMatchingModel(model_name)
         elif model_type == 'em':
-            emb_model = AutoTextEmbeddingModel.from_pretrained(model_name, device=device)
+            emb_model = AutoTextEmbeddingModel.shared_pretrained(model_name, device=device)
             return EmbeddingBasedMatchingModel(emb_model, _default_dist_param)
         else:
             raise ValueError(f'Unknown model type: {model_type}')
+
+
+AutoTextMatchingModel.model_cache = WeakValueDictionary()
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/reranking/base.py` & `goodai-ltm-0.2.0/goodai/ltm/reranking/base.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/reranking/default.py` & `goodai-ltm-0.2.0/goodai/ltm/reranking/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/reranking/emb.py` & `goodai-ltm-0.2.0/goodai/ltm/reranking/emb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-import gc
-from typing import List, Tuple
-
 import torch
-
-from goodai.helpers.tokenizer_helper import get_model_inputs
+from typing import List, Tuple
+from tqdm import tqdm
 from goodai.ltm.embeddings.base import BaseTextEmbeddingModel
-from goodai.ltm.embeddings.trainable import TrainableEmbeddingModel
 from goodai.ltm.reranking.base import BaseTextMatchingModel
 from goodai.modules.loss import EmbCrossProbLossModel
 
 
 class EmbeddingBasedMatchingModel(BaseTextMatchingModel):
     def __init__(self, emb_model: BaseTextEmbeddingModel, dist_param: float):
         super().__init__()
         self.dist_param = dist_param
         self.emb_model = emb_model
 
     def predict(self, sentences: List[Tuple[str, str]], batch_size: int = 32,
                 show_progress_bar: bool = False, add_special_tokens: bool = True) -> List[float]:
-        queries, passages = zip(*sentences)
-        rk = self.emb_model.encode_queries(queries, batch_size=batch_size, show_progress_bar=show_progress_bar,
-                                           convert_to_tensor=True)
-        rk = rk.detach()
-        gc.collect()
-        sk = self.emb_model.encode_corpus(passages, batch_size=batch_size, show_progress_bar=show_progress_bar,
-                                          convert_to_tensor=True)
-        sk = sk.detach()
-        # rk: (batch_size, num_r_emb, emb_dim,)
-        # sk: (batch_size, num_s_emb, emb_dim,)
-        distances = torch.cdist(rk, sk)
-        # distances: (batch_size, num_r_emb, num_s_emb,)
-        batch_size = distances.size(0)
-        distances = distances.view(batch_size, -1)
-        min_distances = torch.amin(distances, dim=1, keepdim=True)
-        prob_t = EmbCrossProbLossModel.get_prob(min_distances, self.dist_param)
-        return prob_t.squeeze(1).tolist()
+        with torch.no_grad():
+            rng = range(0, len(sentences), batch_size)
+            if show_progress_bar:
+                rng = tqdm(rng, desc='Encoding QPs', unit='batch')
+            result: List[float] = []
+            for b0 in rng:
+                b_sentences = sentences[b0:b0 + batch_size]
+                queries, passages = zip(*b_sentences)
+                rk = self.emb_model.encode_queries(queries, batch_size=batch_size, show_progress_bar=False,
+                                                   convert_to_tensor=True)
+                rk = rk.detach()
+                sk = self.emb_model.encode_corpus(passages, batch_size=batch_size, show_progress_bar=False,
+                                                  convert_to_tensor=True)
+                sk = sk.detach()
+                # rk: (batch_size, num_r_emb, emb_dim,)
+                # sk: (batch_size, num_s_emb, emb_dim,)
+                distances = torch.cdist(rk, sk)
+                # distances: (batch_size, num_r_emb, num_s_emb,)
+                batch_size = distances.size(0)
+                distances = distances.view(batch_size, -1)
+                min_distances = torch.amin(distances, dim=1, keepdim=True)
+                prob_t = EmbCrossProbLossModel.get_prob(min_distances, self.dist_param)
+                partial_result = prob_t.squeeze(1).tolist()
+                result.extend(partial_result)
+            return result
 
     def get_info(self):
         return f'{self.__class__}: EmbModel {self.emb_model.get_info()}'
```

### Comparing `goodai-ltm-0.1.0/goodai/ltm/reranking/prob_model.py` & `goodai-ltm-0.2.0/goodai/ltm/reranking/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/training/query_passage/em_trainer.py` & `goodai-ltm-0.2.0/goodai/ltm/training/query_passage/em_trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/ltm/training/query_passage/qppm_trainer.py` & `goodai-ltm-0.2.0/goodai/ltm/training/query_passage/qppm_trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai/modules/loss.py` & `goodai-ltm-0.2.0/goodai/modules/loss.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.1.0/goodai_ltm.egg-info/PKG-INFO` & `goodai-ltm-0.2.0/goodai_ltm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodai-ltm
-Version: 0.1.0
+Version: 0.2.0
 Summary: A text memory meant to be used with conversational language models.
 Home-page: https://github.com/GoodAI/goodai-ltm
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## GoodAI-LTM
```

### Comparing `goodai-ltm-0.1.0/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.2.0/goodai_ltm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 goodai/helpers/__init__.py
-goodai/helpers/collections_helper.py
 goodai/helpers/file_helper.py
 goodai/helpers/html_helper.py
 goodai/helpers/json_helper.py
 goodai/helpers/sched_opt.py
 goodai/helpers/tokenizer_helper.py
 goodai/helpers/torch_helper.py
 goodai/ltm/__init__.py
@@ -45,15 +44,14 @@
 goodai/ltm/eval/qrecc.py
 goodai/ltm/eval/strategy_qa.py
 goodai/ltm/eval/tests/test_metrics.py
 goodai/ltm/mem/__init__.py
 goodai/ltm/mem/auto.py
 goodai/ltm/mem/base.py
 goodai/ltm/mem/chunk.py
-goodai/ltm/mem/chunk_mixin.py
 goodai/ltm/mem/chunk_queue.py
 goodai/ltm/mem/config.py
 goodai/ltm/mem/default.py
 goodai/ltm/mem/mem_foundation.py
 goodai/ltm/mem/rewrite_model.py
 goodai/ltm/mem/simple_vector_db.py
 goodai/ltm/mem/tests/__init__.py
@@ -62,17 +60,20 @@
 goodai/ltm/reranking/__init__.py
 goodai/ltm/reranking/auto.py
 goodai/ltm/reranking/base.py
 goodai/ltm/reranking/default.py
 goodai/ltm/reranking/emb.py
 goodai/ltm/reranking/prob_model.py
 goodai/ltm/reranking/st_ce.py
+goodai/ltm/reranking/stanford.py
 goodai/ltm/training/__init__.py
 goodai/ltm/training/query_passage/__init__.py
 goodai/ltm/training/query_passage/em_trainer.py
 goodai/ltm/training/query_passage/qppm_trainer.py
 goodai/modules/loss.py
+goodai/text_gen/base.py
+goodai/text_gen/openai_tg.py
 goodai_ltm.egg-info/PKG-INFO
 goodai_ltm.egg-info/SOURCES.txt
 goodai_ltm.egg-info/dependency_links.txt
 goodai_ltm.egg-info/requires.txt
 goodai_ltm.egg-info/top_level.txt
```

### Comparing `goodai-ltm-0.1.0/setup.py` & `goodai-ltm-0.2.0/setup.py`

 * *Files identical despite different names*

