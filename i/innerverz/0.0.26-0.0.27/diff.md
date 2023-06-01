# Comparing `tmp/innerverz-0.0.26.tar.gz` & `tmp/innerverz-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.26.tar", last modified: Thu Jun  1 06:14:27 2023, max compression
+gzip compressed data, was "innerverz-0.0.27.tar", last modified: Thu Jun  1 06:16:04 2023, max compression
```

## Comparing `innerverz-0.0.26.tar` & `innerverz-0.0.27.tar`

### file list

```diff
@@ -1,127 +1,132 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.301515 innerverz-0.0.26/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.26/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:14:27.301925 innerverz-0.0.26/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.26/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.284318 innerverz-0.0.26/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1417 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.285427 innerverz-0.0.26/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.285996 innerverz-0.0.26/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2171 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.286478 innerverz-0.0.26/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.287623 innerverz-0.0.26/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.26/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.288525 innerverz-0.0.26/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.288991 innerverz-0.0.26/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.290025 innerverz-0.0.26/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3414 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.291073 innerverz-0.0.26/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)     9719 2023-06-01 06:14:15.000000 innerverz-0.0.26/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.291851 innerverz-0.0.26/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.292529 innerverz-0.0.26/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.293469 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.294049 innerverz-0.0.26/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3760 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.294655 innerverz-0.0.26/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.295240 innerverz-0.0.26/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.296001 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.296679 innerverz-0.0.26/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.297370 innerverz-0.0.26/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.298072 innerverz-0.0.26/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2250 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.298697 innerverz-0.0.26/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.299366 innerverz-0.0.26/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.299547 innerverz-0.0.26/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.301301 innerverz-0.0.26/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.26/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:14:27.285104 innerverz-0.0.26/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:14:27.000000 innerverz-0.0.26/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     3484 2023-06-01 06:14:27.000000 innerverz-0.0.26/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 06:14:27.000000 innerverz-0.0.26/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 06:14:27.000000 innerverz-0.0.26/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-01 06:14:27.000000 innerverz-0.0.26/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.26/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 06:14:27.302398 innerverz-0.0.26/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 06:13:37.000000 innerverz-0.0.26/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.249525 innerverz-0.0.27/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.27/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:16:04.249637 innerverz-0.0.27/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.27/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.230153 innerverz-0.0.27/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 06:15:38.000000 innerverz-0.0.27/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.231385 innerverz-0.0.27/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.232040 innerverz-0.0.27/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2171 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.232551 innerverz-0.0.27/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.233709 innerverz-0.0.27/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.27/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.235189 innerverz-0.0.27/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.235536 innerverz-0.0.27/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.236200 innerverz-0.0.27/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3414 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.237191 innerverz-0.0.27/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9719 2023-06-01 06:14:15.000000 innerverz-0.0.27/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.237680 innerverz-0.0.27/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.238294 innerverz-0.0.27/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.239143 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.239748 innerverz-0.0.27/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3760 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.240298 innerverz-0.0.27/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.240914 innerverz-0.0.27/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.241682 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.242298 innerverz-0.0.27/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.243005 innerverz-0.0.27/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.27/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3842 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/reage/net_utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.243657 innerverz-0.0.27/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.244414 innerverz-0.0.27/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2250 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.246420 innerverz-0.0.27/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.248352 innerverz-0.0.27/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.248530 innerverz-0.0.27/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.249359 innerverz-0.0.27/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.27/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:16:04.231068 innerverz-0.0.27/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:16:04.000000 innerverz-0.0.27/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     3588 2023-06-01 06:16:04.000000 innerverz-0.0.27/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 06:16:04.000000 innerverz-0.0.27/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 06:16:04.000000 innerverz-0.0.27/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-01 06:16:04.000000 innerverz-0.0.27/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.27/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 06:16:04.250766 innerverz-0.0.27/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 06:15:54.000000 innerverz-0.0.27/setup.py
```

### Comparing `innerverz-0.0.26/LICENSE.txt` & `innerverz-0.0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/__init__.py` & `innerverz-0.0.27/innerverz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 # video_faceparser
 --------
 
 from innerverz import Video_FaceParser
 
 V_FP = Video_FaceParser()
 
