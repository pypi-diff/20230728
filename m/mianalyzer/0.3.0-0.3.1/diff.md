# Comparing `tmp/mianalyzer-0.3.0.tar.gz` & `tmp/mianalyzer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mianalyzer-0.3.0.tar", last modified: Fri Jul 21 11:58:36 2023, max compression
+gzip compressed data, was "mianalyzer-0.3.1.tar", last modified: Fri Jul 28 12:54:47 2023, max compression
```

## Comparing `mianalyzer-0.3.0.tar` & `mianalyzer-0.3.1.tar`

### file list

```diff
@@ -1,248 +1,247 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/
--rw-rw-rw-   0        0        0    35149 2021-12-20 09:08:37.000000 mianalyzer-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     2639 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2021 2023-07-17 14:38:35.000000 mianalyzer-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.867961 mianalyzer-0.3.0/mia/
--rw-rw-rw-   0        0        0      149 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/__init__.py
--rw-rw-rw-   0        0        0      147 2023-07-21 11:52:39.000000 mianalyzer-0.3.0/mia/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.871962 mianalyzer-0.3.0/mia/dl/
--rw-rw-rw-   0        0        0    12475 2023-07-10 09:57:49.000000 mianalyzer-0.3.0/mia/dl/DeepLearning.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.875963 mianalyzer-0.3.0/mia/dl/data/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/data/__init__.py
--rw-rw-rw-   0        0        0    11571 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/data/imagedata.py
--rw-rw-rw-   0        0        0     5105 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/data/labels.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.883960 mianalyzer-0.3.0/mia/dl/loss/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/__init__.py
--rw-rw-rw-   0        0        0     1898 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/classification_losses.py
--rw-rw-rw-   0        0        0     6053 2022-02-01 16:19:20.000000 mianalyzer-0.3.0/mia/dl/loss/loss_functions.py
--rw-rw-rw-   0        0        0      688 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/losses.py
--rw-rw-rw-   0        0        0     1032 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/regression_losses.py
--rw-rw-rw-   0        0        0     2712 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/segmentation_losses.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.887959 mianalyzer-0.3.0/mia/dl/machine_learning/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/__init__.py
--rw-rw-rw-   0        0        0     8186 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/machine_learning/deploy.prototxt
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.895959 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/__init__.py
--rw-rw-rw-   0        0        0     3650 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/classifiers.py
--rw-rw-rw-   0        0        0     1308 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr.py
--rw-rw-rw-   0        0        0     2275 2021-12-20 14:14:09.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr_segmentation.py
--rw-rw-rw-   0        0        0    10541 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/helpers.py
--rw-rw-rw-   0        0        0     7363 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/resnet.py
--rw-rw-rw-   0        0        0      975 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/grabcut_segmentation.py
--rw-rw-rw-   0        0        0     2632 2021-12-20 15:55:01.000000 mianalyzer-0.3.0/mia/dl/machine_learning/hed.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.899984 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/
--rw-rw-rw-   0        0        0      427 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/__init__.py
--rw-rw-rw-   0        0        0    15148 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/automatic_mask_generator.py
--rw-rw-rw-   0        0        0     2941 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/build_sam.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.911961 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/
--rw-rw-rw-   0        0        0      385 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/common.py
--rw-rw-rw-   0        0        0    14420 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/image_encoder.py
--rw-rw-rw-   0        0        0     6615 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py
--rw-rw-rw-   0        0        0     8594 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py
--rw-rw-rw-   0        0        0     7226 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/sam.py
--rw-rw-rw-   0        0        0     8397 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/transformer.py
--rw-rw-rw-   0        0        0    11633 2023-04-14 12:37:02.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/predictor.py
--rw-rw-rw-   0        0        0     2666 2023-06-30 12:58:42.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/sam.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.911961 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/
--rw-rw-rw-   0        0        0      197 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/__init__.py
--rw-rw-rw-   0        0        0    12712 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/amg.py
--rw-rw-rw-   0        0        0     5812 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/onnx.py
--rw-rw-rw-   0        0        0     3972 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/transforms.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.923288 mianalyzer-0.3.0/mia/dl/method/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/method/__init__.py
--rw-rw-rw-   0        0        0     6698 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/method/classification.py
--rw-rw-rw-   0        0        0     3344 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/mode.py
--rw-rw-rw-   0        0        0     5621 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/method/objectcounting.py
--rw-rw-rw-   0        0        0    10483 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/method/pixelbasedprediction.py
--rw-rw-rw-   0        0        0     3795 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/segmentation.py
--rw-rw-rw-   0        0        0     1149 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/undefinedmode.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.927291 mianalyzer-0.3.0/mia/dl/metric/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/__init__.py
--rw-rw-rw-   0        0        0     1155 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/classification_metrics.py
--rw-rw-rw-   0        0        0     5288 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/metric_functions.py
--rw-rw-rw-   0        0        0      756 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/metrics.py
--rw-rw-rw-   0        0        0     1094 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/regression_metrics.py
--rw-rw-rw-   0        0        0     2313 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/segmentation_metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.931290 mianalyzer-0.3.0/mia/dl/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.939290 mianalyzer-0.3.0/mia/dl/models/classification_models/
--rw-rw-rw-   0        0        0      508 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/__init__.py
--rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/__version__.py
--rw-rw-rw-   0        0        0    12132 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/classification_models.py
--rw-rw-rw-   0        0        0      347 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/keras.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.943290 mianalyzer-0.3.0/mia/dl/models/classification_models/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/__init__.py
--rw-rw-rw-   0        0        0     4470 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/_common_blocks.py
--rw-rw-rw-   0        0        0    13989 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnet.py
--rw-rw-rw-   0        0        0    10009 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnext.py
--rw-rw-rw-   0        0        0    15389 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/senet.py
--rw-rw-rw-   0        0        0     3417 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models_factory.py
--rw-rw-rw-   0        0        0      381 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/tfkeras.py
--rw-rw-rw-   0        0        0     1279 2021-12-20 15:29:13.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/weights.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.947290 mianalyzer-0.3.0/mia/dl/models/deeplab/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/deeplab/__init__.py
--rw-rw-rw-   0        0        0    21934 2023-07-07 15:01:40.000000 mianalyzer-0.3.0/mia/dl/models/deeplab/deeplab.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.956069 mianalyzer-0.3.0/mia/dl/models/efficientnet/
--rw-rw-rw-   0        0        0     2769 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/__init__.py
--rw-rw-rw-   0        0        0      772 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/__version__.py
--rw-rw-rw-   0        0        0      708 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/keras.py
--rw-rw-rw-   0        0        0    23513 2023-07-10 10:00:11.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/model.py
--rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/preprocessing.py
--rw-rw-rw-   0        0        0      732 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/tfkeras.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.972802 mianalyzer-0.3.0/mia/dl/models/keras_applications/
--rw-rw-rw-   0        0        0     2059 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/__init__.py
--rw-rw-rw-   0        0        0    10731 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/densenet.py
--rw-rw-rw-   0        0        0    12855 2021-12-20 15:53:29.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/imagenet_utils.py
--rw-rw-rw-   0        0        0    14086 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_resnet_v2.py
--rw-rw-rw-   0        0        0    13814 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_v3.py
--rw-rw-rw-   0        0        0    18056 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet.py
--rw-rw-rw-   0        0        0    19723 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet_v2.py
--rw-rw-rw-   0        0        0    28646 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/nasnet.py
--rw-rw-rw-   0        0        0     1041 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet.py
--rw-rw-rw-   0        0        0    11888 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet50.py
--rw-rw-rw-   0        0        0    20729 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_common.py
--rw-rw-rw-   0        0        0     1051 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_v2.py
--rw-rw-rw-   0        0        0     1020 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnext.py
--rw-rw-rw-   0        0        0     7706 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg16.py
--rw-rw-rw-   0        0        0     8178 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg19.py
--rw-rw-rw-   0        0        0    12771 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/xception.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.976804 mianalyzer-0.3.0/mia/dl/models/segmentation_models/
--rw-rw-rw-   0        0        0     4162 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/__init__.py
--rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/__version__.py
--rw-rw-rw-   0        0        0     8428 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/_losses.py
--rw-rw-rw-   0        0        0     8812 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/_metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.984883 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/__init__.py
--rw-rw-rw-   0        0        0     5302 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/backbones_factory.py
--rw-rw-rw-   0        0        0    14288 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py
--rw-rw-rw-   0        0        0    13856 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_v3.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.984883 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/
--rw-rw-rw-   0        0        0       71 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/__init__.py
--rw-rw-rw-   0        0        0    11669 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/functional.py
--rw-rw-rw-   0        0        0     2687 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/objects.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.992804 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/__init__.py
--rw-rw-rw-   0        0        0     2143 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_common_blocks.py
--rw-rw-rw-   0        0        0      377 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_utils.py
--rw-rw-rw-   0        0        0     9035 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/fpn.py
--rw-rw-rw-   0        0        0     9703 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/linknet.py
--rw-rw-rw-   0        0        0     8440 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/pspnet.py
--rw-rw-rw-   0        0        0     8355 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/unet.py
--rw-rw-rw-   0        0        0     3012 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.992804 mianalyzer-0.3.0/mia/dl/optimizer/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/optimizer/__init__.py
--rw-rw-rw-   0        0        0     1693 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/optimizer/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.002366 mianalyzer-0.3.0/mia/dl/training/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/training/__init__.py
--rw-rw-rw-   0        0        0    11693 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/training/augment.py
--rw-rw-rw-   0        0        0     6288 2023-07-10 09:57:49.000000 mianalyzer-0.3.0/mia/dl/training/datagenerator.py
--rw-rw-rw-   0        0        0     1664 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/training/lrschedule.py
--rw-rw-rw-   0        0        0     2929 2022-02-01 15:15:32.000000 mianalyzer-0.3.0/mia/dl/training/training_record.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.006369 mianalyzer-0.3.0/mia/dl/utils/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/utils/__init__.py
--rw-rw-rw-   0        0        0    22005 2023-07-10 10:00:11.000000 mianalyzer-0.3.0/mia/dl/utils/dl_downloads.py
--rw-rw-rw-   0        0        0     6657 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/utils/dl_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.045312 mianalyzer-0.3.0/mia/icons/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/__init__.py
--rw-rw-rw-   0        0        0     1282 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/addobject.png
--rw-rw-rw-   0        0        0     3070 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/assign.png
--rw-rw-rw-   0        0        0     1554 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/assignclass.png
--rw-rw-rw-   0        0        0     2432 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/augmentation.png
--rw-rw-rw-   0        0        0     2436 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/clear.png
--rw-rw-rw-   0        0        0     2144 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/delete.png
--rw-rw-rw-   0        0        0     3607 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/dextr.png
--rw-rw-rw-   0        0        0     2444 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/drag.png
--rw-rw-rw-   0        0        0     2215 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/draw.png
--rw-rw-rw-   0        0        0     1233 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/expand.png
--rw-rw-rw-   0        0        0     3697 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/exportallmasks.png
--rw-rw-rw-   0        0        0     5231 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/exportmask.png
--rw-rw-rw-   0        0        0     1445 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/load.png
--rw-rw-rw-   0        0        0    52773 2022-01-17 10:13:34.000000 mianalyzer-0.3.0/mia/icons/loading.png
--rw-rw-rw-   0        0        0     1676 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/loadmodel.png
--rw-rw-rw-   0        0        0    23516 2022-01-17 10:33:29.000000 mianalyzer-0.3.0/mia/icons/logo.png
--rw-rw-rw-   0        0        0     1951 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/magicwand.png
--rw-rw-rw-   0        0        0     3934 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/measure.png
--rw-rw-rw-   0        0        0     2879 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/next.png
--rw-rw-rw-   0        0        0     2797 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/objectcolor.png
--rw-rw-rw-   0        0        0     2012 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/objectnumber.png
--rw-rw-rw-   0        0        0     4019 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/poly.png
--rw-rw-rw-   0        0        0     3365 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/postprocessing.png
--rw-rw-rw-   0        0        0     7403 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/predict.png
--rw-rw-rw-   0        0        0     4157 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/predictall.png
--rw-rw-rw-   0        0        0     2975 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/previous.png
--rw-rw-rw-   0        0        0     4149 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/reset.png
--rw-rw-rw-   0        0        0     2703 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/results.png
--rw-rw-rw-   0        0        0     1599 2023-06-26 14:16:10.000000 mianalyzer-0.3.0/mia/icons/sam.png
--rw-rw-rw-   0        0        0     2682 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/saveall.png
--rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/savemodel.png
--rw-rw-rw-   0        0        0     3221 2022-05-24 12:04:22.000000 mianalyzer-0.3.0/mia/icons/setallclass.png
--rw-rw-rw-   0        0        0     2502 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/setclass.png
--rw-rw-rw-   0        0        0     4695 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/settings.png
--rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/shift.png
--rw-rw-rw-   0        0        0     3505 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/tracking.png
--rw-rw-rw-   0        0        0     7888 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/train.png
--rw-rw-rw-   0        0        0    45731 2023-06-30 12:51:41.000000 mianalyzer-0.3.0/mia/mia_gui.py
--rw-rw-rw-   0        0        0      802 2023-07-07 15:01:40.000000 mianalyzer-0.3.0/mia/startup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.061363 mianalyzer-0.3.0/mia/ui/
--rw-rw-rw-   0        0        0    30223 2023-06-30 12:48:33.000000 mianalyzer-0.3.0/mia/ui/Tools.py
--rw-rw-rw-   0        0        0    31651 2023-06-30 12:30:19.000000 mianalyzer-0.3.0/mia/ui/UI.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.069391 mianalyzer-0.3.0/mia/ui/classification/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/classification/__init__.py
--rw-rw-rw-   0        0        0     1878 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/classification/ui_ClassResults.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.073362 mianalyzer-0.3.0/mia/ui/objectdetection/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/objectdetection/__init__.py
--rw-rw-rw-   0        0        0     1558 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODPostProcessing.py
--rw-rw-rw-   0        0        0     4816 2022-02-18 13:59:46.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODResults.py
--rw-rw-rw-   0        0        0     4995 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODSettings.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.077363 mianalyzer-0.3.0/mia/ui/painter/
--rw-rw-rw-   0        0        0     8971 2023-06-30 10:23:21.000000 mianalyzer-0.3.0/mia/ui/painter/ContourPainter.py
--rw-rw-rw-   0        0        0     3687 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/ui/painter/ImageLabelPainter.py
--rw-rw-rw-   0        0        0      490 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/painter/NoPainter.py
--rw-rw-rw-   0        0        0     6900 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/ui/painter/ObjectPainter.py
--rw-rw-rw-   0        0        0    12001 2023-04-26 14:49:10.000000 mianalyzer-0.3.0/mia/ui/painter/Painter.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/painter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.085001 mianalyzer-0.3.0/mia/ui/segmentation/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/segmentation/__init__.py
--rw-rw-rw-   0        0        0     6103 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegPostProcessing.py
--rw-rw-rw-   0        0        0     8869 2022-02-01 15:26:27.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegResults.py
--rw-rw-rw-   0        0        0     5082 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegSettings.py
--rw-rw-rw-   0        0        0     3597 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/settings.py
--rw-rw-rw-   0        0        0     2272 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/style.py
--rw-rw-rw-   0        0        0      886 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_Abstract.py
--rw-rw-rw-   0        0        0    13878 2022-02-01 14:26:11.000000 mianalyzer-0.3.0/mia/ui/ui_Augment.py
--rw-rw-rw-   0        0        0    14250 2023-04-14 12:57:59.000000 mianalyzer-0.3.0/mia/ui/ui_Canvas.py
--rw-rw-rw-   0        0        0      886 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/ui/ui_Log.py
--rw-rw-rw-   0        0        0    11122 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/ui/ui_Results.py
--rw-rw-rw-   0        0        0    12026 2023-06-26 11:44:10.000000 mianalyzer-0.3.0/mia/ui/ui_Settings.py
--rw-rw-rw-   0        0        0     7685 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_TrainPlot.py
--rw-rw-rw-   0        0        0    18156 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_TrainSettings.py
--rw-rw-rw-   0        0        0    16270 2022-02-18 10:26:13.000000 mianalyzer-0.3.0/mia/ui/ui_Training.py
--rw-rw-rw-   0        0        0    10712 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/ui/ui_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.088349 mianalyzer-0.3.0/mia/utils/
--rw-rw-rw-   0        0        0     9081 2022-02-18 10:26:13.000000 mianalyzer-0.3.0/mia/utils/FilesAndFolders.py
--rw-rw-rw-   0        0        0     7370 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/utils/Image.py
--rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/Observer.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.092431 mianalyzer-0.3.0/mia/utils/postprocessing/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     9443 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/utils/postprocessing/tracking.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.096352 mianalyzer-0.3.0/mia/utils/shapes/
--rw-rw-rw-   0        0        0    16247 2022-10-13 14:15:31.000000 mianalyzer-0.3.0/mia/utils/shapes/Contour.py
--rw-rw-rw-   0        0        0     1533 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/ImageLabel.py
--rw-rw-rw-   0        0        0     4433 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/utils/shapes/Point.py
--rw-rw-rw-   0        0        0     2966 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/Shape.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/__init__.py
--rw-rw-rw-   0        0        0       86 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/utility_functions.py
--rw-rw-rw-   0        0        0      578 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/workerthread.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/mianalyzer.egg-info/
--rw-rw-rw-   0        0        0     2639 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7414 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      730 2023-07-21 11:58:21.000000 mianalyzer-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2474 2023-04-21 11:45:16.000000 mianalyzer-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.965330 mianalyzer-0.3.1/
+-rw-rw-rw-   0        0        0    35149 2021-12-20 09:08:37.000000 mianalyzer-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2640 2023-07-28 12:54:47.965330 mianalyzer-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2022 2023-07-21 12:33:20.000000 mianalyzer-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.842122 mianalyzer-0.3.1/mia/
+-rw-rw-rw-   0        0        0      149 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-07-28 12:48:20.000000 mianalyzer-0.3.1/mia/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.857749 mianalyzer-0.3.1/mia/dl/
+-rw-rw-rw-   0        0        0    12475 2023-07-10 09:57:49.000000 mianalyzer-0.3.1/mia/dl/DeepLearning.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.873369 mianalyzer-0.3.1/mia/dl/data/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/data/__init__.py
+-rw-rw-rw-   0        0        0    11571 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/dl/data/imagedata.py
+-rw-rw-rw-   0        0        0     5105 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/dl/data/labels.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.888990 mianalyzer-0.3.1/mia/dl/loss/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/loss/__init__.py
+-rw-rw-rw-   0        0        0     1898 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/loss/classification_losses.py
+-rw-rw-rw-   0        0        0     6053 2022-02-01 16:19:20.000000 mianalyzer-0.3.1/mia/dl/loss/loss_functions.py
+-rw-rw-rw-   0        0        0      688 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/loss/losses.py
+-rw-rw-rw-   0        0        0     1032 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/loss/regression_losses.py
+-rw-rw-rw-   0        0        0     2712 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/loss/segmentation_losses.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.911090 mianalyzer-0.3.1/mia/dl/machine_learning/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0     8186 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/machine_learning/deploy.prototxt
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.942350 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/__init__.py
+-rw-rw-rw-   0        0        0     3650 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/classifiers.py
+-rw-rw-rw-   0        0        0     1308 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/dextr.py
+-rw-rw-rw-   0        0        0     2275 2021-12-20 14:14:09.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/dextr_segmentation.py
+-rw-rw-rw-   0        0        0    10541 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/helpers.py
+-rw-rw-rw-   0        0        0     7363 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/dextr/resnet.py
+-rw-rw-rw-   0        0        0      975 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/machine_learning/grabcut_segmentation.py
+-rw-rw-rw-   0        0        0     2632 2021-12-20 15:55:01.000000 mianalyzer-0.3.1/mia/dl/machine_learning/hed.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:46.989215 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/
+-rw-rw-rw-   0        0        0      427 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/__init__.py
+-rw-rw-rw-   0        0        0    15148 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/automatic_mask_generator.py
+-rw-rw-rw-   0        0        0     2941 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/build_sam.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.058209 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/
+-rw-rw-rw-   0        0        0      385 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/common.py
+-rw-rw-rw-   0        0        0    14420 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/image_encoder.py
+-rw-rw-rw-   0        0        0     6615 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py
+-rw-rw-rw-   0        0        0     8594 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py
+-rw-rw-rw-   0        0        0     7226 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/sam.py
+-rw-rw-rw-   0        0        0     8397 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/transformer.py
+-rw-rw-rw-   0        0        0    11633 2023-04-14 12:37:02.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/predictor.py
+-rw-rw-rw-   0        0        0     2666 2023-06-30 12:58:42.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/sam.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.089450 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/
+-rw-rw-rw-   0        0        0      197 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/__init__.py
+-rw-rw-rw-   0        0        0    12712 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/amg.py
+-rw-rw-rw-   0        0        0     5812 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/onnx.py
+-rw-rw-rw-   0        0        0     3972 2023-04-14 11:35:19.000000 mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/transforms.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.127201 mianalyzer-0.3.1/mia/dl/method/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/method/__init__.py
+-rw-rw-rw-   0        0        0     6698 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/dl/method/classification.py
+-rw-rw-rw-   0        0        0     3344 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/dl/method/mode.py
+-rw-rw-rw-   0        0        0     5621 2022-10-13 11:57:14.000000 mianalyzer-0.3.1/mia/dl/method/objectcounting.py
+-rw-rw-rw-   0        0        0    10483 2022-10-13 11:57:14.000000 mianalyzer-0.3.1/mia/dl/method/pixelbasedprediction.py
+-rw-rw-rw-   0        0        0     3795 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/dl/method/segmentation.py
+-rw-rw-rw-   0        0        0     1149 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/dl/method/undefinedmode.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.158444 mianalyzer-0.3.1/mia/dl/metric/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/__init__.py
+-rw-rw-rw-   0        0        0     1155 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/classification_metrics.py
+-rw-rw-rw-   0        0        0     5288 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/metric_functions.py
+-rw-rw-rw-   0        0        0      756 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/metrics.py
+-rw-rw-rw-   0        0        0     1094 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/regression_metrics.py
+-rw-rw-rw-   0        0        0     2313 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/metric/segmentation_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.158444 mianalyzer-0.3.1/mia/dl/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.189687 mianalyzer-0.3.1/mia/dl/models/classification_models/
+-rw-rw-rw-   0        0        0      508 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/__version__.py
+-rw-rw-rw-   0        0        0    12132 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/classification_models.py
+-rw-rw-rw-   0        0        0      347 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/keras.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.227466 mianalyzer-0.3.1/mia/dl/models/classification_models/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models/__init__.py
+-rw-rw-rw-   0        0        0     4470 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models/_common_blocks.py
+-rw-rw-rw-   0        0        0    13989 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models/resnet.py
+-rw-rw-rw-   0        0        0    10009 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models/resnext.py
+-rw-rw-rw-   0        0        0    15389 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models/senet.py
+-rw-rw-rw-   0        0        0     3417 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/models_factory.py
+-rw-rw-rw-   0        0        0      381 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/tfkeras.py
+-rw-rw-rw-   0        0        0     1279 2021-12-20 15:29:13.000000 mianalyzer-0.3.1/mia/dl/models/classification_models/weights.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.243060 mianalyzer-0.3.1/mia/dl/models/deeplab/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/deeplab/__init__.py
+-rw-rw-rw-   0        0        0    21934 2023-07-07 15:01:40.000000 mianalyzer-0.3.1/mia/dl/models/deeplab/deeplab.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.274303 mianalyzer-0.3.1/mia/dl/models/efficientnet/
+-rw-rw-rw-   0        0        0     2769 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/__init__.py
+-rw-rw-rw-   0        0        0      772 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/__version__.py
+-rw-rw-rw-   0        0        0      708 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/keras.py
+-rw-rw-rw-   0        0        0    23513 2023-07-10 10:00:11.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/model.py
+-rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/preprocessing.py
+-rw-rw-rw-   0        0        0      732 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/efficientnet/tfkeras.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.425700 mianalyzer-0.3.1/mia/dl/models/keras_applications/
+-rw-rw-rw-   0        0        0     2059 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/__init__.py
+-rw-rw-rw-   0        0        0    10731 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/densenet.py
+-rw-rw-rw-   0        0        0    12855 2021-12-20 15:53:29.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/imagenet_utils.py
+-rw-rw-rw-   0        0        0    14086 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    13814 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/inception_v3.py
+-rw-rw-rw-   0        0        0    18056 2022-04-14 12:14:09.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/mobilenet.py
+-rw-rw-rw-   0        0        0    19723 2022-04-14 12:14:09.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/mobilenet_v2.py
+-rw-rw-rw-   0        0        0    28646 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/nasnet.py
+-rw-rw-rw-   0        0        0     1041 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet.py
+-rw-rw-rw-   0        0        0    11888 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet50.py
+-rw-rw-rw-   0        0        0    20729 2022-04-14 12:14:09.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet_common.py
+-rw-rw-rw-   0        0        0     1051 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet_v2.py
+-rw-rw-rw-   0        0        0     1020 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/resnext.py
+-rw-rw-rw-   0        0        0     7706 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/vgg16.py
+-rw-rw-rw-   0        0        0     8178 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/vgg19.py
+-rw-rw-rw-   0        0        0    12771 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/keras_applications/xception.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.453972 mianalyzer-0.3.1/mia/dl/models/segmentation_models/
+-rw-rw-rw-   0        0        0     4162 2022-10-13 11:57:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/__version__.py
+-rw-rw-rw-   0        0        0     8428 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/_losses.py
+-rw-rw-rw-   0        0        0     8812 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.479600 mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/__init__.py
+-rw-rw-rw-   0        0        0     5302 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/backbones_factory.py
+-rw-rw-rw-   0        0        0    14288 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    13856 2022-04-14 12:14:09.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/inception_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.495250 mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/
+-rw-rw-rw-   0        0        0       71 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/__init__.py
+-rw-rw-rw-   0        0        0    11669 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/functional.py
+-rw-rw-rw-   0        0        0     2687 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/objects.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.542115 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/__init__.py
+-rw-rw-rw-   0        0        0     2143 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/_common_blocks.py
+-rw-rw-rw-   0        0        0      377 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/_utils.py
+-rw-rw-rw-   0        0        0     9035 2022-01-31 10:47:17.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/fpn.py
+-rw-rw-rw-   0        0        0     9703 2022-01-31 10:47:17.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/linknet.py
+-rw-rw-rw-   0        0        0     8440 2022-01-31 10:47:17.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/pspnet.py
+-rw-rw-rw-   0        0        0     8355 2022-01-31 10:47:17.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/unet.py
+-rw-rw-rw-   0        0        0     3012 2021-12-20 08:40:49.000000 mianalyzer-0.3.1/mia/dl/models/segmentation_models/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.542115 mianalyzer-0.3.1/mia/dl/optimizer/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     1693 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/dl/optimizer/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.579920 mianalyzer-0.3.1/mia/dl/training/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/training/__init__.py
+-rw-rw-rw-   0        0        0    11693 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/dl/training/augment.py
+-rw-rw-rw-   0        0        0     6288 2023-07-10 09:57:49.000000 mianalyzer-0.3.1/mia/dl/training/datagenerator.py
+-rw-rw-rw-   0        0        0     1664 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/training/lrschedule.py
+-rw-rw-rw-   0        0        0     2929 2022-02-01 15:15:32.000000 mianalyzer-0.3.1/mia/dl/training/training_record.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.595543 mianalyzer-0.3.1/mia/dl/utils/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/dl/utils/__init__.py
+-rw-rw-rw-   0        0        0    22005 2023-07-10 10:00:11.000000 mianalyzer-0.3.1/mia/dl/utils/dl_downloads.py
+-rw-rw-rw-   0        0        0     6657 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/dl/utils/dl_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.742645 mianalyzer-0.3.1/mia/icons/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/__init__.py
+-rw-rw-rw-   0        0        0     1282 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/addobject.png
+-rw-rw-rw-   0        0        0     3070 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/assign.png
+-rw-rw-rw-   0        0        0     1554 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/assignclass.png
+-rw-rw-rw-   0        0        0     2432 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/augmentation.png
+-rw-rw-rw-   0        0        0     2436 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/clear.png
+-rw-rw-rw-   0        0        0     2144 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/delete.png
+-rw-rw-rw-   0        0        0     3607 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/dextr.png
+-rw-rw-rw-   0        0        0     2444 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/drag.png
+-rw-rw-rw-   0        0        0     2215 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/draw.png
+-rw-rw-rw-   0        0        0     1233 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/expand.png
+-rw-rw-rw-   0        0        0     3697 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/exportallmasks.png
+-rw-rw-rw-   0        0        0     5231 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/exportmask.png
+-rw-rw-rw-   0        0        0     1445 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/load.png
+-rw-rw-rw-   0        0        0    52773 2022-01-17 10:13:34.000000 mianalyzer-0.3.1/mia/icons/loading.png
+-rw-rw-rw-   0        0        0     1676 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/loadmodel.png
+-rw-rw-rw-   0        0        0    23516 2022-01-17 10:33:29.000000 mianalyzer-0.3.1/mia/icons/logo.png
+-rw-rw-rw-   0        0        0     1951 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/magicwand.png
+-rw-rw-rw-   0        0        0     3934 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/measure.png
+-rw-rw-rw-   0        0        0     2879 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/next.png
+-rw-rw-rw-   0        0        0     2797 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/objectcolor.png
+-rw-rw-rw-   0        0        0     2012 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/objectnumber.png
+-rw-rw-rw-   0        0        0     4019 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/poly.png
+-rw-rw-rw-   0        0        0     3365 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/postprocessing.png
+-rw-rw-rw-   0        0        0     7403 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/predict.png
+-rw-rw-rw-   0        0        0     4157 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/predictall.png
+-rw-rw-rw-   0        0        0     2975 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/previous.png
+-rw-rw-rw-   0        0        0     4149 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/reset.png
+-rw-rw-rw-   0        0        0     2703 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/results.png
+-rw-rw-rw-   0        0        0     2682 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/saveall.png
+-rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/savemodel.png
+-rw-rw-rw-   0        0        0     3221 2022-05-24 12:04:22.000000 mianalyzer-0.3.1/mia/icons/setallclass.png
+-rw-rw-rw-   0        0        0     2502 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/setclass.png
+-rw-rw-rw-   0        0        0     4695 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/settings.png
+-rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/shift.png
+-rw-rw-rw-   0        0        0     3505 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/tracking.png
+-rw-rw-rw-   0        0        0     7888 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/icons/train.png
+-rw-rw-rw-   0        0        0    45731 2023-06-30 12:51:41.000000 mianalyzer-0.3.1/mia/mia_gui.py
+-rw-rw-rw-   0        0        0      802 2023-07-07 15:01:40.000000 mianalyzer-0.3.1/mia/startup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.811636 mianalyzer-0.3.1/mia/ui/
+-rw-rw-rw-   0        0        0    30223 2023-06-30 12:48:33.000000 mianalyzer-0.3.1/mia/ui/Tools.py
+-rw-rw-rw-   0        0        0    31614 2023-07-28 12:48:09.000000 mianalyzer-0.3.1/mia/ui/UI.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.827288 mianalyzer-0.3.1/mia/ui/classification/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/classification/__init__.py
+-rw-rw-rw-   0        0        0     1878 2022-02-01 14:06:24.000000 mianalyzer-0.3.1/mia/ui/classification/ui_ClassResults.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.842878 mianalyzer-0.3.1/mia/ui/objectdetection/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/objectdetection/__init__.py
+-rw-rw-rw-   0        0        0     1558 2022-02-01 14:06:24.000000 mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODPostProcessing.py
+-rw-rw-rw-   0        0        0     4816 2022-02-18 13:59:46.000000 mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODResults.py
+-rw-rw-rw-   0        0        0     4995 2022-10-13 11:57:14.000000 mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODSettings.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.865064 mianalyzer-0.3.1/mia/ui/painter/
+-rw-rw-rw-   0        0        0     8971 2023-06-30 10:23:21.000000 mianalyzer-0.3.1/mia/ui/painter/ContourPainter.py
+-rw-rw-rw-   0        0        0     3687 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/ui/painter/ImageLabelPainter.py
+-rw-rw-rw-   0        0        0      490 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/painter/NoPainter.py
+-rw-rw-rw-   0        0        0     6900 2022-05-31 12:40:55.000000 mianalyzer-0.3.1/mia/ui/painter/ObjectPainter.py
+-rw-rw-rw-   0        0        0    12001 2023-04-26 14:49:10.000000 mianalyzer-0.3.1/mia/ui/painter/Painter.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/painter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.880689 mianalyzer-0.3.1/mia/ui/segmentation/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     6103 2022-02-01 14:06:24.000000 mianalyzer-0.3.1/mia/ui/segmentation/ui_SegPostProcessing.py
+-rw-rw-rw-   0        0        0     8869 2022-02-01 15:26:27.000000 mianalyzer-0.3.1/mia/ui/segmentation/ui_SegResults.py
+-rw-rw-rw-   0        0        0     5082 2022-02-01 14:06:24.000000 mianalyzer-0.3.1/mia/ui/segmentation/ui_SegSettings.py
+-rw-rw-rw-   0        0        0     3597 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/settings.py
+-rw-rw-rw-   0        0        0     2272 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/ui/style.py
+-rw-rw-rw-   0        0        0      886 2022-02-01 14:04:45.000000 mianalyzer-0.3.1/mia/ui/ui_Abstract.py
+-rw-rw-rw-   0        0        0    13878 2022-02-01 14:26:11.000000 mianalyzer-0.3.1/mia/ui/ui_Augment.py
+-rw-rw-rw-   0        0        0    14250 2023-04-14 12:57:59.000000 mianalyzer-0.3.1/mia/ui/ui_Canvas.py
+-rw-rw-rw-   0        0        0      886 2022-04-14 12:14:09.000000 mianalyzer-0.3.1/mia/ui/ui_Log.py
+-rw-rw-rw-   0        0        0    11122 2022-05-24 10:06:51.000000 mianalyzer-0.3.1/mia/ui/ui_Results.py
+-rw-rw-rw-   0        0        0    12026 2023-06-26 11:44:10.000000 mianalyzer-0.3.1/mia/ui/ui_Settings.py
+-rw-rw-rw-   0        0        0     7685 2022-02-01 14:04:45.000000 mianalyzer-0.3.1/mia/ui/ui_TrainPlot.py
+-rw-rw-rw-   0        0        0    18156 2022-02-01 14:04:45.000000 mianalyzer-0.3.1/mia/ui/ui_TrainSettings.py
+-rw-rw-rw-   0        0        0    16270 2022-02-18 10:26:13.000000 mianalyzer-0.3.1/mia/ui/ui_Training.py
+-rw-rw-rw-   0        0        0    10712 2022-05-31 12:40:55.000000 mianalyzer-0.3.1/mia/ui/ui_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.927580 mianalyzer-0.3.1/mia/utils/
+-rw-rw-rw-   0        0        0     9081 2022-02-18 10:26:13.000000 mianalyzer-0.3.1/mia/utils/FilesAndFolders.py
+-rw-rw-rw-   0        0        0     7370 2022-10-13 11:57:14.000000 mianalyzer-0.3.1/mia/utils/Image.py
+-rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/Observer.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.927580 mianalyzer-0.3.1/mia/utils/postprocessing/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     9443 2021-11-26 09:23:09.000000 mianalyzer-0.3.1/mia/utils/postprocessing/tracking.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.958826 mianalyzer-0.3.1/mia/utils/shapes/
+-rw-rw-rw-   0        0        0    16247 2022-10-13 14:15:31.000000 mianalyzer-0.3.1/mia/utils/shapes/Contour.py
+-rw-rw-rw-   0        0        0     1533 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/shapes/ImageLabel.py
+-rw-rw-rw-   0        0        0     4433 2022-05-31 12:40:55.000000 mianalyzer-0.3.1/mia/utils/shapes/Point.py
+-rw-rw-rw-   0        0        0     2966 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/shapes/Shape.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/shapes/__init__.py
+-rw-rw-rw-   0        0        0       86 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/utility_functions.py
+-rw-rw-rw-   0        0        0      578 2021-06-29 14:36:14.000000 mianalyzer-0.3.1/mia/utils/workerthread.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:54:47.965330 mianalyzer-0.3.1/mianalyzer.egg-info/
+-rw-rw-rw-   0        0        0     2640 2023-07-28 12:54:46.000000 mianalyzer-0.3.1/mianalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-07-28 12:54:46.000000 mianalyzer-0.3.1/mianalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:54:46.000000 mianalyzer-0.3.1/mianalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-28 12:54:46.000000 mianalyzer-0.3.1/mianalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-07-28 12:54:46.000000 mianalyzer-0.3.1/mianalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      669 2023-07-28 12:48:31.000000 mianalyzer-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:54:47.965330 mianalyzer-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2474 2023-04-21 11:45:16.000000 mianalyzer-0.3.1/setup.py
```

### Comparing `mianalyzer-0.3.0/LICENSE` & `mianalyzer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/PKG-INFO` & `mianalyzer-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mianalyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: MIA, deep learning based Microscopic Image Analyzer
 Home-page: https://github.com/MIAnalyzer/MIA/
 Author: Nils Koerber
 Project-URL: Homepage, https://github.com/MIAnalyzer/MIA/
 Project-URL: Bug Tracker, https://github.com/MIAnalyzer/MIA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,15 +17,15 @@
 ![MIA](https://github.com/MIAnalyzer/MIA/blob/master/docs/source/gettingstarted/images/user_interface.PNG?raw=true)
 
 MIA is a software for deep learning based image analysis. It covers image labeling, neural network training and inference. It can be used for image classification, object detection, semantic segmentation and tracking.
 
 ## Installation
 The easiest way to install MIA is via conda (see https://docs.conda.io/en/latest/miniconda.html for installation options).
 
-After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/v0.2.4/mia_environment.yaml) file. 
+After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/weights/mia_environment.yaml) file. 
 
 Then, open an anaconda prompt and type:
 - ```cd /path/to/mia_environment.yaml```  (change ```/path/to/``` to the path of the folder with the environment file)
 - ```conda env create -f mia_environment.yaml```
 - wait and follow instructions
   
 ### to start the software
