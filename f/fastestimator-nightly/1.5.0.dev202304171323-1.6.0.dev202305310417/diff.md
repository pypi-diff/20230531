# Comparing `tmp/fastestimator-nightly-1.5.0.dev202304171323.tar.gz` & `tmp/fastestimator-nightly-1.6.0.dev202305310417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastestimator-nightly-1.5.0.dev202304171323.tar", last modified: Mon Apr 17 13:23:26 2023, max compression
+gzip compressed data, was "fastestimator-nightly-1.6.0.dev202305310417.tar", last modified: Wed May 31 04:17:47 2023, max compression
```

## Comparing `fastestimator-nightly-1.5.0.dev202304171323.tar` & `fastestimator-nightly-1.6.0.dev202305310417.tar`

### file list

```diff
@@ -1,775 +1,779 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.311324 fastestimator-nightly-1.5.0.dev202304171323/
--rw-r--r--   0 root         (0) root         (0)      615 2023-04-17 13:23:26.307325 fastestimator-nightly-1.5.0.dev202304171323/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:25.991322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/
--rw-r--r--   0 root         (0) root         (0)     3092 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:25.995322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:25.995322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1609 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7452 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/lenet.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/unet.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:25.999322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/lenet.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/unet.py
--rw-r--r--   0 root         (0) root         (0)     5580 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.027322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/
--rw-r--r--   0 root         (0) root         (0)    10420 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_abs.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_argmax.py
--rw-r--r--   0 root         (0) root         (0)     4853 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_cast.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_concat.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_convert_tensor_precision.py
--rw-r--r--   0 root         (0) root         (0)     7866 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_exp.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_flip.py
--rw-r--r--   0 root         (0) root         (0)     6816 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_gather_from_batch.py
--rw-r--r--   0 root         (0) root         (0)     4694 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_shape.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_huber.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_iwd.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     4558 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_load_model.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_maximum.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_permute.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_pow.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_roll.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_save_model.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_sign.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_smooth_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     5742 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5245 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_update_model.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_watch.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_where.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.031322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/history.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/logs.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/plot.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.039322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16465 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/csv_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.051322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/
--rw-r--r--   0 root         (0) root         (0)     1798 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)     4020 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifair10.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifair100.py
--rw-r--r--   0 root         (0) root         (0)     3516 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifar10.py
--rw-r--r--   0 root         (0) root         (0)     3557 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifar100.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cub200.py
--rw-r--r--   0 root         (0) root         (0)     5955 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/em_3d.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/food101.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/horse2zebra.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/imdb_review.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mendeley.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mitmovie_ner.py
--rw-r--r--   0 root         (0) root         (0)     1338 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mnist.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/montgomery.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mscoco.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/nih_chestxray.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/omniglot.py
--rw-r--r--   0 root         (0) root         (0)     9835 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/pascal_voc.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/penn_treebank.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/shakespeare.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/skl_digits.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/svhn.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/svhn_cropped.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/tednmt.py
--rw-r--r--   0 root         (0) root         (0)     4183 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/tiny_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     5509 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/usps.py
--rw-r--r--   0 root         (0) root         (0)    20437 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    25446 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)     8402 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/op_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9018 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/siamese_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    31654 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.051322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.051322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1200 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.055322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/reflection_padding_2d.py
--rw-r--r--   0 root         (0) root         (0)    50620 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.055322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.055322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.059322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     5873 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4997 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.075322 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)     5956 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/affine.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/center_crop.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/crop.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     4920 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/flip.py
--rw-r--r--   0 root         (0) root         (0)     4545 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4014 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/multivariate.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     5191 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_crop.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_scale.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     5023 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/read_mat.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/resize.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/rotate.py
--rw-r--r--   0 root         (0) root         (0)     6176 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/transpose.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)    16413 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.099323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)    10320 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/binarize.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/blur.py
--rw-r--r--   0 root         (0) root         (0)     3497 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/brightness.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/calibate.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/clahe.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/color.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/contrast.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/downscale.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/equalize.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/from_float.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/median_blur.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/minmax.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/normalize.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/onehot.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/posterize.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_rain.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_snow.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/read_image.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/rua.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/sharpness.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/shear_x.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/solarize.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_array.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_float.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_gray.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/translate_x.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/translate_y.py
--rw-r--r--   0 root         (0) root         (0)     3279 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/univariate.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/word_to_id.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.103323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)     2326 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/argmax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.103323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7214 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/cutmix_batch.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/mixup_batch.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/average.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.107323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/fgsm.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/gradient.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.111323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)     2300 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5748 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/dice_loss.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/hinge.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     9186 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.115323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)     1454 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4335 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.115323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10649 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/model.py
--rw-r--r--   0 root         (0) root         (0)    11964 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/update.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/normalize.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/permute.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/resize3d.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/tensorop.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)    35670 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.115323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/lr_shedule.py
--rw-r--r--   0 root         (0) root         (0)     9875 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.119323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/golden_section.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/grid_search.py
--rw-r--r--   0 root         (0) root         (0)     9239 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.123323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/cartesian.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/heatmap.py
--rw-r--r--   0 root         (0) root         (0)     4789 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/parallel_coordinate_plot.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/vis_util.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.127323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41578 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.127323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/log_parse.py
--rw-r--r--   0 root         (0) root         (0)    34392 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/log_plot.py
--rw-r--r--   0 root         (0) root         (0)     9909 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/summary.py
--rw-r--r--   0 root         (0) root         (0)    18146 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.131323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/nightly_util.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.131323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.135323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)     1678 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3867 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     5529 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.143323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/
--rw-r--r--   0 root         (0) root         (0)     2539 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7889 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     8764 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/grid_display.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/image_saver.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)    23853 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    22579 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/test_report.py
--rw-r--r--   0 root         (0) root         (0)    41848 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.143323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/meta/
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/meta/_per_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.151323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/
--rw-r--r--   0 root         (0) root         (0)     2360 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/accuracy.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/auc.py
--rw-r--r--   0 root         (0) root         (0)    10591 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/bleu_score.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/dice.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/f1_score.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/mcc.py
--rw-r--r--   0 root         (0) root         (0)    18344 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/precision.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/recall.py
--rw-r--r--   0 root         (0) root         (0)    21156 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/trace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.155323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10667 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/eigen_cam.py
--rw-r--r--   0 root         (0) root         (0)     7808 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/grad_cam.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     6905 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/label_tracker.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.163323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/
--rw-r--r--   0 root         (0) root         (0)     3768 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25225 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/base_util.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/cli_util.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/data.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/google_download_util.py
--rw-r--r--   0 root         (0) root         (0)    31984 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/img_data.py
--rw-r--r--   0 root         (0) root         (0)     8260 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/latex_util.py
--rw-r--r--   0 root         (0) root         (0)    58370 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    11038 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/util.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.163323 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/xai/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12171 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.307325 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      615 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34951 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-17 13:23:25.000000 fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 13:23:26.311324 fastestimator-nightly-1.5.0.dev202304171323/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2865 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.167323 fastestimator-nightly-1.5.0.dev202304171323/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.167323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.171323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.171323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_save_model_load_model.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_update_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.175323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4980 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.175323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/dataset/test_batch_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.175323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.175323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.179323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.179323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.179323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.183323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.183323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.187323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.187323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)    10344 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.191323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.191323 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
--rw-r--r--   0 root         (0) root         (0)    22429 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_average.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.195324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_arc.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14280 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.195324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.195324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/visualize/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/visualize/test_visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.199324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11980 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/test_system.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_estimator.py
--rw-r--r--   0 root         (0) root         (0)    28036 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_network.py
--rw-r--r--   0 root         (0) root         (0)    98463 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.203324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.203324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.211324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     7106 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_image_saver.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     8180 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_test_report.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.215324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_accuracy.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_dice.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_f1_score.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_mcc.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_precision.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_recall.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_eval_essential.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_test_essential.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_trace.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_train_essential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.219324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/
--rw-r--r--   0 root         (0) root         (0)      702 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/test_label_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.219324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_img_data.py
--rw-r--r--   0 root         (0) root         (0)    11099 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.219324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.219324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.223324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.223324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.243324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_abs.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     6396 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_cast.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     8362 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_exp.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_gather.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_gather_from_batch.py
--rwxr-xr-x   0 root         (0) root         (0)     3742 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_iwd.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_maximum.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_permute.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_pow.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_roll.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_sign.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_watch.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_where.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.247324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/cli/test_cli_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.251324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_csv_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_data.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13000 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.251324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.251324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.255324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.255324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.255324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/loss/test_focal_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.255324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.259324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.267324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/test_numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.287324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.291324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.291324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.295324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     5249 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     3686 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_tensorop.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.295324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.295324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_golden_section_search.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_grid_search.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.299324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.299324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/logs/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/logs/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/test_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.299324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/test/test_unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.299324 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.303325 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/test_auc_score.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/test_bleu_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.303325 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    18690 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:23:26.307325 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/xai/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/xai/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-17 13:15:05.000000 fastestimator-nightly-1.5.0.dev202304171323/test/run_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.986497 fastestimator-nightly-1.6.0.dev202305310417/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-31 04:17:47.986497 fastestimator-nightly-1.6.0.dev202305310417/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.674508 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.674508 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.678508 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7452 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/unet.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.678508 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/unet.py
+-rw-r--r--   0 root         (0) root         (0)     5580 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.706507 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/
+-rw-r--r--   0 root         (0) root         (0)    10420 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_cast.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_concat.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_convert_tensor_precision.py
+-rw-r--r--   0 root         (0) root         (0)     7866 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_flip.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_gather_from_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_shape.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_huber.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_roll.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_save_model.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_smooth_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     5742 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_update_model.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_watch.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_where.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.710507 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/history.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.718507 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16450 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/combined_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/csv_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.730506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifair10.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifair100.py
+-rw-r--r--   0 root         (0) root         (0)     3511 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifar10.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifar100.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/em_3d.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/food101.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/horse2zebra.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/imdb_review.py
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/medmnist.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mendeley.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mitmovie_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/montgomery.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mscoco.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/nih_chestxray.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/omniglot.py
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/pascal_voc.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/penn_treebank.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/shakespeare.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/skl_digits.py
+-rw-r--r--   0 root         (0) root         (0)     6097 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/svhn.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/svhn_cropped.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/tednmt.py
+-rw-r--r--   0 root         (0) root         (0)     4183 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/tiny_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/usps.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    26096 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/op_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/siamese_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    32327 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.730506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.734506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.734506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/reflection_padding_2d.py
+-rw-r--r--   0 root         (0) root         (0)    51046 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.734506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.738506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.738506 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.754505 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/affine.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/crop.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/flip.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/multivariate.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/read_mat.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/resize.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     6186 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/transpose.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)    16330 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.778504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/binarize.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/blur.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/brightness.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/calibate.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/clahe.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/color.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/equalize.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/from_float.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/onehot.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/posterize.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/read_image.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/rua.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/solarize.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/univariate.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/word_to_id.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.782504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/argmax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.782504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/cutmix_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/mixup_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/average.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.786504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.790504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/dice_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/hinge.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     9186 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.794504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.794504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    12067 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/update.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/permute.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)    35579 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.794504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10488 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.798504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/golden_section.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     9239 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.802504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/cartesian.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/parallel_coordinate_plot.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/vis_util.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.806504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41454 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.806504 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/log_parse.py
+-rw-r--r--   0 root         (0) root         (0)    33817 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/log_plot.py
+-rw-r--r--   0 root         (0) root         (0)     9909 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/summary.py
+-rw-r--r--   0 root         (0) root         (0)    18174 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.810503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/nightly_util.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.810503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.814503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.822503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/grid_display.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)    23754 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    22579 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/test_report.py
+-rw-r--r--   0 root         (0) root         (0)    41429 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.822503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/meta/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/meta/_per_ds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.830503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/auc.py
+-rw-r--r--   0 root         (0) root         (0)    10591 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/bleu_score.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/dice.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/mcc.py
+-rw-r--r--   0 root         (0) root         (0)    18372 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/precision.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/recall.py
+-rw-r--r--   0 root         (0) root         (0)    21156 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/trace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.834503 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10667 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/eigen_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7808 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/grad_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/label_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.842502 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25329 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/base_util.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/cli_util.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/data.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/google_download_util.py
+-rw-r--r--   0 root         (0) root         (0)    31984 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/img_data.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/latex_util.py
+-rw-r--r--   0 root         (0) root         (0)    58364 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    17105 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/util.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.842502 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/xai/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.986497 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35102 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-31 04:17:47.000000 fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:17:47.986497 fastestimator-nightly-1.6.0.dev202305310417/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.842502 fastestimator-nightly-1.6.0.dev202305310417/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.842502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.846502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.850502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_save_model_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_update_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.850502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.850502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/dataset/test_batch_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.854502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.854502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.854502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.854502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.858502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.858502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.858502 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.862501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.862501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)    10341 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.866501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.866501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
+-rw-r--r--   0 root         (0) root         (0)    22429 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_average.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.870501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_arc.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    14280 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.870501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.870501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/visualize/test_visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.874501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)    17978 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/test_system.py
+-rw-r--r--   0 root         (0) root         (0)    23833 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    28311 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_network.py
+-rw-r--r--   0 root         (0) root         (0)    98463 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.878501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.878501 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.886500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4498 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     8180 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_test_report.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.890500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_dice.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_mcc.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_recall.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_eval_essential.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_test_essential.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_train_essential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.890500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/test_label_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.894500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_img_data.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.894500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.894500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.898500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.898500 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.922499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_cast.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_concat.py
+-rw-r--r--   0 root         (0) root         (0)     8362 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_gather_from_batch.py
+-rwxr-xr-x   0 root         (0) root         (0)     3742 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_roll.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_watch.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_where.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.922499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/cli/test_cli_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.926499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_combine_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_csv_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.926499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.930499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.930499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.930499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.930499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/loss/test_focal_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.934499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.934499 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.946498 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/test_numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.966498 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.970497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.970497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.970497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     7142 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.974497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.974497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_golden_section_search.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.978497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.978497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/logs/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/test_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.978497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/test/test_unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.978497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.978497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/test_auc_score.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/test_bleu_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.982497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    18690 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:17:47.982497 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/xai/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/xai/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-05-31 04:06:17.000000 fastestimator-nightly-1.6.0.dev202305310417/test/run_pr_test.py
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202305310417/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.5.0.dev202304171323
+Version: 1.6.0.dev202305310417
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
-Author-email: UNKNOWN
 License: Apache License 2.0
-Description: FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
+License-File: LICENSE
+
+FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/README.md` & `fastestimator-nightly-1.6.0.dev202305310417/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,132 +1,144 @@
 # FastEstimator
