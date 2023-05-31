# Comparing `tmp/autogluon.multimodal-0.7.1b20230530.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230530.tar", last modified: Tue May 30 09:04:19 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230531.tar", last modified: Wed May 31 09:04:22 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230530.tar` & `autogluon.multimodal-0.7.1b20230531.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.753749 autogluon.multimodal-0.7.1b20230530/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-30 09:04:19.753749 autogluon.multimodal-0.7.1b20230530/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:04:19.753749 autogluon.multimodal-0.7.1b20230530/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.745749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    84510 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.749749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.749749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.749749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   120730 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.753749 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-30 09:03:44.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:19.741749 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:04:19.000000 autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.735572 autogluon.multimodal-0.7.1b20230531/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-31 09:04:22.735572 autogluon.multimodal-0.7.1b20230531/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:04:22.735572 autogluon.multimodal-0.7.1b20230531/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.719572 autogluon.multimodal-0.7.1b20230531/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.719572 autogluon.multimodal-0.7.1b20230531/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.723572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.723572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.723572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.727572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.731572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.731572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.731572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.731572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.731572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.735572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118889 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.735572 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-31 09:03:45.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:22.723572 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:22.000000 autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230530/PKG-INFO` & `autogluon.multimodal-0.7.1b20230531/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230530
+Version: 0.7.1b20230531
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230530/setup.py` & `autogluon.multimodal-0.7.1b20230531/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,18 @@
     create_siamese_model,
     customize_model_names,
     data_to_df,
     extract_from_output,
     filter_hyperparameters,
     get_available_devices,
     get_config,
+    get_dir_ckpt_paths,
     get_fit_complete_message,
     get_fit_start_message,
+    get_load_ckpt_paths,
     get_local_pretrained_config_paths,
     get_minmax_mode,
     get_stopping_threshold,
     hyperparameter_tune,
     infer_dtypes_by_model_names,
     infer_metrics,
     infer_precision,
