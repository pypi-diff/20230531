# Comparing `tmp/returnn-1.20230531.120344.tar.gz` & `tmp/returnn-1.20230531.135404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230531.120344.tar", last modified: Wed May 31 10:18:37 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230531.135404.tar", last modified: Wed May 31 12:11:19 2023, max compression
```

## Comparing `returnn-1.20230531.120344.tar` & `returnn-1.20230531.135404.tar`

### file list

```diff
@@ -1,445 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 10:18:36.000000 returnn-1.20230531.120344/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 10:18:18.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-31 10:18:20.000000 returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157757 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151459 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   552356 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:18:37.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-31 10:18:17.000000 returnn-1.20230531.120344/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 12:11:00.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-31 12:11:02.000000 returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157757 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   296804 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31004 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   552356 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:11:19.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-31 12:10:59.000000 returnn-1.20230531.135404/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230531.120344/.gitignore` & `returnn-1.20230531.135404/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/.gitmodules` & `returnn-1.20230531.135404/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/CHANGELOG.md` & `returnn-1.20230531.135404/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/CODEOWNERS` & `returnn-1.20230531.135404/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/CONTRIBUTING.md` & `returnn-1.20230531.135404/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/LICENSE` & `returnn-1.20230531.135404/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/MANIFEST.in` & `returnn-1.20230531.135404/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/PKG-INFO` & `returnn-1.20230531.135404/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230531.120344
+Version: 1.20230531.135404
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230531.120344/README.rst` & `returnn-1.20230531.135404/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/__init__.py` & `returnn-1.20230531.135404/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/12AX.cluster_map` & `returnn-1.20230531.135404/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-fwd.config` & `returnn-1.20230531.135404/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-horovod-mpi.py` & `returnn-1.20230531.135404/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230531.135404/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-hyper-param-tuning.config` & `returnn-1.20230531.135404/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-iter-dataset.py` & `returnn-1.20230531.135404/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-list-devices.py` & `returnn-1.20230531.135404/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-lua-torch-layer.config` & `returnn-1.20230531.135404/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230531.135404/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-returnn-as-framework.py` & `returnn-1.20230531.135404/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-rf.config` & `returnn-1.20230531.135404/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-rhn-enwik8.config` & `returnn-1.20230531.135404/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-sprint-interface.py` & `returnn-1.20230531.135404/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-att-copy.config` & `returnn-1.20230531.135404/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-attention.config` & `returnn-1.20230531.135404/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-enc-dec.config` & `returnn-1.20230531.135404/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230531.135404/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230531.135404/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230531.135404/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230531.135404/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230531.135404/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-rec-self-att.config` & `returnn-1.20230531.135404/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230531.135404/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230531.135404/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-torch.config` & `returnn-1.20230531.135404/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230531.135404/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/demo.sh` & `returnn-1.20230531.135404/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230531.135404/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/README.txt` & `returnn-1.20230531.135404/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/config_demo` & `returnn-1.20230531.135404/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230531.135404/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/config_real` & `returnn-1.20230531.135404/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230531.135404/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/decode.py` & `returnn-1.20230531.135404/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230531.135404/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230531.135404/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230531.135404/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230531.135404/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230531.135404/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230531.135404/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230531.135404/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230531.135404/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/__init__.py` & `returnn-1.20230531.135404/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/__main__.py` & `returnn-1.20230531.135404/returnn/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -441,30 +441,44 @@
             output_per_seq_file=config.value("eval_output_file_per_seq", None),
             loss_name=config.value("loss_name", None),
             output_per_seq_format=config.list("output_per_seq_format", ["score"]),
             output_per_seq_file_format=config.value("output_per_seq_file_format", "txt"),
             lr_control_update_scores=lr_control_update_scores,
         )
     elif task in ["forward", "hpx"]:
-        assert eval_data is not None, "no eval data provided"
-        combine_labels = config.value("combine_labels", "")
-        engine.use_search_flag = config.bool("forward_use_search", False)
-        if config.has("epoch"):
-            config.set("load_epoch", config.int("epoch", 0))
-        engine.init_network_from_config(config)
-        output_file = config.value("output_file", "dump-fwd-epoch-%i.hdf" % engine.epoch)
-        forward_batch_size = config.int("forward_batch_size", 0)
-        if not forward_batch_size:
-            raise Exception("forward_batch_size not set")
-        engine.forward_to_hdf(
-            data=eval_data,
-            output_file=output_file,
-            combine_labels=combine_labels,
-            batch_size=forward_batch_size,
-        )
+        if config.typed_value("forward_callback") or not BackendEngine.is_tensorflow_selected():
+            engine.init_network_from_config(config)
+            if config.value("forward_data", "eval") in ["train", "dev", "eval"]:
+                data = {"train": train_data, "dev": dev_data, "eval": eval_data}[config.value("forward_data", "eval")]
+                assert data, "set forward_data"
+            else:
+                data = init_dataset(config.opt_typed_value("forward_data"))
+            forward_callback = config.typed_value("forward_callback")
+            assert forward_callback, "no forward_callback specified"
+            if callable(forward_callback):
+                forward_callback = forward_callback()
+            engine.forward_with_callback(dataset=data, callback=forward_callback)
+        else:
+            assert BackendEngine.is_tensorflow_selected()
+            assert eval_data is not None, "no eval data provided"
+            combine_labels = config.value("combine_labels", "")
+            engine.use_search_flag = config.bool("forward_use_search", False)
+            if config.has("epoch"):
+                config.set("load_epoch", config.int("epoch", 0))
+            engine.init_network_from_config(config)
+            output_file = config.value("output_file", "dump-fwd-epoch-%i.hdf" % engine.epoch)
+            forward_batch_size = config.int("forward_batch_size", 0)
+            if not forward_batch_size:
+                raise Exception("forward_batch_size not set")
+            engine.forward_to_hdf(
+                data=eval_data,
+                output_file=output_file,
+                combine_labels=combine_labels,
+                batch_size=forward_batch_size,
+            )
     elif task == "search":
         engine.use_search_flag = True
         engine.use_eval_flag = config.bool("search_do_eval", True)
         engine.init_network_from_config(config)
         if config.value("search_data", "eval") in ["train", "dev", "eval"]:
             data = {"train": train_data, "dev": dev_data, "eval": eval_data}[config.value("search_data", "eval")]
             assert data, "set search_data"
