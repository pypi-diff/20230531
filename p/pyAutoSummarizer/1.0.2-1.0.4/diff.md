# Comparing `tmp/pyAutoSummarizer-1.0.2.tar.gz` & `tmp/pyAutoSummarizer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyAutoSummarizer-1.0.2.tar", last modified: Thu May 25 21:51:01 2023, max compression
+gzip compressed data, was "dist\pyAutoSummarizer-1.0.4.tar", last modified: Wed May 31 14:07:59 2023, max compression
```

## Comparing `pyAutoSummarizer-1.0.2.tar` & `pyAutoSummarizer-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/
--rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3450 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3053 2023-05-25 21:50:09.000000 pyAutoSummarizer-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/
--rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/__init__.py
--rw-rw-rw-   0        0        0    29591 2023-05-18 23:11:32.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/psr.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/
--rw-rw-rw-   0        0        0     3450 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 21:50:59.000000 pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-25 21:51:01.000000 pyAutoSummarizer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      820 2023-05-25 21:49:46.000000 pyAutoSummarizer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/
+-rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4761 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4361 2023-05-31 14:05:55.000000 pyAutoSummarizer-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/
+-rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/__init__.py
+-rw-rw-rw-   0        0        0    31949 2023-05-31 13:56:47.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/psr.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/
+-rw-rw-rw-   0        0        0     4761 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-05-31 14:07:58.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      820 2023-05-31 01:42:33.000000 pyAutoSummarizer-1.0.4/setup.py
```

### Comparing `pyAutoSummarizer-1.0.2/LICENSE` & `pyAutoSummarizer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/PKG-INFO` & `pyAutoSummarizer-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.2
+Version: 1.0.4
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyAutoSummarizer
 
 pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence. 
 
 ## Introduction
 
-pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+
+pyAutoSummarizer stands out for its proficient preprocessing capabilities that pave the way for high-quality text summarization. Recognizing the importance of text normalization, the library offers a range of text cleansing and standardization features. It can convert text to **lowercase**, ensuring uniformity across the data. Additionally, it can **remove accents**, **remove special characters**, and **remove numbers**, which helps mitigate the text's noise. It also offers the functionality to **remove custom words**, enabling users to tailor their preprocessing needs. Notably, pyAutoSummarizer supports **stopwords** removal across various languages, including Arabic, Bengali, Bulgarian, Chinese, Czech, English, Finnish, French, German, Greek, Hebrew, Hind, Hungarian, Italian, Japanese, Korean, Marathi, Persia, Polish, Portuguese-br, Romanian, Russian, Slovak, Spanish, Swedish, Thai, and Ukrainian. The library provides flexibility in sentence segmentation, allowing sentences to be split based on **punctuation**, **character count**, or **word count**. 
 
 To evaluate the quality of the summaries generated, pyAutoSummarizer integrates various metrics such as **Rouge-N**, **Rouge-L**, and **Rouge-S**, which compare the overlap of n-grams, longest common subsequence, and skip-bigram between the generated summary and the reference summary respectively. Additionally, it employs **BLEU** (Bilingual Evaluation Understudy), and **METEOR** (Metric for Evaluation of Translation with Explicit ORdering).
 
 ## Usage
 
 1. Install
 ```bash
@@ -31,13 +33,14 @@
 Extractive Summarization
 - Example 01: TextRank           ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
-Abstractive Summarization. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5))
+Abstractive Summarization. 
+- Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- Example 02: Pegasus (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
 
 - [pyBibX](https://github.com/Valdecy/pyBibX) - A Bibliometric and Scientometric Python Library Powered with Artificial Intelligence Tools
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/psr.py` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/psr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ############################################################################
 
 # Created by: Prof. Valdecy Pereira, D.Sc.
 # UFF - Universidade Federal Fluminense (Brazil)
 # email:  valdecy.pereira@gmail.com
-# pyAutoSummarizer - A Extrative and Abstractive Summarization Library Powered with Artificial Intelligence
+#pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 
 # Citation: 
-# PEREIRA, V. (2023). Project: pyAutoSummarizer, File: pySummarizer.py, GitHub repository: <https://github.com/Valdecy/pyAutoSummarizer>
+# PEREIRA, V. (2023). Project: pyAutoSummarizer, GitHub repository: <https://github.com/Valdecy/pyAutoSummarizer>
 
 ############################################################################
 
 # Required Libraries
 import numpy as np
 import openai 
 import re 
