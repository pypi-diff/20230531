# Comparing `tmp/evals-nightly-1.0.3.dev20230522.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev20230522.tar", last modified: Mon May 22 19:47:47 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230530.tar", last modified: Wed May 31 00:13:44 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev20230522.tar` & `evals-nightly-1.0.3.dev20230530.tar`

### file list

```diff
@@ -1,205 +1,298 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/LICENSE
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5460 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.035118 evals-nightly-1.0.3.dev20230522/evals/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/api.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/cli/
--rw-r--r--   0 root         (0) root         (0)     5645 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/cli/oaieval.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/cli/oaievalset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/completion_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/cot.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/langchain_math.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/openai.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/completion_fns/retrieval.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/elsuite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/
--rw-r--r--   0 root         (0) root         (0)     1756 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/includes.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/multiple_choice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/elsuite/test/
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/test/match.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/translate.py
--rw-r--r--   0 root         (0) root         (0)     6438 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/elsuite/utils.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/eval.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/formatting.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/prompt/
--rw-r--r--   0 root         (0) root         (0)     4093 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/prompt/base.py
--rw-r--r--   0 root         (0) root         (0)    18168 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.035118 evals-nightly-1.0.3.dev20230522/evals/registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/registry/completion_fns/
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.039118 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.055119 evals-nightly-1.0.3.dev20230522/evals/registry/evals/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/afrikaans-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/aime_evaluation.yaml
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/ascii-wordart.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/banking77.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/body-movement.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/born-first.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/building_floorplan.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/chess.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 root         (0) root         (0)     1719 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/counterfactual-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/crepe.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/day-of-week-from-date.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/determinant.yaml
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/event-categories.yaml
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/finance.yaml
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/find-thirukkural.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/integer-sequence-predictions.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/invoices.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/irish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      233 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/isosceles-right-triangle.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/language.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/largest_country.yaml
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 root         (0) root         (0)      456 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/logic-liar-paradox.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/logic.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/logical_counting.yaml
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 root         (0) root         (0)    14586 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/mmlu.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 root         (0) root         (0)     1193 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/nepali-song-singer.yaml
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/ordered-history-events.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/physics-interaction.yaml
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/probability_questions.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/qa.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/rot13.yaml
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/rubiks-colors.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/rucola.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/russe.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/sexagenary-cycle-calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/shape-in-shape.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/south-african-bands.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/sql.yaml
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/squares-gpt.yaml
--rw-r--r--   0 root         (0) root         (0)     4472 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/syntax-check.yaml
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/taxes.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 root         (0) root         (0)     1169 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 root         (0) root         (0)     3040 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 root         (0) root         (0)      360 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/tetris.yaml
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/time-zone-conversion.yaml
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/vintage_phone_keyboard_decode.yaml
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/evals/which-is-heavier.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      492 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 root         (0) root         (0)     1157 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 root         (0) root         (0)     2564 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 root         (0) root         (0)     9610 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/evals/utils/
--rw-r--r--   0 root         (0) root         (0)     2136 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/utils/api_utils.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/evals/utils/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7303 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-22 19:47:47.000000 evals-nightly-1.0.3.dev20230522/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-22 19:47:44.000000 evals-nightly-1.0.3.dev20230522/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 19:47:47.059120 evals-nightly-1.0.3.dev20230522/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5460 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.233058 evals-nightly-1.0.3.dev20230530/evals/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/cli/
+-rw-r--r--   0 root         (0) root         (0)     5645 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/cli/oaieval.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/cli/oaievalset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/cot.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/openai.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/completion_fns/retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/includes.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/multiple_choice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/elsuite/test/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/test/match.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/utils.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/elsuite/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/prompt/
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/prompt/base.py
+-rw-r--r--   0 root         (0) root         (0)    18168 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.233058 evals-nightly-1.0.3.dev20230530/evals/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.237058 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.241059 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/registry/evals/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/2d_movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/adultery_state_laws.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/afrikaans-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/aime_evaluation.yaml
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      451 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ambiguous-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/arithmetical_puzzles.yaml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ascii-wordart.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/atpl_exams.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/body-movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/building_floorplan.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chess.yaml
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chinese_poem.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/chinese_tang_poetries.yaml
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/cissp-study-questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/color_theory_complementary.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/count_intersections_polynomial.yaml
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/count_token_freq_dna.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/counterfactual-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/countries.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/crontab.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 root         (0) root         (0)      179 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/date-booking.yaml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/date-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/day-of-week-from-date.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/detect-hshd.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/diabetes.yaml
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/direct-speech-tag.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/directions.yaml
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dna-melting-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/european-date-format-challenge.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/event-categories.yaml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/finance.yaml
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/financial-derivatives.yaml
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find-letter.yaml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find-thirukkural.yaml
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/find_country_from_svg.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/finnish-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/food.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/french-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/french-part-of-speech.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/gol.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/guess-the-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hebrew-same-noun-gender.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_shuddha.yaml
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/hindi_words.yaml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/integer-sequence-predictions.yaml
+-rw-r--r--   0 root         (0) root         (0)      235 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/internal_representations.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invert_word_wise.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/irish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/irony.yaml
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/islands.yaml
+-rw-r--r--   0 root         (0) root         (0)      233 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/isosceles-right-triangle.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/italian-new-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/italian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese-itpassport-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_city_name_pronuciation.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_number_reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/jee-math.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/kanji-idioms.yaml
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/korean-consonant-vowel-combination.yaml
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/korean_spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/language.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/largest_country.yaml
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/linear-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/linear-regression.yaml
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/list_comparison_missing_name.yaml
+-rw-r--r--   0 root         (0) root         (0)      456 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic-liar-paradox.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logical_counting.yaml
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/lunar-calendar.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mandaliof-table.yaml
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mate-in-one.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/matrix-mult-rows.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/missing-operators.yaml
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/multistep-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music-theory-chord-names.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music-theory-chord-notes.yaml
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/music_theory_scale_modes.yaml
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/nepali-song-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      340 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/newsology.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/norwegian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/numbers_game.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/nutrition.yaml
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ordered-history-events.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/physics-interaction.yaml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 root         (0) root         (0)      270 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/polish_rhymes_generation.yaml
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/portuguese-sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/portuguese-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/probability_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/python_list_comprehension.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/qa.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/resistor-ohm-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/reverse-polish-notation.yaml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rhetorical-devices.yaml
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rubiks-colors.yaml
+-rw-r--r--   0 root         (0) root         (0)      236 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russe.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/seating_arrangements.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/security_guide.yaml
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sexagenary-cycle-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/shape-in-shape.yaml
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/shared-borders.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/simple-visual-understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/south-african-bands.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/spanish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/squares-gpt.yaml
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/superficial-patterns.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swap-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/swedish_sat.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/syntax-check.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/test_japanese_units.yaml
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tetris.yaml
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/time-zone-conversion.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/track_objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/tracking-shuffled-objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unique_combinations.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unsolvable_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/unwanted-rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/vigenere.yaml
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/vintage_phone_keyboard_decode.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/which-is-heavier.yaml
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/wkt_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/evals/word_vector_over_reliance.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 root         (0) root         (0)      887 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/regression-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals/utils/
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/api_utils.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/evals/utils/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11480 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-31 00:13:44.000000 evals-nightly-1.0.3.dev20230530/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 00:13:41.000000 evals-nightly-1.0.3.dev20230530/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 00:13:44.265060 evals-nightly-1.0.3.dev20230530/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev20230522/LICENSE` & `evals-nightly-1.0.3.dev20230530/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/README.md` & `evals-nightly-1.0.3.dev20230530/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Access will be granted to the email address associated with an accepted Eval. Due to high volume, we are unable to grant access to any email other than the one used for the pull request.
 ____________________
 
 ## Setup
 
 To run evals, you will need to set up and specify your OpenAI API key. You can generate one at <https://platform.openai.com/account/api-keys>. After you obtain an API key, specify it using the `OPENAI_API_KEY` environment variable. **Please be aware of the [costs](https://openai.com/pricing) associated with using the API when running evals.**
 
-**Minimal Required Version: Python 3.9**
+**Minimum Required Version: Python 3.9**
 
 ### Downloading evals
 
 Our Evals registry is stored using [Git-LFS](https://git-lfs.com/). Once you have downloaded and installed LFS, you can fetch the evals with:
 ```sh
 git lfs fetch --all
 git lfs pull
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/api.py` & `evals-nightly-1.0.3.dev20230530/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/base.py` & `evals-nightly-1.0.3.dev20230530/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230530/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230530/evals/cli/oaievalset.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,22 @@
         action=argparse.BooleanOptionalAction,
         default=True,
         help="Exit if any oaieval command fails.",
     )
     return parser
 
 