+# reage
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

### Comparing `innerverz-0.0.26/innerverz/data_process/main.py` & `innerverz-0.0.27/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deblurrer/main.py` & `innerverz-0.0.27/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deblurrer/nets.py` & `innerverz-0.0.27/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deblurrer/test.py` & `innerverz-0.0.27/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/main.py` & `innerverz-0.0.27/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/FLAME.py` & `innerverz-0.0.27/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/decoders.py` & `innerverz-0.0.27/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/detectors.py` & `innerverz-0.0.27/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/encoders.py` & `innerverz-0.0.27/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.27/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/lbs.py` & `innerverz-0.0.27/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/models/resnet.py` & `innerverz-0.0.27/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/test.py` & `innerverz-0.0.27/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/cfg.py` & `innerverz-0.0.27/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.27/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/renderer.py` & `innerverz-0.0.27/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.27/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.27/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deca/utils/util.py` & `innerverz-0.0.27/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deep3dmm/main.py` & `innerverz-0.0.27/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deep3dmm/nets.py` & `innerverz-0.0.27/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/deep3dmm/test.py` & `innerverz-0.0.27/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.27/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/landmark.py` & `innerverz-0.0.27/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/main.py` & `innerverz-0.0.27/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.27/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/test.py` & `innerverz-0.0.27/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.27/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.27/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/main.py` & `innerverz-0.0.27/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.27/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.27/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_color_transfer/test.py` & `innerverz-0.0.27/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_enhancer/main.py` & `innerverz-0.0.27/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_enhancer/nets.py` & `innerverz-0.0.27/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_enhancer/test.py` & `innerverz-0.0.27/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_parser/main.py` & `innerverz-0.0.27/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_parser/nets.py` & `innerverz-0.0.27/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/face_parser/test.py` & `innerverz-0.0.27/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/main.py` & `innerverz-0.0.27/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.27/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.27/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/head_color_transfer/test.py` & `innerverz-0.0.27/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/id_extractor/main.py` & `innerverz-0.0.27/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/id_extractor/nets.py` & `innerverz-0.0.27/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/id_extractor/test.py` & `innerverz-0.0.27/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/relighter/main.py` & `innerverz-0.0.27/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/relighter/nets.py` & `innerverz-0.0.27/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/relighter/test.py` & `innerverz-0.0.27/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/upsampler/main.py` & `innerverz-0.0.27/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/upsampler/nets.py` & `innerverz-0.0.27/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/upsampler/test.py` & `innerverz-0.0.27/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/utils/download.py` & `innerverz-0.0.27/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/utils/input.py` & `innerverz-0.0.27/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/utils/utils.py` & `innerverz-0.0.27/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/main.py` & `innerverz-0.0.27/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/nets.py` & `innerverz-0.0.27/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.27/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.27/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.27/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.27/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.26/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.27/innerverz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 innerverz/head_color_transfer/sub_nets/discriminator.py
 innerverz/head_color_transfer/sub_nets/vgg19_net.py
 innerverz/head_color_transfer/sub_nets/warp_net.py
 innerverz/id_extractor/__init__.py
 innerverz/id_extractor/main.py
 innerverz/id_extractor/nets.py
 innerverz/id_extractor/test.py
+innerverz/reage/__init__.py
+innerverz/reage/main.py
+innerverz/reage/net.py
+innerverz/reage/net_utils.py
 innerverz/relighter/__init__.py
 innerverz/relighter/main.py
 innerverz/relighter/nets.py
 innerverz/relighter/test.py
 innerverz/upsampler/__init__.py
 innerverz/upsampler/main.py
 innerverz/upsampler/nets.py
```

### Comparing `innerverz-0.0.26/setup.py` & `innerverz-0.0.27/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.26",
+    version="0.0.27",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