@@ -25,14 +25,15 @@
 
 from itertools import combinations
 from sentence_transformers import SentenceTransformer 
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
 from transformers import T5ForConditionalGeneration, T5Tokenizer
+from transformers import PegasusForConditionalGeneration, PegasusTokenizer
 
 ############################################################################
 
 class summarization():
     def __init__(self, text, stop_words = ['en'], n_words = 0, n_chars = 0, lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = [], verbose = False):
         self.p_sw     = stop_words
         self.p_lc     = lowercase
@@ -131,52 +132,68 @@
                 print('Removing Special Characters: Working...')
             corpus = [re.sub(r"[^a-zA-Z0-9']+", ' ', i) for i in corpus]
             if (verbose == True):
                 print('Removing Special Characters: Done!')
         # Remove Stopwords
         if (len(stop_words) > 0):
             for sw_ in stop_words: 
-                if   (sw_ == 'ar' or sw_ == 'ara'):
+                if   (sw_ == 'ar' or sw_ == 'ara' or 'arabic'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Arabic.txt', encoding = 'utf8')
-                elif (sw_ == 'bn' or sw_ == 'ben'):
+                elif (sw_ == 'bn' or sw_ == 'ben' or 'bengali'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Bengali.txt', encoding = 'utf8')
-                elif (sw_ == 'bg' or sw_ == 'bul'):
+                elif (sw_ == 'bg' or sw_ == 'bul' or 'bulgarian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Bulgarian.txt', encoding = 'utf8')
-                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces'):
+                elif (sw_ == 'zh' or sw_ == 'chi' or 'chinese'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Chinese.txt', encoding = 'utf8')
+                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces' or 'czech'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Czech.txt', encoding = 'utf8')
-                elif (sw_ == 'en' or sw_ == 'eng'):
+                elif (sw_ == 'en' or sw_ == 'eng' or 'english'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-English.txt', encoding = 'utf8')
-                elif (sw_ == 'fi' or sw_ == 'fin'):
+                elif (sw_ == 'fi' or sw_ == 'fin' or 'finnish'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Finnish.txt', encoding = 'utf8')
-                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra'):
+                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra' or 'french'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-French.txt', encoding = 'utf8')
-                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu'):
+                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu' or 'german'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-German.txt', encoding = 'utf8')
-                elif (sw_ == 'hi' or sw_ == 'hin'):
+                elif (sw_ == 'el' or sw_ == 'gre' or 'greek'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Greek.txt', encoding = 'utf8')
+                elif (sw_ == 'he' or sw_ == 'heb' or 'hebrew'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hebrew.txt', encoding = 'utf8')
+                elif (sw_ == 'hi' or sw_ == 'hin' or 'hind'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Hind.txt', encoding = 'utf8')
-                elif (sw_ == 'hu' or sw_ == 'hun'):
+                elif (sw_ == 'hu' or sw_ == 'hun' or 'hungarian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Hungarian.txt', encoding = 'utf8')
-                elif (sw_ == 'it' or sw_ == 'ita'):
+                elif (sw_ == 'it' or sw_ == 'ita' or 'italian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Italian.txt', encoding = 'utf8')
-                elif (sw_ == 'mr' or sw_ == 'mar'):
+                elif (sw_ == 'ja' or sw_ == 'jpn' or 'japanese'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Japanese.txt', encoding = 'utf8')
+                elif (sw_ == 'ko' or sw_ == 'kor' or 'korean'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Korean.txt', encoding = 'utf8')
+                elif (sw_ == 'mr' or sw_ == 'mar' or 'marathi'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Marathi.txt', encoding = 'utf8')
-                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas'):
+                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas' or 'persian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Persian.txt', encoding = 'utf8')
-                elif (sw_ == 'pl' or sw_ == 'pol'):
+                elif (sw_ == 'pl' or sw_ == 'pol' or 'polish'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Polish.txt', encoding = 'utf8')
-                elif (sw_ == 'pt-br' or sw_ == 'por-br'):
+                elif (sw_ == 'pt-br' or sw_ == 'por-br' or 'portuguese-br'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Portuguese-br.txt', encoding = 'utf8')
-                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron'):
+                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron' or 'romanian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Romanian.txt', encoding = 'utf8')
-                elif (sw_ == 'ru' or sw_ == 'rus'):
+                elif (sw_ == 'ru' or sw_ == 'rus' or 'russian'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Russian.txt', encoding = 'utf8')
-                elif (sw_ == 'es' or sw_ == 'spa'):
+                elif (sw_ == 'sk' or sw_ == 'slo' or 'slovak'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Slovak.txt', encoding = 'utf8')
+                elif (sw_ == 'es' or sw_ == 'spa' or 'spanish'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Spanish.txt', encoding = 'utf8')
-                elif (sw_ == 'sv' or sw_ == 'swe'):
+                elif (sw_ == 'sv' or sw_ == 'swe' or 'swedish'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Swedish.txt', encoding = 'utf8')
+                elif (sw_ == 'th' or sw_ == 'tha' or 'thai'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Thai.txt', encoding = 'utf8')
+                elif (sw_ == 'uk' or sw_ == 'ukr' or 'ukrainian'):
+                    f_file = pkg_resources.open_text(stws, 'Stopwords-Ukrainian.txt', encoding = 'utf8')
                 f_lines = f_file.read()
                 sw      = f_lines.split('\n')
                 sw      = list(filter(None, sw))
                 sw_full.extend(sw)
             if (verbose == True):
                 print('Removing Stopwords: Working...')
             for i in range(0, len(corpus)):
@@ -556,15 +573,15 @@
         summary   = tokenizer.decode(outputs[0], skip_special_tokens = True)
         self.summ = summary 
         print(summary)
         return summary
 
     ##############################################################################
     
-    # Function: ChatGPT
+    # Function: chatGPT
     def summ_abst_chatgpt(self, api_key = 'your_api_key_here', query = 'make an abstratctive summarization', model = 'text-davinci-003', max_tokens = 250, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
                                                 max_tokens  = max_tokens,
                                                 n           = n,
@@ -574,9 +591,20 @@
             return response.choices[0].text.strip()
         openai.api_key = api_key   
         prompt         = query + ':\n\n' + f'{self.full_txt}\n'
         summary        = query_chatgpt(prompt)
         self.summ      = summary 
         print(summary)
         return summary 
+    
+    # Function: PEGASUS
+    def summ_abst_pegasus(self, text, model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150):
+        tokenizer = PegasusTokenizer.from_pretrained(model_name)
+        pegasus   = PegasusForConditionalGeneration.from_pretrained(model_name)
+        tokens    = tokenizer.encode('summarize: ' + text, return_tensors = 'pt', max_length = 1024, truncation = True)
+        summary   = pegasus.generate(tokens, min_length = min_L, max_length = max_L, length_penalty = 2.0, num_beams = 4, early_stopping = True)
+        summary   = tokenizer.decode(summary[0], skip_special_tokens = True)
+        self.summ = summary 
+        print(summary)
+        return summary
 
-    ##############################################################################   
+    ##############################################################################
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Czech.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Czech.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,256 +1,338 @@
-ačkoli
+a
+aby
 ahoj
+aj
 ale
 anebo
+ani
+aniž
 ano
 asi
 aspoň
-během
+ačkoli
+až
+ba
 bez
 beze
 blízko
 bohužel
 brzo
 bude
+budem
 budeme
-budeš
 budete
+budeš
 budou
 budu
+by
 byl
 byla
 byli
 bylo
 byly
 bys
-čau
+být
+během
 chce
 chceme
-chceš
 chcete
+chceš
 chci
-chtějí
 chtít
+chtějí
 chut'
 chuti
 co
-čtrnáct
-čtyři
-dál
-dále
+což
 daleko
-děkovat
-děkujeme
-děkuji
+další
 den
 deset
 devatenáct
 devět
 do
 dobrý
 docela
 dva
 dvacet
 dvanáct
 dvě
+dál
+dále
+děkovat
+děkujeme
+děkuji
+ho
 hodně
-já
+i
 jak
+jako
+jaké
 jde
 je
 jeden
 jedenáct
 jedna
 jedno
 jednou
 jedou
 jeho
-její
+jej
 jejich
+její
 jemu
 jen
 jenom
-ještě
+jenž
 jestli
 jestliže
-jí
+ještě
+ji
 jich
-jím
 jimi
 jinak
+jiné
+již
 jsem
+jseš
 jsi
 jsme
 jsou
 jste
+já
+jí
+jím
+k
 kam
+každý
 kde
 kdo
 kdy
 když
 ke
 kolik
 kromě
+kterou
 která
 které
-kteří
 který
+kteři
+kteří
+ku
 kvůli
-má
+ma
 mají
-málo
-mám
-máme
-máš
-máte
-mé
-mě
+me
 mezi
-mí
-mít
-mně
+mi
 mnou
+mně
 moc
 mohl
 mohou
 moje
 moji
 možná
-můj
 musí
-může
 my
+má
+málo
+mám
+máme
+máte
+máš
+mé
+mí
+mít
+mě
+měl
+můj
+může
 na
 nad
 nade
-nám
-námi
+napište
 naproti
-nás
-náš
 naše
 naši
 ne
-ně
 nebo
+nebot
 nebyl
 nebyla
 nebyli
 nebyly
-něco
-nedělá
+nechť
 nedělají
+nedělá
 nedělám
 neděláme
-neděláš
 neděláte
-nějak
+neděláš
 nejsi
-někde
-někdo
+nejsou
 nemají
 nemáme
 nemáte
 neměl
-němu
 není
 nestačí
 nevadí
 než
 nic
 nich
-ním
 nimi
 nula
+nám
+námi
+nás
+náš
+ní
+ním
+nýbrž
+ně
+něco
+nějak
+někde
+někdo
+němu
+o
 od
 ode
 on
 ona
 oni
 ono
 ony
 osm
 osmnáct
 pak
 patnáct
-pět
 po
-pořád
+pod
+podle
+pokud
 potom
 pozdě
-před
-přes
-přese
+pořád
 pro
-proč
-prosím
 prostě
+prosím
 proti
+proto
 protože
+proč
+první
+práve
+pět
+před
+přede
+přes
+přese
+při
 rovně
+s
 se
 sedm
 sedmnáct
-šest
-šestnáct
+si
+sice
 skoro
-smějí
 smí
+smějí
 snad
 spolu
 sta
-sté
 sto
+sté
+své
+svých
+svým
+svými
+svůj
 ta
 tady
 tak
 takhle
 taky
+také
+takže
 tam
 tamhle
 tamhleto
 tamto
-tě
+tato
+te
 tebe
 tebou
 ted'
 tedy
 ten
+tento
+teď
 ti
 tisíc
 tisíce
 to
 tobě
 tohle
+toho
+tohoto
+tom
+tomto
+tomuto
+totiž
 toto
-třeba
-tři
-třináct
 trošku
+tu
+tudíž
+tuto
+tvoje
 tvá
 tvé
-tvoje
 tvůj
 ty
+tyto
+této
+tím
+tímto
+tě
+těma
+třeba
+tři
+třináct
+u
 určitě
 už
-vám
-vámi
-vás
-váš
+v
 vaše
 vaši
 ve
-večer
 vedle
+večer
 vlastně
+vy
+vám
+vámi
+vás
+váš
+však
 všechno
 všichni
 vůbec
-vy
 vždy
+vždyť
+z
 za
-zač
 zatímco
+zač
+zda
+zde
 ze
-že
+čau
+či
+čtrnáct
+čtyři
+šest
+šestnáct
+že
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-English.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-English.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 a
+a's
 able
 about
 above
 according
 accordingly
 across
 actually
@@ -40,15 +41,14 @@
 appreciate
 appropriate
 are
 aren
 aren't
 around
 as
-a's
 aside
 ask
 asking
 associated
 at
 available
 away
@@ -75,26 +75,27 @@
 between
 beyond
 both
 brief
 but
 by
 c
+c'mon
+c's
 came
 can
+can't
 cannot
 cant
-can't
 cause
 causes
 certain
 certainly
 changes
 clearly
-c'mon
 co
 com
 come
 comes
 concerning
 consequently
 consider
@@ -102,29 +103,28 @@
 contain
 containing
 contains
 corresponding
 could
 couldn't
 course
-c's
 currently
 d
 definitely
 described
 despite
 did
 didn't
 different
 do
 does
 doesn't
 doing
-done
 don't
+done
 down
 downwards
 during
 e
 each
 edu
 eg
@@ -186,44 +186,48 @@
 hardly
 has
 hasn't
 have
 haven't
 having
 he
+he'd
+he'll
+he's
 hello
 help
 hence
 her
 here
+here's
 hereafter
 hereby
 herein
-here's
 hereupon
 hers
 herself
-he's
 hi
 high
 him
 himself
 his
 hither
 hopefully
 how
+how's
 howbeit
 however
 i
 i'd
+i'll
+i'm
+i've
 ie
 if
 ignored
-i'll
-i'm
 immediate
 in
 inasmuch
 inc
 indeed
 indicate
 indicated
@@ -234,18 +238,17 @@
 into
 inward
 is
 isn't
 it
 it'd
 it'll
-its
 it's
+its
 itself
-i've
 j
 just
 k
 keep
 keeps
 kept
 know
@@ -282,14 +285,15 @@
 might
 more
 moreover
 most
 mostly
 much
 must
+mustn't
 my
 myself
 n
 name
 namely
 nd
 near
@@ -394,15 +398,19 @@
 sent
 serious
 seriously
 set
 seven
 several
 shall
+shan't
 she
+she'd
+she'll
+she's
 should
 shouldn't
 since
 six
 snot
 snt
 so
@@ -422,40 +430,41 @@
 specifying
 still
 sub
 such
 sup
 sure
 t
+t's
 take
 taken
 tell
 tends
 th
 than
 thank
 thanks
 thanx
 that
-thats
 that's
+thats
 the
 their
 theirs
 them
 themselves
 then
 thence
 there
+there's
 thereafter
 thereby
 therefore
 therein
 theres
-there's
 thereupon
 these
 they
 they'd
 they'll
 they're
 they've
@@ -480,15 +489,14 @@
 toward
 towards
 tried
 tries
 truly
 try
 trying
-t's
 twice
 two
 u
 un
 under
 unfortunately
 unless
@@ -516,65 +524,67 @@
 want
 wants
 was
 wasn't
 way
 we
 we'd
+we'll
+we're
+we've
 welcome
 well
-we'll
 went
 were
-we're
 weren't
-we've
 what
-whatever
 what's
+whatever
 when
+when's
 whence
 whenever
 where
+where's
 whereafter
 whereas
 whereby
 wherein
-where's
 whereupon
 wherever
 whether
 which
 while
 whither
 who
+who's
 whoever
 whole
 whom
-who's
 whose
 why
+why's
 will
 willing
 wish
 with
 within
 without
-wonder
 won't
+wonder
 would
 wouldn't
 x
 y
 yes
 yet
 you
 you'd
 you'll
-your
 you're
+you've
+your
 yours
 yourself
 yourselves
-you've
 z
-zero
+zero
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-French.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-French.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 a
-à
-â
 abord
 afin
 ah
 ai
 aie
 ainsi
 allaient
 allo
-allô
 allons
+allô
+alors
 après
 assez
 attendu
 au
 aucun
 aucune
+aucuns
 aujourd
 aujourd'hui
 auquel
 aura
 auront
 aussi
 autre
@@ -36,19 +36,19 @@
 avoir
 ayant
 b
 bah
 beaucoup
 bien
 bigre
+bon
 boum
 bravo
 brrr
 c
-ça
 car
 ce
 ceci
 cela
 celle
 celle-ci
 celle-là
@@ -70,20 +70,20 @@
 cette
 ceux
 ceux-ci
 ceux-là
 chacun
 chaque
 cher
-chère
-chères
 chers
 chez
 chiche
 chut
+chère
+chères
 ci
 cinq
 cinquantaine
 cinquante
 cinquantième
 cinquième
 clac
@@ -103,97 +103,97 @@
 debout
 dedans
 dehors
 delà
 depuis
 derrière
 des
-dès
-désormais
 desquelles
 desquels
 dessous
 dessus
 deux
 deuxième
 deuxièmement
 devant
 devers
 devra
+devrait
 différent
 différente
 différentes
 différents
 dire
 divers
 diverse
 diverses
 dix
 dix-huit
-dixième
 dix-neuf
 dix-sept
+dixième
 doit
 doivent
 donc
 dont
+dos
 douze
 douzième
 dring
+droite
 du
 duquel
 durant
+dès
+début
+désormais
 e
 effet
 eh
 elle
 elle-même
 elles
 elles-mêmes
 en
 encore
 entre
 envers
 environ
 es
-ès
+essai
 est
 et
 etant
-étaient
-étais
-était
-étant
 etc
-été
 etre
-être
 eu
 euh
 eux
 eux-mêmes
 excepté
 f
-façon
 fais
 faisaient
 faisant
 fait
+faites
+façon
 feront
 fi
 flac
 floc
+fois
 font
+force
 g
 gens
 h
 ha
-hé
+haut
 hein
-hélas
 hem
 hep
 hi
 ho
 holà
 hop
 hormis
@@ -202,153 +202,166 @@
 houp
 hue
 hui
 huit
 huitième
 hum
 hurrah
+hé
+hélas
 i
+ici
 il
 ils
 importe
 j
 je
 jusqu
 jusque
+juste
 k
 l
 la
-là
 laquelle
 las
 le
 lequel
 les
-lès
 lesquelles
 lesquels
 leur
 leurs
 longtemps
 lorsque
 lui
 lui-même
+là
+lès
 m
 ma
 maint
+maintenant
 mais
 malgré
 me
-même
-mêmes
 merci
 mes
 mien
 mienne
 miennes
 miens
 mille
 mince
+mine
 moi
 moi-même
 moins
 mon
+mot
 moyennant
+même
+mêmes
 n
 na
 ne
-néanmoins
 neuf
 neuvième
 ni
 nombreuses
 nombreux
+nommés
 non
 nos
 notre
-nôtre
-nôtres
 nous
 nous-mêmes
+nouveaux
 nul
+néanmoins
+nôtre
+nôtres
 o
-o|
-ô
 oh
 ohé
-olé
 ollé
+olé
 on
 ont
 onze
 onzième
 ore
 ou
-où
 ouf
 ouias
 oust
 ouste
 outre
+o|
+où
 p
 paf
 pan
 par
+parce
 parmi
+parole
 partant
 particulier
 particulière
 particulièrement
 pas
 passé
 pendant
 personne
+personnes
 peu
 peut
 peuvent
 peux
 pff
 pfft
 pfut
 pif
+pièce
 plein
 plouf
+plupart
 plus
 plusieurs
 plutôt
 pouah
 pour
 pourquoi
 premier
 première
 premièrement
-près
 proche
+près
 psitt
 puisque
 q
 qu
 quand
 quant
-quanta
 quant-à-soi
+quanta
 quarante
 quatorze
 quatre
 quatre-vingt
 quatrième
 quatrièmement
 que
 quel
 quelconque
 quelle
 quelles
+quelqu'un
 quelque
 quelques
-quelqu'un
 quels
 qui
 quiconque
 quinze
 quoi
 quoique
 r
@@ -365,14 +378,15 @@
 seize
 selon
 sept
 septième
 sera
 seront
 ses
+seulement
 si
 sien
 sienne
 siennes
 siens
 sinon
 six
@@ -380,25 +394,27 @@
 soi
 soi-même
 soit
 soixante
 son
 sont
 sous
+soyez
 stop
 suis
 suivant
+sujet
 sur
 surtout
 t
 ta
 tac
+tandis
 tant
 te
-té
 tel
 telle
 tellement
 telles
 tels
 tenant
 tes
@@ -415,49 +431,67 @@
 toujours
 tous
 tout
 toute
 toutes
 treize
 trente
-très
 trois
 troisième
 troisièmement
 trop
+très
 tsoin
 tsouin
 tu
+té
 u
 un
 une
 unes
 uns
 v
 va
 vais
+valeur
 vas
-vé
 vers
 via
 vif
 vifs
 vingt
 vivat
 vive
 vives
 vlan
 voici
+voie
+voient
 voilà
 vont
 vos
 votre
-vôtre
-vôtres
 vous
 vous-mêmes
 vu
+vé
+vôtre
+vôtres
 w
 x
 y
 z
 zut
+à
+â
+ça
+ès
+étaient
+étais
+était
+étant
+état
+étions
+été
+êtr
+être
+ô
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-German.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-German.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 a
 ab
 aber
-aber
 ach
 acht
 achte
 achten
 achter
 achtes
 ag
@@ -14,30 +13,28 @@
 allem
 allen
 aller
 allerdings
 alles
 allgemeinen
 als
-als
 also
 am
 an
 andere
 anderen
 andern
 anders
 au
 auch
-auch
 auf
 aus
 ausser
-außer
 ausserdem
+außer
 außerdem
 b
 bald
 bei
 beide
 beiden
 beim
@@ -49,14 +46,15 @@
 besten
 bin
 bis
 bisher
 bist
 c
 d
+d.h
 da
 dabei
 dadurch
 dafür
 dagegen
 daher
 dahin
@@ -69,58 +67,55 @@
 dann
 daran
 darauf
 daraus
 darf
 darfst
 darin
-darüber
 darum
 darunter
-das
+darüber
 das
 dasein
 daselbst
 dass
-daß
 dasselbe
 davon
 davor
 dazu
 dazwischen
+daß
 dein
 deine
 deinem
 deiner
 dem
 dementsprechend
 demgegenüber
 demgemäss
 demgemäß
 demselben
 demzufolge
 den
 denen
 denn
-denn
 denselben
 der
 deren
 derjenige
 derjenigen
 dermassen
 dermaßen
 derselbe
 derselben
 des
 deshalb
 desselben
 dessen
 deswegen
-d.h
 dich
 die
 diejenige
 diejenigen
 dies
 diese
 dieselbe
@@ -137,25 +132,24 @@
 dritte
 dritten
 dritter
 drittes
 du
 durch
 durchaus
-dürfen
-dürft
 durfte
 durften
+dürfen
+dürft
 e
 eben
 ebenso
 ehrlich
 ei
 ei,
-ei,
 eigen
 eigene
 eigenen
 eigener
 eigenes
 ein
 einander
@@ -165,33 +159,33 @@
 einer
 eines
 einige
 einigen
 einiger
 einiges
 einmal
-einmal
 eins
 elf
 en
 ende
 endlich
 entweder
-entweder
 er
-Ernst
+ernst
 erst
 erste
 ersten
 erster
 erstes
 es
 etwa
 etwas
 euch
+euer
+eure
 f
 früher
 fünf
 fünfte
 fünften
 fünfter
 fünftes
@@ -215,88 +209,87 @@
 gemacht
 gemocht
 gemusst
 genug
 gerade
 gern
 gesagt
-gesagt
 geschweige
 gewesen
 gewollt
 geworden
 gibt
 ging
 gleich
 gott
 gross
-groß
 grosse
-große
 grossen
-großen
 grosser
-großer
 grosses
+groß
+große
+großen
+großer
 großes
 gut
 gute
 guter
 gutes
 h
 habe
 haben
 habt
 hast
 hat
 hatte
-hätte
 hatten
-hätten
+hattest
+hattet
 heisst
 her
 heute
 hier
 hin
 hinter
 hoch
+hätte
+hätten
 i
 ich
 ihm
 ihn
 ihnen
 ihr
 ihre
 ihrem
 ihren
 ihrer
 ihres
 im
-im
 immer
 in
-in
 indem
 infolgedessen
 ins
 irgend
 ist
 j
 ja
-ja
 jahr
 jahre
 jahren
 je
 jede
 jedem
 jeden
 jeder
 jedermann
 jedermanns
+jedes
 jedoch
 jemand
 jemandem
 jemanden
 jene
 jenem
 jenen
@@ -315,24 +308,23 @@
 keiner
 kleine
 kleinen
 kleiner
 kleines
 kommen
 kommt
-können
-könnt
 konnte
-könnte
 konnten
 kurz
+können
+könnt
+könnte
 l
 lang
 lange
-lange
 leicht
 leide
 lieber
 los
 m
 machen
 macht
@@ -357,27 +349,29 @@
 mensch
 menschen
 mich
 mir
 mit
 mittel
 mochte
-möchte
 mochten
-mögen
-möglich
-mögt
 morgen
 muss
-muß
-müssen
 musst
-müsst
 musste
 mussten
+muß
+mußt
+möchte
+mögen
+möglich
+mögt
+müssen
+müsst
+müßt
 n
 na
 nach
 nachdem
 nahm
 natürlich
 neben
@@ -386,35 +380,30 @@
 neuen
 neun
 neunte
 neunten
 neunter
 neuntes
 nicht
-nicht
 nichts
 nie
 niemand
 niemandem
 niemanden
 noch
 nun
-nun
 nur
 o
 ob
-ob
 oben
 oder
-oder
 offen
 oft
-oft
 ohne
-Ordnung
+ordnung
 p
 q
 r
 recht
 rechte
 rechten
 rechter
@@ -425,36 +414,34 @@
 sa
 sache
 sagt
 sagte
 sah
 satt
 schlecht
-Schluss
+schluss
 schon
 sechs
 sechste
 sechsten
 sechster
 sechstes
 sehr
 sei
-sei
 seid
 seien
 sein
 seine
 seinem
 seinen
 seiner
 seines
 seit
 seitdem
 selbst
-selbst
 sich
 sie
 sieben
 siebente
 siebenten
 siebenter
 siebentes
@@ -464,35 +451,35 @@
 solche
 solchem
 solchen
 solcher
 solches
 soll
 sollen
+sollst
+sollt
 sollte
 sollten
 sondern
 sonst
+soweit
 sowie
 später
 statt
 t
 tag
 tage
 tagen
 tat
 teil
 tel
 tritt
 trotzdem
 tun
 u
-über
-überhaupt
-übrigens
 uhr
 um
 und
 und?
 uns
 unser
 unsere
@@ -511,20 +498,16 @@
 vierter
 viertes
 vom
 von
 vor
 w
 wahr?
-während
-währenddem
-währenddessen
 wann
 war
-wäre
 waren
 wart
 warum
 was
 wegen
 weil
 weit
@@ -536,45 +519,50 @@
 welchem
 welchen
 welcher
 welches
 wem
 wen
 wenig
-wenig
 wenige
 weniger
 weniges
 wenigstens
 wenn
-wenn
 wer
 werde
 werden
 werdet
+weshalb
 wessen
 wie
-wie
 wieder
+wieso
 will
 willst
 wir
 wird
 wirklich
 wirst
 wo
+woher
+wohin
 wohl
 wollen
 wollt
 wollte
 wollten
 worden
 wurde
-würde
 wurden
+während
+währenddem
+währenddessen
+wäre
+würde
 würden
 x
 y
 z
 z.b
 zehn
 zehnte
@@ -582,22 +570,23 @@
 zehnter
 zehntes
 zeit
 zu
 zuerst
 zugleich
 zum
-zum
 zunächst
 zur
 zurück
 zusammen
 zwanzig
 zwar
-zwar
 zwei
 zweite
 zweiten
 zweiter
 zweites
 zwischen
 zwölf
+über
+überhaupt
+übrigens
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Persian.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Polish.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Russian.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/PKG-INFO` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.2
+Version: 1.0.4
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyAutoSummarizer
 
 pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence. 
 
 ## Introduction
 
-pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+
+pyAutoSummarizer stands out for its proficient preprocessing capabilities that pave the way for high-quality text summarization. Recognizing the importance of text normalization, the library offers a range of text cleansing and standardization features. It can convert text to **lowercase**, ensuring uniformity across the data. Additionally, it can **remove accents**, **remove special characters**, and **remove numbers**, which helps mitigate the text's noise. It also offers the functionality to **remove custom words**, enabling users to tailor their preprocessing needs. Notably, pyAutoSummarizer supports **stopwords** removal across various languages, including Arabic, Bengali, Bulgarian, Chinese, Czech, English, Finnish, French, German, Greek, Hebrew, Hind, Hungarian, Italian, Japanese, Korean, Marathi, Persia, Polish, Portuguese-br, Romanian, Russian, Slovak, Spanish, Swedish, Thai, and Ukrainian. The library provides flexibility in sentence segmentation, allowing sentences to be split based on **punctuation**, **character count**, or **word count**. 
 
 To evaluate the quality of the summaries generated, pyAutoSummarizer integrates various metrics such as **Rouge-N**, **Rouge-L**, and **Rouge-S**, which compare the overlap of n-grams, longest common subsequence, and skip-bigram between the generated summary and the reference summary respectively. Additionally, it employs **BLEU** (Bilingual Evaluation Understudy), and **METEOR** (Metric for Evaluation of Translation with Explicit ORdering).
 
 ## Usage
 
 1. Install
 ```bash
@@ -31,13 +33,14 @@
 Extractive Summarization
 - Example 01: TextRank           ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
-Abstractive Summarization. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5))
+Abstractive Summarization. 
+- Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- Example 02: Pegasus (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
 
 - [pyBibX](https://github.com/Valdecy/pyBibX) - A Bibliometric and Scientometric Python Library Powered with Artificial Intelligence Tools
```

### Comparing `pyAutoSummarizer-1.0.2/pyAutoSummarizer.egg-info/SOURCES.txt` & `pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,24 +10,32 @@
 pyAutoSummarizer.egg-info/top_level.txt
 pyAutoSummarizer.egg-info/zip-safe
 pyAutoSummarizer/base/__init__.py
 pyAutoSummarizer/base/psr.py
 pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
 pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
 pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
+pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
 pyAutoSummarizer/base/stws/Stopwords-Czech.txt
 pyAutoSummarizer/base/stws/Stopwords-English.txt
 pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
 pyAutoSummarizer/base/stws/Stopwords-French.txt
 pyAutoSummarizer/base/stws/Stopwords-German.txt
+pyAutoSummarizer/base/stws/Stopwords-Greek.txt
+pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
 pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
 pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
 pyAutoSummarizer/base/stws/Stopwords-Italian.txt
+pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
+pyAutoSummarizer/base/stws/Stopwords-Korean.txt
 pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
 pyAutoSummarizer/base/stws/Stopwords-Persian.txt
 pyAutoSummarizer/base/stws/Stopwords-Polish.txt
 pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
 pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
 pyAutoSummarizer/base/stws/Stopwords-Russian.txt
+pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
 pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
 pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
+pyAutoSummarizer/base/stws/Stopwords-Thai.txt
+pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
 pyAutoSummarizer/base/stws/__init__.py
```

### Comparing `pyAutoSummarizer-1.0.2/setup.py` & `pyAutoSummarizer-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyAutoSummarizer',
-    version='1.0.2',
+    version='1.0.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyAutoSummarizer',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

