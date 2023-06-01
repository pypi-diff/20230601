# Comparing `tmp/innerverz-0.0.24.tar.gz` & `tmp/innerverz-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.24.tar", last modified: Thu Jun  1 06:03:37 2023, max compression
+gzip compressed data, was "innerverz-0.0.25.tar", last modified: Thu Jun  1 06:11:49 2023, max compression
```

## Comparing `innerverz-0.0.24.tar` & `innerverz-0.0.25.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.916183 innerverz-0.0.24/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.24/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:03:37.916284 innerverz-0.0.24/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.24/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.898876 innerverz-0.0.24/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 05:57:40.000000 innerverz-0.0.24/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.900001 innerverz-0.0.24/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 innerverz-0.0.24/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-05-28 05:12:20.000000 innerverz-0.0.24/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.900594 innerverz-0.0.24/innerverz/deblurrer/
--rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deblurrer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     2171 2023-05-26 02:33:03.000000 innerverz-0.0.24/innerverz/deblurrer/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deblurrer/nets.py
--rwxr-xr-x   0 jjy        (501) staff       (20)      867 2023-05-26 02:27:23.000000 innerverz-0.0.24/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.901145 innerverz-0.0.24/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 innerverz-0.0.24/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.902305 innerverz-0.0.24/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 innerverz-0.0.24/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 innerverz-0.0.24/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-05-26 02:23:15.000000 innerverz-0.0.24/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.903198 innerverz-0.0.24/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 innerverz-0.0.24/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.903506 innerverz-0.0.24/innerverz/deca/utils/rasterizer/
--rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rasterizer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.904138 innerverz-0.0.24/innerverz/deep3dmm/
--rwxrwxr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deep3dmm/__init__.py
--rwxrwxr-x   0 jjy        (501) staff       (20)     3414 2023-05-26 02:33:38.000000 innerverz-0.0.24/innerverz/deep3dmm/main.py
--rwxrwxr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 innerverz-0.0.24/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-05-26 02:18:50.000000 innerverz-0.0.24/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.905086 innerverz-0.0.24/innerverz/face_alignment/
--rw-rw-r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/__init__.py
--rw-rw-r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/graphic_utils.py
--rw-rw-r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 innerverz-0.0.24/innerverz/face_alignment/landmark.py
--rw-rw-r--   0 jjy        (501) staff       (20)     9474 2023-05-26 08:21:43.000000 innerverz-0.0.24/innerverz/face_alignment/main.py
--rw-rw-r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-05-26 02:19:25.000000 innerverz-0.0.24/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.905592 innerverz-0.0.24/innerverz/face_alignment/utils/
--rw-rw-r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 innerverz-0.0.24/innerverz/face_alignment/utils/__init__.py
--rw-rw-r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.906211 innerverz-0.0.24/innerverz/face_color_transfer/
--rw-rw-r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 innerverz-0.0.24/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-05-26 02:39:45.000000 innerverz-0.0.24/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 innerverz-0.0.24/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.906999 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-05-26 03:32:45.000000 innerverz-0.0.24/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.907654 innerverz-0.0.24/innerverz/face_enhancer/
--rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 innerverz-0.0.24/innerverz/face_enhancer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 innerverz-0.0.24/innerverz/face_enhancer/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 innerverz-0.0.24/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-05-26 02:19:38.000000 innerverz-0.0.24/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.908244 innerverz-0.0.24/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 innerverz-0.0.24/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-05-26 02:47:45.000000 innerverz-0.0.24/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 innerverz-0.0.24/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-05-26 02:19:14.000000 innerverz-0.0.24/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.908844 innerverz-0.0.24/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 innerverz-0.0.24/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-05-26 02:40:27.000000 innerverz-0.0.24/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 innerverz-0.0.24/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.909609 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-05-26 02:24:21.000000 innerverz-0.0.24/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.910201 innerverz-0.0.24/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-05-26 07:17:39.000000 innerverz-0.0.24/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-05-26 02:18:55.000000 innerverz-0.0.24/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.910789 innerverz-0.0.24/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 05:57:17.000000 innerverz-0.0.24/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 05:56:03.000000 innerverz-0.0.24/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3349 2023-06-01 05:57:53.000000 innerverz-0.0.24/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 05:33:33.000000 innerverz-0.0.24/innerverz/reage/net_utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.911366 innerverz-0.0.24/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 innerverz-0.0.24/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-05-26 07:18:12.000000 innerverz-0.0.24/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 innerverz-0.0.24/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-05-26 02:26:04.000000 innerverz-0.0.24/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.913524 innerverz-0.0.24/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/upsampler/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     2250 2023-05-26 02:43:13.000000 innerverz-0.0.24/innerverz/upsampler/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-05-26 02:25:02.000000 innerverz-0.0.24/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.914237 innerverz-0.0.24/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 innerverz-0.0.24/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 innerverz-0.0.24/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-05-26 10:10:45.000000 innerverz-0.0.24/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.914882 innerverz-0.0.24/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 innerverz-0.0.24/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-05-26 03:34:40.000000 innerverz-0.0.24/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.915066 innerverz-0.0.24/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 innerverz-0.0.24/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-05-26 01:33:53.000000 innerverz-0.0.24/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-05-26 02:26:51.000000 innerverz-0.0.24/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.916010 innerverz-0.0.24/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.899685 innerverz-0.0.24/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     3588 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.24/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 06:03:37.916637 innerverz-0.0.24/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 06:03:29.000000 innerverz-0.0.24/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.779596 innerverz-0.0.25/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.25/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:11:49.779690 innerverz-0.0.25/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.25/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.761180 innerverz-0.0.25/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 05:57:40.000000 innerverz-0.0.25/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.762326 innerverz-0.0.25/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 innerverz-0.0.25/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-05-28 05:12:20.000000 innerverz-0.0.25/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.763317 innerverz-0.0.25/innerverz/deblurrer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/deblurrer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2171 2023-05-26 02:33:03.000000 innerverz-0.0.25/innerverz/deblurrer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/deblurrer/nets.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      843 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.763967 innerverz-0.0.25/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 innerverz-0.0.25/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.765634 innerverz-0.0.25/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 innerverz-0.0.25/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 innerverz-0.0.25/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1102 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.766671 innerverz-0.0.25/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.25/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 innerverz-0.0.25/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.767096 innerverz-0.0.25/innerverz/deca/utils/rasterizer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.25/innerverz/deca/utils/rasterizer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 innerverz-0.0.25/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 innerverz-0.0.25/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 innerverz-0.0.25/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 innerverz-0.0.25/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.768371 innerverz-0.0.25/innerverz/deep3dmm/
+-rwxrwxr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/deep3dmm/__init__.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)     3414 2023-05-26 02:33:38.000000 innerverz-0.0.25/innerverz/deep3dmm/main.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 innerverz-0.0.25/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      627 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.769345 innerverz-0.0.25/innerverz/face_alignment/
+-rw-rw-r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_alignment/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_alignment/graphic_utils.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 innerverz-0.0.25/innerverz/face_alignment/landmark.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     9474 2023-05-26 08:21:43.000000 innerverz-0.0.25/innerverz/face_alignment/main.py
+-rw-rw-r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      640 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.769844 innerverz-0.0.25/innerverz/face_alignment/utils/
+-rw-rw-r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 innerverz-0.0.25/innerverz/face_alignment/utils/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.770569 innerverz-0.0.25/innerverz/face_color_transfer/
+-rw-rw-r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 innerverz-0.0.25/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-05-26 02:39:45.000000 innerverz-0.0.25/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 innerverz-0.0.25/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.771405 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2015 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.772032 innerverz-0.0.25/innerverz/face_enhancer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 innerverz-0.0.25/innerverz/face_enhancer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 innerverz-0.0.25/innerverz/face_enhancer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 innerverz-0.0.25/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      768 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.772628 innerverz-0.0.25/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 innerverz-0.0.25/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-05-26 02:47:45.000000 innerverz-0.0.25/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 innerverz-0.0.25/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      689 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.773225 innerverz-0.0.25/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 innerverz-0.0.25/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-05-26 02:40:27.000000 innerverz-0.0.25/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 innerverz-0.0.25/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.774074 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1965 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.774732 innerverz-0.0.25/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-05-26 07:17:39.000000 innerverz-0.0.25/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      693 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.775325 innerverz-0.0.25/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 05:57:17.000000 innerverz-0.0.25/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 06:11:37.000000 innerverz-0.0.25/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3349 2023-06-01 05:57:53.000000 innerverz-0.0.25/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 05:33:33.000000 innerverz-0.0.25/innerverz/reage/net_utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.775883 innerverz-0.0.25/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 innerverz-0.0.25/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-05-26 07:18:12.000000 innerverz-0.0.25/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 innerverz-0.0.25/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3030 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.776559 innerverz-0.0.25/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/upsampler/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2250 2023-05-26 02:43:13.000000 innerverz-0.0.25/innerverz/upsampler/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      830 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.777474 innerverz-0.0.25/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 innerverz-0.0.25/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 innerverz-0.0.25/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 innerverz-0.0.25/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-05-26 10:10:45.000000 innerverz-0.0.25/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.778102 innerverz-0.0.25/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 innerverz-0.0.25/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-05-26 03:34:40.000000 innerverz-0.0.25/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.778285 innerverz-0.0.25/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 innerverz-0.0.25/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-05-26 01:33:53.000000 innerverz-0.0.25/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      209 2023-06-01 06:03:46.000000 innerverz-0.0.25/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.779401 innerverz-0.0.25/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 innerverz-0.0.25/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 innerverz-0.0.25/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 innerverz-0.0.25/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 innerverz-0.0.25/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 innerverz-0.0.25/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:11:49.762016 innerverz-0.0.25/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:11:49.000000 innerverz-0.0.25/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     3588 2023-06-01 06:11:49.000000 innerverz-0.0.25/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 06:11:49.000000 innerverz-0.0.25/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 06:11:49.000000 innerverz-0.0.25/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-01 06:11:49.000000 innerverz-0.0.25/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.25/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 06:11:49.780602 innerverz-0.0.25/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 06:11:46.000000 innerverz-0.0.25/setup.py
```

### Comparing `innerverz-0.0.24/LICENSE.txt` & `innerverz-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/__init__.py` & `innerverz-0.0.25/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/data_process/main.py` & `innerverz-0.0.25/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deblurrer/main.py` & `innerverz-0.0.25/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deblurrer/nets.py` & `innerverz-0.0.25/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deblurrer/test.py` & `innerverz-0.0.25/innerverz/deblurrer/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import cv2
 from PIL import Image
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 """
                 deblurrer usage
 """
