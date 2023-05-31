# Comparing `tmp/merlin-models-23.4.0.tar.gz` & `tmp/merlin-models-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-models-23.4.0.tar", last modified: Wed Apr 26 20:35:57 2023, max compression
+gzip compressed data, was "merlin-models-23.5.0.tar", last modified: Wed May 31 14:39:51 2023, max compression
```

## Comparing `merlin-models-23.4.0.tar` & `merlin-models-23.5.0.tar`

### file list

```diff
@@ -1,457 +1,428 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-26 19:35:34.000000 merlin-models-23.4.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-26 19:35:34.000000 merlin-models-23.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-26 19:35:34.000000 merlin-models-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-26 19:35:34.000000 merlin-models-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-26 20:35:57.823311 merlin-models-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-26 19:35:34.000000 merlin-models-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.635310 merlin-models-23.4.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.647310 merlin-models-23.4.0/merlin/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/criteo/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/ecommerce/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/large/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/large/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/large/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/ecommerce/small/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/small/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/small/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/social/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/social/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/merlin/models/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 20:35:57.823311 merlin-models-23.4.0/merlin/models/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/lightfm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.679310 merlin-models-23.4.0/merlin/models/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.679310 merlin-models-23.4.0/merlin/models/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15357 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.683310 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.683310 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.687310 merlin-models-23.4.0/merlin/models/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.687310 merlin-models-23.4.0/merlin/models/tf/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/experimental/sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    47966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/listwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.695310 merlin-models-23.4.0/merlin/models/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.699310 merlin-models-23.4.0/merlin/models/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100235 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    23180 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.699310 merlin-models-23.4.0/merlin/models/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.703310 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/popularity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.703310 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.707310 merlin-models-23.4.0/merlin/models/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.707310 merlin-models-23.4.0/merlin/models/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    53093 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)    46929 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/repr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.715310 merlin-models-23.4.0/merlin/models/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.715310 merlin-models-23.4.0/merlin/models/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/prediction_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.723311 merlin-models-23.4.0/merlin/models/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.727311 merlin-models-23.4.0/merlin/models/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/examples_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.731311 merlin-models-23.4.0/merlin/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/example_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/nvt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.731311 merlin-models-23.4.0/merlin/models/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/xgb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.735311 merlin-models-23.4.0/merlin_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-26 19:35:34.000000 merlin-models-23.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 19:35:34.000000 merlin-models-23.4.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/horovod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/implicit.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/lightfm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/transformers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 20:35:57.823311 merlin-models-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-26 19:35:34.000000 merlin-models-23.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/common/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.743311 merlin-models-23.4.0/tests/common/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_tests_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.743311 merlin-models-23.4.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/integration/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/integration/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/retrieval/test_integration_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/config/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.751311 merlin-models-23.4.0/tests/unit/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_advertising.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_entertainment.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_social.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.755311 merlin-models-23.4.0/tests/unit/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/implicit/test_implicit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.755311 merlin-models-23.4.0/tests/unit/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/lightfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/lightfm/test_lightfm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.759311 merlin-models-23.4.0/tests/unit/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.763311 merlin-models-23.4.0/tests/unit/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.763311 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.767311 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.771311 merlin-models-23.4.0/tests/unit/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.779311 merlin-models-23.4.0/tests/unit/tf/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_07_train_traditional_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.779311 merlin-models-23.4.0/tests/unit/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/experimental/test_sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.783311 merlin-models-23.4.0/tests/unit/tf/horovod/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/test_horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.787311 merlin-models-23.4.0/tests/unit/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    28970 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.787311 merlin-models-23.4.0/tests/unit/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/layers/test_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.791311 merlin-models-23.4.0/tests/unit/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/losses/test_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.791311 merlin-models-23.4.0/tests/unit/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_popularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.795311 merlin-models-23.4.0/tests/unit/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    36730 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.799311 merlin-models-23.4.0/tests/unit/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.803311 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.803311 merlin-models-23.4.0/tests/unit/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17308 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.807311 merlin-models-23.4.0/tests/unit/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    39661 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.807311 merlin-models-23.4.0/tests/unit/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.811311 merlin-models-23.4.0/tests/unit/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.811311 merlin-models-23.4.0/tests/unit/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/test_mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.815311 merlin-models-23.4.0/tests/unit/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.815311 merlin-models-23.4.0/tests/unit/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/test_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_dataloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/utils/test_schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/tests/unit/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/xgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/xgb/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-04-26 19:35:34.000000 merlin-models-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-31 14:39:25.000000 merlin-models-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-31 14:39:25.000000 merlin-models-23.5.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-31 14:39:25.000000 merlin-models-23.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-31 14:39:25.000000 merlin-models-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 14:39:25.000000 merlin-models-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-31 14:39:51.915997 merlin-models-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-31 14:39:25.000000 merlin-models-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.815997 merlin-models-23.5.0/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/conda/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 14:39:25.000000 merlin-models-23.5.0/conda/recipes/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.815997 merlin-models-23.5.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/criteo/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/large/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/large/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/large/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/small/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/small/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/small/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/social/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/merlin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:51.915997 merlin-models-23.5.0/merlin/models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/lightfm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.843997 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.843997 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/experimental/sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51818 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/logging/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/listwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99187 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23318 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.855997 merlin-models-23.5.0/merlin/models/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.855997 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54513 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46941 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/repr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/torchscript_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.867997 merlin-models-23.5.0/merlin/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/example_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/nvt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.867997 merlin-models-23.5.0/merlin/models/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/xgb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.871997 merlin-models-23.5.0/merlin_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-31 14:39:25.000000 merlin-models-23.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:39:25.000000 merlin-models-23.5.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.871997 merlin-models-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/horovod-cpu-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/horovod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/implicit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/lightfm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/transformers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 14:39:51.915997 merlin-models-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-31 14:39:25.000000 merlin-models-23.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_tests_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25747 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/integration/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/integration/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/retrieval/test_integration_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/config/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_advertising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_entertainment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/implicit/test_implicit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/lightfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/lightfm/test_lightfm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.887997 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.887997 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.891997 merlin-models-23.5.0/tests/unit/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_07_train_traditional_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/experimental/test_sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/horovod/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/test_horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/layers/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/losses/test_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.903997 merlin-models-23.5.0/tests/unit/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.903997 merlin-models-23.5.0/tests/unit/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.907997 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.907997 merlin-models-23.5.0/tests/unit/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24815 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.911997 merlin-models-23.5.0/tests/unit/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52913 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.911997 merlin-models-23.5.0/tests/unit/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/test_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/test_torchscript_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/utils/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/xgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/xgb/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-05-31 14:39:25.000000 merlin-models-23.5.0/versioneer.py
```

### Comparing `merlin-models-23.4.0/.pre-commit-config.yaml` & `merlin-models-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/CLA.md` & `merlin-models-23.5.0/CLA.md`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/CONTRIBUTING.md` & `merlin-models-23.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/LICENSE` & `merlin-models-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/MANIFEST.in` & `merlin-models-23.5.0/MANIFEST.in`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-
+include Makefile
 
 include *.md
 include *.yaml
 include *.ini
 
 recursive-include _images *.png
 recursive-exclude docs *
 recursive-exclude docs *.ipynb
 exclude docs/source/_images
 
+recursive-include conda *.yaml
+
 recursive-include requirements *.txt
+recursive-include requirements *.yml
 
 recursive-exclude tests *.coveragerc
 recursive-include tests *.parquet
 recursive-include tests *.pbtxt
 recursive-include tests *.py
 
 recursive-include merlin *.json