```

### Comparing `returnn-1.20230531.120344/returnn/__old_mod_loader__.py` & `returnn-1.20230531.135404/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/__setup__.py` & `returnn-1.20230531.135404/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/config.py` & `returnn-1.20230531.135404/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/audio.py` & `returnn-1.20230531.135404/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/basic.py` & `returnn-1.20230531.135404/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/bundle_file.py` & `returnn-1.20230531.135404/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/cached.py` & `returnn-1.20230531.135404/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/cached2.py` & `returnn-1.20230531.135404/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/generating.py` & `returnn-1.20230531.135404/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/hdf.py` & `returnn-1.20230531.135404/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/lm.py` & `returnn-1.20230531.135404/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/map.py` & `returnn-1.20230531.135404/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/meta.py` & `returnn-1.20230531.135404/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/multi_proc.py` & `returnn-1.20230531.135404/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/normalization_data.py` & `returnn-1.20230531.135404/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/numpy_dump.py` & `returnn-1.20230531.135404/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/raw_wav.py` & `returnn-1.20230531.135404/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/sprint.py` & `returnn-1.20230531.135404/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/stereo.py` & `returnn-1.20230531.135404/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230531.135404/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/datasets/util/vocabulary.py` & `returnn-1.20230531.135404/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/engine/base.py` & `returnn-1.20230531.135404/returnn/engine/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 import sys
 
 from returnn.config import Config, get_global_config
 from returnn.learning_rate_control import load_learning_rate_control_from_config, LearningRateControl
 from returnn.log import log
 from returnn.pretrain import Pretrain
 from returnn.util import basic as util