-from innerverz_package import DeBlurrer
+from innerverz import DeBlurrer
 DB = DeBlurrer()
 ts_aligned_face = DP.image_pp(aligned_face, 1024, False, True, True, 'cuda')
 fake, fake_res, edge = DB(ts_aligned_face)
 _fake = DP.vis_pp(fake)
 _fake_res = DP.vis_pp(fake_res)
 _edge = DP.vis_pp(edge)
```

### Comparing `innerverz-0.0.24/innerverz/deca/main.py` & `innerverz-0.0.25/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/FLAME.py` & `innerverz-0.0.25/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/decoders.py` & `innerverz-0.0.25/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/detectors.py` & `innerverz-0.0.25/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/encoders.py` & `innerverz-0.0.25/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.25/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/lbs.py` & `innerverz-0.0.25/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/models/resnet.py` & `innerverz-0.0.25/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/test.py` & `innerverz-0.0.25/innerverz/deca/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import cv2
 import torch.nn.functional as F
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
 image_path = 'sample.png'
 DP = Data_Process()
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
 """
         DECA usage
 """
-from innerverz_package import DECA
+from innerverz import DECA
 deca = DECA()
 image_dict = deca.data_preprocess(aligned_face, aligned_lmk)
 code_dict, vis_dict = deca(image_dict)
 
 inputs = DP.vis_pp(vis_dict['inputs'], normalize=False)
 landmarks2d = DP.vis_pp(vis_dict['landmarks2d'], normalize=False)
 landmarks3d = DP.vis_pp(vis_dict['landmarks3d'], normalize=False)