```

### Comparing `merlin-models-23.4.0/PKG-INFO` & `merlin-models-23.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,137 +1,14 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.4.0
+Version: 23.5.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
-Description: ## Merlin Models
-        
-        [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
-        ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
-        [![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
-        
-        The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
-        that range from classic machine learning models to highly-advanced deep learning models.
-        
-        The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
-        practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
-        models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
-        example offline
-        datasets.
-        
-        In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
-        
-        ### Benefits of Merlin Models
-        
-        **[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
-        These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
-        
-        **Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
-        The design makes it easy to combine the blocks to define new architectures.
-        The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
-        
-        **Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
-        For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
-        The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
-        
-        **[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
-        When training deep learning recommender system models, data loading can be a bottleneck.
-        To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
-        The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
-        
-        With the Merlin dataloaders, you can:
-        
-        - Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
-        - Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
-        - Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
-        - Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
-        
-        To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
-        
-        ### Installation
-        
-        #### Installing Merlin Models Using Pip
-        
-        Merlin Models can be installed with `pip` by running the following command:
-        
-        ```shell
-        pip install merlin-models
-        ```
-        
-        > Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
-        > When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
-        
-        #### Docker Containers that include Merlin Models
-        
-        Merlin Models is included in the Merlin Containers.
-        
-        Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
-        
-        #### Installing Merlin Models from Source
-        
-        Merlin Models can be installed from source by running the following commands:
-        
-        ```shell
-        git clone https://github.com/NVIDIA-Merlin/models
-        cd models && pip install -e .
-        ```
-        
-        ### Getting Started
-        
-        Merlin Models makes it straightforward to define architectures that adapt to different input features.
-        This adaptability is provided by building on a core feature of the NVTabular library.
-        When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
-        You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
-        
-        You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
-        After you define the model, you can train and evaluate it with a typical Keras model.
-        
-        ```python
-        import merlin.models.tf as mm
-        from merlin.io.dataset import Dataset
-        
-        train = Dataset(PATH_TO_TRAIN_DATA)
-        valid = Dataset(PATH_TO_VALID_DATA)
-        
-        model = mm.DLRMModel(
-            train.schema,                                                   # 1
-            embedding_dim=64,
-            bottom_block=mm.MLPBlock([128, 64]),                            # 2
-            top_block=mm.MLPBlock([128, 64, 32]),
-            prediction_tasks=mm.BinaryClassificationTask(train.schema)      # 3
-        )
-        
-        model.compile(optimizer="adagrad", run_eagerly=False)
-        model.fit(train, validation_data=valid, batch_size=1024)
-        eval_metrics = model.evaluate(valid, batch_size=1024, return_dict=True)
-        ```
-        
-        1.  To build the internal input layer, the model identifies them from the schema object.
-            The schema identifies the continuous features and categorical features, for which embedding tables are created.
-        2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
-        3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
-            The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
-        
-        You can find more details and information about a low-level API in our overview of the
-        [Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
-        
-        ### Notebook Examples and Tutorials
-        
-        View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
-        
-        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
-        
-        ### Feedback and Support
-        
-        If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-        We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
-        To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
@@ -150,7 +27,133 @@
 Provides-Extra: docs
 Provides-Extra: tensorflow-dev
 Provides-Extra: pytorch-dev
 Provides-Extra: implicit-dev
 Provides-Extra: lightfm-dev
 Provides-Extra: xgboost-dev
 Provides-Extra: all
+License-File: LICENSE
+
+## Merlin Models
+
+[![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
+![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
+
+The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
+that range from classic machine learning models to highly-advanced deep learning models.
+
+The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
+practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
+models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
+example offline
+datasets.
+
+In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
+
+### Benefits of Merlin Models
+
+**[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
+These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
+
+**Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
+The design makes it easy to combine the blocks to define new architectures.
+The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
+
+**Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
+For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
+The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
+
+**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
+When training deep learning recommender system models, data loading can be a bottleneck.
+To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
+The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
+
+With the Merlin dataloaders, you can:
+
+- Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
+- Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
+- Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
+- Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
+
+To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
+
+### Installation
+
+#### Installing Merlin Models Using Pip
+
+Merlin Models can be installed with `pip` by running the following command:
+
+```shell
+pip install merlin-models
+```
+
+> Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
+> When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
+
+#### Docker Containers that include Merlin Models
+
+Merlin Models is included in the Merlin Containers.
+
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
+
+#### Installing Merlin Models from Source
+
+Merlin Models can be installed from source by running the following commands:
+
+```shell
+git clone https://github.com/NVIDIA-Merlin/models
+cd models && pip install -e .
+```
+
+### Getting Started
+
+Merlin Models makes it straightforward to define architectures that adapt to different input features.
+This adaptability is provided by building on a core feature of the NVTabular library.
+When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
+You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
+
+You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
+After you define the model, you can train and evaluate it with a typical Keras model.
+
+```python
+import merlin.models.tf as mm
+from merlin.io.dataset import Dataset
+
+train = Dataset(PATH_TO_TRAIN_DATA)
+valid = Dataset(PATH_TO_VALID_DATA)
+
+model = mm.DLRMModel(
+    train.schema,                                                   # 1
+    embedding_dim=64,
+    bottom_block=mm.MLPBlock([128, 64]),                            # 2
+    top_block=mm.MLPBlock([128, 64, 32]),
+    prediction_tasks=mm.BinaryClassificationTask(train.schema)      # 3
+)
+
+model.compile(optimizer="adagrad", run_eagerly=False)
+model.fit(train, validation_data=valid, batch_size=1024)
+eval_metrics = model.evaluate(valid, batch_size=1024, return_dict=True)
+```
+
+1.  To build the internal input layer, the model identifies them from the schema object.
+    The schema identifies the continuous features and categorical features, for which embedding tables are created.
+2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
+3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
+    The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
+
+You can find more details and information about a low-level API in our overview of the
+[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
+
+### Notebook Examples and Tutorials
+
+View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
+
+The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
+
+### Feedback and Support
+
+If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
+To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
+
+
```

### Comparing `merlin-models-23.4.0/README.md` & `merlin-models-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/__init__.py` & `merlin-models-23.5.0/merlin/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/advertising/__init__.py` & `merlin-models-23.5.0/merlin/datasets/advertising/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/advertising/criteo/__init__.py` & `merlin-models-23.5.0/merlin/datasets/advertising/criteo/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/advertising/criteo/dataset.py` & `merlin-models-23.5.0/merlin/datasets/advertising/criteo/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/__init__.py` & `merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/dataset.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/dataset.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/dataset.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/large/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/large/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/large/schema.json` & `merlin-models-23.5.0/merlin/datasets/ecommerce/large/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/small/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/small/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/small/schema.json` & `merlin-models-23.5.0/merlin/datasets/ecommerce/small/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/__init__.py` & `merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt`

 * *Files 4% similar despite different names*

```diff
@@ -1,160 +1,159 @@
 feature {
-  name: "movieId"
+  name: "user_id"
   type: INT
   int_domain {
-    name: "movieId"
-    max: 1680
+    name: "user_id"
+    max: 100000
     is_categorical: true
   }
   annotation {
-    tag: "item"
+    tag: "user_id"
     tag: "categorical"
-    tag: "item_id"
+    tag: "user"
+    tag: "id"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\r\n\007is_list\022\002 \000\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\200Y@\n\030\n\013cardinality\022\t\021\000\000\000\000\000@\232@\n2\n\010cat_path\022&\032$.//categories/unique.movieId.parquet\n\021\n\013num_buckets\022\002\010\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000"
+      value: "\n\017\n\tis_ragged\022\002 \000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\021\n\013num_buckets\022\002\010\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n2\n\010cat_path\022&\032$.//categories/unique.user_id.parquet\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\r\n\007is_list\022\002 \000\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\200=\030DA\n\026\n\tdimension\022\t\021\000\000\000\000\000\000\200@"
     }
   }
 }
 feature {
-  name: "userId"
+  name: "item_id"
   type: INT
   int_domain {
-    name: "userId"
-    max: 943
+    name: "item_id"
+    max: 179280
     is_categorical: true
   }
   annotation {
+    tag: "item_id"
+    tag: "item"
     tag: "categorical"
-    tag: "user"
-    tag: "user_id"
+    tag: "id"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000x\215@\n\026\n\tdimension\022\t\021\000\000\000\000\000\200R@\n\021\n\013num_buckets\022\002\010\000\n\017\n\tis_ragged\022\002 \000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\r\n\007is_list\022\002 \000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n1\n\010cat_path\022%\032#.//categories/unique.userId.parquet"
+      value: "\n\021\n\013num_buckets\022\002\010\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\000\200@\n\030\n\013cardinality\022\t\021\000\000\000\000\200\342\005A\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n2\n\010cat_path\022&\032$.//categories/unique.item_id.parquet\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000"
     }
   }
 }
 feature {
-  name: "genres"
+  name: "video_category"
   type: INT
   int_domain {
-    name: "genres"
-    max: 216
+    name: "video_category"
+    max: 5
     is_categorical: true
   }
   annotation {
     tag: "item"
     tag: "categorical"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\021\n\013num_buckets\022\002\010\000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000k@\n\026\n\tdimension\022\t\021\000\000\000\000\000\000@@\n1\n\010cat_path\022%\032#.//categories/unique.genres.parquet\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000"
-    }
-  }
-}
-feature {
-  name: "TE_movieId_rating"
-  type: FLOAT
-  annotation {
-    tag: "continuous"
-    extra_metadata {
-      type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\017\n\tis_ragged\022\002 \000"
-    }
-  }
-}
-feature {
-  name: "userId_count"
-  type: FLOAT
-  annotation {
-    tag: "continuous"
-    extra_metadata {
-      type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\017\n\tis_ragged\022\002 \000"
+      value: "\n9\n\010cat_path\022-\032+.//categories/unique.video_category.parquet\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\024@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\r\n\007is_list\022\002 \000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \000\n\021\n\013num_buckets\022\002\010\000"
     }
   }
 }
 feature {
   name: "gender"
   type: INT
   int_domain {
     name: "gender"
-    max: 2
+    max: 5
     is_categorical: true
   }
   annotation {
     tag: "categorical"
     tag: "user"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\000@\n\021\n\013num_buckets\022\002\010\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n1\n\010cat_path\022%\032#.//categories/unique.gender.parquet"
+      value: "\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\024@\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\021\n\013num_buckets\022\002\010\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n1\n\010cat_path\022%\032#.//categories/unique.gender.parquet\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000"
     }
   }
 }
 feature {
-  name: "zip_code"
+  name: "age"
   type: INT
   int_domain {
-    name: "zip_code"
-    max: 795
+    name: "age"
+    max: 10
     is_categorical: true
   }
   annotation {
     tag: "categorical"
     tag: "user"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\330\210@\n\026\n\tdimension\022\t\021\000\000\000\000\000\300P@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n3\n\010cat_path\022\'\032%.//categories/unique.zip_code.parquet\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\021\n\013num_buckets\022\002\010\000"
+      value: "\n\021\n\013num_buckets\022\002\010\000\n.\n\010cat_path\022\"\032 .//categories/unique.age.parquet\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000$@\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000"
     }
   }
 }
 feature {
-  name: "rating"
+  name: "click"
   type: INT
   annotation {
-    tag: "regression"
     tag: "target"
+    tag: "binary_classification"
+    tag: "binary"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\017\n\tis_ragged\022\002 \000"
+      value: "\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000 @"
     }
   }
 }
 feature {
-  name: "rating_binary"
+  name: "follow"
   type: INT
   annotation {
     tag: "target"
     tag: "binary_classification"
+    tag: "binary"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000"
+      value: "\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000 @\n\017\n\tis_ragged\022\002 \000"
     }
   }
 }
 feature {
-  name: "age"
+  name: "like"
   type: INT
-  int_domain {
-    name: "age"
-    max: 8
-    is_categorical: true
+  annotation {
+    tag: "target"
+    tag: "binary_classification"
+    tag: "binary"
+    extra_metadata {
+      type_url: "type.googleapis.com/google.protobuf.Struct"
+      value: "\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000 @\n\017\n\tis_ragged\022\002 \000"
+    }
   }
+}
+feature {
+  name: "share"
+  type: INT
   annotation {
-    tag: "categorical"
-    tag: "user"
+    tag: "target"
+    tag: "binary_classification"
+    tag: "binary"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000 @\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n\021\n\013num_buckets\022\002\010\000\n.\n\010cat_path\022\"\032 .//categories/unique.age.parquet\n\r\n\007is_list\022\002 \000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \000"
+      value: "\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000 @\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000"
     }
   }
 }
 feature {
-  name: "title"
-  type: BYTES
+  name: "watching_times"
+  type: INT
+  int_domain {
+    name: "watching_times"
+    max: 5
+    is_categorical: false
+  }
   annotation {
+    tag: "regression"
+    tag: "target"
     extra_metadata {
       type_url: "type.googleapis.com/google.protobuf.Struct"
-      value: "\n\r\n\007is_list\022\002 \000\n\017\n\tis_ragged\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@"
+      value: "\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\0000@"
     }
   }
 }
+
```

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/dataset.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/schema.json` & `merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975961538461539%*

 * *Differences: {"'feature'": "{2: {'annotation': {'extraMetadata': [OrderedDict([('_dims', [[0.0, None]])])]}}}"}*

```diff
@@ -28,14 +28,24 @@
                 "name": "item_id"
             },
             "name": "item_id",
             "type": "INT"
         },
         {
             "annotation": {
+                "extraMetadata": [
+                    {
+                        "_dims": [
+                            [
+                                0.0,
+                                null
+                            ]
+                        ]
+                    }
+                ],
                 "tag": [
                     "categorical",
                     "item"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
```

### Comparing `merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/__init__.py` & `merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/social/__init__.py` & `merlin-models-23.5.0/merlin/datasets/social/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/social/schema.json` & `merlin-models-23.5.0/merlin/datasets/social/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/synthetic.py` & `merlin-models-23.5.0/merlin/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/testing/__init__.py` & `merlin-models-23.5.0/merlin/datasets/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/testing/schema.json` & `merlin-models-23.5.0/merlin/datasets/testing/schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951704545454545%*

 * *Differences: {"'feature'": "{0: {'intDomain': {'max': '90'}}, 7: {'intDomain': {'max': '100'}, 'annotation': "*

 * *              "{'extraMetadata': [OrderedDict([('_dims', [[0.0, None]])])]}}, 8: {'intDomain': "*

 * *              "{'max': '70'}}}"}*

```diff
@@ -6,15 +6,15 @@
                     "categorical",
                     "user_id",
                     "user"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
-                "max": "1797",
+                "max": "90",
                 "min": "1",
                 "name": "user_id"
             },
             "name": "user_id",
             "type": "INT"
         },
         {
@@ -91,23 +91,33 @@
                 "name": "event_weekday_cos"
             },
             "name": "event_weekday_cos",
             "type": "FLOAT"
         },
         {
             "annotation": {
+                "extraMetadata": [
+                    {
+                        "_dims": [
+                            [
+                                0.0,
+                                null
+                            ]
+                        ]
+                    }
+                ],
                 "tag": [
                     "item_id",
                     "categorical",
                     "item"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
-                "max": "51996",
+                "max": "100",
                 "min": "1",
                 "name": "item_id"
             },
             "name": "item_id",
             "type": "INT"
         },
         {
@@ -116,15 +126,15 @@
                     "list",
                     "categorical",
                     "item"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
-                "max": "331",
+                "max": "70",
                 "min": "1",
                 "name": "categories"
             },
             "name": "categories",
             "type": "INT",
             "valueCount": {
                 "max": "4",
```

### Comparing `merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/__init__.py` & `merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/schema.json` & `merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958806818181818%*

 * *Differences: {"'feature'": "{0: {'intDomain': {'max': '90'}, 'annotation': {'extraMetadata': "*

 * *              "[OrderedDict([('_dims', [[0.0, None]])])]}}, 7: {'intDomain': {'max': '100'}}}"}*

```diff
@@ -1,20 +1,30 @@
 {
     "feature": [
         {
             "annotation": {
+                "extraMetadata": [
+                    {
+                        "_dims": [
+                            [
+                                0.0,
+                                null
+                            ]
+                        ]
+                    }
+                ],
                 "tag": [
                     "categorical",
                     "user_id",
                     "user"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
-                "max": "1797",
+                "max": "90",
                 "min": "1",
                 "name": "test_user_id"
             },
             "name": "test_user_id",
             "type": "INT"
         },
         {
@@ -120,15 +130,15 @@
                     "categorical",
                     "item",
                     "sequence"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
-                "max": "51996",
+                "max": "100",
                 "min": "1",
                 "name": "item_id_seq"
             },
             "name": "item_id_seq",
             "type": "INT",
             "valueCount": {
                 "min": "4"
```

### Comparing `merlin-models-23.4.0/merlin/models/__init__.py` & `merlin-models-23.5.0/merlin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/api.py` & `merlin-models-23.5.0/merlin/models/api.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/config/__init__.py` & `merlin-models-23.5.0/merlin/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/config/schema.py` & `merlin-models-23.5.0/merlin/models/config/schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/implicit/__init__.py` & `merlin-models-23.5.0/merlin/models/implicit/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/io.py` & `merlin-models-23.5.0/merlin/models/io.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/lightfm/__init__.py` & `merlin-models-23.5.0/merlin/models/lightfm/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/loader/__init__.py` & `merlin-models-23.5.0/merlin/models/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/loader/backend.py` & `merlin-models-23.5.0/merlin/models/loader/backend.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from merlin.models.tf.blocks.sampling.cross_batch import PopularityBasedSampler
 from merlin.models.tf.blocks.sampling.in_batch import InBatchSampler
 from merlin.models.tf.blocks.sampling.queue import FIFOQueue
 from merlin.models.tf.core.aggregation import (
     ConcatFeatures,
     ElementwiseSum,
     ElementwiseSumItemMulti,
+    SequenceAggregator,
     StackFeatures,
 )
 from merlin.models.tf.core.base import (
     Block,
     EmbeddingWithMetadata,
     ModelContext,
     NoOp,
@@ -82,19 +83,21 @@
     AverageEmbeddingsByWeightFeature,
     ContinuousEmbedding,
     EmbeddingFeatures,
     EmbeddingOptions,
     Embeddings,
     EmbeddingTable,
     FeatureConfig,
+    PretrainedEmbeddings,
     SequenceEmbeddingFeatures,
     TableConfig,
 )
 from merlin.models.tf.loader import KerasSequenceValidator, Loader, sample_batch
 from merlin.models.tf.losses import LossType
+from merlin.models.tf.metrics.evaluation import LogLossMetric
 from merlin.models.tf.metrics.topk import (
     AvgPrecisionAt,
     MRRAt,
     NDCGAt,
     PrecisionAt,
     RecallAt,
     TopKMetricsAggregator,
@@ -210,14 +213,15 @@
     "ContinuousProjection",
     "EmbeddingFeatures",
     "SequenceEmbeddingFeatures",
     "EmbeddingOptions",
     "EmbeddingTable",
     "AverageEmbeddingsByWeightFeature",
     "Embeddings",
+    "PretrainedEmbeddings",
     "FeatureConfig",
     "TableConfig",
     "ParallelPredictionBlock",
     "TwoTowerBlock",
     "MatrixFactorizationBlock",
     "QueryItemIdsEmbeddingsBlock",
     "PrepareFeatures",
@@ -231,14 +235,15 @@
     "ElementwiseSum",
     "ElementwiseSumItemMulti",
     "AsTabular",
     "ConcatFeatures",
     "Filter",
     "ParallelBlock",
     "StackFeatures",
+    "SequenceAggregator",
     "DotProductInteraction",
     "FMPairwiseInteraction",
     "FMBlock",
     "ToOneHot",
     "ModelOutput",
     "OutputBlock",
     "ColumnBasedSampleWeight",
@@ -297,8 +302,9 @@
     "SequencePredictLast",
     "SequencePredictRandom",
     "SequenceTargetAsInput",
     "SequenceMaskLast",
     "SequenceMaskRandom",
     "ReplaceMaskedEmbeddings",
     "Prediction",
+    "LogLossMetric",
 ]
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/cross.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/cross.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/dlrm.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/dlrm.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/experts.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/experts.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/interaction.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/interaction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/mlp.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,20 @@
         Activation length: {len(activation)}, Dimensions length: {len(dimensions)}"
         )
 
     block_layers = []
 
     for idx, dim in enumerate(dimensions):
         dropout_layer = None
-        activation_idx = activation if isinstance(activation, str) else activation[idx]
+        activation = activation or "linear"
+        if isinstance(activation, str):
+            activation_idx = activation
+        else:
+            activation_idx = activation[idx]
+
         if no_activation_last_layer and idx == len(dimensions) - 1:
             activation_idx = "linear"
         else:
             if dropout:
                 if activation_idx in ["selu", tf.keras.activations.selu]:
                     # Best practice for SeLU. It is also recommended
                     # kernel_initializer="lecun_normal"
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/optimizer.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
       user_tower = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([512, 256]))
       item_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([512, 256]))
       third_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([64]))
       three_tower = ml.ParallelBlock({"user": user_tower, "item": item_tower, "third": third_tower})
       model = ml.Model(three_tower,  ml.BinaryClassificationTask("click"))
 
       # The third_tower would be assigned the default_optimizer ("adagrad" in this example)
-      optimizer = ml.MultiOptimizer(default_optimizer="adagrad",
+      optimizer = ml.MultiOptimizer(default_optimizer=tf.keras.optimizers.legacy.Adagrad(),
         optimizers_and_blocks=[
           ml.OptimizerBlocks(tf.keras.optimizers.legacy.SGD(), user_tower),
           ml.OptimizerBlocks(tf.keras.optimizers.legacy.Adam(), item_tower),
         ])
 
       # The string identification of optimizer is also acceptable, here "sgd" for the third_tower
       # The variables of BinaryClassificationTask("click") would still use the default_optimizer
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/base.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/two_tower.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/two_tower.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/base.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/cross_batch.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/in_batch.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/queue.py` & `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/aggregation.py` & `merlin-models-23.5.0/merlin/models/tf/core/aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,16 +410,18 @@
             for k, v in inputs.items():
                 if len(v.shape) > self.axis + 1:
                     outputs[k] = combiner(v, axis=self.axis, **kwargs)
                 else:
                     outputs[k] = v
             return outputs
         else:
-            assert len(inputs.shape) == 3, "Tensor inputs should be 3-D"
-            return combiner(inputs, axis=self.axis, **kwargs)
+            if inputs.get_shape().rank > self.axis + 1:
+                return combiner(inputs, axis=self.axis, **kwargs)
+            else:
+                return inputs
 
     def parse_combiner(self, combiner):
         if isinstance(combiner, str):
             if combiner == "sum":
                 combiner = tf.reduce_sum
             elif combiner == "max":
                 combiner = tf.reduce_max
@@ -437,14 +439,18 @@
             for k, v in input_shape.items():
                 if len(v) > self.axis + 1:
                     outputs[k] = tf.TensorShape(list(v)[: self.axis] + list(v)[self.axis + 1 :])
                 else:
                     outputs[k] = v
             return outputs
         else:
-            batch_size, _, last_dim = input_shape
-            return batch_size, last_dim
+            if len(input_shape) > self.axis + 1:
+                return tf.TensorShape(
+                    list(input_shape)[: self.axis] + list(input_shape)[self.axis + 1 :]
+                )
+            else:
+                return input_shape
 
     def get_config(self):
         config = super().get_config()
         config.update(axis=self.axis, combiner=self.combiner)
         return config
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/base.py` & `merlin-models-23.5.0/merlin/models/tf/core/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/combinators.py` & `merlin-models-23.5.0/merlin/models/tf/core/combinators.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/encoder.py` & `merlin-models-23.5.0/merlin/models/tf/core/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 
 import os
 from typing import Dict, Optional, Union
 
 import numpy as np
 import tensorflow as tf
-from packaging import version
 
 import merlin.io
 from merlin.models.io import save_merlin_metadata
 from merlin.models.tf.core import combinators
 from merlin.models.tf.core.base import NoOp
 from merlin.models.tf.core.prediction import TopKPrediction
 from merlin.models.tf.inputs.base import InputBlockV2
@@ -210,24 +209,14 @@
     def fit(self, *args, **kwargs):
         """Fit model"""
         raise NotImplementedError(
             "This block is not meant to be trained by itself. ",
             "It can only be trained as part of a model.",
         )
 
-    def _set_save_spec(self, inputs, args=None, kwargs=None):
-        super()._set_save_spec(inputs, args, kwargs)
-
-        # We need to overwrite this in order to fix a Keras-bug in TF<2.9
-        if version.parse(tf.__version__) < version.parse("2.9.0"):
-            # Keras will interpret kwargs like `features` & `targets` as
-            # required args, which is wrong. This is a workaround.
-            _arg_spec = self._saved_model_arg_spec
-            self._saved_model_arg_spec = ([_arg_spec[0][0]], _arg_spec[1])
-
     def save(
         self,
         export_path: Union[str, os.PathLike],
         include_optimizer=True,
         save_traces=True,
     ) -> None:
         """Saves the model to export_path as a Tensorflow Saved Model.
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/index.py` & `merlin-models-23.5.0/merlin/models/tf/core/index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/prediction.py` & `merlin-models-23.5.0/merlin/models/tf/core/prediction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/core/tabular.py` & `merlin-models-23.5.0/merlin/models/tf/core/tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/distributed/backend.py` & `merlin-models-23.5.0/merlin/models/tf/distributed/backend.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/distributed/embedding.py` & `merlin-models-23.5.0/merlin/models/tf/distributed/embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/experimental/sample_weight.py` & `merlin-models-23.5.0/merlin/models/tf/experimental/sample_weight.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/inputs/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/inputs/base.py` & `merlin-models-23.5.0/merlin/models/tf/inputs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from merlin.models.tf.core.combinators import ParallelBlock, TabularAggregationType
 from merlin.models.tf.inputs.continuous import Continuous, ContinuousFeatures
 from merlin.models.tf.inputs.embedding import (
     ContinuousEmbedding,
     EmbeddingFeatures,
     EmbeddingOptions,
     Embeddings,
+    PretrainedEmbeddings,
     SequenceEmbeddingFeatures,
 )
 from merlin.schema import Schema, Tags, TagsType
 
 LOG = logging.getLogger("merlin-models")
 
 
@@ -202,21 +203,23 @@
     kwargs["is_input"] = kwargs.get("is_input", True)
     return ParallelBlock(branches, pre=pre, aggregation=aggregation, post=post, **kwargs)
 
 
 INPUT_TAG_TO_BLOCK: Dict[Tags, Callable[[Schema], Layer]] = {
     Tags.CONTINUOUS: Continuous,
     Tags.CATEGORICAL: Embeddings,
+    Tags.EMBEDDING: PretrainedEmbeddings,
 }
 
 
 def InputBlockV2(
     schema: Optional[Schema] = None,
     categorical: Union[Tags, Layer] = Tags.CATEGORICAL,
     continuous: Union[Tags, Layer] = Tags.CONTINUOUS,
+    pretrained_embeddings: Union[Tags, Layer] = Tags.EMBEDDING,
     pre: Optional[BlockType] = None,
     post: Optional[BlockType] = None,
     aggregation: Optional[TabularAggregationType] = "concat",
     tag_to_block=INPUT_TAG_TO_BLOCK,
     **branches,
 ) -> ParallelBlock:
     """The entry block of the model to process input features from a schema.
@@ -258,19 +261,23 @@
     schema : Schema
         Schema of the input data. This Schema object will be automatically generated using
         [NVTabular](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html).
         Next to this, it's also possible to construct it manually.
     categorical : Union[Tags, Layer], defaults to `Tags.CATEGORICAL`
         A block or column-selector to use for categorical-features.
         If a column-selector is provided (either a schema or tags), the selector
-        will be passed to `Embeddings` to infer the embedding tables from the column-selector.
+        will be passed to `Embeddings()` to infer the embedding tables from the column-selector.
     continuous : Union[Tags, Layer], defaults to `Tags.CONTINUOUS`
         A block to use for continuous-features.
         If a column-selector is provided (either a schema or tags), the selector
-        will be passed to `Continuous` to infer the features from the column-selector.
+        will be passed to `Continuous()` to infer the features from the column-selector.
+    pretrained_embeddings : Union[Tags, Layer], defaults to `Tags.EMBEDDING`
+        A block to use for pre-trained embeddings
+        If a column-selector is provided (either a schema or tags), the selector
+        will be passed to `PretrainedEmbeddings()` to infer the features from the column-selector.
     pre : Optional[BlockType], optional
         Transformation block to apply before the embeddings lookup, by default None
     post : Optional[BlockType], optional
         Transformation block to apply after the embeddings lookup, by default None
     aggregation : Optional[TabularAggregationType], optional
         Transformation block to apply for aggregating the inputs, by default "concat"
     tag_to_block : Dict[str, Callable[[Schema], Layer]], optional
@@ -293,15 +300,20 @@
         warnings.warn(
             "The `embeddings` argument is deprecated and should be replaced "
             "by `categorical` argument",
             DeprecationWarning,
         )
         categorical = branches["embeddings"]
 
-    unparsed = {"categorical": categorical, "continuous": continuous, **branches}
+    unparsed = {
+        "categorical": categorical,
+        "continuous": continuous,
+        "pretrained_embeddings": pretrained_embeddings,
+        **branches,
+    }
     parsed = {}
     for name, branch in unparsed.items():
         if isinstance(branch, Layer):
             parsed[name] = branch
         else:
             if not isinstance(schema, Schema):
                 raise ValueError(
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/inputs/continuous.py` & `merlin-models-23.5.0/merlin/models/tf/inputs/continuous.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/inputs/embedding.py` & `merlin-models-23.5.0/merlin/models/tf/inputs/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 from tensorflow.keras import backend
 from tensorflow.python import to_dlpack
 from tensorflow.python.tpu.tpu_embedding_v2_utils import FeatureConfig, TableConfig
 
 import merlin.io
 from merlin.core.dispatch import DataFrameType
 from merlin.io import Dataset
-from merlin.models.tf.blocks.mlp import InitializerType, RegularizerType
-from merlin.models.tf.core.base import Block, BlockType
+from merlin.models.tf.blocks.mlp import InitializerType, MLPBlock, RegularizerType
+from merlin.models.tf.core.aggregation import SequenceAggregator
+from merlin.models.tf.core.base import Block, BlockType, NoOp, block_registry
 from merlin.models.tf.core.combinators import ParallelBlock, SequentialBlock
 from merlin.models.tf.core.tabular import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     Filter,
     TabularAggregationType,
     TabularBlock,
 )
@@ -419,19 +420,15 @@
                     self.sequence_combiner, tf.keras.layers.Layer
                 ):
                     out = call_layer(self.sequence_combiner, out, **kwargs)
         else:
             if inputs.shape.as_list()[-1] == 1:
                 inputs = tf.squeeze(inputs, axis=-1)
             out = call_layer(self.table, inputs, **kwargs)
-            if len(out.get_shape()) > 2 and self.sequence_combiner is not None:
-                if isinstance(self.sequence_combiner, tf.keras.layers.Layer):
-                    out = call_layer(self.sequence_combiner, out, **kwargs)
-                elif isinstance(self.sequence_combiner, str):
-                    out = process_str_sequence_combiner(out, self.sequence_combiner, **kwargs)
+            out = process_sequence_combiner(out, self.sequence_combiner, **kwargs)
 
         if self.l2_batch_regularization_factor > 0:
             self.add_loss(self.l2_batch_regularization_factor * tf.reduce_sum(tf.square(out)))
 
         if self._dtype_policy.compute_dtype != self._dtype_policy.variable_dtype:
             # Instead of casting the variable as in most layers, cast the output, as
             # this is mathematically equivalent but is faster.
@@ -621,14 +618,103 @@
 
     if not dim:
         dim = infer_dim_fn(col)
 
     return dim
 
 
+def PretrainedEmbeddings(
+    schema: Schema,
+    output_dims: Optional[Union[Dict[str, int], int]] = None,
+    sequence_combiner: Optional[Union[CombinerType, Dict[str, CombinerType]]] = "mean",
+    normalizer: Union[str, tf.keras.layers.Layer] = None,
+    pre: Optional[BlockType] = None,
+    post: Optional[BlockType] = None,
+    aggregation: Optional[TabularAggregationType] = None,
+    block_name: str = "pretrained_embeddings",
+    **kwargs,
+) -> ParallelBlock:
+    """Creates a ParallelBlock with branch for each pre-trained embedding feature
+    in the schema.
+
+    Parameters
+    ----------
+    schema: Schema
+        Schema of the input data, with the pre-trained embeddings.
+        You typically will pass schema.select_by_tag(Tags.EMBEDDING), as that is the tag
+        added to pre-trained embedding features when using the
+        merlin.dataloader.ops.embeddings.EmbeddingOperator
+    output_dims: Optional[Union[Dict[str, int], int]], optional
+        If provided, it projects features to specified dim(s).
+        If an int, all features are projected to that dim.
+        If a dict, only features provided in the dict will be mapped to the specified dim,
+        for example {"feature_name": projection_dim, ...}. By default None
+    sequence_combiner: Optional[Union[str, tf.keras.layers.Layer]], optional
+       A string ("mean", "sum", "max", "min") or Layer specifying
+       how to combine the second dimension of
+       the pre-trained embeddings if it is 3D.
+       Default is None (no sequence combiner used)
+    normalizer: Union[str, tf.keras.layers.Layer], optional
+       A Layer (e.g. mm.L2Norm()) or string ("l2-norm") to be applied
+       to pre-trained embeddings after projected and sequence combined
+       Default is None (no normalization)
+    pre: Optional[BlockType], optional
+        Transformation block to apply before the embeddings lookup, by default None
+    post: Optional[BlockType], optional
+        Transformation block to apply after the embeddings lookup, by default None
+    aggregation: Optional[TabularAggregationType], optional
+        Transformation block to apply for aggregating the inputs, by default None
+    block_name: str, optional
+        Name of the block, by default "pretrained_embeddings"
+    Returns
+    -------
+    ParallelBlock
+        Returns a parallel block with a branch for each pre-trained embedding
+    """
+
+    tables = {}
+
+    for col in schema:
+        table_name = col.name
+
+        tables[table_name] = NoOp()
+
+        if output_dims:
+            new_dim = output_dims
+            if isinstance(output_dims, dict):
+                if table_name in output_dims:
+                    new_dim = (
+                        output_dims[table_name] if isinstance(output_dims, dict) else output_dims
+                    )
+                else:
+                    new_dim = None
+            if new_dim:
+                tables[table_name] = MLPBlock([new_dim], activation=None)
+
+        if sequence_combiner:
+            if isinstance(sequence_combiner, str):
+                sequence_combiner = SequenceAggregator(sequence_combiner)
+
+            tables[table_name] = SequentialBlock([tables[table_name], sequence_combiner])
+
+        if normalizer:
+            normalizer = block_registry.parse(normalizer)
+            tables[table_name] = SequentialBlock([tables[table_name], normalizer])
+
+    return ParallelBlock(
+        tables,
+        pre=pre,
+        post=post,
+        aggregation=aggregation,
+        name=block_name,
+        schema=schema,
+        **kwargs,
+    )
+
+
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class AverageEmbeddingsByWeightFeature(tf.keras.layers.Layer):
     def __init__(self, weight_feature_name: str, axis=1, **kwargs):
         """Computes the weighted average of a Tensor based
         on one of the input features.
         Typically used as a combiner for EmbeddingTable
         for aggregating sequential embedding features
@@ -1211,37 +1297,50 @@
         feature_config_dict = dict(name=val.name, max_sequence_length=val.max_sequence_length)
         feature_config_dict["table"] = serialize_table_config(feature_config_dict["table"])
         outputs[key] = feature_config_dict
 
     return outputs
 
 
+def process_sequence_combiner(inputs, combiner, **kwargs):
+    result = inputs
+    if len(inputs.get_shape()) > 2 and combiner:
+        if isinstance(combiner, tf.keras.layers.Layer):
+            result = call_layer(combiner, inputs, **kwargs)
+        elif isinstance(combiner, str):
+            result = process_str_sequence_combiner(inputs, combiner, **kwargs)
+
+    return result
+
+
 def process_str_sequence_combiner(
     inputs: Union[tf.Tensor, tf.RaggedTensor], combiner: str, **kwargs
 ) -> tf.Tensor:
-    """Process inputs with str sequence combiners ("mean" or "sum")
+    """Process inputs with str sequence combiners ("mean", "sum" or "max")
 
     Parameters
     ----------
     inputs : Union[tf.Tensor, tf.RaggedTensor]
         Input 3D tensor (batch size, seq length, embedding dim)
     combiner : str
-        The combiner: "mean" or "sum"
+        The combiner: "mean", "sum" or "max"
 
     Returns
     -------
     tf.Tensor
         A 2D tensor with values combined on axis=1
     """
     if not combiner or len(inputs.get_shape()) <= 2:
         return inputs
     if combiner == "mean":
         combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1))
     elif combiner == "sum":
         combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_sum(x, axis=1))