-def run(args, unknown_args, registry: Optional[Registry] = None) -> None:
+def run(
+    args, unknown_args, registry: Optional[Registry] = None, run_command: str = "oaieval"
+) -> None:
     registry = registry or Registry()
     commands: list[Task] = []
     eval_set = registry.get_eval_set(args.eval_set)
     for eval in registry.get_evals(eval_set.evals):
-        command = ["oaieval", args.model, eval.key] + unknown_args
+        command = [run_command, args.model, eval.key] + unknown_args
         if command in commands:
             continue
         commands.append(command)
     num_evals = len(commands)
 
     progress = Progress(f"/tmp/oaievalset/{args.model}.{args.eval_set}.progress.txt")
     if args.resume and progress.load():
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230530/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230530/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230530/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230530/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/data.py` & `evals-nightly-1.0.3.dev20230530/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/fuzzy_match_test.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/fuzzy_match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/includes.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/multiple_choice.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/test/match.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/test/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230530/evals/elsuite/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         counts[answer] += 1
     counts[None] = 0
     return max(counts, key=counts.get)
 
 
 def normalize(s: str) -> str:
     """Lower text and remove punctuation, articles and extra whitespace."""
-    s = s.split("\n")[0]
     s = s.lower()
     exclude = set(string.punctuation)
     s = "".join(char for char in s if char not in exclude)
     s = re.sub(r"\b(a|an|the)\b", " ", s)
     s = " ".join(s.split())
     return s
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/eval.py` & `evals-nightly-1.0.3.dev20230530/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/formatting.py` & `evals-nightly-1.0.3.dev20230530/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/metrics.py` & `evals-nightly-1.0.3.dev20230530/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230530/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/record.py` & `evals-nightly-1.0.3.dev20230530/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/integer-sequence-predictions.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/integer-sequence-predictions.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/mmlu.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/sql.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,8 @@
     Yu, Tao, et al. \"Spider; A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task.\" Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, 2018, https://doi.org/10.18653/v1/d18-1425.
   disclaimer: Problems are solved zero-shot with no prompting other than the schema; performance may improve with training examples, fine tuning, or a different schema format. Evaluation is currently done through model-grading, where SQL code is not actually executed; the model may judge correct SQL to be incorrect, or vice-versa.
 spider-sql.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: sql/spider_sql.jsonl
     eval_type: cot_classify
