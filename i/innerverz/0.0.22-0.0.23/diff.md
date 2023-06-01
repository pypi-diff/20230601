# Comparing `tmp/innerverz-0.0.22.tar.gz` & `tmp/innerverz-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.22.tar", last modified: Tue May 30 06:43:14 2023, max compression
+gzip compressed data, was "innerverz-0.0.23.tar", last modified: Thu Jun  1 05:59:29 2023, max compression
```

## Comparing `innerverz-0.0.22.tar` & `innerverz-0.0.23.tar`

### file list

```diff
@@ -1,241 +1,132 @@
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.971875 innerverz-0.0.22/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1073 2023-05-26 05:00:26.000000 innerverz-0.0.22/LICENSE.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-30 06:43:14.971875 innerverz-0.0.22/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       10 2023-05-26 05:00:26.000000 innerverz-0.0.22/README.md
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/__init__.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz/data_process/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/data_process/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3493 2023-05-30 02:35:02.000000 innerverz-0.0.22/innerverz/data_process/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz/deblurrer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deblurrer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deblurrer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deblurrer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deblurrer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz/deca/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz/deca/models/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/FLAME.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/decoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/encoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/face_detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/lbs.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/models/resnet.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/deca/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/cfg.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/deca/utils/rasterizer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/rasterizer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/rasterizer/setup.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/renderer.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/rotation_converter.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/tensor_cropper.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deca/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/deep3dmm/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deep3dmm/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deep3dmm/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deep3dmm/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/deep3dmm/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_alignment/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/graphic_utils.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/landmark.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9719 2023-05-30 02:24:53.000000 innerverz-0.0.22/innerverz/face_alignment/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/retina_face.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_alignment/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/utils/face_align.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_alignment/utils/transform.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_enhancer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_enhancer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3760 2023-05-30 06:41:41.000000 innerverz-0.0.22/innerverz/face_enhancer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_enhancer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_enhancer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/face_parser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_parser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_parser/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_parser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/face_parser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/head_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/head_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/id_extractor/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/id_extractor/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/id_extractor/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/id_extractor/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/id_extractor/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/relighter/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/relighter/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/relighter/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/relighter/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/relighter/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/upsampler/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/upsampler/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/upsampler/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/upsampler/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/upsampler/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/utils/download.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1135 2023-05-30 02:34:43.000000 innerverz-0.0.22/innerverz/utils/input.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15896 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/utils/utils.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/video_faceparser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/video_faceparser/model/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/model/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz/video_faceparser/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/utils/corr.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/utils/extractor.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/utils/update.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-28 05:15:07.000000 innerverz-0.0.22/innerverz/video_faceparser/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.959875 innerverz-0.0.22/innerverz.egg-info/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      194 2023-05-30 06:43:14.000000 innerverz-0.0.22/innerverz.egg-info/PKG-INFO
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6840 2023-05-30 06:43:14.000000 innerverz-0.0.22/innerverz.egg-info/SOURCES.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        1 2023-05-30 06:43:14.000000 innerverz-0.0.22/innerverz.egg-info/dependency_links.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       74 2023-05-30 06:43:14.000000 innerverz-0.0.22/innerverz.egg-info/requires.txt
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       21 2023-05-30 06:43:14.000000 innerverz-0.0.22/innerverz.egg-info/top_level.txt
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz_/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1417 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/__init__.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz_/data_process/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/data_process/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3459 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/data_process/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz_/deblurrer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/deblurrer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2171 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/deblurrer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3609 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/deblurrer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      867 2023-05-26 07:19:35.000000 innerverz-0.0.22/innerverz_/deblurrer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz_/deca/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       23 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    16976 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.963875 innerverz-0.0.22/innerverz_/deca/models/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12616 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/FLAME.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2464 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/decoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1427 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/encoders.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1983 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/face_detectors.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    13786 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/lbs.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8386 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/models/resnet.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1126 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/deca/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5036 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/cfg.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/deca/utils/rasterizer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)        0 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/rasterizer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      706 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/rasterizer/setup.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    22281 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/renderer.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12710 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/rotation_converter.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5574 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/tensor_cropper.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    26962 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deca/utils/util.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/deep3dmm/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deep3dmm/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3414 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deep3dmm/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    25860 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deep3dmm/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      651 2023-05-26 07:19:36.000000 innerverz-0.0.22/innerverz_/deep3dmm/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_alignment/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      125 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6646 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/graphic_utils.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5089 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/landmark.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9535 2023-05-26 08:27:23.000000 innerverz-0.0.22/innerverz_/face_alignment/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    12774 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/retina_face.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      656 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_alignment/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       24 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3354 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/utils/face_align.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4933 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_alignment/utils/transform.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5238 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8503 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2047 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_enhancer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       30 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_enhancer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3745 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_enhancer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4079 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_enhancer/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      792 2023-05-26 07:19:37.000000 innerverz-0.0.22/innerverz_/face_enhancer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/face_parser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/face_parser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2682 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/face_parser/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    11822 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/face_parser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      713 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/face_parser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/head_color_transfer/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       22 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5409 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8742 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/nets.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      100 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     7018 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/blend_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3642 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/discriminator.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3788 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/vgg19_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     9366 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/sub_nets/warp_net.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1997 2023-05-26 07:19:38.000000 innerverz-0.0.22/innerverz_/head_color_transfer/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/id_extractor/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       29 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/id_extractor/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2253 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/id_extractor/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     5192 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/id_extractor/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      717 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/id_extractor/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/relighter/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       27 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/relighter/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2912 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/relighter/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4546 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/relighter/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3078 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/relighter/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.967875 innerverz-0.0.22/innerverz_/upsampler/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       28 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/upsampler/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     2250 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/upsampler/main.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    36818 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/upsampler/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      854 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/upsampler/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.971875 innerverz-0.0.22/innerverz_/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      109 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1438 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/utils/download.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     1009 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/utils/input.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)    15902 2023-05-26 07:19:39.000000 innerverz-0.0.22/innerverz_/utils/utils.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.971875 innerverz-0.0.22/innerverz_/video_faceparser/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       34 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6039 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/main.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.971875 innerverz-0.0.22/innerverz_/video_faceparser/model/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       79 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/model/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     4009 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/nets.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      217 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/test.py
-drwxrwxr-x   0 deep3090  (1000) deep3090  (1000)        0 2023-05-30 06:43:14.971875 innerverz-0.0.22/innerverz_/video_faceparser/utils/
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       94 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/utils/__init__.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3079 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/utils/corr.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     8847 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/utils/extractor.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     3984 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/utils/update.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)     6502 2023-05-26 07:19:40.000000 innerverz-0.0.22/innerverz_/video_faceparser/utils/util.py
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       89 2023-05-26 05:00:26.000000 innerverz-0.0.22/pyproject.toml
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)       38 2023-05-30 06:43:14.971875 innerverz-0.0.22/setup.cfg
--rw-rw-r--   0 deep3090  (1000) deep3090  (1000)      809 2023-05-30 06:43:13.000000 innerverz-0.0.22/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.848049 innerverz-0.0.23/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.23/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 05:59:29.848143 innerverz-0.0.23/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.23/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.827716 innerverz-0.0.23/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4348 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       18 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/top_level.txt
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.827891 innerverz-0.0.23/innerverz_package/
+-rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 05:57:40.000000 innerverz-0.0.23/innerverz_package/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.828207 innerverz-0.0.23/innerverz_package/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 innerverz-0.0.23/innerverz_package/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-05-28 05:12:20.000000 innerverz-0.0.23/innerverz_package/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.828811 innerverz-0.0.23/innerverz_package/deblurrer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deblurrer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2171 2023-05-26 02:33:03.000000 innerverz-0.0.23/innerverz_package/deblurrer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deblurrer/nets.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      867 2023-05-26 02:27:23.000000 innerverz-0.0.23/innerverz_package/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.829273 innerverz-0.0.23/innerverz_package/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 innerverz-0.0.23/innerverz_package/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.830461 innerverz-0.0.23/innerverz_package/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 innerverz-0.0.23/innerverz_package/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 innerverz-0.0.23/innerverz_package/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-05-26 02:23:15.000000 innerverz-0.0.23/innerverz_package/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.831342 innerverz-0.0.23/innerverz_package/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 innerverz-0.0.23/innerverz_package/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.831664 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.832325 innerverz-0.0.23/innerverz_package/deep3dmm/
+-rwxrwxr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deep3dmm/__init__.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)     3414 2023-05-26 02:33:38.000000 innerverz-0.0.23/innerverz_package/deep3dmm/main.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 innerverz-0.0.23/innerverz_package/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-05-26 02:18:50.000000 innerverz-0.0.23/innerverz_package/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.833253 innerverz-0.0.23/innerverz_package/face_alignment/
+-rw-rw-r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/graphic_utils.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 innerverz-0.0.23/innerverz_package/face_alignment/landmark.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     9474 2023-05-26 08:21:43.000000 innerverz-0.0.23/innerverz_package/face_alignment/main.py
+-rw-rw-r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-05-26 02:19:25.000000 innerverz-0.0.23/innerverz_package/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.833739 innerverz-0.0.23/innerverz_package/face_alignment/utils/
+-rw-rw-r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.834501 innerverz-0.0.23/innerverz_package/face_color_transfer/
+-rw-rw-r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-05-26 02:39:45.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.837227 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-05-26 03:32:45.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.837859 innerverz-0.0.23/innerverz_package/face_enhancer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 innerverz-0.0.23/innerverz_package/face_enhancer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 innerverz-0.0.23/innerverz_package/face_enhancer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 innerverz-0.0.23/innerverz_package/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-05-26 02:19:38.000000 innerverz-0.0.23/innerverz_package/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.838480 innerverz-0.0.23/innerverz_package/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 innerverz-0.0.23/innerverz_package/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-05-26 02:47:45.000000 innerverz-0.0.23/innerverz_package/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 innerverz-0.0.23/innerverz_package/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-05-26 02:19:14.000000 innerverz-0.0.23/innerverz_package/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.839171 innerverz-0.0.23/innerverz_package/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-05-26 02:40:27.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.841171 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-05-26 02:24:21.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.841836 innerverz-0.0.23/innerverz_package/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-05-26 07:17:39.000000 innerverz-0.0.23/innerverz_package/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-05-26 02:18:55.000000 innerverz-0.0.23/innerverz_package/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.842889 innerverz-0.0.23/innerverz_package/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 05:57:17.000000 innerverz-0.0.23/innerverz_package/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 05:56:03.000000 innerverz-0.0.23/innerverz_package/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3349 2023-06-01 05:57:53.000000 innerverz-0.0.23/innerverz_package/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 05:33:33.000000 innerverz-0.0.23/innerverz_package/reage/net_utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.843597 innerverz-0.0.23/innerverz_package/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 innerverz-0.0.23/innerverz_package/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-05-26 07:18:12.000000 innerverz-0.0.23/innerverz_package/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 innerverz-0.0.23/innerverz_package/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-05-26 02:26:04.000000 innerverz-0.0.23/innerverz_package/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.845053 innerverz-0.0.23/innerverz_package/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/upsampler/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2250 2023-05-26 02:43:13.000000 innerverz-0.0.23/innerverz_package/upsampler/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-05-26 02:25:02.000000 innerverz-0.0.23/innerverz_package/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.845884 innerverz-0.0.23/innerverz_package/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 innerverz-0.0.23/innerverz_package/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 innerverz-0.0.23/innerverz_package/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-05-26 10:10:45.000000 innerverz-0.0.23/innerverz_package/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.846962 innerverz-0.0.23/innerverz_package/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 innerverz-0.0.23/innerverz_package/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-05-26 03:34:40.000000 innerverz-0.0.23/innerverz_package/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.847125 innerverz-0.0.23/innerverz_package/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 innerverz-0.0.23/innerverz_package/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-05-26 01:33:53.000000 innerverz-0.0.23/innerverz_package/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-05-26 02:26:51.000000 innerverz-0.0.23/innerverz_package/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.847910 innerverz-0.0.23/innerverz_package/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.23/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 05:59:29.848488 innerverz-0.0.23/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 05:59:27.000000 innerverz-0.0.23/setup.py
```

### Comparing `innerverz-0.0.22/LICENSE.txt` & `innerverz-0.0.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/__init__.py` & `innerverz-0.0.23/innerverz_package/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 # video_faceparser
 --------
 
 from innerverz import Video_FaceParser
 
 V_FP = Video_FaceParser()
 