+    elif combiner == "max":
+        combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_max(x, axis=1))
     else:
         raise ValueError(
-            "Only 'mean' and 'sum' str combiners is implemented for dense"
+            "Only 'mean', 'sum', and 'max' str combiners is implemented for dense"
             " list/multi-hot embedded features. You can also"
             " provide a tf.keras.layers.Layer instance as a sequence combiner."
         )
     return call_layer(combiner, inputs, **kwargs)
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/loader.py` & `merlin-models-23.5.0/merlin/models/tf/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,14 +262,15 @@
         global_size=None,
         global_rank=None,
         drop_last=False,
         sparse_names=None,
         sparse_max=None,
         sparse_as_dense=False,
         schema=None,
+        **loader_kwargs,
     ):
         dataset = _validate_dataset(
             paths_or_dataset, batch_size, buffer_size, engine, device, reader_kwargs
         )
         if schema:
             dataset.schema = schema
 
@@ -316,14 +317,15 @@
             shuffle=shuffle,
             seed_fn=seed_fn,
             parts_per_chunk=parts_per_chunk,
             device=device,
             global_size=global_size,
             global_rank=global_rank,
             drop_last=drop_last,
+            **loader_kwargs,
         )
 
         # Override these parameters after initializing the parent dataloader
         # class since the new dataloader will use sparse tensors for list
         # columns by default, but sparse tensors were disabled by default
         # and were optional in the old version of merlin.loader.
         self.sparse_names = sparse_names or []
@@ -402,15 +404,15 @@
         loader = dataset_or_loader
 
     batch = loader.peek()
     # batch could be of type Prediction, so we can't unpack directly
     inputs, targets = batch[0], batch[1]
 
     if prepare_features:
-        pf = PrepareFeatures(loader.schema)
+        pf = PrepareFeatures(loader.output_schema)
         if targets is not None:
             inputs, targets = pf(inputs, targets=targets)
         else:
             inputs = pf(inputs)
 
     if not include_targets:
         return inputs
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/losses/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/losses/base.py` & `merlin-models-23.5.0/merlin/models/tf/losses/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/losses/listwise.py` & `merlin-models-23.5.0/merlin/models/tf/losses/listwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/losses/pairwise.py` & `merlin-models-23.5.0/merlin/models/tf/losses/pairwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/metrics/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/metrics/evaluation.py` & `merlin-models-23.5.0/merlin/models/tf/metrics/evaluation.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 
 # Adapted from source code: https://github.com/karlhigley/ranking-metrics-torch
 from typing import Optional, Sequence, Union
 
 import tensorflow as tf
 from tensorflow.keras import backend
+from tensorflow.keras.losses import binary_crossentropy
 from tensorflow.keras.metrics import Mean, Metric
 from tensorflow.keras.metrics import get as get_metric
 
 from merlin.models.tf.metrics import metrics_registry
 from merlin.models.tf.utils.tf_utils import get_candidate_probs
 
 EPSILON = 1e-16
@@ -35,14 +36,54 @@
     k : int
         The cut-off for popularity metrics
 """
 
 MetricType = Union[Metric, str]
 
 
+@tf.keras.utils.register_keras_serializable(package="merlin.models")
+@metrics_registry.register_with_multiple_names("logloss")
+class LogLossMetric(Mean):
+    """Log loss metric.
+    Keras offers the log loss (a.k.a. binary cross entropy), but it
+    may be affected by class weights, which you might not
+    want for the metric calculation).
+    This is the corresponding metric, that is useful to evaluate
+    the performance of binary classification tasks.
+
+    Parameters
+    ----------
+    name : str, optional
+        Name of the metric, by default "logloss"
+    from_logits : bool, optional
+        Whether the metric should expect the likelihood (e.g. sigmoid function in output)
+        or logits (False). By default False
+    dtype
+        Dtype of metric output, by default None
+    """
+
+    def __init__(self, name="logloss", from_logits=False, dtype=None):
+        self.from_logits = from_logits
+        super().__init__(name=name, dtype=dtype)
+
+    def update_state(
+        self,
+        y_true: tf.Tensor,
+        y_pred: tf.Tensor,
+        sample_weight: Optional[tf.Tensor] = None,
+    ):
+        result = binary_crossentropy(y_true, y_pred, from_logits=self.from_logits)
+        return super().update_state(result, sample_weight=sample_weight)
+
+    def get_config(self):
+        config = super().get_config()
+        config["from_logits"] = self.from_logits
+        return config
+
+
 def novelty_at(
     predicted_candidates_probs: tf.Tensor,
     k: int = 5,
 ) -> tf.Tensor:
     """
     Computes novely@K metric
     ----------
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/metrics/topk.py` & `merlin-models-23.5.0/merlin/models/tf/metrics/topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/models/base.py` & `merlin-models-23.5.0/merlin/models/tf/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,24 +278,14 @@
         block = tf.keras.utils.deserialize_keras_object(config.pop("block"))
 
         return cls(block, **config)
 
     def get_config(self):
         return {"block": tf.keras.utils.serialize_keras_object(self.block)}
 