```

### Comparing `mianalyzer-0.3.0/README.md` & `mianalyzer-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ![MIA](https://github.com/MIAnalyzer/MIA/blob/master/docs/source/gettingstarted/images/user_interface.PNG?raw=true)
 
 MIA is a software for deep learning based image analysis. It covers image labeling, neural network training and inference. It can be used for image classification, object detection, semantic segmentation and tracking.
 
 ## Installation
 The easiest way to install MIA is via conda (see https://docs.conda.io/en/latest/miniconda.html for installation options).
 
-After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/v0.2.4/mia_environment.yaml) file. 
+After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/weights/mia_environment.yaml) file. 
 
 Then, open an anaconda prompt and type:
 - ```cd /path/to/mia_environment.yaml```  (change ```/path/to/``` to the path of the folder with the environment file)
 - ```conda env create -f mia_environment.yaml```
 - wait and follow instructions
   
 ### to start the software
```

### Comparing `mianalyzer-0.3.0/mia/dl/DeepLearning.py` & `mianalyzer-0.3.1/mia/dl/DeepLearning.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/data/imagedata.py` & `mianalyzer-0.3.1/mia/dl/data/imagedata.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/data/labels.py` & `mianalyzer-0.3.1/mia/dl/data/labels.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/loss/classification_losses.py` & `mianalyzer-0.3.1/mia/dl/loss/classification_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/loss/loss_functions.py` & `mianalyzer-0.3.1/mia/dl/loss/loss_functions.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/loss/losses.py` & `mianalyzer-0.3.1/mia/dl/loss/losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/loss/regression_losses.py` & `mianalyzer-0.3.1/mia/dl/loss/regression_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/loss/segmentation_losses.py` & `mianalyzer-0.3.1/mia/dl/loss/segmentation_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/deploy.prototxt` & `mianalyzer-0.3.1/mia/dl/machine_learning/deploy.prototxt`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/classifiers.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/dextr/classifiers.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/dextr/dextr.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr_segmentation.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/dextr/dextr_segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/helpers.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/dextr/helpers.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/resnet.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/dextr/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/grabcut_segmentation.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/grabcut_segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/hed.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/hed.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/automatic_mask_generator.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/build_sam.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/common.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/image_encoder.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/sam.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/transformer.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/predictor.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/sam.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/sam.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/amg.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/onnx.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/transforms.py` & `mianalyzer-0.3.1/mia/dl/machine_learning/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/classification.py` & `mianalyzer-0.3.1/mia/dl/method/classification.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/mode.py` & `mianalyzer-0.3.1/mia/dl/method/mode.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/objectcounting.py` & `mianalyzer-0.3.1/mia/dl/method/objectcounting.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/pixelbasedprediction.py` & `mianalyzer-0.3.1/mia/dl/method/pixelbasedprediction.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/segmentation.py` & `mianalyzer-0.3.1/mia/dl/method/segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/method/undefinedmode.py` & `mianalyzer-0.3.1/mia/dl/method/undefinedmode.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/metric/classification_metrics.py` & `mianalyzer-0.3.1/mia/dl/metric/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/metric/metric_functions.py` & `mianalyzer-0.3.1/mia/dl/metric/metric_functions.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/metric/metrics.py` & `mianalyzer-0.3.1/mia/dl/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/metric/regression_metrics.py` & `mianalyzer-0.3.1/mia/dl/metric/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/metric/segmentation_metrics.py` & `mianalyzer-0.3.1/mia/dl/metric/segmentation_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/classification_models.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/classification_models.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/models/_common_blocks.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/models/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnet.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/models/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnext.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/models/resnext.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/models/senet.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/models/senet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/models_factory.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/models_factory.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/classification_models/weights.py` & `mianalyzer-0.3.1/mia/dl/models/classification_models/weights.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/deeplab/deeplab.py` & `mianalyzer-0.3.1/mia/dl/models/deeplab/deeplab.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/__init__.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/__version__.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/__version__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/keras.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/keras.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/model.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/model.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/preprocessing.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/efficientnet/tfkeras.py` & `mianalyzer-0.3.1/mia/dl/models/efficientnet/tfkeras.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/__init__.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/densenet.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/densenet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/imagenet_utils.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_resnet_v2.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_v3.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet_v2.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/nasnet.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet50.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet50.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_common.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet_common.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_v2.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnext.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/resnext.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg16.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg19.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/keras_applications/xception.py` & `mianalyzer-0.3.1/mia/dl/models/keras_applications/xception.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/__init__.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/_losses.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/_metrics.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/backbones_factory.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/backbones_factory.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_v3.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/backbones/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/functional.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/functional.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/objects.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/base/objects.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_common_blocks.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/fpn.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/fpn.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/linknet.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/linknet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/pspnet.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/pspnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/unet.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/models/unet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/models/segmentation_models/utils.py` & `mianalyzer-0.3.1/mia/dl/models/segmentation_models/utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/optimizer/optimizer.py` & `mianalyzer-0.3.1/mia/dl/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/training/augment.py` & `mianalyzer-0.3.1/mia/dl/training/augment.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/training/datagenerator.py` & `mianalyzer-0.3.1/mia/dl/training/datagenerator.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/training/lrschedule.py` & `mianalyzer-0.3.1/mia/dl/training/lrschedule.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/training/training_record.py` & `mianalyzer-0.3.1/mia/dl/training/training_record.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/utils/dl_downloads.py` & `mianalyzer-0.3.1/mia/dl/utils/dl_downloads.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/dl/utils/dl_utils.py` & `mianalyzer-0.3.1/mia/dl/utils/dl_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/addobject.png` & `mianalyzer-0.3.1/mia/icons/addobject.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/assign.png` & `mianalyzer-0.3.1/mia/icons/assign.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/assignclass.png` & `mianalyzer-0.3.1/mia/icons/assignclass.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/augmentation.png` & `mianalyzer-0.3.1/mia/icons/augmentation.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/clear.png` & `mianalyzer-0.3.1/mia/icons/clear.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/delete.png` & `mianalyzer-0.3.1/mia/icons/delete.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/dextr.png` & `mianalyzer-0.3.1/mia/icons/dextr.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/drag.png` & `mianalyzer-0.3.1/mia/icons/drag.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/draw.png` & `mianalyzer-0.3.1/mia/icons/draw.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/expand.png` & `mianalyzer-0.3.1/mia/icons/expand.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/exportallmasks.png` & `mianalyzer-0.3.1/mia/icons/exportallmasks.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/exportmask.png` & `mianalyzer-0.3.1/mia/icons/exportmask.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/load.png` & `mianalyzer-0.3.1/mia/icons/load.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/loading.png` & `mianalyzer-0.3.1/mia/icons/loading.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/loadmodel.png` & `mianalyzer-0.3.1/mia/icons/loadmodel.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/logo.png` & `mianalyzer-0.3.1/mia/icons/logo.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/magicwand.png` & `mianalyzer-0.3.1/mia/icons/magicwand.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/measure.png` & `mianalyzer-0.3.1/mia/icons/measure.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/next.png` & `mianalyzer-0.3.1/mia/icons/next.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/objectcolor.png` & `mianalyzer-0.3.1/mia/icons/objectcolor.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/objectnumber.png` & `mianalyzer-0.3.1/mia/icons/objectnumber.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/poly.png` & `mianalyzer-0.3.1/mia/icons/poly.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/postprocessing.png` & `mianalyzer-0.3.1/mia/icons/postprocessing.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/predict.png` & `mianalyzer-0.3.1/mia/icons/predict.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/predictall.png` & `mianalyzer-0.3.1/mia/icons/predictall.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/previous.png` & `mianalyzer-0.3.1/mia/icons/previous.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/reset.png` & `mianalyzer-0.3.1/mia/icons/reset.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/results.png` & `mianalyzer-0.3.1/mia/icons/results.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/saveall.png` & `mianalyzer-0.3.1/mia/icons/saveall.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/savemodel.png` & `mianalyzer-0.3.1/mia/icons/savemodel.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/setallclass.png` & `mianalyzer-0.3.1/mia/icons/setallclass.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/setclass.png` & `mianalyzer-0.3.1/mia/icons/setclass.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/settings.png` & `mianalyzer-0.3.1/mia/icons/settings.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/shift.png` & `mianalyzer-0.3.1/mia/icons/shift.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/tracking.png` & `mianalyzer-0.3.1/mia/icons/tracking.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/icons/train.png` & `mianalyzer-0.3.1/mia/icons/train.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/mia_gui.py` & `mianalyzer-0.3.1/mia/mia_gui.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/startup.py` & `mianalyzer-0.3.1/mia/startup.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/Tools.py` & `mianalyzer-0.3.1/mia/ui/Tools.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/UI.py` & `mianalyzer-0.3.1/mia/ui/UI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Oct 10 11:28:44 2019
 
 @author: Koerber
 """
 
-from msilib.schema import RadioButton
+
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 from PyQt5.QtCore import *
 
 from ui.ui_utils import ClassList, ClassWidget, DCDButton, LabelledSpinBox
 from ui.style import styleForm, getHighlightColor, getBackgroundColor, getBrightColor
```