+# Reage
+--------
+
+from innerverz import Reage
+
+reage = Reage()
 
 """
 
 from .deblurrer import *
 from .data_process import *
 from .upsampler import *
 from .deep3dmm import *
@@ -102,8 +108,9 @@
 from .id_extractor import *
 from .face_parser import *
 from .utils import *
 from .face_color_transfer import *
 from .deca import *
 from .face_enhancer import *
 from .relighter import *
-from .video_faceparser import *
+from .video_faceparser import *
+from .reage import *
```

### Comparing `innerverz-0.0.22/innerverz/data_process/main.py` & `innerverz-0.0.23/innerverz_package/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deblurrer/main.py` & `innerverz-0.0.23/innerverz_package/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deblurrer/nets.py` & `innerverz-0.0.23/innerverz_package/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deblurrer/test.py` & `innerverz-0.0.23/innerverz_package/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/main.py` & `innerverz-0.0.23/innerverz_package/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/FLAME.py` & `innerverz-0.0.23/innerverz_package/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/decoders.py` & `innerverz-0.0.23/innerverz_package/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/detectors.py` & `innerverz-0.0.23/innerverz_package/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/encoders.py` & `innerverz-0.0.23/innerverz_package/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.23/innerverz_package/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/lbs.py` & `innerverz-0.0.23/innerverz_package/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/models/resnet.py` & `innerverz-0.0.23/innerverz_package/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/test.py` & `innerverz-0.0.23/innerverz_package/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/cfg.py` & `innerverz-0.0.23/innerverz_package/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/renderer.py` & `innerverz-0.0.23/innerverz_package/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.23/innerverz_package/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.23/innerverz_package/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deca/utils/util.py` & `innerverz-0.0.23/innerverz_package/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deep3dmm/main.py` & `innerverz-0.0.23/innerverz_package/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deep3dmm/nets.py` & `innerverz-0.0.23/innerverz_package/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/deep3dmm/test.py` & `innerverz-0.0.23/innerverz_package/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.23/innerverz_package/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/landmark.py` & `innerverz-0.0.23/innerverz_package/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/main.py` & `innerverz-0.0.23/innerverz_package/face_alignment/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .retina_face import RetinaFace
 from .landmark import Landmark
 from .graphic_utils import *
 
 class FaceAligner():
     def __init__(self, size = 1024, align_style = 'invz'):
         '''
-        align_style has 2 options  
+        algin_style has 2 options  
         
         "ffhq" : algorithm used in FFHQ dataset  
         
         "invz" : algorithm costumed by Innerverz.co    
         
         Methods
         --------
@@ -22,16 +22,16 @@
         - align_face_from_106
         - affine_transform
         '''
         
         self.backbone = RetinaFace()
         self.lmk_detector = Landmark()
         self.size = size
-        self.align_style = align_style
-        if self.align_style == 'ffhq':
+        self.algin_style = align_style
+        if self.algin_style == 'ffhq':
             self.index_5 = [38,88,86,52,61]
         else:
             self.index_5 = None
         
     
     def get_face(self, img):
         """