+from returnn.forward_iface import ForwardCallbackIface
+from returnn.datasets import Dataset
 
 
-class EngineBase(object):
+class EngineBase:
     """
     Base class for a backend engine, such as :class:`TFEngine.Engine`.
     """
 
     def __init__(self, config: Optional[Config] = None):
         """
         :param config:
@@ -30,14 +32,21 @@
         self.epoch = 0
         self.global_train_step = None  # type: Optional[int]
         self.pretrain = None  # type: Optional[Pretrain]
         self.model_filename = None  # type: Optional[str]
         self.learning_rate = 0.0  # set in init_train_epoch
         self.learning_rate_control = None  # type: Optional[LearningRateControl]
 
+    def init_network_from_config(self, config: Optional[Config] = None):
+        """
+        Initialize network/model
+
+        :param config:
+        """
+
     def init_train_from_config(self, config: Optional[Config] = None):
         """
         Initialize all engine parts needed for training
 
         :param config:
         """
         self.learning_rate_control = load_learning_rate_control_from_config(config)
@@ -230,7 +239,15 @@
 
     def is_first_epoch_after_pretrain(self):
         """
         :return: whether the current epoch is the first epoch right after pretraining
         :rtype: bool
         """
         return self.pretrain and self.epoch == self.pretrain.get_train_num_epochs() + 1
+
+    def forward_with_callback(self, *, dataset: Dataset, callback: ForwardCallbackIface):
+        """
+        Iterate through the dataset, calling `forward_step` from user config,
+        collecting outputs in `rf.get_run_ctx()` via `mark_as_output` calls,
+        and then calling `callback` for each entry.
+        """
+        raise NotImplementedError
```

### Comparing `returnn-1.20230531.120344/returnn/engine/batch.py` & `returnn-1.20230531.135404/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230531.135404/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/edit.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/select.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/transform.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/extern/graph_editor/util.py` & `returnn-1.20230531.135404/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/__init__.py` & `returnn-1.20230531.135404/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/_backend.py` & `returnn-1.20230531.135404/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/_numpy_backend.py` & `returnn-1.20230531.135404/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/_utils.py` & `returnn-1.20230531.135404/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/array_.py` & `returnn-1.20230531.135404/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/attention.py` & `returnn-1.20230531.135404/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/cond.py` & `returnn-1.20230531.135404/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/const.py` & `returnn-1.20230531.135404/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/container.py` & `returnn-1.20230531.135404/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/conv.py` & `returnn-1.20230531.135404/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/device.py` & `returnn-1.20230531.135404/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/dims.py` & `returnn-1.20230531.135404/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/dropout.py` & `returnn-1.20230531.135404/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/dtype.py` & `returnn-1.20230531.135404/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/encoder/base.py` & `returnn-1.20230531.135404/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/encoder/conformer.py` & `returnn-1.20230531.135404/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/init.py` & `returnn-1.20230531.135404/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/linear.py` & `returnn-1.20230531.135404/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/loop.py` & `returnn-1.20230531.135404/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/loss.py` & `returnn-1.20230531.135404/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/math_.py` & `returnn-1.20230531.135404/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/matmul.py` & `returnn-1.20230531.135404/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/module.py` & `returnn-1.20230531.135404/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/normalization.py` & `returnn-1.20230531.135404/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/parameter.py` & `returnn-1.20230531.135404/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/rand.py` & `returnn-1.20230531.135404/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/rec.py` & `returnn-1.20230531.135404/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/reduce.py` & `returnn-1.20230531.135404/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/run_ctx.py` & `returnn-1.20230531.135404/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/signal.py` & `returnn-1.20230531.135404/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/state.py` & `returnn-1.20230531.135404/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/tensor_array.py` & `returnn-1.20230531.135404/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/frontend/types.py` & `returnn-1.20230531.135404/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/import_/common.py` & `returnn-1.20230531.135404/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/import_/git.py` & `returnn-1.20230531.135404/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/import_/import_.py` & `returnn-1.20230531.135404/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/learning_rate_control.py` & `returnn-1.20230531.135404/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/log.py` & `returnn-1.20230531.135404/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/native_op.cpp` & `returnn-1.20230531.135404/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/native_op.py` & `returnn-1.20230531.135404/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/pretrain.py` & `returnn-1.20230531.135404/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/sprint/cache.py` & `returnn-1.20230531.135404/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/sprint/control.py` & `returnn-1.20230531.135404/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/sprint/error_signals.py` & `returnn-1.20230531.135404/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/sprint/extern_interface.py` & `returnn-1.20230531.135404/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/sprint/interface.py` & `returnn-1.20230531.135404/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/_dim_extra.py` & `returnn-1.20230531.135404/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/_tensor_extra.py` & `returnn-1.20230531.135404/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230531.135404/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230531.135404/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230531.135404/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/dim.py` & `returnn-1.20230531.135404/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/marked_dim.py` & `returnn-1.20230531.135404/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/tensor.py` & `returnn-1.20230531.135404/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/tensor_dict.py` & `returnn-1.20230531.135404/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tensor/utils.py` & `returnn-1.20230531.135404/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/compat.py` & `returnn-1.20230531.135404/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/data_pipeline.py` & `returnn-1.20230531.135404/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/distributed.py` & `returnn-1.20230531.135404/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/engine.py` & `returnn-1.20230531.135404/returnn/tf/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from returnn.tf.util.data import Data
 from returnn.tf.layers.base import LayerBase
 from returnn.tf.updater import Updater
 from returnn.tf.data_pipeline import FeedDictDataProvider, DatasetDataProvider
 import returnn.tf.horovod as tf_horovod
 import returnn.util.basic as util
 from returnn.util.basic import hms, NumbersDict, BackendEngine, BehaviorVersion
+from returnn.forward_iface import ForwardCallbackIface
 from pprint import pprint
 
 
 class CancelTrainingException(Exception):
     """
     Training was cancelled.
     """
@@ -1171,19 +1172,20 @@
             net_dict = self.pretrain.get_final_network_json()
         else:
             from returnn.config import network_json_from_config
 
             net_dict = network_json_from_config(config)
         return net_dict
 
-    def init_network_from_config(self, config=None, net_dict_post_proc=None):
+    def init_network_from_config(self, config=None, *, net_dict_post_proc=None):
         """
         :param returnn.config.Config|None config:
         :param ((dict)->dict)|None net_dict_post_proc:
         """
+        super().init_network_from_config(config=config)
         if not config:
             config = self.config
         self.model_filename = config.value("model", None)
         self.preload_from_files = config.typed_value("preload_from_files", {})
         self.pretrain = pretrain_from_config(config)
         self.custom_get_net_dict = config.typed_value("get_network")
         self._have_rf_get_model_func = bool(config.typed_value("get_model"))
@@ -2452,14 +2454,19 @@
         forwarder.run(report_prefix=self.get_epoch_str() + " forward")
         if not forwarder.finalized:
             print("Error happened. Exit now.")
             forwarder.exit_due_to_error()
 
         writer.close()
 
+    def forward_with_callback(self, *, dataset: Dataset, callback: ForwardCallbackIface):
+        """forward"""
+        # https://github.com/rwth-i6/returnn/issues/1336
+        raise NotImplementedError("TF engine does not support the generic forward func yet...")
+
     # noinspection PyUnusedLocal
     def analyze(self, data, statistics):
         """
         :param Dataset.Dataset data:
         :param list[str]|None statistics: ignored at the moment
         :return: print everything to log.v1, and return the Runner instance to get access to all the stats
         :rtype: Runner