@@ -1937,61 +1939,31 @@
             Verbosity levels range from 0 to 4 and control how much information is printed.
             Higher levels correspond to more detailed print statements (you can set verbosity = 0 to suppress warnings).
 
         Returns
         -------
         The loaded matcher object.
         """
-        path = os.path.abspath(os.path.expanduser(path))
-        assert os.path.isdir(path), f"'{path}' must be an existing directory."
+        dir_path, ckpt_path = get_dir_ckpt_paths(path=path)
+
+        assert os.path.isdir(dir_path), f"'{dir_path}' must be an existing directory."
         matcher = cls(query="", response="")
-        matcher = cls._load_metadata(matcher=matcher, path=path, resume=resume, verbosity=verbosity)
+        matcher = cls._load_metadata(matcher=matcher, path=dir_path, resume=resume, verbosity=verbosity)
 
         query_model, response_model = create_siamese_model(
             query_config=matcher._query_config,
             response_config=matcher._response_config,
             pretrained=False,
         )
 
-        resume_ckpt_path = os.path.join(path, LAST_CHECKPOINT)
-        final_ckpt_path = os.path.join(path, MODEL_CHECKPOINT)
-        if resume:  # resume training which crashed before
-            if not os.path.isfile(resume_ckpt_path):
-                if os.path.isfile(final_ckpt_path):
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' doesn't exist, but "
-                        f"final checkpoint '{final_ckpt_path}' exists, which means training "
-                        f"is already completed."
-                    )
-                else:
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' and "
-                        f"final checkpoint '{final_ckpt_path}' both don't exist. "
-                        f"Consider starting training from scratch."
-                    )
-            load_path = resume_ckpt_path
-            logger.info(f"Resume training from checkpoint: '{resume_ckpt_path}'")
-            ckpt_path = resume_ckpt_path
-        else:  # load a model checkpoint for prediction, evaluation, or continuing training on new data
-            if not os.path.isfile(final_ckpt_path):
-                if os.path.isfile(resume_ckpt_path):
-                    raise ValueError(
-                        f"Final checkpoint '{final_ckpt_path}' doesn't exist, but "
-                        f"resuming checkpoint '{resume_ckpt_path}' exists, which means training "
-                        f"is not done yet. Consider resume training from '{resume_ckpt_path}'."
-                    )
-                else:
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' and "
-                        f"final checkpoint '{final_ckpt_path}' both don't exist. "
-                        f"Consider starting training from scratch."
-                    )
-            load_path = final_ckpt_path
-            logger.info(f"Load pretrained checkpoint: {os.path.join(path, MODEL_CHECKPOINT)}")
-            ckpt_path = None  # must set None since we do not resume training
+        load_path, ckpt_path = get_load_ckpt_paths(
+            ckpt_path=ckpt_path,
+            dir_path=dir_path,
+            resume=resume,
+        )
 
         query_model, response_model = cls._load_state_dict(
             query_model=query_model,
             response_model=response_model,
             path=load_path,
         )
```

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,18 @@
     data_to_df,
     evaluate_coco,
     extract_from_output,
     filter_hyperparameters,
     get_available_devices,
     get_config,
     get_detection_classes,
+    get_dir_ckpt_paths,
     get_fit_complete_message,
     get_fit_start_message,
+    get_load_ckpt_paths,
     get_local_pretrained_config_paths,
     get_minmax_mode,
     get_mixup,
     get_stopping_threshold,
     hyperparameter_tune,
     infer_dtypes_by_model_names,
     infer_metrics,
@@ -148,15 +150,14 @@
     list_timm_models,
     load_text_tokenizers,
     logits_to_prob,
     merge_bio_format,
     modify_duplicate_model_names,
     object_detection_data_to_df,
     predict,
-    process_batch,
     save_ovd_result_df,
     save_pretrained_model_configs,
     save_result_df,
     save_text_tokenizers,
     select_model,
     setup_detection_train_tuning_data,
     setup_save_path,
@@ -2619,14 +2620,15 @@
         verbosity: Optional[int] = 3,
     ):
         """
         Load a predictor object from a directory specified by `path`. The to-be-loaded predictor
         can be completely or partially trained by .fit(). If a previous training has completed,
         it will load the checkpoint `model.ckpt`. Otherwise if a previous training accidentally
         collapses in the middle, it can load the `last.ckpt` checkpoint by setting `resume=True`.
+        It also supports loading one specific checkpoint given its path.
 
         Parameters
         ----------
         path
             The directory to load the predictor object.
         resume
             Whether to resume training from `last.ckpt`. This is useful when a training was accidentally
