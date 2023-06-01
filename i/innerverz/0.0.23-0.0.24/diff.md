# Comparing `tmp/innerverz-0.0.23.tar.gz` & `tmp/innerverz-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.23.tar", last modified: Thu Jun  1 05:59:29 2023, max compression
+gzip compressed data, was "innerverz-0.0.24.tar", last modified: Thu Jun  1 06:03:37 2023, max compression
```

## Comparing `innerverz-0.0.23.tar` & `innerverz-0.0.24.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.848049 innerverz-0.0.23/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.23/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 05:59:29.848143 innerverz-0.0.23/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.23/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.827716 innerverz-0.0.23/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4348 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       18 2023-06-01 05:59:29.000000 innerverz-0.0.23/innerverz.egg-info/top_level.txt
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.827891 innerverz-0.0.23/innerverz_package/
--rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 05:57:40.000000 innerverz-0.0.23/innerverz_package/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.828207 innerverz-0.0.23/innerverz_package/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 innerverz-0.0.23/innerverz_package/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-05-28 05:12:20.000000 innerverz-0.0.23/innerverz_package/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.828811 innerverz-0.0.23/innerverz_package/deblurrer/
--rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deblurrer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     2171 2023-05-26 02:33:03.000000 innerverz-0.0.23/innerverz_package/deblurrer/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deblurrer/nets.py
--rwxr-xr-x   0 jjy        (501) staff       (20)      867 2023-05-26 02:27:23.000000 innerverz-0.0.23/innerverz_package/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.829273 innerverz-0.0.23/innerverz_package/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 innerverz-0.0.23/innerverz_package/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.830461 innerverz-0.0.23/innerverz_package/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 innerverz-0.0.23/innerverz_package/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 innerverz-0.0.23/innerverz_package/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-05-26 02:23:15.000000 innerverz-0.0.23/innerverz_package/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.831342 innerverz-0.0.23/innerverz_package/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 innerverz-0.0.23/innerverz_package/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.831664 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/
--rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 innerverz-0.0.23/innerverz_package/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 innerverz-0.0.23/innerverz_package/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.832325 innerverz-0.0.23/innerverz_package/deep3dmm/
--rwxrwxr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/deep3dmm/__init__.py
--rwxrwxr-x   0 jjy        (501) staff       (20)     3414 2023-05-26 02:33:38.000000 innerverz-0.0.23/innerverz_package/deep3dmm/main.py
--rwxrwxr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 innerverz-0.0.23/innerverz_package/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-05-26 02:18:50.000000 innerverz-0.0.23/innerverz_package/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.833253 innerverz-0.0.23/innerverz_package/face_alignment/
--rw-rw-r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/__init__.py
--rw-rw-r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/graphic_utils.py
--rw-rw-r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 innerverz-0.0.23/innerverz_package/face_alignment/landmark.py
--rw-rw-r--   0 jjy        (501) staff       (20)     9474 2023-05-26 08:21:43.000000 innerverz-0.0.23/innerverz_package/face_alignment/main.py
--rw-rw-r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-05-26 02:19:25.000000 innerverz-0.0.23/innerverz_package/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.833739 innerverz-0.0.23/innerverz_package/face_alignment/utils/
--rw-rw-r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/__init__.py
--rw-rw-r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.834501 innerverz-0.0.23/innerverz_package/face_color_transfer/
--rw-rw-r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-05-26 02:39:45.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.837227 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-05-26 03:32:45.000000 innerverz-0.0.23/innerverz_package/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.837859 innerverz-0.0.23/innerverz_package/face_enhancer/
--rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 innerverz-0.0.23/innerverz_package/face_enhancer/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 innerverz-0.0.23/innerverz_package/face_enhancer/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 innerverz-0.0.23/innerverz_package/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-05-26 02:19:38.000000 innerverz-0.0.23/innerverz_package/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.838480 innerverz-0.0.23/innerverz_package/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 innerverz-0.0.23/innerverz_package/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-05-26 02:47:45.000000 innerverz-0.0.23/innerverz_package/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 innerverz-0.0.23/innerverz_package/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-05-26 02:19:14.000000 innerverz-0.0.23/innerverz_package/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.839171 innerverz-0.0.23/innerverz_package/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-05-26 02:40:27.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.841171 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-05-26 02:24:21.000000 innerverz-0.0.23/innerverz_package/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.841836 innerverz-0.0.23/innerverz_package/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-05-26 07:17:39.000000 innerverz-0.0.23/innerverz_package/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-05-26 02:18:55.000000 innerverz-0.0.23/innerverz_package/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.842889 innerverz-0.0.23/innerverz_package/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 05:57:17.000000 innerverz-0.0.23/innerverz_package/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 05:56:03.000000 innerverz-0.0.23/innerverz_package/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3349 2023-06-01 05:57:53.000000 innerverz-0.0.23/innerverz_package/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 05:33:33.000000 innerverz-0.0.23/innerverz_package/reage/net_utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.843597 innerverz-0.0.23/innerverz_package/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 innerverz-0.0.23/innerverz_package/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-05-26 07:18:12.000000 innerverz-0.0.23/innerverz_package/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 innerverz-0.0.23/innerverz_package/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-05-26 02:26:04.000000 innerverz-0.0.23/innerverz_package/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.845053 innerverz-0.0.23/innerverz_package/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/upsampler/__init__.py
--rwxr-xr-x   0 jjy        (501) staff       (20)     2250 2023-05-26 02:43:13.000000 innerverz-0.0.23/innerverz_package/upsampler/main.py
--rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-05-26 02:25:02.000000 innerverz-0.0.23/innerverz_package/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.845884 innerverz-0.0.23/innerverz_package/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 innerverz-0.0.23/innerverz_package/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 innerverz-0.0.23/innerverz_package/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 innerverz-0.0.23/innerverz_package/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-05-26 10:10:45.000000 innerverz-0.0.23/innerverz_package/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.846962 innerverz-0.0.23/innerverz_package/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 innerverz-0.0.23/innerverz_package/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-05-26 03:34:40.000000 innerverz-0.0.23/innerverz_package/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.847125 innerverz-0.0.23/innerverz_package/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 innerverz-0.0.23/innerverz_package/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-05-26 01:33:53.000000 innerverz-0.0.23/innerverz_package/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-05-26 02:26:51.000000 innerverz-0.0.23/innerverz_package/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 05:59:29.847910 innerverz-0.0.23/innerverz_package/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 innerverz-0.0.23/innerverz_package/video_faceparser/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.23/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 05:59:29.848488 innerverz-0.0.23/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 05:59:27.000000 innerverz-0.0.23/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.916183 innerverz-0.0.24/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.24/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:03:37.916284 innerverz-0.0.24/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.24/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.898876 innerverz-0.0.24/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 05:57:40.000000 innerverz-0.0.24/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.900001 innerverz-0.0.24/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-05-25 04:27:01.000000 innerverz-0.0.24/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-05-28 05:12:20.000000 innerverz-0.0.24/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.900594 innerverz-0.0.24/innerverz/deblurrer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deblurrer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2171 2023-05-26 02:33:03.000000 innerverz-0.0.24/innerverz/deblurrer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3609 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deblurrer/nets.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      867 2023-05-26 02:27:23.000000 innerverz-0.0.24/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.901145 innerverz-0.0.24/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    16976 2023-05-25 06:56:05.000000 innerverz-0.0.24/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.902305 innerverz-0.0.24/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-05-24 06:09:07.000000 innerverz-0.0.24/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-05-24 04:57:50.000000 innerverz-0.0.24/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-05-26 02:23:15.000000 innerverz-0.0.24/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.903198 innerverz-0.0.24/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-05-24 05:33:36.000000 innerverz-0.0.24/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.903506 innerverz-0.0.24/innerverz/deca/utils/rasterizer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rasterizer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)      706 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-05-24 04:57:52.000000 innerverz-0.0.24/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-05-24 04:57:51.000000 innerverz-0.0.24/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.904138 innerverz-0.0.24/innerverz/deep3dmm/
+-rwxrwxr-x   0 jjy        (501) staff       (20)       27 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/deep3dmm/__init__.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)     3414 2023-05-26 02:33:38.000000 innerverz-0.0.24/innerverz/deep3dmm/main.py
+-rwxrwxr-x   0 jjy        (501) staff       (20)    25860 2023-05-25 02:02:16.000000 innerverz-0.0.24/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-05-26 02:18:50.000000 innerverz-0.0.24/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.905086 innerverz-0.0.24/innerverz/face_alignment/
+-rw-rw-r--   0 jjy        (501) staff       (20)      125 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     6646 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/graphic_utils.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     5089 2023-05-25 02:04:04.000000 innerverz-0.0.24/innerverz/face_alignment/landmark.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     9474 2023-05-26 08:21:43.000000 innerverz-0.0.24/innerverz/face_alignment/main.py
+-rw-rw-r--   0 jjy        (501) staff       (20)    12774 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-05-26 02:19:25.000000 innerverz-0.0.24/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.905592 innerverz-0.0.24/innerverz/face_alignment/utils/
+-rw-rw-r--   0 jjy        (501) staff       (20)       24 2023-05-25 02:04:18.000000 innerverz-0.0.24/innerverz/face_alignment/utils/__init__.py
+-rw-rw-r--   0 jjy        (501) staff       (20)     3354 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.906211 innerverz-0.0.24/innerverz/face_color_transfer/
+-rw-rw-r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:44.000000 innerverz-0.0.24/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-05-26 02:39:45.000000 innerverz-0.0.24/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-05-25 06:09:56.000000 innerverz-0.0.24/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.906999 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-05-26 03:32:45.000000 innerverz-0.0.24/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.907654 innerverz-0.0.24/innerverz/face_enhancer/
+-rwxr-xr-x   0 jjy        (501) staff       (20)       30 2023-05-24 05:06:22.000000 innerverz-0.0.24/innerverz/face_enhancer/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     3745 2023-05-25 05:57:15.000000 innerverz-0.0.24/innerverz/face_enhancer/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     4079 2023-05-24 05:06:21.000000 innerverz-0.0.24/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-05-26 02:19:38.000000 innerverz-0.0.24/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.908244 innerverz-0.0.24/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-25 02:00:51.000000 innerverz-0.0.24/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-05-26 02:47:45.000000 innerverz-0.0.24/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-05-25 02:00:38.000000 innerverz-0.0.24/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-05-26 02:19:14.000000 innerverz-0.0.24/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.908844 innerverz-0.0.24/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-05-25 04:32:32.000000 innerverz-0.0.24/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-05-26 02:40:27.000000 innerverz-0.0.24/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-05-25 06:24:09.000000 innerverz-0.0.24/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.909609 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-05-26 02:24:21.000000 innerverz-0.0.24/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.910201 innerverz-0.0.24/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-05-26 07:17:39.000000 innerverz-0.0.24/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-05-26 02:18:55.000000 innerverz-0.0.24/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.910789 innerverz-0.0.24/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 05:57:17.000000 innerverz-0.0.24/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 05:56:03.000000 innerverz-0.0.24/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3349 2023-06-01 05:57:53.000000 innerverz-0.0.24/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 05:33:33.000000 innerverz-0.0.24/innerverz/reage/net_utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.911366 innerverz-0.0.24/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-05-24 05:03:33.000000 innerverz-0.0.24/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-05-26 07:18:12.000000 innerverz-0.0.24/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-05-25 04:23:49.000000 innerverz-0.0.24/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-05-26 02:26:04.000000 innerverz-0.0.24/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.913524 innerverz-0.0.24/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/upsampler/__init__.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)     2250 2023-05-26 02:43:13.000000 innerverz-0.0.24/innerverz/upsampler/main.py
+-rwxr-xr-x   0 jjy        (501) staff       (20)    36818 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-05-26 02:25:02.000000 innerverz-0.0.24/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.914237 innerverz-0.0.24/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-05-25 01:56:47.000000 innerverz-0.0.24/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-05-24 07:27:58.000000 innerverz-0.0.24/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1009 2023-05-23 07:04:26.000000 innerverz-0.0.24/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-05-26 10:10:45.000000 innerverz-0.0.24/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.914882 innerverz-0.0.24/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-05-25 11:12:49.000000 innerverz-0.0.24/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-05-26 03:34:40.000000 innerverz-0.0.24/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.915066 innerverz-0.0.24/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-05-24 07:24:49.000000 innerverz-0.0.24/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-05-26 01:33:53.000000 innerverz-0.0.24/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-05-26 02:26:51.000000 innerverz-0.0.24/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.916010 innerverz-0.0.24/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-05-25 05:03:53.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-05-25 05:01:36.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-05-25 04:43:21.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-05-25 04:43:21.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-05-25 04:58:45.000000 innerverz-0.0.24/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-01 06:03:37.899685 innerverz-0.0.24/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     3588 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-01 06:03:37.000000 innerverz-0.0.24/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.24/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-01 06:03:37.916637 innerverz-0.0.24/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-01 06:03:29.000000 innerverz-0.0.24/setup.py
```

### Comparing `innerverz-0.0.23/LICENSE.txt` & `innerverz-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/__init__.py` & `innerverz-0.0.24/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/data_process/main.py` & `innerverz-0.0.24/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deblurrer/main.py` & `innerverz-0.0.24/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deblurrer/nets.py` & `innerverz-0.0.24/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deblurrer/test.py` & `innerverz-0.0.24/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/main.py` & `innerverz-0.0.24/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/FLAME.py` & `innerverz-0.0.24/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/decoders.py` & `innerverz-0.0.24/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/detectors.py` & `innerverz-0.0.24/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/encoders.py` & `innerverz-0.0.24/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/face_detectors.py` & `innerverz-0.0.24/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/lbs.py` & `innerverz-0.0.24/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/models/resnet.py` & `innerverz-0.0.24/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/test.py` & `innerverz-0.0.24/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/cfg.py` & `innerverz-0.0.24/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/rasterizer/setup.py` & `innerverz-0.0.24/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/renderer.py` & `innerverz-0.0.24/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/rotation_converter.py` & `innerverz-0.0.24/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/tensor_cropper.py` & `innerverz-0.0.24/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deca/utils/util.py` & `innerverz-0.0.24/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deep3dmm/main.py` & `innerverz-0.0.24/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deep3dmm/nets.py` & `innerverz-0.0.24/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/deep3dmm/test.py` & `innerverz-0.0.24/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/graphic_utils.py` & `innerverz-0.0.24/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/landmark.py` & `innerverz-0.0.24/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/main.py` & `innerverz-0.0.24/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/retina_face.py` & `innerverz-0.0.24/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/test.py` & `innerverz-0.0.24/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/utils/face_align.py` & `innerverz-0.0.24/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_alignment/utils/transform.py` & `innerverz-0.0.24/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/main.py` & `innerverz-0.0.24/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/nets.py` & `innerverz-0.0.24/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.24/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_color_transfer/test.py` & `innerverz-0.0.24/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_enhancer/main.py` & `innerverz-0.0.24/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_enhancer/nets.py` & `innerverz-0.0.24/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_enhancer/test.py` & `innerverz-0.0.24/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_parser/main.py` & `innerverz-0.0.24/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_parser/nets.py` & `innerverz-0.0.24/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/face_parser/test.py` & `innerverz-0.0.24/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/main.py` & `innerverz-0.0.24/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/nets.py` & `innerverz-0.0.24/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.24/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/head_color_transfer/test.py` & `innerverz-0.0.24/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/id_extractor/main.py` & `innerverz-0.0.24/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/id_extractor/nets.py` & `innerverz-0.0.24/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/id_extractor/test.py` & `innerverz-0.0.24/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/reage/main.py` & `innerverz-0.0.24/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/reage/net.py` & `innerverz-0.0.24/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/reage/net_utils.py` & `innerverz-0.0.24/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/relighter/main.py` & `innerverz-0.0.24/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/relighter/nets.py` & `innerverz-0.0.24/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/relighter/test.py` & `innerverz-0.0.24/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/upsampler/main.py` & `innerverz-0.0.24/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/upsampler/nets.py` & `innerverz-0.0.24/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/upsampler/test.py` & `innerverz-0.0.24/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/utils/download.py` & `innerverz-0.0.24/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/utils/input.py` & `innerverz-0.0.24/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/utils/utils.py` & `innerverz-0.0.24/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/main.py` & `innerverz-0.0.24/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/nets.py` & `innerverz-0.0.24/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/utils/corr.py` & `innerverz-0.0.24/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/utils/extractor.py` & `innerverz-0.0.24/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/utils/update.py` & `innerverz-0.0.24/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/innerverz_package/video_faceparser/utils/util.py` & `innerverz-0.0.24/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.23/setup.py` & `innerverz-0.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.23",
+    version="0.0.24",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