-    def _set_save_spec(self, inputs, args=None, kwargs=None):
-        # We need to overwrite this in order to fix a Keras-bug in TF<2.9
-        super()._set_save_spec(inputs, args, kwargs)
-
-        if version.parse(tf.__version__) < version.parse("2.9.0"):
-            # Keras will interpret kwargs like `features` & `targets` as
-            # required args, which is wrong. This is a workaround.
-            _arg_spec = self._saved_model_arg_spec
-            self._saved_model_arg_spec = ([_arg_spec[0][0]], _arg_spec[1])
-
 
 class BaseModel(tf.keras.Model):
     def __init__(self, **kwargs):
         super(BaseModel, self).__init__(**kwargs)
 
         # Initializing model control flags controlled by MetricsComputeCallback()
         self._should_compute_train_metrics_for_batch = tf.Variable(
@@ -1941,24 +1931,14 @@
         config["schema"] = schema_utils.schema_to_tensorflow_metadata_json(self.schema)
         for i, layer in enumerate(self.blocks):
             config[i] = tf.keras.utils.serialize_keras_object(layer)
         config["batch_size"] = self._batch_size
 
         return config
 
-    def _set_save_spec(self, inputs, args=None, kwargs=None):
-        # We need to overwrite this in order to fix a Keras-bug in TF<2.9
-        super()._set_save_spec(inputs, args, kwargs)
-
-        if version.parse(tf.__version__) < version.parse("2.9.0"):
-            # Keras will interpret kwargs like `features` & `targets` as
-            # required args, which is wrong. This is a workaround.
-            _arg_spec = self._saved_model_arg_spec
-            self._saved_model_arg_spec = ([_arg_spec[0][0]], _arg_spec[1])
-
     @property
     def frozen_blocks(self):
         """
         Get frozen blocks of model, only on which you called freeze_blocks before, the result dose
         not include those blocks frozen in other methods, for example, if you create the embedding
         and set the `trainable` as False, it would not be tracked by this property, but you can also
         call unfreeze_blocks on those blocks.
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/models/benchmark.py` & `merlin-models-23.5.0/merlin/models/tf/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/models/ranking.py` & `merlin-models-23.5.0/merlin/models/tf/models/ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,19 +433,21 @@
         sparse embeddings parameters (FTRL). You can implement that by using `MultiOptimizer` class.
         For example:
         ```python
             wide_model = model.blocks[0].parallel_layers["wide"]
             deep_model = model.blocks[0].parallel_layers["deep"]
 
             multi_optimizer = ml.MultiOptimizer(
-                default_optimizer="adagrad",
+                default_optimizer=tf.keras.optimizers.legacy.Adagrad(learning_rate=0.001),
                 optimizers_and_blocks=[
                     ml.OptimizerBlocks("ftrl", wide_model),
-                    ml.OptimizerBlocks("adagrad", deep_model),
-                ],
+                    ml.OptimizerBlocks(
+                    tf.keras.optimizers.legacy.Adagrad(learning_rate=0.001), deep_model
+                    ),
+                    ],
             )
         ```
 
     References
     ----------
     [1] Cheng, Koc, Harmsen, Shaked, Chandra, Aradhye, Anderson et al. "Wide & deep learning for
     recommender systems." In Proceedings of the 1st workshop on deep learning for recommender
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/models/retrieval.py` & `merlin-models-23.5.0/merlin/models/tf/models/retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/models/utils.py` & `merlin-models-23.5.0/merlin/models/tf/models/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/base.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/block.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/classification.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/contrastive.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/contrastive.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,40 +219,63 @@
             return self.call_contrastive(inputs, **call_kwargs)
 
         return tf_utils.call_layer(self.to_call, inputs, **call_kwargs)
 
     def call_contrastive(self, inputs, features, targets, training=False, testing=False):
         if isinstance(inputs, dict) and self.query_name in inputs:
             query_embedding = inputs[self.query_name]
-        elif isinstance(inputs, tf.Tensor):
+        elif isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
             query_embedding = inputs
         else:
             raise ValueError("Couldn't infer query embedding")
 
+        is_ragged = isinstance(query_embedding, tf.RaggedTensor)
+        if is_ragged:
+            # Get flat values of the ragged tensor
+            original_query_embedding = query_embedding
+            query_embedding = query_embedding.flat_values
+
         if self.has_candidate_weights:
             positive_id = targets
             if isinstance(targets, dict):
                 positive_id = targets[self.col_schema.name]
             positive_embedding = self.embedding_lookup(positive_id)
         else:
             positive_id = features[self.col_schema.name]
             positive_embedding = inputs[self.candidate_name]
 
+        if isinstance(positive_id, tf.RaggedTensor):
+            # Select positive candidates at masked positions
+            target_mask = positive_id._keras_mask.with_row_splits_dtype(
+                positive_id.row_splits.dtype
+            )
+            # Flatten target tensor to have the same shape as the query tensor
+            positive_id = tf.ragged.boolean_mask(positive_id, target_mask)
+            original_target = positive_id
+            positive_id = positive_id.flat_values
+            positive_embedding = tf.ragged.boolean_mask(positive_embedding, target_mask).flat_values
+
         positive = Candidate(id=positive_id, metadata={**features}).with_embedding(
             positive_embedding
         )
         negative, positive = self.sample_negatives(
             positive, features, training=training, testing=testing
         )
         if self.has_candidate_weights and (
             positive.id.shape != negative.id.shape or positive != negative
         ):
             negative = negative.with_embedding(self.embedding_lookup(negative.id))
 
-        return self.outputs(query_embedding, positive, negative)
+        logits = self.outputs(query_embedding, positive, negative)
+        if is_ragged:
+            logits.copy_with_updates(
+                outputs=original_query_embedding.with_flat_values(logits.outputs),
+                targets=original_target.with_flat_values(logits.targets),
+            )
+        return logits
 
     def outputs(
         self, query_embedding: tf.Tensor, positive: Candidate, negative: Candidate
     ) -> Prediction:
         """Method to compute the dot product between the query embeddings and
         positive/negative candidates
 
@@ -378,15 +401,15 @@
         if len(candidates) > 1:
             for neg in candidates[1:]:
                 negatives += neg
 
         return negatives, positive
 
     def embedding_lookup(self, ids: tf.Tensor):
-        return self.to_call.embedding_lookup(tf.squeeze(ids))
+        return self.to_call.embedding_lookup(tf.squeeze(ids, axis=-1))
 
     def to_dataset(self, gpu=None) -> merlin.io.Dataset:
         return merlin.io.Dataset(tf_utils.tensor_to_df(self.to_call.embeddings, gpu=gpu))
 
     @property
     def has_candidate_weights(self) -> bool:
         if isinstance(self.to_call, DotProduct):
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/regression.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/sampling/base.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/sampling/in_batch.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/sampling/popularity.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/popularity.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         by using tf.random.log_uniform_candidate_sampler()
 
         Returns
         -------
         tf.Tensor
             Probabilities of each item to be sampled
         """
-        log_indices = tf.math.log(tf.range(1.0, self.max_id - self.min_id + 2.0, 1.0))
+        log_indices = tf.math.log(tf.range(1.0, self.max_id - self.min_id + 3.0, 1.0))
         sampling_probs = (log_indices[1:] - log_indices[:-1]) / log_indices[-1]
 
         if self.unique:
             # Below is a more numerically stable implementation of the probability of
             # sampling an item at least once (suitable for sampling unique items)
             # P(item is sampled at least once) = 1 - P(item is not sampled)^num_trials
             # where P(item is not sampled) = 1-p and p is the
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/outputs/topk.py` & `merlin-models-23.5.0/merlin/models/tf/outputs/topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/base.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/classification.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/multi.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/multi.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/next_item.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/next_item.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/regression.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/retrieval.py` & `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transformers/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transformers/block.py` & `merlin-models-23.5.0/merlin/models/tf/transformers/block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transformers/transforms.py` & `merlin-models-23.5.0/merlin/models/tf/transformers/transforms.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/bias.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/bias.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/features.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,31 +177,47 @@
                 if col_schema_shape.is_list:
                     if name in inputs:
                         val = inputs[name]
                         if isinstance(val, tf.RaggedTensor):
                             val = inputs[name]
                         elif isinstance(val, tf.SparseTensor):
                             val = tf.RaggedTensor.from_sparse(val)
+                        else:
+                            if Tags.EMBEDDING in self.schema[name].tags:
+                                # This fix ensures that for pre-trained embeddings
+                                # the last dim is defined (not None) in graph mode
+                                val = tf.reshape(val, (-1, col_schema_shape.dims[-1].max))
                     else:
                         if col_schema_shape.is_ragged:
                             if f"{name}__values" not in inputs or f"{name}__offsets" not in inputs:
                                 raise ValueError(
                                     f"The ragged list feature '{name}' is expected to be "
                                     f"represented by two features in the inputs: '{name}__values' "
                                     f"and '{name}__offsets', but they were not found."
                                 )
+                            ragged_values = inputs[f"{name}__values"]
+                            if Tags.EMBEDDING in self.schema[name].tags:
+                                # This fix ensures that for pre-trained embeddings
+                                # the last dim is defined (not None) in graph mode
+                                ragged_values = tf.reshape(
+                                    ragged_values, (-1, col_schema_shape.dims[-1].max)
+                                )
                             val = list_col_to_ragged(
-                                inputs[f"{name}__values"], inputs[f"{name}__offsets"]
+                                ragged_values,
+                                inputs[f"{name}__offsets"],
                             )
+
                             del inputs[f"{name}__values"]
                             del inputs[f"{name}__offsets"]
                         else:
                             raise ValueError(f"Feature '{name}' was not found in the inputs")
 
-                    if len(val.shape) == 2:
+                    if len(val.shape) == 2 and Tags.EMBEDDING not in self.schema[name].tags:
+                        # Only expands 2D sequential features if
+                        # they are not pre-trained embeeddings
                         val = tf.expand_dims(val, axis=-1)
 
                     if self.list_as_dense:
                         val = to_dense(val, max_seq_length=col_schema_shape.dims[1].max)
 
                 elif name in inputs:
                     val = inputs[name]
@@ -237,18 +253,24 @@
                             if col_schema_shape.dims[1] is None:
                                 raise Exception(
                                     f"List feature {name} does not have maximum"
                                     "length set in the schema ({col_schema_shape})"
                                 )
                             seq_length = int(col_schema_shape.dims[1].max)
 
-                        output_shapes[name] = tf.TensorShape([batch_size, seq_length, 1])
+                        last_dim = 1
+                        if Tags.EMBEDDING in self.schema[name].tags:
+                            last_dim = col_schema_shape[-1].max
+                        output_shapes[name] = tf.TensorShape([batch_size, seq_length, last_dim])
 
                     else:
-                        if len(input_shapes[name]) == 2:
+                        if (
+                            len(input_shapes[name]) == 2
+                            and Tags.EMBEDDING not in self.schema[name].tags
+                        ):
                             output_shapes[name] = input_shapes[name] + (1,)
 
                 elif name in input_shapes:
                     output_shapes[name] = input_shapes[name]
 
         # Adding other inputs that might not be in the schema,
         # as they might be treated by other block
@@ -312,24 +334,24 @@
         out_targets = {}
         if self.has_schema:
             # Preparing non-list features and targets
             for name in self.schema.column_names:
                 if name in inputs:
                     val = inputs[name]
 
-                    if not self.schema[name].shape.is_list:
+                    if not self.schema[name].shape.is_list and val.get_shape().rank == 1:
                         # Expanding / setting last dim of non-list input features to be 2D
                         val = tf.reshape(val, (-1, 1))
 
                     outputs[name] = val
 
                 if isinstance(targets, dict) and name in targets:
                     val = targets[name]
 
-                    if not self.schema[name].shape.is_list:
+                    if not self.schema[name].shape.is_list and val.get_shape().rank == 1:
                         # Expanding / setting last dim of non-list target features to be 2D
                         val = tf.reshape(val, (-1, 1))
 
                     out_targets[name] = val
 
         # Adding other inputs that might not be in the schema,
         # as they might be treated by other block
@@ -349,14 +371,15 @@
             elif targets.get_shape().rank == 1:
                 # Expanding / setting last dim of non-list
                 # target features to be 2D
                 out_targets = tf.reshape(targets, (-1, 1))
             else:
                 out_targets = targets
             return (outputs, out_targets)
+
         return outputs
 
     def compute_output_shape(self, input_shapes):
         output_shapes = self.prepare_lists.compute_output_shape(input_shapes)
 
         if self.has_schema:
             for name in self.schema.column_names:
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/negative_sampling.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/noise.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/regularization.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/regularization.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,43 @@
     """Apply L2-normalization to input tensors along a given axis"""
 
     def __init__(self, **kwargs):
         super(L2Norm, self).__init__(**kwargs)
 
     def call(self, inputs: Union[tf.Tensor, TabularData], axis: int = -1, **kwargs):
         if isinstance(inputs, dict):
-            inputs = {key: tf.linalg.l2_normalize(inp, axis=axis) for key, inp in inputs.items()}
+            inputs = {key: self._l2_norm(inp, axis=axis) for key, inp in inputs.items()}
         else:
-            inputs = tf.linalg.l2_normalize(inputs, axis=axis)
+            inputs = self._l2_norm(inputs, axis=axis)
 
         return inputs
 
+    def _l2_norm(
+        self,
+        inputs: Union[tf.Tensor, tf.SparseTensor, tf.RaggedTensor],
+        epsilon: float = 1e-12,
+        axis: int = -1,
+    ) -> Union[tf.Tensor, tf.SparseTensor, tf.RaggedTensor]:
+        """Computes L2-norm for a given axis, typically axis = -1.
+        Equivalent to tf.linalg.l2_normalize(), but that function
+        does not support tf.RaggedTensor
+
+        Parameters
+        ----------
+        inputs : Union[tf.Tensor, tf.SparseTensor, tf.RaggedTensor]
+            A dense or sparse/ragged tensor
+        epsilon : float, optional
+            A small value to add to the sum(vector**2) to avoid div by 0, by default 1e-12
+        axis : int, optional
+            The axis on which to normalize, by default -1
+
+        Returns
+        -------
+        Union[tf.Tensor, tf.SparseTensor, tf.RaggedTensor]
+            The L2 normalized tensor
+        """
+        return inputs / tf.math.sqrt(
+            tf.math.maximum(tf.reduce_sum(tf.pow(inputs, 2), axis=axis, keepdims=True), epsilon)
+        )
+
     def compute_output_shape(self, input_shape):
         return input_shape
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/sequence.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,17 @@
             )
 
         seq_inputs_shapes = {
             col: inputs[col].get_shape().as_list() for col in self.schema.column_names
         }
 
         seq_shapes = list(seq_inputs_shapes.values())
-        if not all(x == seq_shapes[0] for x in seq_shapes):
+        if not all(x[:2] == seq_shapes[0][:2] for x in seq_shapes):
             raise ValueError(
-                "The sequential inputs must have the same shape, but the shapes "
+                "The sequential inputs must have the first two dims equal, but they "
                 f"are different: {seq_inputs_shapes}"
             )
 
     def compute_output_shape(self, input_shape):
         new_input_shapes = dict()
         for k, v in input_shape.items():
             new_input_shapes[k] = v
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/transforms/tensor.py` & `merlin-models-23.5.0/merlin/models/tf/transforms/tensor.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/typing.py` & `merlin-models-23.5.0/merlin/models/tf/typing.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/__init__.py` & `merlin-models-23.5.0/merlin/models/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/batch_utils.py` & `merlin-models-23.5.0/merlin/models/tf/utils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/repr_utils.py` & `merlin-models-23.5.0/merlin/models/tf/utils/repr_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/search_utils.py` & `merlin-models-23.5.0/merlin/models/tf/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/testing_utils.py` & `merlin-models-23.5.0/merlin/models/tf/utils/testing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,18 +109,18 @@
 
         model_preds = model.predict(iter(batch))
         loaded_model_preds = loaded_model.predict(iter(batch))
 
         if isinstance(model_preds, dict):
             for task_name in model_preds:
                 tf.debugging.assert_near(
-                    model_preds[task_name], loaded_model_preds[task_name], atol=1e-5
+                    model_preds[task_name], loaded_model_preds[task_name], atol=1e-4
                 )
         else:
-            tf.debugging.assert_near(model_preds, loaded_model_preds, atol=1e-5)
+            tf.debugging.assert_near(model_preds, loaded_model_preds, atol=1e-4)
 
         loaded_model.compile(run_eagerly=run_eagerly, optimizer=optimizer, **kwargs)
         loaded_model.fit(iter(batch))
 
         if model.input_schema:
             signature = loaded_model.signatures["serving_default"]
             signature_input_names = set(signature.structured_input_signature[1].keys())
@@ -165,16 +165,19 @@
 
 
 def numeric_test(actual, expected):
     np.testing.assert_allclose(actual, expected, rtol=1e-3, atol=1e-6)
 
 
 # This function is copied from keras/testing_infra/test_utils.py
-# We need it here because this was not publicly exposed prior to 2.9.0
-# and our CI tests multiple versions of tensorflow/keras
+# We need it here because the EmbeddingTable signature requires us to pass some args
+# as positional instead of keyword arguments
+# If we change the signature of EmbeddingTable,
+# or if keras adds support for passing args as well as kwargs
+# we may be able to remove this in future and replace with the keras version
 @disable_cudnn_autotune
 def layer_test(
     layer_cls,
     args=None,
     kwargs=None,
     input_shape=None,
     input_dtype=None,
```

### Comparing `merlin-models-23.4.0/merlin/models/tf/utils/tf_utils.py` & `merlin-models-23.5.0/merlin/models/tf/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/torch/block/__init__.py` & `merlin-models-23.5.0/merlin/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/torch/block/base.py` & `merlin-models-23.5.0/merlin/models/torch/block.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,321 +1,337 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import abc
-import inspect
-import logging
-from collections import OrderedDict
-from typing import List, Optional, Union
+from copy import deepcopy
+from typing import Dict, Optional, Union
 
 import torch
-from torch.nn import Module
+from torch import nn
 
-from merlin.models.torch.utils import torch_utils
-from merlin.models.utils.misc_utils import filter_kwargs
+from merlin.models.torch.batch import Batch
+from merlin.models.torch.container import BlockContainer, BlockContainerDict
 
-LOG = logging.getLogger("merlin.models")
 
+class Block(BlockContainer):
+    """A base-class that calls it's modules sequentially.
 
-class BlockBase(torch_utils.OutputSizeMixin, torch.nn.Module, metaclass=abc.ABCMeta):
-    def to_model(self, prediction_task_or_head, inputs=None, **kwargs):
-        """Converts the block to a model
+    Parameters
+    ----------
+    *module : nn.Module
+        Variable length argument list of PyTorch modules to be contained in the block.
+    name : Optional[str], default = None
+        The name of the block. If None, no name is assigned.
+    """
+
+    def __init__(self, *module: nn.Module, name: Optional[str] = None):
+        super().__init__(*module, name=name)
+
+    def forward(
+        self, inputs: Union[torch.Tensor, Dict[str, torch.Tensor]], batch: Optional[Batch] = None
+    ):
+        """
+        Forward pass through the block. Applies each contained module sequentially on the input.
 
         Parameters
         ----------
-        prediction_task_or_head
-            Prediction task or head
-        inputs, optional
-            Inputs, by default None
+        inputs : Union[torch.Tensor, Dict[str, torch.Tensor]]
+            The input data as a tensor or a dictionary of tensors.
+        batch : Optional[Batch], default = None
+            Optional batch of data. If provided, it is used by the `module`s.
 
         Returns
         -------
-        Model
-            Returns a model from a block
+        torch.Tensor or Dict[str, torch.Tensor]
+            The output of the block after processing the input.
         """
-        from merlin.models.torch.model.base import Head, Model, PredictionTask
-
-        if isinstance(prediction_task_or_head, PredictionTask):
-            head = prediction_task_or_head.to_head(self, inputs=inputs, **kwargs)
-        elif isinstance(prediction_task_or_head, Head):
-            head = prediction_task_or_head
-        else:
-            raise ValueError(
-                "`prediction_task_or_head` needs to be a `Head` or `PredictionTask` "
-                f"found: {type(prediction_task_or_head)}"
-            )
+        for module in self.values:
+            inputs = module(inputs, batch=batch)
 
-        return Model(head, **kwargs)
+        return inputs
 
-    def as_tabular(self, name=None):
-        """Makes the output of the block a Tabular output
+    def repeat(self, n: int = 1, name=None) -> "Block":
+        """
+        Creates a new block by repeating the current block `n` times.
+        Each repetition is a deep copy of the current block.
 
         Parameters
         ----------
-        name : str, optional
-            Name of the key for tabular output dict, by default None
+        n : int
+            The number of times to repeat the current block.
+        name : Optional[str], default = None
+            The name for the new block. If None, no name is assigned.
 
         Returns
         -------
-        SequentialBlock
-            The input block with tabular data output
+        Block
+            The new block created by repeating the current block `n` times.
         """
-        from merlin.models.torch.tabular.base import AsTabular
-
-        if not name:
-            name = self.name
+        if not isinstance(n, int):
+            raise TypeError("n must be an integer")
 
-        return SequentialBlock(self, AsTabular(name))
+        if n < 1:
+            raise ValueError("n must be greater than 0")
 
+        repeats = [self.copy() for _ in range(n - 1)]
 
-class Block(BlockBase):
-    """Core abstraction in Merlin models."""
+        return Block(self, *repeats, name=name)
 
-    def __init__(self, module: torch.nn.Module, output_size: Union[List[int], torch.Size]):
-        super().__init__()
-        self.module = module
-        self._output_size = output_size
+    def copy(self) -> "Block":
+        """
+        Creates a deep copy of the current block.
 
-    def forward(self, inputs):
-        return self.module(inputs)
+        Returns
+        -------
+        Block
+            The copy of the current block.
+        """
+        return deepcopy(self)
 
-    def forward_output_size(self, input_size):
-        if self._output_size[0] is None:
-            batch_size = torch_utils.calculate_batch_size_from_input_size(input_size)
 
-            return [batch_size] + self._output_size[1:]
+class ParallelBlock(Block):
+    """A base-class that calls it's modules in parallel.
 
-        return self._output_size
+    A ParallelBlock contains multiple branches that will be executed
+    in parallel. Each branch can contain multiple modules, and
+    the outputs of all branches are collected into a dictionary.
+
+    If a branch returns a dictionary of tensors instead of a single tensor,
+    it will be flattened into the output dictionary. This ensures the output-type
+    is always Dict[str, torch.Tensor].
+
+    Example usage::
+        >>> parallel_block = ParallelBlock({"a": nn.LazyLinear(2), "b": nn.LazyLinear(2)})
+        >>> x = torch.randn(2, 2)
+        >>> output = parallel_block(x)
+        >>> # The output is a dictionary containing the output of each branch
+        >>> print(output)
+        {
+            'a': tensor([[-0.0801,  0.0436],
+                        [ 0.1235, -0.0318]]),
+            'b': tensor([[ 0.0918, -0.0274],
+                        [-0.0652,  0.0381]])
+        }
+
+    Parameters
+    ----------
+    *module : nn.Module
+        Variable length argument list of PyTorch modules to be contained in the block.
+    name : Optional[str], default = None
+        The name of the block. If None, no name is assigned.
+    """
+
+    def __init__(
+        self,
+        *inputs: Union[nn.Module, Dict[str, nn.Module]],
+    ):
+        pre = BlockContainer(name="pre")
+        branches = BlockContainerDict(*inputs)
+        post = BlockContainer(name="post")
 
+        super().__init__()
 
-class SequentialBlock(BlockBase, torch.nn.Sequential):
-    def __init__(self, *args, output_size=None):
-        """Create a composition.
+        self.pre = pre
+        self.branches = branches
+        self.post = post
+
+    def forward(
+        self, inputs: Union[torch.Tensor, Dict[str, torch.Tensor]], batch: Optional[Batch] = None
+    ):
+        """Forward pass through the block.
+
+        The steps are as follows:
+        1. Pre-processing stage: Applies each module in the pre-processing stage sequentially.
+        2. Branching stage: Applies each module in each branch sequentially.
+        3. Post-processing stage: Applies each module in the post-processing stage sequentially.
+
+        If a branch returns a dictionary of tensors instead of a single tensor,
+        it will be flattened into the output dictionary. This ensures the output-type
+        is always Dict[str, torch.Tensor].
 
         Parameters
         ----------
-        *args:
-            A list or tuple of layers to compose.
-        """
+        inputs : Union[torch.Tensor, Dict[str, torch.Tensor]]
+            The input tensor or dictionary of tensors.
+        batch : Optional[Batch], default=None
+            An optional batch of data.
 
-        super().__init__()
-        self._static_output_size = output_size
-        self.input_size = None
-
-        if len(args) == 1 and isinstance(args[0], OrderedDict):
-            last = None
-            for idx, key, module in enumerate(args[0].items()):
-                self.add_module_and_maybe_build(key, module, last, idx)
-                last = module
-        else:
-            if len(args) == 1 and isinstance(args[0], list):
-                args = args[0]
-            last = None
-            for idx, module in enumerate(args):
-                last = self.add_module_and_maybe_build(str(idx), module, last, idx)
-
-    @property
-    def inputs(self):
-        from merlin.models.torch import TabularFeatures
-
-        first = list(self)[0]
-        if isinstance(first, TabularFeatures):
-            return first
-
-    def add_module(self, name: str, module: Optional[Module]) -> None:
-        from merlin.models.torch.tabular.base import FilterFeatures
-
-        if isinstance(module, list):
-            module = FilterFeatures(module)
-        super().add_module(name, module)
-
-    def add_module_and_maybe_build(self, name: str, module, parent, idx) -> torch.nn.Module:
-        # Check if module needs to be built
-        if getattr(parent, "output_size", None) and getattr(module, "build", None):
-            module = module.build(parent.output_size())
+        Returns
+        -------
+        Dict[str, torch.Tensor]
+            The output tensors.
+        """
+        for module in self.pre.values:
+            inputs = module(inputs, batch=batch)
 
-        if idx == 0:
-            self.input_size = getattr(module, "input_size", None)
+        outputs = {}
+        for name, branch_container in self.branches.items():
+            branch = inputs
+            for module in branch_container.values:
+                branch = module(branch, batch=batch)
+
+            if isinstance(branch, torch.Tensor):
+                branch_dict = {name: branch}
+            elif torch.jit.isinstance(branch, Dict[str, torch.Tensor]):
+                branch_dict = branch
+            else:
+                raise TypeError(
+                    f"Branch output must be a tensor or a dictionary of tensors. Got {type(branch)}"
+                )
 
-        self.add_module(name, module)
+            for key in branch_dict.keys():
+                if key in outputs:
+                    raise RuntimeError(f"Duplicate output name: {key}")
 
-        return module
+            outputs.update(branch_dict)
 
-    def __rrshift__(self, other):
-        return right_shift_block(self, other)
+        for module in self.post.values:
+            outputs = module(outputs, batch=batch)
 
-    def __rshift__(self, other):
-        # pylint: disable=arguments-out-of-order
-        return right_shift_block(other, self)
+        return outputs
 
-    def forward(self, input, training=False, **kwargs):
-        """Forwards inputs over this block
+    def append(self, module: nn.Module):
+        """Appends a module to the post-processing stage.
 
         Parameters
         ----------
-        input : Tensor
-            Tensor or dict of tensors
-        training : bool, optional
-            Training flag, by default False
+        module : nn.Module
+            The module to append.
 
         Returns
         -------
-        Tensor or dict of tensors
-            Output of the block
+        ParallelBlock
+            The current object itself.
         """
 
-        for i, module in enumerate(self):
-            if i == len(self) - 1:
-                filtered_kwargs = filter_kwargs(kwargs, module)
-                input = module(input, **filtered_kwargs)
+        self.post.append(module)
 
-            elif "training" in inspect.signature(module.forward).parameters:
-                input = module(input, training=training)
-            else:
-                input = module(input)
-
-        return input
+        return self
 
-    def build(self, input_size, schema=None, **kwargs):
-        """Build the block
+    def prepend(self, module: nn.Module):
+        """Prepends a module to the pre-processing stage.
 
         Parameters
         ----------
-        input_size : tuple
-            The input shape
-        schema : Schema, optional
-            Features schema, by default None
-        """
-        output_size = input_size
-        for module in self:
-            if not hasattr(module, "build"):
-                break
-            module.build(output_size, schema=schema)
-            output_size = module.output_size()
-
-        return super(SequentialBlock, self).build(input_size, schema=None, **kwargs)
-
-    def as_tabular(self, name=None):
-        from merlin.models.torch import AsTabular
-
-        if not name:
-            name = self.name
+        module : nn.Module
+            The module to prepend.
 
-        return SequentialBlock(self, AsTabular(name))
+        Returns
+        -------
+        ParallelBlock
+            The current object itself.
+        """
 
-    def __add__(self, other):
-        from merlin.models.torch.tabular.base import merge_tabular
+        self.pre.prepend(module)
 
-        return merge_tabular(self, other)
+        return self
 
-    def forward_output_size(self, input_size):
-        if self._static_output_size:
-            return self._static_output_size
+    def append_to(self, name: str, module: nn.Module):
+        """Appends a module to a specified branch.
 
-        x = input_size
-        for module in list(self):
-            if getattr(module, "output_size", None):
-                x = module.output_size(x)
-            else:
-                # TODO log warning here
-                return None
-
-        return x
+        Parameters
+        ----------
+        name : str
+            The name of the branch.
+        module : nn.Module
+            The module to append.
 
-    @staticmethod
-    def get_children_by_class_name(parent, *class_name):
-        children = []
+        Returns
+        -------
+        ParallelBlock
+            The current object itself.
+        """
 
-        def add_if_class_name_matches(to_check):
-            if to_check.__class__.__name__ in class_name:
-                children.append(to_check)
+        self.branches[name].append(module)
 
-        for child in parent:
-            if getattr(child, "merge_values", None):
-                for to_merge in child.merge_values:
-                    add_if_class_name_matches(to_merge)
+        return self
 
-            add_if_class_name_matches(child)
+    def prepend_to(self, name: str, module: nn.Module):
+        """Prepends a module to a specified branch.
 
-        return children
+        Parameters
+        ----------
+        name : str
+            The name of the branch.
+        module : nn.Module
+            The module to prepend.
 
+        Returns
+        -------
+        ParallelBlock
+            The current object itself.
+        """
+        self.branches[name].prepend(module)
 
-def build_blocks(*modules):
-    return list(SequentialBlock(*modules))
+        return self
 
+    def append_for_each(self, module: nn.Module, shared=False):
+        """Appends a module to each branch.
 
-class BuildableBlock(abc.ABC):
-    @abc.abstractmethod
-    def build(self, input_size) -> BlockBase:
-        raise NotImplementedError
+        Parameters
+        ----------
+        module : nn.Module
+            The module to append.
+        shared : bool, default=False
+            If True, the same module is shared across all branches.
+            Otherwise a deep copy of the module is used in each branch.
 
-    def __rrshift__(self, other):
-        return right_shift_block(self, other)
+        Returns
+        -------
+        ParallelBlock
+            The current object itself.
+        """
 
-    def to_module(self, shape_or_module):
-        shape = shape_or_module
-        if isinstance(shape_or_module, torch.nn.Module):
-            shape = getattr(shape_or_module, "output_size", None)
-            if shape:
-                shape = shape()
+        self.branches.append_for_each(module, shared=shared)
 
-        return self.build(shape)
+        return self
 
+    def prepend_for_each(self, module: nn.Module, shared=False):
+        """Prepends a module to each branch.
 
-def right_shift_block(self, other):
-    from merlin.models.torch.tabular.base import FilterFeatures
+        Parameters
+        ----------
+        module : nn.Module
+            The module to prepend.
+        shared : bool, default=False
+            If True, the same module is shared across all branches.
+            Otherwise a deep copy of the module is used in each branch.
 
-    if isinstance(other, list):
-        left_side = [FilterFeatures(other)]
-    else:
-        left_side = list(other) if isinstance(other, SequentialBlock) else [other]
-    right_side = list(self) if isinstance(self, SequentialBlock) else [self]
+        Returns
+        -------
+        ParallelBlock
+            The current object itself.
+        """
 
-    # Maybe build right-side
-    if hasattr(left_side[-1], "output_size") and left_side[-1].output_size():
-        _right_side = []
-        x = left_side[-1].output_size()
-        for module in right_side:
-            if getattr(module, "build", None):
-                if "parents" in inspect.signature(module.build).parameters:
-                    build = module.build(x, left_side)
-                else:
-                    build = module.build(x)
-                if build:
-                    module = build
-                x = module.output_size() if hasattr(module, "output_size") else None
-            _right_side.append(module)
-        right_side = _right_side
+        self.branches.prepend_for_each(module, shared=shared)
 
-    sequential = left_side + right_side
+        return self
 
-    need_moving_to_gpu = False
-    if isinstance(self, torch.nn.Module):
-        need_moving_to_gpu = need_moving_to_gpu or torch_utils.check_gpu(self)
-    if isinstance(other, torch.nn.Module):
-        need_moving_to_gpu = need_moving_to_gpu or torch_utils.check_gpu(other)
+    def __getitem__(self, idx: Union[slice, int, str]):
+        if isinstance(idx, str) and idx in self.branches:
+            return self.branches[idx]
 
-    out = SequentialBlock(*sequential)
-    if getattr(left_side[-1], "input_size", None) and left_side[-1].input_size:
-        out.input_size = left_side[-1].input_size
+        if idx == 0:
+            return self.pre
 
-    if need_moving_to_gpu:
-        out.to("cuda")
+        if idx == -1 or idx == 2:
+            return self.post
 
-    return out
+        raise IndexError(f"Index {idx} is out of range for {self.__class__.__name__}")
 
+    def __len__(self):
+        return len(self.branches)
 
-BlockType = Union[BlockBase, BuildableBlock]
-BlockOrModule = Union[BlockBase, BuildableBlock, torch.nn.Module]
+    def __contains__(self, name):
+        return name in self.branches
```

### Comparing `merlin-models-23.4.0/merlin/models/torch/features/__init__.py` & `merlin-models-23.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/torch/features/base.py` & `merlin-models-23.5.0/tests/unit/implicit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import pytest
 
-from abc import ABC
-
-from merlin.models.torch.tabular.base import TabularBlock
-
-
-class InputBlock(TabularBlock, ABC):
-    pass
+pytest.importorskip("implicit")
```

### Comparing `merlin-models-23.4.0/merlin/models/torch/model/__init__.py` & `merlin-models-23.5.0/tests/common/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/torch/tabular/__init__.py` & `merlin-models-23.5.0/tests/common/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/torch/typing.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_in_batch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2022, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import tensorflow as tf
 
-import typing
-from typing import Dict
+from merlin.models.tf.blocks.sampling.in_batch import InBatchSampler
 
-import torch
 
-# TODO: Make this more generic and work with multi-hot features
-TabularData = Dict[str, torch.Tensor]
-TensorOrTabularData = typing.Union[torch.Tensor, TabularData]
-
-
-__all__ = [
-    "TabularData",
-    "TensorOrTabularData",
-]
+def test_in_batch_sampler_reload():
+    batch_size = 43
+    sampler = InBatchSampler(batch_size=batch_size)
+    serialized = tf.keras.layers.serialize(sampler)
+    reloaded = tf.keras.layers.deserialize(serialized)
+    assert reloaded.batch_size == batch_size
```

### Comparing `merlin-models-23.4.0/merlin/models/torch/utils/__init__.py` & `merlin-models-23.5.0/tests/common/tf/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/constants.py` & `merlin-models-23.5.0/merlin/models/utils/constants.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/dataset.py` & `merlin-models-23.5.0/merlin/models/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/dependencies.py` & `merlin-models-23.5.0/merlin/models/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/doc_utils.py` & `merlin-models-23.5.0/merlin/models/utils/doc_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/example_utils.py` & `merlin-models-23.5.0/merlin/models/utils/example_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/misc_utils.py` & `merlin-models-23.5.0/merlin/models/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/nvt_utils.py` & `merlin-models-23.5.0/merlin/models/utils/nvt_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/registry.py` & `merlin-models-23.5.0/merlin/models/utils/registry.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/utils/schema_utils.py` & `merlin-models-23.5.0/merlin/models/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin/models/xgb/__init__.py` & `merlin-models-23.5.0/merlin/models/xgb/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/merlin_models.egg-info/PKG-INFO` & `merlin-models-23.5.0/merlin_models.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,137 +1,14 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.4.0
+Version: 23.5.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
-Description: ## Merlin Models
-        
-        [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
-        ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
-        [![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
-        
-        The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
-        that range from classic machine learning models to highly-advanced deep learning models.
-        
-        The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
-        practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
-        models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
-        example offline
-        datasets.
-        
-        In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
-        
-        ### Benefits of Merlin Models
-        
-        **[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
-        These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
-        
-        **Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
-        The design makes it easy to combine the blocks to define new architectures.
-        The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
-        
-        **Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
-        For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
-        The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
-        
-        **[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
-        When training deep learning recommender system models, data loading can be a bottleneck.
-        To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
-        The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
-        
-        With the Merlin dataloaders, you can:
-        
-        - Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
-        - Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
-        - Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
-        - Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
-        
-        To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
-        
-        ### Installation
-        
-        #### Installing Merlin Models Using Pip
-        
-        Merlin Models can be installed with `pip` by running the following command:
-        
-        ```shell
-        pip install merlin-models
-        ```
-        
-        > Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
-        > When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
-        
-        #### Docker Containers that include Merlin Models
-        
-        Merlin Models is included in the Merlin Containers.
-        
-        Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
-        
-        #### Installing Merlin Models from Source
-        
-        Merlin Models can be installed from source by running the following commands:
-        
-        ```shell
-        git clone https://github.com/NVIDIA-Merlin/models
-        cd models && pip install -e .
-        ```
-        
-        ### Getting Started
-        
-        Merlin Models makes it straightforward to define architectures that adapt to different input features.
-        This adaptability is provided by building on a core feature of the NVTabular library.
-        When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
-        You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
-        
-        You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
-        After you define the model, you can train and evaluate it with a typical Keras model.
-        
-        ```python
-        import merlin.models.tf as mm
-        from merlin.io.dataset import Dataset
-        
-        train = Dataset(PATH_TO_TRAIN_DATA)
-        valid = Dataset(PATH_TO_VALID_DATA)
-        
-        model = mm.DLRMModel(
-            train.schema,                                                   # 1
-            embedding_dim=64,
-            bottom_block=mm.MLPBlock([128, 64]),                            # 2
-            top_block=mm.MLPBlock([128, 64, 32]),
-            prediction_tasks=mm.BinaryClassificationTask(train.schema)      # 3
-        )
-        
-        model.compile(optimizer="adagrad", run_eagerly=False)
-        model.fit(train, validation_data=valid, batch_size=1024)
-        eval_metrics = model.evaluate(valid, batch_size=1024, return_dict=True)
-        ```
-        
-        1.  To build the internal input layer, the model identifies them from the schema object.
-            The schema identifies the continuous features and categorical features, for which embedding tables are created.
-        2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
-        3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
-            The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
-        
-        You can find more details and information about a low-level API in our overview of the
-        [Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
-        
-        ### Notebook Examples and Tutorials
-        
-        View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
-        
-        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
-        
-        ### Feedback and Support
-        
-        If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-        We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
-        To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
@@ -150,7 +27,133 @@
 Provides-Extra: docs
 Provides-Extra: tensorflow-dev
 Provides-Extra: pytorch-dev
 Provides-Extra: implicit-dev
 Provides-Extra: lightfm-dev
 Provides-Extra: xgboost-dev
 Provides-Extra: all
+License-File: LICENSE
+
+## Merlin Models
+
+[![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
+![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
+
+The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
+that range from classic machine learning models to highly-advanced deep learning models.
+
+The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
+practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
+models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
+example offline
+datasets.
+
+In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
+
+### Benefits of Merlin Models
+
+**[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
+These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
+
+**Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
+The design makes it easy to combine the blocks to define new architectures.
+The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
+
+**Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
+For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
+The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
+
+**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
+When training deep learning recommender system models, data loading can be a bottleneck.
+To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
+The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
+
+With the Merlin dataloaders, you can:
+
+- Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
+- Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
+- Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
+- Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
+
+To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
+
+### Installation
+
+#### Installing Merlin Models Using Pip
+
+Merlin Models can be installed with `pip` by running the following command:
+
+```shell
+pip install merlin-models
+```
+
+> Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
+> When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
+
+#### Docker Containers that include Merlin Models
+
+Merlin Models is included in the Merlin Containers.
+
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
+
+#### Installing Merlin Models from Source
+
+Merlin Models can be installed from source by running the following commands:
+
+```shell
+git clone https://github.com/NVIDIA-Merlin/models
+cd models && pip install -e .
+```
+
+### Getting Started
+
+Merlin Models makes it straightforward to define architectures that adapt to different input features.
+This adaptability is provided by building on a core feature of the NVTabular library.
+When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
+You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
+
+You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
+After you define the model, you can train and evaluate it with a typical Keras model.
+
+```python
+import merlin.models.tf as mm
+from merlin.io.dataset import Dataset
+
+train = Dataset(PATH_TO_TRAIN_DATA)
+valid = Dataset(PATH_TO_VALID_DATA)
+
+model = mm.DLRMModel(
+    train.schema,                                                   # 1
+    embedding_dim=64,
+    bottom_block=mm.MLPBlock([128, 64]),                            # 2
+    top_block=mm.MLPBlock([128, 64, 32]),
+    prediction_tasks=mm.BinaryClassificationTask(train.schema)      # 3
+)
+
+model.compile(optimizer="adagrad", run_eagerly=False)
+model.fit(train, validation_data=valid, batch_size=1024)
+eval_metrics = model.evaluate(valid, batch_size=1024, return_dict=True)
+```
+
+1.  To build the internal input layer, the model identifies them from the schema object.
+    The schema identifies the continuous features and categorical features, for which embedding tables are created.
+2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
+3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
+    The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
+
+You can find more details and information about a low-level API in our overview of the
+[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
+
+### Notebook Examples and Tutorials
+
+View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
+
+The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
+
+### Feedback and Support
+
+If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
+To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
+
+
```

### Comparing `merlin-models-23.4.0/merlin_models.egg-info/SOURCES.txt` & `merlin-models-23.5.0/merlin_models.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .pre-commit-config.yaml
 CLA.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
+Makefile
 README.md
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
 versioneer.py
+conda/recipes/meta.yaml
 merlin/datasets/__init__.py
 merlin/datasets/synthetic.py
 merlin/datasets/advertising/__init__.py
 merlin/datasets/advertising/criteo/__init__.py
 merlin/datasets/advertising/criteo/dataset.py
 merlin/datasets/advertising/criteo/transformed/__init__.py
 merlin/datasets/advertising/criteo/transformed/schema.pbtxt
@@ -40,15 +42,15 @@
 merlin/datasets/ecommerce/small/schema.json
 merlin/datasets/ecommerce/transactions/__init__.py
 merlin/datasets/ecommerce/transactions/schema.pbtxt
 merlin/datasets/entertainment/__init__.py
 merlin/datasets/entertainment/movielens/__init__.py
 merlin/datasets/entertainment/movielens/dataset.py
 merlin/datasets/entertainment/movielens/100k/__init__.py
-merlin/datasets/entertainment/movielens/100k/schema.pbtxt
+merlin/datasets/entertainment/movielens/100k/schema.json
 merlin/datasets/entertainment/movielens/1m/__init__.py
 merlin/datasets/entertainment/movielens/1m/schema.pbtxt
 merlin/datasets/entertainment/movielens/1m-raw/__init__.py
 merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
 merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
 merlin/datasets/entertainment/movielens/25m/__init__.py
 merlin/datasets/entertainment/movielens/25m/schema.pbtxt
@@ -104,14 +106,15 @@
 merlin/models/tf/distributed/backend.py
 merlin/models/tf/distributed/embedding.py
 merlin/models/tf/experimental/sample_weight.py
 merlin/models/tf/inputs/__init__.py
 merlin/models/tf/inputs/base.py
 merlin/models/tf/inputs/continuous.py
 merlin/models/tf/inputs/embedding.py
+merlin/models/tf/logging/callbacks.py
 merlin/models/tf/losses/__init__.py
 merlin/models/tf/losses/base.py
 merlin/models/tf/losses/listwise.py
 merlin/models/tf/losses/pairwise.py
 merlin/models/tf/metrics/__init__.py
 merlin/models/tf/metrics/evaluation.py
 merlin/models/tf/metrics/topk.py
@@ -153,35 +156,20 @@
 merlin/models/tf/utils/__init__.py
 merlin/models/tf/utils/batch_utils.py
 merlin/models/tf/utils/repr_utils.py
 merlin/models/tf/utils/search_utils.py
 merlin/models/tf/utils/testing_utils.py
 merlin/models/tf/utils/tf_utils.py
 merlin/models/torch/__init__.py
-merlin/models/torch/losses.py
-merlin/models/torch/typing.py
-merlin/models/torch/block/__init__.py
-merlin/models/torch/block/base.py
-merlin/models/torch/block/mlp.py
-merlin/models/torch/features/__init__.py
-merlin/models/torch/features/base.py
-merlin/models/torch/features/continuous.py
-merlin/models/torch/features/embedding.py
-merlin/models/torch/features/tabular.py
-merlin/models/torch/model/__init__.py
-merlin/models/torch/model/base.py
-merlin/models/torch/model/prediction_task.py
-merlin/models/torch/tabular/__init__.py
-merlin/models/torch/tabular/aggregation.py
-merlin/models/torch/tabular/base.py
-merlin/models/torch/tabular/transformations.py
+merlin/models/torch/batch.py
+merlin/models/torch/block.py
+merlin/models/torch/container.py
 merlin/models/torch/utils/__init__.py
-merlin/models/torch/utils/data_utils.py
-merlin/models/torch/utils/examples_utils.py
-merlin/models/torch/utils/torch_utils.py
+merlin/models/torch/utils/module_utils.py
+merlin/models/torch/utils/torchscript_utils.py
 merlin/models/utils/__init__.py
 merlin/models/utils/constants.py
 merlin/models/utils/dataset.py
 merlin/models/utils/dependencies.py
 merlin/models/utils/doc_utils.py
 merlin/models/utils/example_utils.py
 merlin/models/utils/misc_utils.py
@@ -193,14 +181,15 @@
 merlin_models.egg-info/SOURCES.txt
 merlin_models.egg-info/dependency_links.txt
 merlin_models.egg-info/requires.txt
 merlin_models.egg-info/top_level.txt
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
+requirements/horovod-cpu-environment.yml
 requirements/horovod.txt
 requirements/implicit.txt
 requirements/lightfm.txt
 requirements/nvtabular.txt
 requirements/pytorch.txt
 requirements/tensorflow.txt
 requirements/test.txt
@@ -291,15 +280,15 @@
 tests/unit/tf/inputs/test_embedding.py
 tests/unit/tf/inputs/test_tabular.py
 tests/unit/tf/layers/__init__.py
 tests/unit/tf/layers/test_queue.py
 tests/unit/tf/losses/__init__.py
 tests/unit/tf/losses/test_losses.py
 tests/unit/tf/metrics/__init__.py
-tests/unit/tf/metrics/test_metrics_popularity.py
+tests/unit/tf/metrics/test_metrics.py
 tests/unit/tf/metrics/test_metrics_topk.py
 tests/unit/tf/models/__init__.py
 tests/unit/tf/models/test_base.py
 tests/unit/tf/models/test_benchmark.py
 tests/unit/tf/models/test_ranking.py
 tests/unit/tf/models/test_retrieval.py
 tests/unit/tf/outputs/__init__.py
@@ -328,29 +317,16 @@
 tests/unit/tf/transforms/test_sequence.py
 tests/unit/tf/transforms/test_tensor.py
 tests/unit/tf/utils/__init__.py
 tests/unit/tf/utils/test_batch.py
 tests/unit/tf/utils/test_dataset.py
 tests/unit/tf/utils/test_tf_utils.py
 tests/unit/torch/__init__.py
-tests/unit/torch/_conftest.py
-tests/unit/torch/test_dataloader_utils.py
-tests/unit/torch/test_losses.py
-tests/unit/torch/test_public_api.py
-tests/unit/torch/block/__init__.py
-tests/unit/torch/block/test_base.py
-tests/unit/torch/block/test_mlp.py
-tests/unit/torch/features/__init__.py
-tests/unit/torch/features/test_continuous.py
-tests/unit/torch/features/test_embedding.py
-tests/unit/torch/features/test_tabular.py
-tests/unit/torch/model/__init__.py
-tests/unit/torch/model/test_head.py
-tests/unit/torch/model/test_model.py
-tests/unit/torch/tabular/__init__.py
-tests/unit/torch/tabular/test_aggregation.py
-tests/unit/torch/tabular/test_tabular.py
-tests/unit/torch/tabular/test_transformations.py
+tests/unit/torch/test_batch.py
+tests/unit/torch/test_block.py
+tests/unit/torch/test_container.py
 tests/unit/torch/utils/__init__.py
+tests/unit/torch/utils/test_module_utils.py
+tests/unit/torch/utils/test_torchscript_utils.py
 tests/unit/utils/test_schema_utils.py
 tests/unit/xgb/__init__.py
 tests/unit/xgb/test_xgboost.py
```

### Comparing `merlin-models-23.4.0/merlin_models.egg-info/requires.txt` & `merlin-models-23.5.0/merlin_models.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 merlin-core>=23.4.0
 merlin-dataloader>=23.4.0
 
 [all]
 merlin-core>=23.4.0
 merlin-dataloader>=23.4.0
-tensorflow>=2.8
+tensorflow>=2.9
 torch>=1.0
 torchmetrics>=0.10.0
 lightfm>=1.0.0
 implicit>=0.5.2
 xgboost>=1.0.0
 transformers<5,>=4.23
 horovod
@@ -164,18 +164,18 @@
 fiddle==0.2.2
 wandb
 optuna
 plotly
 nvtabular>=1.0.0
 
 [tensorflow]
-tensorflow>=2.8
+tensorflow>=2.9
 
 [tensorflow-dev]
-tensorflow>=2.8
+tensorflow>=2.9
 transformers<5,>=4.23
 bokeh
 check-manifest
 pytest>=5
 pytest-cov>=2
 pytest-xdist
 black==20.8b1
```

### Comparing `merlin-models-23.4.0/pyproject.toml` & `merlin-models-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/pytest.ini` & `merlin-models-23.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/setup.cfg` & `merlin-models-23.5.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 exclude = build,.eggs
 
 [flake8_nb]
 max-line-length = 120
 ignore = E203,E402,W503
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = merlin/models/_version.py
 versionfile_build = merlin/models/_version.py
 tag_prefix = v
 parentdir_prefix = merlin-models-
 
 [mypy]
```

### Comparing `merlin-models-23.4.0/setup.py` & `merlin-models-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/common/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/common/tf/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/common/tf/retrieval/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_config.py` & `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import fiddle as fdl
 
 from merlin.io import Dataset
+from merlin.models.tf.logging.callbacks import WandbLogger
 from tests.common.tf.retrieval.retrieval_utils import (
     RetrievalTrainEvalRunner,
     RetrievalTrainEvalRunnerV2,
-    WandbLogger,
     filter_schema,
     get_callbacks,
     get_dual_encoder_model,
     get_dual_encoder_model_v2,
     get_item_frequencies,
     get_loss,
     get_metrics,
@@ -55,15 +55,19 @@
     train_ds: Dataset,
     eval_ds: Dataset,
     model_type: str,
     log_to_wandb: bool,
     wandb_project: str,
     retrieval_api_version: int,
 ):
-    wandb_logger_cfg = fdl.Config(WandbLogger, enabled=log_to_wandb, wandb_project=wandb_project)
+    wandb_logger_cfg = None
+    if log_to_wandb:
+        wandb_logger_cfg = fdl.Config(
+            WandbLogger, wandb_project=wandb_project, auto_init=log_to_wandb
+        )
 
     schema_cfg = fdl.Config(filter_schema, schema=train_ds.schema)
     optimizer = fdl.Config(get_optimizer)
     metrics = fdl.Config(get_metrics)
     loss = fdl.Config(get_loss)
     callbacks = fdl.Config(get_callbacks, wandb_logger=wandb_logger_cfg)
     if retrieval_api_version == 1:
```

### Comparing `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_tests_common.py` & `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_tests_common.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_utils.py` & `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import logging
 import os
 import time
 from dataclasses import dataclass
 from functools import partial
 from typing import Any, Optional
 
 import numpy as np
 import tensorflow as tf
-import wandb
 from tensorflow.keras import regularizers
 from tensorflow.keras.utils import set_random_seed
 
 import merlin.models.tf as mm
 from merlin.io.dataset import Dataset
+from merlin.models.tf.logging.callbacks import ExamplesPerSecondCallback
 from merlin.models.tf.outputs.base import DotProduct
 from merlin.models.tf.transforms.bias import PopularityLogitsCorrection
 from merlin.models.utils import schema_utils
 from merlin.models.utils.dataset import unique_rows_by_features
 from merlin.schema.tags import Tags
 
 
@@ -490,139 +489,40 @@
     if optimizer == "adam":
         opt = tf.keras.optimizers.Adam(
             learning_rate=lerning_rate,
             clipnorm=opt_clip_norm,
             clipvalue=opt_clip_value,
         )
     elif optimizer == "adagrad":
-        opt = tf.keras.optimizers.Adagrad(
+        opt = tf.keras.optimizers.legacy.Adagrad(
             learning_rate=lerning_rate,
             clipnorm=opt_clip_norm,
             clipvalue=opt_clip_value,
         )
     else:
         raise ValueError("Invalid optimizer")
 
     return opt
 
 
-class ExamplesPerSecondCallback(tf.keras.callbacks.Callback):
-    """ExamplesPerSecond callback.
-    This callback records the average_examples_per_sec and
-    current_examples_per_sec during training.
-    """
-
-    def __init__(self, batch_size, every_n_steps=1, log_as_print=True, wandb_logger=None):
-        self.log_as_print = log_as_print
-        self.wandb_logger = wandb_logger
-        self._batch_size = batch_size
-        self._every_n_steps = every_n_steps
-        super(ExamplesPerSecondCallback, self).__init__()
-
-    def on_train_begin(self, logs=None):
-        self._first_batch = True
-        self._epoch_steps = 0
-        self._train_batches_average_examples_per_sec = []
-        # self._train_start_time = time.time()
-        # self._last_recorded_time = time.time()
-
-    def on_train_end(self, logs=None):
-        average_examples_per_sec = self.get_avg_examples_per_sec()
-        self._train_batches_average_examples_per_sec.append(average_examples_per_sec)
-
-    def get_train_batches_mean_of_avg_examples_per_sec(self):
-        if len(self._train_batches_average_examples_per_sec) > 0:
-            return np.mean(self._train_batches_average_examples_per_sec)
-        else:
-            return 0.0
-
-    def get_avg_examples_per_sec(self):
-        current_time = time.time()
-        average_examples_per_sec = self._batch_size * (
-            self._epoch_steps / (current_time - self._epoch_start_time)
-        )
-        return average_examples_per_sec
-
-    def on_train_batch_end(self, batch, logs=None):
-        # Discards the first batch, as it is used to compile the
-        # graph and affects the average
-        if self._first_batch:
-            self._epoch_steps = 0
-            self._first_batch = False
-            self._epoch_start_time = time.time()
-            self._last_recorded_time = time.time()
-            return
-
-        """Log the examples_per_sec metric every_n_steps."""
-        self._epoch_steps += 1
-        current_time = time.time()
-
-        if self._epoch_steps % self._every_n_steps == 0:
-            average_examples_per_sec = self.get_avg_examples_per_sec()
-            current_examples_per_sec = self._batch_size * (
-                self._every_n_steps / (current_time - self._last_recorded_time)
-            )
-
-            if self.log_as_print:
-                logging.info(
-                    f"[Examples/sec - Epoch step: {self._epoch_steps}] "
-                    f"current: {current_examples_per_sec:.2f}, avg: {average_examples_per_sec:.2f}"
-                )
-
-            self.wandb_logger.log(
-                {
-                    "current_examples_per_sec": current_examples_per_sec,
-                    "average_examples_per_sec": average_examples_per_sec,
-                }
-            )
-
-            self._last_recorded_time = current_time  # Update last_recorded_time
-
-
 def get_callbacks(train_batch_size=16, metrics_log_frequency=10, wandb_logger=None):
-    callbacks = [
-        ExamplesPerSecondCallback(
-            train_batch_size, every_n_steps=metrics_log_frequency, wandb_logger=wandb_logger
-        )
-    ]
+    callbacks = []
 
     if wandb_logger:
         wandb_callback = wandb_logger.get_callback(metrics_log_frequency=metrics_log_frequency)
         if wandb_callback:
             callbacks.append(wandb_callback)
 
-    return callbacks
-
-
-class WandbLogger:
-    def __init__(self, enabled, wandb_project="", config={}):
-        self.enabled = enabled
-        if self.enabled:
-            wandb.init(project=wandb_project, config=config)
-
-    def config(self, config={}):
-        if self.enabled:
-            wandb.config.update(config)
-
-    def log(self, metrics):
-        if self.enabled:
-            wandb.log(metrics)
-
-    def get_callback(self, metrics_log_frequency, save_model=False, save_graph=False):
-        callback = None
-        if self.enabled:
-            callback = wandb.keras.WandbCallback(
-                log_batch_frequency=metrics_log_frequency,
-                save_model=save_model,
-                save_graph=save_graph,
-            )
-        return callback
+    callbacks.append(
+        ExamplesPerSecondCallback(
+            train_batch_size, every_n_steps=metrics_log_frequency, logger=wandb_logger
+        )
+    )
 
-    def teardown(self, exit_code=0):
-        wandb.finish(exit_code=exit_code)
+    return callbacks
 
 
 @dataclass
 class RetrievalTrainEvalRunner:
     wandb_logger: Any = None
     model_type: str = None
     schema: Any = None
@@ -643,15 +543,17 @@
     eval_batch_size: int = 128
 
     def run(self, hparams):
         start_time = time.time()
 
         set_random_seed(self.random_seed)
 
-        self.wandb_logger.config(hparams)
+        if self.wandb_logger:
+            self.wandb_logger.config(hparams)
+            self.wandb_logger.init()
 
         # Marks W&B execution as failed by default
         exit_code = 1
         try:
             self.model.compile(
                 run_eagerly=False, optimizer=self.optimizer, loss=self.loss, metrics=self.metrics
             )
@@ -704,20 +606,22 @@
             )[0]
             avg_examples_per_sec = (
                 examples_per_sec_callback.get_train_batches_mean_of_avg_examples_per_sec()
             )
             final_metrics["avg_examples_per_sec"] = avg_examples_per_sec
 
             final_metrics = {f"{k}-final": v for k, v in final_metrics.items()}
-            self.wandb_logger.log(final_metrics)
+            if self.wandb_logger:
+                self.wandb_logger.log(final_metrics)
 
             # Marks W&B execution as successfully finished
             exit_code = 0
         finally:
-            self.wandb_logger.teardown(exit_code=exit_code)
+            if self.wandb_logger:
+                self.wandb_logger.teardown(exit_code=exit_code)
 
         return final_metrics
 
 
 @dataclass
 class RetrievalTrainEvalRunnerV2:
     wandb_logger: Any = None
@@ -740,15 +644,16 @@
     eval_batch_size: int = 128
 
     def run(self, hparams):
         start_time = time.time()
 
         set_random_seed(self.random_seed)
 
-        self.wandb_logger.config(hparams)
+        if self.wandb_logger:
+            self.wandb_logger.config(hparams)
 
         # Marks W&B execution as failed by default
         exit_code = 1
         try:
             self.model.compile(
                 run_eagerly=False, optimizer=self.optimizer, loss=self.loss, metrics=self.metrics
             )
@@ -821,10 +726,11 @@
 
             final_metrics = {f"{k}-final": v for k, v in final_metrics.items()}
             self.wandb_logger.log(final_metrics)
 
             # Marks W&B execution as successfully finished
             exit_code = 0
         finally:
-            self.wandb_logger.teardown(exit_code=exit_code)
+            if self.wandb_logger:
+                self.wandb_logger.teardown(exit_code=exit_code)
 
         return final_metrics
```

### Comparing `merlin-models-23.4.0/tests/common/tf/tests_utils.py` & `merlin-models-23.5.0/tests/common/tf/tests_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/conftest.py` & `merlin-models-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/__init__.py` & `merlin-models-23.5.0/tests/integration/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/retrieval/__init__.py` & `merlin-models-23.5.0/tests/integration/tf/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/retrieval/test_integration_retrieval.py` & `merlin-models-23.5.0/tests/integration/tf/retrieval/test_integration_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_01_getting_started.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_02_dataschema.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_03_exploring_different_models.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_04_export_ranking_models.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_05_export_retrieval_model.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py` & `merlin-models-23.5.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/config/test_schema.py` & `merlin-models-23.5.0/tests/unit/config/test_schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/datasets/test_advertising.py` & `merlin-models-23.5.0/tests/unit/datasets/test_advertising.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/datasets/test_ecommerce.py` & `merlin-models-23.5.0/tests/unit/datasets/test_ecommerce.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/datasets/test_entertainment.py` & `merlin-models-23.5.0/tests/unit/datasets/test_entertainment.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/datasets/test_synthetic.py` & `merlin-models-23.5.0/tests/unit/datasets/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/implicit/__init__.py` & `merlin-models-23.5.0/tests/unit/torch/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import pytest
 
-pytest.importorskip("implicit")
+pytest.importorskip("torch")
```

### Comparing `merlin-models-23.4.0/tests/unit/implicit/test_implicit.py` & `merlin-models-23.5.0/tests/unit/implicit/test_implicit.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/lightfm/__init__.py` & `merlin-models-23.5.0/tests/unit/lightfm/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/lightfm/test_lightfm.py` & `merlin-models-23.5.0/tests/unit/lightfm/test_lightfm.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/_conftest.py` & `merlin-models-23.5.0/tests/unit/tf/_conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_base.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_two_tower.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_two_tower.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_cross_batch.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_in_batch.py` & `merlin-models-23.5.0/tests/unit/tf/test_public_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import tensorflow as tf
 
-from merlin.models.tf.blocks.sampling.in_batch import InBatchSampler
+import pytest
 
+import merlin.models.tf as ml
 
-def test_in_batch_sampler_reload():
-    batch_size = 43
-    sampler = InBatchSampler(batch_size=batch_size)
-    serialized = tf.keras.layers.serialize(sampler)
-    reloaded = tf.keras.layers.deserialize(serialized)
-    assert reloaded.batch_size == batch_size
+
+def test_tf_import():
+    pytest.importorskip("tensorflow")
+
+    assert ml is not None
+    assert ml.Model is not None
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/test_cross.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/test_cross.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/test_dlrm.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/test_dlrm.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,73 +10,75 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import numpy as np
 import pytest
 
 import merlin.models.tf as mm
+from merlin.dataloader.ops.embeddings import EmbeddingOperator
 from merlin.io import Dataset
 from merlin.schema import Tags
 
 
 def test_dlrm_block(testing_data: Dataset):
     schema = testing_data.schema
     dlrm = mm.DLRMBlock(
         schema,
         embedding_dim=64,
         bottom_block=mm.MLPBlock([64]),
         top_block=mm.DenseResidualBlock(),
     )
-    features = mm.sample_batch(testing_data, batch_size=100, include_targets=False)
+    features = mm.sample_batch(testing_data, batch_size=10, include_targets=False)
     outputs = dlrm(features)
     num_features = len(schema.select_by_tag(Tags.CATEGORICAL)) + 1
     dot_product_dim = (num_features - 1) * num_features // 2
-    assert list(outputs.shape) == [100, dot_product_dim + 64]
+    assert list(outputs.shape) == [10, dot_product_dim + 64]
 
 
 def test_dlrm_block_no_top_block(testing_data: Dataset):
     schema = testing_data.schema
     dlrm = mm.DLRMBlock(
         schema,
         embedding_dim=64,
         bottom_block=mm.MLPBlock([64]),
     )
-    outputs = dlrm(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
+    outputs = dlrm(mm.sample_batch(testing_data, batch_size=10, include_targets=False))
     num_features = len(schema.select_by_tag(Tags.CATEGORICAL)) + 1
     dot_product_dim = (num_features - 1) * num_features // 2
 
-    assert list(outputs.shape) == [100, dot_product_dim]
+    assert list(outputs.shape) == [10, dot_product_dim]
 
 
 def test_dlrm_block_no_continuous_features(testing_data: Dataset):
     schema = testing_data.schema.remove_by_tag(Tags.CONTINUOUS)
     dlrm = mm.DLRMBlock(schema, embedding_dim=64, top_block=mm.MLPBlock([32]))
-    outputs = dlrm(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
+    outputs = dlrm(mm.sample_batch(testing_data, batch_size=10, include_targets=False))
 
-    assert list(outputs.shape) == [100, 32]
+    assert list(outputs.shape) == [10, 32]
 
 
 def test_dlrm_block_no_categ_features(testing_data: Dataset):
     schema = testing_data.schema.remove_by_tag(Tags.CATEGORICAL)
     with pytest.raises(ValueError) as excinfo:
         mm.DLRMBlock(
             schema, embedding_dim=64, bottom_block=mm.MLPBlock([64]), top_block=mm.MLPBlock([16])
         )
     assert "DLRM requires categorical features" in str(excinfo.value)
 
 
 def test_dlrm_block_single_categ_feature(testing_data: Dataset):
     schema = testing_data.schema.select_by_tag([Tags.ITEM_ID])
     dlrm = mm.DLRMBlock(schema, embedding_dim=64, top_block=mm.MLPBlock([32]))
-    outputs = dlrm(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
+    outputs = dlrm(mm.sample_batch(testing_data, batch_size=10, include_targets=False))
 
-    assert list(outputs.shape) == [100, 32]
+    assert list(outputs.shape) == [10, 32]
 
 
 def test_dlrm_block_no_schema():
     with pytest.raises(ValueError) as excinfo:
         mm.DLRMBlock(
             schema=None,
             embedding_dim=64,
@@ -116,10 +118,47 @@
     top_dim = 4
     dlrm = mm.DLRMBlock(
         schema,
         embeddings=mm.Embeddings(schema.select_by_tag(Tags.CATEGORICAL), dim=embedding_dim),
         bottom_block=mm.MLPBlock([embedding_dim]),
         top_block=mm.MLPBlock([top_dim]),
     )
-    outputs = dlrm(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
+    outputs = dlrm(mm.sample_batch(testing_data, batch_size=10, include_targets=False))
 
-    assert list(outputs.shape) == [100, 4]
+    assert list(outputs.shape) == [10, 4]
+
+
+def test_dlrm_with_pretrained_embeddings(testing_data: Dataset):
+    embedding_dim = 12
+    top_dim = 4
+
+    item_cardinality = testing_data.schema["item_id"].int_domain.max + 1
+    pretrained_embedding = np.random.rand(item_cardinality, 12)
+
+    loader = mm.Loader(
+        testing_data,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                pretrained_embedding,
+                lookup_key="item_id",
+                embedding_name="pretrained_item_embeddings",
+            ),
+        ],
+    )
+    schema = loader.output_schema
+
+    embeddings = mm.Embeddings(schema.select_by_tag(Tags.CATEGORICAL), dim=embedding_dim)
+    pretrained_embeddings = mm.PretrainedEmbeddings(
+        schema.select_by_tag(Tags.EMBEDDING),
+        output_dims=embedding_dim,
+    )
+
+    dlrm = mm.DLRMBlock(
+        schema,
+        embeddings=mm.ParallelBlock(embeddings, pretrained_embeddings),
+        bottom_block=mm.MLPBlock([embedding_dim]),
+        top_block=mm.MLPBlock([top_dim]),
+    )
+    outputs = dlrm(mm.sample_batch(loader, include_targets=False))
+
+    assert list(outputs.shape) == [10, 4]
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/test_interactions.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/test_interactions.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/test_mlp.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/test_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         model, loader, run_eagerly=run_eagerly, reload_model=True, fit_kwargs={"pre": predict_last}
     )
 
     metrics = model.evaluate(loader, steps=1, return_dict=True, pre=predict_last)
     assert len(metrics) > 0
 
     predictions = model.predict(loader, steps=1)
-    assert predictions.shape == (8, 51997)
+    assert predictions.shape == (8, 101)
 
 
 @pytest.mark.parametrize("no_activation_last_layer", [False, True])
 @pytest.mark.parametrize("dims", [[32], [64, 32]])
 def test_mlp_block_no_activation_last_layer(no_activation_last_layer, dims):
     mlp = ml.MLPBlock(dims, activation="relu", no_activation_last_layer=no_activation_last_layer)
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/blocks/test_optimizer.py` & `merlin-models-23.5.0/tests/unit/tf/blocks/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_aggregation.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_base.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_combinators.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_combinators.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_encoder.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_encoder.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_index.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_prediction.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,9 @@
         mm.BinaryClassificationTask("click"),
         pre=FlipTargets(),
     )
 
     features, targets = mm.sample_batch(ecommerce_data, batch_size=100)
     outputs, context = model(features, targets=targets, training=True, output_context=True)
 
-    flipped = np.logical_not(targets["click"].numpy()).astype(np.int)
+    flipped = np.logical_not(targets["click"].numpy()).astype(int)
     assert np.array_equal(context.targets["click"], flipped)
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/core/test_tabular.py` & `merlin-models-23.5.0/tests/unit/tf/core/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_01_getting_started.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_02_dataschema.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_03_exploring_different_models.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_04_export_ranking_models.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_05_export_retrieval_model.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_07_train_traditional_models.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_07_train_traditional_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py` & `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import shutil
 
 import pytest
 from testbook import testbook
 
-from merlin.systems.triton.utils import run_triton_server
 from tests.conftest import REPO_ROOT
 
 pytest.importorskip("transformers")
+utils = pytest.importorskip("merlin.systems.triton.utils")
 
 TRITON_SERVER_PATH = shutil.which("tritonserver")
 
 
 @pytest.mark.skipif(not TRITON_SERVER_PATH, reason="triton server not found")
 @testbook(
     REPO_ROOT / "examples/usecases/transformers-next-item-prediction.ipynb",
     timeout=720,
     execute=False,
 )
 @pytest.mark.notebook
-def test_next_item_prediction(tb):
+def test_next_item_prediction(tb, tmpdir):
     tb.inject(
-        """
+        f"""
         import os, random
         from datetime import datetime, timedelta
         from merlin.datasets.synthetic import generate_data
         ds = generate_data('booking.com-raw', 10000)
         df = ds.compute()
         def generate_date():
             date = datetime.today()
             if random.randint(0, 1):
                 date -= timedelta(days=7)
             return date
         df['checkin'] = [generate_date() for _ in range(df.shape[0])]
         df['checkout'] = [generate_date() for _ in range(df.shape[0])]
-        df.to_csv('/tmp/train_set.csv')
+        df.to_csv('{tmpdir}/train_set.csv')
         """
     )
     tb.cells[4].source = tb.cells[4].source.replace("get_booking('/workspace/data')", "")
     tb.cells[4].source = tb.cells[4].source.replace(
-        "read_csv('/workspace/data/train_set.csv'", "read_csv('/tmp/train_set.csv'"
+        "read_csv('/workspace/data/train_set.csv'", f"read_csv('{tmpdir}/train_set.csv'"
     )
     tb.cells[31].source = tb.cells[31].source.replace("epochs=5", "epochs=1")
-    tb.cells[37].source = tb.cells[37].source.replace("/workspace/ensemble", "/tmp/ensemble")
+    tb.cells[37].source = tb.cells[37].source.replace("/workspace/ensemble", f"{tmpdir}/ensemble")
     tb.execute_cell(list(range(0, 38)))
 
-    with run_triton_server("/tmp/ensemble", grpc_port=8001):
+    with utils.run_triton_server(f"{tmpdir}/ensemble", grpc_port=8001):
         tb.execute_cell(list(range(38, len(tb.cells))))
+
+    tb.inject(
+        """
+        logits_count = predictions.shape[1]
+        """
+    )
+    tb.execute_cell(len(tb.cells) - 1)
+
+    cardinality = tb.ref("cardinality")
+    logits_count = tb.ref("logits_count")
+    assert logits_count == cardinality
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/experimental/__init__.py` & `merlin-models-23.5.0/merlin/models/torch/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/experimental/test_sample_weight.py` & `merlin-models-23.5.0/tests/unit/tf/experimental/test_sample_weight.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/horovod/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/horovod/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/horovod/test_embedding.py` & `merlin-models-23.5.0/tests/unit/tf/horovod/test_embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/horovod/test_horovod.py` & `merlin-models-23.5.0/tests/unit/tf/horovod/test_horovod.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/__init__.py` & `merlin-models-23.5.0/tests/unit/xgb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+import pytest
+
+pytest.importorskip("xgboost")
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/test_base.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/test_block.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/test_block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/test_continuous.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/test_continuous.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/test_embedding.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/test_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
     dim = 16
     embeddings_wo_reg = mm.Embeddings(schema, dim=dim)
     embeddings_batch_reg = mm.Embeddings(schema, dim=dim, l2_batch_regularization_factor=0.2)
     embeddings_table_reg = mm.Embeddings(
         schema, dim=dim, embeddings_regularizer=tf.keras.regularizers.L2(0.2)
     )
 
-    inputs = mm.sample_batch(testing_data, batch_size=100, include_targets=False)
+    inputs = mm.sample_batch(testing_data, batch_size=20, include_targets=False)
     _ = embeddings_wo_reg(inputs)
     _ = embeddings_batch_reg(inputs)
     _ = embeddings_table_reg(inputs)
 
     assert not embeddings_wo_reg.losses
     assert embeddings_batch_reg.losses[0] > 0
     tf.debugging.assert_greater(embeddings_table_reg.losses[0], embeddings_batch_reg.losses[0])
@@ -493,30 +493,30 @@
     )
 
     embeddings = emb_module(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
 
     assert (
         emb_module.embedding_tables["user_id"].embeddings.shape[1]
         == embeddings["user_id"].shape[1]
-        == 20
+        == 10
     )
     assert (
         emb_module.embedding_tables["user_country"].embeddings.shape[1]
         == embeddings["user_country"].shape[1]
         == 9
     )
     assert (
         emb_module.embedding_tables["item_id"].embeddings.shape[1]
         == embeddings["item_id"].shape[1]
-        == 46
+        == 10
     )
     assert (
         emb_module.embedding_tables["categories"].embeddings.shape[1]
         == embeddings["categories"].shape[1]
-        == 13
+        == 9
     )
 
 
 def test_embedding_features_yoochoose_infer_embedding_sizes_multiple_8(testing_data: Dataset):
     schema = testing_data.schema.select_by_tag(Tags.CATEGORICAL)
 
     emb_module = mm.EmbeddingFeatures.from_schema(
@@ -529,25 +529,25 @@
     )
 
     embeddings = emb_module(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
 
     assert (
         emb_module.embedding_tables["user_id"].embeddings.shape[1]
         == embeddings["user_id"].shape[1]
-        == 24
+        == 16
     )
     assert (
         emb_module.embedding_tables["user_country"].embeddings.shape[1]
         == embeddings["user_country"].shape[1]
         == 16
     )
     assert (
         emb_module.embedding_tables["item_id"].embeddings.shape[1]
         == embeddings["item_id"].shape[1]
-        == 48
+        == 16
     )
     assert (
         emb_module.embedding_tables["categories"].embeddings.shape[1]
         == embeddings["categories"].shape[1]
         == 16
     )
 
@@ -575,20 +575,20 @@
         emb_module.embedding_tables["user_country"].embeddings.shape[1]
         == embeddings["user_country"].shape[1]
         == 100
     )
     assert (
         emb_module.embedding_tables["item_id"].embeddings.shape[1]
         == embeddings["item_id"].shape[1]
-        == 46
+        == 10
     )
     assert (
         emb_module.embedding_tables["categories"].embeddings.shape[1]
         == embeddings["categories"].shape[1]
-        == 13
+        == 9
     )
 
 
 def test_embedding_features_yoochoose_custom_initializers(testing_data: Dataset):
     schema = testing_data.schema.select_by_tag(Tags.CATEGORICAL)
 
     random_max_abs_value = 0.3
@@ -628,16 +628,16 @@
         default_truncated_normal_std, abs=0.04
     )
 
 
 def test_embedding_features_yoochoose_pretrained_initializer(testing_data: Dataset):
     schema = testing_data.schema.select_by_tag(Tags.CATEGORICAL)
 
-    pretrained_emb_item_ids = np.random.random((51997, 64))
-    pretrained_emb_categories = np.random.random((332, 64))
+    pretrained_emb_item_ids = np.random.random((101, 64))
+    pretrained_emb_categories = np.random.random((71, 64))
 
     emb_module = mm.EmbeddingFeatures.from_schema(
         schema,
         embedding_options=mm.EmbeddingOptions(
             embeddings_initializers={
                 "item_id": mm.TensorInitializer(pretrained_emb_item_ids),
                 "categories": mm.TensorInitializer(pretrained_emb_categories),
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/inputs/test_tabular.py` & `merlin-models-23.5.0/tests/unit/tf/inputs/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/layers/test_queue.py` & `merlin-models-23.5.0/tests/unit/tf/layers/test_queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/losses/__init__.py` & `merlin-models-23.5.0/tests/unit/tf/transformers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import pytest
+
+pytest.importorskip("transformers")
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/losses/test_losses.py` & `merlin-models-23.5.0/tests/unit/tf/losses/test_losses.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_popularity.py` & `merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 import tensorflow as tf
+from tensorflow.keras.losses import binary_crossentropy
 
-from merlin.models.tf.metrics.evaluation import ItemCoverageAt, NoveltyAt, PopularityBiasAt
+from merlin.models.tf.metrics import metrics_registry
+from merlin.models.tf.metrics.evaluation import (
+    ItemCoverageAt,
+    LogLossMetric,
+    NoveltyAt,
+    PopularityBiasAt,
+)
+
+
+@pytest.mark.parametrize("metric", [LogLossMetric(), "logloss"])
+def test_logloss_metric(metric):
+    metric = metrics_registry.parse(metric)
+
+    y_pred = tf.convert_to_tensor([1.0, 0.5, 0.2, 2.3, 5.0], tf.float32)
+    y_true = tf.convert_to_tensor([0, 1, 0, 0, 1], tf.int32)
+
+    expected_result = binary_crossentropy(y_true, y_pred, from_logits=False)
+
+    metric.update_state(y_true, y_pred)
+    result = metric.result()
+
+    tf.debugging.assert_near(result, expected_result)
 
 
 @pytest.fixture
 def popularity_metrics_test_data():
     labels = tf.convert_to_tensor([[1], [3], [7], [6]], tf.int64)
     predictions = tf.convert_to_tensor(
         [[1, 9, 8, 7, 6], [1, 4, 3, 2, 5], [5, 9, 8, 7, 6]], tf.int64
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_topk.py` & `merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics_topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/models/test_base.py` & `merlin-models-23.5.0/tests/unit/tf/models/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/models/test_benchmark.py` & `merlin-models-23.5.0/tests/unit/tf/models/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/models/test_ranking.py` & `merlin-models-23.5.0/tests/unit/tf/models/test_ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #
 import numpy as np
 import pytest
 import tensorflow as tf
 from tensorflow.keras import regularizers
 
 import merlin.models.tf as mm
+from merlin.dataloader.ops.embeddings import EmbeddingOperator
 from merlin.datasets.synthetic import generate_data
 from merlin.io import Dataset
 from merlin.models.tf.transforms.features import expected_input_cols_from_schema
 from merlin.models.tf.utils import testing_utils
 from merlin.schema import Tags
 
 
@@ -161,14 +162,55 @@
         prediction_tasks=mm.BinaryOutput("click"),
     )
 
     testing_utils.model_test(model, music_streaming_data, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
+def test_dcn_model_with_pretrained_embeddings(music_streaming_data: Dataset, run_eagerly):
+    music_streaming_data.schema = music_streaming_data.schema.select_by_name(
+        ["item_id", "item_category", "user_age", "click"]
+    )
+
+    cardinality = music_streaming_data.schema["item_category"].int_domain.max + 1
+    pretrained_embedding = np.random.rand(cardinality, 12)
+
+    loader = mm.Loader(
+        music_streaming_data,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                pretrained_embedding,
+                lookup_key="item_category",
+                embedding_name="pretrained_category_embeddings",
+            ),
+        ],
+    )
+    schema = loader.output_schema
+
+    pretrained_embeddings = mm.PretrainedEmbeddings(
+        schema.select_by_tag(Tags.EMBEDDING),
+        output_dims=16,
+    )
+
+    input_block = mm.InputBlockV2(schema, pretrained_embeddings=pretrained_embeddings)
+
+    model = mm.DCNModel(
+        schema,
+        input_block=input_block,
+        depth=1,
+        deep_block=mm.MLPBlock([2]),
+        stacked=True,
+        prediction_tasks=mm.BinaryOutput("click"),
+    )
+
+    testing_utils.model_test(model, loader, run_eagerly=run_eagerly)
+
+
+@pytest.mark.parametrize("run_eagerly", [True, False])
 def test_deepfm_model_only_categ_feats(music_streaming_data, run_eagerly):
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(
         ["item_id", "item_category", "user_id", "click"]
     )
     model = mm.DeepFMModel(
         music_streaming_data.schema,
         embedding_dim=16,
@@ -462,16 +504,16 @@
 
     testing_utils.model_test(model, ecommerce_data, run_eagerly=True)
 
     wide_model = model.blocks[0].parallel_layers["wide"]
     deep_model = model.blocks[0].parallel_layers["deep"]
 
     multi_optimizer = mm.MultiOptimizer(
-        default_optimizer="adagrad",
+        default_optimizer=tf.keras.optimizers.legacy.Adagrad(learning_rate=0.001),
         optimizers_and_blocks=[
             mm.OptimizerBlocks("ftrl", wide_model),
-            mm.OptimizerBlocks("adagrad", deep_model),
+            mm.OptimizerBlocks(tf.keras.optimizers.legacy.Adagrad(learning_rate=0.001), deep_model),
         ],
     )
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizer
     )
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/models/test_retrieval.py` & `merlin-models-23.5.0/tests/unit/tf/models/test_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -864,15 +864,15 @@
     sequence_testing_data.schema = sequence_testing_data.schema.excluding_by_name(to_remove)
 
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
     target = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID).column_names[0]
     target_augmentation = target_augmentation(schema=seq_schema, target=target)
 
     model = mm.YoutubeDNNRetrievalModelV2(
-        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([32]), num_sampled=1000
+        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([8]), num_sampled=10
     )
 
     dataloader = mm.Loader(sequence_testing_data, batch_size=50)
 
     _, losses = testing_utils.model_test(
         model,
         dataloader,
@@ -948,25 +948,25 @@
     sequence_testing_data.schema = sequence_testing_data.schema.excluding_by_name(to_remove)
 
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
     target = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID).column_names[0]
     predict_next = mm.SequencePredictLast(schema=seq_schema, target=target)
 
     model = mm.YoutubeDNNRetrievalModelV2(
-        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([32]), num_sampled=1000
+        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([8]), num_sampled=10
     )
 
     dataloader = mm.Loader(sequence_testing_data, batch_size=50)
     model, _ = testing_utils.model_test(
         model, dataloader, reload_model=False, fit_kwargs=dict(pre=predict_next)
     )
 
     candidates = model.candidate_embeddings().compute()
-    assert list(candidates.columns) == [str(i) for i in range(32)]
-    assert len(candidates.index) == 51997
+    assert list(candidates.columns) == [str(i) for i in range(8)]
+    assert len(candidates.index) == 101
 
     # Export the query embeddings is raising an error from dask, related to
     # the support of multi-hot input features.
 
     # queries = model.query_embeddings(
     #    sequence_testing_data, batch_size=10, index=Tags.USER_ID
     # ).compute()
@@ -983,15 +983,15 @@
     sequence_testing_data.schema = sequence_testing_data.schema.excluding_by_name(to_remove)
 
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
     target = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID).column_names[0]
     predict_next = mm.SequencePredictLast(schema=seq_schema, target=target)
 
     model = mm.YoutubeDNNRetrievalModelV2(
-        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([32]), num_sampled=1000
+        schema=sequence_testing_data.schema, top_block=mm.MLPBlock([8]), num_sampled=10
     )
 
     dataloader = mm.Loader(sequence_testing_data, batch_size=50)
 
     model, _ = testing_utils.model_test(
         model, dataloader, reload_model=False, fit_kwargs=dict(pre=predict_next)
     )
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_base.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_block.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_classification.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,11 +112,11 @@
         embeddings["item_id_seq"],
         EmbeddingTablePrediction(embeddings["item_id_seq"]),
     ]
 
     for target in predictions:
         model = mm.Model(
             mm.InputBlockV2(schema, categorical=embeddings),
-            mm.MLPBlock([32]),
+            mm.MLPBlock([8]),
             mm.CategoricalOutput(target),
         )
         testing_utils.model_test(model, dataloader, run_eagerly=run_eagerly)
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_contrastive.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_contrastive.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,22 +140,22 @@
     model.compile(optimizer="adam")
 
     batch = next(iter(dataloader))
     output = model(batch[0], batch[1], training=True)
     assert output[1].shape == (batch[1].shape[0], 51)
 
     model_out.set_negative_samplers(
-        [PopularityBasedSamplerV2(max_id=51996, max_num_samples=20)],
+        [PopularityBasedSamplerV2(max_id=100, max_num_samples=20)],
     )
 
     output = model(batch[0], batch[1], training=True)
     assert output.outputs.shape == (batch[1].shape[0], 21)
 
     model_out.set_negative_samplers(
-        ["in-batch", PopularityBasedSamplerV2(max_id=51996, max_num_samples=20)],
+        ["in-batch", PopularityBasedSamplerV2(max_id=100, max_num_samples=20)],
     )
     output = model(batch[0], batch[1], training=True)
     assert output.outputs.shape == (batch[1].shape[0], 71)
 
 
 def test_contrastive_output_without_sampler(ecommerce_data: Dataset):
     with pytest.raises(Exception) as excinfo:
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_regression.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_sampling.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/outputs/test_topk.py` & `merlin-models-23.5.0/tests/unit/tf/outputs/test_topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_classification.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_multi_task.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_multi_task.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_next_item.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_next_item.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_regression.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_retrieval.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_sampling.py` & `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/test_core.py` & `merlin-models-23.5.0/tests/unit/tf/test_core.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/test_loader.py` & `merlin-models-23.5.0/tests/unit/tf/test_loader.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transformers/test_block.py` & `merlin-models-23.5.0/tests/unit/tf/transformers/test_block.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pytest
 import tensorflow as tf
 from tensorflow.keras.utils import set_random_seed
 from transformers import BertConfig
 
 import merlin.models.tf as mm
+from merlin.dataloader.ops.embeddings import EmbeddingOperator
 from merlin.io import Dataset
 from merlin.models.tf.loader import Loader
 from merlin.models.tf.transformers.block import (
     AlbertBlock,
     BertBlock,
     GPT2Block,
     RobertaBlock,
@@ -66,25 +67,25 @@
         run_eagerly=run_eagerly,
         reload_model=False,
         metrics={},
         fit_kwargs={"pre": predict_last},
     )
 
     predictions = model.predict(loader)
-    assert list(predictions.shape) == [100, 51997]
+    assert list(predictions.shape) == [100, 101]
 
     query_embeddings = query_encoder.predict(loader)
     assert list(query_embeddings.shape) == [100, d_model]
 
     item_embeddings = model.candidate_embeddings().compute().to_numpy()
 
-    assert list(item_embeddings.shape) == [51997, d_model]
+    assert list(item_embeddings.shape) == [101, d_model]
     predicitons_2 = np.dot(query_embeddings, item_embeddings.T)
 
-    np.testing.assert_allclose(predictions, predicitons_2, atol=1e-6)
+    np.testing.assert_allclose(predictions, predicitons_2, atol=1e-3)
 
 
 def test_transformer_encoder():
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
 
@@ -164,14 +165,15 @@
     loader, schema = classification_loader(sequence_testing_data)
 
     model = mm.Model(
         mm.InputBlockV2(
             schema,
             categorical=mm.Embeddings(schema, sequence_combiner=None),
         ),
+        mm.MLPBlock([EMBED_DIM]),
         BertBlock(
             d_model=EMBED_DIM,
             n_head=8,
             n_layer=2,
             transformer_post="pooler_output",
         ),
         mm.CategoricalOutput(
@@ -182,15 +184,15 @@
     batch = loader.peek()[0]
 
     outputs = model(batch)
     assert list(outputs.shape) == [64, 63]
     testing_utils.model_test(model, loader, run_eagerly=run_eagerly)
 
 
-def test_tranformer_with_prepare_module(sequence_testing_data):
+def test_tranformer_with_prepare_module():
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
     inputs = tf.random.uniform((NUM_ROWS, SEQ_LENGTH, EMBED_DIM))
 
     class DummyPrepare(tf.keras.layers.Layer):
         def __init__(self, transformer, **kwargs):
@@ -305,21 +307,21 @@
 
     testing_utils.model_test(
         model, loader, run_eagerly=run_eagerly, reload_model=True, fit_kwargs={"pre": predict_next}
     )
 
     batch = next(iter(loader))[0]
     outputs = model(batch)
-    assert list(outputs.shape) == [8, 51997]
+    assert list(outputs.shape) == [8, 101]
 
     metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=predict_next)
     assert len(metrics) > 0
 
     predictions = model.predict(loader, batch_size=8, steps=1)
-    assert predictions.shape == (8, 51997)
+    assert predictions.shape == (8, 101)
 
     predict_last = mm.SequencePredictLast(
         schema=seq_schema, target=target, transformer=transformer_block
     )
     metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=predict_last)
     assert len(metrics) > 0
 
@@ -354,15 +356,15 @@
     seq_mask_random = mm.SequenceMaskRandom(
         schema=seq_schema, target=target, masking_prob=0.3, transformer=transformer_block
     )
 
     inputs, targets = loader.peek()
 
     outputs = model(inputs, targets=targets, training=True)
-    assert list(outputs.shape) == [8, 4, 51997]
+    assert list(outputs.shape) == [8, 4, 101]
     testing_utils.model_test(
         model,
         loader,
         run_eagerly=run_eagerly,
         reload_model=True,
         fit_kwargs={"pre": seq_mask_random},
     )
@@ -371,15 +373,15 @@
         schema=seq_schema, target=target, transformer=transformer_block
     )
     metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=seq_mask_last)
     assert len(metrics) > 0
 
     # Get predictions for next-item position
     predictions = model.predict(loader, batch_size=8, steps=1)
-    assert predictions.shape == (8, 51997)
+    assert predictions.shape == (8, 101)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_transformer_with_masked_language_modeling_check_eval_masked(
     sequence_testing_data: Dataset, run_eagerly
 ):
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
@@ -413,20 +415,20 @@
 
     testing_utils.model_test(
         model,
         loader,
         run_eagerly=run_eagerly,
         reload_model=True,
         fit_kwargs={"pre": seq_mask_random},
-        metrics=[mm.RecallAt(5000), mm.NDCGAt(5000, seed=4)],
+        metrics=[mm.RecallAt(50), mm.NDCGAt(50, seed=4)],
     )
 
     inputs = itertools.islice(iter(loader), 1)
     outputs = model.predict(inputs, pre=seq_mask_random)
-    assert list(outputs.shape) == [8, 51997]
+    assert list(outputs.shape) == [8, 101]
 
     # This transform only extracts targets, but without applying mask
     seq_target_as_input_no_mask = mm.SequenceTargetAsInput(schema=seq_schema, target=target)
 
     with Loader(sequence_testing_data, batch_size=8, shuffle=False) as loader:
         metrics_all_positions1 = model.evaluate(
             loader, batch_size=8, steps=1, return_dict=True, pre=seq_target_as_input_no_mask
@@ -466,35 +468,37 @@
     seq_schema = schema.select_by_name(["item_id_seq", "categories", "item_age_days_norm"])
     context_schema = schema.select_by_name(["user_country", "user_age"])
     sequence_testing_data.schema = seq_schema + context_schema
 
     target = schema.select_by_tag(Tags.ITEM_ID).column_names[0]
     item_id_name = schema.select_by_tag(Tags.ITEM_ID).first.properties["domain"]["name"]
 
+    item_id_emb_dim = 16
     input_block = mm.InputBlockV2(
         sequence_testing_data.schema,
         embeddings=mm.Embeddings(
             seq_schema.select_by_tag(Tags.CATEGORICAL)
             + context_schema.select_by_tag(Tags.CATEGORICAL),
             sequence_combiner=None,
+            dim={"item_id_seq": item_id_emb_dim},
         ),
         post=mm.BroadcastToSequence(context_schema, seq_schema),
     )
 
     dmodel = 32
     mlp_block = mm.MLPBlock([128, dmodel], activation="relu")
     transformer_block = mm.GPT2Block(
         d_model=dmodel,
         n_head=4,
         n_layer=2,
     )
 
     dense_block = mm.SequentialBlock(input_block, mlp_block, transformer_block)
 
-    mlp_block2 = mm.MLPBlock([128, dmodel], activation="relu")
+    mlp_block2 = mm.MLPBlock([128, item_id_emb_dim], activation="relu")
 
     prediction_task = mm.CategoricalOutput(
         to_call=input_block["categorical"][item_id_name],
     )
     model = mm.Model(dense_block, mlp_block2, prediction_task)
 
     fit_pre = mm.SequenceMaskRandom(
@@ -503,7 +507,231 @@
     testing_utils.model_test(
         model,
         sequence_testing_data,
         run_eagerly=run_eagerly,
         reload_model=False,
         fit_kwargs={"pre": fit_pre},
     )
+
+
+@pytest.mark.parametrize("pre", [mm.SequenceMaskRandom, mm.SequencePredictNext])
+def test_transformer_encoder_with_contrastive_output(sequence_testing_data: Dataset, pre):
+    dmodel = 32
+    seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
+    target_schema = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID)
+    model_schema = seq_schema + target_schema
+    target = target_schema.column_names[0]
+
+    input_block = mm.InputBlockV2(
+        model_schema,
+        categorical=mm.Embeddings(
+            model_schema.select_by_tag(Tags.CATEGORICAL), dim=dmodel, sequence_combiner=None
+        ),
+    )
+    transformer_block = XLNetBlock(d_model=dmodel, n_head=4, n_layer=1)
+    session_encoder = mm.Encoder(
+        input_block,
+        mm.MLPBlock([dmodel]),
+        transformer_block,
+    )
+    output_block = mm.ContrastiveOutput(
+        to_call=target_schema,
+        negative_samplers=mm.PopularityBasedSamplerV2(
+            max_num_samples=10,
+            max_id=100,
+            min_id=1,
+        ),
+        logq_sampling_correction=True,
+    )
+    model = mm.RetrievalModelV2(query=session_encoder, output=output_block)
+
+    sequence_testing_data.schema = model_schema
+    loader = Loader(sequence_testing_data, batch_size=64, shuffle=False)
+
+    fit_pre = pre(schema=seq_schema, target=target, transformer=transformer_block)
+    model.compile()
+    _ = model.fit(loader, pre=fit_pre)
+
+    inputs, _ = loader.peek()
+    predictions = model(inputs)
+    assert list(predictions.shape) == [64, 101]
+
+
+@pytest.mark.parametrize("run_eagerly", [True, False])
+def test_transformer_model_with_masking_broadcast_and_pretrained_emb(
+    sequence_testing_data, run_eagerly: bool
+):
+    sequence_testing_data.schema = sequence_testing_data.schema.select_by_name(
+        [
+            "item_id_seq",
+            "categories",
+            "item_age_days_norm",
+            "test_user_id",
+            "user_country",
+            "user_age",
+        ]
+    )
+
+    item_cardinality = sequence_testing_data.schema["item_id_seq"].int_domain.max + 1
+    user_cardinality = sequence_testing_data.schema["test_user_id"].int_domain.max + 1
+
+    loader = mm.Loader(
+        sequence_testing_data,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np.random.rand(user_cardinality, 12),
+                lookup_key="test_user_id",
+                embedding_name="pretrained_user_id_embeddings",
+            ),
+            EmbeddingOperator(
+                np.random.rand(item_cardinality, 16),
+                lookup_key="item_id_seq",
+                embedding_name="pretrained_item_id_embeddings",
+            ),
+        ],
+    )
+
+    schema = loader.output_schema
+    seq_schema = schema.select_by_name(
+        ["item_id_seq", "categories", "item_age_days_norm", "pretrained_item_id_embeddings"]
+    )
+    context_schema = schema.select_by_name(
+        ["test_user_id", "user_country", "user_age", "pretrained_user_id_embeddings"]
+    )
+
+    item_id_name = schema.select_by_tag(Tags.ITEM_ID).column_names[0]
+    item_id_embedding_dim = 16
+
+    input_block = mm.InputBlockV2(
+        schema,
+        embeddings=mm.Embeddings(
+            seq_schema.select_by_tag(Tags.CATEGORICAL)
+            + context_schema.select_by_tag(Tags.CATEGORICAL),
+            dim={"item_id_seq": item_id_embedding_dim},
+            sequence_combiner=None,
+        ),
+        pretrained_embeddings=mm.PretrainedEmbeddings(
+            schema.select_by_tag(Tags.EMBEDDING),
+            sequence_combiner=None,
+        ),
+        post=mm.BroadcastToSequence(context_schema, seq_schema),
+    )
+
+    dmodel = 32
+    mlp_block = mm.MLPBlock([128, dmodel], activation="relu")
+    transformer_block = mm.GPT2Block(
+        d_model=dmodel,
+        n_head=4,
+        n_layer=2,
+    )
+
+    dense_block = mm.SequentialBlock(input_block, mlp_block, transformer_block)
+
+    mlp_block2 = mm.MLPBlock([64, item_id_embedding_dim], activation="relu")
+
+    prediction_task = mm.CategoricalOutput(
+        to_call=input_block["categorical"][item_id_name],
+    )
+    model = mm.Model(dense_block, mlp_block2, prediction_task)
+
+    fit_pre = mm.SequenceMaskRandom(
+        schema=seq_schema, target=item_id_name, masking_prob=0.3, transformer=transformer_block
+    )
+    testing_utils.model_test(
+        model,
+        loader,
+        run_eagerly=run_eagerly,
+        reload_model=False,
+        fit_kwargs={"pre": fit_pre},
+    )
+
+
+@pytest.mark.parametrize("run_eagerly", [True, False])
+def test_transformer_model_with_causal_language_modeling_and_pretrained_emb(
+    sequence_testing_data, run_eagerly: bool
+):
+    sequence_testing_data.schema = sequence_testing_data.schema.select_by_name(
+        [
+            "item_id_seq",
+            "categories",
+            "item_age_days_norm",
+            "test_user_id",
+            "user_country",
+            "user_age",
+        ]
+    )
+
+    item_cardinality = sequence_testing_data.schema["item_id_seq"].int_domain.max + 1
+    user_cardinality = sequence_testing_data.schema["test_user_id"].int_domain.max + 1
+
+    loader = mm.Loader(
+        sequence_testing_data,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np.random.rand(user_cardinality, 12),
+                lookup_key="test_user_id",
+                embedding_name="pretrained_user_id_embeddings",
+            ),
+            EmbeddingOperator(
+                np.random.rand(item_cardinality, 16),
+                lookup_key="item_id_seq",
+                embedding_name="pretrained_item_id_embeddings",
+            ),
+        ],
+    )
+
+    schema = loader.output_schema
+    seq_schema = schema.select_by_name(
+        ["item_id_seq", "categories", "item_age_days_norm", "pretrained_item_id_embeddings"]
+    )
+    context_schema = schema.select_by_name(
+        ["test_user_id", "user_country", "user_age", "pretrained_user_id_embeddings"]
+    )
+
+    item_id_name = schema.select_by_tag(Tags.ITEM_ID).column_names[0]
+    item_id_embedding_dim = 16
+
+    input_block = mm.InputBlockV2(
+        schema,
+        embeddings=mm.Embeddings(
+            seq_schema.select_by_tag(Tags.CATEGORICAL)
+            + context_schema.select_by_tag(Tags.CATEGORICAL),
+            dim={"item_id_seq": item_id_embedding_dim},
+            sequence_combiner=None,
+        ),
+        pretrained_embeddings=mm.PretrainedEmbeddings(
+            schema.select_by_tag(Tags.EMBEDDING),
+            sequence_combiner=None,
+        ),
+        post=mm.BroadcastToSequence(context_schema, seq_schema),
+    )
+
+    dmodel = 32
+    mlp_block = mm.MLPBlock([128, dmodel], activation="relu")
+    transformer_block = mm.GPT2Block(
+        d_model=dmodel,
+        n_head=4,
+        n_layer=2,
+    )
+
+    dense_block = mm.SequentialBlock(input_block, mlp_block, transformer_block)
+
+    mlp_block2 = mm.MLPBlock([64, item_id_embedding_dim], activation="relu")
+
+    prediction_task = mm.CategoricalOutput(
+        to_call=input_block["categorical"][item_id_name],
+    )
+    model = mm.Model(dense_block, mlp_block2, prediction_task)
+
+    predict_next = mm.SequencePredictNext(
+        schema=seq_schema, target=item_id_name, transformer=transformer_block
+    )
+
+    testing_utils.model_test(
+        model,
+        loader,
+        run_eagerly=run_eagerly,
+        reload_model=False,
+        fit_kwargs={"pre": predict_next},
+    )
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/transformers/test_transforms.py` & `merlin-models-23.5.0/tests/unit/tf/transformers/test_transforms.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_bias.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_bias.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_features.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_features.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 import tensorflow as tf
 from tensorflow.test import TestCase
 
 import merlin.models.tf as mm
+from merlin.dataloader.ops.embeddings import EmbeddingOperator
 from merlin.io import Dataset
 from merlin.models.tf.transforms.features import BroadcastToSequence, ContinuousPowers
 from merlin.models.tf.utils import testing_utils
 from merlin.models.utils.schema_utils import create_categorical_column
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
@@ -876,15 +877,15 @@
     assert set(input_batch.keys()) == set(
         ["item_id_seq", "categories", "item_age_days_norm", "user_age", "user_country"]
     )
     assert set([len(v.shape) for v in input_batch.values()]) == set([3])
     assert set([tuple(list(v.shape)[:-1]) for v in input_batch.values()]) == set(
         [tuple([100, None])]
     )
-    assert list(input_batch["item_id_seq"].shape) == [100, None, 32]
+    assert list(input_batch["item_id_seq"].shape) == [100, None, 8]
     assert list(input_batch["categories"].shape) == [100, None, 16]
     assert list(input_batch["item_age_days_norm"].shape) == [100, None, 1]
     assert list(input_batch["user_age"].shape) == [100, None, 1]
     assert list(input_batch["user_country"].shape) == [100, None, 8]
 
 
 @pytest.mark.parametrize(
@@ -1035,7 +1036,417 @@
             ColumnSchema("b", tags=[Tags.USER, Tags.CATEGORICAL]),
             ColumnSchema("label", tags=[Tags.CATEGORICAL]),
         ]
     )
     to_target = mm.ToTarget(schema, "label")
     output_schema = to_target.compute_output_schema(schema)
     assert "label" in output_schema.select_by_tag(Tags.TARGET).column_names
+
+
+def test_loader_with_pretrained_embeddings_2d():
+    from merlin.dtypes.shape import Shape
+
+    MAX_CARDINALITY = 20
+    schema = Schema(
+        [
+            ColumnSchema("user_id", tags=[Tags.USER_ID, Tags.CATEGORICAL]),
+            ColumnSchema(
+                "item_id",
+                tags=[Tags.ITEM_ID, Tags.CATEGORICAL],
+                properties={
+                    "domain": {"min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None,),
+            ),
+            ColumnSchema("item_category", tags=[Tags.ITEM, Tags.CATEGORICAL]),
+        ]
+    )
+
+    input_df = pd.DataFrame(
+        [
+            {"user_id": 1, "item_id": 2, "item_category": 3},
+            {"user_id": 2, "item_id": 3, "item_category": 2},
+        ]
+    )
+    input_df = input_df[input_df.columns]
+    dataset = Dataset(input_df, schema=schema)
+
+    np_emb_item_id = np.random.rand(MAX_CARDINALITY, 16)
+
+    loader = mm.Loader(
+        dataset,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np_emb_item_id, lookup_key="item_id", embedding_name="pretrained_item_id_embeddings"
+            ),
+        ],
+    )
+
+    assert set(loader.output_schema.column_names) == set(
+        ["user_id", "item_id", "item_category", "pretrained_item_id_embeddings"]
+    )
+    assert loader.output_schema["pretrained_item_id_embeddings"].shape == Shape((None, 16))
+
+    assert Tags.EMBEDDING in loader.output_schema["pretrained_item_id_embeddings"].tags
+    assert Tags.CATEGORICAL not in loader.output_schema["pretrained_item_id_embeddings"].tags
+    assert Tags.CONTINUOUS not in loader.output_schema["pretrained_item_id_embeddings"].tags
+
+    inputs0, _ = next(iter(loader))
+
+    assert set(inputs0.keys()) == set(list(input_df.columns) + ["pretrained_item_id_embeddings"])
+    assert inputs0["user_id"].shape == [2]
+    assert inputs0["item_id"].shape == [2]
+    assert inputs0["item_category"].shape == [2]
+    assert inputs0["pretrained_item_id_embeddings"].shape == [2, 16]
+    np.testing.assert_almost_equal(
+        inputs0["pretrained_item_id_embeddings"].numpy(), np_emb_item_id[2:4]
+    )
+
+
+def test_loader_with_pretrained_embeddings_seq_3d():
+    from merlin.dtypes.shape import Dimension
+    from merlin.schema import Tags
+
+    MAX_CARDINALITY = 20
+    schema = Schema(
+        [
+            ColumnSchema("user_id", tags=[Tags.USER_ID, Tags.CATEGORICAL], dims=(None,)),
+            ColumnSchema(
+                "item_ids",
+                tags=[Tags.ITEM_ID, Tags.CATEGORICAL],
+                properties={
+                    "domain": {"min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None, (1, 4)),
+            ),
+            ColumnSchema(
+                "item_categories", tags=[Tags.ITEM, Tags.CATEGORICAL], dims=(None, (1, 4))
+            ),
+        ]
+    )
+
+    input_df = pd.DataFrame(
+        [
+            {"user_id": 1, "item_ids": [1, 2, 3], "item_categories": [3, 4, 5]},
+            {"user_id": 2, "item_ids": [4, 5], "item_categories": [6, 7]},
+        ]
+    )
+    input_df = input_df[sorted(input_df.columns)]
+    dataset = Dataset(input_df, schema=schema)
+
+    np_emb_item_id = np.random.rand(MAX_CARDINALITY, 16)
+
+    loader = mm.Loader(
+        dataset,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np_emb_item_id,
+                lookup_key="item_ids",
+                embedding_name="pretrained_item_id_embeddings",
+            ),
+        ],
+    )
+
+    assert set(loader.output_schema.column_names) == set(
+        ["user_id", "item_ids", "item_categories", "pretrained_item_id_embeddings"]
+    )
+    assert loader.output_schema["pretrained_item_id_embeddings"].shape.dims == (
+        Dimension(min=0, max=None),
+        Dimension(min=1, max=4),
+        Dimension(min=16, max=16),
+    )
+
+    assert Tags.EMBEDDING in loader.output_schema["pretrained_item_id_embeddings"].tags
+    assert Tags.CATEGORICAL not in loader.output_schema["pretrained_item_id_embeddings"].tags
+    assert Tags.CONTINUOUS not in loader.output_schema["pretrained_item_id_embeddings"].tags
+
+    inputs0, _ = next(iter(loader))
+    assert inputs0["user_id"].shape == [2]
+    assert inputs0["item_ids__values"].shape == [5]
+    np.testing.assert_array_equal(inputs0["item_ids__offsets"], [0, 3, 5])
+    assert inputs0["item_categories__values"].shape == [5]
+    np.testing.assert_array_equal(inputs0["item_categories__offsets"], [0, 3, 5])
+    assert inputs0["pretrained_item_id_embeddings__values"].shape == [5, 16]
+    np.testing.assert_array_equal(inputs0["pretrained_item_id_embeddings__offsets"], [0, 3, 5])
+    np.testing.assert_almost_equal(
+        inputs0["pretrained_item_id_embeddings__values"].numpy(), np_emb_item_id[1:6]
+    )
+
+
+def get_loader_with_contextual_seq_pretrained_embeddings():
+    MAX_CARDINALITY = 20
+    schema = Schema(
+        [
+            # TODO: Check why dims / value_count cannot be None for scalar features
+            # otherwise EmbeddingOperator raises an error
+            ColumnSchema(
+                "user_id",
+                tags=[Tags.USER_ID],
+                dims=(None,),
+            ),
+            ColumnSchema(
+                "user_country",
+                dtype=np.int32,
+                tags=[Tags.USER, Tags.CATEGORICAL],
+                properties={
+                    "domain": {"name": "user_country", "min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None,),
+            ),
+            ColumnSchema(
+                "item_ids",
+                dtype=np.int32,
+                tags=[Tags.ITEM_ID, Tags.CATEGORICAL, Tags.SEQUENCE],
+                properties={
+                    "domain": {"name": "item_ids", "min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None, (1, 4)),
+            ),
+            ColumnSchema(
+                "item_categories",
+                dtype=np.int32,
+                tags=[Tags.ITEM, Tags.CATEGORICAL, Tags.SEQUENCE],
+                properties={
+                    "domain": {"name": "item_categories", "min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None, (1, 4)),
+            ),
+            ColumnSchema(
+                "purchase",
+                dtype=np.int32,
+                tags=[Tags.TARGET],
+                dims=(None,),
+            ),
+        ]
+    )
+
+    from merlin.models.utils.schema_utils import schema_to_tensorflow_metadata_json
+
+    schema_to_tensorflow_metadata_json(schema, "sequential_with_pretrained_embeddings.json")
+
+    input_df = pd.DataFrame(
+        [
+            {
+                "user_id": 1,
+                "user_country": 10,
+                "item_ids": [1, 2, 3],
+                "item_categories": [3, 4, 5],
+                "purchase": 1,
+            },
+            {
+                "user_id": 2,
+                "user_country": 20,
+                "item_ids": [4, 5],
+                "item_categories": [6, 7],
+                "purchase": 0,
+            },
+        ]
+    )
+    input_df = input_df[sorted(input_df.columns)]
+    dataset = Dataset(input_df, schema=schema)
+
+    np_emb_item_id = np.random.rand(MAX_CARDINALITY, 16)
+
+    loader = mm.Loader(
+        dataset,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np_emb_item_id,
+                lookup_key="user_id",
+                embedding_name="pretrained_user_id_embeddings",
+            ),
+            EmbeddingOperator(
+                np_emb_item_id,
+                lookup_key="item_ids",
+                embedding_name="pretrained_item_id_embeddings",
+            ),
+        ],
+    )
+    return loader
+
+
+@pytest.mark.parametrize(
+    "broadcast_non_seq_features",
+    [False, True],
+)
+def test_inputblock_with_pretrained_embeddings(broadcast_non_seq_features):
+    loader = get_loader_with_contextual_seq_pretrained_embeddings()
+    schema = loader.output_schema
+
+    input_kwargs = {}
+    if broadcast_non_seq_features:
+        # TODO: Check if it would be possible for EmbeddingOperator to keep the Tags.SEQUENCE
+        # in the output embedding schema if lookup_key has that tag
+        seq_schema = schema.select_by_tag(Tags.SEQUENCE) + schema.select_by_name(
+            "pretrained_item_id_embeddings"
+        )
+        non_seq_schema = schema.select_by_name(["user_country", "pretrained_user_id_embeddings"])
+        input_kwargs = {"post": mm.BroadcastToSequence(non_seq_schema, seq_schema)}
+
+    input_block = mm.InputBlockV2(
+        schema,
+        embeddings=mm.Embeddings(
+            schema.select_by_tag(Tags.CATEGORICAL),
+            sequence_combiner=None,
+        ),
+        pretrained_embeddings=mm.PretrainedEmbeddings(
+            schema.select_by_tag(Tags.EMBEDDING),
+            sequence_combiner=None,
+            normalizer="l2-norm",
+            output_dims={"pretrained_item_id_embeddings": 6},
+        ),
+        aggregation=None,
+        **input_kwargs
+    )
+
+    inputs = mm.sample_batch(loader, batch_size=10, include_targets=False, prepare_features=True)
+    input_batch = input_block(inputs)
+    assert set(input_batch.keys()) == set(
+        [
+            "user_country",
+            "item_ids",
+            "item_categories",
+            "pretrained_item_id_embeddings",
+            "pretrained_user_id_embeddings",
+        ]
+    )
+    assert list(input_batch["item_ids"].shape) == [2, None, 8]
+    assert list(input_batch["item_categories"].shape) == [2, None, 8]
+    assert list(input_batch["pretrained_item_id_embeddings"].shape) == [2, None, 6]
+    assert (
+        list(input_batch["pretrained_user_id_embeddings"].shape) == [2, None, 16]
+        if broadcast_non_seq_features
+        else [2, 16]
+    )
+
+
+@testing_utils.mark_run_eagerly_modes
+def test_model_with_pretrained_embeddings(run_eagerly: bool):
+    MAX_CARDINALITY = 20
+    schema = Schema(
+        [
+            # TODO: Check why dims / value_count cannot be None for scalar features
+            # otherwise EmbeddingOperator raises an error
+            ColumnSchema(
+                "user_id",
+                tags=[Tags.USER_ID],
+                dims=(None,),
+            ),
+            ColumnSchema(
+                "user_country",
+                dtype=np.int32,
+                tags=[Tags.USER, Tags.CATEGORICAL],
+                properties={
+                    "domain": {"name": "user_country", "min": 0, "max": MAX_CARDINALITY},
+                },
+                dims=(None,),
+            ),
+            ColumnSchema(
+                "purchase",
+                dtype=np.int32,
+                tags=[Tags.TARGET],
+                dims=(None,),
+            ),
+        ]
+    )
+
+    input_df = pd.DataFrame(
+        [
+            {
+                "user_id": 1,
+                "user_country": 10,
+                "purchase": 1,
+            },
+            {
+                "user_id": 2,
+                "user_country": 20,
+                "purchase": 0,
+            },
+        ]
+    )
+    input_df = input_df[sorted(input_df.columns)]
+    dataset = Dataset(input_df, schema=schema)
+
+    np_emb_item_id = np.random.rand(MAX_CARDINALITY, 16)
+
+    loader = mm.Loader(
+        dataset,
+        batch_size=10,
+        transforms=[
+            EmbeddingOperator(
+                np_emb_item_id,
+                lookup_key="user_id",
+                embedding_name="pretrained_user_id_embeddings",
+            ),
+        ],
+    )
+
+    schema = loader.output_schema
+
+    input_block = mm.InputBlockV2(
+        schema,
+        embeddings=mm.Embeddings(schema.select_by_tag(Tags.CATEGORICAL)),
+        pretrained_embeddings=mm.PretrainedEmbeddings(
+            schema.select_by_tag(Tags.EMBEDDING),
+            normalizer="l2-norm",
+            output_dims={"pretrained_user_id_embeddings": 6},
+        ),
+    )
+
+    model = mm.Model(
+        input_block,
+        mm.MLPBlock([4]),
+        mm.BinaryOutput("purchase"),
+    )
+
+    _, history = testing_utils.model_test(model, loader, run_eagerly=run_eagerly)
+
+    assert set(history.history.keys()) == {
+        "loss",
+        "loss_batch",
+        "precision",
+        "recall",
+        "binary_accuracy",
+        "auc",
+        "regularization_loss",
+    }
+
+
+@testing_utils.mark_run_eagerly_modes
+def test_model_with_pretrained_embeddings_seq_aggregation(run_eagerly: bool):
+    loader = get_loader_with_contextual_seq_pretrained_embeddings()
+
+    schema = loader.output_schema
+
+    input_block = mm.InputBlockV2(
+        schema,
+        embeddings=mm.Embeddings(
+            schema.select_by_tag(Tags.CATEGORICAL),
+            sequence_combiner="mean",
+        ),
+        pretrained_embeddings=mm.PretrainedEmbeddings(
+            schema.select_by_tag(Tags.EMBEDDING),
+            sequence_combiner="mean",
+            normalizer="l2-norm",
+            output_dims={"pretrained_item_id_embeddings": 6},
+        ),
+    )
+
+    model = mm.Model(
+        input_block,
+        mm.BinaryOutput("purchase"),
+    )
+
+    _, history = testing_utils.model_test(model, loader, run_eagerly=run_eagerly)
+
+    assert set(history.history.keys()) == {
+        "loss",
+        "loss_batch",
+        "precision",
+        "recall",
+        "binary_accuracy",
+        "auc",
+        "regularization_loss",
+    }
```

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_negative_sampling.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_negative_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_noise.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_noise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_sequence.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_sequence.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/transforms/test_tensor.py` & `merlin-models-23.5.0/tests/unit/tf/transforms/test_tensor.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/utils/test_batch.py` & `merlin-models-23.5.0/tests/unit/tf/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/utils/test_dataset.py` & `merlin-models-23.5.0/tests/unit/tf/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/tf/utils/test_tf_utils.py` & `merlin-models-23.5.0/tests/unit/tf/utils/test_tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/utils/test_schema_utils.py` & `merlin-models-23.5.0/tests/unit/utils/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tests/unit/xgb/test_xgboost.py` & `merlin-models-23.5.0/tests/unit/xgb/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.4.0/tox.ini` & `merlin-models-23.5.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
     pip install --upgrade pip
     pip install -e .[all]
 
 [testenv:py38-gpu]
 ; Runs in: Github Actions
 ; Runs GPU-based tests.
 deps =
-    -rrequirements/test.txt
+    --no-deps -rrequirements/test.txt
 setenv =
-    CUDA_VISIBLE_DEVICES=0
     TF_GPU_ALLOCATOR=cuda_malloc_async
 sitepackages=true
 commands =
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/systems.git@{posargs:main}
@@ -114,26 +113,28 @@
     python -m pytest Transformers4Rec-{env:GIT_COMMIT}/tests/unit
 
 [testenv:docs]
 ; Runs in: Github Actions
 ; Generates documentation with sphinx. There are other steps in the Github Actions workflow
 ; to publish the documentation on release.
 changedir = {toxinidir}
-deps = -rrequirements/docs.txt
-       {[testenv:py38-gpu]deps}
+deps =
+    -rrequirements/docs.txt
+    -rrequirements/test.txt
 commands =
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git
     python -m sphinx.cmd.build -E -P -b html docs/source docs/build/html
 
 [testenv:docs-multi]
 ; Run the multi-version build that is shown on GitHub Pages.
 changedir = {toxinidir}
-deps = -rrequirements/docs.txt
-       {[testenv:py38-gpu]deps}
+deps =
+    -rrequirements/docs.txt
+    -rrequirements/test.txt
 commands =
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git
     sphinx-multiversion --dump-metadata docs/source docs/build/html | jq "keys"
     sphinx-multiversion docs/source docs/build/html
```

### Comparing `merlin-models-23.4.0/versioneer.py` & `merlin-models-23.5.0/versioneer.py`

 * *Files identical despite different names*

