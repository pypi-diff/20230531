# Comparing `tmp/sohuprompt-1.0.6.tar.gz` & `tmp/sohuprompt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sohuprompt-1.0.6.tar", last modified: Thu Apr 27 12:28:21 2023, max compression
+gzip compressed data, was "dist/sohuprompt-1.0.7.tar", last modified: Wed May 31 02:58:19 2023, max compression
```

## Comparing `sohuprompt-1.0.6.tar` & `sohuprompt-1.0.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6324 2023-04-27 12:25:38.000000 sohuprompt-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-27 12:24:04.000000 sohuprompt-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.563380 sohuprompt-1.0.6/sohuprompt/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-27 12:24:19.000000 sohuprompt-1.0.6/sohuprompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.565380 sohuprompt-1.0.6/sohuprompt/data_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.566380 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/closed_QA.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/coreference.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/entity_typing.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/generation.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/nli.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/paraphrase.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/processor.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/reading_comprehensation.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/relation.py
--rw-r--r--   0 root         (0) root         (0)    11478 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/summarization.py
--rw-r--r--   0 root         (0) root         (0)     5336 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/topic_classification.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/conditional_generation_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/data_sampler.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/fewglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/huggingface_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/lama_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/nli_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/relation_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-04-26 03:20:48.000000 sohuprompt-1.0.6/sohuprompt/data_utils/text_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/typing_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    15913 2023-04-26 03:20:48.000000 sohuprompt-1.0.6/sohuprompt/default_config.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/lm_bff_trainer.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/pipeline_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.567380 sohuprompt-1.0.6/sohuprompt/plms/
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.568380 sohuprompt-1.0.6/sohuprompt/plms/glm/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/glm.py
--rw-r--r--   0 root         (0) root         (0)    56656 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    15054 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    17877 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/tokenization_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/lm.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/mlm.py
--rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/seq2seq.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/utils.py
--rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompt_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.569380 sohuprompt-1.0.6/sohuprompt/prompts/
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/automatic_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/generation_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/knowledgeable_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/manual_template.py
--rw-r--r--   0 root         (0) root         (0)     9524 2023-04-26 03:24:53.000000 sohuprompt-1.0.6/sohuprompt/prompts/manual_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/mixed_template.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/one2one_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prefix_tuning_template.py
--rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prompt_generator.py
--rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prototypical_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/ptr_prompts.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/ptuning_prompts.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/soft_template.py
--rw-r--r--   0 root         (0) root         (0)     9069 2023-04-24 04:19:02.000000 sohuprompt-1.0.6/sohuprompt/prompts/soft_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/protoverb_trainer.py
--rw-r--r--   0 root         (0) root         (0)    31328 2023-04-26 04:32:13.000000 sohuprompt-1.0.6/sohuprompt/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/sohuprompt/utils/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    10852 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/crossfit_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/cuda.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-26 04:32:31.000000 sohuprompt-1.0.6/sohuprompt/utils/logging.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/metrics.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/reproduciblity.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.564380 sohuprompt-1.0.6/sohuprompt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6491 2023-04-28 01:53:01.000000 sohuprompt-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      762 2023-05-31 02:43:34.000000 sohuprompt-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-05-31 02:55:25.000000 sohuprompt-1.0.7/sohuprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/data_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/closed_QA.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/coreference.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/entity_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/generation.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/nli.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/paraphrase.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/processor.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/reading_comprehensation.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/relation.py
+-rw-r--r--   0 root         (0) root         (0)    11478 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/summarization.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/ZH/topic_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/conditional_generation_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/data_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/fewglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/huggingface_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/lama_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/nli_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/relation_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-04-26 03:20:48.000000 sohuprompt-1.0.7/sohuprompt/data_utils/text_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/typing_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/data_utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15913 2023-04-26 03:20:48.000000 sohuprompt-1.0.7/sohuprompt/default_config.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/lm_bff_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/pipeline_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/plms/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2023-05-31 02:51:43.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/glm.py
+-rw-r--r--   0 root         (0) root         (0)    57620 2023-05-31 02:51:51.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    15054 2023-05-31 02:51:59.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    17047 2023-05-31 02:52:03.000000 sohuprompt-1.0.7/sohuprompt/plms/glm/tokenization_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/lm.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/mlm.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/seq2seq.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/plms/utils.py
+-rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompt_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/prompts/
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/automatic_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/generation_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/knowledgeable_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/manual_template.py
+-rw-r--r--   0 root         (0) root         (0)     9524 2023-04-26 03:24:53.000000 sohuprompt-1.0.7/sohuprompt/prompts/manual_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/mixed_template.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/one2one_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/prefix_tuning_template.py
+-rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/prompt_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/prototypical_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/ptr_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/ptuning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/prompts/soft_template.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2023-04-24 04:19:02.000000 sohuprompt-1.0.7/sohuprompt/prompts/soft_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/protoverb_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    31406 2023-05-25 09:56:47.000000 sohuprompt-1.0.7/sohuprompt/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt/utils/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    10852 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/crossfit_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/cuda.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-26 04:32:31.000000 sohuprompt-1.0.7/sohuprompt/utils/logging.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/reproduciblity.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 06:32:08.000000 sohuprompt-1.0.7/sohuprompt/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-31 02:58:19.000000 sohuprompt-1.0.7/sohuprompt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sohuprompt-1.0.6/README.md` & `sohuprompt-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  
 
 - ❗️ 2023年4月：版本更新，支持[ChatGLM](https://github.com/THUDM/ChatGLM-6B), 可以使用SohuPrompt工具对ChatGLM进行微调。
 - 2023年4月：SohuPrompt v1.0.1版本发布，欢迎大家为SohuPrompt贡献代码。
 
 ## 预览
 
-Prompt-learning是最新的训练范式，它可以将预训练语言模型（PLMs）更好的适配下游NLP任务。SohuPrompt库提供了一个标准、灵活和可扩展的框架，用于部署prompt-learning流水线，它支持直接从[huggingface transformers](https://github.com/huggingface/transformers)加载PLMs。在未来，我们将支持[deepspeed](https://github.com/microsoft/DeepSpeed)或[colossal ai](https://github.com/hpcaitech/ColossalAI)来加快训练和预测速度。
+Prompt-learning是最新的训练范式，它可以将预训练语言模型（PLMs）更好的适配下游NLP任务，详细了解请参考[Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing](https://arxiv.org/pdf/2107.13586.pdf)。SohuPrompt库提供了一个标准、灵活和可扩展的框架，用于部署prompt-learning流水线，它支持直接从[huggingface transformers](https://github.com/huggingface/transformers)加载PLMs。在未来，我们将支持[deepspeed](https://github.com/microsoft/DeepSpeed)或[colossal ai](https://github.com/hpcaitech/ColossalAI)来加快训练和预测速度。
 
 
 <div align="center">
 
 
 <img src="https://z3.ax1x.com/2021/11/03/IAdT3D.png" width="85%" align="center"/>
```

#### html2text {}

```diff
@@ -2,15 +2,18 @@
                  [https://s1.ax1x.com/2023/04/23/p9e0XDA.png]
                       é¢è§ â¢ å®è£ â¢ å¿«éå¼å§
 ![version](https://img.shields.io/badge/version-v1.0.6-green) ## æ°é» -
 âï¸ 2023å¹´4æï¼çæ¬æ´æ°ï¼æ¯æ[ChatGLM](https://github.com/THUDM/
 ChatGLM-6B), å¯ä»¥ä½¿ç¨SohuPromptå·¥å·å¯¹ChatGLMè¿è¡å¾®è°ã -
 2023å¹´4æï¼SohuPrompt
 v1.0.1çæ¬åå¸ï¼æ¬¢è¿å¤§å®¶ä¸ºSohuPromptè´¡ç®ä»£ç ã ## é¢è§ Prompt-
-learningæ¯ææ°çè®­ç»èå¼ï¼å®å¯ä»¥å°é¢è®­ç»è¯­è¨æ¨¡åï¼PLMsï¼æ´å¥½çééä¸æ¸¸NLPä»»å¡ãSohuPromptåºæä¾äºä¸ä¸ªæ åãçµæ´»åå¯æ©å±çæ¡æ¶ï¼ç¨äºé¨ç½²prompt-
+learningæ¯ææ°çè®­ç»èå¼ï¼å®å¯ä»¥å°é¢è®­ç»è¯­è¨æ¨¡åï¼PLMsï¼æ´å¥½çééä¸æ¸¸NLPä»»å¡ï¼è¯¦ç»äºè§£è¯·åè
+[Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in
+Natural Language Processing](https://arxiv.org/pdf/
+2107.13586.pdf)ãSohuPromptåºæä¾äºä¸ä¸ªæ åãçµæ´»åå¯æ©å±çæ¡æ¶ï¼ç¨äºé¨ç½²prompt-
 learningæµæ°´çº¿ï¼å®æ¯æç´æ¥ä»[huggingface transformers](https://
 github.com/huggingface/transformers)å è½½PLMsãå¨æªæ¥ï¼æä»¬å°æ¯æ
 [deepspeed](https://github.com/microsoft/DeepSpeed)æ[colossal ai](https://
 github.com/hpcaitech/ColossalAI)æ¥å å¿«è®­ç»åé¢æµéåº¦ã
                   [https://z3.ax1x.com/2021/11/03/IAdT3D.png]
 ## å®è£ ### ä½¿ç¨ pip ```shell pip install sohuprompt ```
 ä½ ä¹å¯ä»¥ä»gitlabæºå®è£ææ°çæ¬çSohuPromptã ## å¿«éå¼å§ ###
```

### Comparing `sohuprompt-1.0.6/setup.py` & `sohuprompt-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='sohuprompt',
-        version='1.0.6',
+        version='1.0.7',
         packages=find_packages(),  # 查找包的路径
         # package_dir={'': 'src'},  # 包的root路径映射到的实际路径
         # include_package_data=False,
         # package_data={'data': []},
         description='A python lib for sohuprompt',
         # long_description='',
         author='senhaowang,chencheng',
         author_email='senhaowang@sohu-inc.com',
         # url='http://www.xxxxx.com/',  # homepage
         license='MIT',
-        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'scikit-learn', 'jieba', 'tensorboard==2.9.0', 'icetk', 'yacs', 'rouge', 'openpyxl'],
-        )
+        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'scikit-learn', 'jieba', 'tensorboard==2.9.0', 'icetk', 'yacs', 'rouge', 'openpyxl', 'tensorboardX',"nltk"],
+)
```

### Comparing `sohuprompt-1.0.6/sohuprompt/config.py` & `sohuprompt-1.0.7/sohuprompt/config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/closed_QA.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/closed_QA.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/coreference.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/coreference.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/entity_typing.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/entity_typing.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/generation.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/generation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/nli.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/nli.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/paraphrase.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/paraphrase.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/reading_comprehensation.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/reading_comprehensation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/relation.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/relation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/sentiment.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/sentiment.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/summarization.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/summarization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/topic_classification.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/ZH/topic_classification.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/__init__.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/conditional_generation_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/conditional_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/data_processor.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/data_sampler.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/data_sampler.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/fewglue_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/fewglue_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/huggingface_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/lama_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/lama_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/nli_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/nli_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/relation_classification_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/relation_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/text_classification_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/typing_dataset.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/typing_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/data_utils/utils.py` & `sohuprompt-1.0.7/sohuprompt/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/default_config.py` & `sohuprompt-1.0.7/sohuprompt/default_config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/lm_bff_trainer.py` & `sohuprompt-1.0.7/sohuprompt/lm_bff_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/pipeline_base.py` & `sohuprompt-1.0.7/sohuprompt/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/__init__.py` & `sohuprompt-1.0.7/sohuprompt/plms/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/glm/configuration_chatglm.py` & `sohuprompt-1.0.7/sohuprompt/plms/glm/configuration_chatglm.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             hidden_size=4096,
             num_layers=28,
             num_attention_heads=32,
             layernorm_epsilon=1e-5,
             use_cache=False,
             bos_token_id=150004,
             eos_token_id=150005,
+            mask_token_id=150000,
+            gmask_token_id=150001,
             pad_token_id=0,
             max_sequence_length=2048,
             inner_hidden_size=16384,
             position_encoding_2d=True,
             quantization_bit=0,
             pre_seq_len=None,
             prefix_projection=False,
@@ -82,14 +84,16 @@
         self.max_sequence_length = max_sequence_length
         self.layernorm_epsilon = layernorm_epsilon
         self.inner_hidden_size = inner_hidden_size
         self.use_cache = use_cache
         self.bos_token_id = bos_token_id
         self.eos_token_id = eos_token_id
         self.pad_token_id = pad_token_id
+        self.mask_token_id = mask_token_id
+        self.gmask_token_id = gmask_token_id
         self.position_encoding_2d = position_encoding_2d
         self.quantization_bit = quantization_bit
         self.pre_seq_len = pre_seq_len
         self.prefix_projection = prefix_projection
 
         super().__init__(
             pad_token_id=pad_token_id,
```

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/glm/glm.py` & `sohuprompt-1.0.7/sohuprompt/plms/glm/glm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/glm/modeling_chatglm.py` & `sohuprompt-1.0.7/sohuprompt/plms/glm/modeling_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ]
 
 
 class InvalidScoreLogitsProcessor(LogitsProcessor):
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor) -> torch.FloatTensor:
         if torch.isnan(scores).any() or torch.isinf(scores).any():
             scores.zero_()
-            scores[..., 20005] = 5e4
+            scores[..., 5] = 5e4
         return scores
 
 
 def load_tf_weights_in_chatglm_6b(model, config, tf_checkpoint_path):
     """Load tf checkpoints in a pytorch model."""
     try:
         import re
@@ -276,18 +276,16 @@
     output_size = (query_layer.size(1), query_layer.size(2), query_layer.size(0), key_layer.size(0))
 
     # [sq, b, np, hn] -> [sq, b * np, hn]
     query_layer = query_layer.view(output_size[2], output_size[0] * output_size[1], -1)
     # [sk, b, np, hn] -> [sk, b * np, hn]
     key_layer = key_layer.view(output_size[3], output_size[0] * output_size[1], -1)
 
-    matmul_result = torch.empty(
-        output_size[0] * output_size[1],
-        output_size[2],
-        output_size[3],
+    matmul_result = torch.zeros(
+        1, 1, 1,
         dtype=query_layer.dtype,
         device=query_layer.device,
     )
 
     matmul_result = torch.baddbmm(
         matmul_result,
         query_layer.transpose(0, 1),  # [b * np, sq, hn]
@@ -344,18 +342,26 @@
     context_layer = context_layer.view(*new_context_layer_shape)
 
     outputs = (context_layer, present, attention_probs)
 
     return outputs
 
 
+def default_init(cls, *args, **kwargs):
+    return cls(*args, **kwargs)
+
+
 class SelfAttention(torch.nn.Module):
     def __init__(self, hidden_size, num_attention_heads,
                  layer_id, hidden_size_per_attention_head=None, bias=True,
-                 params_dtype=torch.float, position_encoding_2d=True):
+                 params_dtype=torch.float, position_encoding_2d=True, empty_init=True):
+        if empty_init:
+            init_method = skip_init
+        else:
+            init_method = default_init
         super(SelfAttention, self).__init__()
 
         self.layer_id = layer_id
         self.hidden_size = hidden_size
         self.hidden_size_per_partition = hidden_size
         self.num_attention_heads = num_attention_heads
         self.num_attention_heads_per_partition = num_attention_heads
@@ -375,23 +381,23 @@
             self.hidden_size_per_attention_head = hidden_size // num_attention_heads
         else:
             self.hidden_size_per_attention_head = hidden_size_per_attention_head
 
         self.inner_hidden_size = num_attention_heads * self.hidden_size_per_attention_head
 
         # Strided linear layer.
-        self.query_key_value = skip_init(
+        self.query_key_value = init_method(
             torch.nn.Linear,
             hidden_size,
             3 * self.inner_hidden_size,
             bias=bias,
             dtype=params_dtype,
         )
 
-        self.dense = skip_init(
+        self.dense = init_method(
             torch.nn.Linear,
             self.inner_hidden_size,
             hidden_size,
             bias=bias,
             dtype=params_dtype,
         )
 
@@ -496,33 +502,37 @@
         # dim=-1 breaks in jit for pt<1.10
         x1, x2 = x.chunk(2, dim=(x.ndim - 1))
         return x1 * self.activation_fn(x2)
 
 
 class GLU(torch.nn.Module):
     def __init__(self, hidden_size, inner_hidden_size=None,
-                 layer_id=None, bias=True, activation_func=gelu, params_dtype=torch.float):
+                 layer_id=None, bias=True, activation_func=gelu, params_dtype=torch.float, empty_init=True):
         super(GLU, self).__init__()
+        if empty_init:
+            init_method = skip_init
+        else:
+            init_method = default_init
         self.layer_id = layer_id
         self.activation_func = activation_func
 
         # Project to 4h.
         self.hidden_size = hidden_size
         if inner_hidden_size is None:
             inner_hidden_size = 4 * hidden_size
         self.inner_hidden_size = inner_hidden_size
-        self.dense_h_to_4h = skip_init(
+        self.dense_h_to_4h = init_method(
             torch.nn.Linear,
             self.hidden_size,
             self.inner_hidden_size,
             bias=bias,
             dtype=params_dtype,
         )
         # Project back to h.
-        self.dense_4h_to_h = skip_init(
+        self.dense_4h_to_h = init_method(
             torch.nn.Linear,
             self.inner_hidden_size,
             self.hidden_size,
             bias=bias,
             dtype=params_dtype,
         )
 
@@ -550,15 +560,16 @@
             layer_id,
             inner_hidden_size=None,
             hidden_size_per_attention_head=None,
             layernorm=LayerNorm,
             use_bias=True,
             params_dtype=torch.float,
             num_layers=28,
-            position_encoding_2d=True
+            position_encoding_2d=True,
+            empty_init=True
     ):
         super(GLMBlock, self).__init__()
         # Set output layer initialization if not provided.
 
         self.layer_id = layer_id
 
         # Layernorm on the input data.
@@ -570,29 +581,31 @@
         self.attention = SelfAttention(
             hidden_size,
             num_attention_heads,
             layer_id,
             hidden_size_per_attention_head=hidden_size_per_attention_head,
             bias=use_bias,
             params_dtype=params_dtype,
-            position_encoding_2d=self.position_encoding_2d
+            position_encoding_2d=self.position_encoding_2d,
+            empty_init=empty_init
         )
 
         # Layernorm on the input data.
         self.post_attention_layernorm = layernorm(hidden_size, eps=layernorm_epsilon)
 
         self.num_layers = num_layers
 
         # GLU
         self.mlp = GLU(
             hidden_size,
             inner_hidden_size=inner_hidden_size,
             bias=use_bias,
             layer_id=layer_id,
             params_dtype=params_dtype,
+            empty_init=empty_init
         )
 
     def forward(
             self,
             hidden_states: torch.Tensor,
             position_ids,
             attention_mask: torch.Tensor,
@@ -672,32 +685,34 @@
         for i, context_length in enumerate(context_lengths):
             attention_mask[i, :, :context_length] = 1
         attention_mask.unsqueeze_(1)
         attention_mask = (attention_mask < 0.5).bool()
 
         return attention_mask
 
-    def get_position_ids(self, input_ids, mask_positions, device, gmask=False):
+    def get_position_ids(self, input_ids, mask_positions, device, use_gmasks=None):
         batch_size, seq_length = input_ids.shape
+        if use_gmasks is None:
+            use_gmasks = [False] * batch_size
         context_lengths = [seq.tolist().index(self.config.bos_token_id) for seq in input_ids]
         if self.position_encoding_2d:
             position_ids = torch.arange(seq_length, dtype=torch.long, device=device).unsqueeze(0).repeat(batch_size, 1)
             for i, context_length in enumerate(context_lengths):
                 position_ids[i, context_length:] = mask_positions[i]
             block_position_ids = [torch.cat((
                 torch.zeros(context_length, dtype=torch.long, device=device),
                 torch.arange(seq_length - context_length, dtype=torch.long, device=device) + 1
             )) for context_length in context_lengths]
             block_position_ids = torch.stack(block_position_ids, dim=0)
             position_ids = torch.stack((position_ids, block_position_ids), dim=1)
         else:
             position_ids = torch.arange(seq_length, dtype=torch.long, device=device).unsqueeze(0).repeat(batch_size, 1)
-            if not gmask:
-                for i, context_length in enumerate(context_lengths):
-                    position_ids[context_length:] = mask_positions[i]
+            for i, context_length in enumerate(context_lengths):
+                if not use_gmasks[i]:
+                    position_ids[i, context_length:] = mask_positions[i]
 
         return position_ids
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, ChatGLMModel):
             module.gradient_checkpointing = value
 
@@ -779,32 +794,35 @@
     To behave as an decoder the model needs to be initialized with the
     `is_decoder` argument of the configuration set to `True`.
     To be used in a Seq2Seq model, the model needs to initialized with both `is_decoder`
     argument and `add_cross_attention` set to `True`; an
     `encoder_hidden_states` is then expected as an input to the forward pass.
     """
 
-    def __init__(self, config: ChatGLMConfig):
+    def __init__(self, config: ChatGLMConfig, empty_init=True):
         super().__init__(config)
-
+        if empty_init:
+            init_method = skip_init
+        else:
+            init_method = default_init
         # recording parameters
         self.max_sequence_length = config.max_sequence_length
         self.hidden_size = config.hidden_size
         self.params_dtype = torch.half
         self.num_attention_heads = config.num_attention_heads
         self.vocab_size = config.vocab_size
         self.num_layers = config.num_layers
         self.layernorm_epsilon = config.layernorm_epsilon
         self.inner_hidden_size = config.inner_hidden_size
         self.hidden_size_per_attention_head = self.hidden_size // self.num_attention_heads
         self.position_encoding_2d = config.position_encoding_2d
         self.pre_seq_len = config.pre_seq_len
         self.prefix_projection = config.prefix_projection
 
-        self.word_embeddings = skip_init(
+        self.word_embeddings = init_method(
             torch.nn.Embedding,
             num_embeddings=self.vocab_size, embedding_dim=self.hidden_size,
             dtype=self.params_dtype
         )
         self.gradient_checkpointing = False
 
         def get_layer(layer_id):
@@ -815,14 +833,15 @@
                 layer_id,
                 inner_hidden_size=self.inner_hidden_size,
                 hidden_size_per_attention_head=self.hidden_size_per_attention_head,
                 layernorm=LayerNorm,
                 use_bias=True,
                 params_dtype=self.params_dtype,
                 position_encoding_2d=self.position_encoding_2d,
+                empty_init=empty_init
             )
 
         self.layers = torch.nn.ModuleList(
             [get_layer(layer_id) for layer_id in range(self.num_layers)]
         )
 
         # Final layer norm before output.
@@ -895,15 +914,15 @@
                 use_cache = False
 
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
         elif input_ids is not None:
             batch_size, seq_length = input_ids.shape[:2]
         elif inputs_embeds is not None:
-            batch_size, seq_length, _ = inputs_embeds.shape[:3]
+            batch_size, seq_length = inputs_embeds.shape[:2]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
         if inputs_embeds is None:
             inputs_embeds = self.word_embeddings(input_ids)
 
         if past_key_values is None:
@@ -917,24 +936,29 @@
                 attention_mask = self.get_masks(
                     input_ids,
                     device=input_ids.device
                 )
 
 
             if position_ids is None:
-                MASK, gMASK = 150000, 150001
-                mask_token = MASK if MASK in input_ids else gMASK
-                use_gmask = False if MASK in input_ids else gMASK
+                MASK, gMASK = self.config.mask_token_id, self.config.gmask_token_id
+                seqs = input_ids.tolist()
+
+                mask_positions, use_gmasks = [], []
+                for seq in seqs:
+                    mask_token = gMASK if gMASK in seq else MASK
+                    use_gmask = mask_token == gMASK
+                    mask_positions.append(seq.index(mask_token))
+                    use_gmasks.append(use_gmask)
 
-                mask_positions = [seq.tolist().index(mask_token) for seq in input_ids]
                 position_ids = self.get_position_ids(
                     input_ids,
                     mask_positions=mask_positions,
                     device=input_ids.device,
-                    gmask=use_gmask
+                    use_gmasks=use_gmasks
                 )
 
         if self.pre_seq_len is not None and attention_mask is not None:
             prefix_attention_mask = torch.ones(batch_size, 1, input_ids.size(-1), self.pre_seq_len).to(
                 attention_mask.device)
             prefix_attention_mask = (prefix_attention_mask < 0.5).bool()
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=3)
@@ -944,20 +968,16 @@
 
         presents = () if use_cache else None
         all_self_attentions = () if output_attentions else None
         all_hidden_states = () if output_hidden_states else None
 
         if attention_mask is None:
             attention_mask = torch.zeros(1, 1, device=input_ids.device).bool()
-
         else:
-            if input_ids is None:
-                attention_mask = attention_mask.to(inputs_embeds.device)
-            else:
-                attention_mask = attention_mask.to(input_ids.device)
+            attention_mask = attention_mask.to(hidden_states.device)
 
         for i, layer in enumerate(self.layers):
 
             if output_hidden_states:
                 all_hidden_states = all_hidden_states + (hidden_states,)
             layer_past = past_key_values[i]
 
@@ -1005,27 +1025,31 @@
             past_key_values=presents,
             hidden_states=all_hidden_states,
             attentions=all_self_attentions,
         )
 
 
 class ChatGLMForConditionalGeneration(ChatGLMPreTrainedModel):
-    def __init__(self, config: ChatGLMConfig):
+    def __init__(self, config: ChatGLMConfig, empty_init=True):
         super().__init__(config)
+        if empty_init:
+            init_method = skip_init
+        else:
+            init_method = default_init
 
         # self.hidden_size = config.hidden_size
         # self.params_dtype = torch.half
         # self.vocab_size = config.vocab_size
         self.max_sequence_length = config.max_sequence_length
 
         self.position_encoding_2d = config.position_encoding_2d
 
-        self.transformer = ChatGLMModel(config)
+        self.transformer = ChatGLMModel(config, empty_init=empty_init)
 
-        self.lm_head = skip_init(
+        self.lm_head = init_method(
             nn.Linear,
             config.hidden_size,
             config.vocab_size,
             bias=False,
             dtype=torch.half
         )
 
@@ -1083,19 +1107,22 @@
             past: Optional[torch.Tensor] = None,
             past_key_values: Optional[torch.Tensor] = None,
             attention_mask: Optional[torch.Tensor] = None,
             position_ids: Optional[torch.Tensor] = None,
             **kwargs
     ) -> dict:
         batch_size, seq_length = input_ids.shape
-        MASK, gMASK = 150000, 150001
-        mask_token = MASK if MASK in input_ids else gMASK
-        use_gmask = False if MASK in input_ids else gMASK
+        MASK, gMASK = self.config.mask_token_id, self.config.gmask_token_id
         seqs = input_ids.tolist()
-        mask_positions = [seq.index(mask_token) for seq in seqs]
+        mask_positions, use_gmasks = [], []
+        for seq in seqs:
+            mask_token = gMASK if gMASK in seq else MASK
+            use_gmask = mask_token == gMASK
+            mask_positions.append(seq.index(mask_token))
+            use_gmasks.append(use_gmask)
 
         # only last token for input_ids if past is not None
         if past is not None or past_key_values is not None:
             last_token = input_ids[:, -1].unsqueeze(-1)
             if attention_mask is not None and attention_mask.dtype == torch.bool:
                 attention_mask = attention_mask[:, :, -1:]
             else:
@@ -1130,15 +1157,15 @@
                     device=input_ids.device
                 )
             if position_ids is None:
                 position_ids = self.get_position_ids(
                     input_ids,
                     device=input_ids.device,
                     mask_positions=mask_positions,
-                    gmask=use_gmask
+                    use_gmasks=use_gmasks
                 )
 
             return {
                 "input_ids": input_ids,
                 "past_key_values": past,
                 "position_ids": position_ids,
                 "attention_mask": attention_mask
```

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/glm/quantization.py` & `sohuprompt-1.0.7/sohuprompt/plms/glm/quantization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/glm/tokenization_chatglm.py` & `sohuprompt-1.0.7/sohuprompt/plms/glm/tokenization_chatglm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,85 @@
 """Tokenization classes for ChatGLM."""
 from typing import List, Optional, Union
 import os
 
 from transformers.tokenization_utils import PreTrainedTokenizer
-from icetk.text_tokenizer import TextTokenizer
-import icetk.sentencepiece_model_pb2 as sp_model
 from transformers.utils import logging, PaddingStrategy
 from transformers.tokenization_utils_base import EncodedInput, BatchEncoding
 from typing import Dict
+import sentencepiece as spm
 import numpy as np
 
 logger = logging.get_logger(__name__)
 
 PRETRAINED_POSITIONAL_EMBEDDINGS_SIZES = {
     "THUDM/chatglm-6b": 2048,
 }
 
 
+class TextTokenizer:
+    def __init__(self, model_path):
+        self.sp = spm.SentencePieceProcessor()
+        self.sp.Load(model_path)
+        self.num_tokens = self.sp.vocab_size()
+
+    def encode(self, text):
+        return self.sp.EncodeAsIds(text)
+
+    def decode(self, ids: List[int]):
+        return self.sp.DecodeIds(ids)
+
+    def tokenize(self, text):
+        return self.sp.EncodeAsPieces(text)
+
+    def convert_tokens_to_string(self, tokens):
+        return self.sp.DecodePieces(tokens)
+
+    def convert_tokens_to_ids(self, tokens):
+        return [self.sp.PieceToId(token) for token in tokens]
+
+    def convert_token_to_id(self, token):
+        return self.sp.PieceToId(token)
+
+    def convert_id_to_token(self, idx):
+        return self.sp.IdToPiece(idx)
+
+    def __len__(self):
+        return self.num_tokens
+
+
 class SPTokenizer:
     def __init__(
-        self,
-        vocab_file,
-        max_blank_length=80,
-        byte_fallback=True,
+            self,
+            vocab_file,
+            num_image_tokens=20000,
+            max_blank_length=80,
+            byte_fallback=True,
     ):
         assert vocab_file is not None
         self.vocab_file = vocab_file
+        self.num_image_tokens = num_image_tokens
         self.special_tokens = ["[MASK]", "[gMASK]", "[sMASK]", "<unused_0>", "<sop>", "<eop>", "<ENC>", "<dBLOCK>"]
         self.max_blank_length = max_blank_length
         self.byte_fallback = byte_fallback
-        self.text_tokenizer = self._build_text_tokenizer(encode_special_tokens=False)
-        self.special_text_tokenizer = self._build_text_tokenizer(encode_special_tokens=True)
-
-    @staticmethod
-    def _configure_tokenizer(
-        text_tokenizer: TextTokenizer,
-        special_tokens: List[str],
-        max_blank_length: int,
-        byte_fallback: bool,
-        encode_special_tokens=False,
-    ):
-        # special token
-        special_token_type = 4 if encode_special_tokens else 3  # 3 - CONTROL, 4 - USER_DEFINE
-        for token in special_tokens:
-            text_tokenizer.proto.pieces.append(
-                sp_model.ModelProto.SentencePiece(piece=token, score=0.0, type=special_token_type)
-            )
-        # whitespaces
-        for token in [SPTokenizer.get_tab_token()] + [
-            SPTokenizer.get_blank_token(i) for i in range(2, max_blank_length + 1)
-        ]:
-            text_tokenizer.proto.pieces.append(sp_model.ModelProto.SentencePiece(piece=token, score=0.0, type=4))
-        # byte fallback
-        if byte_fallback:
-            text_tokenizer.proto.trainer_spec.byte_fallback = True
-            for i in range(256):
-                text_tokenizer.proto.pieces.append(
-                    sp_model.ModelProto.SentencePiece(piece="<0x{:02X}>".format(i), score=0.0, type=6)
-                )
-        text_tokenizer.refresh()
-
-    def _build_text_tokenizer(self, encode_special_tokens=False):
-        tokenizer = TextTokenizer(self.vocab_file)
-        self._configure_tokenizer(
-            tokenizer, self.special_tokens, self.max_blank_length, self.byte_fallback, encode_special_tokens
-        )
-        return tokenizer
+        self.text_tokenizer = TextTokenizer(vocab_file)
 
-    def _get_text_tokenizer(self, encode_special_tokens=False):
-        if encode_special_tokens:
-            return self.special_text_tokenizer
-        else:
-            return self.text_tokenizer
+    def _get_text_tokenizer(self):
+        return self.text_tokenizer
 
     @staticmethod
     def get_blank_token(length: int):
         assert length >= 2
         return f"<|blank_{length}|>"
 
     @staticmethod
     def get_tab_token():
         return f"<|tab|>"
 
     @property
-    def num_image_tokens(self):
-        return 20000
-
-    @property
     def num_text_tokens(self):
         return self.text_tokenizer.num_tokens
 
     @property
     def num_tokens(self):
         return self.num_image_tokens + self.num_text_tokens
 
@@ -105,54 +94,63 @@
         if linebreak:
             text = text.replace("\n", "<n>")
         if whitespaces:
             text = self._encode_whitespaces(text, max_len=self.max_blank_length)
         return text
 
     def encode(
-        self, text: str, linebreak=True, whitespaces=True, special_tokens=False, add_dummy_prefix=True
+            self, text: str, linebreak=True, whitespaces=True, add_dummy_prefix=True
     ) -> List[int]:
         """
         @param text: Text to encode.
         @param linebreak: Whether to encode newline (\n) in text.
         @param whitespaces: Whether to encode multiple whitespaces or tab in text, useful for source code encoding.
         @param special_tokens: Whether to encode special token ([MASK], [gMASK], etc.) in text.
         @param add_dummy_prefix: Whether to add dummy blank space in the beginning.
         """
         text = self._preprocess(text, linebreak, whitespaces)
         if not add_dummy_prefix:
             text = "<n>" + text
-        tmp = self._get_text_tokenizer(encode_special_tokens=special_tokens).encode(text)
+        tmp = self._get_text_tokenizer().encode(text)
         tokens = [x + self.num_image_tokens for x in tmp]
         return tokens if add_dummy_prefix else tokens[2:]
 
-    def decode(self, text_ids: List[int], special_tokens=False) -> str:
-        ids = [int(_id) - self.num_image_tokens for _id in text_ids]
-        ids = [_id for _id in ids if _id >= 0]
-        text = self._get_text_tokenizer(encode_special_tokens=special_tokens).decode(ids)
+    def postprocess(self, text):
         text = text.replace("<n>", "\n")
         text = text.replace(SPTokenizer.get_tab_token(), "\t")
         for i in range(2, self.max_blank_length + 1):
             text = text.replace(self.get_blank_token(i), " " * i)
         return text
 
+    def decode(self, text_ids: List[int]) -> str:
+        ids = [int(_id) - self.num_image_tokens for _id in text_ids]
+        ids = [_id for _id in ids if _id >= 0]
+        text = self._get_text_tokenizer().decode(ids)
+        text = self.postprocess(text)
+        return text
+
+    def decode_tokens(self, tokens: List[str]) -> str:
+        text = self._get_text_tokenizer().convert_tokens_to_string(tokens)
+        text = self.postprocess(text)
+        return text
+
     def tokenize(
-        self, text: str, linebreak=True, whitespaces=True, special_tokens=False, add_dummy_prefix=True
+            self, text: str, linebreak=True, whitespaces=True, add_dummy_prefix=True
     ) -> List[str]:
         """
         @param text: Text to encode.
         @param linebreak: Whether to encode newline (\n) in text.
         @param whitespaces: Whether to encode multiple whitespaces or tab in text, useful for source code encoding.
         @param special_tokens: Whether to encode special token ([MASK], [gMASK], etc.) in text.
         @param add_dummy_prefix: Whether to add dummy blank space in the beginning.
         """
         text = self._preprocess(text, linebreak, whitespaces)
         if not add_dummy_prefix:
             text = "<n>" + text
-        tokens = self._get_text_tokenizer(encode_special_tokens=special_tokens).tokenize(text)
+        tokens = self._get_text_tokenizer().tokenize(text)
         return tokens if add_dummy_prefix else tokens[2:]
 
     def __getitem__(self, x: Union[int, str]):
         if isinstance(x, int):
             if x < self.num_image_tokens:
                 return "<image_{}>".format(x)
             else:
@@ -180,52 +178,69 @@
     model_input_names = ["input_ids", "attention_mask", "position_ids"]
 
     def __init__(
             self,
             vocab_file,
             do_lower_case=False,
             remove_space=False,
-            bos_token='sop',
-            eos_token='eos',
-            eop_token='eop',
+            bos_token='<sop>',
+            eos_token='<eop>',
+            end_token='</s>',
             mask_token='[MASK]',
             gmask_token='[gMASK]',
             padding_side="left",
+            pad_token="<pad>",
+            unk_token="<unk>",
+            num_image_tokens=20000,
             **kwargs
     ) -> None:
         super().__init__(
             do_lower_case=do_lower_case,
             remove_space=remove_space,
             padding_side=padding_side,
+            bos_token=bos_token,
+            eos_token=eos_token,
+            end_token=end_token,
+            mask_token=mask_token,
+            gmask_token=gmask_token,
+            pad_token=pad_token,
+            unk_token=unk_token,
+            num_image_tokens=num_image_tokens,
             **kwargs
         )
 
         self.do_lower_case = do_lower_case
         self.remove_space = remove_space
         self.vocab_file = vocab_file
 
         self.bos_token = bos_token
         self.eos_token = eos_token
-        self.eop_token = eop_token
+        self.end_token = end_token
         self.mask_token = mask_token
         self.gmask_token = gmask_token
 
-        self.sp_tokenizer = SPTokenizer(vocab_file)
+        self.sp_tokenizer = SPTokenizer(vocab_file, num_image_tokens=num_image_tokens)
 
         """ Initialisation """
 
     @property
-    def eop_token_id(self) -> Optional[int]:
+    def gmask_token_id(self) -> Optional[int]:
+        if self.gmask_token is None:
+            return None
+        return self.convert_tokens_to_ids(self.gmask_token)
+
+    @property
+    def end_token_id(self) -> Optional[int]:
         """
-        `Optional[int]`: Id of the end of sentence token in the vocabulary. Returns `None` if the token has not been
+        `Optional[int]`: Id of the end of context token in the vocabulary. Returns `None` if the token has not been
         set.
         """
-        if self.eop_token is None:
+        if self.end_token is None:
             return None
-        return self.convert_tokens_to_ids(self.eop_token)
+        return self.convert_tokens_to_ids(self.end_token)
 
     @property
     def vocab_size(self):
         """ Returns vocab size """
         return self.sp_tokenizer.num_tokens
 
     def get_vocab(self):
@@ -249,37 +264,29 @@
         """ Returns a tokenized string. """
         text = self.preprocess_text(text)
 
         seq = self.sp_tokenizer.tokenize(text)
 
         return seq
 
-    def decode(
+    def convert_tokens_to_string(self, tokens: List[str]) -> str:
+        return self.sp_tokenizer.decode_tokens(tokens)
+
+    def _decode(
             self,
-            token_ids: Union[List[int], List[List[int]]],
-            skip_special_tokens: bool = False,
-            clean_up_tokenization_spaces: bool = True,
-            spaces_between_special_tokens: bool = True,
+            token_ids: Union[int, List[int]],
             **kwargs
     ) -> str:
-        if not isinstance(token_ids, list):
+        if isinstance(token_ids, int):
             token_ids = [token_ids]
         if len(token_ids) == 0:
             return ""
-        if isinstance(token_ids[0], list):
-            tokens = []
-            for single_token_ids in token_ids:
-                if self.pad_token_id in single_token_ids:  # remove pad
-                    single_token_ids = list(filter((self.pad_token_id).__ne__, single_token_ids))
-                tokens.append(self.sp_tokenizer.decode(single_token_ids))
-            return (tokens)
-        else:
-            if self.pad_token_id in token_ids:  # remove pad
-                token_ids = list(filter((self.pad_token_id).__ne__, token_ids))
-            return self.sp_tokenizer.decode(token_ids)
+        if self.pad_token_id in token_ids:  # remove pad
+            token_ids = list(filter((self.pad_token_id).__ne__, token_ids))
+        return super()._decode(token_ids, **kwargs)
 
     def _convert_token_to_id(self, token):
         """ Converts a token (str) in an id using the vocab. """
         return self.sp_tokenizer[token]
 
     def _convert_id_to_token(self, index):
         """Converts an index (integer) in a token (str) using the vocab."""
@@ -328,39 +335,28 @@
                 List of IDs to which the special tokens will be added.
             token_ids_1 (`List[int]`, *optional*):
                 Optional second list of IDs for sequence pairs.
 
         Returns:
             `List[int]`: List of [input IDs](../glossary#input-ids) with the appropriate special tokens.
         """
-        mask_ids = self.sp_tokenizer[self.mask_token]
-        gmask_ids = self.sp_tokenizer[self.gmask_token]
-        eop_id = self.sp_tokenizer[self.eop_token]
-        if mask_ids not in token_ids_0 and gmask_ids not in token_ids_0:
-            token_ids_0 += [gmask_ids]
-
-        if token_ids_0[-1] != mask_ids and token_ids_0[-1] != gmask_ids:
-            token_ids_0 += [self.sp_tokenizer[self.eos_token]]
-
-        token_ids_0 += [self.sp_tokenizer[self.bos_token]]
-
+        gmask_id = self.sp_tokenizer[self.gmask_token]
+        eos_id = self.sp_tokenizer[self.eos_token]
+        token_ids_0 = token_ids_0 + [gmask_id, self.sp_tokenizer[self.bos_token]]
         if token_ids_1 is not None:
-            if not token_ids_1 or token_ids_1[-1] != eop_id:
-                token_ids_1 += [eop_id]
-            token_ids_0 += token_ids_1
-
+            token_ids_0 = token_ids_0 + token_ids_1 + [eos_id]
         return token_ids_0
 
     def _pad(
-        self,
-        encoded_inputs: Union[Dict[str, EncodedInput], BatchEncoding],
-        max_length: Optional[int] = None,
-        padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
-        pad_to_multiple_of: Optional[int] = None,
-        return_attention_mask: Optional[bool] = None,
+            self,
+            encoded_inputs: Union[Dict[str, EncodedInput], BatchEncoding],
+            max_length: Optional[int] = None,
+            padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
+            pad_to_multiple_of: Optional[int] = None,
+            return_attention_mask: Optional[bool] = None,
     ) -> dict:
         """
         Pad encoded inputs (on left/right and up to predefined length or max length in the batch)
 
         Args:
             encoded_inputs:
                 Dictionary of tokenized inputs (`List[int]`) or batch of tokenized inputs (`List[List[int]]`).
@@ -408,14 +404,18 @@
                 attention_mask = np.ones((1, seq_length, seq_length))
                 attention_mask = np.tril(attention_mask)
                 attention_mask[:, :, :context_length] = 1
                 attention_mask = np.bool_(attention_mask < 0.5)
                 encoded_inputs["attention_mask"] = attention_mask
 
             if "position_ids" not in encoded_inputs:
+                if bos_token_id in required_input:
+                    context_length = required_input.index(bos_token_id)
+                else:
+                    context_length = seq_length
                 position_ids = np.arange(seq_length, dtype=np.int64)
                 mask_token = mask_token_id if mask_token_id in required_input else gmask_token_id
                 if mask_token in required_input:
                     mask_position = required_input.index(mask_token)
                     position_ids[context_length:] = mask_position
                 block_position_ids = np.concatenate(
                     [np.zeros(context_length, dtype=np.int64),
```

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/lm.py` & `sohuprompt-1.0.7/sohuprompt/plms/lm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/mlm.py` & `sohuprompt-1.0.7/sohuprompt/plms/mlm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/seq2seq.py` & `sohuprompt-1.0.7/sohuprompt/plms/seq2seq.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/plms/utils.py` & `sohuprompt-1.0.7/sohuprompt/plms/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompt_base.py` & `sohuprompt-1.0.7/sohuprompt/prompt_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/__init__.py` & `sohuprompt-1.0.7/sohuprompt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/automatic_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/automatic_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/generation_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/generation_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/knowledgeable_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/knowledgeable_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/manual_template.py` & `sohuprompt-1.0.7/sohuprompt/prompts/manual_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/manual_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/manual_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/mixed_template.py` & `sohuprompt-1.0.7/sohuprompt/prompts/mixed_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/one2one_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/one2one_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/prefix_tuning_template.py` & `sohuprompt-1.0.7/sohuprompt/prompts/prefix_tuning_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/prompt_generator.py` & `sohuprompt-1.0.7/sohuprompt/prompts/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/prototypical_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/prototypical_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/ptr_prompts.py` & `sohuprompt-1.0.7/sohuprompt/prompts/ptr_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/ptuning_prompts.py` & `sohuprompt-1.0.7/sohuprompt/prompts/ptuning_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/soft_template.py` & `sohuprompt-1.0.7/sohuprompt/prompts/soft_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/prompts/soft_verbalizer.py` & `sohuprompt-1.0.7/sohuprompt/prompts/soft_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/protoverb_trainer.py` & `sohuprompt-1.0.7/sohuprompt/protoverb_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/trainer.py` & `sohuprompt-1.0.7/sohuprompt/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from sohuprompt import PromptDataLoader
 from sohuprompt.prompts import *
 from sohuprompt.utils.logging import logger
 from sohuprompt.utils.metrics import classification_metrics, generation_metric
 from transformers import AdamW, get_linear_schedule_with_warmup
 from transformers.optimization import Adafactor, AdafactorSchedule
 from transformers.trainer_pt_utils import LabelSmoother
+from transformers.deepspeed import deepspeed_init, is_deepspeed_zero3_enabled
 from packaging import version
 import time
 
 parsed_torch_version_base = version.parse(version.parse(torch.__version__).base_version)
 
 is_torch_greater_or_equal_than_1_10 = parsed_torch_version_base >= version.parse("1.10")
 is_torch_less_than_1_11 = parsed_torch_version_base < version.parse("1.11")
```

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/calibrate.py` & `sohuprompt-1.0.7/sohuprompt/utils/calibrate.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/crossfit_metrics.py` & `sohuprompt-1.0.7/sohuprompt/utils/crossfit_metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/cuda.py` & `sohuprompt-1.0.7/sohuprompt/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/logging.py` & `sohuprompt-1.0.7/sohuprompt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/metrics.py` & `sohuprompt-1.0.7/sohuprompt/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt/utils/utils.py` & `sohuprompt-1.0.7/sohuprompt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.6/sohuprompt.egg-info/SOURCES.txt` & `sohuprompt-1.0.7/sohuprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