```

### Comparing `innerverz-0.0.24/innerverz/deca/utils/cfg.py` & `innerverz-0.0.25/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.25/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/utils/renderer.py` & `innerverz-0.0.25/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.25/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.25/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deca/utils/util.py` & `innerverz-0.0.25/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deep3dmm/main.py` & `innerverz-0.0.25/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/deep3dmm/nets.py` & `innerverz-0.0.25/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.25/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/landmark.py` & `innerverz-0.0.25/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/main.py` & `innerverz-0.0.25/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.25/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/test.py` & `innerverz-0.0.25/innerverz/face_alignment/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import cv2
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
```

### Comparing `innerverz-0.0.24/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.25/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.25/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/main.py` & `innerverz-0.0.25/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.25/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.25/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_color_transfer/test.py` & `innerverz-0.0.25/innerverz/head_color_transfer/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,66 @@
+import torch
 import cv2
-import numpy as np
 from PIL import Image
-import torch
-from innerverz_package import Data_Process
+
+from innerverz import Data_Process
+from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
-    
+
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
     
+
 """
-        face color transfer
+        head color transfer
 """
-from innerverz_package import IWCT
-iwct = IWCT()
+from innerverz import HWCT
+hwct = HWCT()
+
 # data pp
-pp_label = DP.vis_pp(label, normalize=False, color=False)
-convexhull_onehot = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=True)
+head_onehot = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=True)
 gray_aligned_face = DP.image_pp(aligned_face, 512, True, True)
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True)
-convexhull_mask = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=False)
-convexhull_mask = torch.where(convexhull_mask != 0, 1, 0)
-color_aligned_face = color_aligned_face * convexhull_mask
-gray_aligned_face = gray_aligned_face * convexhull_mask
+head_mask = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=False)
+head_mask = torch.where(head_mask != 0, 1, 0)
+color_aligned_face = color_aligned_face * head_mask
+gray_aligned_face = gray_aligned_face * head_mask
 