@@ -78,49 +78,45 @@
 
             aligned_face, tfm, tfm_inv = self.align_face_from_5(img, lms_5)
             return aligned_face, tfm, tfm_inv, lms_5, FaceBool, lms_106
     
         else :
             return None, None, None, None, False, None, 
     
-    def detect_lmk(self, img, target_face_num=0, pad=256):
+    def detect_lmk(self, img, target_face_num=0):
         """
         Input
         ---------
             - dtype : cv2 image
             - shape : (h, w, 3)
             - min max : (0, 255)
-            - pad[int]
             
         Output
         ---------
             - FaceBool
                 - dtype : Bool
             - lms_106
                 - dtype : numpy array
                 - shape : (106, 2)
             - lms_5
                 - dtype : numpy array
                 - shape : (5, 2)
         """
         FaceBool = False
-        pad_img = np.pad(img, ((pad, pad), (pad,pad), (0,0))) 
-        temp, _ = self.backbone.detect(pad_img)
+        temp, _ = self.backbone.detect(img)
         
         assert target_face_num < len(temp), 'index is larger than detected face' 
         
         if len(temp):
             FaceBool = True
             bbox = temp[0][0:4]
-            pad_lms_106 = self.lmk_detector.get(pad_img, bbox)
-            if self.align_style == 'ffhq': pad_lms_5 = np.array([pad_lms_106[self.index_5[0]], pad_lms_106[self.index_5[1]], pad_lms_106[self.index_5[2]], pad_lms_106[self.index_5[3]], pad_lms_106[self.index_5[4]]])
+            lms_106 = self.lmk_detector.get(img, bbox)
+            if self.align_style == 'ffhq': lms_5 = np.array([lms_106[self.index_5[0]], lms_106[self.index_5[1]], lms_106[self.index_5[2]], lms_106[self.index_5[3]], lms_106[self.index_5[4]]])
 
         if FaceBool:
-            lms_106 = pad_lms_106 - pad
-            lms_5 = pad_lms_5 - pad if self.align_style=='ffhq' else None
             return FaceBool, lms_106, lms_5
 
         else:
             return FaceBool, None, None
     
     def align_face_from_5(self, img, lms_5p, size = None) :
         """
@@ -144,15 +140,15 @@
                 - shape : (2, 3)
             - tfm_inv
                 - dtype : numpy array
                 - shape : (2, 3)
         """
         if size == None: size = self.size 
         
-        if self.align_style == 'ffhq':
+        if self.algin_style == 'ffhq':
             eye_left     = lms_5p[0]
             eye_right    = lms_5p[1]
             eye_avg      = (eye_left + eye_right) * 0.5
             eye_to_eye   = eye_right - eye_left
             mouth_left   = lms_5p[3]
             mouth_right  = lms_5p[4]
             mouth_avg    = (mouth_left + mouth_right) * 0.5
```

### Comparing `innerverz-0.0.22/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.23/innerverz_package/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/test.py` & `innerverz-0.0.23/innerverz_package/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.23/innerverz_package/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.23/innerverz_package/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/main.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_color_transfer/test.py` & `innerverz-0.0.23/innerverz_package/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_enhancer/main.py` & `innerverz-0.0.23/innerverz_package/face_enhancer/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         self.grad_mask = torch.from_numpy(get_grad_mask()).to(device)
 
     def forward(self, lmks, imgs):
         batch_num = imgs.size()[0]
 
         full_result = self.face_enhancer(imgs) # size: 1024, value range: [-1, 1]
 