```

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230531.135404/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230531.135404/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/horovod.py` & `returnn-1.20230531.135404/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230531.135404/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/base.py` & `returnn-1.20230531.135404/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/basic.py` & `returnn-1.20230531.135404/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/rec.py` & `returnn-1.20230531.135404/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/segmental_model.py` & `returnn-1.20230531.135404/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/signal_processing.py` & `returnn-1.20230531.135404/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/layers/variable.py` & `returnn-1.20230531.135404/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/native_op.py` & `returnn-1.20230531.135404/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/network.py` & `returnn-1.20230531.135404/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/sprint.py` & `returnn-1.20230531.135404/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/updater.py` & `returnn-1.20230531.135404/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/util/basic.py` & `returnn-1.20230531.135404/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/util/data.py` & `returnn-1.20230531.135404/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/util/ken_lm.py` & `returnn-1.20230531.135404/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/tf/util/open_fst.py` & `returnn-1.20230531.135404/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/data/pipeline.py` & `returnn-1.20230531.135404/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230531.135404/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/data/tensor_utils.py` & `returnn-1.20230531.135404/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/engine.py` & `returnn-1.20230531.135404/returnn/torch/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
 from returnn.tensor import TensorDict, Tensor, Dim
 from returnn.datasets.basic import init_dataset, Dataset
 from returnn.util import basic as util
 from returnn.util import NumbersDict
 from returnn.util.basic import NotSpecified
+from returnn.forward_iface import ForwardCallbackIface
+
 from .updater import Updater
 from .data import pipeline as data_pipeline
 from .data import returnn_dataset_wrapper
 from .frontend.bridge import rf_module_to_pt_module
 
 
 class Engine(EngineBase):
@@ -51,14 +53,19 @@
         self._eval_dataloaders = {}  # type: Dict[str, DataLoader2]
 
         self._start_epoch = None  # type: Optional[int]
         self._final_epoch = None  # type: Optional[int]
         self._orig_model = None  # type: Optional[Union[rf.Module, torch.nn.Module]]
         self._pt_model = None  # type: Optional[torch.nn.Module]
         self._train_step_func = None  # type: Optional[Callable]
+        self._forward_step_func = self.config.typed_value("forward_step")  # type: Optional[Callable]
+        self._forward_step_expected_outputs = None  # type: Optional[TensorDict]
+        if self.config.typed_value("model_outputs") is not None:
+            self._forward_step_expected_outputs = TensorDict()
+            self._forward_step_expected_outputs.update(self.config.typed_value("model_outputs"), auto_convert=True)
         self._save_model_epoch_interval = 1
         self._updater = None  # type: Optional[Updater]
 
         self._use_autocast = False
         self._autocast_dtype = None  # type: Optional[str]
         self._grad_scaler = None  # type: Optional[amp.GradScaler]
 
@@ -87,83 +94,97 @@
         if grad_scaler_opts is NotSpecified:
             grad_scaler_opts = {} if self._use_autocast else None
         if grad_scaler_opts is not None:
             assert isinstance(grad_scaler_opts, dict)
             print("Using GradScaler with options:", grad_scaler_opts, file=log.v2)
             self._grad_scaler = amp.GradScaler(**grad_scaler_opts)
 
+    def init_network_from_config(self, config: Optional[Config] = None):
+        """init model"""
+        assert config is self.config or not config
+        super().init_network_from_config(config=config)
+
+        extern_data = TensorDict()
+        extern_data_dict = self.config.typed_value("extern_data")
+        assert extern_data_dict, "extern_data is not specified in config"
+        extern_data.update(extern_data_dict, auto_convert=True)
+        if "seq_tag" not in extern_data.data:
+            batch_dim = _get_batch_dim_from_extern_data(extern_data)
+            extern_data.data["seq_tag"] = Tensor(name="seq_tag", dtype="string", dims=[batch_dim])
+        self.extern_data = extern_data
+
+        self._load_model()
+
     def init_train_from_config(
         self,
         config: Optional[Config] = None,
         train_data: Optional[Dataset] = None,
         dev_data: Optional[Dataset] = None,
         eval_data: Optional[Dataset] = None,
     ):
         """
         :param config:
         :param train_data:
         :param dev_data:
         :param eval_data:
         """
-        assert config is self.config
+        assert config is self.config or not config
         super().init_train_from_config(config=config)
+
         self.train_dataset = train_data
         self.eval_datasets.clear()
         if dev_data:
             self.eval_datasets["dev"] = dev_data
         if eval_data:
             self.eval_datasets["eval"] = eval_data
         if config.has("eval_datasets"):
             for dataset_name, dataset_opts in config.typed_value("eval_datasets", {}).items():
                 self.eval_datasets[dataset_name] = init_dataset(dataset_opts, default_kwargs={"name": dataset_name})
 
-        extern_data = TensorDict()
-        extern_data_dict = self.config.typed_value("extern_data")
-        extern_data.update(extern_data_dict, auto_convert=True)
-        if "seq_tag" not in extern_data.data:
-            batch_dim = _get_batch_dim_from_extern_data(extern_data)
-            extern_data.data["seq_tag"] = Tensor(name="seq_tag", dtype="string", dims=[batch_dim])
-        self.extern_data = extern_data
-
         self._train_dataloader = self._create_data_loader(train_data) if train_data else None
         for dataset_name, dataset in self.eval_datasets.items():
             self._eval_dataloaders[dataset_name] = self._create_data_loader(dataset)
 
         self._start_epoch = self.get_train_start_epoch(self.config)
         self._final_epoch = self.config_get_final_epoch(self.config)
 
-        self._load_model(epoch=self._start_epoch)
+        self.init_network_from_config(config=config)
+
         self._save_model_epoch_interval = config.int("save_interval", 1)
 
         self._updater = Updater(self.config, self._pt_model, self.learning_rate)
         self._updater.create_optimizer()
         if self._start_epoch > 1:
-            self._load_optimizer(self._start_epoch)
+            self._load_optimizer()
 
         self._train_step_func = self.config.typed_value("train_step")
         assert self._train_step_func, "train_step not defined"
 
     def train(self):
         """
         Main training loop.
         """
-
-        print("Starting training at epoch {}.".format(self._start_epoch), file=log.v3)
         assert self._pt_model is not None, "Model not initialized, call init_train_from_config()."
 
-        self.epoch = self._start_epoch
-        self._epoch_mp_shared.value = self.epoch
-        while self.epoch <= self._final_epoch:
-            self.init_train_epoch()
-            self.train_epoch()
+        if self._start_epoch > self._final_epoch:
+            print(f"Already trained until final epoch {self._final_epoch}, nothing to do.", file=log.v3)
+            return
 
+        print(
+            f"Starting training at epoch {self._start_epoch}, global train step {self.global_train_step}", file=log.v3
+        )
+        self.epoch = self._start_epoch - 1
+        while self.epoch + 1 <= self._final_epoch:
             self.epoch += 1
             self._epoch_mp_shared.value = self.epoch
 
-        print("Finished training at epoch {}.".format(self.epoch), file=log.v3)
+            self.init_train_epoch()
+            self.train_epoch()
+
+        print(f"Finished training at epoch {self.epoch}, global train step {self.global_train_step}", file=log.v3)
 
     def init_train_epoch(self):
         """
         init train (sub)epoch. LR etc
         """
         self.learning_rate = self.learning_rate_control.get_learning_rate_for_epoch(self.epoch)
 
@@ -177,17 +198,20 @@
         print("start", self.get_epoch_str(), "with learning rate", self.learning_rate, "...", file=log.v4)
 
         self._pt_model.train()
 
         accumulated_losses_dict = NumbersDict()
         accumulated_inv_norm_factors_dict = NumbersDict()
         step_idx = 0
-        for data in self._train_dataloader:
+        for extern_data_raw in self._train_dataloader:
             self._updater.get_optimizer().zero_grad()
-            self._run_step(data, train_flag=True)
+            extern_data = _raw_dict_to_extern_data(
+                extern_data_raw, extern_data_template=self.extern_data, device=self._device
+            )
+            self._run_step(extern_data, train_func=True, train_flag=True)
 
             train_ctx = rf.get_run_ctx()
             total_loss = train_ctx.total_loss()
             losses_dict = NumbersDict(
                 {
                     name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
                     for name, loss in train_ctx.losses.items()
@@ -248,17 +272,20 @@
             data_loader = self._eval_dataloaders[dataset_name]
 
             accumulated_losses_dict = NumbersDict()
             accumulated_inv_norm_factors_dict = NumbersDict()
             step_idx = 0
 
             with torch.no_grad():
-                for data in data_loader:
+                for extern_data_raw in data_loader:
+                    extern_data = _raw_dict_to_extern_data(
+                        extern_data_raw, extern_data_template=self.extern_data, device=self._device
+                    )
 
-                    self._run_step(data)
+                    self._run_step(extern_data, train_func=True)
                     train_ctx = rf.get_run_ctx()
 
                     if score_keys is None:
                         score_keys = [name for name, loss in train_ctx.losses.items() if not loss.as_error]
                         error_keys = [name for name, loss in train_ctx.losses.items() if loss.as_error]
 
                     losses_dict = NumbersDict(
@@ -328,53 +355,77 @@
             try:
                 # noinspection PyPackageRequirements
                 import dill
             except ImportError:
                 raise ModuleNotFoundError("Possible type error in DataLoader2 due to missing module 'dill'") from exc
             raise
 
-    def _run_step(self, extern_data_raw: Dict[str, torch.Tensor], *, train_flag: bool = False):
+    def _run_step(self, extern_data: TensorDict, *, train_flag: bool = False, train_func: bool):
         """
-        :param dict[str, torch.Tensor] extern_data_raw: model inputs for the step
+        :param extern_data: model inputs for the step
         """
-        extern_data = _raw_dict_to_extern_data(
-            extern_data_raw, extern_data_template=self.extern_data, device=self._device
-        )
-
-        rf.init_train_step_run_ctx(train_flag=train_flag)
+        if train_func:
+            assert self._train_step_func is not None
+            rf.init_train_step_run_ctx(train_flag=train_flag)
+        else:
+            assert self._forward_step_func is not None, "define forward_step in the config"
+            rf.init_forward_step_run_ctx(expected_outputs=self._forward_step_expected_outputs)
 
         with autocast(device_type=self._device, dtype=self._autocast_dtype) if self._use_autocast else nullcontext():
             sentinel_kw = {"__fwd_compatible_random_arg_%i" % int(random() * 100): None}
-            self._train_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
+            if train_func:
+                self._train_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
+            else:
+                self._forward_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
 
-    def _load_model(self, *, epoch: int):
+    def _load_model(self):
         """
         Sets self._model to a torch.nn.Module.
-
-        :param epoch:
         """
+        # Check existing model. This takes `load` and `load_epoch` into account,
+        # and also whether we are in train or eval mode.
+        epoch, model_epoch_filename = self.get_epoch_model(self.config)
+
         checkpoint_state = None
-        if epoch > 1:
-            filename = self.get_epoch_model_filename(epoch=epoch - 1) + util.get_model_filename_postfix()
+        if model_epoch_filename:
+            filename = model_epoch_filename + util.get_model_filename_postfix()
             print("Load model %s" % (filename,), file=log.v4)
             checkpoint_state = torch.load(filename)
-            assert checkpoint_state["epoch"] == epoch - 1
+            if epoch is None:
+                epoch = checkpoint_state["epoch"]
             step = checkpoint_state["step"]
+            print(f"  epoch {epoch}, global train step {step}", file=log.v4)
+            # The checkpoint was saved when the step was already increased (but not the epoch yet).
+            # Restore the last step.
+            # Below, we will increase the step again in case we are training.
+            step -= 1
         else:
             step = 0
-        self.global_train_step = step
+            epoch = self._start_epoch or 1
+
+        is_training = self.config.value("task", "train") == "train"
+        is_first_train_epoch = not epoch and (is_training or self.config.value("task", "train") == "initialize_model")
 
         # See :mod:`rf.rand` docstring for an explanation of this logic.
         random_seed = self.config.int("random_seed", 42)
         random_seed = (epoch * 193939 + step * 19937 + random_seed * 27644437 + 479001599) % (2**31)
         rf.set_random_seed(random_seed)
 
         get_model_func = self.config.typed_value("get_model")
-        assert get_model_func, "get_model not defined"
+        assert get_model_func, "get_model not defined in config"
         sentinel_kw = {"__fwd_compatible_random_arg_%i" % int(random() * 100): None}
+        # Note on the `epoch` and `step` args:
+        # This is the current epoch and step, i.e. the epoch and step we are about to run.
+        # This is not the epoch and step of the model we are loading.
+        # Epoch starts at 1, step starts at 0.
+        # It is the global train step, i.e. the number of train steps we have done so far over all epochs,
+        # so it does not reset to 0 at each epoch.
+        # In a checkpoint, we stored the epoch of the most recent epoch we just finished.
+        # We stored the global train step after we already incremented it.
+        # The checkpoint is always stored when we just have finished the epoch.
         model = get_model_func(epoch=epoch, step=step, **sentinel_kw)
         self._orig_model = model
         if isinstance(model, rf.Module):
             self._pt_model = rf_module_to_pt_module(model)
         elif isinstance(model, torch.nn.Module):
             self._pt_model = model
         else:
@@ -383,18 +434,14 @@
         print("Model:", self._pt_model, file=log.v4)
 
         if checkpoint_state is not None:
             self._pt_model.load_state_dict(checkpoint_state["model"])
         preload_from_files = self.config.typed_value("preload_from_files", {})
         if preload_from_files:
             # see `preload_from_files` in tf engine and `returnn.tf.network.CustomCheckpointLoader`
-            is_training = self.config.value("task", "train") == "train"
-            is_first_train_epoch = epoch == 1 and (
-                is_training or self.config.value("task", "train") == "initialize_model"
-            )
             # We use the reversed sorted order here to achieve consistent behavior with the TF engine.
             # There, the keys are used in sorted order but if a variable is loaded,
             # it will not be considered anymore afterward.
             # So the first occurrence is used.
             # Here, we overwrite variables even if they have been loaded before.
             # In order to get consistent behavior, we use the reversed order.
             for preload_key, opts in reversed(sorted(preload_from_files.items())):
@@ -436,36 +483,45 @@
                     prefix_keys = [key for key in self._pt_model.state_dict() if key.startswith(opts.get("prefix", ""))]
                     missing_prefix_keys = set(prefix_keys).intersection(set(missing_keys))
                     assert not missing_prefix_keys, f"Missing keys and ignore_missing=False: {missing_prefix_keys}"
                 print(f"Missing keys: {missing_keys}", file=log.v4)
 
         self._pt_model.to(self._device)
 
+        if model_epoch_filename and is_training:
+            # We loaded a model from a checkpoint, and the epoch and step were taken from it.
+            # The epoch was just finished, so we need to increment it.
+            # We decremented the step above.
+            epoch += 1
+            step += 1
+        self.epoch = epoch  # in training, this will be reset to start_epoch
+        self.global_train_step = step
+
     def _save_model(self):
         """
         Saves the state of self._model to file.
         """
         filename = self.get_epoch_model_filename() + util.get_model_filename_postfix()
         directory = os.path.dirname(filename)
         if not os.path.exists(directory):
             os.makedirs(directory, exist_ok=True)
 
         print("Save model under %s" % (filename,), file=log.v4)
         torch.save(
             {"model": self._pt_model.state_dict(), "epoch": self.epoch, "step": self.global_train_step}, filename
         )
 
-    def _load_optimizer(self, epoch):
+    def _load_optimizer(self):
         """
         Loads a torch.optim.Optimizer from disk and uses it as the optimizer.
         This function is a wrapper to Updater.load_optimizer().
-
-        :param int epoch: Epoch from which to load the optimizer state.
         """
-        filename = self.get_epoch_model_filename(epoch=epoch - 1) + ".opt" + util.get_model_filename_postfix()
+        filename = (
+            self.get_epoch_model_filename(epoch=self._start_epoch - 1) + ".opt" + util.get_model_filename_postfix()
+        )
         self._updater.load_optimizer(filename)
 
     def _save_optimizer(self):
         """
         Saves the optimizer state to a file.
         This function is a wrapper to Updater.save_optimizer().
         """
@@ -479,14 +535,50 @@
         # keep only the last two optimizer states (two in case one file gets corrupted)
         clean_epoch = self.epoch - 2
         if clean_epoch > 0:
             filename = self.get_epoch_model_filename(epoch=clean_epoch) + ".opt" + util.get_model_filename_postfix()
             if os.path.isfile(filename):
                 os.unlink(filename)
 
+    def forward_with_callback(self, *, dataset: Dataset, callback: ForwardCallbackIface):
+        """forward"""
+        assert isinstance(dataset, Dataset)
+        assert isinstance(callback, ForwardCallbackIface)
+
+        self._pt_model.eval()
+
+        data_loader = self._create_data_loader(dataset)
+        batch_dim = _get_batch_dim_from_extern_data(self.extern_data)
+
+        with torch.no_grad():
+            callback.init(model=self._orig_model)
+
+            for extern_data_raw in data_loader:
+                extern_data = _raw_dict_to_extern_data(
+                    extern_data_raw, extern_data_template=self.extern_data, device=self._device
+                )
+                self._run_step(extern_data, train_func=False)
+                ctx = rf.get_run_ctx()
+                ctx.check_outputs_complete()
+
+                model_outputs = ctx.outputs
+                model_outputs_per_batch_template = TensorDict(
+                    {k: v.copy_template_excluding_axis(0) for k, v in model_outputs.data.items()}
+                )
+                for batch_idx in range(batch_dim.get_dim_value()):
+                    seq_tag = extern_data["seq_tag"].raw_tensor[batch_idx].item()
+                    model_outputs_per_batch = TensorDict(
+                        {k: v.copy() for k, v in model_outputs_per_batch_template.data.items()}
+                    )
+                    for k, v in model_outputs.data.items():
+                        model_outputs_per_batch[k].raw_tensor = v.raw_tensor[batch_idx]
+                    callback.process_seq(seq_tag=seq_tag, outputs=model_outputs_per_batch)
+
+            callback.finish()
+
 
 def _to_raw(n: Union[int, float, Tensor]):
     if isinstance(n, (int, float)):
         return n
     if isinstance(n, Tensor):
         return n.raw_tensor.detach().cpu().numpy()
     raise TypeError(f"Unexpected {n} of type {type(n)}")
```