-    modelgraded_spec_file: sql
+    modelgraded_spec: sql
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/evals/test-modelgraded.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     eval_type: cot_classify
     modelgraded_spec: diversity
     multicomp_n: 4
     sample_kwargs:
       temperature: 0.4
 
 # a simple modelgraded eval checking which of N completions to the sample prompt is the best response
-# command: `oaleval gpt-3.5-turbo,gpt-4,gpt-3.5-turbo best`
+# command: `oaieval gpt-3.5-turbo,gpt-4,gpt-3.5-turbo best`
 best:
   id: best.dev.v0
   metrics: [accuracy]
 best.dev.v0:
   class: evals.elsuite.modelgraded.classify:ModelBasedClassify
   args:
     samples_jsonl: test_modelgraded/joke_fruits.jsonl
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230530/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/registry.py` & `evals-nightly-1.0.3.dev20230530/evals/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,24 @@
     for model_prefix, n_ctx in DICT_OF_N_CTX_BY_MODEL_NAME_PREFIX.items():
         if model_name.startswith(model_prefix):
             return n_ctx
     # otherwise, look for an exact match and return None if not found
     return DICT_OF_N_CTX_BY_MODEL_NAME.get(model_name, None)
 
 
+CHAT_MODELS = {
+    "gpt-3.5-turbo",
+    "gpt-3.5-turbo-0301",
+    "gpt-4",
+    "gpt-4-0314",
+    "gpt-4-32k",
+    "gpt-4-32k-0314",
+}
+
+
 class Registry:
     def __init__(self, registry_paths: Sequence[Union[str, Path]] = DEFAULT_PATHS):
         self._registry_paths = [Path(p) if isinstance(p, str) else p for p in registry_paths]
 
     def add_registry_paths(self, paths: list[Union[str, Path]]):
         self._registry_paths.extend([Path(p) if isinstance(p, str) else p for p in paths])
 
@@ -82,23 +92,14 @@
         """
 
         if name == "dummy":
             return DummyCompletionFn()
 
         n_ctx = n_ctx_from_model_name(name)
 
-        CHAT_MODELS = {
-            "gpt-3.5-turbo",
-            "gpt-3.5-turbo-0301",
-            "gpt-4",
-            "gpt-4-0314",
-            "gpt-4-32k",
-            "gpt-4-32k-0314",
-        }
-
         if name in CHAT_MODELS:
             return OpenAIChatCompletionFn(model=name, n_ctx=n_ctx)
         elif name in self.api_model_ids:
             return OpenAICompletionFn(model=name, n_ctx=n_ctx)
 
         # No match, so try to find a completion-fn-id in the registry
         spec = self.get_completion_fn(name)
```

### Comparing `evals-nightly-1.0.3.dev20230522/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230530/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230530/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230530/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230522/pyproject.toml` & `evals-nightly-1.0.3.dev20230530/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "evals-nightly"
-version = "1.0.3.dev20230522"
+version = "1.0.3.dev20230530"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
```