-        target_R_eye = torch.zeros((batch_num, 3, 256, 256), device=self.device)
-        target_L_eye = torch.zeros((batch_num, 3, 256, 256), device=self.device) 
-        target_Mouth = torch.zeros((batch_num, 3, 256, 256), device=self.device) 
+        target_R_eye = torch.zeros((batch_num, 3, 256, 256), device='cuda')
+        target_L_eye = torch.zeros((batch_num, 3, 256, 256), device='cuda') 
+        target_Mouth = torch.zeros((batch_num, 3, 256, 256), device='cuda') 
 
         for idx in range(batch_num):
             L_xc, L_yc, _, _ = get_center_coord(lmks[idx], 'L_eye')
             R_xc, R_yc, _, _ = get_center_coord(lmks[idx], 'R_eye')
             M_xc, M_yc, _, _ = get_center_coord(lmks[idx], 'mouth')
 
             target_L_eye[idx] = full_result[idx, :, L_yc-128:L_yc+128, L_xc-128:L_xc+128]
```

### Comparing `innerverz-0.0.22/innerverz/face_enhancer/nets.py` & `innerverz-0.0.23/innerverz_package/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_enhancer/test.py` & `innerverz-0.0.23/innerverz_package/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_parser/main.py` & `innerverz-0.0.23/innerverz_package/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_parser/nets.py` & `innerverz-0.0.23/innerverz_package/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/face_parser/test.py` & `innerverz-0.0.23/innerverz_package/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/main.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/head_color_transfer/test.py` & `innerverz-0.0.23/innerverz_package/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/id_extractor/main.py` & `innerverz-0.0.23/innerverz_package/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/id_extractor/nets.py` & `innerverz-0.0.23/innerverz_package/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/id_extractor/test.py` & `innerverz-0.0.23/innerverz_package/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/relighter/main.py` & `innerverz-0.0.23/innerverz_package/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/relighter/nets.py` & `innerverz-0.0.23/innerverz_package/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/relighter/test.py` & `innerverz-0.0.23/innerverz_package/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/upsampler/main.py` & `innerverz-0.0.23/innerverz_package/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/upsampler/nets.py` & `innerverz-0.0.23/innerverz_package/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/upsampler/test.py` & `innerverz-0.0.23/innerverz_package/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/utils/download.py` & `innerverz-0.0.23/innerverz_package/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/utils/input.py` & `innerverz-0.0.23/innerverz_package/utils/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,11 @@
     elif source_type == 'pillow':
         if target == 'pillow':
             image = source
         elif target == 'cv2':
             image = np.array(source)[:,:,::-1]
     elif source_type == 'cv2':
         if target == 'pillow':
-            if len(source.shape) == 2:
-                image = Image.fromarray(source.astype(np.uint8))
-            else:
-                image = Image.fromarray(source[:,:,::-1]).convert("RGB")
+            image = Image.fromarray(source[:,:,::-1]).convert("RGB")
         elif target == 'cv2':
             image = source
     return image