-result, color_reference_map = iwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), convexhull_onehot, convexhull_onehot, gray_aligned_face, convexhull_mask)
+result, color_reference_map = hwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), head_onehot, head_onehot, gray_aligned_face, head_mask)
 _color_aligned_face = DP.vis_pp(color_aligned_face)
 _result = DP.vis_pp(result)
 _color_reference_map = DP.vis_pp(color_reference_map)
 
-cv2.imwrite('pp_label.png', pp_label*10+60)
-cv2.imwrite('color_alinged_face.png', _color_aligned_face)
-cv2.imwrite('ct_result.png', _result)
-cv2.imwrite('color_reference.png', _color_reference_map)
+cv2.imwrite('head_pp_label.png', pp_label*10+60)
+cv2.imwrite('head_color_alinged_face.png', _color_aligned_face)
+cv2.imwrite('head_ct_result.png', _result)
+cv2.imwrite('head_color_reference.png', _color_reference_map)
```

### Comparing `innerverz-0.0.24/innerverz/face_enhancer/main.py` & `innerverz-0.0.25/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_enhancer/nets.py` & `innerverz-0.0.25/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_enhancer/test.py` & `innerverz-0.0.25/innerverz/upsampler/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import cv2
+from PIL import Image
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
-image_path = 'sample.png'
 DP = Data_Process()
 
+image_path = 'sample.png'
+pil_image = Image.open(image_path)
+ts_image = DP.image_pp(pil_image, 512, normalize=True)
+
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
 """
-        face enhancer usage
+            Upsampler usage
 """
-from innerverz_package import FaceEnhancer
-FE = FaceEnhancer()
-ts_1024_aligned_face = DP.image_pp(aligned_face, 1024, normalize=True)
-result = FE(aligned_lmk[None,:,:], ts_1024_aligned_face)
-pp_result = DP.vis_pp(result, normalize=True, color=True)
+from innerverz import Upsampler
+US = Upsampler()
+ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=False)
+result = US(ts_aligned_face)
+_result = DP.vis_pp(result, normalize=False)
```

### Comparing `innerverz-0.0.24/innerverz/face_parser/main.py` & `innerverz-0.0.25/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_parser/nets.py` & `innerverz-0.0.25/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/face_parser/test.py` & `innerverz-0.0.25/innerverz/face_parser/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import cv2
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
```

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/main.py` & `innerverz-0.0.25/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.25/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.25/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/head_color_transfer/test.py` & `innerverz-0.0.25/innerverz/face_color_transfer/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-import torch
 import cv2
+import numpy as np
 from PIL import Image
-
-from innerverz_package import Data_Process
-from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
+import torch
+from innerverz import Data_Process
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
 aligned_face, tfm, tfm_inv = FA.align_face_from_5(cv2_image, lms_5)
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
-
+    
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
     
-
 """
-        head color transfer
+        face color transfer
 """
-from innerverz_package import HWCT
-hwct = HWCT()
-
+from innerverz import IWCT
+iwct = IWCT()
 # data pp
-head_onehot = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=True)
+pp_label = DP.vis_pp(label, normalize=False, color=False)
+convexhull_onehot = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=True)
 gray_aligned_face = DP.image_pp(aligned_face, 512, True, True)
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True)
-head_mask = DP.label_pp(pp_label, 'head', aligned_lmk/2, 512, one_hot=False)
-head_mask = torch.where(head_mask != 0, 1, 0)
-color_aligned_face = color_aligned_face * head_mask
-gray_aligned_face = gray_aligned_face * head_mask
+convexhull_mask = DP.label_pp(pp_label, 'convexhull', aligned_lmk/2, 512, one_hot=False)
+convexhull_mask = torch.where(convexhull_mask != 0, 1, 0)
+color_aligned_face = color_aligned_face * convexhull_mask
+gray_aligned_face = gray_aligned_face * convexhull_mask
 
-result, color_reference_map = hwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), head_onehot, head_onehot, gray_aligned_face, head_mask)
+result, color_reference_map = iwct(color_aligned_face, gray_aligned_face.repeat(1,3,1,1), convexhull_onehot, convexhull_onehot, gray_aligned_face, convexhull_mask)
 _color_aligned_face = DP.vis_pp(color_aligned_face)
 _result = DP.vis_pp(result)
 _color_reference_map = DP.vis_pp(color_reference_map)
 
-cv2.imwrite('head_pp_label.png', pp_label*10+60)
-cv2.imwrite('head_color_alinged_face.png', _color_aligned_face)
-cv2.imwrite('head_ct_result.png', _result)
-cv2.imwrite('head_color_reference.png', _color_reference_map)
+cv2.imwrite('pp_label.png', pp_label*10+60)
+cv2.imwrite('color_alinged_face.png', _color_aligned_face)
+cv2.imwrite('ct_result.png', _result)
+cv2.imwrite('color_reference.png', _color_reference_map)
```