### Comparing `returnn-1.20230531.120344/returnn/torch/frontend/_backend.py` & `returnn-1.20230531.135404/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/frontend/_rand.py` & `returnn-1.20230531.135404/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/frontend/bridge.py` & `returnn-1.20230531.135404/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/torch/updater.py` & `returnn-1.20230531.135404/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/basic.py` & `returnn-1.20230531.135404/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/better_exchook.py` & `returnn-1.20230531.135404/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/bpe.py` & `returnn-1.20230531.135404/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/debug.py` & `returnn-1.20230531.135404/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/debug_helpers.py` & `returnn-1.20230531.135404/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/fsa.py` & `returnn-1.20230531.135404/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230531.135404/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/pprint.py` & `returnn-1.20230531.135404/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/py-to-pickle.cpp` & `returnn-1.20230531.135404/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/sig_proc.py` & `returnn-1.20230531.135404/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn/util/task_system.py` & `returnn-1.20230531.135404/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/returnn.egg-info/PKG-INFO` & `returnn-1.20230531.135404/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230531.120344
+Version: 1.20230531.135404
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230531.120344/returnn.egg-info/SOURCES.txt` & `returnn-1.20230531.135404/returnn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 demos/mdlstm/artificial_rgb/go.sh
 demos/mdlstm/artificial_rgb/trainconfig
 returnn/__init__.py
 returnn/__main__.py
 returnn/__old_mod_loader__.py
 returnn/__setup__.py
 returnn/config.py