```

### Comparing `innerverz-0.0.22/innerverz/utils/utils.py` & `innerverz-0.0.23/innerverz_package/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/main.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/nets.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.23/innerverz_package/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.22/innerverz_/relighter/main.py` & `innerverz-0.0.23/innerverz_package/reage/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,59 @@
 import os
 import sys
-sys.path.append('../')
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
-
-from .nets import MyGenerator
-
-from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
+from .net import MyGenerator
 from ..utils import check_ckpt_exist, get_url_id
 
-class ReLighter(nn.Module):
-    def __init__(self, folder_name='relighter', ckpt_name = 'G_129k.pt', force=False, device = 'cuda'):
+class Reage(nn.Module):
+    def __init__(self, folder_name='reage', ckpt_name = 'G_512_110k.pt', force=False, device = 'cuda'):
         """
-        Input
+        Related Links
         --------
-        - masked_gray_face
-            - dtype : tensor
-            - shape : (b, 1, 512, 512)
-            - min max (-1 1)
-            
-        - relight_detail_shape
-            - dtype : tensor
-            - shape : (b, 1, 512, 512)
-            - min max : (-1 1)
-            
-        - code_dict
-            - dtype : dict
-            
-        - id_param
-            - dtype : tensor
-            - shape : (b 512)
+        https://studios.disneyresearch.com/2022/11/30/production-ready-face-re-aging-for-visual-effects/
+        
+        Options
+        --------
+        ckpt_name
+            - G_512_130k.pt : image size(512)
+            - G_1024_110k.pt : image size(1024)
         
-        Output
+        Forwards
         --------
-        - result
+        - face image
+            - aligned face with ffhq rules
             - dtype : tensor
-            - shape : (b, 1 , 512, 512)
+            - shape : (b, 3, h, w)
             - min max : (-1 1)
+        
+        - mask 
+            - skin(1) + brow(2,3) + ears(7,8) + nose(10) + mouth(11) + lip(12,13) + neck(14) area
+            - dtype : tensor
+            - shape : (b, 1, h, w)
+            - min max : (0 or 1)
         """
-        super(ReLighter, self).__init__()
+        super(Reage, self).__init__()
         self.device = device
-        
-        self.img_size = 512
         self.generator = MyGenerator().to(self.device)
-
+        
         url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
         root = os.path.join('~/.invz_pack/', folder_name)
         ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
-        
-        ckpt = torch.load(os.path.join(ckpt_path), map_location=self.device)
+        ckpt = torch.load(ckpt_path, map_location=self.device)
+
         self.generator.load_state_dict(ckpt['model'])
         for param in self.generator.parameters():
             param.requires_grad = False
         self.generator.eval()
         del ckpt
-
-    def relight(self,):
-        return
-
-    # source light -> target light
-    def forward(self, masked_gray_face, relight_detail_shape, code_dict, id_param, output_size=None):
-        _, _, origin_h, origin_w = masked_gray_face.shape
-        
-        masked_gray_face = F.interpolate(masked_gray_face, (self.img_size, self.img_size), mode='bilinear')
-        relight_detail_shape = F.interpolate(relight_detail_shape, (self.img_size, self.img_size), mode='bilinear')
-        
-        params = torch.cat((code_dict['light'].view(1, -1), code_dict['cam'].view(1, -1), code_dict['pose'].view(1, -1), code_dict['detail'].view(1, -1), id_param), dim=-1)
-        res = self.generator(masked_gray_face, relight_detail_shape, params)
-        result = (res + masked_gray_face).clip(-1,1)
-        
-        if output_size == None:
-            _result = F.interpolate(result, (origin_h, origin_w), mode='bilinear')
-            _res = F.interpolate(res, (origin_h, origin_w), mode='bilinear')
-        else:
-            _result = F.interpolate(result, (output_size, output_size), mode='bilinear')
-            _res = F.interpolate(res, (output_size, output_size), mode='bilinear')
         
-        return _result, _res
-        
+    def forward(self, masked_image, mask, from_age, to_age):
+        
+        model_input = torch.cat((masked_image, mask * from_age / 100, mask * to_age / 100), dim=1)
+        
+        aging_delta = self.generator(model_input)
+        result = masked_image + aging_delta
+        
+        return result, aging_delta
```

### Comparing `innerverz-0.0.22/setup.py` & `innerverz-0.0.23/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.22",
+    version="0.0.23",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