+
 <p align="center">
   <img src="https://github.com/fastestimator-util/fastestimator-misc/blob/master/resource/pictures/icon.png?raw=true" title="we are cool">
 </p>
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-informational.svg)](LICENSE)
 [![Build Status](http://jenkins.fastestimator.org:8080/buildStatus/icon?subject=PR-build&job=fastestimator%2Ffastestimator%2Fmaster)](http://jenkins.fastestimator.org:8080/job/fastestimator/job/fastestimator/job/master/)
 [![Build Status](http://jenkins.fastestimator.org:8080/buildStatus/icon?subject=nightly-build&job=nightly)](http://jenkins.fastestimator.org:8080/job/nightly/)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3a46ea86b8f04caab271f2a7bd6f4bd9)](https://www.codacy.com/gh/fastestimator/fastestimator/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=fastestimator/fastestimator&amp;utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/3a46ea86b8f04caab271f2a7bd6f4bd9)](https://www.codacy.com/gh/fastestimator/fastestimator/dashboard?utm_source=github.com&utm_medium=referral&utm_content=fastestimator/fastestimator&utm_campaign=Badge_Coverage)
 [![PyPI version](https://badge.fury.io/py/fastestimator.svg)](https://pypi.org/project/fastestimator/)
 [![PyPI stable Download](https://img.shields.io/pypi/dm/fastestimator?label=stable%20downloads&color=16D1B4)](https://pypistats.org/packages/fastestimator)
 [![PyPI stable Download](https://img.shields.io/pypi/dm/fastestimator-nightly?label=nightly%20downloads&color=16D1B4)](https://pypistats.org/packages/fastestimator-nightly)
 
-
 FastEstimator is a high-level deep learning library built on TensorFlow2 and PyTorch. With the help of FastEstimator, you can easily build a high-performance deep learning model and run it anywhere. :wink:
 
 For more information, please visit our [website](https://www.fastestimator.org/).
 
-## Installation:
-### Prerequisites
-* Python >=3.7
-* Nvidia Driver >= 450 (GPU only)
-* CUDA >= 11.0 (GPU only)
+## Support Matrix
+
+| FastEstimator  | Python | TensorFlow | PyTorch | CUDA |  Installation Instruction |
+| -------------  | ------  | --------- | ------- | ---- | ----------- |
+| Nightly  | 3.8-3.10  | 2.11.1 | 2.0.1 | 11.8 | master branch |
+| 1.5 (Stable)  | 3.7-3.9  | 2.9.1 | 1.10.2 | 11.0 | [r1.5 branch](https://github.com/fastestimator/fastestimator/tree/r1.5) |
+| 1.4  | 3.6-3.8  | 2.4.1 | 1.7.1 | 11.0 | [r1.4 branch](https://github.com/fastestimator/fastestimator/tree/r1.4) |
+| 1.3  | 3.6-3.8  | 2.4.1 | 1.7.1 | 11.0 | [r1.3 branch](https://github.com/fastestimator/fastestimator/tree/r1.3) |
+| 1.2  | 3.6-3.8  | 2.4.1 | 1.7.1 | 11.0 | [r1.2 branch](https://github.com/fastestimator/fastestimator/tree/r1.2) |
+| 1.1  | 3.6-3.8  | 2.3.0 | 1.6.0 | 10.1 | [r1.1 branch](https://github.com/fastestimator/fastestimator/tree/r1.1) |
 
-### 1. Install Dependencies:
+## Installation
+
+### 1. Install Dependencies
 
 * Install TensorFlow
-    * Linux/MAC:
-        ```bash
-        pip install tensorflow==2.9.1
-        ```
-    * Windows:
-        Please follow [this](https://github.com/fastestimator/fastestimator/blob/master/installation_docs/tensorflow_windows_installation.md) installation guide.
+  * Linux:
+
+      ```bash
+      pip install tensorflow==2.11.1
+      ```
+
+  * Mac (M1/M2):
+        Please follow this [installation guide](https://github.com/fastestimator/fastestimator/blob/master/installation_docs/mac_installation.md)
+
+  * Windows:
+        Please follow this [installation guide](https://github.com/fastestimator/fastestimator/blob/master/installation_docs/tensorflow_windows_installation.md)
 
 * Install PyTorch
-    * CPU:
-        ```bash
-        pip install torch==1.10.2 torchvision==0.11.3 torchaudio==0.10.2 -f https://download.pytorch.org/whl/cpu/torch_stable.html
-        ```
-    * GPU:
-        ```bash
-        pip install torch==1.10.2+cu113 torchvision==0.11.3+cu113 torchaudio==0.10.2+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
-        ```
+  * CPU:
+
+      ```bash
+      pip install torch==2.0.1+cpu torchvision==0.15.2+cpu torchaudio==2.0.2+cpu -f https://download.pytorch.org/whl/cpu/torch_stable.html
+      ```
+
+  * GPU:
+
+      ```bash
+      pip install torch==2.0.1+cu118 torchvision==0.15.2+cu118 torchaudio==2.0.2+cu118 -f https://download.pytorch.org/whl/cu118/torch_stable.html
+      ```
+
 * Extra Dependencies:
-    * Windows:
+  * Windows:
+    * Install Build Tools for Visual Studio 2019 [here](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019).
 
-        * Install Build Tools for Visual Studio 2019 [here](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019).
+    * Install latest Visual C++ redistributable [here](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) and choose x86 for 32 bit OS, x64 for 64 bit OS.
 
-        * Install latest Visual C++ redistributable [here](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) and choose x86 for 32 bit OS, x64 for 64 bit OS.
+  * Linux:
 
-    * Linux:
-        ``` bash
-        $ apt-get install libglib2.0-0 libsm6 libxrender1 libxext6
-        ```
+      ``` bash
+      apt-get install libglib2.0-0 libsm6 libxrender1 libxext6
+      ```
 
-    * Mac:
-        ``` bash
-        $ echo No extra dependency needed ":)"
-        ```
+  * Mac:
+    * Please follow this [installation guide](https://github.com/fastestimator/fastestimator/blob/master/installation_docs/mac_installation.md)
 
-### 2. Install FastEstimator:
-* Stable (Linux/Mac):
-    ``` bash
-    $ pip install fastestimator
-    ```
+### 2. Install FastEstimator
 
-* Stable (Windows):
+* Stable:
 
-    First download zip file from [available releases](https://github.com/fastestimator/fastestimator/releases)
     ``` bash
-    $ pip install fastestimator-x.x.x.zip
+    pip install fastestimator
     ```
 
 * Nightly (Linux/Mac):
-    ``` bash
-    $ pip install fastestimator-nightly
-    ```
-
-* Nightly (Windows):
 
-    First download zip file [here](https://github.com/fastestimator/fastestimator/archive/master.zip)
     ``` bash
-    $ pip install fastestimator-master.zip
+    pip install fastestimator-nightly
     ```
 
-
-
 ## Docker Hub
+
 Docker containers create isolated virtual environments that share resources with a host machine. Docker provides an easy way to set up a FastEstimator environment. You can simply pull our image from [Docker Hub](https://hub.docker.com/r/fastestimator/fastestimator/tags) and get started:
+
 * Stable:
-    * GPU:
-        ``` bash
-        docker pull fastestimator/fastestimator:latest-gpu
-        ```
-    * CPU:
-        ``` bash
-        docker pull fastestimator/fastestimator:latest-cpu
-        ```
+  * GPU:
+
+      ``` bash
+      docker pull fastestimator/fastestimator:latest-gpu
+      ```
+
+  * CPU:
+
+      ``` bash
+      docker pull fastestimator/fastestimator:latest-cpu
+      ```
+
 * Nighly:
-    * GPU:
-        ``` bash
-        docker pull fastestimator/fastestimator:nightly-gpu
-        ```
-    * CPU:
-        ``` bash
-        docker pull fastestimator/fastestimator:nightly-cpu
-        ```
+  * GPU:
+
+      ``` bash
+      docker pull fastestimator/fastestimator:nightly-gpu
+      ```
+
+  * CPU:
+
+      ``` bash
+      docker pull fastestimator/fastestimator:nightly-cpu
+      ```
+
+## Useful Links
 
-## Useful Links:
 * [Website](https://www.fastestimator.org): More info about FastEstimator API and news.
 * [Tutorial Series](https://github.com/fastestimator/fastestimator/tree/master/tutorial): Everything you need to know about FastEstimator.
 * [Application Hub](https://github.com/fastestimator/fastestimator/tree/master/apphub): End-to-end deep learning examples in FastEstimator.
 
-
-
 ## Citation
+
 Please cite FastEstimator in your publications if it helps your research:
+
 ```
 @misc{fastestimator,
   title  = {FastEstimator: A Deep Learning Library for Fast Prototyping and Productization},
   author = {Xiaomeng Dong and Junpyo Hong and Hsi-Ming Chang and Michael Potter and Aritra Chowdhury and
             Purujit Bahl and Vivek Soni and Yun-Chan Tsai and Rajesh Tamada and Gaurav Kumar and Caroline Favart and
             V. Ratna Saripalli and Gopal Avinash},
   note   = {NeurIPS Systems for ML Workshop},
   year   = {2019},
   url    = {http://learningsys.org/neurips19/assets/papers/10_CameraReadySubmission_FastEstimator_final_camera.pdf}
 }
 ```
 
 ## License
+
 [Apache License 2.0](https://github.com/fastestimator/fastestimator/blob/master/LICENSE)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     # Block the tkinter module from being imported on Mac. This is necessary in order for Mac multiprocessing to work,
     # since other modules such as nltk import tkinter, and it seems more likely that AI developers will need
     # multiprocessing than tkinter.
     sys.modules['tkinter'] = None
 
 # Fix known bugs with libraries which use multiprocessing in a way which conflicts with pytorch data loader
 import cv2
+
 cv2.setNumThreads(0)
 try:
     import SimpleITK as sitk
     sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(1)
 except ModuleNotFoundError:
     pass
 
@@ -45,15 +46,15 @@
 if TYPE_CHECKING:
     # Allow IDEs to play nice with lazy loading
     from fastestimator import architecture, backend, dataset, layers, op, schedule, search, summary, trace, util, xai
     from fastestimator.estimator import Estimator, enable_deterministic, record_history
     from fastestimator.network import Network, build
     from fastestimator.pipeline import Pipeline
 
-__version__ = '1.5.0'
+__version__ = '1.6.0'
 fe_deterministic_seed = None
 fe_history_path = None  # Where to save training histories. None for ~/fastestimator_data/history.db, False to disable
 fe_build_count = 0
 
 # Disable history logging for tests by default (they can still turn it on/off manually in setUpClass/tearDownClass)
 if __name__ != '__main__':
     for frame in inspect.stack()[1:]:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/lenet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/resnet9.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/pytorch/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/pytorch/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/lenet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/resnet9.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/architecture/tensorflow/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/architecture/tensorflow/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_abs.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_argmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_cast.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_check_nan.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_concat.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_convert_tensor_precision.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_convert_tensor_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_dice_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_exp.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_gather.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
             gradients = tape.gradient(target, sources)
     elif isinstance(target, torch.Tensor):
         gradients = torch.autograd.grad(target,
                                         sources,
                                         grad_outputs=torch.ones_like(target),
                                         retain_graph=retain_graph,
                                         create_graph=higher_order,
-                                        allow_unused=True,
-                                        only_inputs=True)
+                                        allow_unused=True)
 
         if isinstance(sources, torch.Tensor):
             #  The behavior table of tf and torch backend
             #  ---------------------------------------------------------------
             #        | case 1                     | case 2                    |
             #  ---------------------------------------------------------------|
             #  tf    | target: tf.Tensor          | target: tf.Tensor         |
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_lr.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_get_shape.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_get_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_hinge.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_huber.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_huber.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_iwd.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_iwd.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,12 @@
     """
     if eps is None:
         eps = np.array(pairwise_distance * math.pow((1.0 - max_prob) / (max_prob * (tensor.shape[-1] - 1)), 1 / power),
                        dtype=TENSOR_TO_NP_DTYPE[tensor.dtype])
         eps = to_tensor(
             eps, target_type='torch' if isinstance(tensor, torch.Tensor) else 'tf' if tf.is_tensor(tensor) else 'np')
         if isinstance(eps, torch.Tensor):
-            eps = eps.to("cuda:0" if torch.cuda.is_available() else "cpu")
+            eps = eps.to(tensor.device)
     tensor = maximum(tensor, eps)
     tensor = tensor_pow(1.0 / tensor, power)
     tensor = tensor / reshape(reduce_sum(tensor, axis=-1), shape=[-1, 1])
     return tensor
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_l1_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,13 +59,13 @@
     Raises:
         ValueError: If `y_pred` is an unacceptable data type.
     """
     if tf.is_tensor(y_pred):
         if tf.rank(y_pred) == 1:
             y_true = tf.expand_dims(y_true, axis=-1)
             y_pred = tf.expand_dims(y_pred, axis=-1)
-        mae = tf.losses.MAE(y_true,y_pred)
+        mae = tf.losses.MAE(y_true, y_pred)
     elif isinstance(y_pred, torch.Tensor):
         mae = reduce_mean(torch.nn.L1Loss(reduction="none")(y_pred, y_true), axis=-1)
     else:
         raise ValueError("Unrecognized tensor type {}".format(type(y_pred)))
     return mae
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_lambertw.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_load_model.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_matmul.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_maximum.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_ones_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_percentile.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_permute.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_pow.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_resize3d.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_roll.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_save_model.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_save_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,19 @@
         model.save_weights(model_path)
         if save_architecture:
             model.save(filepath=os.path.join(save_dir, model_name), include_optimizer=save_optimizer)
         if save_optimizer:
             assert model.current_optimizer, "optimizer does not exist"
             optimizer_path = os.path.join(save_dir, "{}_opt.pkl".format(model_name))
             with open(optimizer_path, 'wb') as f:
-                saved_data = {'weights': model.current_optimizer.get_weights(), 'lr': get_lr(model)}
+                saved_data = {'lr': get_lr(model)}
+                if hasattr(model.current_optimizer, 'get_weights'):
+                    saved_data['weights'] = model.current_optimizer.get_weights()
+                else:
+                    saved_data['weights'] = model.current_optimizer.variables()
                 if isinstance(model.current_optimizer, tfa.optimizers.DecoupledWeightDecayExtension) or hasattr(
                         model.current_optimizer, "inner_optimizer") and isinstance(
                             model.current_optimizer.inner_optimizer, tfa.optimizers.DecoupledWeightDecayExtension):
                     saved_data['weight_decay'] = tf.keras.backend.get_value(model.current_optimizer.weight_decay)
                 pickle.dump(saved_data, f)
         return model_path
     elif isinstance(model, torch.nn.Module):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_set_lr.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_sign.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_smooth_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_squeeze.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_shape.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Collection, TypeVar, Union
+from typing import Collection, TypeVar, Union, overload
 
 import numpy as np
 import tensorflow as tf
 import torch
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor, np.ndarray)
+CollectionT = TypeVar('CollectionT', bound=Collection)
 
 
-def to_tensor(data: Union[Collection, Tensor, float, int, None],
-              target_type: str,
+@overload
+def to_tensor(data: CollectionT, target_type: str, shared_memory: bool = False) -> CollectionT:
+    ...
+
+
+@overload
+def to_tensor(data: Union[Tensor, float, int], target_type: str, shared_memory: bool = False) -> Tensor:
+    ...
+
+
+@overload
+def to_tensor(data: None, target_type: str, shared_memory: bool = False) -> None:
+    ...
+
+
+def to_tensor(data: Union[Collection, Tensor, float, int, None], target_type: str,
               shared_memory: bool = False) -> Union[Collection, Tensor, None]:
     """Convert tensors within a collection of `data` to a given `target_type` recursively.
 
     This method can be used with Numpy data:
     ```python
     data = {"x": np.ones((10,15)), "y":[np.ones((4)), np.ones((5, 3))], "z":{"key":np.ones((2,2))}}
     t = fe.backend.to_tensor(data, target_type='tf')
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_to_type.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_update_model.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_update_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 from typing import Callable, Dict, List, Optional, Union
 
 import tensorflow as tf
 import torch
 
+from fastestimator.util.base_util import warn
 
 _ALREADY_GAVE_FE_GRAD_WARNING = False
 
 
 def update_model(model: Union[tf.keras.Model, torch.nn.Module],
                  gradients: List[Union[tf.Tensor, torch.Tensor]],
                  defer: bool = False,
@@ -77,16 +78,16 @@
 
     elif isinstance(model, torch.nn.Module):
         trainable_params = [p for p in model.parameters() if p.requires_grad]
         for gradient, parameter in zip(gradients, trainable_params):
             if gradient is None:
                 global _ALREADY_GAVE_FE_GRAD_WARNING
                 if not _ALREADY_GAVE_FE_GRAD_WARNING:
-                    print("\033[93m{}\033[00m".format("FastEstimator-Warn: 'None' detected in gradients. Some or all "
-                                                      "of your computation graph may not be connected to your loss."))
+                    warn("'None' detected in gradients. Some or all of your computation graph may not be connected " +
+                         "to your loss.")
                     _ALREADY_GAVE_FE_GRAD_WARNING = True
                 continue
             if parameter.grad is not None:
                 parameter.grad += gradient
             else:
                 parameter.grad = gradient.clone()
         if defer:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_watch.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_where.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/backend/_zscore.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/backend/_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/history.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/logs.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/logs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/main.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/plot.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/run.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/run.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/cli/train.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,36 @@
 # limitations under the License.
 # ==============================================================================
 # FEDataset, OpDataset, and FEDataLoader intentionally not imported here to reduce user confusion with auto-complete
 from typing import TYPE_CHECKING
 
 import lazy_loader as lazy
 
-__getattr__, __dir__, __all__ = lazy.attach(__name__,
-                                            submodules={'data'},
-                                            submod_attrs={'batch_dataset': ['BatchDataset'],
-                                                          'csv_dataset': ['CSVDataset'],
-                                                          'dir_dataset': ['DirDataset'],
-                                                          'generator_dataset': ['GeneratorDataset'],
-                                                          'labeled_dir_dataset': ['LabeledDirDataset'],
-                                                          'numpy_dataset': ['NumpyDataset'],
-                                                          'pickle_dataset': ['PickleDataset'],
-                                                          'siamese_dir_dataset': ['SiameseDirDataset'],
-                                                          'extend_dataset': ['ExtendDataset'], })
+__getattr__, __dir__, __all__ = lazy.attach(
+    __name__,
+    submodules={"data"},
+    submod_attrs={
+        "batch_dataset": ["BatchDataset"],
+        "csv_dataset": ["CSVDataset"],
+        "dir_dataset": ["DirDataset"],
+        "generator_dataset": ["GeneratorDataset"],
+        "labeled_dir_dataset": ["LabeledDirDataset"],
+        "numpy_dataset": ["NumpyDataset"],
+        "pickle_dataset": ["PickleDataset"],
+        "siamese_dir_dataset": ["SiameseDirDataset"],
+        "extend_dataset": ["ExtendDataset"],
+        "combined_dataset": ["CombinedDataset"],
+    },
+)
 
 if TYPE_CHECKING:
     from fastestimator.dataset import data
     from fastestimator.dataset.batch_dataset import BatchDataset
+    from fastestimator.dataset.combined_dataset import CombinedDataset
     from fastestimator.dataset.csv_dataset import CSVDataset
     from fastestimator.dataset.dir_dataset import DirDataset
+    from fastestimator.dataset.extend_dataset import ExtendDataset
     from fastestimator.dataset.generator_dataset import GeneratorDataset
     from fastestimator.dataset.labeled_dir_dataset import LabeledDirDataset
     from fastestimator.dataset.numpy_dataset import NumpyDataset
     from fastestimator.dataset.pickle_dataset import PickleDataset
     from fastestimator.dataset.siamese_dir_dataset import SiameseDirDataset
-    from fastestimator.dataset.extend_dataset import ExtendDataset
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/batch_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import random
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
 import numpy as np
 
 from fastestimator.dataset.dataset import DatasetSummary, FEDataset
 from fastestimator.dataset.extend_dataset import ExtendDataset
+from fastestimator.util.base_util import to_list, warn
 from fastestimator.util.traceability_util import traceable
-from fastestimator.util.base_util import to_list
 
 
 @traceable()
 class BatchDataset(FEDataset):
     """BatchDataset extracts a list (batch) of data from a single dataset or multiple datasets.
 
     This dataset helps to enable several use-cases:
@@ -206,15 +206,15 @@
 
     def summary(self) -> DatasetSummary:
         """Generate a summary representation of this dataset.
         Returns:
             A summary representation of this dataset.
         """
         if not self.all_fe_datasets:
-            print("FastEstimator-Warn: BatchDataset summary will be incomplete since non-FEDatasets were used.")
+            warn("BatchDataset summary will be incomplete since non-FEDatasets were used.")
             return DatasetSummary(num_instances=len(self), keys={})
         summaries = [ds.summary() for ds in self.datasets]
         keys = {k: v for summary in summaries for k, v in summary.keys.items()}
         return DatasetSummary(num_instances=len(self), keys=keys)
 
     def __len__(self) -> int:
         """Compute the length of this dataset.
@@ -276,16 +276,16 @@
             A list of data instance dictionaries corresponding to the current `batch_idx`.
         """
         if self.probability:
             index = list(np.random.choice(range(len(self.datasets)), size=self.num_samples, p=self.probability))
             num_samples = [index.count(i) for i in range(len(self.datasets))]
         else:
             num_samples = self.num_samples
-        indices = [[index_map[batch_idx * num_sample + idx] for idx in range(num_sample)] for num_sample, index_map
-                   in zip(num_samples, self.index_maps)]
+        indices = [[index_map[batch_idx * num_sample + idx] for idx in range(num_sample)] for num_sample,
+                   index_map in zip(num_samples, self.index_maps)]
         return indices
 
     def fe_reset_ds(self, shuffle: bool = True, *, seed: Optional[int] = None) -> None:
         """Rearrange the index maps of this BatchDataset.
 
         Args:
             shuffle: Whether to shuffle the dataset. If False the method will do nothing so long as index maps already
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 import lazy_loader as lazy
 
 __getattr__, __dir__, __all__ = lazy.attach(__name__,
                                             submodules={'breast_cancer', 'cifair10', 'cifair100', 'cifar10',
                                                         'cifar100', 'cub200','em_3d', 'food101', 'horse2zebra', 'imdb_review',
                                                         'mendeley', 'mitmovie_ner', 'mnist', 'montgomery', 'mscoco',
                                                         'nih_chestxray', 'omniglot', 'penn_treebank', 'shakespeare',
-                                                        'skl_digits', 'svhn', 'svhn_cropped', 'tednmt', 'usps', 'pascal_voc'}
+                                                        'skl_digits', 'svhn', 'svhn_cropped', 'tednmt', 'usps', 'pascal_voc', 'medmnist'}
                                             )
 
 if TYPE_CHECKING:
     from fastestimator.dataset.data import breast_cancer, cifair10, cifair100, cifar10, cifar100, cub200, em_3d, \
         food101, horse2zebra, imdb_review, mendeley, mitmovie_ner, mnist, montgomery, mscoco, nih_chestxray, omniglot, \
-        penn_treebank, shakespeare, skl_digits, svhn, svhn_cropped, tednmt, usps, pascal_voc
+        penn_treebank, shakespeare, skl_digits, svhn, svhn_cropped, tednmt, usps, pascal_voc, medmnist
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/breast_cancer.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifair10.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifair10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifair100.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifair100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifar10.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifar10.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from typing import Tuple
 
 import numpy as np
 from keras.datasets.cifar import load_batch
 
 from fastestimator.dataset.numpy_dataset import NumpyDataset
+from fastestimator.util.base_util import warn
 from fastestimator.util.google_download_util import _download_file_from_google_drive
 
 
 def load_data(root_dir: str = None, image_key: str = "x", label_key: str = "y",
               channels_last: bool = True) -> Tuple[NumpyDataset, NumpyDataset]:
     """Load and return the CIFAR10 dataset.
 
@@ -36,15 +37,15 @@
         image_key: The key for image.
         label_key: The key for label.
         channels_last: Whether channel is last
 
     Returns:
         (train_data, eval_data)
     """
-    print("\033[93m {}\033[00m".format("FastEstimator-Warn: Consider using the ciFAIR10 dataset instead."))
+    warn("Consider using the ciFAIR10 dataset instead.")
     home = str(Path.home())
 
     if root_dir is None:
         root_dir = os.path.join(home, 'fastestimator_data', 'cifar10')
     else:
         root_dir = os.path.join(os.path.abspath(root_dir), 'cifar10')
     os.makedirs(root_dir, exist_ok=True)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cifar100.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cifar100.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from typing import Tuple
 
 import numpy as np
 from keras.datasets.cifar import load_batch
 
 from fastestimator.dataset.numpy_dataset import NumpyDataset
+from fastestimator.util.base_util import warn
 from fastestimator.util.google_download_util import _download_file_from_google_drive
 
 
 def load_data(root_dir: str = None,
               image_key: str = "x",
               label_key: str = "y",
               label_mode: str = "fine",
@@ -43,15 +44,15 @@
 
     Returns:
         (train_data, eval_data)
 
     Raises:
         ValueError: If the label_mode is invalid.
     """
-    print("\033[93m {}\033[00m".format("FastEstimator-Warn: Consider using the ciFAIR100 dataset instead."))
+    warn("Consider using the ciFAIR100 dataset instead.")
     if label_mode not in ['fine', 'coarse']:
         raise ValueError("label_mode must be one of either 'fine' or 'coarse'.")
     home = str(Path.home())
 
     if root_dir is None:
         root_dir = os.path.join(home, 'fastestimator_data', 'cifar100')
     else:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/cub200.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/cub200.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/em_3d.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/em_3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/food101.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/food101.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/horse2zebra.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/imdb_review.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/imdb_review.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mendeley.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mendeley.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mitmovie_ner.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mitmovie_ner.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,12 +92,12 @@
 
     x_train, y_train, x_vocab, y_vocab = get_sentences_and_labels(train_data_path)
     x_eval, y_eval, x_eval_vocab, y_eval_vocab = get_sentences_and_labels(test_data_path)
     x_vocab |= x_eval_vocab
     y_vocab |= y_eval_vocab
     x_train = np.array(x_train)
     x_eval = np.array(x_eval)
-    y_train = np.array(y_train)
-    y_eval = np.array(y_eval)
+    y_train = np.array(y_train, dtype=object)
+    y_eval = np.array(y_eval, dtype=object)
     train_data = NumpyDataset({"x": x_train, "y": y_train})
     eval_data = NumpyDataset({"x": x_eval, "y": y_eval})
     return train_data, eval_data, x_vocab, y_vocab
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mnist.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/montgomery.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/montgomery.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/mscoco.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/mscoco.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import wget
 from pycocotools.coco import COCO
 
 from fastestimator.dataset.dir_dataset import DirDataset
-from fastestimator.util.base_util import Suppressor
 from fastestimator.util.traceability_util import traceable
+from fastestimator.util.util import Suppressor
 from fastestimator.util.wget_util import bar_custom, callback_progress
 
 wget.callback_progress = callback_progress
 
 
 @traceable()
 class MSCOCODataset(DirDataset):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/nih_chestxray.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/nih_chestxray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/omniglot.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/omniglot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/pascal_voc.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/penn_treebank.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/penn_treebank.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/shakespeare.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/skl_digits.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/skl_digits.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/svhn.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/svhn.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/svhn_cropped.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/svhn_cropped.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/tednmt.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/tednmt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/tiny_imagenet.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/data/usps.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/data/usps.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Optional, Tuple
 
 import numpy as np
 import wget
 from PIL import Image
 
 from fastestimator.dataset.labeled_dir_dataset import LabeledDirDataset
+from fastestimator.util.google_download_util import _download_file_from_google_drive
 from fastestimator.util.util import cpu_count
 from fastestimator.util.wget_util import bar_custom, callback_progress
 
 wget.callback_progress = callback_progress
 
 
 def _write_image(image: np.ndarray, path: str, idx: int, mode: str) -> None:
@@ -108,25 +109,21 @@
     test_compressed_path = os.path.join(root_dir, "zip.test.gz")
     train_base_path = os.path.join(root_dir, "train")
     test_base_path = os.path.join(root_dir, "test")
 
     if not os.path.exists(train_base_path):
         if not os.path.exists(train_compressed_path):
             print("Downloading train data to {}".format(root_dir))
-            wget.download('http://statweb.stanford.edu/~tibs/ElemStatLearn/datasets/zip.train.gz',
-                          root_dir,
-                          bar=bar_custom)
+            _download_file_from_google_drive("1NlaCnlhV-PA_Rek8w8eQqJUeYCZJ0olG", train_compressed_path)
         train_images, train_labels = _extract_images_labels(train_compressed_path)
         _write_data(train_images, train_labels, train_base_path, "train")
 
     if not os.path.exists(test_base_path):
         if not os.path.exists(test_compressed_path):
             print("Downloading test data to {}".format(root_dir))
-            wget.download('http://statweb.stanford.edu/~tibs/ElemStatLearn/datasets/zip.test.gz',
-                          root_dir,
-                          bar=bar_custom)
+            _download_file_from_google_drive("1lagM-V1nmAdS3Uz9Uk4bB9cKqE_agt59", test_compressed_path)
         test_images, test_labels = _extract_images_labels(test_compressed_path)
         _write_data(test_images, test_labels, test_base_path, "test")
 
     # make datasets
     return LabeledDirDataset(train_base_path, file_extension=".png"), LabeledDirDataset(test_base_path,
                                                                                         file_extension=".png")
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dataloader.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,20 @@
 from torch.utils.data._utils.collate import default_collate, default_convert
 from torch.utils.data._utils.fetch import _MapDatasetFetcher
 from torch.utils.data.dataloader import _BaseDataLoaderIter, _MultiProcessingDataLoaderIter, \
     _SingleProcessDataLoaderIter
 
 from fastestimator.dataset.extend_dataset import ExtendDataset
 from fastestimator.dataset.op_dataset import OpDataset
-from fastestimator.util.base_util import Suppressor
 from fastestimator.util.data import FilteredData
+from fastestimator.util.util import Suppressor
+
+
+class SizedDataset(Dataset, Sized):
+    pass
 
 
 class FEDataLoader(DataLoader):
     """A Data Loader that can handle filtering data.
 
     This class is intentionally not @traceable.
 
@@ -60,21 +64,21 @@
     _current_threads = []
     FE_LOADER_KIND = 7
 
     # The typing for 'dataset' should be an 'and' rather than 'or' but that feature is still under development:
     # https://github.com/python/typing/issues/213
 
     def __init__(self,
-                 dataset: Union[Dataset, Sized],
+                 dataset: SizedDataset,
                  postprocess_fn: Optional[Callable[[Dict[str, Any]], Union[Dict[str, Any], FilteredData]]] = None,
                  batch_size: Optional[int] = 1,
                  steps_per_epoch: Optional[int] = None,
                  shuffle: bool = False,
                  num_workers: int = 0,
-                 collate_fn: Callable = None,
+                 collate_fn: Optional[Callable] = None,
                  drop_last: bool = False):
         reset_fn = dataset.fe_reset_ds if hasattr(dataset, 'fe_reset_ds') else None
         convert_fn = dataset.fe_batch_indices if hasattr(dataset, 'fe_batch_indices') else None
         sampler = InfiniteSampler(data_source=dataset, shuffle=shuffle, reset_fn=reset_fn, convert_fn=convert_fn)
         if batch_size is not None and batch_size < 1:
             raise ValueError(f"batch_size must be None or a positive integer, but got {batch_size}")
         # Figure out the real batch size. This is already done in OpDataset, but if user manually instantiates this
@@ -196,15 +200,14 @@
 
 class _BaseFELoaderIter(_BaseDataLoaderIter, ABC):
     """A base class for the FE Data iterators.
 
     Args:
         loader: The parent loader object that will own this iterator.
     """
-
     def __init__(self, loader: FEDataLoader):
         super().__init__(loader)
         self.fe_batch_size = loader.fe_batch_size
         self.fe_drop_last = loader.fe_drop_last
         self.fe_collate_fn = loader.fe_collate_fn
         self.fe_postprocess_fn = loader.fe_postprocess_fn
         self.fe_samples_to_yield = loader.fe_samples_to_yield
@@ -347,21 +350,20 @@
         data_source: The dataset to be sampled.
         shuffle: Whether to shuffle when sampling.
         reset_fn: A function to be invoked (using the provided `shuffle` arg) every time the dataset has been fully
             traversed.
         convert_fn: A function to be invoked (using the current index) every sample in order to convert an integer index
             into some arbitrary alternative index representation.
     """
-
     def __init__(self,
                  data_source: Sized,
                  shuffle: bool = True,
                  reset_fn: Optional[Callable[[bool], None]] = None,
                  convert_fn: Optional[Callable[[int], Any]] = None):
-        super().__init__(data_source=data_source)
+        super().__init__(data_source=None)  # Arg is unused and triggers a warning in torch 2.1
         self.ds_len = len(data_source)
         if self.ds_len < 1:
             raise ValueError("dataset length must be at least 1")
         self.indices = [i for i in range(self.ds_len)]
         self.shuffle = shuffle
         self.reset_fn = reset_fn
         self.convert_fn = convert_fn
@@ -396,15 +398,14 @@
 # Here we use a hack to patch a special fetcher into the pytorch ecosystem. This allows us to return the dataset indices
 # alongside the collated data points in case the batch needs to be re-constructed later. It won't interfere with regular
 # pytorch usage since our reserved 'kind' value is 7 whereas pytorch only uses 0 and 1.
 ###
 
 
 class _IdxMapDatasetFetcher(_MapDatasetFetcher):
-
     def fetch(self, possibly_batched_index):
         if self.auto_collation:
             data = [self.dataset[idx] for idx in possibly_batched_index]
         else:
             data = self.dataset[possibly_batched_index]
         return possibly_batched_index, self.collate_fn(data)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import math
 import random
 from collections import defaultdict
 from copy import deepcopy
-from typing import Any, Dict, Hashable, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Hashable, Iterable, List, Optional, Sequence, Tuple, Union, cast, overload
 
 import jsonpickle
 import numpy as np
 from torch.utils.data import Dataset
+from typing_extensions import Self
 
+from fastestimator.util.base_util import FEID, get_shape, get_type
 from fastestimator.util.traceability_util import FeSplitSummary, traceable
-from fastestimator.util.base_util import get_type, FEID, get_shape
 
 
 class KeySummary:
     """A summary of the dataset attributes corresponding to a particular key.
 
     This class is intentionally not @traceable.
 
@@ -37,17 +38,18 @@
             ragged.
         dtype: The data type of instances corresponding to the given key.
     """
     num_unique_values: Optional[int]
     shape: List[Optional[int]]
     dtype: str
 
-    def __init__(self, dtype: str, num_unique_values: Optional[int] = None, shape: List[Optional[int]] = ()) -> None:
+    def __init__(self, dtype: str, num_unique_values: Optional[int] = None,
+                 shape: Sequence[Optional[int]] = ()) -> None:
         self.num_unique_values = num_unique_values
-        self.shape = shape
+        self.shape = list(shape)
         self.dtype = dtype
 
     def __repr__(self):
         return "<KeySummary {}>".format(self.__getstate__())
 
     def __getstate__(self):
         return {k: v for k, v in self.__dict__.items() if v is not None}
@@ -166,18 +168,37 @@
                                     seed=seed,
                                     stratify=stratify)
             table.fields['split'] = split_summary
             # Put the new parent summary into the child table to ensure it will always exist in the final set of tables
             for child in children:
                 child._fe_traceability_summary[parent_id] = deepcopy(table)
 
+    @overload
+    def split(self,
+              __fraction1: Union[float, int, Iterable[int]],
+              /,
+              *,
+              seed: Optional[int] = None,
+              stratify: Optional[str] = None) -> Self:
+        ...
+
+    @overload
+    def split(self,
+              __fraction1: Union[float, int, Iterable[int]],
+              __fraction2: Union[float, int, Iterable[int]],
+              /,
+              *fractions: Union[float, int, Iterable[int]],
+              seed: Optional[int] = None,
+              stratify: Optional[str] = None) -> List[Self]:
+        ...
+
     def split(self,
               *fractions: Union[float, int, Iterable[int]],
               seed: Optional[int] = None,
-              stratify: Optional[str] = None) -> Union['FEDataset', List['FEDataset']]:
+              stratify: Optional[str] = None) -> Union[Self, List[Self]]:
         """Split this dataset into multiple smaller datasets.
 
         This function enables several types of splitting:
         1. Splitting by fractions.
             ```python
             ds = fe.dataset.FEDataset(...)  # len(ds) == 1000
             ds2 = ds.split(0.1)  # len(ds) == 900, len(ds2) == 100
@@ -248,15 +269,15 @@
         if method == 'number':
             if stratify is not None:
                 splits = self._get_stratified_splits(n_samples, seed, stratify)
             else:
                 splits = self._get_fractional_splits(n_samples, seed)
         else:  # method == 'indices':
             assert stratify is None, "Stratify may only be specified when splitting by count or fraction, not by index"
-            splits = fractions
+            splits = cast(Sequence[Iterable[int]], fractions)
         splits = self._do_split(splits)
         FEDataset.fix_split_traceabilty(self, splits, fractions, seed, stratify)
         if len(fractions) == 1:
             return splits[0]
         return splits
 
     def _get_stratified_splits(self, split_counts: List[int], seed: Optional[int],
@@ -375,15 +396,15 @@
         Useful if sub-classes want to split by something other than indices (see SiameseDirDataset for example).
 
         Returns:
             The apparent length of the dataset for the purpose of the .split() function
         """
         return len(self)
 
-    def _do_split(self, splits: Sequence[Iterable[int]]) -> List['FEDataset']:
+    def _do_split(self, splits: Sequence[Iterable[int]]) -> List[Self]:
         """Split the current dataset apart into several smaller datasets.
 
         Args:
             splits: Which indices to remove from the current dataset in order to create new dataset(s). One dataset will
                 be generated for every iterable within the `splits` sequence.
 
         Returns:
@@ -469,15 +490,15 @@
         else:
             assert len(value) == len(self.data), \
                 "input value must be of length {}, but had length {}".format(len(self.data), len(value))
             for i in range(len(self.data)):
                 self.data[i][key] = value[i]
         self._summary = None
 
-    def _skip_init(self, data: Dict[int, Dict[str, Any]], **kwargs) -> 'InMemoryDataset':
+    def _skip_init(self, data: Dict[int, Dict[str, Any]], **kwargs) -> Self:
         """A helper method to create new dataset instances without invoking their __init__ methods.
 
         Args:
             data: The data dictionary to be used in the new dataset.
             **kwargs: Any other member variables to be assigned in the new dataset.
 
         Returns:
@@ -486,15 +507,15 @@
         obj = self.__class__.__new__(self.__class__)
         obj.data = data
         for k, v in kwargs.items():
             obj.__setattr__(k, v)
         obj._summary = None
         return obj
 
-    def _do_split(self, splits: Sequence[Iterable[int]]) -> List['InMemoryDataset']:
+    def _do_split(self, splits: Sequence[Iterable[int]]) -> List[Self]:
         """Split the current dataset apart into several smaller datasets.
 
         Args:
             splits: Which indices to remove from the current dataset in order to create new dataset(s). One dataset will
                 be generated for every iterable within the `splits` sequence.
 
         Returns:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/generator_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any, Dict, Generator, Iterable, List, Optional, Sequence, Sized
 
 from fastestimator.dataset.dataset import DatasetSummary, FEDataset, KeySummary
+from fastestimator.util.base_util import get_shape, get_type, warn
 from fastestimator.util.traceability_util import traceable
-from fastestimator.util.base_util import get_type, get_shape
 
 
 @traceable(blacklist='_summary')
 class GeneratorDataset(FEDataset):
     """A dataset from a generator function.
 
     Args:
@@ -49,31 +49,30 @@
         Args:
             splits: Which indices to remove from the current dataset in order to create new dataset(s). One dataset will
                 be generated for every iterable within the `splits` sequence.
 
         Returns:
             New datasets generated by removing data at the indices specified by `splits` from the current dataset.
         """
-        print("FastEstimator-Warn: You probably don't actually want to split a generator dataset")
+        warn("You probably don't actually want to split a generator dataset")
         self._summary = None
         results = []
         for split in splits:
             if isinstance(split, Sized):
                 size = len(split)
             else:
                 # TODO - make this efficient somehow
                 size = sum(1 for _ in split)
             results.append(GeneratorDataset(self.generator, size))
             self.samples_per_epoch -= size
         return results
 
     def _get_stratified_splits(self, split_counts: List[int], seed: Optional[int],
                                stratify: str) -> Sequence[Iterable[int]]:
-        print("\033[93m {}\033[00m".format(
-            "Warning! GeneratorDataset does not support stratified splits. Falling back to classical split method."))
+        warn("GeneratorDataset does not support stratified splits. Falling back to classical split method.")
         return self._get_fractional_splits(split_counts=split_counts, seed=seed)
 
     def summary(self) -> DatasetSummary:
         """Generate a summary representation of this dataset.
         Returns:
             A summary representation of this dataset.
         """
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/op_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/op_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import ctypes
 from copy import deepcopy
-from multiprocessing import Lock
-from typing import Any, Dict, List, Mapping, Optional, Set, Union
+from multiprocessing import Array, Lock
+from typing import Any, Dict, List, Optional, Set, Union
 
 import numpy as np
+from natsort import humansorted
 from torch.utils.data import Dataset
 
 from fastestimator.op.numpyop.numpyop import NumpyOp, forward_numpyop
+from fastestimator.util.base_util import warn
 from fastestimator.util.data import FilteredData
 from fastestimator.util.traceability_util import traceable
 
 
 class _DelayedDeepDict(dict):
     """A class to perform delayed deep copying from another dictionary.
 
@@ -92,14 +95,17 @@
         self.base = {}
         # We need to mark all of the arrays as writeable again to avoid warnings from pytorch. Once torch wraps the
         # arrays, in-place edits on the torch tensors do not impact the numpy arrays anyways.
         for val in self.values():
             if isinstance(val, np.ndarray):
                 val.flags.writeable = True
 
+    def as_dict(self) -> Dict[str, Any]:
+        return dict(self)
+
 
 @traceable(blacklist='lock')
 class OpDataset(Dataset):
     """A wrapper for datasets which allows operators to be applied to them in a pipeline.
 
     This class should not be directly instantiated by the end user. The fe.Pipeline will automatically wrap datasets
     within an Op dataset as needed.
@@ -108,17 +114,14 @@
         dataset: The base dataset to wrap.
         ops: A list of ops to be applied after the base `dataset` `__getitem__` is invoked.
         mode: What mode the system is currently running in ('train', 'eval', 'test', or 'infer').
         output_keys: What keys can be produced from pipeline. If None or empty, all keys will be considered.
         deep_remainder: Whether data which is not modified by Ops should be deep copied or not. This argument is used to
             help with RAM management, but end users can almost certainly ignore it.
     """
-    to_warn: Set[str] = set()
-    warned: Set[str] = set()
-
     def __init__(self,
                  dataset: Dataset,
                  ops: List[NumpyOp],
                  mode: str,
                  output_keys: Optional[Set[str]] = None,
                  deep_remainder: bool = True) -> None:
         # Track whether this dataset returns batches or not (useful for pipeline and traceability)
@@ -132,16 +135,20 @@
         if hasattr(dataset, "fe_batch_indices"):
             self.fe_batch_indices = dataset.fe_batch_indices
         self.ops = ops
         self.mode = mode
         self.output_keys = output_keys
         self.deep_remainder = deep_remainder
         self.lock = Lock()
+        self.to_warn: Set[str] = set()
+        if not hasattr(OpDataset, 'warned'):
+            # Declaring this outside the init would trigger mac multi-processing to pick a non-fork start method
+            OpDataset.warned = Array(ctypes.c_char, 200, lock=False)
 
-    def __getitem__(self, index: int) -> Union[Mapping[str, Any], List[Mapping[str, Any]], FilteredData]:
+    def __getitem__(self, index: int) -> Union[Dict[str, Any], List[Dict[str, Any]], FilteredData]:
         """Fetch a data instance at a specified index, and apply transformations to it.
 
         Args:
             index: Which datapoint to retrieve.
 
         Returns:
             The data dictionary from the specified index, with transformations applied OR an indication that this index
@@ -157,32 +164,47 @@
                 if data_id not in unique_samples:
                     data = _DelayedDeepDict(data)
                     filter_data = forward_numpyop(self.ops, data, {'mode': self.mode})
                     if filter_data:
                         results.append(filter_data)
                     else:
                         data.finalize(retain=self.output_keys, deep_remainder=self.deep_remainder)
-                        results.append(data)
                         if data.warn:
-                            self.to_warn |= (data.to_warn - self.warned)
+                            self.to_warn |= data.to_warn
+                        results.append(data.as_dict())
                     unique_samples[data_id] = idx
                 else:
                     results.append(results[unique_samples[data_id]])
         else:
             results = _DelayedDeepDict(item)
             filter_data = forward_numpyop(self.ops, results, {'mode': self.mode})
             if filter_data:
                 return filter_data
             results.finalize(retain=self.output_keys, deep_remainder=self.deep_remainder)
             if results.warn:
-                self.to_warn |= (results.to_warn - self.warned)
+                self.to_warn |= results.to_warn
+            results = results.as_dict()
         if self.to_warn and self.lock.acquire(block=False):
-            self.warned.update(self.to_warn)
-            print("FastEstimator-Warn: The following key(s) are being pruned since they are unused outside of the "
-                  "Pipeline. To prevent this, you can declare the key(s) as inputs to Traces or TensorOps: "
-                  f"{', '.join(self.to_warn)}")
-            self.to_warn.clear()
+            # Keys can't contain the ":" or ";" character due to check_io_names base_util function
+            warned = set((str(OpDataset.warned.value, 'utf8') or "").split(":"))
+            if ";" not in warned:
+                # We use ; as a special character to indicate that the warned buffer was overflowed by too many keys
+                self.to_warn -= warned
+                if self.to_warn:
+                    warn("The following key(s) are being pruned since they are unused outside of the "
+                         "Pipeline. To prevent this, you can declare the key(s) as inputs to Traces or TensorOps: "
+                         f"{', '.join(humansorted(self.to_warn))}")
+                    warned |= self.to_warn
+                    self.to_warn.clear()
+                    warned = bytes(":".join(warned), 'utf8')
+                    if len(warned) > 198:
+                        # This would overflow the warning buffer, so disable the warning mechanism in the future
+                        # Note that the warning will still happen the first time the overly-long keys appear.
+                        # 198 rather than 199 to allow for a null terminator at the end of the array.
+                        warn("Any further key pruning warnings in subsequent epochs will not be printed.")
+                        warned = bytes(";", 'utf8')
+                    OpDataset.warned.value = warned
             # We intentionally never release the lock so that during multi-threading only 1 message can be printed
         return results
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/dataset/siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/dataset/siamese_dir_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from copy import deepcopy
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Tuple
 
 import numpy as np
 
 from fastestimator.dataset.dataset import DatasetSummary
 from fastestimator.dataset.labeled_dir_dataset import LabeledDirDataset
+from fastestimator.util.base_util import warn
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable(blacklist=('data', 'class_data', '_summary'))
 class SiameseDirDataset(LabeledDirDataset):
     """A dataset which returns pairs of data.
 
@@ -113,16 +114,15 @@
         self.class_data = self._data_to_class(self.data, self.label_key)
         # The summary function is being cached by a base class, so reset our cache here
         self._summary = None
         return results
 
     def _get_stratified_splits(self, split_counts: List[int], seed: Optional[int],
                                stratify: str) -> Sequence[Iterable[int]]:
-        print("\033[93m {}\033[00m".format(
-            "Warning! SiameseDirDataset does not support stratified splits. Falling back to classical split method."))
+        warn("SiameseDirDataset does not support stratified splits. Falling back to classical split method.")
         return self._get_fractional_splits(split_counts=split_counts, seed=seed)
 
     def __getitem__(self, index: int):
         """Extract items from the dataset based on the given `batch_idx`.
 
         Args:
             index: Which data instance to use as the 'left' element.
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/estimator.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import inspect
 import os
 import random
 from collections import ChainMap
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union, overload
 
 import numpy as np
 import tensorflow as tf
 import torch
 from tensorflow.python.distribute.input_lib import DistributedDataset
 from torch.utils.data import DataLoader
 
@@ -35,29 +35,27 @@
 from fastestimator.summary.system import Summary, System
 from fastestimator.trace.io.best_model_saver import BestModelSaver
 from fastestimator.trace.io.model_saver import ModelSaver
 from fastestimator.trace.io.restore_wizard import RestoreWizard
 from fastestimator.trace.io.traceability import Traceability
 from fastestimator.trace.trace import EvalEssential, Logger, PerDSTrace, TestEssential, Trace, TrainEssential, \
     sort_traces
-from fastestimator.util.base_util import NonContext, Suppressor, to_list, to_set
+from fastestimator.util.base_util import NonContext, to_list, to_set, warn
 from fastestimator.util.data import Data, FilteredData
 from fastestimator.util.traceability_util import traceable
-from fastestimator.util.util import draw
+from fastestimator.util.util import Suppressor, draw
 
 
 def _verify_dependency_versions() -> None:
     """Print warning messages if the user is using unexpected versions of TF or torch.
     """
-    if tf.__version__ != '2.9.1':
-        print("\033[93m{}\033[00m".format("FastEstimator-Warn: Expected TensorFlow version 2.9.1 but found "
-                                          f"{tf.__version__}. The framework may not work as expected."))
-    if torch.__version__ not in ('1.10.2', '1.10.2+cpu', '1.10.2+cu113'):
-        print("\033[93m{}\033[00m".format("FastEstimator-Warn: Expected PyTorch version 1.10.2 but found "
-                                          f"{torch.__version__}. The framework may not work as expected."))
+    if tf.__version__ not in {'2.11.1', '2.11.0'}:
+        warn(f"Expected TensorFlow version 2.11.1 but found {tf.__version__}. The framework may not work as expected.")
+    if torch.__version__ not in ('2.0.1', '2.0.1+cpu', '2.0.1+cu118'):
+        warn(f"Expected PyTorch version 2.0.1 but found {torch.__version__}. The framework may not work as expected.")
 
 
 @traceable()
 class Estimator:
     """One class to rule them all.
 
     Estimator is the highest level class within FastEstimator. It is the class which is invoked to actually train
@@ -121,14 +119,22 @@
     def network(self) -> BaseNetwork:
         return self.system.network
 
     @property
     def traces(self) -> List[Union[Trace, Scheduler[Trace]]]:
         return self.system.traces
 
+    @overload
+    def fit(self, summary: None = None, warmup: bool = True, eager: bool = False) -> None:
+        ...
+
+    @overload
+    def fit(self, summary: str, warmup: bool = True, eager: bool = False) -> Summary:
+        ...
+
     def fit(self, summary: Optional[str] = None, warmup: bool = True, eager: bool = False) -> Optional[Summary]:
         """Train the network for the number of epochs specified by the estimator's constructor.
 
         Args:
             summary: A name for the experiment. If provided, the log history will be recorded in-memory and returned as
                 a summary object at the end of training.
             warmup: Whether to perform warmup before training begins. The warmup procedure will test one step at every
@@ -172,23 +178,31 @@
         if "train" in run_modes:
             self.traces_in_use.insert(0, TrainEssential(monitor_names=self.monitor_names.union(extra_monitor_keys)))
             no_save_warning = True
             for trace in get_current_items(self.traces_in_use, run_modes=run_modes):
                 if isinstance(trace, (ModelSaver, BestModelSaver)):
                     no_save_warning = False
             if no_save_warning:
-                print("FastEstimator-Warn: No ModelSaver Trace detected. Models will not be saved.")
+                warn("No ModelSaver Trace detected. Models will not be saved.")
         if "eval" in run_modes and "eval" in self.pipeline.get_modes():
             self.traces_in_use.insert(1, EvalEssential(monitor_names=self.monitor_names.union(extra_monitor_keys)))
         if "test" in run_modes and "test" in self.pipeline.get_modes():
             self.traces_in_use.insert(0, TestEssential(monitor_names=self.monitor_names.union(extra_monitor_keys)))
         # insert system instance to trace
         for trace in get_current_items(self.traces_in_use, run_modes=run_modes):
             trace.system = self.system
 
+    @overload
+    def test(self, summary: None = None, eager: bool = False) -> None:
+        ...
+
+    @overload
+    def test(self, summary: str, eager: bool = False) -> Summary:
+        ...
+
     def test(self, summary: Optional[str] = None, eager: bool = False) -> Optional[Summary]:
         """Run the pipeline / network in test mode for one epoch.
 
         Args:
             summary: A name for the experiment. If provided, the log history will be recorded in-memory and returned as
                 a summary object at the end of training. If None, the default value will be whatever `summary` name was
                 most recently provided to this Estimator's .fit() or .test() methods.
@@ -242,18 +256,19 @@
                     with self.pipeline(mode=mode,
                                        epoch=epoch,
                                        ds_id=ds_id,
                                        steps_per_epoch=None,
                                        output_keys=trace_input_keys - network_output_keys
                                        | network_input_keys) as loader:
                         loader = self._configure_loader(loader)
-                        with Suppressor():
-                            if isinstance(loader, tf.data.Dataset):
-                                batch = list(loader.take(1))[0]
-                            else:
+                        if isinstance(loader, tf.data.Dataset):
+                            batch = list(loader.take(1))[0]
+                        else:
+                            with Suppressor(allow_pyprint=True, show_if_exception=True):
+                                # TF multi-gpu print-spams here in version 2.11
                                 batch = next(iter(loader))
                         batch = self._configure_tensor(loader, batch)
                     assert isinstance(batch, dict), "please make sure data output format is dictionary"
                     pipeline_output_keys = to_set(batch.keys())
 
                     monitor_names = monitor_names - (pipeline_output_keys | network_output_keys)
                     unmet_requirements = trace_input_keys - (pipeline_output_keys | network_output_keys
@@ -286,14 +301,18 @@
         the trace on_end method.
 
         Args:
             run_modes: The current execution modes.
             eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
                 PyTorch by nature is always in eager mode.
         """
+        with Suppressor():
+            # TODO - remove this after updating to TF > 2.11
+            from tensorflow.python.autograph.pyct.static_analysis.liveness import Analyzer
+            Analyzer.lamba_check(None, None)  # type: ignore
         all_traces = sort_traces(get_current_items(self.traces_in_use, run_modes=run_modes), ds_ids=[])
         with NonContext() if fe.fe_history_path is False else HistoryRecorder(
                 self.system, self.filepath, db_path=fe.fe_history_path):
             try:
                 self._run_traces_on_begin(traces=all_traces)
                 if "train" in run_modes or "eval" in run_modes:
                     # If the training is re-starting from a restore wizard, it should re-run the last eval epoch
@@ -362,15 +381,16 @@
                     self.system.eval_log_steps = ([
                         1, log_steps_per_epoch // 3, (2 * log_steps_per_epoch) // 3, log_steps_per_epoch
                     ], log_steps_per_epoch) if not self.system.eval_log_steps_request else \
                         (self.system.eval_log_steps_request, log_steps_per_epoch)
 
                 loader = self._configure_loader(loader)
                 iterator = iter(loader)
-                with Suppressor():
+                with Suppressor(allow_pyprint=True, show_if_exception=True):
+                    # multi-gpu tensorflow prints a ton of complaint messages here
                     batch = next(iterator)
                 ds_traces = sort_traces(ds_traces,
                                         available_outputs=to_set(batch.keys()) | network_output_keys,
                                         ds_ids=ds_ids)
                 per_ds_traces = [trace for trace in ds_traces if isinstance(trace, PerDSTrace)]
                 self._run_traces_on_ds_begin(traces=per_ds_traces)
                 while True:
@@ -384,16 +404,15 @@
                         batch, prediction = self.network.run_step(batch)
                         self._run_traces_on_batch_end(batch, prediction, traces=ds_traces)
                         if isinstance(loader, DataLoader) and (
                             (self.system.batch_idx == self.system.train_steps_per_epoch and self.system.mode == "train")
                                 or
                             (self.system.batch_idx == self.system.eval_steps_per_epoch and self.system.mode == "eval")):
                             raise StopIteration
-                        with Suppressor():
-                            batch = next(iterator)
+                        batch = next(iterator)
                     except StopIteration:
                         break
                 self._run_traces_on_ds_end(traces=per_ds_traces, data=end_epoch_data)
             self.network.unload_epoch()
         self._run_traces_on_epoch_end(traces=epoch_traces, data=end_epoch_data)
 
     def _configure_loader(self, loader: Union[DataLoader, tf.data.Dataset]) -> Union[DataLoader, tf.data.Dataset]:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/pytorch/hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/pytorch/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/instance_norm.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/layers/tensorflow/reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/layers/tensorflow/reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/network.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,40 +13,44 @@
 # limitations under the License.
 # ==============================================================================
 import gc
 import os
 import sys
 import tempfile
 from collections import ChainMap
-from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, Set, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, Sequence, Set, Tuple, TypeVar, \
+    Union, overload
 
 import gdown
+import keras.mixed_precision as mixed_precision_tf
 import numpy as np
 import tensorflow as tf
-import tensorflow.keras.mixed_precision as mixed_precision_tf
 import torch
+from keras.engine.sequential import Sequential
+from keras.mixed_precision.loss_scale_optimizer import LossScaleOptimizer, LossScaleOptimizerV3
 from tensorflow.python.distribute.values import DistributedValues
-from tensorflow.python.keras.engine.sequential import Sequential
 
 import fastestimator as fe
 from fastestimator.backend._load_model import load_model
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.op.numpyop import Batch, NumpyOp, RemoveIf, forward_numpyop
 from fastestimator.op.op import get_inputs_by_op, write_outputs_by_op
 from fastestimator.op.tensorop.model.update import UpdateOp
 from fastestimator.op.tensorop.tensorop import TensorOp
 from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
-from fastestimator.util.base_util import NonContext, to_list
+from fastestimator.util.base_util import NonContext, to_list, warn
 from fastestimator.util.traceability_util import trace_model, traceable
-from fastestimator.util.util import get_batch_size
+from fastestimator.util.util import Suppressor, detach_tensors, get_batch_size, get_device, get_num_gpus, \
+    move_tensors_to_device
 
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 T = TypeVar('T')
 
 GOOGLE_DRIVE_URL = "https://drive.google.com"
+_MAC_BUILD_WARNING = False
 
 
 @traceable()
 class BaseNetwork:
     """A base class for Network objects.
 
     Networks are used to define the computation graph surrounding one or more models during training.
@@ -62,15 +66,15 @@
         ValueError: Mixed precision settings for all models are not the same.
     """
     def __init__(
         self,
         target_type: str,
         device: Optional[torch.device],
         ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Iterable[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
     ) -> None:
         self.ops = to_list(ops)
         self.target_type = target_type
         self.device = device
         for op in get_current_items(self.ops):
             op.build(framework=self.target_type, device=self.device)
         self.models = to_list(_collect_models(ops))
@@ -319,15 +323,15 @@
         models |= op.get_fe_models()
     return models
 
 
 # noinspection PyPep8Naming
 def Network(
         ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        pops: Union[None, NumpyOp, Scheduler[NumpyOp], Iterable[Union[NumpyOp,
+        pops: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp,
                                                                       Scheduler[NumpyOp]]]] = None) -> BaseNetwork:
     """A function to automatically instantiate the correct Network derived class based on the given `ops`.
 
     Args:
         ops: A collection of Ops defining the graph for this Network. It should contain at least one ModelOp, and all
             models should be either TensorFlow or Pytorch. We currently do not support mixing TensorFlow and Pytorch
             models within the same network.
@@ -376,23 +380,22 @@
 
     Args:
         ops: The ops defining the execution graph for this Network.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
 
     """
+    device: torch.device
+
     def __init__(
         self,
         ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Iterable[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
     ) -> None:
-        super().__init__(target_type='torch',
-                         device=torch.device("cuda:0" if torch.cuda.is_available() else "cpu"),
-                         ops=ops,
-                         postprocessing=postprocessing)
+        super().__init__(target_type='torch', device=get_device(), ops=ops, postprocessing=postprocessing)
 
     def load_epoch(self,
                    mode: str,
                    epoch: int,
                    ds_id: str,
                    output_keys: Optional[Set[str]] = None,
                    warmup: bool = False,
@@ -408,15 +411,15 @@
             ds_id: The current dataset id.
             output_keys: What keys must be moved from the GPU back to the CPU after executing a step.
             warmup: Whether to prepare to execute it warmup mode or not (end users can likely ignore this argument).
             eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
                 PyTorch by nature is always in eager mode.
         """
         super().load_epoch(mode=mode, epoch=epoch, ds_id=ds_id, output_keys=output_keys, warmup=warmup, eager=eager)
-        if self.device.type == "cuda":
+        if self.device.type != "cpu":
             for model in self.epoch_models:
                 # move model variables to gpu
                 model.to(self.device)
                 if model.current_optimizer and mode == "train":
                     # move optimizer variables to gpu
                     self._move_optimizer_between_device(model.current_optimizer.state, self.device)
         # Set all of the contiguous final updates to defer their updates by default to enable things like CycleGan
@@ -445,15 +448,15 @@
                     pass
 
     def unload_epoch(self) -> None:
         """Clean up the network after running an epoch.
 
         In this case we move all of the models from the GPU(s) back to the CPU.
         """
-        if self.device.type == "cuda":
+        if self.device.type != "cpu":
             for model in self.epoch_models:
                 # move model variables to cpu
                 model.to("cpu")
                 if model.current_optimizer and self.epoch_state["mode"] == "train":
                     # move optimizer variables to cpu
                     self._move_optimizer_between_device(model.current_optimizer.state, "cpu")
         # Set the final update ops back to their original defer status
@@ -472,17 +475,17 @@
         Args:
             batch: The input data to be moved.
             mode: The current execution mode. One of 'train', 'eval', 'test', or 'infer'.
 
         Returns:
             The input data ready for use on GPU(s).
         """
-        if self.device.type == "cuda":
+        if self.device.type != "cpu":
             new_batch = {
-                key: self._move_tensor_between_device(batch[key], self.device)
+                key: move_tensors_to_device(batch[key], self.device)
                 for key in self.effective_inputs[mode] if key in batch
             }
         else:
             new_batch = {key: batch[key] for key in self.effective_inputs[mode] if key in batch}
         return new_batch
 
     def _run_step(self, batch: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
@@ -498,88 +501,41 @@
             (batch_data, prediction_data)
         """
         mode = self.epoch_state["mode"]
         batch_in = self._get_effective_batch_input(batch, mode)
         self.epoch_state["tape"] = NonContext()
         # gpu operation
         with torch.no_grad() if not self.epoch_state["req_grad"] else NonContext():
-            with torch.cuda.amp.autocast() if self.mixed_precision else NonContext():
+            with torch.autocast(device_type=self.device.type) if self.mixed_precision else NonContext():
                 self._forward_batch(batch_in, self.epoch_state, self.epoch_ops)
 
         # copy data to cpu
-        if self.device.type == "cuda":
+        if self.device.type != "cpu":
             prediction = {
-                key: self._move_tensor_between_device(self._detach_tensor(batch_in[key]), "cpu")
+                key: move_tensors_to_device(detach_tensors(batch_in[key]), "cpu")
                 for key in self.effective_outputs[mode] if key in batch_in
             }
         else:
-            prediction = {
-                key: self._detach_tensor(batch_in[key])
-                for key in self.effective_outputs[mode] if key in batch_in
-            }
+            prediction = {key: detach_tensors(batch_in[key]) for key in self.effective_outputs[mode] if key in batch_in}
         return batch, prediction
 
-    def _move_tensor_between_device(self, data: T, device: Union[str, torch.device]) -> T:
-        """Move tensor between gpu and cpu recursively.
-
-        Args:
-            data: The input data to be moved.
-            device: The target device.
-
-        Returns:
-            Output data.
-        """
-        if isinstance(data, dict):
-            return {key: self._move_tensor_between_device(value, device) for (key, value) in data.items()}
-        elif isinstance(data, list):
-            return [self._move_tensor_between_device(val, device) for val in data]
-        elif isinstance(data, tuple):
-            return tuple([self._move_tensor_between_device(val, device) for val in data])
-        elif isinstance(data, set):
-            return set([self._move_tensor_between_device(val, device) for val in data])
-        elif isinstance(data, torch.Tensor):
-            return data.to(device)
-        else:
-            return data
-
-    def _detach_tensor(self, data: T) -> T:
-        """Detach tensor from current graph recursively.
-
-        Args:
-            data: The data to be detached.
-
-        Returns:
-            Output data.
-        """
-        if isinstance(data, dict):
-            return {key: self._detach_tensor(value) for (key, value) in data.items()}
-        elif isinstance(data, list):
-            return [self._detach_tensor(val) for val in data]
-        elif isinstance(data, tuple):
-            return tuple([self._detach_tensor(val) for val in data])
-        elif isinstance(data, set):
-            return set([self._detach_tensor(val) for val in data])
-        elif isinstance(data, torch.Tensor):
-            return data.detach()
-        return data
-
 
 @traceable()
 class TFNetwork(BaseNetwork):
     """An extension of BaseNetwork for TensorFlow models.
 
     Args:
         ops: The ops defining the execution graph for this Network.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
     """
     def __init__(
         self,
         ops: Iterable[Union[TensorOp, Scheduler[TensorOp]]],
-        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Iterable[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
+        postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[NumpyOp, Scheduler[NumpyOp]]]] = None
     ) -> None:
         super().__init__(target_type='tf', device=None, ops=ops, postprocessing=postprocessing)
 
     def load_epoch(self,
                    mode: str,
                    epoch: int,
                    ds_id: str,
@@ -647,18 +603,19 @@
         else:
             if self.epoch_state["eager"]:
                 prediction = self._forward_step_eager(batch_in,
                                                       self.epoch_state,
                                                       self.epoch_ops,
                                                       to_list(self.effective_outputs[mode]))
             else:
-                prediction = self._forward_step_static(batch_in,
-                                                       self.epoch_state,
-                                                       self.epoch_ops,
-                                                       to_list(self.effective_outputs[mode]))
+                with Suppressor(allow_pyprint=True, show_if_exception=True):
+                    prediction = self._forward_step_static(batch_in,
+                                                           self.epoch_state,
+                                                           self.epoch_ops,
+                                                           to_list(self.effective_outputs[mode]))
         return batch, prediction
 
     def _per_replica_to_global(self, data: T) -> T:
         """Combine data from "per-replica" values recursively.
 
         For multi-GPU training, data are distributed using `tf.distribute.Strategy.experimental_distribute_dataset`.
         This method collects data from all replicas and combines them into one.
@@ -833,16 +790,34 @@
             return set([self._subsample_data(val, n) for val in data])
         elif hasattr(data, "shape") and list(data.shape) and data.shape[0] > n:
             return data[0:n]
         else:
             return data
 
 
-def build(model_fn: Callable[[], Union[Model, List[Model]]],
-          optimizer_fn: Union[str, Scheduler, Callable, List[str], List[Callable], List[Scheduler], None],
+@overload
+def build(model_fn: Callable[[], Model],
+          optimizer_fn: Union[None, str, Scheduler, Callable],
+          weights_path: Union[str, None, List[Union[str, None]]] = None,
+          model_name: Union[str, List[str], None] = None,
+          mixed_precision: bool = False) -> Model:
+    ...
+
+
+@overload
+def build(model_fn: Callable[[], Sequence[Model]],
+          optimizer_fn: Union[None, str, Scheduler, Callable, Sequence[Union[None, str, Callable, Scheduler]]],
+          weights_path: Union[str, None, List[Union[str, None]]] = None,
+          model_name: Union[str, List[str], None] = None,
+          mixed_precision: bool = False) -> List[Model]:
+    ...
+
+
+def build(model_fn: Callable[[], Union[Model, Sequence[Model]]],
+          optimizer_fn: Union[None, str, Scheduler, Callable, Sequence[Union[None, str, Callable, Scheduler]]],
           weights_path: Union[str, None, List[Union[str, None]]] = None,
           model_name: Union[str, List[str], None] = None,
           mixed_precision: bool = False) -> Union[Model, List[Model]]:
     """Build model instances and associate them with optimizers.
 
     This method can be used with TensorFlow models / optimizers:
     ```python
@@ -887,23 +862,22 @@
     # RuntimeError: DataLoader worker (pid 4225) is killed by signal: Aborted.
     # RuntimeError: DataLoader worker (pid(s) 4225, 4226, 4227) exited unexpectedly
     gc.collect()
     # tensorflow models requires setting global policies prior to model creation. Since there is no way to know the
     # framework of model, setting the policy for both tf and pytorch here.
     if mixed_precision:
         if sys.platform == 'darwin':
-            print("\033[93m{}\033[00m".format("FastEstimator-Warn: Mixed Precision is not currently supported on Mac / "
-                                              "Metal. This flag will be ignored."))
+            warn("Mixed Precision is not currently supported on Mac / Metal. This flag will be ignored.")
             mixed_precision = False
         else:
             mixed_precision_tf.set_global_policy(mixed_precision_tf.Policy('mixed_float16'))
     else:
         mixed_precision_tf.set_global_policy(mixed_precision_tf.Policy('float32'))
     models = None
-    if torch.cuda.device_count() > 1:
+    if get_num_gpus() > 1:
         # We need to figure out whether model_fn returns tf models or torch models
         if not isinstance(tf.distribute.get_strategy(), tf.distribute.MirroredStrategy):
             # If we've already done this and gotten TF model, the above flag will be set and this will be skipped. If we
             # are dealing with pytorch models, the model_fn() invocation will be kept so as to not waste clock cycles.
             models = to_list(model_fn())
             if isinstance(models[0], tf.keras.Model):
                 models = None  # We will re-instantiate the models again now that we know we need MirroredStrategy
@@ -961,15 +935,15 @@
         framework = "torch"
     elif isinstance(model, Sequential):
         raise DeprecationWarning("Importing from tensorflow.python.keras.models/layers is deprecated. Import from "
                                  "tensorflow.keras.models/layers instead")
     else:
         raise ValueError("unrecognized model format: {}".format(type(model)))
     # torch multi-gpu handling
-    if framework == "torch" and torch.cuda.device_count() > 1:
+    if framework == "torch" and get_num_gpus() > 1:
         model = torch.nn.DataParallel(model)
     # mark models with its mixed_precision flag
     model.mixed_precision = mixed_precision
     if isinstance(optimizer_fn, EpochScheduler):
         for epoch, optimizer_def in optimizer_fn.epoch_dict.items():
             optimizer_fn.epoch_dict[epoch] = _build_optimizer(optimizer_def, model, framework, mixed_precision)
         model.current_optimizer = optimizer_fn.get_current_value(1)
@@ -991,16 +965,17 @@
             os.rename(os.path.join('./', file_name), os.path.join(tmp_dir, file_name))
             weight = gdown.download(weight, os.path.join(tmp_dir, file_name), quiet=False)
         load_model(model, weight)
     model.model_name = name
     return model
 
 
-def _build_optimizer(optimizer_fn: Union[str, Callable, None], model: Model, framework: str,
-                     mixed_precision: bool) -> Union[None, tf.optimizers.Optimizer, torch.optim.Optimizer]:
+def _build_optimizer(
+    optimizer_fn: Union[str, Callable, None], model: Model, framework: str, mixed_precision: bool
+) -> Union[None, tf.optimizers.Optimizer, tf.optimizers.legacy.Optimizer, torch.optim.Optimizer]:
     """A helper method to instantiate an optimizer.
 
     Args:
         optimizer_fn: The function responsible for constructing an optimizer, or else a string indicating one of the
             default optimizers to be used.
         model: The model to associate the optimizer with.
         framework: Which backend framework should be used ('tf' or 'torch').
@@ -1021,21 +996,23 @@
     Args:
         name: The name of the default optimizer to instantiate.
         framework: Which backend framework should be used ('tf' or 'torch').
 
     Returns:
         An optimizer instance corresponding to the given `name` and `framework`.
     """
+    # The legacy optimizers appear to be faster than the new ones on both mac and linux. Revisit this speed test again
+    # after tf version > 2.12
     tf_optimizer_fn = {
-        'adadelta': tf.optimizers.Adadelta,
-        'adagrad': tf.optimizers.Adagrad,
-        'adam': tf.optimizers.Adam,
-        'adamax': tf.optimizers.Adamax,
-        'rmsprop': tf.optimizers.RMSprop,
-        'sgd': tf.optimizers.SGD
+        'adadelta': tf.optimizers.legacy.Adadelta,
+        'adagrad': tf.optimizers.legacy.Adagrad,
+        'adam': tf.optimizers.legacy.Adam,
+        'adamax': tf.optimizers.legacy.Adamax,
+        'rmsprop': tf.optimizers.legacy.RMSprop,
+        'sgd': tf.optimizers.legacy.SGD
     }
     pytorch_optimizer_fn = {
         'adadelta': lambda x: torch.optim.Adadelta(params=x),
         'adagrad': lambda x: torch.optim.Adagrad(params=x),
         'adam': lambda x: torch.optim.Adam(params=x),
         'adamax': lambda x: torch.optim.Adamax(params=x),
         'rmsprop': lambda x: torch.optim.RMSprop(params=x),
@@ -1044,16 +1021,17 @@
     if framework == "tf":
         optimizer_fn = tf_optimizer_fn[name]
     else:
         optimizer_fn = pytorch_optimizer_fn[name]
     return optimizer_fn
 
 
-def _optimizer_fn_to_optimizer(optimizer_fn: Union[Callable, None], model: Model, framework: str,
-                               mixed_precision: bool) -> Union[None, tf.optimizers.Optimizer, torch.optim.Optimizer]:
+def _optimizer_fn_to_optimizer(
+        optimizer_fn: Union[Callable, None], model: Model, framework: str,
+        mixed_precision: bool) -> Union[None, tf.optimizers.legacy.Optimizer, torch.optim.Optimizer]:
     """A helper function to invoke an optimizer function.
 
     Args:
         optimizer_fn: The function to be invoked in order to instantiate an optimizer.
         model: The model with which the optimizer should be associated.
         framework: Which backend framework should be used ('tf' or 'torch').
         mixed_precision: Whether to enable mixed-precision training.
@@ -1065,22 +1043,41 @@
     if optimizer_fn:
         if framework == "tf":
             try:
                 optimizer = optimizer_fn()
             except:
                 raise AssertionError("optimizer_fn of Tensorflow backend should be callable without args. Please "
                                      "make sure model and optimizer_fn are using the same backend")
+            if sys.platform == 'darwin' and hasattr(optimizer, 'jit_compile'):
+                # Mac doesn't support XLA acceleration as of TF 2.11
+                # TODO - check compatibility again in future release
+                global _MAC_BUILD_WARNING
+                if not _MAC_BUILD_WARNING:
+                    warn("JIT compiling of optimizers is not currently supported by MacOS and will be disabled. You "
+                         "may want to use an optimizer from tf.optimizers.legacy instead for better speed.")
+                    _MAC_BUILD_WARNING = True
+                optimizer.jit_compile = False
             # initialize optimizer variables
-            _ = optimizer.iterations
-            optimizer._create_hypers()
-            optimizer._create_slots(model.trainable_variables)
+            if hasattr(optimizer, 'build'):
+                optimizer.build(var_list=model.trainable_variables)
+            else:
+                _ = optimizer.iterations
+                if hasattr(optimizer, '_create_hypers'):
+                    optimizer._create_hypers()
+                if hasattr(optimizer, '_create_slots'):
+                    optimizer._create_slots(model.trainable_variables)
+            assert isinstance(optimizer, (tf.optimizers.Optimizer, tf.keras.optimizers.experimental.Optimizer,
+                                          tf.optimizers.legacy.Optimizer)), \
+                f"optimizer_fn should generate tensorflow optimizer, but got {type(optimizer)}"
             # handle mixed precision loss scaling
             if mixed_precision:
-                optimizer = mixed_precision_tf.LossScaleOptimizer(optimizer)
-            assert isinstance(optimizer, tf.optimizers.Optimizer), "optimizer_fn should generate tensorflow optimizer"
+                if isinstance(optimizer, tf.optimizers.legacy.Optimizer):
+                    optimizer = LossScaleOptimizer(optimizer)
+                else:
+                    optimizer = LossScaleOptimizerV3(optimizer)
         else:
             try:
                 optimizer = optimizer_fn(model.parameters())
             except Exception as e:
                 print("optimizer_fn of Pytorch backend should be callable with single arg. Please sure model and \
                 optimizer_fn are using the same backend")
                 raise ValueError(repr(e))
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/one_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import inspect
-import random
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 
 from fastestimator.op.numpyop.numpyop import Batch, NumpyOp
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class OneOf(NumpyOp):
     """Perform one of several possible NumpyOps.
 
     Args:
-        *numpy_ops: A list of ops to choose between with uniform probability.
+        *numpy_ops: Ops to choose between with a specified (or uniform) probability.
+        probs: List of probabilities, must sum to 1. When None, the probabilities will be equally distributed.
     """
-    def __init__(self, *numpy_ops: NumpyOp) -> None:
+    def __init__(self, *numpy_ops: NumpyOp, probs: Optional[List[float]] = None) -> None:
         inputs = numpy_ops[0].inputs
         outputs = numpy_ops[0].outputs
         mode = numpy_ops[0].mode
         ds_id = numpy_ops[0].ds_id
         super().__init__(inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
         self.in_list = numpy_ops[0].in_list
         self.out_list = numpy_ops[0].out_list
@@ -41,15 +41,19 @@
             assert not isinstance(op, Batch), "Cannot nest the Batch op inside OneOf"
             assert inputs == op.inputs, "All ops within a OneOf must share the same inputs"
             assert self.in_list == op.in_list, "All ops within OneOf must share the same input configuration"
             assert outputs == op.outputs, "All ops within a OneOf must share the same outputs"
             assert self.out_list == op.out_list, "All ops within OneOf must share the same output configuration"
             assert mode == op.mode, "All ops within a OneOf must share the same mode"
             assert ds_id == op.ds_id, "All ops within a OneOf must share the same ds_id"
+        if probs:
+            assert len(numpy_ops) == len(probs), "The number of probabilities do not match with number of Operators"
+            assert abs(sum(probs) - 1) < 1e-8, "Probabilities must sum to 1"
         self.ops = numpy_ops
+        self.probs = probs
 
     def __getstate__(self) -> Dict[str, List[Dict[Any, Any]]]:
         return {'ops': [elem.__getstate__() if hasattr(elem, '__getstate__') else {} for elem in self.ops]}
 
     def set_rua_level(self, magnitude_coef: float) -> None:
         """Set the augmentation intensity based on the magnitude_coef.
 
@@ -76,13 +80,13 @@
         Args:
             data: The information to be passed to one of the wrapped operators.
             state: Information about the current execution context, for example {"mode": "train"}.
 
         Returns:
             The `data` after application of one of the available numpyOps.
         """
-        return random.choice(self.ops).forward(data, state)
+        return np.random.choice(self.ops, p=self.probs).forward(data, state)
 
     def forward_batch(self,
                       data: Union[np.ndarray, List[np.ndarray]],
                       state: Dict[str, Any]) -> Union[np.ndarray, List[np.ndarray]]:
-        return random.choice(self.ops).forward_batch(data, state)
+        return np.random.choice(self.ops, p=self.probs).forward_batch(data, state)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/affine.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/center_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/flip.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Union
 
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations.transforms import Flip as FlipAlb
+from albumentations.augmentations.geometric.transforms import Flip as FlipAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class Flip(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/grid_distortion.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, List, Optional, Tuple, Union
 
 import cv2
-from albumentations.augmentations.transforms import GridDistortion as GridDistortionAlb
+from albumentations.augmentations.geometric.transforms import GridDistortion as GridDistortionAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class GridDistortion(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/horizontal_flip.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Union
 
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations.transforms import HorizontalFlip as FlipAlb
+from albumentations.augmentations.geometric.transforms import HorizontalFlip as FlipAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class HorizontalFlip(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/longest_max_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Union
 
 import cv2
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations import LongestMaxSize as LongestMaxSizeAlb
+from albumentations.augmentations.geometric import LongestMaxSize as LongestMaxSizeAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class LongestMaxSize(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/mask_dropout.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Tuple, Union
 
-from albumentations.augmentations.transforms import MaskDropout as MaskDropoutAlb
+from albumentations.augmentations.dropout import MaskDropout as MaskDropoutAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class MaskDropout(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/multivariate.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/multivariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/optical_distortion.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, List, Optional, Tuple, Union
 
 import cv2
-from albumentations.augmentations.transforms import OpticalDistortion as OpticalDistortionAlb
+from albumentations.augmentations import OpticalDistortion as OpticalDistortionAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class OpticalDistortion(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/pad_if_needed.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Iterable, List, Optional, Union
+from typing import Iterable, Optional, Sequence, Union
 
 import cv2
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations.transforms import PadIfNeeded as PadIfNeededAlb
+from albumentations.augmentations.geometric.transforms import PadIfNeeded as PadIfNeededAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class PadIfNeeded(MultiVariateAlbumentation):
@@ -43,26 +43,27 @@
         bbox_out: The key to write the modified bounding box(es) (defaults to `bbox_in` if None).
         keypoints_out: The key to write the modified keypoints (defaults to `keypoints_in` if None).
         bbox_params: Parameters defining the type of bounding box ('coco', 'pascal_voc', 'albumentations' or 'yolo').
         keypoint_params: Parameters defining the type of keypoints ('xy', 'yx', 'xya', 'xys', 'xyas', 'xysa').
         min_height: Minimal result image height.
         min_width: Minimal result image width.
         border_mode: Flag that is used to specify the pixel extrapolation method. Should be one of:
-            cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP, cv2.BORDER_REFLECT_101.        value: Padding value if border_mode is cv2.BORDER_CONSTANT.
+            cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP, cv2.BORDER_REFLECT_101.
+        value: Padding value if border_mode is cv2.BORDER_CONSTANT.
         mask_value: Padding value for mask if border_mode is cv2.BORDER_CONSTANT.
 
     Image types:
         uint8, float32
     """
     def __init__(self,
                  min_height: int = 1024,
                  min_width: int = 1024,
                  border_mode: int = cv2.BORDER_REFLECT_101,
-                 value: Union[None, int, float, List[int], List[float]] = None,
-                 mask_value: Union[None, int, float, List[int], List[float]] = None,
+                 value: Union[None, int, float, Sequence[int], Sequence[float]] = None,
+                 mask_value: Union[None, int, float, Sequence[int], Sequence[float]] = None,
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  image_in: Optional[str] = None,
                  mask_in: Optional[str] = None,
                  masks_in: Optional[str] = None,
                  bbox_in: Optional[str] = None,
                  keypoints_in: Optional[str] = None,
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,16 @@
                  ds_id: Union[None, str, Iterable[str]] = None,
                  image_in: Optional[str] = None,
                  mask_in: Optional[str] = None,
                  masks_in: Optional[str] = None,
                  image_out: Optional[str] = None,
                  mask_out: Optional[str] = None,
                  masks_out: Optional[str] = None):
+        import numpy as np  # Albumentations 1.3.0 is relying on deprecated np.int alias.
+        np.int = np.int32  # TODO - Remove this after they upgrade
         super().__init__(RandomGridShuffleAlb(grid=grid, always_apply=True),
                          image_in=image_in,
                          mask_in=mask_in,
                          masks_in=masks_in,
                          bbox_in=None,
                          keypoints_in=None,
                          image_out=image_out,
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_scale.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/read_mat.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/resize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/rotate.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, List, Optional, Tuple, Union
 
 import cv2
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations import ShiftScaleRotate as ShiftScaleRotateAlb
+from albumentations.augmentations.geometric import ShiftScaleRotate as ShiftScaleRotateAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class ShiftScaleRotate(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Union
 
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations.transforms import Transpose as TransposeAlb
+from albumentations.augmentations import Transpose as TransposeAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class Transpose(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/multivariate/vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/multivariate/vertical_flip.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Optional, Union
 
 from albumentations import BboxParams, KeypointParams
-from albumentations.augmentations.transforms import VerticalFlip as VerticalFlipAlb
+from albumentations.augmentations.geometric.transforms import VerticalFlip as VerticalFlipAlb
 
 from fastestimator.op.numpyop.multivariate.multivariate import MultiVariateAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class VerticalFlip(MultiVariateAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/numpyop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/numpyop.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, TypeVar, Union
+from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 import tensorflow as tf
 import torch
 from torch.utils.data.dataloader import default_collate
 
 from fastestimator.backend._to_tensor import to_tensor
@@ -67,16 +67,15 @@
 
         Returns:
             The `data` after applying whatever transform this Op is responsible for. It will be written into the data
             dictionary based on whatever keys this Op declares as its `outputs`.
         """
         return data
 
-    def forward_batch(self,
-                      data: Union[np.ndarray, List[np.ndarray]],
+    def forward_batch(self, data: Union[np.ndarray, List[np.ndarray]],
                       state: Dict[str, Any]) -> Union[None, FilteredData, np.ndarray, List[np.ndarray]]:
         """A method which will be invoked in order to transform a batch of data.
 
         This method will be invoked on batches of data during network postprocessing. It should expect to receive
         batched data and should itself return batched data.
 
         Args:
@@ -172,15 +171,15 @@
         mode: What mode(s) to execute this Op in. For example, "train", "eval", "test", or "infer". To execute
             regardless of mode, pass None. To execute in all modes except for a particular one, you can pass an argument
             like "!infer" or "!train".
         ds_id: What dataset id(s) to execute this Op in. To execute regardless of ds_id, pass None. To execute in all
             ds_ids except for a particular one, you can pass an argument like "!ds1".
     """
     def __init__(self,
-                 keys: Union[str, List[str]],
+                 keys: Union[str, Sequence[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None) -> None:
         super().__init__(inputs=keys, mode=mode, ds_id=ds_id)
 
     def forward(self, data: Union[np.ndarray, List[np.ndarray]], state: Dict[str, Any]) -> None:
         pass
 
@@ -259,16 +258,15 @@
         self.replacement = replacement
 
     def forward(self, data: List[np.ndarray], state: Dict[str, Any]) -> Optional[FilteredData]:
         if self.filter_fn(*data):
             return FilteredData(replacement=self.replacement)
         return None
 
-    def forward_batch(self, data: Union[Tensor, List[Tensor]], state: Dict[str,
-                                                                           Any]) -> Optional[FilteredData]:
+    def forward_batch(self, data: Union[Tensor, List[Tensor]], state: Dict[str, Any]) -> Optional[FilteredData]:
         return self.forward(data, state)
 
 
 def forward_numpyop(ops: List[NumpyOp],
                     data: MutableMapping[str, Any],
                     state: Dict[str, Any],
                     batched: Optional[str] = None) -> Optional[FilteredData]:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/autocontrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/binarize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/motion_blur.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,37 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Tuple, Union
 
-from albumentations.augmentations.transforms import Blur as BlurAlb
+from albumentations.augmentations.blur import MotionBlur as MotionBlurAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
-class Blur(ImageOnlyAlbumentation):
-    """Blur the image with a randomly-sized kernel
+class MotionBlur(ImageOnlyAlbumentation):
+    """Motion Blur the image with a randomly-sized kernel.
 
     Args:
         inputs: Key(s) of images to be modified.
         outputs: Key(s) into which to write the modified images.
         mode: What mode(s) to execute this Op in. For example, "train", "eval", "test", or "infer". To execute
             regardless of mode, pass None. To execute in all modes except for a particular one, you can pass an argument
             like "!infer" or "!train".
         ds_id: What dataset id(s) to execute this Op in. To execute regardless of ds_id, pass None. To execute in all
             ds_ids except for a particular one, you can pass an argument like "!ds1".
-        blur_limit: maximum kernel size for blurring the input image. Should be in range [3, inf).
+        blur_limit: maximum kernel size for blurring the input image. Should be in the range [3, inf).
 
     Image types:
         uint8, float32
     """
     def __init__(self,
                  inputs: Union[str, Iterable[str]],
                  outputs: Union[str, Iterable[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  blur_limit: Union[int, Tuple[int, int]] = 7):
-        super().__init__(BlurAlb(blur_limit=blur_limit, always_apply=True), inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
+        super().__init__(MotionBlurAlb(blur_limit=blur_limit, always_apply=True),
+                         inputs=inputs,
+                         outputs=outputs,
+                         mode=mode,
+                         ds_id=ds_id)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/brightness.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/calibate.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/calibate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_dropout.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Iterable, Tuple, Union
+from typing import Iterable, Sequence, Tuple, Union
 
-from albumentations.augmentations.transforms import ChannelDropout as ChannelDropoutAlb
+from albumentations.augmentations.dropout import ChannelDropout as ChannelDropoutAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class ChannelDropout(ImageOnlyAlbumentation):
@@ -35,16 +35,16 @@
         channel_drop_range: Range from which we choose the number of channels to drop.
         fill_value: Pixel values for the dropped channel.
 
     Image types:
         int8, uint16, unit32, float32
     """
     def __init__(self,
-                 inputs: Union[str, Iterable[str]],
-                 outputs: Union[str, Iterable[str]],
+                 inputs: Union[str, Sequence[str]],
+                 outputs: Union[str, Sequence[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  channel_drop_range: Tuple[int, int] = (1, 1),
                  fill_value: Union[int, float] = 0):
         super().__init__(
             ChannelDropoutAlb(channel_drop_range=channel_drop_range, fill_value=fill_value, always_apply=True),
             inputs=inputs,
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/clahe.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/coarse_dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, List, Optional, Union
 
-from albumentations.augmentations.transforms import CoarseDropout as CoarseDropoutAlb
+from albumentations.augmentations.dropout import CoarseDropout as CoarseDropoutAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class CoarseDropout(ImageOnlyAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/color.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/color_jitter.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/contrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/downscale.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/equalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/expand_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/from_float.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/from_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/gaussian_blur.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Tuple, Union
 
-from albumentations.augmentations.transforms import GaussianBlur as GaussianBlurAlb
+from albumentations.augmentations import GaussianBlur as GaussianBlurAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class GaussianBlur(ImageOnlyAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/image_compression.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/invert_img.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/iso_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/median_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/median_blur.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Tuple, Union
 
-from albumentations.augmentations.transforms import MedianBlur as MedianBlurAlb
+from albumentations.augmentations.blur import MedianBlur as MedianBlurAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class MedianBlur(ImageOnlyAlbumentation):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/minmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/motion_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/blur.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Iterable, Tuple, Union
 
-from albumentations.augmentations.transforms import MotionBlur as MotionBlurAlb
+from albumentations.augmentations.blur.transforms import Blur as BlurAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
-class MotionBlur(ImageOnlyAlbumentation):
-    """Motion Blur the image with a randomly-sized kernel.
+class Blur(ImageOnlyAlbumentation):
+    """Blur the image with a randomly-sized kernel
 
     Args:
         inputs: Key(s) of images to be modified.
         outputs: Key(s) into which to write the modified images.
         mode: What mode(s) to execute this Op in. For example, "train", "eval", "test", or "infer". To execute
             regardless of mode, pass None. To execute in all modes except for a particular one, you can pass an argument
             like "!infer" or "!train".
         ds_id: What dataset id(s) to execute this Op in. To execute regardless of ds_id, pass None. To execute in all
             ds_ids except for a particular one, you can pass an argument like "!ds1".
-        blur_limit: maximum kernel size for blurring the input image. Should be in the range [3, inf).
+        blur_limit: maximum kernel size for blurring the input image. Should be in range [3, inf).
 
     Image types:
         uint8, float32
     """
     def __init__(self,
                  inputs: Union[str, Iterable[str]],
                  outputs: Union[str, Iterable[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  blur_limit: Union[int, Tuple[int, int]] = 7):
-        super().__init__(MotionBlurAlb(blur_limit=blur_limit, always_apply=True),
+        super().__init__(BlurAlb(blur_limit=blur_limit, always_apply=True),
                          inputs=inputs,
                          outputs=outputs,
                          mode=mode,
                          ds_id=ds_id)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Iterable, Tuple, Union
+from typing import Any, Dict, Iterable, List, Sequence, Tuple, Union
 
+import numpy as np
 from albumentations.augmentations.transforms import Normalize as NormalizeAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
@@ -36,19 +37,24 @@
         std: The divisor.
         max_pixel_value: Maximum possible pixel value.
 
     Image types:
         uint8, float32
     """
     def __init__(self,
-                 inputs: Union[str, Iterable[str]],
-                 outputs: Union[str, Iterable[str]],
+                 inputs: Union[str, Sequence[str]],
+                 outputs: Union[str, Sequence[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  mean: Union[float, Tuple[float, ...]] = (0.485, 0.456, 0.406),
                  std: Union[float, Tuple[float, ...]] = (0.229, 0.224, 0.225),
                  max_pixel_value: float = 255.0):
         super().__init__(NormalizeAlb(mean=mean, std=std, max_pixel_value=max_pixel_value, always_apply=True),
                          inputs=inputs,
                          outputs=outputs,
                          mode=mode,
                          ds_id=ds_id)
+
+    def forward(self, data: List[np.ndarray], state: Dict[str, Any]) -> List[np.ndarray]:
+        results = super().forward(data, state)
+        # Albumentation library casts the result to float64 iff the image is HxWx3, but we want consistent output
+        return [result.astype(np.float32) for result in results]
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/onehot.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/onehot.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,10 +64,10 @@
         if data.size == 1:
             output = np.eye(self.num_classes, dtype=np.float32)[data[0]]
         else:
             output = np.eye(self.num_classes, dtype=np.float32)[data]
 
         if self.label_smoothing != 0:
             smooth_label = self.label_smoothing / self.num_classes
-            output = np.where(output != 0, 1.0 - self.label_smoothing + smooth_label, smooth_label)
+            output = np.where(output != 0, 1.0 - self.label_smoothing + smooth_label, smooth_label).astype(np.float32)
 
         return output
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/posterize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_fog.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_gamma.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_rain.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_shadow.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_shadow.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Iterable, Tuple, Union
+from typing import Iterable, Sequence, Tuple, Union
 
 from albumentations.augmentations.transforms import RandomShadow as RandomShadowAlb
 
 from fastestimator.op.numpyop.univariate.univariate import ImageOnlyAlbumentation
+from fastestimator.util.base_util import warn
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class RandomShadow(ImageOnlyAlbumentation):
     """Add shadows to an image
 
@@ -39,25 +40,24 @@
             Should be in range [`num_shadows_lower`, inf].
         shadow_dimension: Number of edges in the shadow polygons.
 
     Image types:
         uint8, float32
     """
     def __init__(self,
-                 inputs: Union[str, Iterable[str]],
-                 outputs: Union[str, Iterable[str]],
+                 inputs: Union[str, Sequence[str]],
+                 outputs: Union[str, Sequence[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  shadow_roi: Tuple[float, float, float, float] = (0.0, 0.5, 1.0, 1.0),
                  num_shadows_lower: int = 1,
                  num_shadows_upper: int = 2,
                  shadow_dimension: int = 5):
-        print("\033[93m {}\033[00m".format(
-            "Warning! RandomShadow does not work with multi-threaded Pipelines. Either do not use this Op or else " +
-            "set your Pipeline num_process=0"))
+        warn("RandomShadow does not work with multi-threaded Pipelines. Either do not use this Op or else " +
+             "set your Pipeline num_process=0")
         # TODO - Have pipeline look for bad ops and auto-magically set num_process correctly
         super().__init__(
             RandomShadowAlb(shadow_roi=shadow_roi,
                             num_shadows_lower=num_shadows_lower,
                             num_shadows_upper=num_shadows_upper,
                             shadow_dimension=shadow_dimension,
                             always_apply=True),
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_shapes.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_snow.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/read_image.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/rua.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/sharpness.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/shear_x.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/shear_y.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/solarize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_array.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_float.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_gray.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/to_sepia.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/tokenize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/translate_x.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/translate_y.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/univariate.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/univariate.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from copy import deepcopy
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, List, Sequence, Union
 
 import numpy as np
 from albumentations import Compose, ImageOnlyTransform, ReplayCompose
 
 from fastestimator.op.numpyop.numpyop import NumpyOp
 from fastestimator.util.traceability_util import traceable
 
@@ -39,16 +39,16 @@
             regardless of mode, pass None. To execute in all modes except for a particular one, you can pass an argument
             like "!infer" or "!train".
         ds_id: What dataset id(s) to execute this Op in. To execute regardless of ds_id, pass None. To execute in all
             ds_ids except for a particular one, you can pass an argument like "!ds1".
     """
     def __init__(self,
                  func: ImageOnlyTransform,
-                 inputs: Union[str, List[str]],
-                 outputs: Union[str, List[str]],
+                 inputs: Union[str, Sequence[str]],
+                 outputs: Union[str, Sequence[str]],
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None):
         super().__init__(inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
         assert len(self.inputs) == len(self.outputs), "Input and Output lengths must match"
         self.func = Compose(transforms=[func])
         self.replay_func = ReplayCompose(transforms=[deepcopy(func)])
         self.in_list, self.out_list = True, True
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/numpyop/univariate/word_to_id.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/numpyop/univariate/word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/op.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/argmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/augmentation/mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/augmentation/mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/average.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gather.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/fgsm.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/gradient.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/gradient/watch.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/gradient/watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/dice_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/dice_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/focal_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/hinge.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/l1_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/loss/super_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/loss/super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/one_of.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any, Dict, List, Optional, Set, TypeVar, Union
 
+import numpy as np
 import tensorflow as tf
-import tensorflow_probability as tfp
 import torch
 
 from fastestimator.backend._cast import cast
 from fastestimator.op.tensorop.tensorop import TensorOp
 from fastestimator.util.traceability_util import traceable
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
@@ -27,47 +27,46 @@
 
 
 @traceable()
 class OneOf(TensorOp):
     """Perform one of several possible TensorOps.
 
     Args:
-        *tensor_ops: A list of ops to choose between with uniform probability.
+        *tensor_ops: Ops to choose between with a specified (or uniform) probability.
+        probs: List of probabilities, must sum to 1. When None, the probabilities will be equally distributed.
     """
-    def __init__(self, *tensor_ops: TensorOp) -> None:
+    def __init__(self, *tensor_ops: TensorOp, probs: Optional[List[float]] = None) -> None:
         inputs = tensor_ops[0].inputs
         outputs = tensor_ops[0].outputs
         mode = tensor_ops[0].mode
         ds_id = tensor_ops[0].ds_id
         super().__init__(inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
         self.in_list = tensor_ops[0].in_list
         self.out_list = tensor_ops[0].out_list
         for op in tensor_ops[1:]:
             assert inputs == op.inputs, "All ops within a OneOf must share the same inputs"
             assert self.in_list == op.in_list, "All ops within OneOf must share the same input configuration"
             assert outputs == op.outputs, "All ops within a OneOf must share the same outputs"
             assert self.out_list == op.out_list, "All ops within OneOf must share the same output configuration"
             assert mode == op.mode, "All ops within a OneOf must share the same mode"
             assert ds_id == op.ds_id, "All ops within a OneOf must share the same ds_id"
+        if probs:
+            assert len(tensor_ops) == len(probs), "The number of probabilities do not match with number of Operators"
+            assert abs(sum(probs) - 1) < 1e-8, "Probabilities must sum to 1"
+        else:
+            probs = [1 / len(tensor_ops) for _ in tensor_ops]
         self.ops = tensor_ops
-        self.prob_fn = None
-        self.invoke_fn = None
+        self.probs = probs
+        self.framework = None
 
     def build(self, framework: str, device: Optional[torch.device] = None) -> None:
+        assert framework in {"tf", "torch"}, "unrecognized framework: {}".format(framework)
+        self.framework = framework
         for op in self.ops:
             op.build(framework, device)
-        if framework == 'tf':
-            self.prob_fn = tfp.distributions.Uniform(low=0, high=len(self.ops))
-            self.invoke_fn = lambda idx, data, state: tf.switch_case(idx, [lambda: op.forward(data, state) for op in
-                                                                           self.ops])
-        elif framework == 'torch':
-            self.prob_fn = torch.distributions.uniform.Uniform(low=0, high=len(self.ops))
-            self.invoke_fn = lambda idx, data, state: self.ops[idx].forward(data, state)
-        else:
-            raise ValueError("unrecognized framework: {}".format(framework))
 
     def get_fe_loss_keys(self) -> Set[str]:
         return set.union(*[op.get_fe_loss_keys() for op in self.ops])
 
     def get_fe_models(self) -> Set[Model]:
         return set.union(*[op.get_fe_models() for op in self.ops])
 
@@ -86,9 +85,13 @@
         Args:
             data: The information to be passed to one of the wrapped operators.
             state: Information about the current execution context, for example {"mode": "train"}.
 
         Returns:
             The `data` after application of one of the available numpyOps.
         """
-        idx = cast(self.prob_fn.sample(), dtype='int32')
-        return self.invoke_fn(idx, data, state)
+        if self.framework == 'tf':
+            idx = cast(tf.random.categorical(tf.math.log([self.probs]), 1), dtype='int32')[0, 0]
+            results = tf.switch_case(idx, [lambda op=op: op.forward(data, state) for op in self.ops])
+        else:
+            results = np.random.choice(self.ops, p=self.probs).forward(data, state)
+        return results
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/model.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar, Union
 
 import tensorflow as tf
 import torch
 
 from fastestimator.backend._feed_forward import feed_forward
 from fastestimator.op.tensorop.tensorop import TensorOp
+from fastestimator.util.base_util import to_list, warn
 from fastestimator.util.traceability_util import FeInputSpec, traceable
 from fastestimator.util.util import get_num_devices
-from fastestimator.util.base_util import to_list
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 
 
 @traceable()
 class ModelOp(TensorOp):
@@ -63,16 +63,15 @@
                  trainable: bool = True,
                  intermediate_layers: Union[None, str, int, List[Union[str, int]]] = None):
         super().__init__(inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
         assert hasattr(model, "fe_compiled"), "must use fe.build to compile the model before use"
         self.intermediate_outputs = []  # [{device: Tensor}]
         intermediate_layers = to_list(intermediate_layers)
         if intermediate_layers and get_num_devices() > 1:
-            print("\033[93m {}\033[00m".format(
-                "FastEstimator-Warn: Layer names / ids may be different between single-gpu and multi-gpu environments"))
+            warn("Layer names / ids may be different between single-gpu and multi-gpu environments")
         for intermediate_layer in intermediate_layers:
             storage = {}
             if isinstance(model, tf.keras.Model):
                 layers = list(model._flatten_layers(include_self=False, recursive=True))
                 if isinstance(intermediate_layer, int):
                     intermediate_layer = layers[intermediate_layer]
                 else:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/model/update.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/model/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 import tensorflow as tf
 import torch
 
 from fastestimator.backend._get_gradient import get_gradient
 from fastestimator.backend._reduce_mean import reduce_mean
 from fastestimator.backend._update_model import update_model
 from fastestimator.op.tensorop.tensorop import TensorOp
+from fastestimator.util.base_util import to_set, warn
 from fastestimator.util.traceability_util import traceable
-from fastestimator.util.base_util import to_set
+from fastestimator.util.util import get_num_gpus
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 
 
 @traceable()
 class UpdateOp(TensorOp):
@@ -55,14 +56,16 @@
     Raise:
         ValueError: When model is mixed-precision and `gradients` is provided.
         ValueError: Network framework is not one of "tf" or "torch".
         ValueError: `merge_grad` is larger than 1 in multi-GPU configuration.
         RuntimeError: If attempting to modify a PyTorch model which relied on gradients within a different PyTorch model
             which has in turn already undergone a non-deferred update.
     """
+    _old_defer: bool  # Used by the Network to automagically fix defer values
+
     def __init__(self,
                  model: Union[tf.keras.Model, torch.nn.Module],
                  loss_name: str,
                  gradients: Optional[str] = None,
                  mode: Union[None, str, Iterable[str]] = "train",
                  ds_id: Union[None, str, Iterable[str]] = None,
                  merge_grad: int = 1,
@@ -71,19 +74,19 @@
         if gradients is None:
             super().__init__(inputs=loss_name, outputs=None, mode=mode, ds_id=ds_id)
         else:
             if model.mixed_precision:
                 raise ValueError("Mixed precision training cannot take input gradients, because the gradients need to "
                                  "be computed in this module")
             if self.extra_loss:
-                print("FastEstimator-Warn: Extra model losses are detected and they will be ignored since the gradients"
-                      " are not computed in UpdateOp class.")
+                warn("Extra model losses are detected and they will be ignored since the gradients are not computed " +
+                     "in UpdateOp class.")
             super().__init__(inputs=gradients, outputs=None, mode=mode, ds_id=ds_id)
 
-        if torch.cuda.device_count() > 1 and merge_grad > 1:
+        if get_num_gpus() > 1 and merge_grad > 1:
             raise ValueError("Currently FastEstimator doesn't support merge_grad feature in multi-GPU configuration "
                              "and thus 'merge_grad' cannot be larger than 1")
 
         if not hasattr(model, "loss_name"):
             model.loss_name = {loss_name}
         else:
             model.loss_name.add(loss_name)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/permute.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/resize3d.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/tensorop.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/op/tensorop/un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/op/tensorop/un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/pipeline.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,25 @@
 
 import numpy as np
 import tensorflow as tf
 from torch.utils.data import DataLoader, Dataset
 
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.dataset.dataloader import FEDataLoader
-from fastestimator.dataset.op_dataset import OpDataset, _DelayedDeepDict
+from fastestimator.dataset.op_dataset import OpDataset
 from fastestimator.op.numpyop.meta.fuse import Fuse
 from fastestimator.op.numpyop.meta.one_of import OneOf
 from fastestimator.op.numpyop.meta.repeat import Repeat
 from fastestimator.op.numpyop.meta.sometimes import Sometimes
-from fastestimator.op.numpyop.numpyop import NumpyOp, forward_numpyop, Batch
-from fastestimator.schedule.schedule import Scheduler, get_current_items, EpochScheduler, \
-    RepeatScheduler
+from fastestimator.op.numpyop.numpyop import Batch, NumpyOp, forward_numpyop
+from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
+from fastestimator.util.base_util import to_list, to_set, warn
 from fastestimator.util.data import FilteredData
 from fastestimator.util.traceability_util import traceable
 from fastestimator.util.util import cpu_count, get_num_devices
-from fastestimator.util.base_util import to_set, to_list
 
 DataSource = TypeVar('DataSource', Dataset, DataLoader, tf.data.Dataset)
 
 
 @traceable(blacklist=('ctx_loader', 'ctx_lock'))
 class Pipeline:
     """A data pipeline class that takes care of data pre-processing.
@@ -52,23 +51,24 @@
         train_data: The training data, or None if no training data is available.
         eval_data: The evaluation data, or None if no evaluation data is available.
         test_data: The testing data, or None if no evaluation data is available.
         batch_size: The batch size to be used by the pipeline. If the batch_size is also set by a Batch Op, that value
             will take precedence over this one (for example, if you want to set the batch_size based on mode or ds_is).
             NOTE: This argument is only applicable when using a FastEstimator Dataset.
             NOTE: This is the global batch size regardless of the number of GPUs available in the machine. If you have
-                multiple (N) GPUs, each will recieve batch_size/N elements during a training step.
+                multiple (N) GPUs, each will receive batch_size/N elements during a training step.
         ops: NumpyOps to be used for pre-processing. NOTE: This argument is only applicable when using a FastEstimator
             Dataset.
         num_process: Number of CPU threads to use for data pre-processing. NOTE: This argument is only applicable when
             using a FastEstimator Dataset. None will default to min(n_cpus, max(32, 32*n_gpus)). Multiprocessing can be
             disabled by passing 0 here, which can be useful for debugging.
     """
+    mp_warned: bool = False
     ops: List[Union[NumpyOp, Scheduler[NumpyOp]]]
-    data: Dict[str, Dict[Optional[str], Union[DataSource, Scheduler[DataSource]]]]  # {"mode": {"ds_id": ds}}
+    data: Dict[str, Dict[str, Union[DataSource, Scheduler[DataSource]]]]  # {"mode": {"ds_id": ds}}
 
     def __init__(self,
                  train_data: Union[None,
                                    DataSource,
                                    Scheduler[DataSource],
                                    Dict[str, Union[DataSource, Scheduler[DataSource]]]] = None,
                  eval_data: Union[None, DataSource, Scheduler[DataSource], Dict[str, DataSource]] = None,
@@ -78,18 +78,19 @@
                  num_process: Optional[int] = None):
         data = {x: y for (x, y) in zip(["train", "eval", "test"], [train_data, eval_data, test_data]) if y}
         self.data = self._register_ds_ids(data)
         self.batch_size = batch_size
         self.ops = to_list(ops)
         if mp.get_start_method(allow_none=True) is None and os.name != 'nt':
             mp.set_start_method('fork')
-        if mp.get_start_method(allow_none=True) != 'fork':
-            print("FastEstimator-Warn: Pipeline multiprocessing is disabled. OS must support the 'fork' start method.")
-            num_process = 0
         self.num_process = num_process if num_process is not None else min(cpu_count(), 32 * get_num_devices())
+        if mp.get_start_method(allow_none=True) != 'fork' and self.num_process > 0 and not self.mp_warned:
+            warn("Pipeline multiprocessing is disabled. OS must support the 'fork' start method.")
+            self.num_process = 0
+            self.mp_warned = True
         self._verify_inputs(**{k: v for k, v in locals().items() if k != 'self'})
         # Loader Variables
         self.ctx_lock = Lock()
         self.ctx_mode = 'train'
         self.ctx_epoch = 1
         self.ctx_shuffle = True
         self.ctx_output_keys = None
@@ -99,17 +100,16 @@
         self.ctx_ops = []
         self.ctx_batch_info = Batch()
         self.ctx_batch_ops = []
         self.ctx_batch_input_keys = set()
 
     @staticmethod
     def _register_ds_ids(
-            data: Dict[
-                str, Union[DataSource, Scheduler[DataSource], Dict[str, Union[DataSource, Scheduler[DataSource]]]]]
-    ) -> Dict[str, Dict[Optional[str], Union[DataSource, Scheduler[DataSource]]]]:
+        data: Dict[str, Union[DataSource, Scheduler[DataSource], Dict[str, Union[DataSource, Scheduler[DataSource]]]]]
+    ) -> Dict[str, Dict[str, Union[DataSource, Scheduler[DataSource]]]]:
         """Associate dataset of each mode with a `ds_id`.
 
         Args:
             data: A dictionary with mode as key, dataset as value.
         """
         forbidden_ds_id_chars = {":", "!", ";", "|"}
         for mode, dataset in data.items():
@@ -162,16 +162,18 @@
                         else:
                             # Some unknown scheduler, no known shortcuts so just try first 100 epochs to be safe
                             schedule_epochs |= {*range(1, 100)}
                         break
         # After m*n steps all possible m and n combinations will be visited
         schedule_cycles = functools.reduce(mul, schedule_cycles, 1)
         # Consider x + m*n epochs for each epoch scheduler x value
-        schedule_epochs = sorted({epoch for base_epoch in schedule_epochs for epoch in
-                                  list(range(base_epoch, base_epoch + schedule_cycles))})
+        schedule_epochs = sorted({
+            epoch
+            for base_epoch in schedule_epochs for epoch in list(range(base_epoch, base_epoch + schedule_cycles))
+        })
         for mode, id_ds in self.data.items():
             for ds_id in id_ds.keys():
                 for epoch in schedule_epochs:
                     ops = get_current_items(batch_ops, run_modes=mode, epoch=epoch, ds_id=ds_id)
                     # We have to do an instance check again since the user could technically use a scheduler that has a
                     # Batch Op at one point, but some other Op (or None) at a different point
                     ops = [op for op in ops if isinstance(op, Batch)]
@@ -199,19 +201,19 @@
             for op in get_current_items(self.ops):
                 assert isinstance(op, NumpyOp), "unsupported op format, must provide NumpyOp in Pipeline"
             # num_process check
             assert isinstance(self.num_process, int), "number of processes must be an integer"
             return True
         elif isinstance(dataset, (DataLoader, tf.data.Dataset)):
             if kwargs['batch_size'] is not None:
-                print("FastEstimator-Warn: batch_size will only be used for built-in dataset")
+                warn("batch_size will only be used for built-in dataset")
             if kwargs['ops'] is not None:
-                print("FastEstimator-Warn: ops will only be used for built-in dataset")
+                warn("ops will only be used for built-in dataset")
             if kwargs['num_process'] is not None:
-                print("FastEstimator-Warn: num_process will only be used for built-in dataset")
+                warn("num_process will only be used for built-in dataset")
             return False
         else:
             raise ValueError("Unsupported dataset type: {}".format(type(dataset)))
 
     def _get_op_split(self, mode: str, epoch: int, ds_id: str) -> Tuple[List[NumpyOp], Batch, List[NumpyOp]]:
         """Figure out which ops are pre-batch vs post-batch.
 
@@ -253,15 +255,15 @@
                 for dataset in datasets.values():
                     if isinstance(dataset, Scheduler):
                         dataset = dataset.get_current_value(epoch)
                     if dataset:
                         all_modes.append(mode)
         return to_set(all_modes)
 
-    def get_ds_ids(self, epoch: int, mode: str) -> List[Union[str, None]]:
+    def get_ds_ids(self, epoch: int, mode: str) -> List[str]:
         """Get the ds_ids for a given epoch and mode.
 
         Args:
             epoch: The current epoch index.
             mode: The current execution mode.
 
         Returns:
@@ -408,18 +410,20 @@
                                             ", ".join([sub_op.__class__.__name__ for sub_op in op.ops]) + ")")
                         elif isinstance(op, Batch):
                             op_names.append("<Collating Batch>")
                         else:
                             op_names.append(op.__class__.__name__)
 
                     max_op_len = max(len(op_name) for op_name in op_names)
-                    max_in_len = max([len(", ".join(op.inputs)) for op in
-                                      self.ctx_ops + [self.ctx_batch_info] + self.ctx_batch_ops] + [len("Inputs")])
-                    max_out_len = max([len(", ".join(op.outputs)) for op in
-                                       self.ctx_ops + [self.ctx_batch_info] + self.ctx_batch_ops] + [len("Outputs")])
+                    max_in_len = max(
+                        [len(", ".join(op.inputs))
+                         for op in self.ctx_ops + [self.ctx_batch_info] + self.ctx_batch_ops] + [len("Inputs")])
+                    max_out_len = max([
+                        len(", ".join(op.outputs)) for op in self.ctx_ops + [self.ctx_batch_info] + self.ctx_batch_ops
+                    ] + [len("Outputs")])
                     ms_visit_len = max(len("{:.3f}".format(max(normalized_times_ms))), len("ms / Visit"))
                     visit_len = max(len(f"{int(np.max(duration_list[:, 0]))}"), len("Visits"))
 
                     print("{}: {}: {}: {}: {}: {}".format("Op".ljust(max_op_len + 1),
                                                           "Inputs".ljust(max_in_len + 1),
                                                           "Outputs".ljust(max_out_len + 1),
                                                           "ms / Visit".ljust(ms_visit_len + 1),
@@ -431,16 +435,18 @@
                             op_names[i + 1].ljust(max_op_len + 1),
                             ", ".join(op.inputs).ljust(max_in_len + 1),
                             ", ".join(op.outputs).ljust(max_out_len + 1),
                             "{:.3f}".format(normalized_times_ms[i]).ljust(ms_visit_len + 1),
                             str(int(duration_list[i][0])).ljust(visit_len + 1),
                             100 * duration_list[i][1] / total_time))
                     if self.ctx_batch_ops:
-                        penalty = round(100*(duration_list[len(self.ctx_ops)][1] - extra_memory_management_time) /
-                                        duration_list[len(self.ctx_ops)][1], 1)
+                        penalty = round(
+                            100 * (duration_list[len(self.ctx_ops)][1] - extra_memory_management_time) /
+                            duration_list[len(self.ctx_ops)][1],
+                            1)
                         print(f"\nNote that collation time would be cut by ~{penalty}% if there were no batched ops.")
                 print("\n")  # to make printing more obvious
 
     def get_scheduled_items(self, mode: str) -> List[Any]:
         """Get a list of items considered for scheduling.
 
         Args:
@@ -471,19 +477,15 @@
                 epochs_with_data = epochs_with_data | epochs_with_data_ds
             elif dataset:
                 epochs_with_data_ds = set(range(1, total_epochs + 1))
                 epochs_with_data = epochs_with_data | epochs_with_data_ds
                 break
         return epochs_with_data
 
-    def transform(self,
-                  data: Dict[str, Any],
-                  mode: str,
-                  epoch: int = 1,
-                  ds_id: str = '',
+    def transform(self, data: Dict[str, Any], mode: str, epoch: int = 1, ds_id: str = '',
                   target_type: str = 'np') -> Union[Dict[str, Any], FilteredData]:
         """Apply all pipeline operations on a given data instance for the specified `mode` and `epoch`.
 
         Args:
             data: Input data in dictionary format.
             mode: The execution mode in which to run. This can be "train", "eval", "test" or "infer".
             epoch: The epoch index to run. Note that epoch indices are 1-indexed.
@@ -673,13 +675,13 @@
 def _batch_postprocess(data: Dict[str, Any], ops: List[NumpyOp], output_keys: Set[str], mode: str) -> \
         Union[Dict[str, Any], FilteredData]:
     op_data = forward_numpyop(ops=ops, data=data, state={'mode': mode}, batched='torch')
     if isinstance(op_data, FilteredData):
         return op_data
     if output_keys:
         for key in data.keys() - output_keys:
-            if key not in _DelayedDeepDict.warned:
-                _DelayedDeepDict.warned.add(key)
-                print("FastEstimator-Warn: the key '{}' is being pruned since it is unused outside of the Pipeline."
-                      " To prevent this, you can declare the key as an input of a Trace or TensorOp.".format(key))
+            if key not in OpDataset.warned:
+                OpDataset.warned.add(key)
+                warn(f"The key '{key}' is being pruned since it is unused outside of the Pipeline. To prevent this, "
+                     "you can declare the key as an input of a Trace or TensorOp.")
             data.pop(key)
     return data
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # ==============================================================================
 from typing import TYPE_CHECKING
 
 import lazy_loader as lazy
 
 __getattr__, __dir__, __all__ = lazy.attach(__name__,
                                             submod_attrs={
-                                                'lr_shedule': ['ARC', 'cosine_decay'],
+                                                'lr_schedule': ['ARC', 'cosine_decay'],
                                                 'schedule': ['EpochScheduler', 'RepeatScheduler', 'Scheduler',
                                                              'get_current_items', 'get_signature_epochs'],
                                             })
 
 if TYPE_CHECKING:
-    from fastestimator.schedule.lr_shedule import ARC, cosine_decay
+    from fastestimator.schedule.lr_schedule import ARC, cosine_decay
     from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items, \
         get_signature_epochs
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/lr_shedule.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/schedule/schedule.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/schedule/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union
+from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union, overload
 
-from fastestimator.util.traceability_util import is_restorable, traceable
 from fastestimator.util.base_util import to_set
+from fastestimator.util.traceability_util import is_restorable, traceable
 
 T = TypeVar('T')
+T2 = TypeVar('T2')
 
 
 @traceable()
 class Scheduler(Generic[T]):
     """A class which can wrap things like Datasets and Ops to make their behavior epoch-dependent.
     """
     def get_current_value(self, epoch: int) -> Optional[T]:
@@ -181,18 +182,34 @@
         epoch_config = get_current_items(items, run_modes=mode, epoch=epoch, ds_id=ds_id)
         if epoch_config not in unique_configs:
             unique_configs.append(epoch_config)
             signature_epochs.append(epoch)
     return signature_epochs
 
 
+@overload
 def get_current_items(items: Iterable[Union[T, Scheduler[T]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
                       ds_id: Optional[str] = None) -> List[T]:
+    ...
+
+
+@overload
+def get_current_items(items: Iterable[Union[T, T2, Scheduler[T], Scheduler[T2]]],
+                      run_modes: Optional[Union[str, Iterable[str]]] = None,
+                      epoch: Optional[int] = None,
+                      ds_id: Optional[str] = None) -> List[Union[T, T2]]:
+    ...
+
+
+def get_current_items(items: Iterable[Union[Any, Scheduler[Any]]],
+                      run_modes: Optional[Union[str, Iterable[str]]] = None,
+                      epoch: Optional[int] = None,
+                      ds_id: Optional[str] = None) -> List[Any]:
     """Select items which should be executed for given mode and epoch.
 
     Args:
         items: A list of possible items or Schedulers of items to choose from.
         run_modes: The desired execution mode. One or more of "train", "eval", "test", or "infer". If None, items of
             all modes will be returned.
         epoch: The desired execution epoch. If None, items across all epochs will be returned.
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/golden_section.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/golden_section.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/grid_search.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/search.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/cartesian.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/cartesian.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/heatmap.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/heatmap.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/parallel_coordinate_plot.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/parallel_coordinate_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/vis_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/vis_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/search/visualize/visualize.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/search/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/history.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 import sys
 import threading
 import traceback
 from collections import defaultdict
 from contextlib import closing
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Type
+from typing import Any, Dict, Iterable, List, Optional, TextIO, Type
 
-import tensorflow.keras.mixed_precision as mixed_precision
-import torch
+from keras import mixed_precision
 from prettytable import PrettyTable, from_db_cursor
 
 from fastestimator.schedule.schedule import Scheduler
 from fastestimator.summary.logs.log_parse import parse_log_iter
 from fastestimator.summary.logs.log_plot import visualize_logs
 from fastestimator.summary.summary import Summary, average_summaries
 from fastestimator.summary.system import System
+from fastestimator.util.base_util import NonContext, warn
 from fastestimator.util.cli_util import SaveAction, parse_string_to_python
-from fastestimator.util.util import cpu_count
-from fastestimator.util.base_util import NonContext
+from fastestimator.util.util import cpu_count, get_num_gpus
 
 _MAKE_HIST_TABLE = 'CREATE TABLE IF NOT EXISTS history (' \
                    'file TEXT, ' \
                    'experiment TEXT, ' \
                    'status TEXT, ' \
                    'args LIST[STR], ' \
                    'fe_version TEXT, ' \
@@ -125,23 +124,23 @@
     if db_path != ':memory:':  # This is a reserved keyword to create an in-memory database
         os.makedirs(os.path.dirname(db_path), exist_ok=True)  # Make sure folders exist before creating disk file
     connection = sql.connect(db_path, detect_types=sql.PARSE_DECLTYPES | sql.PARSE_COLNAMES)
     if db_path != ":memory:":
         # Check to ensure the database isn't corrupted
         cur = connection.execute("PRAGMA integrity_check")
         response = cur.fetchall()[0]
-        if response != ('ok',):
+        if response != ('ok', ):
             connection.close()
-            corrupt_path = os.path.join(os.path.dirname(db_path),
-                                        f"corrupt_{datetime.now().strftime('%Y_%m_%d_%H_%M_%S')}_"
-                                        f"{os.path.basename(db_path)}")
+            corrupt_path = os.path.join(
+                os.path.dirname(db_path),
+                f"corrupt_{datetime.now().strftime('%Y_%m_%d_%H_%M_%S')}_"
+                f"{os.path.basename(db_path)}")
             os.renames(db_path, corrupt_path)
-            print(f"FastEstimator-Warn: The FastEstimator history database has been corrupted. It has been moved to "
-                  f"{corrupt_path} and a new one has been automatically created. The integrity check output is: "
-                  f"{response}")
+            warn(f"The FastEstimator history database has been corrupted. It has been moved to {corrupt_path} and " +
+                 f"a new one has been automatically created. The integrity check output is: {response}")
             connection = sql.connect(db_path, detect_types=sql.PARSE_DECLTYPES | sql.PARSE_COLNAMES)
     connection.execute("PRAGMA foreign_keys = 1")  # Enable FK constraints
     connection.row_factory = sql.Row  # Get nice query return objects
     # Build the schema if it doesn't exist
     connection.execute(_MAKE_HIST_TABLE)
     connection.execute(_MAKE_FEAT_TABLE)
     connection.execute(_MAKE_DS_TABLE)
@@ -203,18 +202,19 @@
                    {'keep': n_keep})
     elif n_keep_logs is not None:
         db.execute("UPDATE settings SET n_keep_logs = MIN(n_keep, (?)) WHERE pk = 0", [n_keep_logs])
     db.commit()
     with closing(db.cursor()) as cursor:
         cursor.execute("SELECT * FROM settings")
         response = from_db_cursor(cursor)
-    # Hide implementation details from end user
-    response.del_column('pk')
-    response.del_column('schema_version')
-    print(response)
+    if response is not None:
+        # Hide implementation details from end user
+        response.del_column('pk')
+        response.del_column('schema_version')
+        print(response)
     db.close()
 
 
 class HistoryRecorder:
     """A class to record what you're doing.
 
     This class is intentionally not @traceable.
@@ -224,25 +224,28 @@
 
     Args:
         system: The system object corresponding to the current training.
         est_path: The path to the file responsible for creating the current estimator (this is for bookkeeping, it can
             technically be any string).
         db_path: The path to the database, or None to use the default location.
     """
+    db: sql.Connection
+    stdout: TextIO
+
     def __init__(self, system: System, est_path: str, db_path: Optional[str] = None):
         # Prepare db adapters
         sql.register_adapter(bool, int)
         sql.register_converter("BOOL", lambda v: bool(int(v)))
         sql.register_adapter(list, str)
         sql.register_converter("LIST[STR]", lambda v: parse_string_to_python(v))
         # Prepare variables
         self.filename = os.path.basename(est_path)
         self.db_path = db_path if db_path else os.path.join(str(Path.home()), 'fastestimator_data', 'history.db')
         self.system = system
-        self.db = None
+        self.db = None  # type: ignore
         self.ident = (multiprocessing.current_process().pid, threading.get_ident())
         self.pk = None
         self.stdout = None
 
     def __enter__(self) -> None:
         self.db = connect(self.db_path)
         self.ident = (multiprocessing.current_process().pid, threading.get_ident())
@@ -258,15 +261,15 @@
                     'pk': self.pk,
                     'fname': self.filename,
                     'status': 'Launched',
                     'exp': self.system.summary.name,
                     'args': sys.argv[1:],
                     'version': sys.modules['fastestimator'].__version__,
                     'start': datetime.now(),
-                    'gpus': torch.cuda.device_count(),
+                    'gpus': get_num_gpus(),
                     'cpus': cpu_count(),
                     'workers': self.system.pipeline.num_process
                 })
             self.db.executemany(_MAKE_FEAT_ENTRY, self._get_features_in_use())
             self.db.executemany(_MAKE_DS_ENTRY, self._get_datasets_in_use())
             self.db.executemany(_MAKE_PIPE_ENTRY, self._get_items_in_use(self.system.pipeline.ops))
             self.db.executemany(_MAKE_NET_ENTRY, self._get_items_in_use(self.system.network.ops))
@@ -304,16 +307,15 @@
                 self.db.execute(_MAKE_ERR_ENTRY_P2, args)
             self.db.commit()
             self._apply_limits()
         except (sql.OperationalError, sql.DatabaseError) as err:
             # This could happen if user has multiple trainings running simultaneously, the database becomes corrupted,
             # and then a new training is launched which detects the corrupted database of the old training and re-names
             # the old database before the old job completes.
-            print(f"FastEstimator-Warn: FastEstimator history tracking failed to capture the final status of the "
-                  f"experiment: {err}")
+            warn(f"FastEstimator history tracking failed to capture the final status of the experiment: {err}")
         self.db.close()
 
     def _check_for_restart(self) -> None:
         """Determine whether a training has been restarted via RestoreWizard. If so, update the history accordingly.
 
         If RestoreWizard has been invoked, then the system exp_id will have changed since self.pk was initialized. This
         method will do related bookkeeping, and then swap self.pk for the restored id.
@@ -409,16 +411,16 @@
             # dropped.
             try:
                 self._check_for_restart()  # Check here instead of waiting for __exit__ in case system powers off later
                 self.db.execute('UPDATE logs SET log = log || (?) WHERE fk = (?)', [output, self.pk])
                 self.db.commit()
             except (sql.OperationalError, sql.DatabaseError) as err:
                 self.ident = (-2, -2)  # No threads should match this identity in the future
-                print(f"\nFastEstimator-Warn: There was a problem writing to the FastEstimator history database. Log "
-                      f"capture will be disabled for the rest of this experiment. Error: {err}")
+                warn("There was a problem writing to the FastEstimator history database. Log " +
+                     f"capture will be disabled for the rest of this experiment. Error: {err}")
 
     def flush(self) -> None:
         self.stdout.flush()
 
 
 class HistoryReader:
     """A class to read history information from the database.
@@ -431,17 +433,19 @@
     with HistoryReader() as reader:
         reader.read_basic()
     ```
 
     Args:
         db_path: The path to the database, or None to use the default location.
     """
+    db: sql.Connection
+
     def __init__(self, db_path: Optional[str] = None):
         self.db_path = db_path
-        self.db = None  # sql.Connection
+        self.db = None  # type: ignore
         self.response = None  # List[sql.Row]
 
     def __enter__(self) -> 'HistoryReader':
         self.db = connect(self.db_path)
         self.db.set_trace_callback(print)  # Show the query in case user wants to adapt it later
         return self
 
@@ -606,15 +610,15 @@
 
         Args:
             subparsers: The parser object to be appended to.
         """
         p_log = subparsers.add_parser(
             'log',
             description='Retrieve one or more output logs. This command requires '
-                        'that you currently have experiments selected.',
+            'that you currently have experiments selected.',
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             allow_abbrev=False)
         p_log.add_argument('indices',
                            metavar='I',
                            type=int,
                            nargs='+',
                            help="Indices of experiments for which to print logs")
@@ -633,16 +637,16 @@
         """Add an error parser to an existing argparser.
 
         Args:
             subparsers: The parser object to be appended to.
         """
         p_err = subparsers.add_parser(
             'err',
-            description='Retrieve one or more error tracebacks. This command requires '
-                        'that you currently have experiments selected.',
+            description='Retrieve one or more error tracebacks. This command requires that you currently have \
+                experiments selected.',
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             allow_abbrev=False)
         p_err.add_argument('indices',
                            metavar='I',
                            type=int,
                            nargs='+',
                            help="Indices of experiments for which to print error tracebacks")
@@ -652,16 +656,16 @@
         """Add a visualization parser to an existing argparser.
 
         Args:
             subparsers: The parser object to be appended to.
         """
         p_vis = subparsers.add_parser(
             'vis',
-            description='Visualize logs for one or more experiments. This command requires '
-                        'that you currently have experiments selected.',
+            description='Visualize logs for one or more experiments. This command requires that you currently '
+            'have experiments selected.',
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             allow_abbrev=False)
         p_vis.add_argument('indices',
                            metavar='idx',
                            type=int,
                            nargs='*',
                            help="Indices of experiments for which to print logs")
@@ -824,15 +828,14 @@
             for group_name, group_indices in args['groups'].items():
                 if idx in group_indices:
                     groups[group_name].append(experiment)
         experiments = [average_summaries(name, exps) for name, exps in groups.items()]
         visualize_logs(experiments,
                        save_path=save_dir,
                        smooth_factor=args['smooth'],
-                       share_legend=args['share_legend'],
                        pretty_names=args['pretty_names'],
                        ignore_metrics=args['ignore'],
                        include_metrics=args['include'])
 
 
 class _GroupAction(argparse._AppendAction):
     """An argparse action which can be invoked multiple times in order to build a dictionary of entries.
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/log_parse.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/log_parse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/logs/log_plot.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/logs/log_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 # ==============================================================================
 import math
 import re
 import tempfile
 from collections import defaultdict
 from itertools import cycle
-from typing import Any, Dict, List, Optional, Set, Union, Tuple
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import plotly.graph_objects as go
 from natsort import humansorted
 from plotly.io import _html, _kaleido
 from plotly.offline.offline import get_plotlyjs
 from plotly.subplots import make_subplots
 from scipy.ndimage.filters import gaussian_filter1d
 
 from fastestimator.summary.summary import Summary, ValWithError
-from fastestimator.util.base_util import get_colors, to_set, to_list, prettify_metric_name, in_notebook, FigureFE
+from fastestimator.util.base_util import FigureFE, get_colors, in_notebook, prettify_metric_name, to_list, to_set, warn
 
 
 class _MetricGroup:
     """A class for wrapping the values recorded for a given metric based on its experiment id and mode.
 
     This class is intentionally not @traceable.
     """
@@ -235,16 +235,15 @@
 
     metric_list = list(sorted(metric_histories.keys()))
     if len(metric_list) == 0:
         return FigureFE.from_figure(make_subplots())
     ds_ids = humansorted(ds_ids)  # Sort them to have consistent ordering (and thus symbols) between plot runs
     n_plots = len(metric_list)
     if len(ds_ids) > 9:  # 9 b/c None is included
-        print("FastEstimator-Warn: Plotting more than 8 different datasets isn't well supported. Symbols will be "
-              "reused.")
+        warn("Plotting more than 8 different datasets isn't well supported. Symbols will be reused.")
 
     # Non-Shared legends aren't supported yet. If they get supported then maybe can have that feature here too.
     #  https://github.com/plotly/plotly.js/issues/5099
     #  https://github.com/plotly/plotly.js/issues/5098
 
     # map the metrics into an n x n grid, then remove any extra columns. Final grid will be n x m with m <= n
     n_rows = math.ceil(math.sqrt(n_plots))
@@ -263,21 +262,29 @@
         metric_grid_location[metric] = (idx // n_cols, idx % n_cols)
         idx += 1
     titles = [k for k, v in sorted(list(metric_grid_location.items()), key=lambda e: e[1][0] * n_cols + e[1][1])]
     if pretty_names:
         titles = [prettify_metric_name(title) for title in titles]
 
     fig = make_subplots(rows=n_rows, cols=n_cols, subplot_titles=titles, shared_xaxes='all')
-    fig.update_layout({'plot_bgcolor': '#FFF',
-                       'hovermode': 'closest',
-                       'margin': {'t': 50},
-                       'modebar': {'add': ['hoverclosest', 'hovercompare'],
-                                   'remove': ['select2d', 'lasso2d']},
-                       'legend': {'tracegroupgap': 5,
-                                  'font': {'size': 11}}})
+    fig.update_layout({
+        'plot_bgcolor': '#FFF',
+        'hovermode': 'closest',
+        'margin': {
+            't': 50
+        },
+        'modebar': {
+            'add': ['hoverclosest', 'hovercompare'], 'remove': ['select2d', 'lasso2d']
+        },
+        'legend': {
+            'tracegroupgap': 5, 'font': {
+                'size': 11
+            }
+        }
+    })
 
     # Set x-labels
     for idx, metric in enumerate(titles, start=1):
         plotly_idx = idx if idx > 1 else ""
         x_axis_name = f'xaxis{plotly_idx}'
         y_axis_name = f'yaxis{plotly_idx}'
         if metric_histories[metric].ndim() > 1:
@@ -372,34 +379,36 @@
                                 y_max = y.y_max
                                 y = y.y
                             marker_style = 'circle' if mode == 'train' else 'diamond' if mode == 'eval' \
                                 else 'square' if mode == 'test' else 'hexagram'
                             limit_data = [(y_max, y_min)] if y_max is not None and y_min is not None else None
                             tip_text = "%{x}: (%{customdata[1]:.3f}, %{y:.3f}, %{customdata[0]:.3f})" if \
                                 limit_data is not None else "%{x}: %{y:.3f}"
-                            error_y = None if limit_data is None else {'type': 'data',
-                                                                       'symmetric': False,
-                                                                       'array': [y_max - y],
-                                                                       'arrayminus': [y - y_min]}
-                            z_order[2].append((go.Scatter(x=[x],
-                                                          y=[y],
-                                                          name=title,
-                                                          legendgroup=title,
-                                                          customdata=limit_data,
-                                                          hovertemplate=tip_text,
-                                                          mode='markers',
-                                                          marker={'color': color,
-                                                                  'size': 12,
-                                                                  'symbol': _symbol_mash(marker_style,
-                                                                                         ds_id_markers[ds_id]),
-                                                                  'line': {'width': 1.5,
-                                                                           'color': 'White'}},
-                                                          error_y=error_y,
-                                                          showlegend=add_label[exp_idx][mode][ds_id]['patch'],
-                                                          legendrank=legend_order[title]),
+                            error_y = None if limit_data is None else {
+                                'type': 'data', 'symmetric': False, 'array': [y_max - y], 'arrayminus': [y - y_min]
+                            }
+                            z_order[2].append((go.Scatter(
+                                x=[x],
+                                y=[y],
+                                name=title,
+                                legendgroup=title,
+                                customdata=limit_data,
+                                hovertemplate=tip_text,
+                                mode='markers',
+                                marker={
+                                    'color': color,
+                                    'size': 12,
+                                    'symbol': _symbol_mash(marker_style, ds_id_markers[ds_id]),
+                                    'line': {
+                                        'width': 1.5, 'color': 'White'
+                                    }
+                                },
+                                error_y=error_y,
+                                showlegend=add_label[exp_idx][mode][ds_id]['patch'],
+                                legendrank=legend_order[title]),
                                                row,
                                                col))
                             add_label[exp_idx][mode][ds_id]['patch'] = False
                         else:
                             # We can draw a line
                             y = data[:, 1]
                             y_min = None
@@ -418,31 +427,36 @@
                             x = data[:, 0]
                             linestyle = 'solid' if mode == 'train' else 'dash' if mode == 'eval' else 'dot' if \
                                 mode == 'test' else 'dashdot'
                             limit_data = [(mx, mn) for mx, mn in zip(y_max, y_min)] if y_max is not None and y_min is \
                                                                                        not None else None
                             tip_text = "%{x}: (%{customdata[1]:.3f}, %{y:.3f}, %{customdata[0]:.3f})" if \
                                 limit_data is not None else "%{x}: %{y:.3f}"
-                            z_order[1].append((go.Scatter(x=x,
-                                                          y=y,
-                                                          name=title,
-                                                          legendgroup=title,
-                                                          mode="lines+markers" if ds_id_markers[ds_id] else 'lines',
-                                                          marker={'color': color,
-                                                                  'size': 8,
-                                                                  'line': {'width': 2,
-                                                                           'color': 'DarkSlateGrey'},
-                                                                  'maxdisplayed': 10,
-                                                                  'symbol': ds_id_markers[ds_id]},
-                                                          line={'dash': linestyle,
-                                                                'color': color},
-                                                          customdata=limit_data,
-                                                          hovertemplate=tip_text,
-                                                          showlegend=add_label[exp_idx][mode][ds_id]['line'],
-                                                          legendrank=legend_order[title]),
+                            z_order[1].append((go.Scatter(
+                                x=x,
+                                y=y,
+                                name=title,
+                                legendgroup=title,
+                                mode="lines+markers" if ds_id_markers[ds_id] else 'lines',
+                                marker={
+                                    'color': color,
+                                    'size': 8,
+                                    'line': {
+                                        'width': 2, 'color': 'DarkSlateGrey'
+                                    },
+                                    'maxdisplayed': 10,
+                                    'symbol': ds_id_markers[ds_id]
+                                },
+                                line={
+                                    'dash': linestyle, 'color': color
+                                },
+                                customdata=limit_data,
+                                hovertemplate=tip_text,
+                                showlegend=add_label[exp_idx][mode][ds_id]['line'],
+                                legendrank=legend_order[title]),
                                                row,
                                                col))
                             add_label[exp_idx][mode][ds_id]['line'] = False
                             if limit_data is not None:
                                 z_order[0].append((go.Scatter(x=x,
                                                               y=y_max,
                                                               mode='lines',
@@ -518,18 +532,17 @@
     """
     base_table = {'circle': 0, 'diamond': 2, 'square': 1, 'hexagram': 18}
     if ds_symbol is None:
         return base_table[base_symbol]
     ds_offsets = {37: 0, 38: 1, 39: 2, 40: 3, 34: 4, 33: 5, 35: 6, 36: 7}
     slots = {i for i in range(53)} - set(base_table.values()) - set(ds_offsets.keys())
     slots = sorted(list(slots))
-    base_offsets = {'circle': 0,
-                    'diamond': len(ds_offsets),
-                    'square': 2 * len(ds_offsets),
-                    'hexagram': 3 * len(ds_offsets)}
+    base_offsets = {
+        'circle': 0, 'diamond': len(ds_offsets), 'square': 2 * len(ds_offsets), 'hexagram': 3 * len(ds_offsets)
+    }
     mashed_symbol = slots[base_offsets[base_symbol] + ds_offsets[ds_symbol]]
     return mashed_symbol
 
 
 def _get_vars(symbol: Union[str, int]) -> str:
     """Get the javascript variable declarations associated with a given symbol.
 
@@ -538,53 +551,65 @@
     Args:
         symbol: The symbol whose variables should be retrieved.
 
     Returns:
         A minified string representation of the variables to be declared in javascript.
     """
     if isinstance(symbol, str):
-        return {'circle': 'var b1=n.round(t,2);',
-                'square': 'var b1=n.round(t,2);',
-                'diamond': 'var b1=n.round(t*1.3,2);',
-                'hexagram': 'var b1=n.round(t,2);var b2=n.round(t/2,2);var b3=n.round(t*Math.sqrt(3)/2,2);'}[symbol]
-    return {37: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
-            38: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
-            39: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
-            40: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
-            34: 'var d1=n.round(t,2);',
-            33: 'var d1=n.round(t*1.4,2);',
-            35: 'var d1=n.round(t*1.2,2);var d2=n.round(t*0.85,2);',
-            36: 'var d1=n.round(t/2,2);var d2=n.round(t,2);'}[symbol]
+        return {
+            'circle': 'var b1=n.round(t,2);',
+            'square': 'var b1=n.round(t,2);',
+            'diamond': 'var b1=n.round(t*1.3,2);',
+            'hexagram': 'var b1=n.round(t,2);var b2=n.round(t/2,2);var b3=n.round(t*Math.sqrt(3)/2,2);'
+        }[symbol]
+    return {
+        37: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
+        38: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
+        39: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
+        40: 'var d1=n.round(t*1.2,2);var d2=n.round(t*1.6,2);var d3=n.round(t*0.8,2);',
+        34: 'var d1=n.round(t,2);',
+        33: 'var d1=n.round(t*1.4,2);',
+        35: 'var d1=n.round(t*1.2,2);var d2=n.round(t*0.85,2);',
+        36: 'var d1=n.round(t/2,2);var d2=n.round(t,2);'
+    }[symbol]
 
 
 def _get_paths(symbol: Union[str, int]) -> str:
     """Get the javascript pen paths associated with a given symbol.
 
     These are adapted from plotly.js -> src/components/drawing/symbol_defs.js
 
     Args:
         symbol: The symbol whose pen paths should be retrieved.
 
     Returns:
         A minified string representation of the paths to be declared in javascript.
     """
     if isinstance(symbol, str):
-        return {'circle': '"M"+b1+",0A"+b1+","+b1+" 0 1,1 0,-"+b1+"A"+b1+","+b1+" 0 0,1 "+b1+",0Z"',
-                'square': '"M"+b1+","+b1+"H-"+b1+"V-"+b1+"H"+b1+"Z"',
-                'diamond': '"M"+b1+",0L0,"+b1+"L-"+b1+",0L0,-"+b1+"Z"',
-                'hexagram': '"M-"+b3+",0l-"+b2+",-"+b1+"h"+b3+"l"+b2+",-"+b1+"l"+b2+","+b1+"h"+b3+"l-"+b2+","+b1+"l"+'
-                            'b2+","+b1+"h-"+b3+"l-"+b2+","+b1+"l-"+b2+",-"+b1+"h-"+b3+"Z"'}[symbol]
-    return {37: '"M-"+d1+","+d3+"L0,0M"+d1+","+d3+"L0,0M0,-"+d2+"L0,0"',
-            38: '"M-"+d1+",-"+d3+"L0,0M"+d1+",-"+d3+"L0,0M0,"+d2+"L0,0"',
-            39: '"M"+d3+","+d1+"L0,0M"+d3+",-"+d1+"L0,0M-"+d2+",0L0,0"',
-            40: '"M-"+d3+","+d1+"L0,0M-"+d3+",-"+d1+"L0,0M"+d2+",0L0,0"',
-            34: '"M"+d1+","+d1+"L-"+d1+",-"+d1+"M"+d1+",-"+d1+"L-"+d1+","+d1',
-            33: '"M0,"+d1+"V-"+d1+"M"+d1+",0H-"+d1',
-            35: '"M0,"+d1+"V-"+d1+"M"+d1+",0H-"+d1+"M"+d2+","+d2+"L-"+d2+",-"+d2+"M"+d2+",-"+d2+"L-"+d2+","+d2',
-            36: '"M"+d1+","+d2+"V-"+d2+"m-"+d2+",0V"+d2+"M"+d2+","+d1+"H-"+d2+"m0,-"+d2+"H"+d2'}[symbol]
+        return {
+            'circle':
+            '"M"+b1+",0A"+b1+","+b1+" 0 1,1 0,-"+b1+"A"+b1+","+b1+" 0 0,1 "+b1+",0Z"',
+            'square':
+            '"M"+b1+","+b1+"H-"+b1+"V-"+b1+"H"+b1+"Z"',
+            'diamond':
+            '"M"+b1+",0L0,"+b1+"L-"+b1+",0L0,-"+b1+"Z"',
+            'hexagram':
+            '"M-"+b3+",0l-"+b2+",-"+b1+"h"+b3+"l"+b2+",-"+b1+"l"+b2+","+b1+"h"+b3+"l-"+b2+","+b1+"l"+'
+            'b2+","+b1+"h-"+b3+"l-"+b2+","+b1+"l-"+b2+",-"+b1+"h-"+b3+"Z"'
+        }[symbol]
+    return {
+        37: '"M-"+d1+","+d3+"L0,0M"+d1+","+d3+"L0,0M0,-"+d2+"L0,0"',
+        38: '"M-"+d1+",-"+d3+"L0,0M"+d1+",-"+d3+"L0,0M0,"+d2+"L0,0"',
+        39: '"M"+d3+","+d1+"L0,0M"+d3+",-"+d1+"L0,0M-"+d2+",0L0,0"',
+        40: '"M-"+d3+","+d1+"L0,0M-"+d3+",-"+d1+"L0,0M"+d2+",0L0,0"',
+        34: '"M"+d1+","+d1+"L-"+d1+",-"+d1+"M"+d1+",-"+d1+"L-"+d1+","+d1',
+        33: '"M0,"+d1+"V-"+d1+"M"+d1+",0H-"+d1',
+        35: '"M0,"+d1+"V-"+d1+"M"+d1+",0H-"+d1+"M"+d2+","+d2+"L-"+d2+",-"+d2+"M"+d2+",-"+d2+"L-"+d2+","+d2',
+        36: '"M"+d1+","+d2+"V-"+d2+"m-"+d2+",0V"+d2+"M"+d2+","+d1+"H-"+d2+"m0,-"+d2+"H"+d2'
+    }[symbol]
 
 
 def _draw_mash(base_symbol: str, ds_symbol: int) -> Tuple[str, str]:
     """Figure out how to draw one symbol on top of another, and propose an existing symbol to overwrite to make room.
 
     The names in this function were extracted from plotly/validators/scatter/marker/_symbol.py
 
@@ -592,25 +617,69 @@
         base_symbol: The symbol to go on the bottom.
         ds_symbol: The symbol to go on the top.
 
     Returns:
         (A regex pattern corresponding to an existing symbol to be replaced, a new javascript string to replace the old
          symbol)
     """
-    id_to_name = {0: 'circle', 1: 'square', 2: 'diamond', 3: 'cross', 4: 'x', 5: '"triangle-up"', 6: '"triangle-down"',
-                  7: '"triangle-left"', 8: '"triangle-right"', 9: '"triangle-ne"', 10: '"triangle-se"',
-                  11: '"triangle-sw"', 12: '"triangle-nw"', 13: 'pentagon', 14: 'hexagon', 15: 'hexagon2',
-                  16: 'octagon', 17: 'star', 18: 'hexagram', 19: '"star-triangle-up"', 20: '"star-triangle-down"',
-                  21: '"star-square"', 22: '"star-diamond"', 23: '"diamond-tall"', 24: '"diamond-wide"',
-                  25: 'hourglass', 26: 'bowtie', 27: '"circle-cross"', 28: '"circle-x"', 29: '"square-cross"',
-                  30: '"square-x"', 31: '"diamond-cross"', 32: '"diamond-x"', 33: '"cross-thin"', 34: '"x-thin"',
-                  35: 'asterisk', 36: 'hash', 37: '"y-up"', 38: '"y-down"', 39: '"y-left"', 40: '"y-right"',
-                  41: '"line-ew"', 42: '"line-ns"', 43: '"line-ne"', 44: '"line-nw"', 45: '"arrow-up"',
-                  46: '"arrow-down"', 47: '"arrow-left"', 48: '"arrow-right"', 49: '"arrow-bar-up"',
-                  50: '"arrow-bar-down"', 51: '"arrow-bar-left"', 52: '"arrow-bar-right"'}
+    id_to_name = {
+        0: 'circle',
+        1: 'square',
+        2: 'diamond',
+        3: 'cross',
+        4: 'x',
+        5: '"triangle-up"',
+        6: '"triangle-down"',
+        7: '"triangle-left"',
+        8: '"triangle-right"',
+        9: '"triangle-ne"',
+        10: '"triangle-se"',
+        11: '"triangle-sw"',
+        12: '"triangle-nw"',
+        13: 'pentagon',
+        14: 'hexagon',
+        15: 'hexagon2',
+        16: 'octagon',
+        17: 'star',
+        18: 'hexagram',
+        19: '"star-triangle-up"',
+        20: '"star-triangle-down"',
+        21: '"star-square"',
+        22: '"star-diamond"',
+        23: '"diamond-tall"',
+        24: '"diamond-wide"',
+        25: 'hourglass',
+        26: 'bowtie',
+        27: '"circle-cross"',
+        28: '"circle-x"',
+        29: '"square-cross"',
+        30: '"square-x"',
+        31: '"diamond-cross"',
+        32: '"diamond-x"',
+        33: '"cross-thin"',
+        34: '"x-thin"',
+        35: 'asterisk',
+        36: 'hash',
+        37: '"y-up"',
+        38: '"y-down"',
+        39: '"y-left"',
+        40: '"y-right"',
+        41: '"line-ew"',
+        42: '"line-ns"',
+        43: '"line-ne"',
+        44: '"line-nw"',
+        45: '"arrow-up"',
+        46: '"arrow-down"',
+        47: '"arrow-left"',
+        48: '"arrow-right"',
+        49: '"arrow-bar-up"',
+        50: '"arrow-bar-down"',
+        51: '"arrow-bar-left"',
+        52: '"arrow-bar-right"'
+    }
     mash_id = _symbol_mash(base_symbol, ds_symbol)
     mash_name = id_to_name[mash_id]
     target_str = mash_name + r':{n.*?}(,needLine:!0)?(,noDot:!0)?(,noFill:!0)?}'
     swap_str = mash_name + r':{n:' + str(mash_id) + ',f:function(t){' + _get_vars(base_symbol) + _get_vars(
         ds_symbol) + f'return{_get_paths(ds_symbol)}+{_get_paths(base_symbol)};' + '}}'
     return target_str, swap_str
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/summary.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/summary/system.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/summary/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from fastestimator.backend._save_model import save_model
 from fastestimator.network import BaseNetwork
 from fastestimator.pipeline import Pipeline
 from fastestimator.schedule.schedule import Scheduler
 from fastestimator.summary.summary import Summary
 from fastestimator.util.base_util import to_list
 from fastestimator.util.traceability_util import FeSummaryTable, is_restorable
+from fastestimator.util.util import get_num_gpus
 
 if TYPE_CHECKING:
     from fastestimator.trace.trace import Trace
 
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 
 
@@ -101,15 +102,15 @@
     mode: Optional[str]
     ds_id: str
     exp_id: int
     global_step: Optional[int]
     num_devices: int
     log_steps: Optional[int]
     total_epochs: int
-    epoch_idx: Optional[int]
+    epoch_idx: int
     batch_idx: Optional[int]
     stop_training: bool
     network: BaseNetwork
     pipeline: Pipeline
     traces: List[Union['Trace', Scheduler['Trace']]]
     train_steps_per_epoch: Optional[int]
     eval_steps_per_epoch: Optional[int]
@@ -121,15 +122,15 @@
 
     def __init__(self,
                  network: BaseNetwork,
                  pipeline: Pipeline,
                  traces: List[Union['Trace', Scheduler['Trace']]],
                  mode: Optional[str] = None,
                  ds_id: str = '',
-                 num_devices: int = torch.cuda.device_count(),
+                 num_devices: int = get_num_gpus(),
                  log_steps: Optional[int] = None,
                  total_epochs: int = 0,
                  train_steps_per_epoch: Optional[int] = None,
                  eval_steps_per_epoch: Optional[int] = None,
                  eval_log_steps: Sequence[int] = (),
                  system_config: Optional[List[FeSummaryTable]] = None) -> None:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/nightly_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/nightly_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/test/unittest_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/test/unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/early_stopping.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/lr_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import numpy as np
 import tensorflow as tf
 import torch
 
 from fastestimator.backend._get_lr import get_lr
 from fastestimator.backend._set_lr import set_lr
-from fastestimator.schedule.lr_shedule import ARC
+from fastestimator.schedule.lr_schedule import ARC
 from fastestimator.summary.system import System
 from fastestimator.trace.trace import Trace
 from fastestimator.util.data import Data
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/adapt/terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/adapt/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/batch_display.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/csv_logger.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/csv_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 class CSVLogger(Trace):
     """Log monitored quantities in a CSV file.
 
     Args:
         filename: Output filename.
         monitor_names: List of keys to monitor. If None then all metrics will be recorded. If you want to record 'all
             the usual stuff' plus a particular key which isn't normally recorded, you can use a '*' character here.
-            For example: monitor_names=['*', 'y_true']
+            For example: monitor_names=['*', 'y_true']. When recording intermediate variables in the pipeline or
+            network, you will need to add their names in the monitor_names argument when calling fe.Estimator.
         instance_id_key: A key corresponding to data instance ids. If provided, the CSV logger will record per-instance
             metric information into the csv file in addition to the standard metrics.
         mode: What mode(s) to execute this Trace in. For example, "train", "eval", "test", or "infer". To execute
             regardless of mode, pass None. To execute in all modes except for a particular one, you can pass an argument
             like "!infer" or "!train".
     """
     def __init__(self,
@@ -72,44 +73,57 @@
             if key not in self.df_agg.columns:
                 self.df_agg[key] = ''
         for col in set(self.df_agg.columns) - {'mode', 'step', 'epoch'} - tmpdic.keys():
             tmpdic[col] = ''
 
         # Only record an entry if there is at least one piece of actual information present
         if any(tmpdic.values()):
-            self.df_agg = pd.concat(objs=[self.df_agg, pd.DataFrame([{"mode": self.system.mode,
-                                                                      "step": self.system.global_step,
-                                                                      "epoch": self.system.epoch_idx,
-                                                                      **tmpdic}])],
-                                    ignore_index=True)
+            self.df_agg = pd.concat(
+                objs=[
+                    self.df_agg,
+                    pd.DataFrame([{
+                        "mode": self.system.mode,
+                        "step": self.system.global_step,
+                        "epoch": self.system.epoch_idx,
+                        **tmpdic
+                    }])
+                ],
+                ignore_index=True)
         self._save()  # Write on epoch end so that people can see results sooner if debugging
 
     def on_batch_end(self, data: Data) -> None:
         if self.instance_id_key:
             ins_data = data.read_per_instance_logs()
             keys = set(self.inputs) if "*" not in self.inputs else set(self.inputs) | ins_data.keys()
             keys = list(keys - {'*', self.instance_id_key})
             ids = data[self.instance_id_key]
             batch_size = len(ids)
             vals = [ins_data.get(key, data.get(key, _SKIP())) for key in keys]
             # Ignore vals which are not batched
-            vals = [val if (hasattr(val, 'ndim') and val.ndim > 0 and val.shape[0] == batch_size) or
-                           (isinstance(val, (list, tuple)) and len(val) == batch_size) else _SKIP() for val in vals]
+            vals = [
+                val if (hasattr(val, 'ndim') and val.ndim > 0 and val.shape[0] == batch_size) or
+                (isinstance(val, (list, tuple)) and len(val) == batch_size) else _SKIP() for val in vals
+            ]
             # Don't bother recording instance if no data is available
             if any((not isinstance(val, _SKIP) for val in vals)):
                 for key in keys:
                     if key not in self.df_ins.columns:
                         self.df_ins[key] = ''
                 rows = []
                 for sample in zip_longest(ids, *vals, fillvalue=''):
-                    row = {"instance_id": self._parse_val(sample[0]),
-                           "mode": self.system.mode,
-                           "step": self.system.global_step,
-                           "epoch": self.system.epoch_idx,
-                           **{key: self._parse_val(val) for key, val in zip(keys, sample[1:])}}
+                    row = {
+                        "instance_id": self._parse_val(sample[0]),
+                        "mode": self.system.mode,
+                        "step": self.system.global_step,
+                        "epoch": self.system.epoch_idx,
+                        **{
+                            key: self._parse_val(val)
+                            for key, val in zip(keys, sample[1:])
+                        }
+                    }
                     for col in self.df_ins.columns:
                         if col not in row.keys():
                             row[col] = ''
                     rows.append(row)
                 self.df_ins = pd.concat(objs=[self.df_ins, pd.DataFrame(rows)], ignore_index=True)
 
         if self.system.mode == "train" and self.system.log_steps and (self.system.global_step % self.system.log_steps
@@ -127,19 +141,25 @@
                     tmpdic[key] = self._parse_val(data.get(key, ''))
                 if key not in self.df_agg.columns:
                     self.df_agg[key] = ''
             for col in set(self.df_agg.columns) - {'mode', 'step', 'epoch'} - tmpdic.keys():
                 tmpdic[col] = ''
             # Only record an entry if there's at least 1 piece of actual information
             if any(tmpdic.values()):
-                self.df_agg = pd.concat(objs=[self.df_agg, pd.DataFrame([{"mode": self.system.mode,
-                                                                          "step": self.system.global_step,
-                                                                          "epoch": self.system.epoch_idx,
-                                                                          **tmpdic}])],
-                                        ignore_index=True)
+                self.df_agg = pd.concat(
+                    objs=[
+                        self.df_agg,
+                        pd.DataFrame([{
+                            "mode": self.system.mode,
+                            "step": self.system.global_step,
+                            "epoch": self.system.epoch_idx,
+                            **tmpdic
+                        }])
+                    ],
+                    ignore_index=True)
 
     def _save(self) -> None:
         """Write the current state to disk.
         """
         stack = [self.df_ins, self.df_agg]
         if self.system.mode == "test":
             if os.path.exists(self.filename):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/grid_display.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/grid_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/image_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/image_viewer.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/model_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/tensorboard.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from typing import Any, Dict, Iterable, List, Optional, Tuple, TypeVar, Union
 
 import cv2
 import numpy as np
 import tensorboard as tb
 import tensorflow as tf
 import torch
+from keras import backend
+from keras.callbacks import keras_model_summary
 from plotly.graph_objs import Figure
-from tensorflow.keras import backend
 from tensorflow.python.framework import ops as tfops
-from tensorflow.python.keras.callbacks import keras_model_summary
 from tensorflow.python.ops import summary_ops_v2
 from torch.utils.tensorboard import SummaryWriter
 
 from fastestimator.backend._abs import abs
 from fastestimator.backend._concat import concat
 from fastestimator.backend._expand_dims import expand_dims
 from fastestimator.backend._permute import permute
@@ -38,18 +38,15 @@
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.network import BaseNetwork, TFNetwork
 from fastestimator.trace.trace import Trace, parse_freq
 from fastestimator.util.base_util import DefaultKeyDict, is_number, to_list, to_set
 from fastestimator.util.data import Data
 from fastestimator.util.img_data import Display
 from fastestimator.util.traceability_util import traceable
-from fastestimator.util.util import to_number
-
-# https://github.com/pytorch/pytorch/issues/30966
-tf.io.gfile = tb.compat.tensorflow_stub.io.gfile
+from fastestimator.util.util import get_num_gpus, to_number
 
 Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
 
 
 class _BaseWriter:
     """A class to write various types of data into TensorBoard summary files.
@@ -120,18 +117,18 @@
             else:
                 self.summary_writers[mode].add_images(tag=key,
                                                       img_tensor=to_number(img),
                                                       global_step=step,
                                                       dataformats='NCHW' if isinstance(img, torch.Tensor) else 'NHWC')
 
     def write_embeddings(
-            self,
-            mode: str,
-            embeddings: Iterable[Tuple[str, Tensor, Optional[List[Any]], Optional[Tensor]]],
-            step: int,
+        self,
+        mode: str,
+        embeddings: Iterable[Tuple[str, Tensor, Optional[List[Any]], Optional[Tensor]]],
+        step: int,
     ):
         """Write embeddings (like UMAP) to TensorBoard.
 
         Args:
             mode: The current mode of execution ('train', 'eval', 'test', 'infer').
             embeddings: A collection of quadruplets like [("key", <features>, [<label1>, ...], <label_images>)].
                 Features are expected to be batched, and if labels and/or label images are provided they should have the
@@ -146,20 +143,26 @@
                     label_imgs = permute(label_imgs, [0, 3, 1, 2])
             self.summary_writers[mode].add_embedding(mat=flat,
                                                      metadata=labels,
                                                      label_img=label_imgs,
                                                      tag=key,
                                                      global_step=step)
 
+    def flush(self) -> None:
+        """Flush all of the associated writers.
+        """
+        for writer in self.summary_writers.values():
+            writer.flush()
+
     def close(self) -> None:
         """A method to flush and close all connections to the files on disk.
         """
         modes = list(self.summary_writers.keys())  # break connection with dictionary so can delete in iteration
         for mode in modes:
-            self.summary_writers[mode].close()
+            self.summary_writers[mode].close()  # Close also flushes
             del self.summary_writers[mode]
 
     @staticmethod
     def _weight_to_image(weight: Tensor, kernel_channels_last: bool = False) -> Optional[Tensor]:
         """Logs a weight as a TensorBoard image.
 
         Implementation from TensorFlow codebase, would have invoked theirs directly but they didn't make it a static
@@ -249,16 +252,15 @@
     """A class to write various Pytorch data into TensorBoard summary files.
 
     This class is intentionally not @traceable.
     """
     def write_epoch_models(self, mode: str, epoch: int) -> None:
         for model in self.network.epoch_models:
             inputs = model.fe_input_spec.get_dummy_input()
-            self.summary_writers[mode].add_graph(model.module if torch.cuda.device_count() > 1 else model,
-                                                 input_to_model=inputs)
+            self.summary_writers[mode].add_graph(model.module if get_num_gpus() > 1 else model, input_to_model=inputs)
 
     def write_weights(self, mode: str, models: Iterable[Model], step: int, visualize: bool) -> None:
         for model in models:
             for name, params in model.named_parameters():
                 name = name.replace(".", "/")
                 name = "{}_{}".format(model.model_name, name)
                 weight = params.data
@@ -312,15 +314,15 @@
                  weight_histogram_freq: Union[None, int, str] = None,
                  paint_weights: bool = False,
                  embedding_freq: Union[None, int, str] = 'epoch',
                  write_embeddings: Union[None, str, List[str]] = None,
                  embedding_labels: Union[None, str, List[str]] = None,
                  embedding_images: Union[None, str, List[str]] = None) -> None:
         super().__init__(inputs=["*"] + to_list(write_images) + to_list(write_embeddings) + to_list(embedding_labels) +
-                                to_list(embedding_images))
+                         to_list(embedding_images))
         self.root_log_dir = log_dir
         self.update_freq = parse_freq(update_freq)
         self.write_graph = write_graph
         self.painted_graphs = set()
         self.write_images = to_set(write_images)
         self.histogram_freq = parse_freq(weight_histogram_freq)
         if paint_weights and self.histogram_freq.freq == 0:
@@ -345,25 +347,24 @@
             assert len(embedding_images) == len(write_embeddings), \
                 f"Expected {len(write_embeddings)} embedding_images keys, but recieved {len(embedding_images)}. Use \
                 None to pad out the list if you have labels for only a subset of all embeddings."
 
         else:
             embedding_images = [None for _ in range(len(write_embeddings))]
         self.write_embeddings = [(feature, label, img_label) for feature,
-                                                                 label,
-                                                                 img_label in
-                                 zip(write_embeddings, embedding_labels, embedding_images)]
+                                 label,
+                                 img_label in zip(write_embeddings, embedding_labels, embedding_images)]
         self.collected_embeddings = defaultdict(list)
 
     def on_begin(self, data: Data) -> None:
         print("FastEstimator-Tensorboard: writing logs to {}".format(
             os.path.abspath(os.path.join(self.root_log_dir, self.system.experiment_time))))
         self.writer = _TfWriter(self.root_log_dir, self.system.experiment_time, self.system.network) if isinstance(
             self.system.network, TFNetwork) else _TorchWriter(
-            self.root_log_dir, self.system.experiment_time, self.system.network)
+                self.root_log_dir, self.system.experiment_time, self.system.network)
         if self.write_graph and self.system.global_step == 1:
             self.painted_graphs = set()
 
     def on_batch_end(self, data: Data) -> None:
         if self.write_graph and self.system.network.epoch_models.symmetric_difference(self.painted_graphs):
             self.writer.write_epoch_models(mode=self.system.mode, epoch=self.system.epoch_idx)
             self.painted_graphs = self.system.network.epoch_models
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/test_report.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/io/traceability.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/io/traceability.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 import platform
 import re
 import shutil
 import sys
 import types
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
-from unittest.mock import Base, MagicMock
+from unittest.mock import Base
 
 import dot2tex as d2t
 import jsonpickle
-import matplotlib
 import numpy as np
 import pydot
 import tensorflow as tf
 import torch
 from natsort import humansorted
 from pylatex import Command, Document, Figure, Hyperref, Itemize, Label, LongTable, Marker, MultiColumn, NoEscape, \
     Package, Section, Subsection, Subsubsection, Tabularx, escape_latex
 from pylatex.base_classes import Arguments
 from pylatex.section import Paragraph
 from pylatex.utils import bold
 from torch.utils.data import Dataset
 from torchinfo import summary as pms
+from torchview import draw_graph
 
 import fastestimator as fe
 from fastestimator.dataset.dataset import FEDataset
 from fastestimator.network import BaseNetwork
 from fastestimator.op.numpyop.meta.fuse import Fuse
 from fastestimator.op.numpyop.meta.one_of import OneOf
 from fastestimator.op.numpyop.meta.repeat import Repeat
@@ -56,19 +56,20 @@
 from fastestimator.op.tensorop.meta.sometimes import Sometimes as SometimesT
 from fastestimator.op.tensorop.model import ModelOp
 from fastestimator.pipeline import Pipeline
 from fastestimator.schedule.schedule import Scheduler, get_current_items, get_signature_epochs
 from fastestimator.summary.logs.log_plot import visualize_logs
 from fastestimator.trace.io.restore_wizard import RestoreWizard
 from fastestimator.trace.trace import Trace, sort_traces
-from fastestimator.util.base_util import FEID, DefaultKeyDict, LogSplicer, NonContext, Suppressor, \
-    prettify_metric_name, to_list
+from fastestimator.util.base_util import FEID, DefaultKeyDict, LogSplicer, NonContext, prettify_metric_name, to_list, \
+    warn
 from fastestimator.util.data import Data
 from fastestimator.util.latex_util import AdjustBox, Center, ContainerList, HrefFEID, Verbatim
 from fastestimator.util.traceability_util import FeSummaryTable, traceable
+from fastestimator.util.util import Suppressor, get_num_gpus
 
 
 @traceable()
 class Traceability(Trace):
     """Automatically generate summary reports of the training.
 
     Args:
@@ -421,67 +422,62 @@
                             # LaTeX \maxdim is around 575cm (226 inches), so the image must have max dimension less than
                             # 226 inches. However, the 'size' parameter doesn't account for the whole node height, so
                             # set the limit lower (100 inches) to leave some wiggle room.
                             dot.set('size', '100')
                             dot.write(file_path, format='pdf')
                         except Exception:
                             file_path = None
-                            print(
-                                f"FastEstimator-Warn: Model {model.model_name} could not be visualized by Traceability")
+                            warn(f"Model {model.model_name} could not be visualized by Traceability")
                     elif isinstance(model, torch.nn.Module):
                         if hasattr(model, 'fe_input_spec'):
                             # Text Summary
                             # noinspection PyUnresolvedReferences
                             inputs = model.fe_input_spec.get_dummy_input()
-                            self.doc.append(
-                                Verbatim(
-                                    str(
-                                        pms(model.module if self.system.num_devices > 1 else model,
-                                            input_data=inputs,
-                                            col_names=("output_size", "num_params", "trainable"),
-                                            col_width=20,
-                                            row_settings=["ascii_only"],
-                                            verbose=0))))
+                            with Suppressor():
+                                self.doc.append(
+                                    Verbatim(
+                                        str(
+                                            pms(model.module if self.system.num_devices > 1 else model,
+                                                input_data=inputs,
+                                                col_names=("output_size", "num_params", "trainable"),
+                                                col_width=20,
+                                                row_settings=["ascii_only"],
+                                                verbose=0))))
 
                             with self.doc.create(Center()):
                                 self.doc.append(HrefFEID(FEID(id(model)), model.model_name))
                             # Visual Summary
-                            # Import has to be done while matplotlib is using the Agg backend
-                            old_backend = matplotlib.get_backend() or 'Agg'
-                            matplotlib.use('Agg')
                             # noinspection PyBroadException
                             try:
-                                # Fake the IPython import when user isn't running from Jupyter
-                                sys.modules.setdefault('IPython', MagicMock())
-                                sys.modules.setdefault('IPython.display', MagicMock())
-                                import hiddenlayer as hl
                                 model.to(inputs.device)
-                                with Suppressor():
-                                    graph = hl.build_graph(model.module if self.system.num_devices > 1 else model,
-                                                           inputs)
-                                graph = graph.build_dot()
-                                graph.attr(rankdir='TB')  # Switch it to Top-to-Bottom instead of Left-to-Right
+                                graph = draw_graph(
+                                    model.module if isinstance(model, torch.nn.parallel.DataParallel) else model,
+                                    input_data=inputs,
+                                    device=inputs.device,
+                                    graph_dir='TB',
+                                    expand_nested=True,
+                                    depth=7).visual_graph
                                 # LaTeX \maxdim is around 575cm (226 inches), so the image must have max dimension less
                                 # than 226 inches. However, the 'size' parameter doesn't account for the whole node
                                 # height, so set the limit lower (100 inches) to leave some wiggle room.
                                 graph.attr(size="100,100")
                                 graph.attr(margin='0')
                                 file_path = graph.render(filename="{}_{}".format(self.report_name, model.model_name),
                                                          directory=self.resource_dir,
                                                          format='pdf',
                                                          cleanup=True)
                             except Exception:
                                 file_path = None
-                                print("FastEstimator-Warn: Model {} could not be visualized by Traceability".format(
-                                    model.model_name))
-                            finally:
-                                matplotlib.use(old_backend)
+                                warn("Model {} could not be visualized by Traceability".format(model.model_name))
                         else:
                             file_path = None
                             self.doc.append("This model was not used by the Network during training.")
+                    else:
+                        file_path = None
+                        self.doc.append(f"Model format: {type(model)} not recognized.")
                     if file_path:
                         with self.doc.create(Figure(position='ht!')) as fig:
                             fig.append(Label(Marker(name=str(FEID(id(model))), prefix="model")))
                             fig.add_image(os.path.relpath(file_path, start=self.save_dir),
                                           width=NoEscape(r'1.0\textwidth,height=0.95\textheight,keepaspectratio'))
                             fig.add_caption(NoEscape(HrefFEID(FEID(id(model)), model.model_name).dumps()))
 
@@ -489,15 +485,15 @@
         """Add a system config summary to the traceability document.
         """
         with self.doc.create(Section("System Configuration")):
             with self.doc.create(Itemize()) as itemize:
                 itemize.add_item(escape_latex(f"FastEstimator {fe.__version__}"))
                 itemize.add_item(escape_latex(f"Python {platform.python_version()}"))
                 itemize.add_item(escape_latex(f"OS: {sys.platform}"))
-                itemize.add_item(f"Number of GPUs: {torch.cuda.device_count()}")
+                itemize.add_item(f"Number of GPUs: {get_num_gpus()}")
                 if fe.fe_deterministic_seed is not None:
                     itemize.add_item(escape_latex(f"Deterministic Seed: {fe.fe_deterministic_seed}"))
             with self.doc.create(LongTable('|lr|', pos=['h!'], booktabs=True)) as tabular:
                 tabular.add_row((bold("Module"), bold("Version")))
                 tabular.add_hline()
                 tabular.end_table_header()
                 tabular.add_hline()
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/meta/_per_ds.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/meta/_per_ds.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,61 +8,59 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Union, List
-
 import functools
+from typing import List, Union
 
-from fastestimator.trace.trace import Trace, PerDSTrace
-from fastestimator.util.data import Data, DSData
+from fastestimator.trace.trace import PerDSTrace
 from fastestimator.util.base_util import to_list
+from fastestimator.util.data import Data, DSData
 
 
-def per_ds(clz: type(Trace)):
+def per_ds(clz):
     """A class annotation which will convert regular traces into dataset-sensitive traces.
 
     Args:
         clz: The base class to be converted.
 
     Returns:
         A dataset aware version of the class. Note that if the annotated class instance has a 'per_ds' member variable
         which is set to False, or has outputs containing the '|' character, then a normal (non-ds-aware) instance will
         be returned instead.
     """
+    @functools.wraps(clz, updated=())
     class PerDS(clz, PerDSTrace):
-        @functools.wraps(clz.__new__)
         def __new__(cls, *args, **kwargs):
             # We will dynamically determine whether to return a base object or a PerDS variant
             # If any of the outputs already use the | character then we cannot make this a PerDS variant
             base_obj = clz.__new__(clz)
             base_obj.__init__(*args, **kwargs)
             for output in base_obj.outputs:
                 if '|' in output:
                     return base_obj
             # If the user set per_ds to False in the constructor then we will not make this a PerDS variant
             if hasattr(base_obj, 'per_ds') and base_obj.per_ds is False:
                 return base_obj
             # Otherwise we are good to go with the PerDS variant
             return super().__new__(cls)
 
-        @functools.wraps(clz.__init__)
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.fe_per_ds_trace = clz.__new__(clz)
             self.fe_per_ds_trace.__init__(*args, **kwargs)
 
         def get_outputs(self, ds_ids: Union[None, str, List[str]]) -> List[str]:
-            ds_ids = to_list(ds_ids)
+            ids = to_list(ds_ids)
             outputs = list(self.outputs)
             for output in self.outputs:
-                for ds_id in ds_ids:
+                for ds_id in ids:
                     outputs.append(f"{output}|{ds_id}")
             return outputs
 
         def on_begin(self, data: Data) -> None:
             super().on_begin(data)
             self.fe_per_ds_trace.on_begin(data)
 
@@ -87,12 +85,8 @@
             if self.system.ds_id != '':
                 self.fe_per_ds_trace.on_epoch_end(DSData(self.system.ds_id, data))
 
         def on_end(self, data: Data) -> None:
             super().on_end(data)
             self.fe_per_ds_trace.on_end(data)
 
-    PerDS.__name__ = clz.__name__
-    PerDS.__qualname__ = clz.__qualname__
-    PerDS.__module__ = clz.__module__
-    PerDS.__doc__ = clz.__doc__  # We want to preserve the docstring of the original class
     return PerDS
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 # limitations under the License.
 # ==============================================================================
 from typing import TYPE_CHECKING
 
 import lazy_loader as lazy
 
 __getattr__, __dir__, __all__ = lazy.attach(__name__,
-                                            submod_attrs={'accuracy': ['Accuracy'],
+                                            submod_attrs={#'accuracy': ['Accuracy'],
                                                           'bleu_score': ['BleuScore'],
                                                           'calibration_error': ['CalibrationError'],
                                                           'confusion_matrix': ['ConfusionMatrix'],
                                                           'dice': ['Dice'],
                                                           'f1_score': ['F1Score'],
                                                           'mcc': ['MCC'],
                                                           'mean_average_precision': ['MeanAveragePrecision'],
                                                           'precision': ['Precision'],
                                                           'recall': ['Recall'], })
 
+from fastestimator.trace.metric.accuracy import Accuracy
+
 if TYPE_CHECKING:
     from fastestimator.trace.metric.accuracy import Accuracy
     from fastestimator.trace.metric.bleu_score import BleuScore
     from fastestimator.trace.metric.calibration_error import CalibrationError
     from fastestimator.trace.metric.confusion_matrix import ConfusionMatrix
     from fastestimator.trace.metric.dice import Dice
     from fastestimator.trace.metric.f1_score import F1Score
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/accuracy.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/auc.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/auc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/bleu_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/calibration_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/dice.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/f1_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/mcc.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/mean_average_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """COCO Mean average precisin (mAP) implementation."""
 from collections import defaultdict
-from typing import Dict, List, Union, Iterable
+from typing import Dict, Iterable, List, Optional, Union
 
 import numpy as np
 from pycocotools import mask as maskUtils
 
 from fastestimator.trace.meta._per_ds import per_ds
 from fastestimator.trace.trace import Trace
 from fastestimator.util.data import Data
@@ -61,16 +61,16 @@
                  ds_id: Union[None, str, Iterable[str]] = None,
                  output_name=("mAP", "AP50", "AP75"),
                  per_ds: bool = True) -> None:
         super().__init__(inputs=(true_key, pred_key), outputs=output_name, mode=mode, ds_id=ds_id)
 
         assert len(self.outputs) == 3, 'MeanAvgPrecision trace adds 3 fields mAP AP50 AP75 to state dict'
 
-        self.iou_thres = np.linspace(.5, 0.95, np.round((0.95 - .5) / .05).astype(np.int) + 1, endpoint=True)
-        self.recall_thres = np.linspace(.0, 1.00, np.round((1.00 - .0) / .01).astype(np.int) + 1, endpoint=True)
+        self.iou_thres = np.linspace(.5, 0.95, np.round((0.95 - .5) / .05).astype(np.int32) + 1, endpoint=True)
+        self.recall_thres = np.linspace(.0, 1.00, np.round((1.00 - .0) / .01).astype(np.int32) + 1, endpoint=True)
         self.categories = range(num_classes)
         self.max_detection = 100
         self.image_ids = []
         self.per_ds = per_ds
 
         # eval
         self.evalimgs = {}
@@ -339,16 +339,16 @@
             # for all images no gt inside this category
             if num_all_gt == 0:
                 continue
 
             tps = det_match > 0
             fps = det_match == 0
 
-            tp_sum = np.cumsum(tps, axis=1).astype(dtype=np.float)
-            fp_sum = np.cumsum(fps, axis=1).astype(dtype=np.float)
+            tp_sum = np.cumsum(tps, axis=1).astype(dtype=np.float32)
+            fp_sum = np.cumsum(fps, axis=1).astype(dtype=np.float32)
 
             for index, (true_positives, false_positives) in enumerate(zip(tp_sum, fp_sum)):
                 true_positives = np.array(true_positives)
                 false_positives = np.array(false_positives)
                 nd = len(true_positives)
                 recall = true_positives / num_all_gt
                 precision = true_positives / (false_positives + true_positives + np.spacing(1))
@@ -384,15 +384,15 @@
         self.eval = {
             'counts': [num_iou_thresh, num_recall_thresh, num_categories],
             'precision': precision_matrix,
             'recall': recall_matrix,
             'scores': scores_matrix,
         }
 
-    def summarize(self, iou: float = None) -> float:
+    def summarize(self, iou: Optional[float] = None) -> float:
         """Compute average precision given one intersection union threshold.
 
         Args:
             iou: Intersection over union threshold. If this value is `None`, then average all iou thresholds. The result
                 is the mean average precision.
 
         Returns:
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/precision.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/metric/recall.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/metric/recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/trace.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/eigen_cam.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/grad_cam.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/grad_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/label_tracker.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/trace/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/trace/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,32 +20,34 @@
                                             submod_attrs={'data': ['Data'],
                                                           'img_data': ['ImageDisplay', 'BatchDisplay', 'GridDisplay'],
                                                           'latex_util': ['AdjustBox', 'Center', 'ContainerList',
                                                                          'HrefFEID', 'PyContainer', 'Verbatim'],
                                                           'traceability_util': ['FeSplitSummary', 'trace_model',
                                                                                 'traceable'],
                                                           'base_util': ['to_set', 'to_list', 'param_to_range',
-                                                                        'NonContext', 'Suppressor', 'LogSplicer',
+                                                                        'NonContext', 'LogSplicer',
                                                                         'prettify_metric_name', 'strip_suffix',
                                                                         'strip_prefix', 'get_type', 'check_io_names',
                                                                         'parse_modes', 'check_ds_id', 'is_number',
                                                                         'DefaultKeyDict', 'FEID', 'Flag', 'in_notebook',
-                                                                        'get_shape', 'get_colors', 'list_files'],
-                                                          'util': ['Timer', 'cpu_count', 'draw', 'get_batch_size',
-                                                                   'get_num_devices', 'pad_batch', 'pad_data',
-                                                                   'to_number'],
+                                                                        'get_shape', 'get_colors', 'list_files',
+                                                                        'warn'],
+                                                          'util': ['Suppressor', 'Timer', 'cpu_count', 'draw', 'get_batch_size',
+                                                                   'get_device', 'get_num_devices', 'get_num_gpus',
+                                                                   'pad_batch', 'pad_data', 'to_number', 'move_tensors_to_device',
+                                                                   'detach_tensors'],
                                                           'cli_util': ['parse_string_to_python'],
                                                           'wget_util': ['bar_custom', 'callback_progress']
                                                           })
 
 if TYPE_CHECKING:
+    from fastestimator.util.base_util import FEID, DefaultKeyDict, Flag, LogSplicer, NonContext, check_ds_id, \
+        check_io_names, get_colors, get_shape, get_type, in_notebook, is_number, list_files, param_to_range, \
+        parse_modes, prettify_metric_name, strip_prefix, strip_suffix, to_list, to_set, warn
+    from fastestimator.util.cli_util import parse_string_to_python
     from fastestimator.util.data import Data
-    from fastestimator.util.img_data import ImageDisplay, BatchDisplay, GridDisplay
+    from fastestimator.util.img_data import BatchDisplay, GridDisplay, ImageDisplay
     from fastestimator.util.latex_util import AdjustBox, Center, ContainerList, HrefFEID, PyContainer, Verbatim
     from fastestimator.util.traceability_util import FeSplitSummary, trace_model, traceable
-    from fastestimator.util.base_util import to_set, to_list, param_to_range, NonContext, Suppressor, LogSplicer, \
-        prettify_metric_name, strip_suffix, strip_prefix, get_type, check_io_names, parse_modes, check_ds_id, \
-        is_number, DefaultKeyDict, FEID, Flag, in_notebook, get_shape, get_colors, list_files
-    from fastestimator.util.cli_util import parse_string_to_python
-    from fastestimator.util.util import Timer, cpu_count, draw, get_batch_size, get_num_devices, pad_batch, pad_data, \
-        to_number
+    from fastestimator.util.util import Suppressor, Timer, cpu_count, detach_tensors, draw, get_batch_size, \
+        get_device, get_num_devices, get_num_gpus, move_tensors_to_device, pad_batch, pad_data, to_number
     from fastestimator.util.wget_util import bar_custom, callback_progress
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/base_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/base_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,35 @@
 
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 import colorsys
 import os
 import re
 import string
 import sys
-from typing import Any, Set, KeysView, List, Union, Tuple, Optional, Type, TypeVar, Dict, Callable
+from typing import Any, Callable, Dict, Iterable, KeysView, List, Literal, Optional, Set, TextIO, Tuple, Type, \
+    TypeVar, Union, overload
+
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 from plotly.graph_objs import Figure
+
 # DO NOT IMPORT FE, TF, Torch, Numpy, Seaborn, OR Matplotlib IN THIS FILE
 
 KT = TypeVar('KT')  # Key type.
 VT = TypeVar('VT')  # Value type.
 
 
+def warn(message: str) -> None:
+    """Print a yellow warning message to catch the users' attention.
+
+    Args:
+        message: The warning to print.
+    """
+    print("\033[93m{}\033[00m".format("FastEstimator-Warn: " + message), flush=True)
+
+
 def to_set(data: Any) -> Set[Any]:
     """Convert data to a set. A single None value will be converted to the empty set.
 
     ```python
     x = fe.util.to_set(None)  # set()
     x = fe.util.to_set([None])  # {None}
     x = fe.util.to_set(7)  # {7}
@@ -52,14 +64,44 @@
         if isinstance(data, (tuple, list, KeysView)):
             data = set(data)
         else:
             data = {data}
     return data
 
 
+@overload
+def to_list(data: Union[None, VT, Iterable[VT]]) -> List[VT]:
+    ...
+
+
+@overload
+def to_list(data: Union[VT, Iterable[VT]]) -> List[VT]:
+    ...
+
+
+@overload
+def to_list(data: Union[None, Iterable[VT]]) -> List[VT]:
+    ...
+
+
+@overload
+def to_list(data: Union[None, VT]) -> List[VT]:
+    ...
+
+
+@overload
+def to_list(data: Iterable[VT]) -> List[VT]:
+    ...
+
+
+@overload
+def to_list(data: VT) -> List[VT]:
+    ...
+
+
 def to_list(data: Any) -> List[Any]:
     """Convert data to a list. A single None value will be converted to the empty list.
 
     ```python
     x = fe.util.to_list(None)  # []
     x = fe.util.to_list([None])  # [None]
     x = fe.util.to_list(7)  # [7]
@@ -121,85 +163,34 @@
     ```python
     a = 5
     with fe.util.NonContext():
         a = a + 37
     print(a)  # 42
     ```
     """
-
     def __enter__(self) -> None:
         pass
 
     def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
         pass
 
 
-class Suppressor(object):
-    """A class which can be used to silence output of function calls.
-
-    This class is intentionally not @traceable.
-
-    Args:
-        allow_pyprint: Whether to allow python printing to occur still within this scope (and therefore only silence
-            printing from non-python sources like c).
-
-    ```python
-    x = lambda: print("hello")
-    x()  # "hello"
-    with fe.util.Suppressor():
-        x()  #
-    x()  # "hello"
-    ```
-    """
-    def __init__(self, allow_pyprint: bool = False):
-        self.allow_pyprint = allow_pyprint
-
-    def __enter__(self) -> None:
-        # This is not necessary to block printing, but lets the system know what's happening
-        self.py_reals = [sys.stdout, sys.stderr]
-        sys.stdout = sys.stderr = self
-        # This part does the heavy lifting
-        self.fakes = [os.open(os.devnull, os.O_RDWR), os.open(os.devnull, os.O_RDWR)]
-        self.reals = [os.dup(1), os.dup(2)]  # [stdout, stderr]
-        os.dup2(self.fakes[0], 1)
-        os.dup2(self.fakes[1], 2)
-
-    def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
-        os.dup2(self.reals[0], 1)
-        os.dup2(self.reals[1], 2)
-        for fd in self.fakes + self.reals:
-            os.close(fd)
-        # Set the python pointers back too
-        sys.stdout, sys.stderr = self.py_reals[0], self.py_reals[1]
-
-    def write(self, dummy: str) -> None:
-        """A function which is invoked during print calls.
-
-        Args:
-            dummy: The string which wanted to be printed.
-        """
-        if self.allow_pyprint:
-            os.write(self.reals[0], dummy.encode('utf-8'))
-
-    def flush(self) -> None:
-        """A function to empty the current print buffer. No-op in this case.
-        """
-
-
 class LogSplicer:
     """A class to send stdout information into a file before passing it along to the normal stdout.
 
     Args:
         log_path: The path/filename into which to append the current stdout.
     """
+    stdout: TextIO
+    log_file: TextIO
 
     def __init__(self, log_path: str):
         self.log_path = log_path
-        self.stdout = None
-        self.log_file = None
+        self.stdout = None  # type: ignore
+        self.log_file = None  # type: ignore
 
     def __enter__(self) -> None:
         self.log_file = open(self.log_path, 'a')
         self.stdout = sys.stdout
         sys.stdout = self
 
     def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
@@ -230,14 +221,24 @@
 
     Returns:
         The formatted version of 'metric'.
     """
     return string.capwords(re.sub("([a-z])([A-Z])", r"\g<1> \g<2>", metric).replace("_", " "))
 
 
+@overload
+def strip_suffix(target: None, suffix: Optional[str]) -> None:
+    ...
+
+
+@overload
+def strip_suffix(target: str, suffix: Optional[str]) -> str:
+    ...
+
+
 def strip_suffix(target: Optional[str], suffix: Optional[str]) -> Optional[str]:
     """Remove the given `suffix` from the `target` if it is present there.
 
     ```python
     x = fe.util.strip_suffix("astring.json", ".json")  # "astring"
     x = fe.util.strip_suffix("astring.json", ".yson")  # "astring.json"
     ```
@@ -253,14 +254,24 @@
         return target
     s_len = len(suffix)
     if target[-s_len:] == suffix:
         return target[:-s_len]
     return target
 
 
+@overload
+def strip_prefix(target: None, prefix: Optional[str]) -> None:
+    ...
+
+
+@overload
+def strip_prefix(target: str, prefix: Optional[str]) -> str:
+    ...
+
+
 def strip_prefix(target: Optional[str], prefix: Optional[str]) -> Optional[str]:
     """Remove the given `prefix` from the `target` if it is present there.
 
     ```python
     x = fe.util.strip_prefix("astring.json", "ast")  # "ring.json"
     x = fe.util.strip_prefix("astring.json", "asa")  # "astring.json"
     ```
@@ -288,15 +299,15 @@
     x = fe.util.get_type(tf.ones((10, 10), dtype='float16'))  # "<dtype: 'float16'>"
     x = fe.util.get_type(torch.ones((10, 10)).type(torch.float))  # "torch.float32"
     x = fe.util.get_type([np.ones((10,10)) for i in range(4)])  # "List[float64]"
     x = fe.util.get_type(27)  # "int"
     ```
 
     For container to look into its element's type, its type needs to be either list or tuple, and the return string will
-    be List[...]. All container elements need to have the same data type becuase it will only check its first element.
+    be List[...]. All container elements need to have the same data type because it will only check its first element.
 
     ```python
     x = fe.util.get_type({"a":1, "b":2})  # "dict"
     x = fe.util.get_type([1, "a"]) # "List[int]"
     x = fe.util.get_type([[[1]]]) # "List[List[List[int]]]"
     ```
 
@@ -314,15 +325,15 @@
         else:
             result = strip_suffix(strip_prefix(str(type(obj)), "<class '"), "'>")
     else:
         result = strip_suffix(strip_prefix(str(type(obj)), "<class '"), "'>")
     return result
 
 
-def check_io_names(names: List[Optional[str]]) -> List[Optional[str]]:
+def check_io_names(names: List[str]) -> List[str]:
     forbidden_chars = {":", ";"}
     for name in names:
         assert not any(char in name for char in forbidden_chars), \
             "inputs/outputs name cannot contain characters like ':', ';', found {}".format(name)
         assert len(name) > 0, "inputs/outputs cannot be an empty string"
         assert len(name.split('|')) < 3, f"inputs/outputs cannot contain more than one '|' character, found {name}"
     return names
@@ -423,15 +434,14 @@
     print(d["c"])  # "cc"
     ```
 
     Args:
         default: A function which takes a key and returns a default value based on the key.
         **kwargs: Initial key/value pairs for the dictionary.
     """
-
     def __init__(self, default: Callable[[Any], Any], **kwargs) -> None:
         super().__init__(**kwargs)
         self.factory = default
 
     def __missing__(self, key: Any) -> Any:
         res = self[key] = self.factory(key)
         return res
@@ -508,15 +518,15 @@
 def in_notebook() -> bool:
     """Determine whether the code is running inside a jupyter notebook
 
     Returns:
         True iff the code is executing inside a Jupyter notebook
     """
     try:
-        from IPython import get_ipython
+        from IPython.core.getipython import get_ipython
         shell = get_ipython().__class__.__name__
         if shell == 'ZMQInteractiveShell':
             return True  # Jupyter notebook or qtconsole
         return False
     except (ImportError, NameError):
         return False
 
@@ -542,32 +552,30 @@
     Returns:
         A list representing the shape of the data.
     """
     if hasattr(obj, "shape"):
         result = list(obj.shape)
     elif isinstance(obj, (List, Tuple)):
         shapes = [get_shape(ob) for ob in obj]
-        result = [None]
+        result: List[Optional[int]] = [None]
         if shapes:
             rank = len(shapes[0])
             if any((len(shape) != rank for shape in shapes)):
                 return result
             result.extend(shapes[0])
             for shape in shapes[1:]:
                 for idx, dim in enumerate(shape):
                     if result[idx + 1] != dim:
                         result[idx + 1] = None
     else:
         result = []
     return result
 
 
-def list_files(root_dir: str,
-               file_extension: Optional[str] = None,
-               recursive_search: bool = True) -> List[str]:
+def list_files(root_dir: str, file_extension: Optional[str] = None, recursive_search: bool = True) -> List[str]:
     """Get the paths of all files in a particular root directory subject to a particular file extension.
 
     Args:
         root_dir: The path to the directory containing data.
         file_extension: If provided then only files ending with the file_extension will be included.
         recursive_search: Whether to search within subdirectories for files.
 
@@ -581,65 +589,88 @@
     paths = []
     root_dir = os.path.normpath(root_dir)
     if not os.path.isdir(root_dir):
         raise AssertionError("Provided path is not a directory")
     try:
         for root, _, files in os.walk(root_dir):
             for file_name in files:
-                if file_name.startswith(".") or (file_extension is not None
-                                                 and not file_name.endswith(file_extension)):
+                if file_name.startswith(".") or (file_extension is not None and not file_name.endswith(file_extension)):
                     continue
                 paths.append(os.path.join(root, file_name))
             if not recursive_search:
                 break
     except StopIteration:
         raise ValueError("Invalid directory structure for DirDataset at root: {}".format(root_dir))
     return paths
 
 
-def get_colors(n_colors: int,
-               alpha: float = 1.0,
-               as_numbers: bool = False) -> List[Union[str, Tuple[float, float, float, float]]]:
+@overload
+def get_colors(n_colors: int, as_numbers: Literal[False] = False, alpha: float = 1.0) -> List[str]:
+    ...
+
+
+@overload
+def get_colors(n_colors: int, as_numbers: Literal[True], alpha: float = 1.0) -> List[Tuple[float, float, float, float]]:
+    ...
+
+
+def get_colors(n_colors: int, as_numbers: bool = False,
+               alpha: float = 1.0) -> Union[List[str], List[Tuple[float, float, float, float]]]:
     """Get a list of colors to use in plotting.
 
     Args:
         n_colors: How many colors to return.
         alpha: What opacity value to use (0 to 1).
         as_numbers: Whether to return the values as a list of numbers [r,g,b,a] or as a string
 
     Returns:
         A list of rgba string colors.
     """
     if n_colors <= 10:
-        colors = [f'rgba(1,115,178,{alpha})', f'rgba(222,143,5,{alpha})', f'rgba(2,158,115,{alpha})',
-                  f'rgba(213,94,0,{alpha})', f'rgba(204,120,188,{alpha})', f'rgba(202,145,97,{alpha})',
-                  f'rgba(251,175,228,{alpha})', f'rgba(148,148,148,{alpha})', f'rgba(236,225,51,{alpha})',
-                  f'rgba(86,180,233,{alpha})']
+        colors = [
+            f'rgba(1,115,178,{alpha})',
+            f'rgba(222,143,5,{alpha})',
+            f'rgba(2,158,115,{alpha})',
+            f'rgba(213,94,0,{alpha})',
+            f'rgba(204,120,188,{alpha})',
+            f'rgba(202,145,97,{alpha})',
+            f'rgba(251,175,228,{alpha})',
+            f'rgba(148,148,148,{alpha})',
+            f'rgba(236,225,51,{alpha})',
+            f'rgba(86,180,233,{alpha})'
+        ]
     else:
         colors = [(i + 0.01) / n_colors for i in range(n_colors)]
         colors = [color - 1 if color >= 1 else color for color in colors]
         colors = [colorsys.hls_to_rgb(color, 0.6, 0.95) for color in colors]
         colors = [f'rgba({int(256*r)},{int(256*g)},{int(256*b)},{alpha})' for r, g, b in colors]
     colors = colors[:n_colors]
     if as_numbers:
-        colors = [[float(x) for x in elem.strip('rgba(').strip(')').split(',')] for elem in colors]
+        colors = [tuple(float(x) for x in elem.strip('rgba(').strip(')').split(',')) for elem in colors]
     return colors
 
 
 class FigureFE(Figure):
     @classmethod
     def from_figure(cls, fig: Figure) -> 'FigureFE':
         new_fig = FigureFE()
         new_fig.__dict__ = fig.__dict__.copy()
         return new_fig
 
-    def _get_color(self,
-                   clazz: str,
-                   label: Union[int, str],
-                   as_numbers: bool = False,
+    @overload
+    def _get_color(self, clazz: str, label: Union[int, str], as_numbers: Literal[False] = False,
+                   n_colors: int = 10) -> Tuple[str, bool]:
+        ...
+
+    @overload
+    def _get_color(self, clazz: str, label: Union[int, str], as_numbers: Literal[True],
+                   n_colors: int = 10) -> Tuple[Tuple[float, float, float, float], bool]:
+        ...
+
+    def _get_color(self, clazz: str, label: Union[int, str], as_numbers: bool = False,
                    n_colors: int = 10) -> Tuple[Union[str, Tuple[float, float, float, float]], bool]:
         """A function which determines what color a plot element ought to be.
 
         Args:
             clazz: The class of the thing to be plotted ('mask', 'keypoint' etc.).
             label: The name of the thing to be plotted ('lung', 'patella', etc.).
             as_numbers: Whether to return the color as a tuple of rgba floats or as a rgba string.
@@ -650,38 +681,37 @@
             has been assigned a color.
         """
         if clazz == 'mask':
             alpha = 0.3
         else:
             alpha = 1.0
         if not hasattr(self, '_fe_color_map'):
-            self._fe_color_map = {}  # ([remaining_colors], {label: assigned_color})
+            self._fe_color_map: Dict[str, Tuple[List[str],
+                                                Dict[Union[int, str],
+                                                     str]]] = {}  # ([remaining_colors], {label: assigned_color})
         if clazz not in self._fe_color_map:
             clazz_colors = get_colors(max(10, n_colors), alpha=alpha)
-            clazz_assignment = {}
+            clazz_assignment: Dict[Union[int, str], str] = {}
             self._fe_color_map[clazz] = (clazz_colors, clazz_assignment)
         clazz_colors, clazz_assignment = self._fe_color_map[clazz]
         if label in clazz_assignment:
             val = clazz_assignment[label]
             if as_numbers:
-                val = [float(x) for x in val.strip('rgba(').strip(')').split(',')]
+                val = tuple([float(x) for x in val.strip('rgba(').strip(')').split(',')])
             return val, False
         if not clazz_colors:
             # The initial estimate of color requirements was insufficient
             clazz_colors.extend(get_colors(max(20, n_colors), alpha=alpha))
         clazz_assignment[label] = clazz_colors.pop(0)
         val = clazz_assignment[label]
         if as_numbers:
-            val = [float(x) for x in val.strip('rgba(').strip(')').split(',')]
+            val = tuple([float(x) for x in val.strip('rgba(').strip(')').split(',')])
         return val, True
 
-    def show(self,
-             save_path: Optional[str] = None,
-             verbose: bool = True,
-             scale: int = 1,
+    def show(self, save_path: Optional[str] = None, verbose: bool = True, scale: int = 1,
              interactive: bool = True) -> None:
         """A function which will save or display plotly figures.
 
         Args:
             save_path: The path where the figure should be saved, or None to display the figure to the screen.
             verbose: Whether to print out the save location.
             scale: A scaling factor to apply when exporting to static images (to increase resolution).
@@ -693,18 +723,19 @@
             'displaylogo': False,
             'toImageButtonOptions': {
                 'format': 'png',  # one of png, svg, jpeg, webp
                 'height': None,
                 'width': None,
                 'filename': 'figure',
                 'scale': scale  # Multiply title/legend/axis/canvas sizes by this factor (high resolution save)
-            }}
+            }
+        }
         if save_path is None:
             if not interactive and in_notebook():
-                from IPython.display import Image, display
+                from IPython.core.display import Image, display
                 display(Image(self.to_image(format='png', scale=scale)))
             else:
                 super().show(config=config)
         else:
             save_path = os.path.normpath(save_path)
             root_dir = os.path.dirname(save_path)
             if root_dir == "":
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/cli_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/data.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/google_download_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/google_download_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/img_data.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/latex_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/latex_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/traceability_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/traceability_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from pylatex import Document, Label, Marker, MultiColumn, NoEscape, Package, Table, Tabularx, TextColor
 from pylatex.base_classes import LatexObject
 from pylatex.utils import bold, escape_latex, italic
 
 from fastestimator.backend._to_shape import to_shape
 from fastestimator.backend._to_type import to_type
 from fastestimator.summary.summary import ValWithError
-from fastestimator.util.base_util import strip_prefix, FEID, Flag
+from fastestimator.util.base_util import FEID, Flag, strip_prefix
 from fastestimator.util.latex_util import ContainerList, HrefFEID, PyContainer
 
 _Function = namedtuple('_Function', ['func', 'name'])
 _BoundFn = namedtuple('_BoundFn', ['func', 'args'])
 _PartialBind = namedtuple('_PartialBind', ['args', 'kwargs'])
 _Command = namedtuple('_Command', ['left', 'right', 'command'])
 _Condition = namedtuple('_Condition', ['left', 'right', 'condition'])
@@ -819,16 +819,16 @@
     refs = code.co_freevars
     lam = lambda_fn[2]
     response = {"function": escape_latex(lam)}
     if refs:
         closure_vars = inspect.getclosurevars(function)
         ref_map = {
             ref:
-                closure_vars.nonlocals.get(ref,
-                                           closure_vars.globals.get(ref, closure_vars.builtins.get(ref, _VarWrap(ref))))
+            closure_vars.nonlocals.get(ref,
+                                       closure_vars.globals.get(ref, closure_vars.builtins.get(ref, _VarWrap(ref))))
             for ref in refs
         }
         response['kwargs'] = _trace_value(ref_map, tables, ret_ref=ret_ref, wrap_str=False).raw_input
     return response
 
 
 def _parse_lambda(function: types.FunctionType, tables: Dict[FEID, FeSummaryTable],
@@ -1180,17 +1180,17 @@
         whitelist: Arguments which should be included in a deep restore of the decorated class.
         blacklist: Arguments which should be excluded from a deep restore of the decorated class.
 
     Returns:
         The decorated class.
     """
     if isinstance(whitelist, str):
-        whitelist = (whitelist,)
+        whitelist = (whitelist, )
     if isinstance(blacklist, str):
-        blacklist = (blacklist,)
+        blacklist = (blacklist, )
     if whitelist and blacklist:
         raise ValueError("Traceable objects may specify a whitelist or a blacklist, but not both")
 
     def make_traceable(cls):
         base_init = getattr(cls, '__init__')
         if hasattr(base_init, '__module__') and base_init.__module__ != 'fastestimator.util.traceability_util':
             # We haven't already overridden this class' init method
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utilities for FastEstimator."""
+import atexit
 import os
+import sys
+import tempfile
 import time
 from contextlib import ContextDecorator
 from typing import Any, Dict, List, MutableMapping, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 import tensorflow as tf
 import torch
+import torch.backends.mps
 from pyfiglet import Figlet
+from tensorflow.python.ops.logging_ops import print_v2
 
+from fastestimator.util.base_util import warn
 
 STRING_TO_TORCH_DTYPE = {
     None: None,
     'float32': torch.float32,
     'float': torch.float,
     'float64': torch.float64,
     'double': torch.double,
@@ -67,36 +73,138 @@
     torch.float64: np.float64,
     torch.float16: np.float16,
     torch.uint8: np.uint8,
     torch.int8: np.int8,
     torch.int16: np.int16,
     torch.int32: np.int32,
     torch.int64: np.int64,
-    torch.bool: np.bool,
+    torch.bool: bool,
     tf.float32: np.float32,
     tf.float64: np.float64,
     tf.float16: np.float16,
     tf.uint8: np.uint8,
     tf.int8: np.int8,
     tf.int16: np.int16,
     tf.int32: np.int32,
     tf.int64: np.int64,
-    tf.bool: np.bool,
+    tf.bool: bool,
     np.dtype('float32'): np.float32,
     np.dtype('float64'): np.float64,
     np.dtype('float16'): np.float16,
     np.dtype('uint8'): np.uint8,
     np.dtype('int8'): np.int8,
     np.dtype('int16'): np.int16,
     np.dtype('int32'): np.int32,
     np.dtype('int64'): np.int64,
-    np.dtype('bool'): np.bool,
+    np.dtype('bool'): bool,
 }
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
+T = TypeVar('T')
+
+
+class Suppressor(object):
+    """A class which can be used to silence output of function calls.
+
+    This class is intentionally not @traceable.
+
+    Args:
+        allow_pyprint: Whether to allow python printing to occur still within this scope (and therefore only silence
+            printing from non-python sources like c).
+        show_if_exception: Whether to retroactively show print messages if an exception is raised from within the
+            suppressor scope.
+
+    ```python
+    x = lambda: print("hello")
+    x()  # "hello"
+    with fe.util.Suppressor():
+        x()  #
+    x()  # "hello"
+    ```
+    """
+    # Only create one file to save on disk IO
+    stash_fd, stash_name = tempfile.mkstemp()
+    os.close(stash_fd)
+    tf_print_fd, tf_print_name = tempfile.mkstemp()
+    os.close(tf_print_fd)
+    tf_print_name_f = 'file://' + tf_print_name
+
+    def __init__(self, allow_pyprint: bool = False, show_if_exception: bool = False):
+        self.allow_pyprint = allow_pyprint
+        self.show_if_exception = show_if_exception
+
+    def __enter__(self) -> None:
+        # This is not necessary to block printing, but lets the system know what's happening
+        self.py_reals = [sys.stdout, sys.stderr]
+        sys.stdout = sys.stderr = self
+        # This part does the heavy lifting
+        if self.show_if_exception:
+            self.fake = os.open(self.stash_name, os.O_RDWR)
+        else:
+            self.fake = os.open(os.devnull, os.O_RDWR)
+        self.reals = [os.dup(1), os.dup(2)]  # [stdout, stderr]
+        os.dup2(self.fake, 1)
+        os.dup2(self.fake, 2)
+        if self.allow_pyprint:
+            tf.print = _custom_tf_print
+
+    def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
+        # If there was an error, display any print messages
+        if exc[0] is not None and self.show_if_exception and not isinstance(exc[1],
+                                                                            (StopIteration, StopAsyncIteration)):
+            for line in open(self.stash_name):
+                os.write(self.reals[0], line.encode('utf-8'))
+        # Set the print pointers back
+        os.dup2(self.reals[0], 1)
+        os.dup2(self.reals[1], 2)
+        # Set the python pointers back too
+        sys.stdout, sys.stderr = self.py_reals[0], self.py_reals[1]
+        # Clean up the descriptors
+        for fd in self.reals:
+            os.close(fd)
+        os.close(self.fake)
+        if self.show_if_exception:
+            # Clear the file
+            open(self.stash_name, 'w').close()
+        if self.allow_pyprint:
+            tf.print = print_v2
+            for line in open(self.tf_print_name, 'r'):
+                print(line, end='')  # Endings already included from tf.print
+            open(self.tf_print_name, 'w').close()
+
+    def write(self, dummy: str) -> None:
+        """A function which is invoked during print calls.
+
+        Args:
+            dummy: The string which wanted to be printed.
+        """
+        if self.allow_pyprint:
+            os.write(self.reals[0], dummy.encode('utf-8'))
+        elif self.show_if_exception:
+            os.write(self.fake, dummy.encode('utf-8'))
+
+    def flush(self) -> None:
+        """A function to empty the current print buffer. No-op in this case.
+        """
+
+    @staticmethod
+    @atexit.register
+    def teardown() -> None:
+        """Clean up the stash files when the program exists
+        """
+        try:
+            os.remove(Suppressor.stash_name)
+            os.remove(Suppressor.tf_print_name)
+        except FileNotFoundError:
+            pass
+
+
+def _custom_tf_print(*args, **kwargs):
+    kwargs['output_stream'] = Suppressor.tf_print_name_f
+    print_v2(*args, **kwargs)
 
 
 class Timer(ContextDecorator):
     """A class that can be used to time things.
 
     This class is intentionally not @traceable.
 
@@ -183,15 +291,90 @@
         The `data`, padded to the `target_shape`.
     """
     shape_difference = np.array(target_shape) - np.array(data.shape)
     padded_shape = np.array([np.zeros_like(shape_difference), shape_difference]).T
     return np.pad(data, padded_shape, 'constant', constant_values=pad_value)
 
 
-def get_num_devices():
+def move_tensors_to_device(data: T, device: Union[str, torch.device]) -> T:
+    """Move torch tensor (collections) between gpu and cpu recursively.
+
+    Args:
+        data: The input data to be moved.
+        device: The target device.
+
+    Returns:
+        Output data.
+    """
+    if isinstance(data, dict):
+        return {key: move_tensors_to_device(value, device) for (key, value) in data.items()}
+    elif isinstance(data, list):
+        return [move_tensors_to_device(val, device) for val in data]
+    elif isinstance(data, tuple):
+        return tuple([move_tensors_to_device(val, device) for val in data])
+    elif isinstance(data, set):
+        return set([move_tensors_to_device(val, device) for val in data])
+    elif isinstance(data, torch.Tensor):
+        return data.to(device)
+    else:
+        return data
+
+
+def detach_tensors(data: T) -> T:
+    """Detach tensor (collections) from current graph recursively.
+
+    Args:
+        data: The data to be detached.
+
+    Returns:
+        Output data.
+    """
+    if isinstance(data, dict):
+        return {key: detach_tensors(value) for (key, value) in data.items()}
+    elif isinstance(data, list):
+        return [detach_tensors(val) for val in data]
+    elif isinstance(data, tuple):
+        return tuple([detach_tensors(val) for val in data])
+    elif isinstance(data, set):
+        return set([detach_tensors(val) for val in data])
+    elif isinstance(data, torch.Tensor):
+        return data.detach()
+    return data
+
+
+def get_device() -> torch.device:
+    """Get the torch device for the current hardware.
+
+    Returns:
+        The torch device most appropriate for the current hardware.
+    """
+    if torch.backends.mps.is_available():
+        device = torch.device("mps")
+    elif torch.cuda.is_available():
+        device = torch.device("cuda:0")
+    else:
+        device = torch.device("cpu")
+    return device
+
+
+def get_num_gpus() -> int:
+    """Get the number of GPUs available.
+
+    Returns:
+        The number of GPUs available.
+    """
+    if torch.backends.mps.is_available():
+        return 1
+    elif torch.cuda.is_available():
+        return torch.cuda.device_count()
+    else:
+        return 0
+
+
+def get_num_devices() -> int:
     """Determine the number of available GPUs.
 
     Returns:
         The number of available GPUs, or 1 if none are found.
     """
     return max(torch.cuda.device_count(), 1)
 
@@ -223,15 +406,15 @@
         return existing_limit
     # Check if user provided an environment variable limit on the number of threads
     env_limit = os.environ.get('FE_NUM_THREADS', None)  # User might set this one in a bash script
     if env_limit:
         try:
             env_limit = int(env_limit)
         except ValueError as err:
-            print(f"FastEstimator-Warn: FE_NUM_THREADS variable must be an integer, but was set to: {env_limit}")
+            warn(f"FE_NUM_THREADS variable must be an integer, but was set to: {env_limit}")
             raise err
     try:
         # In docker containers which have --cpuset-cpus, the limit won't be reflected by normal os.cpu_count() call
         cores = len(os.sched_getaffinity(0))
     except AttributeError:
         # Running on Mac or Windows where the above method isn't available, so use the regular way
         cores = os.cpu_count()
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/util/wget_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/util/wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.5.0.dev202304171323
+Version: 1.6.0.dev202305310417
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
-Author-email: UNKNOWN
 License: Apache License 2.0
-Description: FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
+License-File: LICENSE
+
+FastEstimator is a high-level deep learning API. With the help of FastEstimator, you can easily                     build a high-performance deep learning model and run it anywhere.
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/SOURCES.txt` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 ./fastestimator/__init__.py
 ./fastestimator/estimator.py
 ./fastestimator/network.py
 ./fastestimator/pipeline.py
 ./fastestimator/architecture/__init__.py
@@ -87,14 +88,15 @@
 ./fastestimator/cli/logs.py
 ./fastestimator/cli/main.py
 ./fastestimator/cli/plot.py
 ./fastestimator/cli/run.py
 ./fastestimator/cli/train.py
 ./fastestimator/dataset/__init__.py
 ./fastestimator/dataset/batch_dataset.py
+./fastestimator/dataset/combined_dataset.py
 ./fastestimator/dataset/csv_dataset.py
 ./fastestimator/dataset/dataloader.py
 ./fastestimator/dataset/dataset.py
 ./fastestimator/dataset/dir_dataset.py
 ./fastestimator/dataset/extend_dataset.py
 ./fastestimator/dataset/generator_dataset.py
 ./fastestimator/dataset/labeled_dir_dataset.py
@@ -109,14 +111,15 @@
 ./fastestimator/dataset/data/cifar10.py
 ./fastestimator/dataset/data/cifar100.py
 ./fastestimator/dataset/data/cub200.py
 ./fastestimator/dataset/data/em_3d.py
 ./fastestimator/dataset/data/food101.py
 ./fastestimator/dataset/data/horse2zebra.py
 ./fastestimator/dataset/data/imdb_review.py
+./fastestimator/dataset/data/medmnist.py
 ./fastestimator/dataset/data/mendeley.py
 ./fastestimator/dataset/data/mitmovie_ner.py
 ./fastestimator/dataset/data/mnist.py
 ./fastestimator/dataset/data/montgomery.py
 ./fastestimator/dataset/data/mscoco.py
 ./fastestimator/dataset/data/nih_chestxray.py
 ./fastestimator/dataset/data/omniglot.py
@@ -267,15 +270,15 @@
 ./fastestimator/op/tensorop/meta/one_of.py
 ./fastestimator/op/tensorop/meta/repeat.py
 ./fastestimator/op/tensorop/meta/sometimes.py
 ./fastestimator/op/tensorop/model/__init__.py
 ./fastestimator/op/tensorop/model/model.py
 ./fastestimator/op/tensorop/model/update.py
 ./fastestimator/schedule/__init__.py
-./fastestimator/schedule/lr_shedule.py
+./fastestimator/schedule/lr_schedule.py
 ./fastestimator/schedule/schedule.py
 ./fastestimator/search/__init__.py
 ./fastestimator/search/golden_section.py
 ./fastestimator/search/grid_search.py
 ./fastestimator/search/search.py
 ./fastestimator/search/visualize/__init__.py
 ./fastestimator/search/visualize/cartesian.py
@@ -519,14 +522,15 @@
 ./test/PR_test/unit_test/backend/test_where.py
 ./test/PR_test/unit_test/backend/test_zeros_like.py
 ./test/PR_test/unit_test/backend/test_zscore.py
 ./test/PR_test/unit_test/cli/__init__.py
 ./test/PR_test/unit_test/cli/test_cli_util.py
 ./test/PR_test/unit_test/dataset/__init__.py
 ./test/PR_test/unit_test/dataset/test_batch_dataset.py
+./test/PR_test/unit_test/dataset/test_combine_dataset.py
 ./test/PR_test/unit_test/dataset/test_csv_dataset.py
 ./test/PR_test/unit_test/dataset/test_data.py
 ./test/PR_test/unit_test/dataset/test_dir_dataset.py
 ./test/PR_test/unit_test/dataset/test_extend_dataset.py
 ./test/PR_test/unit_test/dataset/test_generator_dataset.py
 ./test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
 ./test/PR_test/unit_test/dataset/test_numpy_dataset.py
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/fastestimator_nightly.egg-info/requires.txt` & `fastestimator-nightly-1.6.0.dev202305310417/fastestimator_nightly.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-albumentations[imgaug]==1.1.0
-matplotlib==3.4.3
-h5py==3.6.0
-scipy==1.8.0
+albumentations[imgaug]==1.3.0
+matplotlib==3.7.1
+h5py==3.8.0
+scipy==1.9.1
 PyLaTeX==1.4.1
-natsort==8.1.0
-tensorflow_probability==0.16.0
-tensorflow-addons==0.17.0
-transformers==4.16.2
-torchinfo==1.7.0
-graphviz==0.19.1
-hiddenlayer==0.3
+natsort==8.3.1
+tensorflow_probability==0.19.0
+tensorflow-addons==0.19.0
+transformers==4.26.1
+torchinfo==1.7.2
+graphviz==0.20.1
+torchview==0.2.6
 pydot==1.4.2
 dot2tex==2.11.3
-gdown==3.12.0
+gdown==4.6.4
 PySocks==1.7.1
 uncertainty-calibration==0.1.4
-dill==0.3.4
-scikit-image==0.19.1
-prettytable==3.1.0
-nltk==3.7
-requests>=2.22.0
-tqdm>=4.62.3
-numpy>=1.22.1
-pyfiglet>=0.8.post1
-opencv-python>=4.5.5.62
-pandas>=1.4.1
-wget>=3.2
-pillow>=9.0.1
-jsonpickle>=2.1.0
-python-docx>=0.8.11
-plotly==5.7.0
-kaleido>=0.2.1
-orjson>=3.6.7
-scikit-learn
-lazy_loader
-fe_pycocotools
+dill==0.3.6
+scikit-image==0.20.0
+prettytable==3.6.0
+nltk==3.8.1
+requests==2.28.2
+tqdm==4.65.0
+numpy==1.24.2
+pyfiglet==0.8.post1
+opencv-python==4.7.0.72
+pandas==2.0.1
+wget==3.2
+pillow==9.4.0
+jsonpickle==3.0.1
+python-docx==0.8.11
+plotly==5.13.1
+kaleido==0.2.1
+orjson==3.8.7
+scikit-learn==1.2.2
+lazy_loader==0.1
+fe_pycocotools==1.0
+typing_extensions==4.5.0
+charset-normalizer==3.1.0
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_get_lr.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_save_model_load_model.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_save_model_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_set_lr.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/backend/test_update_model.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/backend/test_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/test_main.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/cli/test_train.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/cli/test_train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,36 +175,33 @@
         # Get Data
         train_data, eval_data = mnist.load_data()
         t_d = train_data.split(128)
         # Initializing Pytorch model
         pytorch_l2 = fe.build(model_fn=MyNet_torch, optimizer_fn=lambda x: torch.optim.SGD(params=x, lr=0.01))
         # Initialize Pytorch pipeline
         pipeline = fe.Pipeline(train_data=t_d,
-                        eval_data=eval_data,
-                        batch_size=128,
-                        ops=[ExpandDims(inputs="x", outputs="x", axis=0),
-                                Minmax(inputs="x", outputs="x")])
+                               eval_data=eval_data,
+                               batch_size=128,
+                               ops=[ExpandDims(inputs="x", outputs="x", axis=0), Minmax(inputs="x", outputs="x")])
         # Initialize Pytorch Network
         network_l2 = fe.Network(ops=[
             ModelOp(model=pytorch_l2, inputs="x", outputs="y_pred"),
             CrossEntropy(inputs=("y_pred", "y"), outputs="ce"),
-            L2Regularizaton(inputs="ce",outputs="l2",model=pytorch_l2,beta = self.beta),
+            L2Regularizaton(inputs="ce", outputs="l2", model=pytorch_l2, beta=self.beta),
             UpdateOp(model=pytorch_l2, loss_name="l2")
         ])
         # step 3
-        traces = [
-            Accuracy(true_key="y", pred_key="y_pred")
-        ]
+        traces = [Accuracy(true_key="y", pred_key="y_pred")]
         # Initialize Pytorch estimator
         estimator_l2 = fe.Estimator(pipeline=pipeline,
-                            network=network_l2,
-                            epochs=1,
-                            traces=traces,
-                            train_steps_per_epoch=1,
-                            monitor_names=["ce","l2"])
+                                    network=network_l2,
+                                    epochs=1,
+                                    traces=traces,
+                                    train_steps_per_epoch=1,
+                                    monitor_names=["ce", "l2"])
         print('********************************Pytorch L2 Regularization training************************************')
         estimator_l2.fit()
 
         # Converting Pytorch weights to numpy
         torch_wt = []
         for _, param in pytorch_l2.named_parameters():
             if param.requires_grad:
@@ -216,36 +213,33 @@
                                batch_size=128,
                                ops=[ExpandDims(inputs="x", outputs="x"), Minmax(inputs="x", outputs="x")])
         # step 2
         model_tf = fe.build(model_fn=MyNet_tf, optimizer_fn=lambda: tf.optimizers.SGD(learning_rate=0.01))
         network = fe.Network(ops=[
             ModelOp(model=model_tf, inputs="x", outputs="y_pred"),
             CrossEntropy(inputs=("y_pred", "y"), outputs="ce"),
-            L2Regularizaton(inputs="ce",outputs="l2",model=model_tf,beta = self.beta),
+            L2Regularizaton(inputs="ce", outputs="l2", model=model_tf, beta=self.beta),
             UpdateOp(model=model_tf, loss_name="l2")
         ])
         # step 3
-        traces = [
-            Accuracy(true_key="y", pred_key="y_pred")
-        ]
+        traces = [Accuracy(true_key="y", pred_key="y_pred")]
         estimator = fe.Estimator(pipeline=pipeline,
-                                network=network,
-                                epochs=1,
-                                traces=traces,
-                                train_steps_per_epoch=1,
-                                monitor_names=["ce","l2"])
+                                 network=network,
+                                 epochs=1,
+                                 traces=traces,
+                                 train_steps_per_epoch=1,
+                                 monitor_names=["ce", "l2"])
         print('*******************************Tensorflow L2 Regularization training***********************************')
         estimator.fit()
 
-
         # Converting TF weights to numpy
         tf_wt = []
         for layer in model_tf.layers:
             for w in layer.trainable_variables:
                 tf_wt.append(w.numpy())
 
         # testing weights
         count = 0
-        for tf_t,tr in zip(tf_wt,torch_wt):
-            if np.sum(np.abs(tf_t-np.transpose(tr))) < (10**-5):
+        for tf_t, tr in zip(tf_wt, torch_wt):
+            if np.sum(np.abs(tf_t - np.transpose(tr))) < (10**-5):
                 count += 1
         self.assertTrue(count == 6)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 import tensorflow as tf
 import torch
 
 import fastestimator as fe
 from fastestimator.op.tensorop.loss import CrossEntropy, Hinge, SuperLoss
 from fastestimator.op.tensorop.model import ModelOp
 from fastestimator.test.unittest_util import sample_system_object
+from fastestimator.util.util import get_device
 
 
 class TestSuperLoss(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
+        device = get_device()
         # torch binary ce
-        cls.torch_true_binary = torch.tensor([[1], [0], [1], [0]]).to("cuda:0" if torch.cuda.is_available() else "cpu")
-        cls.torch_pred_binary = torch.tensor([[0.9], [0.3], [0.8],
-                                              [0.1]]).to("cuda:0" if torch.cuda.is_available() else "cpu")
+        cls.torch_true_binary = torch.tensor([[1], [0], [1], [0]]).to(device)
+        cls.torch_pred_binary = torch.tensor([[0.9], [0.3], [0.8], [0.1]]).to(device)
         # categorical ce
         cls.tf_true_cat = tf.constant([[0, 1, 0], [1, 0, 0], [0, 0, 1]])
         cls.tf_pred_cat = tf.constant([[0.1, 0.8, 0.1], [0.9, 0.05, 0.05], [0.1, 0.2, 0.7]])
-        cls.torch_true_cat = torch.tensor([[0, 1, 0], [1, 0, 0],
-                                           [0, 0, 1]]).to("cuda:0" if torch.cuda.is_available() else "cpu")
-        cls.torch_pred_cat = torch.tensor([[0.1, 0.8, 0.1], [0.9, 0.05, 0.05],
-                                           [0.1, 0.2, 0.7]]).to("cuda:0" if torch.cuda.is_available() else "cpu")
+        cls.torch_true_cat = torch.tensor([[0, 1, 0], [1, 0, 0], [0, 0, 1]]).to(device)
+        cls.torch_pred_cat = torch.tensor([[0.1, 0.8, 0.1], [0.9, 0.05, 0.05], [0.1, 0.2, 0.7]]).to(device)
         # sparse categorical ce
         cls.tf_true_sparse = tf.constant([[0], [1], [0]])
         cls.tf_pred_sparse = tf.constant([[0.1, 0.8, 0.1], [0.9, 0.05, 0.05], [0.1, 0.2, 0.7]])
         cls.state = {'warmup': False, 'epoch': 1, 'mode': 'train'}
 
     @staticmethod
     @tf.function
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/test_modelop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/test_modelop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/model/test_updateop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/model/test_updateop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_average.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_arc.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_arc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/schedule/test_schedule.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/schedule/test_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/search/visualize/test_visualize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/search/visualize/test_visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/summary/test_system.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/summary/test_system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_estimator.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_network.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         str_list = ['adadelta', 'adagrad', 'adam', 'adamax', 'rmsprop', 'sgd']
         for opt_name in str_list:
             with self.subTest(optimizer_fn=opt_name):
                 optimizer = fe.network._build_optimizer(optimizer_fn=opt_name,
                                                         model=self.tf_model,
                                                         framework="tf",
                                                         mixed_precision=False)
-                self.assertIsInstance(optimizer, tf.optimizers.Optimizer)
+                self.assertIsInstance(optimizer, tf.optimizers.legacy.Optimizer)
 
     def test_network_build_optimizer_torch_model_optimizer_str(self):
         str_list = ['adadelta', 'adagrad', 'adam', 'adamax', 'rmsprop', 'sgd']
         for opt_name in str_list:
             with self.subTest(optimizer_fn=opt_name):
                 optimizer = fe.network._build_optimizer(optimizer_fn=opt_name,
                                                         model=self.torch_model,
@@ -257,18 +257,18 @@
                                        optimizer_fn=optimizer,
                                        weight=None,
                                        name="test",
                                        mixed_precision=False)
 
         with self.subTest("check optimizer instantiation"):
             for optimizer in model.optimizer.get_all_values():
-                self.assertIsInstance(optimizer, tf.optimizers.Optimizer)
+                self.assertIsInstance(optimizer, tf.optimizers.legacy.Optimizer)
 
         with self.subTest("check current_optimizer"):
-            self.assertIsInstance(model.current_optimizer, tf.optimizers.Adam)
+            self.assertIsInstance(model.current_optimizer, tf.optimizers.legacy.Adam)
 
         with self.subTest("check model_name"):
             self.assertEqual(model.model_name, "test")
 
         with self.subTest("check fe_compiled"):
             self.assertEqual(model.fe_compiled, True)
 
@@ -278,28 +278,28 @@
                                        optimizer_fn=optimizer,
                                        weight=None,
                                        name=None,
                                        mixed_precision=False)
 
         with self.subTest("check optimizer instantiation"):
             for optimizer in model.optimizer.get_all_values():
-                self.assertIsInstance(optimizer, tf.optimizers.Optimizer)
+                self.assertIsInstance(optimizer, tf.optimizers.legacy.Optimizer)
 
         with self.subTest("check current optimizer"):
-            self.assertIsInstance(model.current_optimizer, tf.optimizers.Adam)
+            self.assertIsInstance(model.current_optimizer, tf.optimizers.legacy.Adam)
 
     def test_network_fe_compile_optimizer_no_scheduler_tf_check_optimizer(self):
         optimizer = "adam"
         model = fe.network._fe_compile(model=self.tf_model,
                                        optimizer_fn=optimizer,
                                        weight=None,
                                        name=None,
                                        mixed_precision=False)
         with self.subTest("check optimizer instantiation"):
-            self.assertIsInstance(model.optimizer, tf.optimizers.Optimizer)
+            self.assertIsInstance(model.optimizer, tf.optimizers.legacy.Optimizer)
 
         with self.subTest("check current optimizer"):
             self.assertEqual(model.current_optimizer, model.optimizer)
 
     def test_network_fe_compile_optimizer_epochscheduler_torch_check_optimizer(self):
         optimizer = EpochScheduler(epoch_dict={1: "adam", 10: "sgd"})
         model = fe.network._fe_compile(model=self.torch_model,
@@ -383,17 +383,21 @@
 
     def test_network_build_tf_model_torch_optimizer_check_assertion_error(self):
         with self.assertRaises(AssertionError):
             model = fe.build(model_fn=one_layer_tf_model, optimizer_fn=lambda x: torch.optim.SGD(params=x, lr=0.01))
 
     def test_network_build_torch_model_tf_optimizer_check_assertion_error(self):
         with self.subTest("optimizer_fn directly uses tf optimizer "):
-            with self.assertRaises(AssertionError):
+            with self.assertRaises(ValueError):
                 model = fe.build(model_fn=OneLayerTorchModel, optimizer_fn=tf.optimizers.Adadelta)
 
+        with self.subTest("optimizer_fn directly uses legacy tf optimizer "):
+            with self.assertRaises(AssertionError):
+                model = fe.build(model_fn=OneLayerTorchModel, optimizer_fn=tf.optimizers.legacy.Adadelta)
+
         with self.subTest("optimizer_fn use lambda function"):
             with self.assertRaises(ValueError):
                 model = fe.build(model_fn=OneLayerTorchModel, optimizer_fn=lambda: tf.optimizers.Adadelta())
 
     def test_network_build_unknown_model_check_assertion_error(self):
         with self.assertRaises(ValueError):
             model = fe.build(model_fn=lambda: "string", optimizer_fn=tf.optimizers.Adadelta)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/test_pipeline.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_early_stopping.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_batch_display.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_csv_logger.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_image_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_image_viewer.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_model_saver.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_saliency.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,26 +17,24 @@
 import unittest
 
 import fastestimator as fe
 from fastestimator.architecture.tensorflow import LeNet
 from fastestimator.dataset.data import cifair10
 from fastestimator.op.numpyop.univariate import Normalize
 from fastestimator.op.tensorop.model import ModelOp
-from fastestimator.test.unittest_util import img_to_rgb_array, check_img_similar
+from fastestimator.test.unittest_util import check_img_similar, img_to_rgb_array
 from fastestimator.trace.io import ImageSaver
 from fastestimator.trace.xai import Saliency
 
 
 class TestSaliency(unittest.TestCase):
     """ This test has dependency on:
     * fe.trace.ImageSaver
-    * fe.estimator.enable_deterministic
     """
     def test_saliency(self):
-        fe.enable_deterministic(200)
         label_mapping = {
             'airplane': 0,
             'automobile': 1,
             'bird': 2,
             'cat': 3,
             'deer': 4,
             'dog': 5,
@@ -44,33 +42,33 @@
             'horse': 7,
             'ship': 8,
             'truck': 9
         }
 
         batch_size = 32
 
-        train_data, eval_data = cifair10.load_data()
-        pipeline = fe.Pipeline(test_data=train_data,
-                               batch_size=batch_size,
-                               ops=[Normalize(inputs="x", outputs="x")],
-                               num_process=0)
+        train_data, _ = cifair10.load_data()
+        test_data = train_data.split([i for i in range(10)])
+        pipeline = fe.Pipeline(test_data=test_data, batch_size=batch_size, ops=[Normalize(inputs="x", outputs="x")])
 
         weight_path = os.path.abspath(os.path.join(__file__, "..", "resources", "lenet_cifar10_tf.h5"))
 
         model = fe.build(model_fn=lambda: LeNet(input_shape=(32, 32, 3)), optimizer_fn="adam", weights_path=weight_path)
         network = fe.Network(ops=[ModelOp(model=model, inputs="x", outputs="y_pred")])
 
         save_dir = tempfile.mkdtemp()
         traces = [
             Saliency(model=model,
                      model_inputs="x",
                      class_key="y",
                      model_outputs="y_pred",
                      samples=5,
-                     label_mapping=label_mapping),
+                     label_mapping=label_mapping,
+                     smoothing=0,
+                     integrating=0),
             ImageSaver(inputs="saliency", save_dir=save_dir)
         ]
 
         estimator = fe.Estimator(pipeline=pipeline, network=network, epochs=5, traces=traces, log_steps=1000)
         estimator.test()
 
         ans_img_path = os.path.abspath(os.path.join(__file__, "..", "resources", "saliency_figure.png"))
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_tensorboard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         with self.subTest('Check if tensors.tsv was generated'):
             self.assertTrue(os.path.exists(tsv_path))
         with self.subTest('Check if embed image was generated'):
             self.assertTrue(os.path.exists(embed_img_path))
         with self.subTest('Check content of tensors.tsv'):
             self.assertEqual(tsv_data, 27 * ['1.0'])
         with self.subTest('Check embed image content'):
-            self.assertTrue(is_equal(output_img, 255 * np.ones(shape=(3, 3, 3), dtype=np.int)))
+            self.assertTrue(is_equal(output_img, 255 * np.ones(shape=(3, 3, 3), dtype=np.int32)))
 
     def test_torch_on_begin(self):
         tensorboard = TensorBoard(log_dir=self.log_dir)
         tensorboard.system = sample_system_object_torch()
         tensorboard.system.global_step = 1
         with patch('sys.stdout', new=StringIO()) as fake_stdout:
             tensorboard.on_begin(data=self.torch_data)
@@ -137,14 +137,15 @@
         tensorboard.writer = _TorchWriter(self.log_dir, '', tensorboard.system.network)
         model = fe.build(model_fn=fe.architecture.pytorch.LeNet, optimizer_fn='adam', model_name='torch')
         model.fe_input_spec = FeInputSpec(self.torch_data['x'], model)
         tensorboard.system.network.epoch_models = {model}
         if os.path.exists(self.train_path):
             shutil.rmtree(self.train_path)
         tensorboard.on_batch_end(data=self.torch_data)
+        tensorboard.writer.flush()
         filepath = getfilepath()
         for e in tf.compat.v1.train.summary_iterator(filepath):
             for v in e.summary.value:
                 if v.tag == "torch_fc1/bias":
                     output = v.histo.num
                     self.assertEqual(output, 64.0)
 
@@ -176,8 +177,8 @@
         with self.subTest('Check if tensors.tsv was generated'):
             self.assertTrue(os.path.exists(tsv_path))
         with self.subTest('Check if embed image was generated'):
             self.assertTrue(os.path.exists(embed_img_path))
         with self.subTest('Check content of tensors.tsv'):
             self.assertEqual(tsv_data, 27 * ['1.0'])
         with self.subTest('Check embed image content'):
-            self.assertTrue(is_equal(output_img, 255 * np.ones(shape=(3, 3, 3), dtype=np.int)))
+            self.assertTrue(is_equal(output_img, 255 * np.ones(shape=(3, 3, 3), dtype=np.int32)))
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_test_report.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/io/test_traceability.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/io/test_traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_accuracy.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_calibration_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_dice.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_f1_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_mcc.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_precision.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/metric/test_recall.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/metric/test_recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_eval_essential.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_eval_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_logger.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_test_essential.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_test_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_trace.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/test_train_essential.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/test_train_essential.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import math
 import time
 import unittest
 
-import torch
-
 from fastestimator.test.unittest_util import sample_system_object
 from fastestimator.trace import TrainEssential
 from fastestimator.util.data import Data
+from fastestimator.util.util import get_num_gpus
 
 
 class TestTrainEssential(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.data = Data({'loss': 10})
         cls.train_essential = TrainEssential(monitor_names='loss')
@@ -33,15 +32,15 @@
         cls.train_essential.system.global_step = 10
         cls.train_essential.epoch_start = time.perf_counter() - 500
         cls.train_essential.step_start = time.perf_counter() - 300
 
     def test_on_begin(self):
         self.train_essential.on_begin(data=self.data)
         with self.subTest('Check number of devices'):
-            self.assertEqual(self.data['num_device'], torch.cuda.device_count())
+            self.assertEqual(self.data['num_device'], get_num_gpus())
         with self.subTest('Check logging interval'):
             self.assertEqual(self.data['logging_interval'], 5)
 
     def test_epoch_begin(self):
         self.train_essential.on_epoch_begin(data=self.data)
         with self.subTest('Epoch start time must not be none'):
             self.assertIsNotNone(self.train_essential.epoch_start)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/test_instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/test_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/trace/xai/test_label_tracker.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/trace/xai/test_label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_img_data.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_traceability_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 from pylatex.utils import NoEscape
 
-from fastestimator.schedule.lr_shedule import cosine_decay
+from fastestimator.schedule.lr_schedule import cosine_decay
 from fastestimator.util.latex_util import ContainerList, HrefFEID
 from fastestimator.util.traceability_util import _parse_lambda, _parse_lambda_fallback, _trace_value, traceable
 from fastestimator.util.base_util import Flag
 
 
 class NonTraceableObject:
     def __init__(self, a, b):
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/integration_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/integration_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_unet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_abs.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_cast.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_check_nan.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_concat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_dice_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_exp.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_gather.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_iwd.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_lambertw.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_matmul.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_maximum.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_ones_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_percentile.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_permute.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_pow.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_roll.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_sign.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_squeeze.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_shape.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_to_type.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_watch.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_where.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/backend/test_zscore.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/backend/test_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/cli/test_cli_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_data.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/pytorch/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/pytorch/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/loss/test_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/loss/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,41 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 
-from fastestimator.op.numpyop.meta import OneOf
-from fastestimator.op.numpyop.univariate import Binarize, Minmax, Normalize
+from fastestimator.op.numpyop.univariate import Normalize
 
 
-class TestOneOf(unittest.TestCase):
+class TestNormalize(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.randint(16, size=(28, 28, 3))]
-        cls.output_shape = (28, 28, 3)
-        cls.multi_input = [np.random.randint(16, size=(28, 28, 3)), np.random.randint(16, size=(28, 28, 3))]
+        cls.single_input = [np.random.rand(28, 28, 3)]
+        cls.single_output_shape = (28, 28, 3)
+        cls.multi_input = [np.random.rand(28, 28, 3), np.random.rand(28, 28, 3)]
+        cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
-        minmax = Minmax(inputs='x', outputs='x')
-        binarize = Binarize(inputs='x', outputs='x', threshold=1)
-        oneof = OneOf(minmax, binarize)
-        output = oneof.forward(data=self.single_input, state={})
+        normalize = Normalize(inputs='x', outputs='x')
+        output = normalize.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
-            self.assertEqual(output[0].shape, self.output_shape)
+            self.assertEqual(output[0].shape, self.single_output_shape)
 
     def test_multi_input(self):
-        minmax = Minmax(inputs='x', outputs='x')
         normalize = Normalize(inputs='x', outputs='x')
-        binarize = Binarize(inputs='x', outputs='x', threshold=1)
-        oneof = OneOf(minmax, normalize, binarize)
-        output = oneof.forward(data=self.multi_input, state={})
+        output = normalize.forward(data=self.multi_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
-            with self.subTest('Check output image shape'):
-                self.assertEqual(img_output.shape, self.output_shape)
+            with self.subTest('Check output mask shape'):
+                self.assertEqual(img_output.shape, self.multi_output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/test_numpyop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/test_numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_color.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 from fastestimator.op.numpyop.univariate import InvertImg
 
 
 class TestInvertImg(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.rand(28, 28, 3)]
+        cls.single_input = [np.random.rand(28, 28, 3).astype('float32')]
         cls.single_output_shape = (28, 28, 3)
-        cls.multi_input = [np.random.rand(28, 28, 3), np.random.rand(28, 28, 3)]
+        cls.multi_input = [np.random.rand(28, 28, 3).astype('float32'), np.random.rand(28, 28, 3).astype('float32')]
         cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
         invert_img = InvertImg(inputs='x', outputs='x')
         output = invert_img.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 
-from fastestimator.op.numpyop.univariate import Normalize
+from fastestimator.op.numpyop.univariate import RandomShadow
 
 
-class TestNormalize(unittest.TestCase):
+class TestRandomShadow(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.rand(28, 28, 3)]
+        cls.single_input = [np.random.rand(28, 28, 3).astype(np.float32)]
         cls.single_output_shape = (28, 28, 3)
-        cls.multi_input = [np.random.rand(28, 28, 3), np.random.rand(28, 28, 3)]
+        cls.multi_input = [np.random.rand(28, 28, 3).astype(np.float32), np.random.rand(28, 28, 3).astype(np.float32)]
         cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
-        normalize = Normalize(inputs='x', outputs='x')
-        output = normalize.forward(data=self.single_input, state={})
+        random_shadow = RandomShadow(inputs='x', outputs='x')
+        output = random_shadow.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
             self.assertEqual(output[0].shape, self.single_output_shape)
 
     def test_multi_input(self):
-        normalize = Normalize(inputs='x', outputs='x')
-        output = normalize.forward(data=self.multi_input, state={})
+        random_shadow = RandomShadow(inputs='x', outputs='x')
+        output = random_shadow.forward(data=self.multi_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
             with self.subTest('Check output mask shape'):
                 self.assertEqual(img_output.shape, self.multi_output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         int_output = [np.array([0., 0., 1., 0.])]
         op = Onehot(inputs='x', outputs='x', num_classes=4)
         data = op.forward(data=int_input, state={})
         np.testing.assert_array_equal(data, int_output)
 
     def test_label_smoothing(self):
         label_smoothing_input = [2]
-        label_smoothing_output = [np.array([0.025, 0.025, 0.925, 0.025])]
+        label_smoothing_output = [np.array([0.025, 0.025, 0.925, 0.025], dtype=np.float32)]
         op = Onehot(inputs='x', outputs='x', num_classes=4, label_smoothing=0.1)
         data = op.forward(data=label_smoothing_input, state={})
-        np.testing.assert_array_equal(data, label_smoothing_output)
+        np.testing.assert_array_almost_equal(data, label_smoothing_output, decimal=7)
 
     def test_two_d(self):
         two_d_input = [np.ones((2, 2)).astype(np.int8)]
         two_d_input[0][1, 1] = 0
         two_d_output = np.array([[[0., 1., 0., 0.], [0., 1., 0., 0.]], [[0., 1., 0., 0.], [1., 0., 0., 0.]]])
         op = Onehot(inputs='x', outputs='x', num_classes=4)
         data = op.forward(data=two_d_input, state={})
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 
-from fastestimator.op.numpyop.univariate import RandomShadow
+from fastestimator.op.numpyop.univariate import ToGray
 
 
-class TestRandomShadow(unittest.TestCase):
+class TestToGray(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.single_input = [np.random.rand(28, 28, 3).astype(np.float32)]
         cls.single_output_shape = (28, 28, 3)
         cls.multi_input = [np.random.rand(28, 28, 3).astype(np.float32), np.random.rand(28, 28, 3).astype(np.float32)]
         cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
-        random_shadow = RandomShadow(inputs='x', outputs='x')
-        output = random_shadow.forward(data=self.single_input, state={})
+        to_gray = ToGray(inputs='x', outputs='x')
+        output = to_gray.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
             self.assertEqual(output[0].shape, self.single_output_shape)
 
     def test_multi_input(self):
-        random_shadow = RandomShadow(inputs='x', outputs='x')
-        output = random_shadow.forward(data=self.multi_input, state={})
+        to_gray = ToGray(inputs='x', outputs='x')
+        output = to_gray.forward(data=self.multi_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
             with self.subTest('Check output mask shape'):
                 self.assertEqual(img_output.shape, self.multi_output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 
-from fastestimator.op.numpyop.univariate import ToGray
+from fastestimator.op.numpyop.univariate import ToSepia
 
 
-class TestToGray(unittest.TestCase):
+class TestToSepia(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.rand(28, 28, 3).astype(np.float32)]
+        cls.single_input = [np.random.rand(28, 28, 3)]
         cls.single_output_shape = (28, 28, 3)
-        cls.multi_input = [np.random.rand(28, 28, 3).astype(np.float32), np.random.rand(28, 28, 3).astype(np.float32)]
+        cls.multi_input = [np.random.rand(28, 28, 3), np.random.rand(28, 28, 3)]
         cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
-        to_gray = ToGray(inputs='x', outputs='x')
-        output = to_gray.forward(data=self.single_input, state={})
+        to_sepia = ToSepia(inputs='x', outputs='x')
+        output = to_sepia.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
             self.assertEqual(output[0].shape, self.single_output_shape)
 
     def test_multi_input(self):
-        to_gray = ToGray(inputs='x', outputs='x')
-        output = to_gray.forward(data=self.multi_input, state={})
+        to_sepia = ToSepia(inputs='x', outputs='x')
+        output = to_sepia.forward(data=self.multi_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
             with self.subTest('Check output mask shape'):
                 self.assertEqual(img_output.shape, self.multi_output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 The FastEstimator Authors. All Rights Reserved.
+# Copyright 2021 The FastEstimator Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,36 +12,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
 import numpy as np
 
-from fastestimator.op.numpyop.univariate import ToSepia
+from fastestimator.op.numpyop.univariate import TranslateY
 
 
-class TestToSepia(unittest.TestCase):
+class TestTranslateY(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.rand(28, 28, 3)]
+        cls.single_input = [np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8)]
         cls.single_output_shape = (28, 28, 3)
-        cls.multi_input = [np.random.rand(28, 28, 3), np.random.rand(28, 28, 3)]
+        cls.multi_input = [
+            np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8),
+            np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8)
+        ]
         cls.multi_output_shape = (28, 28, 3)
 
     def test_single_input(self):
-        to_sepia = ToSepia(inputs='x', outputs='x')
-        output = to_sepia.forward(data=self.single_input, state={})
+        translate_y = TranslateY(inputs='x', outputs='x')
+        output = translate_y.forward(data=self.single_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
             self.assertEqual(output[0].shape, self.single_output_shape)
 
     def test_multi_input(self):
-        to_sepia = ToSepia(inputs='x', outputs='x')
-        output = to_sepia.forward(data=self.multi_input, state={})
+        translate_y = TranslateY(inputs='x', outputs='x')
+        output = translate_y.forward(data=self.multi_input, state={})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
-            with self.subTest('Check output mask shape'):
+            with self.subTest('Check output image shape'):
                 self.assertEqual(img_output.shape, self.multi_output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 The FastEstimator Authors. All Rights Reserved.
+# Copyright 2020 The FastEstimator Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,41 +10,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import unittest
 
-import numpy as np
+import tensorflow as tf
 
-from fastestimator.op.numpyop.univariate import TranslateY
+from fastestimator.op.tensorop import LambdaOp
+from fastestimator.op.tensorop.meta import Fuse
 
 
-class TestTranslateY(unittest.TestCase):
+class TestFuse(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.single_input = [np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8)]
-        cls.single_output_shape = (28, 28, 3)
-        cls.multi_input = [
-            np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8),
-            np.random.randint(0, 256, size=(28, 28, 3)).astype(np.uint8)
-        ]
-        cls.multi_output_shape = (28, 28, 3)
-
-    def test_single_input(self):
-        translate_y = TranslateY(inputs='x', outputs='x')
-        output = translate_y.forward(data=self.single_input, state={})
+        cls.output_shape = (28, 28, 3)
+        cls.multi_input_tf = [tf.random.uniform(shape=(28, 28, 3)), tf.random.uniform(shape=(28, 28, 3))]
+
+    def test_single_input_tf(self):
+        a = LambdaOp(inputs='x', outputs='y', fn=lambda x: x + 1, mode='test')
+        b = LambdaOp(inputs=['y', 'z'], outputs='w', fn=lambda x, y: x + y, mode='test')
+        fuse = Fuse([a, b])
+        with self.subTest('Check op inputs'):
+            self.assertListEqual(fuse.inputs, ['x', 'z'])
+        with self.subTest('Check op outputs'):
+            self.assertListEqual(fuse.outputs, ['y', 'w'])
+        with self.subTest('Check op mode'):
+            self.assertSetEqual(fuse.mode, {'test'})
+        output = fuse.forward(data=self.multi_input_tf, state={"mode": "test", "deferred": {}})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output image shape'):
-            self.assertEqual(output[0].shape, self.single_output_shape)
+            self.assertEqual(output[0].shape, self.output_shape)
 
-    def test_multi_input(self):
-        translate_y = TranslateY(inputs='x', outputs='x')
-        output = translate_y.forward(data=self.multi_input, state={})
+    @tf.function
+    def test_single_input_tf_static(self):
+        a = LambdaOp(inputs='x', outputs='y', fn=lambda x: x + 1, mode='test')
+        b = LambdaOp(inputs=['y', 'z'], outputs='w', fn=lambda x, y: x + y, mode='test')
+        fuse = Fuse([a, b])
+        with self.subTest('Check op inputs'):
+            self.assertListEqual(fuse.inputs, ['x', 'z'])
+        with self.subTest('Check op outputs'):
+            self.assertListEqual(fuse.outputs, ['y', 'w'])
+        with self.subTest('Check op mode'):
+            self.assertSetEqual(fuse.mode, {'test'})
+        output = fuse.forward(data=self.multi_input_tf, state={"mode": "test", "deferred": {}})
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
-        with self.subTest('Check output list length'):
-            self.assertEqual(len(output), 2)
-        for img_output in output:
-            with self.subTest('Check output image shape'):
-                self.assertEqual(img_output.shape, self.multi_output_shape)
+        with self.subTest('Check output image shape'):
+            self.assertEqual(output[0].shape, self.output_shape)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py`

 * *Files 27% similar despite different names*

```diff
@@ -105,7 +105,44 @@
         with self.subTest('Check output type'):
             self.assertEqual(type(output), list)
         with self.subTest('Check output list length'):
             self.assertEqual(len(output), 2)
         for img_output in output:
             with self.subTest('Check output image shape'):
                 self.assertEqual(img_output.shape, self.output_shape)
+
+
+    def test_probability_left_tf(self):
+        op1 = LambdaOp(fn=lambda x: tf.convert_to_tensor(1.0), inputs="x", outputs="x")
+        op2 = LambdaOp(fn=lambda x: tf.convert_to_tensor(2.0), inputs="x", outputs="x")
+        oneof = OneOf(op1, op2, probs=[1.0, 0])
+        oneof.build('tf')
+        outputs = set(oneof.forward(data=self.single_input_tf, state={}).numpy() for _ in range(10))
+        self.assertEqual(len(outputs), 1)
+        self.assertEqual(outputs.pop(), 1.0)
+
+    def test_probability_right_tf(self):
+        op1 = LambdaOp(fn=lambda x: tf.convert_to_tensor(1.0), inputs="x", outputs="x")
+        op2 = LambdaOp(fn=lambda x: tf.convert_to_tensor(2.0), inputs="x", outputs="x")
+        oneof = OneOf(op1, op2, probs=[0, 1.0])
+        oneof.build('tf')
+        outputs = set(oneof.forward(data=self.single_input_tf, state={}).numpy() for _ in range(10))
+        self.assertEqual(len(outputs), 1)
+        self.assertEqual(outputs.pop(), 2.0)
+
+    def test_probability_left_torch(self):
+        op1 = LambdaOp(fn=lambda x: torch.zeros(1), inputs="x", outputs="x")
+        op2 = LambdaOp(fn=lambda x: torch.ones(1), inputs="x", outputs="x")
+        oneof = OneOf(op1, op2, probs=[1.0, 0])
+        oneof.build('torch')
+        outputs = set(oneof.forward(data=self.single_input_torch, state={}).numpy()[0] for _ in range(10))
+        self.assertEqual(len(outputs), 1)
+        self.assertEqual(outputs.pop(), 0)
+
+    def test_probability_right_torch(self):
+        op1 = LambdaOp(fn=lambda x: torch.zeros(1), inputs="x", outputs="x")
+        op2 = LambdaOp(fn=lambda x: torch.ones(1), inputs="x", outputs="x")
+        oneof = OneOf(op1, op2, probs=[0, 1.0])
+        oneof.build('torch')
+        outputs = set(oneof.forward(data=self.single_input_torch, state={}).numpy()[0] for _ in range(10))
+        self.assertEqual(len(outputs), 1)
+        self.assertEqual(outputs.pop(), 1)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/tensorop/test_tensorop.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/tensorop/test_tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_lr_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import math
 import unittest
 
-from fastestimator.schedule.lr_shedule import cosine_decay
+from fastestimator.schedule.lr_schedule import cosine_decay
 
 
 class TestLRSchedule(unittest.TestCase):
     def test_cosine_decay(self):
         learning_rate = cosine_decay(time=5, cycle_length=10, init_lr=0.01, min_lr=0.0)
         self.assertEqual(learning_rate, 0.005)
```

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_golden_section_search.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_golden_section_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_grid_search.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/search/test_search.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/search/test_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/logs/test_metrics.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/summary/test_summary.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/summary/test_summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/test/test_unittest_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/test/test_unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/test_auc_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/test_auc_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/trace/metric/test_bleu_score.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/trace/metric/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_data.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/util/test_wget_util.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/util/test_wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/PR_test/unit_test/xai/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/PR_test/unit_test/xai/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.5.0.dev202304171323/test/run_pr_test.py` & `fastestimator-nightly-1.6.0.dev202305310417/test/run_pr_test.py`

 * *Files identical despite different names*