### Comparing `mianalyzer-0.3.0/mia/ui/classification/ui_ClassResults.py` & `mianalyzer-0.3.1/mia/ui/classification/ui_ClassResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODPostProcessing.py` & `mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODPostProcessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODResults.py` & `mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODSettings.py` & `mianalyzer-0.3.1/mia/ui/objectdetection/ui_ODSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/painter/ContourPainter.py` & `mianalyzer-0.3.1/mia/ui/painter/ContourPainter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/painter/ImageLabelPainter.py` & `mianalyzer-0.3.1/mia/ui/painter/ImageLabelPainter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/painter/ObjectPainter.py` & `mianalyzer-0.3.1/mia/ui/painter/ObjectPainter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/painter/Painter.py` & `mianalyzer-0.3.1/mia/ui/painter/Painter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegPostProcessing.py` & `mianalyzer-0.3.1/mia/ui/segmentation/ui_SegPostProcessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegResults.py` & `mianalyzer-0.3.1/mia/ui/segmentation/ui_SegResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegSettings.py` & `mianalyzer-0.3.1/mia/ui/segmentation/ui_SegSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/settings.py` & `mianalyzer-0.3.1/mia/ui/settings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/style.py` & `mianalyzer-0.3.1/mia/ui/style.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Abstract.py` & `mianalyzer-0.3.1/mia/ui/ui_Abstract.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Augment.py` & `mianalyzer-0.3.1/mia/ui/ui_Augment.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Canvas.py` & `mianalyzer-0.3.1/mia/ui/ui_Canvas.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Log.py` & `mianalyzer-0.3.1/mia/ui/ui_Log.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Results.py` & `mianalyzer-0.3.1/mia/ui/ui_Results.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Settings.py` & `mianalyzer-0.3.1/mia/ui/ui_Settings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_TrainPlot.py` & `mianalyzer-0.3.1/mia/ui/ui_TrainPlot.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_TrainSettings.py` & `mianalyzer-0.3.1/mia/ui/ui_TrainSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_Training.py` & `mianalyzer-0.3.1/mia/ui/ui_Training.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/ui/ui_utils.py` & `mianalyzer-0.3.1/mia/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/FilesAndFolders.py` & `mianalyzer-0.3.1/mia/utils/FilesAndFolders.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/Image.py` & `mianalyzer-0.3.1/mia/utils/Image.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/Observer.py` & `mianalyzer-0.3.1/mia/utils/Observer.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/postprocessing/tracking.py` & `mianalyzer-0.3.1/mia/utils/postprocessing/tracking.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/shapes/Contour.py` & `mianalyzer-0.3.1/mia/utils/shapes/Contour.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/shapes/ImageLabel.py` & `mianalyzer-0.3.1/mia/utils/shapes/ImageLabel.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/shapes/Point.py` & `mianalyzer-0.3.1/mia/utils/shapes/Point.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/shapes/Shape.py` & `mianalyzer-0.3.1/mia/utils/shapes/Shape.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mia/utils/workerthread.py` & `mianalyzer-0.3.1/mia/utils/workerthread.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.3.0/mianalyzer.egg-info/PKG-INFO` & `mianalyzer-0.3.1/mianalyzer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mianalyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: MIA, deep learning based Microscopic Image Analyzer
 Home-page: https://github.com/MIAnalyzer/MIA/
 Author: Nils Koerber
 Project-URL: Homepage, https://github.com/MIAnalyzer/MIA/
 Project-URL: Bug Tracker, https://github.com/MIAnalyzer/MIA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,15 +17,15 @@
 ![MIA](https://github.com/MIAnalyzer/MIA/blob/master/docs/source/gettingstarted/images/user_interface.PNG?raw=true)
 
 MIA is a software for deep learning based image analysis. It covers image labeling, neural network training and inference. It can be used for image classification, object detection, semantic segmentation and tracking.
 
 ## Installation
 The easiest way to install MIA is via conda (see https://docs.conda.io/en/latest/miniconda.html for installation options).
 
-After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/v0.2.4/mia_environment.yaml) file. 
+After installation of conda, download the [environment](https://github.com/MIAnalyzer/MIA/releases/download/weights/mia_environment.yaml) file. 
 
 Then, open an anaconda prompt and type:
 - ```cd /path/to/mia_environment.yaml```  (change ```/path/to/``` to the path of the folder with the environment file)
 - ```conda env create -f mia_environment.yaml```
 - wait and follow instructions
   
 ### to start the software
```

### Comparing `mianalyzer-0.3.0/mianalyzer.egg-info/SOURCES.txt` & `mianalyzer-0.3.1/mianalyzer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,14 @@
 mia/icons/poly.png
 mia/icons/postprocessing.png
 mia/icons/predict.png
 mia/icons/predictall.png
 mia/icons/previous.png
 mia/icons/reset.png
 mia/icons/results.png
-mia/icons/sam.png
 mia/icons/saveall.png
 mia/icons/savemodel.png
 mia/icons/setallclass.png
 mia/icons/setclass.png
 mia/icons/settings.png
 mia/icons/shift.png
 mia/icons/tracking.png
```

### Comparing `mianalyzer-0.3.0/pyproject.toml` & `mianalyzer-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mianalyzer"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Nils Koerber" },
 ]
 description = "MIA, deep learning based Microscopic Image Analyzer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,10 +19,7 @@
 
 [project.urls]
 "Homepage" = "https://github.com/MIAnalyzer/MIA/"
 "Bug Tracker" = "https://github.com/MIAnalyzer/MIA/issues"
 
 [project.scripts]
 mianalyzer = "mia.startup:start"
-
-#[tool.setuptools.package-data]
-#"mia.icons" = ["*.png"]
```

### Comparing `mianalyzer-0.3.0/setup.py` & `mianalyzer-0.3.1/setup.py`

 * *Files identical despite different names*