### Comparing `innerverz-0.0.24/innerverz/id_extractor/main.py` & `innerverz-0.0.25/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/id_extractor/nets.py` & `innerverz-0.0.25/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/reage/main.py` & `innerverz-0.0.25/innerverz/reage/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 import torch.nn as nn
 
 from .net import MyGenerator
 from ..utils import check_ckpt_exist, get_url_id
 
 class Reage(nn.Module):
-    def __init__(self, folder_name='reage', ckpt_name = 'G_512_110k.pt', force=False, device = 'cuda'):
+    def __init__(self, folder_name='reage', ckpt_name = 'G_512_130k.pt', force=False, device = 'cuda'):
         """
         Related Links
         --------
         https://studios.disneyresearch.com/2022/11/30/production-ready-face-re-aging-for-visual-effects/
         
         Options
         --------
```

### Comparing `innerverz-0.0.24/innerverz/reage/net.py` & `innerverz-0.0.25/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/reage/net_utils.py` & `innerverz-0.0.25/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/relighter/main.py` & `innerverz-0.0.25/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/relighter/nets.py` & `innerverz-0.0.25/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/relighter/test.py` & `innerverz-0.0.25/innerverz/relighter/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import cv2
 import numpy as np
 from PIL import Image
 
 import torch
 import torch.nn.functional as F
 
-from innerverz_package import Data_Process
+from innerverz import Data_Process
 from torchvision.transforms.functional import to_tensor, rgb_to_grayscale
 
 DP = Data_Process()
 
 image_path = 'sample.png'
 pil_image = Image.open(image_path)
 ts_image = DP.image_pp(pil_image, 512, normalize=True)
 
 
 """
         face alignment usage
 """
-from innerverz_package import FaceAligner
+from innerverz import FaceAligner
 FA = FaceAligner(align_style='ffhq')
 
 cv2_image = cv2.imread(image_path)
 aligned_face, tfm, tfm_inv, lms_5, lms_106, face_bool = FA.get_face(cv2_image)
 
 face_bool, lms_106, lms_5 = FA.detect_lmk(cv2_image)
 
@@ -30,31 +30,31 @@
 
 aligned_lmk = FA.affine_transform(lms_106, tfm)
 
     
 """
         FaceParser usage
 """
-from innerverz_package import FaceParser
+from innerverz import FaceParser
 FP = FaceParser()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 label = FP.get_label(ts_aligned_face)
 pp_label = DP.vis_pp(label, normalize=False, color=False)
 
 """
             Relighting usage
 """
-from innerverz_package import ReLighter
+from innerverz import ReLighter
 RL = ReLighter()
 
-from innerverz_package import IdExtractor
+from innerverz import IdExtractor
 IE = IdExtractor()
 
-from innerverz_package import DECA
+from innerverz import DECA
 deca = DECA()
 
 ts_aligned_face = DP.image_pp(aligned_face, 512, normalize=True)
 id_vector = IE(ts_aligned_face)
 
 # pp
 color_aligned_face = DP.image_pp(aligned_face, 512, False, True, False, 'cpu')
```

### Comparing `innerverz-0.0.24/innerverz/upsampler/main.py` & `innerverz-0.0.25/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/upsampler/nets.py` & `innerverz-0.0.25/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/utils/download.py` & `innerverz-0.0.25/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/utils/input.py` & `innerverz-0.0.25/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/utils/utils.py` & `innerverz-0.0.25/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/main.py` & `innerverz-0.0.25/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/nets.py` & `innerverz-0.0.25/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.25/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.25/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.25/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.25/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.25/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.24/setup.py` & `innerverz-0.0.25/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.24",
+    version="0.0.25",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