@@ -2635,29 +2637,30 @@
             Verbosity levels range from 0 to 4 and control how much information is printed.
             Higher levels correspond to more detailed print statements (you can set verbosity = 0 to suppress warnings).
 
         Returns
         -------
         The loaded predictor object.
         """
-        path = os.path.abspath(os.path.expanduser(path))
-        assert os.path.isdir(path), f"'{path}' must be an existing directory."
+        dir_path, ckpt_path = get_dir_ckpt_paths(path=path)
+
+        assert os.path.isdir(dir_path), f"'{dir_path}' must be an existing directory."
         predictor = cls(label="dummy_label")
 
-        with open(os.path.join(path, "assets.json"), "r") as fp:
+        with open(os.path.join(dir_path, "assets.json"), "r") as fp:
             assets = json.load(fp)
         if "class_name" in assets and assets["class_name"] == "MultiModalMatcher":
             predictor._matcher = MultiModalMatcher.load(
                 path=path,
                 resume=resume,
                 verbosity=verbosity,
             )
             return predictor
 
-        predictor = cls._load_metadata(predictor=predictor, path=path, resume=resume, verbosity=verbosity)
+        predictor = cls._load_metadata(predictor=predictor, path=dir_path, resume=resume, verbosity=verbosity)
 
         efficient_finetune = OmegaConf.select(predictor._config, "optimization.efficient_finetune")
 
         model = create_fusion_model(
             config=predictor._config,
             num_classes=predictor._output_shape,
             classes=predictor._classes,
@@ -2670,50 +2673,19 @@
 
         if predictor._data_processors is None:
             predictor._data_processors = create_fusion_data_processors(
                 config=predictor._config,
                 model=model,
             )
 
-        resume_ckpt_path = os.path.join(path, LAST_CHECKPOINT)
-        final_ckpt_path = os.path.join(path, MODEL_CHECKPOINT)
-        if resume:  # resume training which crashed before
-            if not os.path.isfile(resume_ckpt_path):
-                if os.path.isfile(final_ckpt_path):
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' doesn't exist, but "
-                        f"final checkpoint '{final_ckpt_path}' exists, which means training "
-                        f"is already completed."
-                    )
-                else:
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' and "
-                        f"final checkpoint '{final_ckpt_path}' both don't exist. "
-                        f"Consider starting training from scratch."
-                    )
-            load_path = resume_ckpt_path
-            logger.info(f"Resume training from checkpoint: '{resume_ckpt_path}'")
-            ckpt_path = resume_ckpt_path
-        else:  # load a model checkpoint for prediction, evaluation, or continuing training on new data
-            if not os.path.isfile(final_ckpt_path):
-                if os.path.isfile(resume_ckpt_path):
-                    raise ValueError(
-                        f"Final checkpoint '{final_ckpt_path}' doesn't exist, but "
-                        f"resuming checkpoint '{resume_ckpt_path}' exists, which means training "
-                        f"is not done yet. Consider resume training from '{resume_ckpt_path}'."
-                    )
-                else:
-                    raise ValueError(
-                        f"Resuming checkpoint '{resume_ckpt_path}' and "
-                        f"final checkpoint '{final_ckpt_path}' both don't exist. "
-                        f"Consider starting training from scratch."
-                    )
-            load_path = final_ckpt_path
-            logger.info(f"Load pretrained checkpoint: {os.path.join(path, MODEL_CHECKPOINT)}")
-            ckpt_path = None  # must set None since we do not resume training
+        load_path, ckpt_path = get_load_ckpt_paths(
+            ckpt_path=ckpt_path,
+            dir_path=dir_path,
+            resume=resume,
+        )
 
         model = cls._load_state_dict(
             model=model,
             path=load_path,
             strict=not efficient_finetune or efficient_finetune == "None",
         )
```

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     infer_precision,
     is_interactive,
     move_to_device,
 )
 from .export import ExportMixin
 from .hpo import hyperparameter_tune
 from .inference import extract_from_output, infer_batch, predict, process_batch, use_realtime
-from .load import CustomUnpickler, load_text_tokenizers
+from .load import CustomUnpickler, get_dir_ckpt_paths, get_load_ckpt_paths, load_text_tokenizers
 from .log import LogFilter, apply_log_filter, get_fit_complete_message, get_fit_start_message, make_exp_dir
 from .map import MeanAveragePrecision
 from .matcher import compute_semantic_similarity, convert_data_for_ranking, create_siamese_model, semantic_search
 from .metric import compute_ranking_score, compute_score, get_minmax_mode, get_stopping_threshold, infer_metrics
 from .misc import logits_to_prob, merge_bio_format, shopee_dataset, tensor_to_ndarray, visualize_ner
 from .mmcv import CollateMMDet, CollateMMOcr, send_datacontainers_to_device, unpack_datacontainers
 from .model import create_fusion_model, create_model, list_timm_models, modify_duplicate_model_names, select_model
```

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230531/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230530
+Version: 0.7.1b20230531
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230530/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230531/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230530
-autogluon.features==0.7.1b20230530
-autogluon.common==0.7.1b20230530
+autogluon.core[raytune]==0.7.1b20230531
+autogluon.features==0.7.1b20230531
+autogluon.common==0.7.1b20230531
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>0.1.5
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