+returnn/forward_iface.py
 returnn/learning_rate_control.py
 returnn/log.py
 returnn/native_op.cpp
 returnn/native_op.py
 returnn/pretrain.py
 returnn.egg-info/PKG-INFO
 returnn.egg-info/SOURCES.txt
@@ -327,14 +328,15 @@
 tests/test_rf_math.py
 tests/test_rf_normalization.py
 tests/test_rf_rec.py
 tests/test_rf_reduce.py
 tests/test_rf_signal.py
 tests/test_tensor.py
 tests/test_tools.py
+tests/test_torch_engine.py
 tests/test_torch_frontend.py
 tests/test_torch_internal_frontend.py
 tests/PyCharm.idea/.gitignore
 tests/PyCharm.idea/.name
 tests/PyCharm.idea/codeStyleSettings.xml
 tests/PyCharm.idea/misc.xml
 tests/PyCharm.idea/modules.xml
```

### Comparing `returnn-1.20230531.120344/setup.py` & `returnn-1.20230531.135404/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/DummySprintExec.py` & `returnn-1.20230531.135404/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230531.135404/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230531.135404/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230531.135404/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/_set_num_threads1.py` & `returnn-1.20230531.135404/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/_setup_test_env.py` & `returnn-1.20230531.135404/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/bpe-unicode-demo.codes` & `returnn-1.20230531.135404/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/bpe-unicode-demo.vocab` & `returnn-1.20230531.135404/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/lexicon_opt.isyms` & `returnn-1.20230531.135404/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/lexicon_opt.jpg` & `returnn-1.20230531.135404/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/lint_common.py` & `returnn-1.20230531.135404/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/pycharm-inspect.py` & `returnn-1.20230531.135404/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/pylint.py` & `returnn-1.20230531.135404/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/returnn-as-framework.py` & `returnn-1.20230531.135404/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/rf_utils.py` & `returnn-1.20230531.135404/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/spelling.dic` & `returnn-1.20230531.135404/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Config.py` & `returnn-1.20230531.135404/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Dataset.py` & `returnn-1.20230531.135404/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Fsa.py` & `returnn-1.20230531.135404/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_GeneratingDataset.py` & `returnn-1.20230531.135404/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_HDFDataset.py` & `returnn-1.20230531.135404/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_LearningRateControl.py` & `returnn-1.20230531.135404/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Log.py` & `returnn-1.20230531.135404/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_MultiProcDataset.py` & `returnn-1.20230531.135404/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_PTDataset.py` & `returnn-1.20230531.135404/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Pretrain.py` & `returnn-1.20230531.135404/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_ResNet.py` & `returnn-1.20230531.135404/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_SprintDataset.py` & `returnn-1.20230531.135404/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_SprintInterface.py` & `returnn-1.20230531.135404/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFEngine.py` & `returnn-1.20230531.135404/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFNativeOp.py` & `returnn-1.20230531.135404/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFNetworkLayer.py` & `returnn-1.20230531.135404/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230531.135404/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230531.135404/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFUpdater.py` & `returnn-1.20230531.135404/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TFUtil.py` & `returnn-1.20230531.135404/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TF_determinism.py` & `returnn-1.20230531.135404/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TaskSystem.py` & `returnn-1.20230531.135404/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230531.135404/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_TranslationDataset.py` & `returnn-1.20230531.135404/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_Util.py` & `returnn-1.20230531.135404/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_demos.py` & `returnn-1.20230531.135404/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_fork_exec.py` & `returnn-1.20230531.135404/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_hdf_dump.py` & `returnn-1.20230531.135404/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_array.py` & `returnn-1.20230531.135404/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_attention.py` & `returnn-1.20230531.135404/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_base.py` & `returnn-1.20230531.135404/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_cond.py` & `returnn-1.20230531.135404/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_container.py` & `returnn-1.20230531.135404/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_conv.py` & `returnn-1.20230531.135404/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_encoder_conformer.py` & `returnn-1.20230531.135404/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_loop.py` & `returnn-1.20230531.135404/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_math.py` & `returnn-1.20230531.135404/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_normalization.py` & `returnn-1.20230531.135404/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_rec.py` & `returnn-1.20230531.135404/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_reduce.py` & `returnn-1.20230531.135404/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_rf_signal.py` & `returnn-1.20230531.135404/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_tensor.py` & `returnn-1.20230531.135404/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_tools.py` & `returnn-1.20230531.135404/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_torch_frontend.py` & `returnn-1.20230531.135404/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tests/test_torch_internal_frontend.py` & `returnn-1.20230531.135404/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/analyze-dataset-batches.py` & `returnn-1.20230531.135404/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/bliss-collect-seq-lens.py` & `returnn-1.20230531.135404/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/bliss-dump-text.py` & `returnn-1.20230531.135404/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/bliss-get-segment-names.py` & `returnn-1.20230531.135404/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/bliss-to-ogg-zip.py` & `returnn-1.20230531.135404/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/bpe-create-lexicon.py` & `returnn-1.20230531.135404/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/calculate-word-error-rate.py` & `returnn-1.20230531.135404/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/cleanup-old-models.py` & `returnn-1.20230531.135404/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/collect-orth-symbols.py` & `returnn-1.20230531.135404/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/collect-words.py` & `returnn-1.20230531.135404/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/compile_native_op.py` & `returnn-1.20230531.135404/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/compile_tf_graph.py` & `returnn-1.20230531.135404/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/debug-dump-search-scores.py` & `returnn-1.20230531.135404/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/debug-plot-search-scores.py` & `returnn-1.20230531.135404/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-dataset-raw-strings.py` & `returnn-1.20230531.135404/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-dataset.py` & `returnn-1.20230531.135404/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-forward-stats.py` & `returnn-1.20230531.135404/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-forward.py` & `returnn-1.20230531.135404/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-network-json.py` & `returnn-1.20230531.135404/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/dump-pickle.py` & `returnn-1.20230531.135404/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230531.135404/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/get-attention-weights.py` & `returnn-1.20230531.135404/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/get-best-model-epoch.py` & `returnn-1.20230531.135404/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/hdf_dump.py` & `returnn-1.20230531.135404/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230531.135404/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/import-blocks-mt-model.py` & `returnn-1.20230531.135404/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/import-t2t-mt-model.py` & `returnn-1.20230531.135404/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/Makefile` & `returnn-1.20230531.135404/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/README.md` & `returnn-1.20230531.135404/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/example/README.md` & `returnn-1.20230531.135404/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230531.135404/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230531.135404/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230531.135404/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/file.h` & `returnn-1.20230531.135404/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230531.135404/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230531.135404/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/main.cc` & `returnn-1.20230531.135404/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230531.135404/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230531.135404/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230531.135404/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/tf_avg_checkpoints.py` & `returnn-1.20230531.135404/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/tf_inspect_checkpoint.py` & `returnn-1.20230531.135404/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/tf_inspect_summary_log.py` & `returnn-1.20230531.135404/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230531.120344/tools/torch_export_to_onnx.py` & `returnn-1.20230531.135404/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

