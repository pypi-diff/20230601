# Comparing `tmp/sssegmentation-1.2.0.tar.gz` & `tmp/SSSegmentation-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sssegmentation-1.2.0.tar", last modified: Wed Aug 10 09:00:50 2022, max compression
+gzip compressed data, was "dist\SSSegmentation-1.3.0.tar", last modified: Thu Jun  1 05:55:24 2023, max compression
```

## Comparing `sssegmentation-1.2.0.tar` & `SSSegmentation-1.3.0.tar`

### file list

```diff
@@ -1,266 +1,299 @@
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/
--rw-rw-rw-   0        0        0    11560 2022-07-12 23:16:23.000000 sssegmentation-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     7045 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6439 2022-08-10 06:29:03.000000 sssegmentation-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3335 2022-07-12 22:29:06.000000 sssegmentation-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/
--rw-rw-rw-   0        0        0      496 2022-08-10 06:30:28.000000 sssegmentation-1.2.0/ssseg/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/configs/
--rw-rw-rw-   0        0        0       49 2020-11-19 13:11:51.000000 sssegmentation-1.2.0/ssseg/configs/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-11 15:01:27.000000 sssegmentation-1.2.0/ssseg/configs/builder.py
--rw-rw-rw-   0        0        0    10719 2022-08-10 06:31:13.000000 sssegmentation-1.2.0/ssseg/inference.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/
--rw-rw-rw-   0        0        0      377 2022-07-28 02:44:44.000000 sssegmentation-1.2.0/ssseg/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/datasets/
--rw-rw-rw-   0        0        0       50 2020-11-19 13:15:40.000000 sssegmentation-1.2.0/ssseg/modules/datasets/__init__.py
--rw-rw-rw-   0        0        0     5539 2022-07-09 14:58:40.000000 sssegmentation-1.2.0/ssseg/modules/datasets/ade20k.py
--rw-rw-rw-   0        0        0     1820 2022-07-09 14:59:07.000000 sssegmentation-1.2.0/ssseg/modules/datasets/atr.py
--rw-rw-rw-   0        0        0     6052 2022-07-09 14:59:42.000000 sssegmentation-1.2.0/ssseg/modules/datasets/base.py
--rw-rw-rw-   0        0        0     1989 2022-08-07 06:17:26.000000 sssegmentation-1.2.0/ssseg/modules/datasets/builder.py
--rw-rw-rw-   0        0        0     1881 2022-07-09 15:00:30.000000 sssegmentation-1.2.0/ssseg/modules/datasets/chasedb1.py
--rw-rw-rw-   0        0        0     2037 2022-07-09 15:00:58.000000 sssegmentation-1.2.0/ssseg/modules/datasets/cihp.py
--rw-rw-rw-   0        0        0     3564 2022-07-09 15:01:09.000000 sssegmentation-1.2.0/ssseg/modules/datasets/cityscapes.py
--rw-rw-rw-   0        0        0    11409 2022-07-09 15:01:43.000000 sssegmentation-1.2.0/ssseg/modules/datasets/coco.py
--rw-rw-rw-   0        0        0     1871 2022-07-09 15:02:02.000000 sssegmentation-1.2.0/ssseg/modules/datasets/drive.py
--rw-rw-rw-   0        0        0     1832 2022-07-09 15:02:15.000000 sssegmentation-1.2.0/ssseg/modules/datasets/hrf.py
--rw-rw-rw-   0        0        0     1982 2022-07-09 15:02:26.000000 sssegmentation-1.2.0/ssseg/modules/datasets/lip.py
--rw-rw-rw-   0        0        0     5084 2022-07-09 15:02:45.000000 sssegmentation-1.2.0/ssseg/modules/datasets/mhp.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/datasets/pipelines/
--rw-rw-rw-   0        0        0      227 2021-09-27 14:46:13.000000 sssegmentation-1.2.0/ssseg/modules/datasets/pipelines/__init__.py
--rw-rw-rw-   0        0        0     4553 2022-07-09 15:04:30.000000 sssegmentation-1.2.0/ssseg/modules/datasets/pipelines/evaluation.py
--rw-rw-rw-   0        0        0    13637 2022-07-09 15:05:26.000000 sssegmentation-1.2.0/ssseg/modules/datasets/pipelines/transforms.py
--rw-rw-rw-   0        0        0     1901 2022-07-09 15:02:59.000000 sssegmentation-1.2.0/ssseg/modules/datasets/sbushadow.py
--rw-rw-rw-   0        0        0     1866 2022-07-09 15:03:12.000000 sssegmentation-1.2.0/ssseg/modules/datasets/stare.py
--rw-rw-rw-   0        0        0     1823 2022-07-09 15:03:30.000000 sssegmentation-1.2.0/ssseg/modules/datasets/supervisely.py
--rw-rw-rw-   0        0        0     6483 2022-07-09 15:03:52.000000 sssegmentation-1.2.0/ssseg/modules/datasets/voc.py
--rw-rw-rw-   0        0        0     4289 2022-07-09 15:04:04.000000 sssegmentation-1.2.0/ssseg/modules/datasets/vspw.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/
--rw-rw-rw-   0        0        0      240 2022-07-28 02:43:58.000000 sssegmentation-1.2.0/ssseg/modules/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/
--rw-rw-rw-   0        0        0      416 2022-07-11 01:06:37.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/__init__.py
--rw-rw-rw-   0        0        0    15983 2022-08-06 12:04:17.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/beit.py
--rw-rw-rw-   0        0        0     9831 2022-08-08 04:33:58.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bisenetv1.py
--rw-rw-rw-   0        0        0    16116 2022-07-11 11:28:24.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bisenetv2.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/
--rw-rw-rw-   0        0        0      526 2022-07-11 01:06:21.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/
--rw-rw-rw-   0        0        0       53 2020-09-11 06:20:32.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/__init__.py
--rw-rw-rw-   0        0        0      716 2022-07-10 10:07:56.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/builder.py
--rw-rw-rw-   0        0        0      626 2022-07-10 10:03:19.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/hardsigmoid.py
--rw-rw-rw-   0        0        0      357 2022-07-10 10:03:05.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/hardswish.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/
--rw-rw-rw-   0        0        0      237 2021-09-24 07:04:28.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/__init__.py
--rw-rw-rw-   0        0        0     1850 2022-07-11 01:27:22.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/apconv.py
--rw-rw-rw-   0        0        0     2047 2022-07-11 01:32:19.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/dsconv.py
--rw-rw-rw-   0        0        0     3752 2022-07-11 01:25:19.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/dyconv.py
--rw-rw-rw-   0        0        0     5135 2022-07-11 01:23:25.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/irconv.py
--rw-rw-rw-   0        0        0     1287 2022-07-10 10:43:29.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/seconv.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/dropout/
--rw-rw-rw-   0        0        0       50 2021-07-01 03:21:00.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/dropout/__init__.py
--rw-rw-rw-   0        0        0      543 2022-07-10 10:47:00.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/dropout/builder.py
--rw-rw-rw-   0        0        0      667 2022-07-10 10:44:42.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/dropout/droppath.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/
--rw-rw-rw-   0        0        0      137 2021-07-01 03:22:52.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/__init__.py
--rw-rw-rw-   0        0        0      629 2022-07-10 10:49:39.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/l2norm.py
--rw-rw-rw-   0        0        0      368 2022-07-10 10:49:47.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/scale.py
--rw-rw-rw-   0        0        0      369 2022-07-10 10:49:27.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/utils.py
--rw-rw-rw-   0        0        0     2144 2022-07-10 10:48:44.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/weightinit.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/normalization/
--rw-rw-rw-   0        0        0       92 2022-07-11 01:06:10.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/normalization/__init__.py
--rw-rw-rw-   0        0        0     1209 2022-07-12 22:47:16.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/normalization/builder.py
--rw-rw-rw-   0        0        0      278 2022-07-11 01:05:57.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/normalization/utils.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/
--rw-rw-rw-   0        0        0      202 2022-07-26 16:19:36.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/__init__.py
--rw-rw-rw-   0        0        0     6053 2022-07-26 16:01:47.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/embed.py
--rw-rw-rw-   0        0        0     1655 2022-07-10 14:54:59.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/ffn.py
--rw-rw-rw-   0        0        0     1625 2022-07-10 14:53:46.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/mha.py
--rw-rw-rw-   0        0        0     1405 2022-07-26 15:43:10.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/misc.py
--rw-rw-rw-   0        0        0     1529 2022-08-06 09:01:18.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/builder.py
--rw-rw-rw-   0        0        0     9098 2022-07-11 12:40:05.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/cgnet.py
--rw-rw-rw-   0        0        0     9772 2022-07-29 16:56:00.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/convnext.py
--rw-rw-rw-   0        0        0     8644 2022-07-11 12:43:42.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/erfnet.py
--rw-rw-rw-   0        0        0    11776 2022-07-11 12:46:32.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/fastscnn.py
--rw-rw-rw-   0        0        0    18116 2022-07-11 13:05:04.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/hrnet.py
--rw-rw-rw-   0        0        0    17083 2022-07-27 03:50:40.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/mit.py
--rw-rw-rw-   0        0        0    13288 2022-07-11 11:37:10.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/mobilenet.py
--rw-rw-rw-   0        0        0     9938 2022-07-11 13:38:49.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/resnest.py
--rw-rw-rw-   0        0        0    12029 2022-07-11 13:14:59.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/resnet.py
--rw-rw-rw-   0        0        0    29073 2022-07-27 01:19:25.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/swin.py
--rw-rw-rw-   0        0        0     1522 2022-07-11 13:07:36.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/timmwrapper.py
--rw-rw-rw-   0        0        0    22192 2022-07-27 04:20:37.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/twins.py
--rw-rw-rw-   0        0        0     9369 2022-07-11 12:50:23.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/unet.py
--rw-rw-rw-   0        0        0    11599 2022-07-27 00:03:36.000000 sssegmentation-1.2.0/ssseg/modules/models/backbones/vit.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/
--rw-rw-rw-   0        0        0       87 2021-09-07 14:18:09.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/__init__.py
--rw-rw-rw-   0        0        0     1349 2022-07-09 23:21:35.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/accuracy.py
--rw-rw-rw-   0        0        0      651 2022-08-04 15:25:07.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/builder.py
--rw-rw-rw-   0        0        0     2752 2022-07-10 09:52:26.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/celoss.py
--rw-rw-rw-   0        0        0     2810 2022-07-10 09:54:35.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/diceloss.py
--rw-rw-rw-   0        0        0     1195 2022-07-10 09:56:08.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/focalloss.py
--rw-rw-rw-   0        0        0     1287 2022-07-10 09:57:15.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/klloss.py
--rw-rw-rw-   0        0        0      806 2022-08-04 15:25:29.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/l1loss.py
--rw-rw-rw-   0        0        0     5547 2022-07-10 10:01:31.000000 sssegmentation-1.2.0/ssseg/modules/models/losses/lovaszloss.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/optimizers/
--rw-rw-rw-   0        0        0       52 2022-07-28 02:40:02.000000 sssegmentation-1.2.0/ssseg/modules/models/optimizers/__init__.py
--rw-rw-rw-   0        0        0     1336 2022-07-29 15:32:13.000000 sssegmentation-1.2.0/ssseg/modules/models/optimizers/builder.py
--rw-rw-rw-   0        0        0     7028 2022-07-29 16:26:28.000000 sssegmentation-1.2.0/ssseg/modules/models/optimizers/paramsconstructor.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/samplers/
--rw-rw-rw-   0        0        0       55 2021-12-16 13:29:56.000000 sssegmentation-1.2.0/ssseg/modules/models/samplers/__init__.py
--rw-rw-rw-   0        0        0      342 2022-07-09 15:08:28.000000 sssegmentation-1.2.0/ssseg/modules/models/samplers/base.py
--rw-rw-rw-   0        0        0      437 2022-07-11 10:19:54.000000 sssegmentation-1.2.0/ssseg/modules/models/samplers/builder.py
--rw-rw-rw-   0        0        0     2287 2022-07-09 15:07:18.000000 sssegmentation-1.2.0/ssseg/modules/models/samplers/ohempixelsampler.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/schedulers/
--rw-rw-rw-   0        0        0       52 2022-07-28 02:43:08.000000 sssegmentation-1.2.0/ssseg/modules/models/schedulers/__init__.py
--rw-rw-rw-   0        0        0     2228 2022-07-28 05:01:17.000000 sssegmentation-1.2.0/ssseg/modules/models/schedulers/basescheduler.py
--rw-rw-rw-   0        0        0      533 2022-07-28 02:52:42.000000 sssegmentation-1.2.0/ssseg/modules/models/schedulers/builder.py
--rw-rw-rw-   0        0        0     2060 2022-07-29 16:40:07.000000 sssegmentation-1.2.0/ssseg/modules/models/schedulers/polyscheduler.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/
--rw-rw-rw-   0        0        0       52 2021-12-19 13:25:13.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/
--rw-rw-rw-   0        0        0      105 2020-12-22 11:21:31.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/__init__.py
--rw-rw-rw-   0        0        0     2063 2022-07-11 04:44:09.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/afnblock.py
--rw-rw-rw-   0        0        0     3527 2022-08-08 11:59:26.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/annnet.py
--rw-rw-rw-   0        0        0     2044 2022-07-11 04:44:30.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/apnblock.py
--rw-rw-rw-   0        0        0      706 2022-07-11 00:57:06.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/ppm.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/
--rw-rw-rw-   0        0        0       82 2020-12-18 08:28:07.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/__init__.py
--rw-rw-rw-   0        0        0     3036 2022-07-11 05:39:31.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/acm.py
--rw-rw-rw-   0        0        0     2921 2022-08-08 12:00:47.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/apcnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/
--rw-rw-rw-   0        0        0      160 2022-08-06 09:13:47.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/__init__.py
--rw-rw-rw-   0        0        0    10172 2022-08-08 13:28:41.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/base.py
--rw-rw-rw-   0        0        0     1907 2022-08-06 09:11:32.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/feature2pyramid.py
--rw-rw-rw-   0        0        0     2078 2022-07-13 03:27:16.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/fpn.py
--rw-rw-rw-   0        0        0     4779 2022-08-03 23:24:36.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/selfattention.py
--rw-rw-rw-   0        0        0     2140 2022-07-11 10:24:45.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/builder.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ccnet/
--rw-rw-rw-   0        0        0       41 2020-12-13 04:15:10.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ccnet/__init__.py
--rw-rw-rw-   0        0        0     3193 2022-08-08 12:02:22.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ccnet/ccnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/
--rw-rw-rw-   0        0        0       77 2020-10-16 11:50:21.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/__init__.py
--rw-rw-rw-   0        0        0     5585 2022-08-08 12:04:09.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/ce2p.py
--rw-rw-rw-   0        0        0     1957 2022-07-11 05:56:20.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/epm.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/
--rw-rw-rw-   0        0        0      122 2021-01-05 08:01:13.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/__init__.py
--rw-rw-rw-   0        0        0     1040 2022-07-11 05:58:51.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/cam.py
--rw-rw-rw-   0        0        0     5071 2022-08-08 12:05:48.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/danet.py
--rw-rw-rw-   0        0        0     1137 2022-07-11 05:58:37.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/pam.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/
--rw-rw-rw-   0        0        0       72 2020-12-10 06:03:24.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/__init__.py
--rw-rw-rw-   0        0        0     2562 2022-07-11 06:10:02.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/aspp.py
--rw-rw-rw-   0        0        0     2223 2022-08-08 12:08:02.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/deeplabv3.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/
--rw-rw-rw-   0        0        0       98 2020-12-10 06:00:46.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/__init__.py
--rw-rw-rw-   0        0        0     2514 2022-07-11 06:16:45.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/aspp.py
--rw-rw-rw-   0        0        0     3440 2022-08-08 12:08:35.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/deeplabv3plus.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/
--rw-rw-rw-   0        0        0       85 2020-12-24 12:41:18.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/__init__.py
--rw-rw-rw-   0        0        0     2267 2022-07-11 06:20:43.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/dcm.py
--rw-rw-rw-   0        0        0     2832 2022-08-08 12:09:06.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/dmnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/
--rw-rw-rw-   0        0        0       88 2020-12-15 07:32:39.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/__init__.py
--rw-rw-rw-   0        0        0     2359 2022-07-11 06:26:03.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/dnlblock.py
--rw-rw-rw-   0        0        0     3503 2022-08-08 12:10:23.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/dnlnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/
--rw-rw-rw-   0        0        0       70 2020-12-19 14:10:17.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/__init__.py
--rw-rw-rw-   0        0        0     2099 2022-07-11 06:30:28.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/ema.py
--rw-rw-rw-   0        0        0     4040 2022-08-08 12:11:36.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/emanet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/
--rw-rw-rw-   0        0        0      119 2021-01-06 01:24:55.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/__init__.py
--rw-rw-rw-   0        0        0     1629 2022-07-11 06:37:05.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/contextencoding.py
--rw-rw-rw-   0        0        0     4774 2022-08-08 12:17:07.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/encnet.py
--rw-rw-rw-   0        0        0     2305 2022-07-11 06:33:13.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/encoding.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/
--rw-rw-rw-   0        0        0       66 2021-10-04 15:17:39.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/__init__.py
--rw-rw-rw-   0        0        0     2228 2022-08-08 13:19:27.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/fastfcn.py
--rw-rw-rw-   0        0        0     2966 2022-07-11 06:42:55.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/jpu.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fcn/
--rw-rw-rw-   0        0        0       60 2021-09-24 01:32:56.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fcn/__init__.py
--rw-rw-rw-   0        0        0     5273 2022-08-08 12:19:55.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/fcn/fcn.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/
--rw-rw-rw-   0        0        0       80 2020-12-15 06:54:42.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/__init__.py
--rw-rw-rw-   0        0        0     3516 2022-07-11 06:49:01.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/contextblock.py
--rw-rw-rw-   0        0        0     3484 2022-08-08 12:20:43.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/gcnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/
--rw-rw-rw-   0        0        0      107 2021-10-04 10:32:58.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/__init__.py
--rw-rw-rw-   0        0        0     2794 2022-07-11 06:56:36.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icneck.py
--rw-rw-rw-   0        0        0     3028 2022-08-08 12:21:24.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icnet.py
--rw-rw-rw-   0        0        0     3556 2022-07-11 06:58:48.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icnetencoder.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isanet/
--rw-rw-rw-   0        0        0       43 2021-09-10 01:20:54.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isanet/__init__.py
--rw-rw-rw-   0        0        0     5933 2022-08-08 12:22:33.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isanet/isanet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/
--rw-rw-rw-   0        0        0      131 2021-03-07 06:56:44.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/__init__.py
--rw-rw-rw-   0        0        0     1966 2022-07-11 07:45:27.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/imagelevel.py
--rw-rw-rw-   0        0        0     5951 2022-08-08 12:24:11.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/isnet.py
--rw-rw-rw-   0        0        0     2946 2022-07-11 07:46:22.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/semanticlevel.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/lrasppnet/
--rw-rw-rw-   0        0        0       49 2021-01-04 12:46:24.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/lrasppnet/__init__.py
--rw-rw-rw-   0        0        0     4084 2022-08-08 12:26:07.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/lrasppnet/lrasppnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/
--rw-rw-rw-   0        0        0       51 2021-12-09 16:49:30.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/__init__.py
--rw-rw-rw-   0        0        0     6530 2022-08-08 12:27:46.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/maskformer.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/
--rw-rw-rw-   0        0        0      160 2021-12-09 16:28:36.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/__init__.py
--rw-rw-rw-   0        0        0     8869 2021-12-10 05:53:09.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/criterion.py
--rw-rw-rw-   0        0        0     2949 2021-12-09 15:33:52.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/matcher.py
--rw-rw-rw-   0        0        0     5420 2022-07-11 07:54:15.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/predictor.py
--rw-rw-rw-   0        0        0     9708 2022-07-11 07:57:33.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/transformer.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/
--rw-rw-rw-   0        0        0       84 2021-12-24 17:02:01.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/__init__.py
--rw-rw-rw-   0        0        0     4889 2022-07-11 07:58:01.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/initmemory.py
--rw-rw-rw-   0        0        0    10621 2022-07-11 08:03:22.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/memory.py
--rw-rw-rw-   0        0        0     8719 2022-08-08 12:54:43.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/memorynet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/
--rw-rw-rw-   0        0        0      115 2020-12-15 07:03:33.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/__init__.py
--rw-rw-rw-   0        0        0     5697 2022-07-11 08:09:48.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalblock.py
--rw-rw-rw-   0        0        0     3420 2022-08-08 12:42:55.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/
--rw-rw-rw-   0        0        0      136 2020-12-22 12:45:57.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/__init__.py
--rw-rw-rw-   0        0        0     1968 2022-07-11 08:13:47.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/objectcontext.py
--rw-rw-rw-   0        0        0     3534 2022-08-08 12:43:38.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/ocrnet.py
--rw-rw-rw-   0        0        0      817 2022-07-11 08:12:20.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/spatialgather.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pointrend/
--rw-rw-rw-   0        0        0       49 2021-09-11 03:32:57.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pointrend/__init__.py
--rw-rw-rw-   0        0        0    10191 2022-08-08 12:35:03.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pointrend/pointrend.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/psanet/
--rw-rw-rw-   0        0        0       43 2020-12-24 12:59:31.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/psanet/__init__.py
--rw-rw-rw-   0        0        0     7943 2022-08-08 12:36:39.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/psanet/psanet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/
--rw-rw-rw-   0        0        0       81 2020-10-16 11:51:21.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/__init__.py
--rw-rw-rw-   0        0        0     1751 2022-07-11 08:38:19.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/ppm.py
--rw-rw-rw-   0        0        0     2271 2022-08-08 12:37:02.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/pspnet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/segformer/
--rw-rw-rw-   0        0        0       49 2021-08-15 16:21:35.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/segformer/__init__.py
--rw-rw-rw-   0        0        0     2732 2022-08-08 12:37:55.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/segformer/segformer.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/semanticfpn/
--rw-rw-rw-   0        0        0       53 2021-01-16 13:20:19.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/semanticfpn/__init__.py
--rw-rw-rw-   0        0        0     3439 2022-08-08 12:38:27.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/semanticfpn/semanticfpn.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/
--rw-rw-rw-   0        0        0       92 2021-07-27 02:25:47.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/__init__.py
--rw-rw-rw-   0        0        0     2892 2022-07-11 08:25:00.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/mla.py
--rw-rw-rw-   0        0        0    10242 2022-08-08 12:40:50.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/setr.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/upernet/
--rw-rw-rw-   0        0        0       45 2020-12-05 08:16:00.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/upernet/__init__.py
--rw-rw-rw-   0        0        0     5099 2022-08-08 12:42:10.000000 sssegmentation-1.2.0/ssseg/modules/models/segmentors/upernet/upernet.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/parallel/
--rw-rw-rw-   0        0        0      108 2022-07-09 14:50:39.000000 sssegmentation-1.2.0/ssseg/modules/parallel/__init__.py
--rw-rw-rw-   0        0        0      675 2022-07-11 14:42:33.000000 sssegmentation-1.2.0/ssseg/modules/parallel/dataloader.py
--rw-rw-rw-   0        0        0      247 2022-07-11 14:42:51.000000 sssegmentation-1.2.0/ssseg/modules/parallel/model.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/ssseg/modules/utils/
--rw-rw-rw-   0        0        0      197 2022-07-14 09:25:32.000000 sssegmentation-1.2.0/ssseg/modules/utils/__init__.py
--rw-rw-rw-   0        0        0     1115 2022-08-08 11:22:54.000000 sssegmentation-1.2.0/ssseg/modules/utils/io.py
--rw-rw-rw-   0        0        0      934 2022-07-09 14:52:27.000000 sssegmentation-1.2.0/ssseg/modules/utils/logger.py
--rw-rw-rw-   0        0        0      269 2022-07-09 14:34:59.000000 sssegmentation-1.2.0/ssseg/modules/utils/misc.py
--rw-rw-rw-   0        0        0     7534 2022-07-09 14:34:30.000000 sssegmentation-1.2.0/ssseg/modules/utils/palette.py
--rw-rw-rw-   0        0        0      907 2022-07-18 23:51:54.000000 sssegmentation-1.2.0/ssseg/modules/utils/slurm.py
--rw-rw-rw-   0        0        0    15099 2022-08-10 06:31:24.000000 sssegmentation-1.2.0/ssseg/test.py
--rw-rw-rw-   0        0        0    16603 2022-08-10 06:31:18.000000 sssegmentation-1.2.0/ssseg/train.py
-drwxrwxrwx   0        0        0        0 2022-08-10 09:00:49.000000 sssegmentation-1.2.0/sssegmentation.egg-info/
--rw-rw-rw-   0        0        0     7045 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9667 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-08-10 09:00:48.000000 sssegmentation-1.2.0/sssegmentation.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-25 11:57:53.000000 SSSegmentation-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0    23995 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    23389 2023-06-01 05:53:40.000000 SSSegmentation-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/
+-rw-rw-rw-   0        0        0    23995 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11142 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 05:55:22.000000 SSSegmentation-1.3.0/SSSegmentation.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     3314 2023-05-25 15:36:41.000000 SSSegmentation-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/
+-rw-rw-rw-   0        0        0      496 2023-05-25 11:56:56.000000 SSSegmentation-1.3.0/ssseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/configs/
+-rw-rw-rw-   0        0        0       49 2020-11-19 13:11:51.000000 SSSegmentation-1.3.0/ssseg/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/
+-rw-rw-rw-   0        0        0      685 2023-05-24 15:36:16.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/
+-rw-rw-rw-   0        0        0      246 2023-05-24 11:23:35.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/__init__.py
+-rw-rw-rw-   0        0        0      426 2023-05-25 12:29:03.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/default_dataloader_bs16.py
+-rw-rw-rw-   0        0        0      426 2023-05-25 12:29:07.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/default_dataloader_bs32.py
+-rw-rw-rw-   0        0        0      426 2023-05-25 12:29:11.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/default_dataloader_bs40.py
+-rw-rw-rw-   0        0        0      422 2023-05-25 12:28:56.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/dataloaders/default_dataloader_bs8.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/
+-rw-rw-rw-   0        0        0     1012 2023-05-24 15:36:00.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-05-22 15:44:57.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/ade20k_512x512.py
+-rw-rw-rw-   0        0        0     1076 2023-05-22 15:44:27.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/ade20k_640x640.py
+-rw-rw-rw-   0        0        0     1232 2023-05-25 14:11:51.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/atr_473x473.py
+-rw-rw-rw-   0        0        0     1117 2023-05-24 06:27:00.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/chasedb1_128x128.py
+-rw-rw-rw-   0        0        0     1237 2023-05-25 14:11:45.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/cihp_473x473.py
+-rw-rw-rw-   0        0        0     1108 2023-05-24 08:10:47.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/cityscapes_1024x1024.py
+-rw-rw-rw-   0        0        0     1103 2023-05-22 15:57:15.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/cityscapes_512x1024.py
+-rw-rw-rw-   0        0        0     1098 2023-05-24 09:53:54.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/cityscapes_832x832.py
+-rw-rw-rw-   0        0        0     1107 2023-05-24 10:07:34.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/cocostuff10k_512x512.py
+-rw-rw-rw-   0        0        0     1091 2023-05-24 06:34:32.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/drive_64x64.py
+-rw-rw-rw-   0        0        0     1095 2023-05-24 06:35:11.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/hrf_256x256.py
+-rw-rw-rw-   0        0        0     1232 2023-05-25 14:11:36.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/lip_473x473.py
+-rw-rw-rw-   0        0        0     1122 2023-05-24 03:05:01.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/pascalcontext59_480x480.py
+-rw-rw-rw-   0        0        0     1114 2023-05-24 03:08:45.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/pascalcontext_480x480.py
+-rw-rw-rw-   0        0        0     1101 2023-05-24 06:29:23.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/stare_128x128.py
+-rw-rw-rw-   0        0        0     1087 2023-05-22 15:53:05.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/vocaug_512x512.py
+-rw-rw-rw-   0        0        0     1071 2023-05-24 15:35:22.000000 SSSegmentation-1.3.0/ssseg/configs/_base_/datasets/vspw_512x512.py
+-rw-rw-rw-   0        0        0     2059 2023-05-25 16:43:58.000000 SSSegmentation-1.3.0/ssseg/configs/builder.py
+-rw-rw-rw-   0        0        0    10595 2023-05-29 00:45:14.000000 SSSegmentation-1.3.0/ssseg/inference.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/
+-rw-rw-rw-   0        0        0      351 2023-05-22 16:31:08.000000 SSSegmentation-1.3.0/ssseg/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/
+-rw-rw-rw-   0        0        0       50 2020-11-19 13:15:40.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/__init__.py
+-rw-rw-rw-   0        0        0     7187 2023-05-03 14:22:28.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/ade20k.py
+-rw-rw-rw-   0        0        0     1162 2023-05-03 14:28:58.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/atr.py
+-rw-rw-rw-   0        0        0     6069 2023-05-31 14:22:00.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/base.py
+-rw-rw-rw-   0        0        0     2197 2023-05-04 09:01:53.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/builder.py
+-rw-rw-rw-   0        0        0     1806 2023-05-31 13:31:11.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/chasedb1.py
+-rw-rw-rw-   0        0        0     1649 2023-05-03 15:26:58.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/cihp.py
+-rw-rw-rw-   0        0        0     3817 2023-05-03 15:44:21.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0    10560 2023-05-03 18:18:17.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/coco.py
+-rw-rw-rw-   0        0        0     1697 2023-05-03 16:17:43.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/darkzurich.py
+-rw-rw-rw-   0        0        0     1795 2023-05-31 09:28:09.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/drive.py
+-rw-rw-rw-   0        0        0     1124 2023-05-03 16:31:10.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/hrf.py
+-rw-rw-rw-   0        0        0     1594 2023-05-03 17:12:37.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/lip.py
+-rw-rw-rw-   0        0        0     4735 2023-05-25 16:17:49.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/mhp.py
+-rw-rw-rw-   0        0        0     1641 2023-05-03 17:17:11.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/nighttimedriving.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/pipelines/
+-rw-rw-rw-   0        0        0      211 2023-04-30 19:23:59.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     4546 2023-05-03 13:05:54.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/pipelines/evaluation.py
+-rw-rw-rw-   0        0        0    16893 2023-05-25 17:45:35.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/pipelines/transforms.py
+-rw-rw-rw-   0        0        0     1758 2023-05-03 17:25:20.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/sbushadow.py
+-rw-rw-rw-   0        0        0     1790 2023-05-31 09:39:54.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/stare.py
+-rw-rw-rw-   0        0        0     1636 2023-05-03 17:28:56.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/supervisely.py
+-rw-rw-rw-   0        0        0     6594 2023-05-03 18:02:05.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/voc.py
+-rw-rw-rw-   0        0        0     4094 2023-05-03 17:44:47.000000 SSSegmentation-1.3.0/ssseg/modules/datasets/vspw.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/
+-rw-rw-rw-   0        0        0      240 2022-07-28 02:43:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/
+-rw-rw-rw-   0        0        0      398 2023-05-25 16:19:30.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/__init__.py
+-rw-rw-rw-   0        0        0    15288 2023-05-04 15:48:15.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/beit.py
+-rw-rw-rw-   0        0        0     9603 2023-05-29 13:30:43.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bisenetv1.py
+-rw-rw-rw-   0        0        0    15413 2023-05-04 15:48:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bisenetv2.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/
+-rw-rw-rw-   0        0        0      508 2023-05-04 11:55:11.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/
+-rw-rw-rw-   0        0        0       53 2020-09-11 06:20:32.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-04 11:49:30.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/builder.py
+-rw-rw-rw-   0        0        0      625 2023-04-26 17:53:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/hardsigmoid.py
+-rw-rw-rw-   0        0        0      356 2023-04-26 17:54:06.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/hardswish.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/
+-rw-rw-rw-   0        0        0      237 2021-09-24 07:04:28.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-05-04 11:56:38.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/apconv.py
+-rw-rw-rw-   0        0        0     1990 2023-05-04 12:01:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/dsconv.py
+-rw-rw-rw-   0        0        0     3722 2023-05-04 12:02:01.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/dyconv.py
+-rw-rw-rw-   0        0        0     5018 2023-05-04 12:00:00.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/irconv.py
+-rw-rw-rw-   0        0        0     1288 2023-04-26 17:55:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/seconv.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/dropout/
+-rw-rw-rw-   0        0        0       50 2021-07-01 03:21:00.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/dropout/__init__.py
+-rw-rw-rw-   0        0        0      647 2023-05-04 11:49:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/dropout/builder.py
+-rw-rw-rw-   0        0        0      677 2023-04-26 17:56:14.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/dropout/droppath.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/
+-rw-rw-rw-   0        0        0      137 2021-07-01 03:22:52.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/__init__.py
+-rw-rw-rw-   0        0        0      636 2023-04-26 17:56:35.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/l2norm.py
+-rw-rw-rw-   0        0        0      364 2023-04-26 17:56:42.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/scale.py
+-rw-rw-rw-   0        0        0      380 2023-04-26 17:56:52.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/utils.py
+-rw-rw-rw-   0        0        0     2167 2023-04-26 17:57:17.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/weightinit.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/normalization/
+-rw-rw-rw-   0        0        0       56 2023-05-04 11:50:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/normalization/__init__.py
+-rw-rw-rw-   0        0        0      940 2023-05-25 02:14:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/normalization/builder.py
+-rw-rw-rw-   0        0        0      719 2023-05-30 01:27:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/normalization/layernorm2d.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/
+-rw-rw-rw-   0        0        0      202 2022-07-26 16:19:36.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/__init__.py
+-rw-rw-rw-   0        0        0     6035 2023-05-04 12:02:52.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/embed.py
+-rw-rw-rw-   0        0        0     1616 2023-04-26 17:58:47.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/ffn.py
+-rw-rw-rw-   0        0        0     1634 2023-04-26 17:58:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/mha.py
+-rw-rw-rw-   0        0        0     1412 2023-04-26 17:58:37.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/misc.py
+-rw-rw-rw-   0        0        0     1520 2023-05-25 16:23:10.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/builder.py
+-rw-rw-rw-   0        0        0     8791 2023-05-04 15:50:06.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/cgnet.py
+-rw-rw-rw-   0        0        0     8286 2023-05-25 02:16:22.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/convnext.py
+-rw-rw-rw-   0        0        0     8109 2023-05-04 15:51:26.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/erfnet.py
+-rw-rw-rw-   0        0        0    11252 2023-05-04 15:46:32.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/fastscnn.py
+-rw-rw-rw-   0        0        0    17963 2023-05-04 16:02:22.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/hrnet.py
+-rw-rw-rw-   0        0        0    16773 2023-05-04 16:09:36.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/mit.py
+-rw-rw-rw-   0        0        0    14484 2023-05-04 17:14:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/mobilenet.py
+-rw-rw-rw-   0        0        0     9800 2023-05-25 08:38:30.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/resnest.py
+-rw-rw-rw-   0        0        0    11562 2023-05-25 07:01:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/resnet.py
+-rw-rw-rw-   0        0        0    29214 2023-05-29 00:32:52.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/swin.py
+-rw-rw-rw-   0        0        0      996 2023-05-04 16:23:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/timmwrapper.py
+-rw-rw-rw-   0        0        0    21435 2023-05-31 13:44:33.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/twins.py
+-rw-rw-rw-   0        0        0     9243 2023-05-04 17:05:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/unet.py
+-rw-rw-rw-   0        0        0    11631 2023-05-31 08:19:36.000000 SSSegmentation-1.3.0/ssseg/modules/models/backbones/vit.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/
+-rw-rw-rw-   0        0        0       87 2021-09-07 14:18:09.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-04-26 17:44:54.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/accuracy.py
+-rw-rw-rw-   0        0        0      931 2023-05-04 12:43:20.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/builder.py
+-rw-rw-rw-   0        0        0     3593 2023-05-04 13:00:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/celoss.py
+-rw-rw-rw-   0        0        0     1138 2023-05-04 13:11:54.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/cosinesimilarityloss.py
+-rw-rw-rw-   0        0        0     3261 2023-05-04 13:38:11.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/diceloss.py
+-rw-rw-rw-   0        0        0     1604 2023-05-04 13:20:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/focalloss.py
+-rw-rw-rw-   0        0        0     1395 2023-05-04 13:29:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/klloss.py
+-rw-rw-rw-   0        0        0      907 2023-05-04 13:10:31.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/l1loss.py
+-rw-rw-rw-   0        0        0     6027 2023-05-25 00:47:27.000000 SSSegmentation-1.3.0/ssseg/modules/models/losses/lovaszloss.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/optimizers/
+-rw-rw-rw-   0        0        0       52 2022-07-28 02:40:02.000000 SSSegmentation-1.3.0/ssseg/modules/models/optimizers/__init__.py
+-rw-rw-rw-   0        0        0     1350 2023-05-04 12:35:03.000000 SSSegmentation-1.3.0/ssseg/modules/models/optimizers/builder.py
+-rw-rw-rw-   0        0        0     7041 2023-04-26 17:36:40.000000 SSSegmentation-1.3.0/ssseg/modules/models/optimizers/paramsconstructor.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:23.000000 SSSegmentation-1.3.0/ssseg/modules/models/samplers/
+-rw-rw-rw-   0        0        0       55 2021-12-16 13:29:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/samplers/__init__.py
+-rw-rw-rw-   0        0        0      358 2023-04-26 17:35:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/samplers/base.py
+-rw-rw-rw-   0        0        0      509 2023-05-04 12:36:50.000000 SSSegmentation-1.3.0/ssseg/modules/models/samplers/builder.py
+-rw-rw-rw-   0        0        0     2303 2023-04-26 17:35:42.000000 SSSegmentation-1.3.0/ssseg/modules/models/samplers/ohempixelsampler.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/schedulers/
+-rw-rw-rw-   0        0        0       52 2022-07-28 02:43:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/schedulers/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-04-26 17:34:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/schedulers/basescheduler.py
+-rw-rw-rw-   0        0        0      579 2023-05-25 17:11:01.000000 SSSegmentation-1.3.0/ssseg/modules/models/schedulers/builder.py
+-rw-rw-rw-   0        0        0     2067 2023-04-26 17:35:17.000000 SSSegmentation-1.3.0/ssseg/modules/models/schedulers/polyscheduler.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/
+-rw-rw-rw-   0        0        0       52 2021-12-19 13:25:13.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/
+-rw-rw-rw-   0        0        0      105 2020-12-22 11:21:31.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/__init__.py
+-rw-rw-rw-   0        0        0     2027 2023-05-25 11:14:13.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/afnblock.py
+-rw-rw-rw-   0        0        0     3482 2023-05-25 14:35:04.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/annnet.py
+-rw-rw-rw-   0        0        0     2008 2023-05-25 11:24:41.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/apnblock.py
+-rw-rw-rw-   0        0        0      706 2022-07-11 00:57:06.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/ppm.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/
+-rw-rw-rw-   0        0        0       82 2020-12-18 08:28:07.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/__init__.py
+-rw-rw-rw-   0        0        0     2928 2023-05-25 11:25:41.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/acm.py
+-rw-rw-rw-   0        0        0     2876 2023-05-25 14:35:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/apcnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/
+-rw-rw-rw-   0        0        0      160 2022-08-06 09:13:47.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/__init__.py
+-rw-rw-rw-   0        0        0    10291 2023-05-25 16:47:11.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/base.py
+-rw-rw-rw-   0        0        0     1871 2023-05-25 11:26:37.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/feature2pyramid.py
+-rw-rw-rw-   0        0        0     2024 2023-05-25 11:27:04.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/fpn.py
+-rw-rw-rw-   0        0        0     4725 2023-05-25 11:27:26.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/selfattention.py
+-rw-rw-rw-   0        0        0     2071 2023-05-25 11:00:00.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/builder.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ccnet/
+-rw-rw-rw-   0        0        0       41 2020-12-13 04:15:10.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ccnet/__init__.py
+-rw-rw-rw-   0        0        0     3160 2023-05-25 16:58:44.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ccnet/ccnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/
+-rw-rw-rw-   0        0        0       77 2020-10-16 11:50:21.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/__init__.py
+-rw-rw-rw-   0        0        0     5469 2023-05-25 14:36:35.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/ce2p.py
+-rw-rw-rw-   0        0        0     1921 2023-05-25 11:28:20.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/epm.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/
+-rw-rw-rw-   0        0        0      122 2021-01-05 08:01:13.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/__init__.py
+-rw-rw-rw-   0        0        0     1040 2022-07-11 05:58:51.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/cam.py
+-rw-rw-rw-   0        0        0     4980 2023-05-25 14:37:29.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/danet.py
+-rw-rw-rw-   0        0        0     1137 2022-07-11 05:58:37.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/pam.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/
+-rw-rw-rw-   0        0        0       72 2020-12-10 06:03:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-05-25 11:30:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/aspp.py
+-rw-rw-rw-   0        0        0     2214 2023-05-25 14:37:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/deeplabv3.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/
+-rw-rw-rw-   0        0        0       98 2020-12-10 06:00:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-05-25 11:31:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/aspp.py
+-rw-rw-rw-   0        0        0     3395 2023-05-25 14:38:12.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/deeplabv3plus.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/
+-rw-rw-rw-   0        0        0       85 2020-12-24 12:41:18.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/__init__.py
+-rw-rw-rw-   0        0        0     2195 2023-05-25 11:32:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/dcm.py
+-rw-rw-rw-   0        0        0     2787 2023-05-25 14:38:27.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/dmnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/
+-rw-rw-rw-   0        0        0       88 2020-12-15 07:32:39.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/__init__.py
+-rw-rw-rw-   0        0        0     2359 2022-07-11 06:26:03.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/dnlblock.py
+-rw-rw-rw-   0        0        0     3422 2023-05-25 14:38:42.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/dnlnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/
+-rw-rw-rw-   0        0        0       70 2020-12-19 14:10:17.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/__init__.py
+-rw-rw-rw-   0        0        0     2099 2022-07-11 06:30:28.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/ema.py
+-rw-rw-rw-   0        0        0     3941 2023-05-25 14:38:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/emanet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/
+-rw-rw-rw-   0        0        0      119 2021-01-06 01:24:55.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/__init__.py
+-rw-rw-rw-   0        0        0     1575 2023-05-25 11:39:05.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/contextencoding.py
+-rw-rw-rw-   0        0        0     4701 2023-05-25 14:39:19.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/encnet.py
+-rw-rw-rw-   0        0        0     2305 2022-07-11 06:33:13.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/encoding.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/
+-rw-rw-rw-   0        0        0       66 2021-10-04 15:17:39.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/__init__.py
+-rw-rw-rw-   0        0        0     2199 2023-05-25 14:39:35.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/fastfcn.py
+-rw-rw-rw-   0        0        0     2930 2023-05-25 11:39:35.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/jpu.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fcn/
+-rw-rw-rw-   0        0        0       60 2021-09-24 01:32:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fcn/__init__.py
+-rw-rw-rw-   0        0        0     5219 2023-05-25 14:40:01.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fcn/fcn.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/
+-rw-rw-rw-   0        0        0       80 2020-12-15 06:54:42.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/__init__.py
+-rw-rw-rw-   0        0        0     3462 2023-05-25 11:40:51.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/contextblock.py
+-rw-rw-rw-   0        0        0     3403 2023-05-25 14:40:21.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/gcnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/
+-rw-rw-rw-   0        0        0      107 2021-10-04 10:32:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-05-25 11:41:21.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icneck.py
+-rw-rw-rw-   0        0        0     2983 2023-05-25 14:40:34.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icnet.py
+-rw-rw-rw-   0        0        0     3448 2023-05-25 11:42:19.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icnetencoder.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isanet/
+-rw-rw-rw-   0        0        0       43 2021-09-10 01:20:54.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isanet/__init__.py
+-rw-rw-rw-   0        0        0     5870 2023-05-25 15:08:46.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isanet/isanet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/
+-rw-rw-rw-   0        0        0      131 2021-03-07 06:56:44.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/__init__.py
+-rw-rw-rw-   0        0        0     1930 2023-05-25 11:43:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/imagelevel.py
+-rw-rw-rw-   0        0        0     5860 2023-05-25 15:09:06.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/isnet.py
+-rw-rw-rw-   0        0        0     2910 2023-05-25 11:44:06.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/semanticlevel.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/lrasppnet/
+-rw-rw-rw-   0        0        0       49 2021-01-04 12:46:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/lrasppnet/__init__.py
+-rw-rw-rw-   0        0        0     4003 2023-05-25 15:09:28.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/lrasppnet/lrasppnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/
+-rw-rw-rw-   0        0        0       51 2021-12-09 16:49:30.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/__init__.py
+-rw-rw-rw-   0        0        0     6459 2023-05-25 15:09:41.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/maskformer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/
+-rw-rw-rw-   0        0        0      160 2021-12-09 16:28:36.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/__init__.py
+-rw-rw-rw-   0        0        0     8869 2021-12-10 05:53:09.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/criterion.py
+-rw-rw-rw-   0        0        0     2949 2021-12-09 15:33:52.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/matcher.py
+-rw-rw-rw-   0        0        0     5420 2022-07-11 07:54:15.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/predictor.py
+-rw-rw-rw-   0        0        0     9564 2023-05-25 11:46:05.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/transformer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/
+-rw-rw-rw-   0        0        0       84 2021-12-24 17:02:01.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/__init__.py
+-rw-rw-rw-   0        0        0     4889 2022-07-11 07:58:01.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/initmemory.py
+-rw-rw-rw-   0        0        0    10549 2023-05-25 11:46:56.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/memory.py
+-rw-rw-rw-   0        0        0     8608 2023-05-25 15:33:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/memorynet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynetv2/
+-rw-rw-rw-   0        0        0       92 2022-08-13 15:05:02.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynetv2/__init__.py
+-rw-rw-rw-   0        0        0    11431 2023-05-25 15:33:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynetv2/memorynetv2.py
+-rw-rw-rw-   0        0        0     6135 2023-05-25 11:48:49.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynetv2/memoryv2.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/
+-rw-rw-rw-   0        0        0      115 2020-12-15 07:03:33.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/__init__.py
+-rw-rw-rw-   0        0        0     5661 2023-05-25 11:50:16.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalblock.py
+-rw-rw-rw-   0        0        0     3339 2023-05-25 15:11:22.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/
+-rw-rw-rw-   0        0        0      136 2020-12-22 12:45:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/__init__.py
+-rw-rw-rw-   0        0        0     1932 2023-05-25 11:50:38.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/objectcontext.py
+-rw-rw-rw-   0        0        0     3489 2023-05-25 15:11:37.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/ocrnet.py
+-rw-rw-rw-   0        0        0      817 2022-07-11 08:12:20.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/spatialgather.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pointrend/
+-rw-rw-rw-   0        0        0       49 2021-09-11 03:32:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pointrend/__init__.py
+-rw-rw-rw-   0        0        0    10164 2023-05-25 16:59:30.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pointrend/pointrend.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/psanet/
+-rw-rw-rw-   0        0        0       43 2020-12-24 12:59:31.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/psanet/__init__.py
+-rw-rw-rw-   0        0        0     7844 2023-05-25 16:59:08.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/psanet/psanet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/
+-rw-rw-rw-   0        0        0       81 2020-10-16 11:51:21.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/__init__.py
+-rw-rw-rw-   0        0        0     1697 2023-05-25 11:52:33.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/ppm.py
+-rw-rw-rw-   0        0        0     2262 2023-05-25 15:12:27.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/pspnet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/segformer/
+-rw-rw-rw-   0        0        0       49 2021-08-15 16:21:35.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/segformer/__init__.py
+-rw-rw-rw-   0        0        0     2669 2023-05-25 15:12:42.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/segformer/segformer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/semanticfpn/
+-rw-rw-rw-   0        0        0       53 2021-01-16 13:20:19.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/semanticfpn/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-05-25 15:12:57.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/semanticfpn/semanticfpn.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/
+-rw-rw-rw-   0        0        0       92 2021-07-27 02:25:47.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/__init__.py
+-rw-rw-rw-   0        0        0     2838 2023-05-25 11:54:58.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/mla.py
+-rw-rw-rw-   0        0        0    10098 2023-05-25 15:13:26.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/setr.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/upernet/
+-rw-rw-rw-   0        0        0       45 2020-12-05 08:16:00.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/upernet/__init__.py
+-rw-rw-rw-   0        0        0     5018 2023-05-25 15:13:40.000000 SSSegmentation-1.3.0/ssseg/modules/models/segmentors/upernet/upernet.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/parallel/
+-rw-rw-rw-   0        0        0      108 2022-07-09 14:50:39.000000 SSSegmentation-1.3.0/ssseg/modules/parallel/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-05-22 16:06:01.000000 SSSegmentation-1.3.0/ssseg/modules/parallel/dataloader.py
+-rw-rw-rw-   0        0        0      263 2023-04-26 17:31:53.000000 SSSegmentation-1.3.0/ssseg/modules/parallel/model.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:55:24.000000 SSSegmentation-1.3.0/ssseg/modules/utils/
+-rw-rw-rw-   0        0        0      151 2023-05-04 08:56:46.000000 SSSegmentation-1.3.0/ssseg/modules/utils/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-05-04 08:56:14.000000 SSSegmentation-1.3.0/ssseg/modules/utils/io.py
+-rw-rw-rw-   0        0        0      931 2023-04-26 17:32:34.000000 SSSegmentation-1.3.0/ssseg/modules/utils/logger.py
+-rw-rw-rw-   0        0        0      275 2023-05-04 08:52:39.000000 SSSegmentation-1.3.0/ssseg/modules/utils/misc.py
+-rw-rw-rw-   0        0        0      909 2023-04-26 17:33:55.000000 SSSegmentation-1.3.0/ssseg/modules/utils/slurm.py
+-rw-rw-rw-   0        0        0    15144 2023-05-29 00:39:15.000000 SSSegmentation-1.3.0/ssseg/test.py
+-rw-rw-rw-   0        0        0    17023 2023-05-31 16:27:49.000000 SSSegmentation-1.3.0/ssseg/train.py
```

### Comparing `sssegmentation-1.2.0/LICENSE` & `SSSegmentation-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
```

### Comparing `sssegmentation-1.2.0/setup.py` & `SSSegmentation-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 '''
 Function:
     Setup sssegmentation
 Author:
     Zhenchao Jin
 '''
+import os
+import re
+import sys
 import ssseg
 from setuptools import setup, find_packages
 
 
 '''readme'''
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 '''parse the package dependencies listed in a requirements file but strips specific versioning information'''
 def parserequirements(fname='requirements.txt', with_version=True):
-    import re
-    import sys
-    from os.path import exists
     require_fpath = fname
     '''parse information from a line in a requirements text file'''
     def parseline(line):
         if line.startswith('-r '):
             target = line.split(' ')[1]
             for info in parserequirefile(target):
                 yield info
@@ -51,15 +51,15 @@
             for line in f.readlines():
                 line = line.strip()
                 if line and not line.startswith('#'):
                     for info in parseline(line):
                         yield info
     '''gen packages items'''
     def genpackagesitems():
-        if exists(require_fpath):
+        if os.path.exists(require_fpath):
             for info in parserequirefile(require_fpath):
                 parts = [info['package']]
                 if with_version and 'version' in info:
                     parts.extend(info['version'])
                 if not sys.version.startswith('3.4'):
                     platform_deps = info.get('platform_deps')
                     if platform_deps is not None:
```

### Comparing `sssegmentation-1.2.0/ssseg/configs/builder.py` & `SSSegmentation-1.3.0/ssseg/configs/builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 '''
 Function:
-    Build config file
+    Implementation of BuildConfig
 Author:
     Zhenchao Jin
 '''
 import os
 import time
 import shutil
 import importlib
+from distutils.dir_util import copy_tree
 
 
 '''BuildConfig'''
 def BuildConfig(cfg_file_path, tmp_cfg_dir='tmp_cfg'):
     # assert whether file exists
     assert os.path.exists(cfg_file_path), 'cfg_file_path %s not exist' % cfg_file_path
     # get config file info
     cfg_file_path = os.path.abspath(os.path.expanduser(cfg_file_path))
     cfg_info, ext = os.path.splitext(cfg_file_path)
     assert ext in ['.py'], 'only support .py type, but get %s' % ext
     cfg_dir, cfg_name = '/'.join(cfg_info.split('/')[:-1]), cfg_info.split('/')[-1]
+    _base_cfg_dir = os.path.join('/'.join(cfg_info.split('/')[:-2]), '_base_')
+    segmentor_dir = cfg_info.split('/')[-2]
     # base_cfg.py must exist
     base_cfg_file_path = os.path.join(cfg_dir, 'base_cfg' + ext)
     assert os.path.exists(base_cfg_file_path), 'base_cfg_file_path %s not exist' % base_cfg_file_path
+    assert os.path.exists(_base_cfg_dir), '_base_cfg_dir %s not exist' % _base_cfg_dir
     # make temp dir for loading config
     if not os.path.exists(tmp_cfg_dir):
         try: os.mkdir(tmp_cfg_dir)
         except: pass
+    if not os.path.exists(os.path.join(tmp_cfg_dir, segmentor_dir)):
+        try: os.mkdir(os.path.join(tmp_cfg_dir, segmentor_dir))
+        except: pass
     # copy config file and the base config file
-    shutil.copyfile(cfg_file_path, os.path.join(tmp_cfg_dir, cfg_name + ext))
-    shutil.copyfile(base_cfg_file_path, os.path.join(tmp_cfg_dir, 'base_cfg' + ext))
+    try: copy_tree(_base_cfg_dir, os.path.join(tmp_cfg_dir, '_base_'))
+    except: pass
+    shutil.copyfile(cfg_file_path, os.path.join(tmp_cfg_dir, segmentor_dir, cfg_name + ext))
+    shutil.copyfile(base_cfg_file_path, os.path.join(tmp_cfg_dir, segmentor_dir, 'base_cfg' + ext))
     time.sleep(0.5)
     # load module from the temp dir
     try:
-        cfg = importlib.import_module(f'{tmp_cfg_dir}.{cfg_name}', __package__)
+        cfg = importlib.import_module(f'{tmp_cfg_dir}.{segmentor_dir}.{cfg_name}', __package__)
     except:
         import sys
         sys.path.insert(0, '.')
-        cfg = importlib.import_module(f'{tmp_cfg_dir}.{cfg_name}', __package__)
+        cfg = importlib.import_module(f'{tmp_cfg_dir}.{segmentor_dir}.{cfg_name}', __package__)
     # return cfg
     return cfg, cfg_file_path
```

### Comparing `sssegmentation-1.2.0/ssseg/inference.py` & `SSSegmentation-1.3.0/ssseg/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 '''
 Function:
-    Visualize the segmentation results by using our segmentors
+    Implementation of Demo
 Author:
     Zhenchao Jin
 '''
 import os
 import cv2
 import copy
 import torch
 import warnings
 import argparse
 import numpy as np
 import torch.nn.functional as F
 from tqdm import tqdm
 from configs import BuildConfig
 from modules import (
-    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildOptimizer, BuildScheduler,
-    BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, Logger, setRandomSeed, BuildPalette, checkdir, loadcheckpoints, savecheckpoints
+    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, 
+    Logger, initslurm, setrandomseed, touchdir, loadckpts, saveckpts, BuildOptimizer, BuildScheduler
 )
 warnings.filterwarnings('ignore')
 
 
 '''parse arguments in command line'''
 def parseArgs():
     parser = argparse.ArgumentParser(description='SSSegmentation is an open source supervised semantic segmentation toolbox based on PyTorch')
     parser.add_argument('--imagedir', dest='imagedir', help='images dir for testing multi images', type=str)
     parser.add_argument('--imagepath', dest='imagepath', help='imagepath for testing single image', type=str)
     parser.add_argument('--outputfilename', dest='outputfilename', help='name to save output image(s)', type=str, default='')
     parser.add_argument('--cfgfilepath', dest='cfgfilepath', help='config file path you want to use', type=str, required=True)
-    parser.add_argument('--checkpointspath', dest='checkpointspath', help='checkpoints you want to resume from', type=str, required=True)
+    parser.add_argument('--ckptspath', dest='ckptspath', help='checkpoints you want to resume from', type=str, required=True)
     args = parser.parse_args()
     return args
 
 
 '''Demo'''
 class Demo():
     def __init__(self):
         self.cmd_args = parseArgs()
         self.cfg, self.cfg_file_path = BuildConfig(self.cmd_args.cfgfilepath)
         assert self.cmd_args.imagepath or self.cmd_args.imagedir, 'imagepath or imagedir should be specified'
+        # open full fp32
+        torch.backends.cuda.matmul.allow_tf32 = False
+        torch.backends.cudnn.allow_tf32 = False
     '''start'''
     def start(self):
         cmd_args, cfg, cfg_file_path = self.cmd_args, self.cfg, self.cfg_file_path
         # check work dir
-        checkdir(cfg.COMMON_CFG['work_dir'])
+        checkdir(cfg.SEGMENTOR_CFG['work_dir'])
         # cuda detect
         use_cuda = torch.cuda.is_available()
         # initialize logger_handle
-        logger_handle = Logger(cfg.COMMON_CFG['logfilepath'])
+        logger_handle = Logger(cfg.SEGMENTOR_CFG['logfilepath'])
         # build segmentor
         cfg.SEGMENTOR_CFG['backbone']['pretrained'] = False
-        segmentor = BuildSegmentor(segmentor_cfg=copy.deepcopy(cfg.SEGMENTOR_CFG), mode='TEST')
+        segmentor = BuildSegmentor(segmentor_cfg=cfg.SEGMENTOR_CFG, mode='TEST')
         if use_cuda: segmentor = segmentor.cuda()
         # build dataset
-        dataset_cfg = copy.deepcopy(cfg.DATASET_CFG)
-        dataset_cfg['type'] = 'base'
-        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=copy.deepcopy(cfg.DATASET_CFG))
+        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=cfg.SEGMENTOR_CFG['dataset'])
         # build palette
-        palette = BuildPalette(dataset_type=cfg.DATASET_CFG['type'], num_classes=cfg.SEGMENTOR_CFG['num_classes'], logger_handle=logger_handle)
-        # load checkpoints
+        palette = dataset.palette
+        # load ckpts
         cmd_args.local_rank = 0
-        checkpoints = loadcheckpoints(cmd_args.checkpointspath, logger_handle=logger_handle, cmd_args=cmd_args)
+        ckpts = loadckpts(cmd_args.ckptspath)
         try:
-            segmentor.load_state_dict(checkpoints['model'])
+            segmentor.load_state_dict(ckpts['model'])
         except Exception as e:
-            logger_handle.warning(str(e) + '\n' + 'Try to load checkpoints by using strict=False')
-            segmentor.load_state_dict(checkpoints['model'], strict=False)
+            logger_handle.warning(str(e) + '\n' + 'Try to load ckpts by using strict=False')
+            segmentor.load_state_dict(ckpts['model'], strict=False)
         # set eval
         segmentor.eval()
         # start to test
-        inference_cfg = copy.deepcopy(cfg.INFERENCE_CFG)
+        inference_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['inference'])
         FloatTensor = torch.cuda.FloatTensor if use_cuda else torch.FloatTensor
         if not cmd_args.imagedir:
             imagepaths = [cmd_args.imagepath]
         else:
             imagenames = os.listdir(cmd_args.imagedir)
             imagepaths = [os.path.join(cmd_args.imagedir, name) for name in imagenames]
         pbar = tqdm(range(len(imagepaths)))
@@ -113,17 +114,17 @@
             pred = (torch.argmax(output[0], dim=0)).cpu().numpy().astype(np.int32)
             mask = np.zeros((pred.shape[0], pred.shape[1], 3), dtype=np.uint8)
             for clsid, color in enumerate(palette):
                 mask[pred == clsid, :] = np.array(color)[::-1]
             image = image * 0.5 + mask * 0.5
             image = image.astype(np.uint8)
             if cmd_args.outputfilename:
-                cv2.imwrite(os.path.join(cfg.COMMON_CFG['work_dir'], cmd_args.outputfilename + '_%d' % idx + '.png'), image)
+                cv2.imwrite(os.path.join(cfg.SEGMENTOR_CFG['work_dir'], cmd_args.outputfilename + '_%d' % idx + '.png'), image)
             else:
-                cv2.imwrite(os.path.join(cfg.COMMON_CFG['work_dir'], imagepath.split('/')[-1].split('.')[0] + '.png'), image)
+                cv2.imwrite(os.path.join(cfg.SEGMENTOR_CFG['work_dir'], imagepath.split('/')[-1].split('.')[0] + '.png'), image)
     '''inference with augmentations'''
     def auginference(self, segmentor, images, inference_cfg, num_classes, FloatTensor, align_corners, forward_args=None):
         infer_tricks, outputs_list = inference_cfg['tricks'], []
         for scale_factor in infer_tricks['multiscale']:
             images_scale = F.interpolate(images, scale_factor=scale_factor, mode='bilinear', align_corners=align_corners)
             outputs = self.inference(
                 segmentor=segmentor, 
@@ -138,22 +139,22 @@
                 outputs_flip = self.inference(
                     segmentor=segmentor, 
                     images=images_flip.type(FloatTensor), 
                     inference_cfg=inference_cfg, 
                     num_classes=num_classes, 
                     forward_args=forward_args,
                 )
-                fix_ann_pairs = inference_cfg.get('fix_ann_pairs', None)
-                if fix_ann_pairs is None:
-                    for aug_opt in self.cfg.DATASET_CFG['train']['aug_opts']:
-                        if 'RandomFlip' in aug_opt: 
-                            fix_ann_pairs = aug_opt[-1].get('fix_ann_pairs', None)
-                if fix_ann_pairs is not None:
+                fixed_seg_target_pairs = inference_cfg.get('fixed_seg_target_pairs', None)
+                if fixed_seg_target_pairs is None:
+                    for data_pipeline in self.cfg.SEGMENTOR_CFG['dataset']['train']['data_pipelines']:
+                        if 'RandomFlip' in data_pipeline: 
+                            fixed_seg_target_pairs = data_pipeline[-1].get('fixed_seg_target_pairs', None)
+                if fixed_seg_target_pairs is not None:
                     outputs_flip_clone = outputs_flip.data.clone()
-                    for (pair_a, pair_b) in fix_ann_pairs:
+                    for (pair_a, pair_b) in fixed_seg_target_pairs:
                         outputs_flip[:, pair_a, :, :] = outputs_flip_clone[:, pair_b, :, :]
                         outputs_flip[:, pair_b, :, :] = outputs_flip_clone[:, pair_a, :, :]
                 outputs_flip = torch.from_numpy(np.flip(outputs_flip.cpu().numpy(), axis=3).copy()).type_as(outputs)
                 outputs_list.append(outputs_flip)
         return outputs_list
     '''inference'''
     def inference(self, segmentor, images, inference_cfg, num_classes, forward_args=None):
@@ -163,15 +164,15 @@
             if forward_args is None:
                 outputs = segmentor(images)
             else:
                 outputs = segmentor(images, **forward_args)
             if use_probs_before_resize: 
                 outputs = F.softmax(outputs, dim=1)
         else:
-            align_corners = segmentor.module.align_corners
+            align_corners = segmentor.align_corners
             opts = inference_cfg['opts']
             stride_h, stride_w = opts['stride']
             cropsize_h, cropsize_w = opts['cropsize']
             batch_size, _, image_h, image_w = images.size()
             num_grids_h = max(image_h - cropsize_h + stride_h - 1, 0) // stride_h + 1
             num_grids_w = max(image_w - cropsize_w + stride_w - 1, 0) // stride_w + 1
             outputs = images.new_zeros((batch_size, num_classes, image_h, image_w))
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/atr.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/sbushadow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 '''
 Function:
-    Load the ATR dataset
+    Implementation of SBUShadowDataset
 Author:
     Zhenchao Jin
 '''
 import os
-import pandas as pd
 from .base import BaseDataset
 
 
-'''ATRDataset'''
-class ATRDataset(BaseDataset):
-    num_classes = 18
-    classnames = [
-        '__background__', 'hat', 'hair', 'sunglasses', 'coat', 'skirt', 
-        'pants', 'dress', 'belt', 'leftShoe', 'rightShoe', 'face', 
-        'leftLeg', 'rightLeg', 'leftHand', 'rightHand', 'bags', 'scarf'
-    ]
-    assert num_classes == len(classnames)
+'''SBUShadowDataset'''
+class SBUShadowDataset(BaseDataset):
+    num_classes = 2
+    classnames = ['__backgroud__', 'shadow']
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(ATRDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(SBUShadowDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
-        self.image_dir = os.path.join(rootdir, 'JPEGImages')
-        self.ann_dir = os.path.join(rootdir, 'SegmentationClassAug')
+        setmap_dict = {'train': 'SBUTrain4KRecoveredSmall', 'val': 'SBU-Test'}
+        self.image_dir = os.path.join(rootdir, setmap_dict[dataset_cfg['set']], 'ShadowImages')
+        self.ann_dir = os.path.join(rootdir, setmap_dict[dataset_cfg['set']], 'ShadowMasks')
         # obatin imageids
-        df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'_id.txt'), names=['imageids'])
-        self.imageids = df['imageids'].values
+        self.imageids = []
+        for line in open(os.path.join(rootdir, dataset_cfg['set']+'.txt'), 'r').readlines():
+            if line.strip(): self.imageids.append(line.strip())
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
+    '''getitem'''
     def __getitem__(self, index):
-        imageid = self.imageids[index]
-        imagepath = os.path.join(self.image_dir, imageid+'.jpg')
-        annpath = os.path.join(self.ann_dir, imageid+'.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        sample_meta['seg_target'][sample_meta['seg_target'] > 0] = 1.
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/base.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,145 @@
 '''
 Function:
-    Base class for loadding dataset
+    Implementation of BaseDataset
 Author:
     Zhenchao Jin
 '''
+import os
 import cv2
 import torch
 import numpy as np
 import scipy.io as sio
 from PIL import Image
 from chainercv.evaluations import eval_semantic_segmentation
-from .pipelines import Evaluation, Resize, RandomCrop, RandomFlip, PhotoMetricDistortion, RandomRotation, Padding, ToTensor, Normalize, Compose
+from .pipelines import (
+    Evaluation, Resize, RandomCrop, RandomFlip, PhotoMetricDistortion,
+    RandomRotation, Padding, ToTensor, Normalize, Compose, EdgeExtractor
+)
 
 
 '''BaseDataset'''
 class BaseDataset(torch.utils.data.Dataset):
     def __init__(self, mode, logger_handle, dataset_cfg):
+        # assert
         assert mode in ['TRAIN', 'TEST']
+        # set attributes
         self.mode = mode
-        self.logger_handle = logger_handle
+        self.ann_ext = '.png'
+        self.image_ext = '.jpg'
         self.dataset_cfg = dataset_cfg
-        self.transforms = Compose(self.constructtransforms(self.dataset_cfg['aug_opts']))
-    '''pull item'''
+        self.logger_handle = logger_handle
+        self.repeat_times = dataset_cfg.get('repeat_times', 1)
+        self.transforms = self.constructtransforms(self.dataset_cfg['data_pipelines'])
+    '''getitem'''
     def __getitem__(self, index):
-        raise NotImplementedError('not be implemented')
-    '''length'''
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
+    '''len'''
     def __len__(self):
-        raise NotImplementedError('not be implemented')
-    '''sync transform'''
-    def synctransform(self, sample, transform_type):
-        assert hasattr(self, 'transforms') and self.transforms, 'undefined transforms'
-        assert transform_type in ['all', 'only_totensor_normalize_pad', 'without_totensor_normalize_pad']
-        sample = self.transforms(sample, transform_type)
-        return sample
-    '''read sample'''
-    def read(self, imagepath, annpath, with_ann=True):
-        assert self.mode in ['TRAIN', 'TEST']
+        return len(self.imageids) * self.repeat_times
+    '''read sample_meta'''
+    def read(self, imagepath, annpath):
         # read image
         image = cv2.imread(imagepath)
         # read annotation
-        if annpath.endswith('.png'):
-            if self.dataset_cfg['type'] in ['vspw']:
-                segmentation = np.array(Image.open(annpath)) if with_ann else np.zeros((image.shape[0], image.shape[1]))
+        assert annpath.split('.')[-1] in ['png', 'mat']
+        if not os.path.exists(annpath):
+            seg_target = np.zeros((image.shape[0], image.shape[1]))
+            self.logger_handle.warning(f'seg_target from {annpath} is missed')
+        elif annpath.endswith('.png'):
+            if self.dataset_cfg['type'] in ['VSPWDataset']:
+                seg_target = np.array(Image.open(annpath))
             else:
-                segmentation = cv2.imread(annpath, cv2.IMREAD_GRAYSCALE) if with_ann else np.zeros((image.shape[0], image.shape[1]))
+                seg_target = cv2.imread(annpath, cv2.IMREAD_GRAYSCALE)
         elif annpath.endswith('.mat'):
-            segmentation = sio.loadmat(annpath)
-            if self.dataset_cfg['type'] in ['cocostuff10k']:
-                segmentation = segmentation['S']
+            seg_target = sio.loadmat(annpath)
+            if self.dataset_cfg['type'] in ['COCOStuff10kDataset']:
+                seg_target = seg_target['S']
         else:
-            raise NotImplementedError('Unsupport data type of %s' % annpath.split('.')[-1])
-        if with_ann and hasattr(self, 'clsid2label'):
+            seg_target = np.zeros((image.shape[0], image.shape[1]))
+            self.logger_handle.warning(f'seg_target from {annpath} is not supported to read')
+        # auto transform seg_target to train labels
+        if hasattr(self, 'clsid2label'):
             for key, value in self.clsid2label.items():
-                segmentation[segmentation == key] = value
-        # edge placeholder
-        edge = np.zeros((32, 32))
-        # return sample
-        sample = {
-            'image': image, 
-            'segmentation': segmentation.copy(), 
-            'edge': edge, 
-            'width': image.shape[1], 
-            'height': image.shape[0]
+                seg_target[seg_target == key] = value
+        # construct sample_meta
+        sample_meta = {
+            'image': image, 'seg_target': seg_target, 'width': image.shape[1], 'height': image.shape[0],
         }
-        if self.mode == 'TEST': sample.update({'groundtruth': segmentation.copy()})
-        return sample
-    '''construct the transforms'''
-    def constructtransforms(self, aug_opts):
-        # obtain the transforms
-        transforms = []
-        supported_transforms = {
-            'Resize': Resize,
-            'RandomCrop': RandomCrop,
-            'RandomFlip': RandomFlip,
-            'PhotoMetricDistortion': PhotoMetricDistortion,
-            'RandomRotation': RandomRotation,
-            'Padding': Padding,
-            'ToTensor': ToTensor,
-            'Normalize': Normalize
-        }
-        for aug_opt in aug_opts:
-            key, value = aug_opt
-            assert key in supported_transforms, 'unsupport transform %s' % key
-            transforms.append(supported_transforms[key](**value))
-        # return the transforms
-        return transforms
-    '''evaluate the predictions'''
-    def evaluate(self, predictions, groundtruths, metric_list=['iou', 'miou'], num_classes=None, ignore_index=-1, nan_to_num=None, beta=1.0):
-        eval_client = None
-        result = eval_semantic_segmentation(predictions, groundtruths)
-        result_selected = {}
+        # return
+        return sample_meta
+    '''evaluate'''
+    def evaluate(self, seg_preds, seg_targets, metric_list=['iou', 'miou'], num_classes=None, ignore_index=-1, nan_to_num=None, beta=1.0):
+        # basic evaluation
+        result = eval_semantic_segmentation(seg_preds, seg_targets)
+        # selected result
+        selected_result, eval_client = {}, None
         for metric in metric_list:
             if metric in result:
-                result_selected[metric] = result[metric]
+                selected_result[metric] = result[metric]
             else:
-                if eval_client is None:
-                    eval_client = Evaluation(predictions, groundtruths, num_classes, ignore_index, nan_to_num, beta)
-                assert metric in eval_client.all_metric_results, 'unsupport %s as the metric' % metric
-                result_selected[metric] = eval_client.all_metric_results[metric]
-        if 'iou' in result_selected:
-            iou_list = result_selected['iou']
-            iou_dict = {}
+                if eval_client is None: eval_client = Evaluation(seg_preds, seg_targets, num_classes, ignore_index, nan_to_num, beta)
+                assert metric in eval_client.all_metric_results
+                selected_result[metric] = eval_client.all_metric_results[metric]
+        # insert class names for iou and dice
+        if 'iou' in selected_result:
+            iou_list, iou_dict = selected_result['iou'], {}
             for idx, item in enumerate(iou_list):
                 iou_dict[self.classnames[idx]] = item
-            result_selected['iou'] = iou_dict
-        if 'dice' in result_selected:
-            dice_list = result_selected['dice']
-            dice_dict = {}
+            selected_result['iou'] = iou_dict
+        if 'dice' in selected_result:
+            dice_list, dice_dict = selected_result['dice'], {}
             for idx, item in enumerate(dice_list):
                 dice_dict[self.classnames[idx]] = item
-            result_selected['dice'] = dice_dict
-        return result_selected
-    '''generate edge'''
-    def generateedge(self, segmentation, edge_width=3, ignore_index=255):
-        h, w = segmentation.shape
-        edge = np.zeros(segmentation.shape)
-        # right
-        edge_right = edge[1: h, :]
-        edge_right[(segmentation[1: h, :] != segmentation[:h-1, :]) & (segmentation[1: h, :] != ignore_index) & (segmentation[:h-1, :] != ignore_index)] = 1
-        # up
-        edge_up = edge[:, :w-1]
-        edge_up[(segmentation[:, :w-1] != segmentation[:, 1: w]) & (segmentation[:, :w-1] != ignore_index) & (segmentation[:, 1: w] != ignore_index)] = 1
-        # upright
-        edge_upright = edge[:h-1, :w-1]
-        edge_upright[(segmentation[:h-1, :w-1] != segmentation[1: h, 1: w]) & (segmentation[:h-1, :w-1] != ignore_index) & (segmentation[1: h, 1: w] != ignore_index)] = 1
-        # bottomright
-        edge_bottomright = edge[:h-1, 1: w]
-        edge_bottomright[(segmentation[:h-1, 1: w] != segmentation[1: h, :w-1]) & (segmentation[: h-1, 1: w] != ignore_index) & (segmentation[1: h, :w-1] != ignore_index)] = 1
+            selected_result['dice'] = dice_dict
+        # return
+        return selected_result      
+    '''constructtransforms'''
+    def constructtransforms(self, data_pipelines):
+        # supported transforms
+        supported_transforms = {
+            'Resize': Resize, 'RandomCrop': RandomCrop, 'RandomFlip': RandomFlip, 'RandomRotation': RandomRotation, 'EdgeExtractor': EdgeExtractor,
+            'PhotoMetricDistortion': PhotoMetricDistortion, 'Padding': Padding, 'ToTensor': ToTensor, 'Normalize': Normalize,
+        }
+        # build transforms
+        transforms = []
+        for data_pipeline in data_pipelines:
+            assert len(data_pipeline) == 2
+            transforms.append(supported_transforms[data_pipeline[0]](**data_pipeline[1]))
+        transforms = Compose(transforms)
         # return
-        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (edge_width, edge_width))
-        edge = cv2.dilate(edge, kernel)
-        return edge
+        return transforms
+    '''synctransforms'''
+    def synctransforms(self, sample_meta):
+        if self.mode == 'TEST':
+            seg_target = sample_meta.pop('seg_target')
+        sample_meta = self.transforms(sample_meta)
+        if self.mode == 'TEST':
+            sample_meta['seg_target'] = seg_target
+        return sample_meta
+    '''randompalette'''
+    @staticmethod
+    def randompalette(num_classes):
+        palette = [0] * (num_classes * 3)
+        for j in range(0, num_classes):
+            i, lab = 0, j
+            palette[j * 3 + 0], palette[j * 3 + 1], palette[j * 3 + 2] = 0, 0, 0
+            while lab:
+                palette[j * 3 + 0] |= (((lab >> 0) & 1) << (7 - i))
+                palette[j * 3 + 1] |= (((lab >> 1) & 1) << (7 - i))
+                palette[j * 3 + 2] |= (((lab >> 2) & 1) << (7 - i))
+                i += 1
+                lab >>= 3
+        palette = np.array(palette).reshape(-1, 3)
+        palette = palette.tolist()
+        return palette
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/chasedb1.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/drive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 '''
 Function:
-    Load the chasedb1 dataset
+    Implementation of DRIVEDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import pandas as pd
 from .base import BaseDataset
 
 
-'''ChaseDB1Dataset'''
-class ChaseDB1Dataset(BaseDataset):
+'''DRIVEDataset'''
+class DRIVEDataset(BaseDataset):
     num_classes = 2
     classnames = ['__background__', 'vessel']
-    assert num_classes == len(classnames)
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(ChaseDB1Dataset, self).__init__(mode, logger_handle, dataset_cfg)
-        self.repeat_times = dataset_cfg.get('repeat_times', 1)
+        super(DRIVEDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         setmap_dict = {'train': 'training', 'val': 'validation'}
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, 'images', setmap_dict[dataset_cfg['set']])
         self.ann_dir = os.path.join(rootdir, 'annotations', setmap_dict[dataset_cfg['set']])
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
+        self.ann_ext = '_manual1.png'
+        self.image_ext = self.imageids[0].split('.')[-1]
+        self.imageids = [_id.split('.')[0] for _id in self.imageids]
+    '''getitem'''
     def __getitem__(self, index):
+        # imageid
         imageid = self.imageids[index % len(self.imageids)]
-        imagepath = os.path.join(self.image_dir, imageid)
-        annpath = os.path.join(self.ann_dir, imageid.split('.')[0] + '_1stHO.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids) * self.repeat_times
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}.{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/cihp.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/stare.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 '''
 Function:
-    Load the CIHP dataset
+    Implementation of STAREDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import pandas as pd
 from .base import BaseDataset
 
 
-'''CIHPDataset'''
-class CIHPDataset(BaseDataset):
-    num_classes = 20
-    classnames = [
-        '__background__', 'hat', 'hair', 'glove', 'sunglasses', 'upperclothes', 'dress', 
-        'coat', 'socks', 'pants', 'torsoSkin', 'scarf', 'skirt', 'face', 
-        'leftArm', 'rightArm', 'leftLeg', 'rightLeg', 'leftShoe', 'rightShoe'
-    ]
-    assert num_classes == len(classnames)
+'''STAREDataset'''
+class STAREDataset(BaseDataset):
+    num_classes = 2
+    classnames = ['__background__', 'vessel']
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(CIHPDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(STAREDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
+        setmap_dict = {'train': 'training', 'val': 'validation'}
         rootdir = dataset_cfg['rootdir']
-        setmap_dict = {'train': 'Training', 'val': 'Validation', 'test': 'Testing'}
-        self.image_dir = os.path.join(rootdir, f"{setmap_dict[dataset_cfg['set']]}/Images")
-        self.ann_dir = os.path.join(rootdir, f"{setmap_dict[dataset_cfg['set']]}/Category_ids")
+        self.image_dir = os.path.join(rootdir, 'images', setmap_dict[dataset_cfg['set']])
+        self.ann_dir = os.path.join(rootdir, 'annotations', setmap_dict[dataset_cfg['set']])
         # obatin imageids
-        df = pd.read_csv(os.path.join(rootdir, setmap_dict[dataset_cfg['set']], dataset_cfg['set']+'_id.txt'), names=['imageids'])
+        df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
-        self.imageids = [str(_id).zfill(7) for _id in self.imageids]
-    '''pull item'''
+        self.imageids = [str(_id) for _id in self.imageids]
+        self.ann_ext = '.ah.png'
+        self.image_ext = self.imageids[0].split('.')[-1]
+        self.imageids = [_id.split('.')[0] for _id in self.imageids]
+    '''getitem'''
     def __getitem__(self, index):
-        imageid = self.imageids[index]
-        imagepath = os.path.join(self.image_dir, imageid+'.jpg')
-        annpath = os.path.join(self.ann_dir, imageid+'.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}.{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/cityscapes.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/cityscapes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 '''
 Function:
-    Load the CityScapes dataset
+    Implementation of CityScapesDataset
 Author:
     Zhenchao Jin
 '''
 import os
+import numpy as np
 import pandas as pd
 from PIL import Image
 from .base import BaseDataset
 
 
 '''CityScapesDataset'''
 class CityScapesDataset(BaseDataset):
     num_classes = 19
     classnames = [
         'road', 'sidewalk', 'building', 'wall', 'fence', 'pole', 'traffic_light', 
         'traffic_sign', 'vegetation', 'terrain', 'sky', 'person', 'rider', 'car', 
         'truck', 'bus', 'train', 'motorcycle', 'bicycle'
     ]
+    palette = [
+        (128, 64, 128), (244, 35, 232), (70, 70, 70), (102, 102, 156), (190, 153, 153), (153, 153, 153), (250, 170, 30), (220, 220, 0),
+        (107, 142, 35), (152, 251, 152), (70, 130, 180), (220, 20, 60), (255, 0, 0), (0, 0, 142), (0, 0, 70), (0, 60, 100),
+        (0, 80, 100), (0, 0, 230), (119, 11, 32)
+    ]
     clsid2label = {
         -1: 255, 0: 255, 1: 255, 2: 255, 3: 255, 4: 255, 5: 255, 6: 255,
         7: 0, 8: 1, 9: 255, 10: 255, 11: 2, 12: 3, 13: 4, 14: 255, 
         15: 255, 16: 255, 17: 5, 18: 255, 19: 6, 20: 7, 21: 8, 22: 9, 
         23: 10, 24: 11, 25: 12, 26: 13, 27: 14, 28: 15, 29: 255, 30: 255, 
         31: 16, 32: 17, 33: 18
     }
-    assert num_classes == len(classnames)
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(CityScapesDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(CityScapesDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, 'leftImg8bit', dataset_cfg['set'])
         self.ann_dir = os.path.join(rootdir, 'gtFine', dataset_cfg['set'])
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
+        self.ann_ext = '.png'
+        self.image_ext = '.png'
+    '''getitem'''
     def __getitem__(self, index):
-        imageid = self.imageids[index]
-        imagepath = os.path.join(self.image_dir, imageid+'.png')
-        annpath = os.path.join(self.ann_dir, imageid.replace('leftImg8bit', 'gtFine_labelIds')+'.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid.replace("leftImg8bit", "gtFine_labelIds")}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
     '''format results for test set of Cityscapes'''
     @staticmethod
     def formatresults(results, filenames, to_label_id=True, savedir='results'):
         assert len(filenames) == len(results)
         def convert(result):
             import cityscapesscripts.helpers.labels as CSLabels
             result_copy = result.copy()
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/coco.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/coco.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Load the coco dataset
+    Implementation of COCODataset, COCOStuff10kDataset and COCOStuffDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import cv2
 import pandas as pd
 from tqdm import tqdm
@@ -15,18 +15,23 @@
 class COCODataset(BaseDataset):
     num_classes = 21
     classnames = [
         '__background__', 'airplane', 'bicycle', 'bird', 'boat', 'bottle', 'bus', 'car', 
         'cat', 'chair', 'cow', 'diningtable', 'dog', 'horse', 'motorcycle', 'person', 
         'potted-plant', 'sheep', 'sofa', 'train', 'tv'
     ]
+    palette = [
+        (0, 0, 0), (128, 0, 0), (0, 128, 0), (128, 128, 0), (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128), (64, 0, 0),
+        (192, 0, 0), (64, 128, 0), (192, 128, 0), (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128), (0, 64, 0),
+        (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)
+    ]
     valid_clsids = [0, 5, 2, 16, 9, 44, 6, 3, 17, 62, 21, 67, 18, 19, 4, 1, 64, 20, 63, 7, 72]
-    assert num_classes == len(classnames)
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(COCODataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(COCODataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         from pycocotools import mask
         from pycocotools.coco import COCO
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, f"{dataset_cfg['set']}2017")
         # obatin imageids
         self.annfilepath = os.path.join(rootdir, f"annotations/instances_{dataset_cfg['set']}2017.json")
@@ -34,48 +39,37 @@
         self.cocomask_api = mask
         self.imageids = []
         imageids_bar = tqdm(list(self.coco_api.imgs.keys()))
         for imageid in imageids_bar:
             imageids_bar.set_description('Preprocess imageid %s' % imageid)
             target = self.coco_api.loadAnns(self.coco_api.getAnnIds(imgIds=imageid))
             image_meta = self.coco_api.loadImgs(imageid)[0]
-            segmentation = self.getsegmentation(target, image_meta['height'], image_meta['width'])
-            if (segmentation > 0).sum() > 1000:
+            seg_target = self.getsegtarget(target, image_meta['height'], image_meta['width'])
+            if (seg_target > 0).sum() > 1000:
                 self.imageids.append(imageid)
-    '''pull item'''
+    '''getitem'''
     def __getitem__(self, index):
-        imageid = self.imageids[index]
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
         image_meta = self.coco_api.loadImgs(imageid)[0]
         imagepath = os.path.join(self.image_dir, image_meta['file_name'])
         # read image
         image = cv2.imread(imagepath)
         # read annotation
-        if self.dataset_cfg.get('with_ann', True):
-            target = self.coco_api.loadAnns(self.coco_api.getAnnIds(imgIds=imageid))
-            segmentation = self.getsegmentation(target, image_meta['height'], image_meta['width'])
-        else:
-            segmentation = np.zeros((image.shape[0], image.shape[1]))
-        # construct sample
-        sample = {'image': image, 'segmentation': segmentation, 'width': image.shape[1], 'height': image.shape[0]}
-        if self.mode == 'TEST':
-            sample.update({'groundtruth': segmentation.copy()})
-        sample.update({'id': imageid})
-        # preprocess and return sample
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
-    '''get segmentation mask'''
-    def getsegmentation(self, target, height, width):
+        seg_target = self.coco_api.loadAnns(self.coco_api.getAnnIds(imgIds=imageid))
+        seg_target = self.getsegtarget(seg_target, image_meta['height'], image_meta['width'])
+        # construct sample_meta
+        sample_meta = {'image': image, 'seg_target': seg_target, 'width': image.shape[1], 'height': image.shape[0]}
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
+    '''getsegtarget'''
+    def getsegtarget(self, target, height, width):
         segmentation = np.zeros((height, width), dtype=np.uint8)
         for instance in target:
             rle = self.cocomask_api.frPyObjects(instance['segmentation'], height, width)
             mask = self.cocomask_api.decode(rle)
             clsid = instance['category_id']
             if clsid not in self.valid_clsids: continue
             label = self.valid_clsids.index(clsid)
@@ -103,44 +97,30 @@
         'fruit', 'furniture-other', 'grass', 'gravel', 'ground-other', 'hill', 'house', 'leaves', 'light', 'mat', 'metal',
         'mirror-stuff', 'moss', 'mountain', 'mud', 'napkin', 'net', 'paper', 'pavement', 'pillow', 'plant-other', 'plastic',
         'platform', 'playingfield', 'railing', 'railroad', 'river', 'road', 'rock', 'roof', 'rug', 'salad', 'sand', 'sea',
         'shelf', 'sky-other', 'skyscraper', 'snow', 'solid-other', 'stairs', 'stone', 'straw', 'structural-other', 'table',
         'tent', 'textile-other', 'towel', 'tree', 'vegetable', 'wall-brick', 'wall-concrete', 'wall-other', 'wall-panel',
         'wall-stone', 'wall-tile', 'wall-wood', 'water-other', 'waterdrops', 'window-blind', 'window-other', 'wood'
     ]
+    palette = BaseDataset.randompalette(num_classes)
     clsid2label = {0: 255}
     for i in range(1, num_classes+1): clsid2label[i] = i - 1
-    assert num_classes == len(classnames)
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(COCOStuff10kDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(COCOStuff10kDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, 'images')
         self.ann_dir = os.path.join(rootdir, 'annotations')
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, 'imageLists', dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
-    def __getitem__(self, index):
-        imageid = self.imageids[index]
-        imagepath = os.path.join(self.image_dir, imageid+'.jpg')
-        annpath = os.path.join(self.ann_dir, imageid+'.mat')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+        self.ann_ext = '.mat'
+        self.image_ext = '.jpg'
 
 
 '''COCOStuffDataset'''
 class COCOStuffDataset(BaseDataset):
     num_classes = 182
     classnames = [
         'person', 'bicycle', 'car', 'motorcycle', 'airplane', 'bus', 'train', 'truck', 'boat', 'traffic light',
@@ -158,39 +138,37 @@
         'fruit', 'furniture-other', 'grass', 'gravel', 'ground-other', 'hill', 'house', 'leaves', 'light', 'mat', 'metal',
         'mirror-stuff', 'moss', 'mountain', 'mud', 'napkin', 'net', 'paper', 'pavement', 'pillow', 'plant-other', 'plastic',
         'platform', 'playingfield', 'railing', 'railroad', 'river', 'road', 'rock', 'roof', 'rug', 'salad', 'sand', 'sea',
         'shelf', 'sky-other', 'skyscraper', 'snow', 'solid-other', 'stairs', 'stone', 'straw', 'structural-other', 'table',
         'tent', 'textile-other', 'towel', 'tree', 'vegetable', 'wall-brick', 'wall-concrete', 'wall-other', 'wall-panel',
         'wall-stone', 'wall-tile', 'wall-wood', 'water-other', 'waterdrops', 'window-blind', 'window-other', 'wood'
     ]
+    palette = BaseDataset.randompalette(num_classes)
     clsid2label = {0: 255}
     for i in range(1, num_classes+1): clsid2label[i] = i - 1
-    assert num_classes == len(classnames)
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(COCOStuffDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(COCOStuffDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         from pycocotools import mask
         from pycocotools.coco import COCO
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, f"{dataset_cfg['set']}2017")
         # obatin imageids
         self.annfilepath = os.path.join(rootdir, f"annotations/stuff_{dataset_cfg['set']}2017.json")
         self.coco_api = COCO(self.annfilepath)
         self.imageids = list(self.coco_api.imgs.keys())
-    '''pull item'''
+    '''getitem'''
     def __getitem__(self, index):
-        imageid = self.imageids[index]
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
         image_meta = self.coco_api.loadImgs(imageid)[0]
         imagepath = os.path.join(self.image_dir, image_meta['file_name'])
         annpath = imagepath.replace('jpg', 'png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/drive.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/chasedb1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 '''
 Function:
-    Load the drive dataset
+    Implementation of ChaseDB1Dataset
 Author:
     Zhenchao Jin
 '''
 import os
 import pandas as pd
 from .base import BaseDataset
 
 
-'''DRIVEDataset'''
-class DRIVEDataset(BaseDataset):
+'''ChaseDB1Dataset'''
+class ChaseDB1Dataset(BaseDataset):
     num_classes = 2
     classnames = ['__background__', 'vessel']
-    assert num_classes == len(classnames)
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(DRIVEDataset, self).__init__(mode, logger_handle, dataset_cfg)
-        self.repeat_times = dataset_cfg.get('repeat_times', 1)
+        super(ChaseDB1Dataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg) 
         # obtain the dirs
-        setmap_dict = {'train': 'training', 'val': 'validation'}
         rootdir = dataset_cfg['rootdir']
+        setmap_dict = {'train': 'training', 'val': 'validation'}
         self.image_dir = os.path.join(rootdir, 'images', setmap_dict[dataset_cfg['set']])
         self.ann_dir = os.path.join(rootdir, 'annotations', setmap_dict[dataset_cfg['set']])
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
+        self.image_ext = self.imageids[0].split('.')[-1]
+        self.ann_ext = '_1stHO.png'
+        self.imageids = [_id.split('.')[0] for _id in self.imageids]
+    '''getitem'''
     def __getitem__(self, index):
+        # imageid
         imageid = self.imageids[index % len(self.imageids)]
-        imagepath = os.path.join(self.image_dir, imageid)
-        annpath = os.path.join(self.ann_dir, imageid.split('.')[0] + '_manual1.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids) * self.repeat_times
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}.{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/hrf.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/hrf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,30 @@
 '''
 Function:
-    Load the hrf dataset
+    Implementation of HRFDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import pandas as pd
 from .base import BaseDataset
 
 
 '''HRFDataset'''
 class HRFDataset(BaseDataset):
     num_classes = 2
     classnames = ['__background__', 'vessel']
-    assert num_classes == len(classnames)
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(HRFDataset, self).__init__(mode, logger_handle, dataset_cfg)
-        self.repeat_times = dataset_cfg.get('repeat_times', 1)
+        super(HRFDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         setmap_dict = {'train': 'training', 'val': 'validation'}
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, 'images', setmap_dict[dataset_cfg['set']])
         self.ann_dir = os.path.join(rootdir, 'annotations', setmap_dict[dataset_cfg['set']])
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
-    def __getitem__(self, index):
-        imageid = self.imageids[index % len(self.imageids)]
-        imagepath = os.path.join(self.image_dir, imageid)
-        annpath = os.path.join(self.ann_dir, imageid)
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids) * self.repeat_times
+        self.ann_ext = ''
+        self.image_ext = ''
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/pipelines/evaluation.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/pipelines/evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Function:
-    Define some evaluation metric
+    Implementation of Evaluation
 Author:
     Zhenchao Jin
 '''
 import torch
 import numpy as np
 from collections import OrderedDict
 
 
 '''Evaluation'''
 class Evaluation():
-    def __init__(self, predictions, groundtruths, num_classes, ignore_index=-1, nan_to_num=None, beta=1.0):
+    def __init__(self, seg_preds, seg_targets, num_classes, ignore_index=-1, nan_to_num=None, beta=1.0):
         total_area_intersect, total_area_union, total_area_pred_label, total_area_label = self.totalintersectandunion(
-            results=predictions,
-            gt_seg_maps=groundtruths,
+            results=seg_preds,
+            gt_seg_maps=seg_targets,
             num_classes=num_classes,
             ignore_index=ignore_index
         )
         self.all_metric_results = self.totalareatometrics(
             total_area_intersect=total_area_intersect, 
             total_area_union=total_area_union, 
             total_area_pred_label=total_area_pred_label,
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/stare.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/supervisely.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 '''
 Function:
-    Load the stare dataset
+    Implementation of SuperviselyDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import pandas as pd
 from .base import BaseDataset
 
 
-'''STAREDataset'''
-class STAREDataset(BaseDataset):
+'''SuperviselyDataset'''
+class SuperviselyDataset(BaseDataset):
     num_classes = 2
-    classnames = ['__background__', 'vessel']
-    assert num_classes == len(classnames)
+    classnames = ['__background__', 'person']
+    palette = [(0, 0, 0), (255, 0, 0)]
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(STAREDataset, self).__init__(mode, logger_handle, dataset_cfg)
-        self.repeat_times = dataset_cfg.get('repeat_times', 1)
+        super(SuperviselyDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
-        setmap_dict = {'train': 'training', 'val': 'validation'}
         rootdir = dataset_cfg['rootdir']
-        self.image_dir = os.path.join(rootdir, 'images', setmap_dict[dataset_cfg['set']])
-        self.ann_dir = os.path.join(rootdir, 'annotations', setmap_dict[dataset_cfg['set']])
+        self.image_dir = os.path.join(rootdir, 'Images', dataset_cfg['set'])
+        self.ann_dir = os.path.join(rootdir, 'Anno-Person', dataset_cfg['set'])
         # obatin imageids
         df = pd.read_csv(os.path.join(rootdir, dataset_cfg['set']+'.txt'), names=['imageids'])
         self.imageids = df['imageids'].values
         self.imageids = [str(_id) for _id in self.imageids]
-    '''pull item'''
+    '''getitem'''
     def __getitem__(self, index):
+        # imageid
         imageid = self.imageids[index % len(self.imageids)]
-        imagepath = os.path.join(self.image_dir, imageid)
-        annpath = os.path.join(self.ann_dir, imageid.split('.')[0] + '.ah.png')
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': imageid})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids) * self.repeat_times
+        # read sample_meta
+        imagepath = os.path.join(self.image_dir, f'{imageid}{self.image_ext}')
+        annpath = os.path.join(self.ann_dir, f'{imageid}{self.ann_ext}')
+        sample_meta = self.read(imagepath, annpath)
+        sample_meta['seg_target'][sample_meta['seg_target'] == 255] = 1.
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/datasets/vspw.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/vspw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Load the VSPW dataset
+    Implementation of VSPWDataset
 Author:
     Zhenchao Jin
 '''
 import os
 import random
 from .base import BaseDataset
 
@@ -23,54 +23,52 @@
         'bat', 'ball', 'cupboard_or_showcase_or_storage_rack', 'box', 'traveling_case_or_trolley_case', 'basket', 'bag_or_package', 
         'trash_can', 'cage', 'plate', 'tub_or_bowl_or_pot', 'bottle_or_cup', 'barrel', 'fishbowl', 'bed', 'pillow', 'table_or_desk', 
         'chair_or_seat', 'bench', 'sofa', 'shelf', 'bathtub', 'gun', 'commode', 'roaster', 'other_machine', 'refrigerator', 'washing_machine', 
         'Microwave_oven', 'fan', 'curtain', 'textiles', 'clothes', 'painting_or_poster', 'mirror', 'flower_pot_or_vase', 'clock', 'book', 'tool', 
         'blackboard', 'tissue', 'screen_or_television', 'computer', 'printer', 'Mobile_phone', 'keyboard', 'other_electronic_product', 'fruit', 
         'food', 'instrument', 'train'
     ]
+    palette = BaseDataset.randompalette(num_classes)
     clsid2label = {0: 255, 254: 255}
     for i in range(1, num_classes+1): clsid2label[i] = i - 1
-    assert num_classes == len(classnames)
+    assert num_classes == len(classnames) and num_classes == len(palette)
     def __init__(self, mode, logger_handle, dataset_cfg):
-        super(VSPWDataset, self).__init__(mode, logger_handle, dataset_cfg)
+        super(VSPWDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
         # obtain the dirs
         rootdir = dataset_cfg['rootdir']
         self.image_dir = os.path.join(rootdir, 'data')
         self.ann_dir = os.path.join(rootdir, 'data')
         # obatin imageids
         self.imageids, self.annids = [], []
         with open(os.path.join(rootdir, dataset_cfg['set']+'.txt')) as fp:
             dirnames = fp.readlines()
             for dirname in dirnames:
                 dirname = dirname.strip()
                 if not dirname: continue
                 if mode == 'TRAIN':
                     self.imageids.append(dirname)
                 else:
-                    for imgname in os.listdir(os.path.join(self.image_dir, dirname, 'origin')):
-                        imageid = f'{dirname}/origin/{imgname}'
-                        annid = f'{dirname}/mask/{imgname.replace(".jpg", ".png")}'
+                    for imagename in os.listdir(os.path.join(self.image_dir, dirname, 'origin')):
+                        imageid = f'{dirname}/origin/{imagename}'
+                        annid = f'{dirname}/mask/{imagename.replace(".jpg", ".png")}'
                         self.imageids.append(imageid)
                         self.annids.append(annid)
-    '''pull item'''
+    '''getitem'''
     def __getitem__(self, index):
+        # imageid
+        imageid = self.imageids[index % len(self.imageids)]
+        # read sample_meta
         if self.mode == 'TRAIN':
-            imagedir = os.path.join(self.image_dir, self.imageids[index], 'origin')
-            imgname = random.choice(os.listdir(imagedir))
-            imagepath = os.path.join(imagedir, imgname)
-            annpath = os.path.join(self.ann_dir, self.imageids[index], f'mask/{imgname.replace(".jpg", ".png")}')
+            imagedir = os.path.join(self.image_dir, imageid, 'origin')
+            imagename = random.choice(os.listdir(imagedir))
+            imagepath = os.path.join(imagedir, imagename)
+            annpath = os.path.join(self.ann_dir, imageid, f'mask/{imagename.replace(".jpg", ".png")}')
         else:
-            imagepath = os.path.join(self.image_dir, self.imageids[index])
-            annpath = os.path.join(self.ann_dir, self.annids[index])
-        if self.dataset_cfg['set'] == 'test': self.dataset_cfg['with_ann'] = False
-        sample = self.read(imagepath, annpath, self.dataset_cfg.get('with_ann', True))
-        sample.update({'id': self.imageids[index]})
-        if self.mode == 'TRAIN':
-            sample = self.synctransform(sample, 'without_totensor_normalize_pad')
-            sample['edge'] = self.generateedge(sample['segmentation'].copy())
-            sample = self.synctransform(sample, 'only_totensor_normalize_pad')
-        else:
-            sample = self.synctransform(sample, 'all')
-        return sample
-    '''length'''
-    def __len__(self):
-        return len(self.imageids)
+            imagepath = os.path.join(self.image_dir, imageid)
+            annpath = os.path.join(self.ann_dir, self.annids[index % len(self.imageids)])
+        sample_meta = self.read(imagepath, annpath)
+        # add image id
+        sample_meta.update({'id': imageid})
+        # synctransforms
+        sample_meta = self.synctransforms(sample_meta)
+        # return
+        return sample_meta
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/beit.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/beit.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,30 @@
 import torch
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 from scipy import interpolate
 from .vit import TransformerEncoderLayer as VisionTransformerEncoderLayer
-from .bricks import BuildNormalization, constructnormcfg, PatchEmbed, BuildDropout, truncnormal
+from .bricks import BuildNormalization, PatchEmbed, BuildDropout, truncnormal
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'beit_base_patch16_224_pt22k_ft22k': 'https://conversationhub.blob.core.windows.net/beit-share-public/beit/beit_base_patch16_224_pt22k_ft22k.pth',
     'beit_large_patch16_224_pt22k_ft22k': 'https://conversationhub.blob.core.windows.net/beit-share-public/beit/beit_large_patch16_224_pt22k_ft22k.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {
+    'beit_base_patch16_224_pt22k_ft22k': {},
+    'beit_large_patch16_224_pt22k_ft22k': {
+        'embed_dims': 1024, 'num_layers': 24, 'num_heads': 16, 'mlp_ratio': 4,
+        'qv_bias': True, 'init_values': 1e-6, 'drop_path_rate': 0.2, 'out_indices': [7, 11, 15, 23]
+    },
+}
 
 
 '''BEiTAttention'''
 class BEiTAttention(nn.Module):
     def __init__(self, embed_dims, num_heads, window_size, bias='qv_bias', qk_scale=None, attn_drop_rate=0., proj_drop_rate=0.):
         super(BEiTAttention, self).__init__()
         self.embed_dims = embed_dims
@@ -104,15 +112,15 @@
     def __init__(self, embed_dims, num_heads, feedforward_channels, attn_drop_rate=0., drop_path_rate=0., num_fcs=2, bias='qv_bias', 
                  act_cfg=None, norm_cfg=None, window_size=None, attn_cfg=dict(), ffn_cfg=dict(add_identity=False), init_values=None):
         super(BEiTTransformerEncoderLayer, self).__init__(
             embed_dims=embed_dims, num_heads=num_heads, feedforward_channels=feedforward_channels, attn_drop_rate=attn_drop_rate,
             drop_path_rate=0., drop_rate=0., num_fcs=num_fcs, qkv_bias=bias, act_cfg=act_cfg, norm_cfg=norm_cfg, attn_cfg=dict(), 
             ffn_cfg=ffn_cfg
         )
-        dropout_cfg = dict(type='droppath', drop_prob=drop_path_rate)
+        dropout_cfg = dict(type='DropPath', drop_prob=drop_path_rate)
         self.drop_path = BuildDropout(dropout_cfg) if dropout_cfg else nn.Identity()
         self.gamma_1 = nn.Parameter(init_values * torch.ones((embed_dims)), requires_grad=True)
         self.gamma_2 = nn.Parameter(init_values * torch.ones((embed_dims)), requires_grad=True)
         attn_cfg.update(dict(
             window_size=window_size,
             qk_scale=None,
             embed_dims=embed_dims,
@@ -127,52 +135,63 @@
         x = x + self.drop_path(self.gamma_1 * self.attn(self.ln1(x)))
         x = x + self.drop_path(self.gamma_2 * self.ffn(self.ln2(x)))
         return x
 
 
 '''BEiT'''
 class BEiT(nn.Module):
-    def __init__(self, img_size=224, patch_size=16, in_channels=3, embed_dims=768, num_layers=12, num_heads=12, mlp_ratio=4,
-                 out_indices=-1, qv_bias=True, attn_drop_rate=0., drop_path_rate=0., norm_cfg=None, act_cfg=None, patch_norm=False,
-                 final_norm=False, num_fcs=2, init_values=0.1):
+    def __init__(self, structure_type, img_size=(640, 640), patch_size=16, in_channels=3, embed_dims=768, num_layers=12, num_heads=12, mlp_ratio=4,
+                 out_indices=(3, 5, 7, 11), qv_bias=True, attn_drop_rate=0., drop_path_rate=0.1, norm_cfg={'type': 'LayerNorm', 'eps': 1e-6}, 
+                 act_cfg={'type': 'GELU'}, patch_norm=False, final_norm=False, num_fcs=2, init_values=0.1, pretrained=True, pretrained_model_path=''):
         super(BEiT, self).__init__()
         img_size = img_size if isinstance(img_size, tuple) else (img_size, img_size)
-        # set attrs
-        self.in_channels = in_channels
+        # set attributes
+        self.structure_type = structure_type
         self.img_size = img_size
         self.patch_size = patch_size
-        self.num_layers = num_layers
+        self.in_channels = in_channels
         self.embed_dims = embed_dims
+        self.num_layers = num_layers
         self.num_heads = num_heads
         self.mlp_ratio = mlp_ratio
+        self.out_indices = out_indices
+        self.qv_bias = qv_bias
         self.attn_drop_rate = attn_drop_rate
         self.drop_path_rate = drop_path_rate
-        self.num_fcs = num_fcs
-        self.qv_bias = qv_bias
-        self.act_cfg = act_cfg
         self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
         self.patch_norm = patch_norm
+        self.final_norm = final_norm
+        self.num_fcs = num_fcs
         self.init_values = init_values
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
         self.window_size = (img_size[0] // patch_size, img_size[1] // patch_size)
         self.patch_shape = self.window_size
-        # define modules
-        self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dims))
-        self.buildpatchembedding()
-        self.buildlayers()
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         if isinstance(out_indices, int):
             if out_indices == -1:
                 out_indices = num_layers - 1
             self.out_indices = [out_indices]
         elif isinstance(out_indices, list) or isinstance(out_indices, tuple):
             self.out_indices = out_indices
         else:
             raise TypeError('out_indices must be type of int, list or tuple')
-        self.final_norm = final_norm
+        # set modules
+        self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dims))
+        self.buildpatchembedding()
+        self.buildlayers()
         if final_norm:
-            self.norm1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+            self.norm1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''buildpatchembedding'''
     def buildpatchembedding(self):
         self.patch_embed = PatchEmbed(
             in_channels=self.in_channels, embed_dims=self.embed_dims,
             kernel_size=self.patch_size, stride=self.patch_size, padding=0,
             norm_cfg=self.norm_cfg if self.patch_norm else None
         )
@@ -242,19 +261,19 @@
                     extra_tokens = rel_pos_bias[-num_extra_tokens:, :]
                     rel_pos_bias = rel_pos_bias[:-num_extra_tokens, :]
                     new_rel_pos_bias = self.geometricsequenceinterpolation(src_size, dst_size, rel_pos_bias, num_attn_heads)
                     new_rel_pos_bias = torch.cat((new_rel_pos_bias, extra_tokens), dim=0)
                     state_dict[key] = new_rel_pos_bias
         return state_dict
     '''initweights'''
-    def initweights(self, beit_type='beit_base_patch16_224_pt22k_ft22k', pretrained_model_path=''):
+    def initweights(self, structure_type='beit_base_patch16_224_pt22k_ft22k', pretrained_model_path=''):
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[beit_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         state_dict = self.beitconvert(state_dict)
@@ -295,59 +314,8 @@
                 if self.final_norm:
                     x = self.norm1(x)
             if i in self.out_indices:
                 out = x[:, 1:]
                 B, _, C = out.shape
                 out = out.reshape(B, hw_shape[0], hw_shape[1], C).permute(0, 3, 1, 2).contiguous()
                 outs.append(out)
-        return tuple(outs)
-
-
-'''BuildBEiT'''
-def BuildBEiT(beit_cfg):
-    # assert whether support
-    beit_type = beit_cfg.pop('type')
-    supported_beits = {
-        'beit_base_patch16_224_pt22k_ft22k': {},
-        'beit_large_patch16_224_pt22k_ft22k': {
-            'embed_dims': 1024, 'num_layers': 24, 'num_heads': 16, 'mlp_ratio': 4,
-            'qv_bias': True, 'init_values': 1e-6, 'drop_path_rate': 0.2, 'out_indices': [7, 11, 15, 23]
-        },
-    }
-    assert beit_type in supported_beits, 'unspport the beit_type %s' % beit_type
-    # parse cfg
-    default_cfg = {
-        'img_size': (640, 640), 
-        'patch_size': 16, 
-        'in_channels': 3, 
-        'embed_dims': 768, 
-        'num_layers': 12, 
-        'num_heads': 12, 
-        'mlp_ratio': 4,
-        'out_indices': (3, 5, 7, 11), 
-        'qv_bias': True, 
-        'attn_drop_rate': 0., 
-        'drop_path_rate': 0.1, 
-        'norm_cfg': {'type': 'layernorm', 'eps': 1e-6},
-        'act_cfg': {'type': 'gelu'},
-        'patch_norm': False,
-        'final_norm': False, 
-        'num_fcs': 2, 
-        'init_values': 0.1,
-        'pretrained': True,
-        'pretrained_model_path': '',
-    }
-    default_cfg.update(supported_beits[beit_type])
-    for key, value in beit_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain beit_cfg
-    beit_cfg = default_cfg.copy()
-    pretrained = beit_cfg.pop('pretrained')
-    pretrained_model_path = beit_cfg.pop('pretrained_model_path')
-    # obtain the instanced beit
-    model = BEiT(**beit_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(beit_type, pretrained_model_path)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bisenetv1.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bisenetv1.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,46 +5,48 @@
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Spatial Path to preserve the spatial size of the original input image and encode affluent spatial information'''
 class SpatialPath(nn.Module):
     def __init__(self, in_channels=3, num_channels_list=(64, 64, 64, 128), norm_cfg=None, act_cfg=None):
         super(SpatialPath, self).__init__()
         assert len(num_channels_list) == 4
         self.layers = []
         for idx in range(len(num_channels_list)):
             layer_name = f'layer{idx + 1}'
             self.layers.append(layer_name)
             if idx == 0:
                 conv = nn.Sequential(
                     nn.Conv2d(in_channels, num_channels_list[idx], kernel_size=7, stride=2, padding=3, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=num_channels_list[idx], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=num_channels_list[idx], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             elif idx == len(num_channels_list) - 1:
                 conv = nn.Sequential(
                     nn.Conv2d(num_channels_list[idx - 1], num_channels_list[idx], kernel_size=1, stride=1, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=num_channels_list[idx], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=num_channels_list[idx], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             else:
                 conv = nn.Sequential(
                     nn.Conv2d(num_channels_list[idx - 1], num_channels_list[idx], kernel_size=3, stride=2, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=num_channels_list[idx], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=num_channels_list[idx], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             self.add_module(layer_name, conv)
     '''forward'''
     def forward(self, x):
         for idx, layer_name in enumerate(self.layers):
             layer_stage = getattr(self, layer_name)
@@ -54,21 +56,21 @@
 
 '''Attention Refinement Module (ARM) to refine the features of each stage'''
 class AttentionRefinementModule(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None):
         super(AttentionRefinementModule, self).__init__()
         self.conv_layer = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.atten_conv_layer = nn.Sequential(
             nn.AdaptiveAvgPool2d((1, 1)),
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             nn.Sigmoid(),
         )
     '''forward'''
     def forward(self, x):
         x = self.conv_layer(x)
         x_atten = self.atten_conv_layer(x)
         x_out = x * x_atten
@@ -82,26 +84,26 @@
         assert len(context_channels_list) == 3
         if 'norm_cfg' not in backbone_cfg: backbone_cfg['norm_cfg'] = norm_cfg
         self.backbone_net = self.buildbackbone(backbone_cfg)
         self.arm16 = AttentionRefinementModule(context_channels_list[1], context_channels_list[0], norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.arm32 = AttentionRefinementModule(context_channels_list[2], context_channels_list[0], norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.conv_head32 = nn.Sequential(
             nn.Conv2d(context_channels_list[0], context_channels_list[0], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=context_channels_list[0], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=context_channels_list[0], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.conv_head16 = nn.Sequential(
             nn.Conv2d(context_channels_list[0], context_channels_list[0], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=context_channels_list[0], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=context_channels_list[0], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.gap_conv = nn.Sequential(
             nn.AdaptiveAvgPool2d((1, 1)),
             nn.Conv2d(context_channels_list[2], context_channels_list[0], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=context_channels_list[0], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=context_channels_list[0], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         x_4, x_8, x_16, x_32 = self.backbone_net(x)
         x_gap = self.gap_conv(x_32)
         x_32_arm = self.arm32(x_32)
@@ -111,35 +113,36 @@
         x_16_arm = self.arm16(x_16)
         x_16_sum = x_16_arm + x_32_up
         x_16_up = F.interpolate(input=x_16_sum, size=x_8.shape[2:], mode='nearest')
         x_16_up = self.conv_head16(x_16_up)
         return x_16_up, x_32_up
     '''build the backbone'''
     def buildbackbone(self, cfg):
-        from .resnet import BuildResNet
+        from .resnet import ResNet
         supported_backbones = {
-            'resnet': BuildResNet,
+            'ResNet': ResNet,
         }
-        assert cfg['series'] in supported_backbones, 'unsupport backbone type %s' % cfg['type']
-        return supported_backbones[cfg['series']](cfg)
+        backbone_type = cfg.pop('type')
+        assert backbone_type, f'unsupport backbone type {backbone_type}'
+        return supported_backbones[backbone_type](**cfg)
 
 
 '''Feature Fusion Module to fuse low level output feature of Spatial Path and high level output feature of Context Path'''
 class FeatureFusionModule(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None):
         super(FeatureFusionModule, self).__init__()
         self.conv1 = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.gap = nn.AdaptiveAvgPool2d((1, 1))
         self.conv_atten = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Sigmoid(),
         )
     '''forward'''
     def forward(self, x_sp, x_cp):
         x_concat = torch.cat([x_sp, x_cp], dim=1)
         x_fuse = self.conv1(x_concat)
@@ -148,72 +151,55 @@
         x_atten = x_fuse * x_atten
         x_out = x_atten + x_fuse
         return x_out
 
 
 '''BiSeNetV1'''
 class BiSeNetV1(nn.Module):
-    def __init__(self, backbone_cfg, in_channels=3, spatial_channels_list=(64, 64, 64, 128), context_channels_list=(128, 256, 512),
-                 out_indices=(0, 1, 2), out_channels=256, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, backbone_cfg=None, in_channels=3, spatial_channels_list=(64, 64, 64, 128), 
+                 context_channels_list=(128, 256, 512), out_indices=(0, 1, 2), out_channels=256, norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'ReLU', 'inplace': True}, pretrained=False, pretrained_model_path=''):
         super(BiSeNetV1, self).__init__()
         assert (len(spatial_channels_list) == 4) and (len(context_channels_list) == 3)
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
+        self.backbone_cfg = backbone_cfg
+        self.in_channels = in_channels
+        self.spatial_channels_list = spatial_channels_list
+        self.context_channels_list = context_channels_list
         self.out_indices = out_indices
+        self.out_channels = out_channels
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
-        # define modules
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # set modules
         self.context_path = ContextPath(backbone_cfg, context_channels_list, norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.spatial_path = SpatialPath(in_channels, spatial_channels_list, norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.ffm = FeatureFusionModule(context_channels_list[1], out_channels, norm_cfg=norm_cfg, act_cfg=act_cfg)
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         x_context8, x_context16 = self.context_path(x)
         x_spatial = self.spatial_path(x)
         x_fuse = self.ffm(x_spatial, x_context8)
         outs = [x_context8, x_context16, x_fuse]
         outs = [outs[i] for i in self.out_indices]
-        return tuple(outs)
-
-
-'''BuildBiSeNetV1'''
-def BuildBiSeNetV1(bisenetv1_cfg):
-    # assert whether support
-    bisenetv1_type = bisenetv1_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'backbone_cfg': None,
-        'in_channels': 3, 
-        'spatial_channels_list': (64, 64, 64, 128),
-        'context_channels_list': (128, 256, 512),
-        'out_indices': (0, 1, 2),
-        'out_channels': 256,
-        'norm_cfg': None, 
-        'act_cfg': {'type': 'relu', 'inplace': True},
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in bisenetv1_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain bisenetv1_cfg
-    bisenetv1_cfg = default_cfg.copy()
-    pretrained = bisenetv1_cfg.pop('pretrained')
-    pretrained_model_path = bisenetv1_cfg.pop('pretrained_model_path')
-    # obtain the instanced bisenetv1
-    model = BiSeNetV1(**bisenetv1_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[bisenetv1_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bisenetv2.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bisenetv2.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,46 +5,48 @@
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, DepthwiseSeparableConv2d, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation, DepthwiseSeparableConv2d
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Detail Branch with wide channels and shallow layers to capture low-level details and generate high-resolution feature representation'''
 class DetailBranch(nn.Module):
     def __init__(self, detail_channels=(64, 64, 128), in_channels=3, norm_cfg=None, act_cfg=None):
         super(DetailBranch, self).__init__()
         detail_branch = []
         for i in range(len(detail_channels)):
             if i == 0:
                 detail_branch.append(nn.Sequential(
                     nn.Conv2d(in_channels, detail_channels[i], kernel_size=3, stride=2, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=detail_channels[i], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=detail_channels[i], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                     nn.Conv2d(detail_channels[i], detail_channels[i], kernel_size=3, stride=1, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=detail_channels[i], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=detail_channels[i], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 ))
             else:
                 detail_branch.append(nn.Sequential(
                     nn.Conv2d(detail_channels[i - 1], detail_channels[i], kernel_size=3, stride=2, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=detail_channels[i], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=detail_channels[i], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                     nn.Conv2d(detail_channels[i], detail_channels[i], kernel_size=3, stride=1, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=detail_channels[i], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=detail_channels[i], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                     nn.Conv2d(detail_channels[i], detail_channels[i], kernel_size=3, stride=1, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=detail_channels[i], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=detail_channels[i], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 ))
         self.detail_branch = nn.ModuleList(detail_branch)
     '''forward'''
     def forward(self, x):
         for stage in self.detail_branch:
             x = stage(x)
@@ -53,29 +55,29 @@
 
 '''Stem Block at the beginning of Semantic Branch'''
 class StemBlock(nn.Module):
     def __init__(self, in_channels=3, out_channels=16, norm_cfg=None, act_cfg=None):
         super(StemBlock, self).__init__()
         self.conv_first = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.convs = nn.Sequential(
             nn.Conv2d(out_channels, out_channels // 2, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels//2, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels//2, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(out_channels // 2, out_channels, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.pool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1, ceil_mode=False)
         self.fuse_last = nn.Sequential(
             nn.Conv2d(out_channels * 2, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         x = self.conv_first(x)
         x_left = self.convs(x)
         x_right = self.pool(x)
@@ -86,30 +88,30 @@
 '''Gather-and-Expansion Layer'''
 class GELayer(nn.Module):
     def __init__(self, in_channels, out_channels, exp_ratio=6, stride=1, norm_cfg=None, act_cfg=None):
         super(GELayer, self).__init__()
         mid_channel = in_channels * exp_ratio
         self.conv1 = nn.Sequential(
             nn.Conv2d(in_channels, in_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         if stride == 1:
             self.dwconv = nn.Sequential(
                 nn.Conv2d(in_channels, mid_channel, kernel_size=3, stride=stride, padding=1, groups=in_channels, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=mid_channel, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=mid_channel, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.shortcut = None
         else:
             self.dwconv = nn.Sequential(
                 nn.Conv2d(in_channels, mid_channel, kernel_size=3, stride=stride, padding=1, groups=in_channels, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=mid_channel, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=mid_channel, norm_cfg=norm_cfg),
                 nn.Conv2d(mid_channel, mid_channel, kernel_size=3, stride=1, padding=1, groups=mid_channel, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=mid_channel, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=mid_channel, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.shortcut = nn.Sequential(DepthwiseSeparableConv2d(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=3,
                 stride=stride,
@@ -117,15 +119,15 @@
                 dw_norm_cfg=norm_cfg,
                 dw_act_cfg=None,
                 pw_norm_cfg=norm_cfg,
                 pw_act_cfg=None,
             ))
         self.conv2 = nn.Sequential(
             nn.Conv2d(mid_channel, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
         )
         self.act = BuildActivation(act_cfg)
     '''forward'''
     def forward(self, x):
         identity = x
         x = self.conv1(x)
         x = self.dwconv(x)
@@ -145,37 +147,37 @@
         super(CEBlock, self).__init__()
         # set attrs
         self.in_channels = in_channels
         self.out_channels = out_channels
         # define modules
         self.gap = nn.Sequential(
             nn.AdaptiveAvgPool2d((1, 1)),
-            BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg),
         )
         self.conv_gap = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.conv_last = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         identity = x
         x = self.gap(x)
         x = self.conv_gap(x)
         x = identity + x
         x = self.conv_last(x)
         return x
 
 
-'''Semantic Branch which is lightweight with narrow channels and deep layers to obtain　high-level semantic context'''
+'''Semantic Branch which is lightweight with narrow channels and deep layers to obtain high-level semantic context'''
 class SemanticBranch(nn.Module):
     def __init__(self, semantic_channels=(16, 32, 64, 128), in_channels=3, exp_ratio=6, norm_cfg=None, act_cfg=None):
         super(SemanticBranch, self).__init__()
         # set attrs
         self.in_channels = in_channels
         self.semantic_channels = semantic_channels
         self.semantic_stages = []
@@ -235,35 +237,35 @@
             dw_norm_cfg=norm_cfg,
             dw_act_cfg=None,
             pw_norm_cfg=None,
             pw_act_cfg=None,
         ))
         self.detail_down = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             nn.AvgPool2d(kernel_size=3, stride=2, padding=1, ceil_mode=False),
         )
         self.semantic_conv = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
         )
         self.semantic_dwconv = nn.Sequential(DepthwiseSeparableConv2d(
             in_channels=out_channels,
             out_channels=out_channels,
             kernel_size=3,
             stride=1,
             padding=1,
             dw_norm_cfg=norm_cfg,
             dw_act_cfg=None,
             pw_norm_cfg=None,
             pw_act_cfg=None,
         ))
         self.conv = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x_d, x_s):
         detail_dwconv = self.detail_dwconv(x_d)
         detail_down = self.detail_down(x_d)
         semantic_conv = self.semantic_conv(x_s)
@@ -278,78 +280,55 @@
         )
         output = self.conv(fuse_1 + fuse_2)
         return output
 
 
 '''BiSeNetV2: Bilateral Network with Guided Aggregation for Real-time Semantic Segmentation'''
 class BiSeNetV2(nn.Module):
-    def __init__(self, in_channels=3, detail_channels=(64, 64, 128), semantic_channels=(16, 32, 64, 128), semantic_expansion_ratio=6,
-                 bga_channels=128, out_indices=(0, 1, 2, 3, 4), align_corners=False, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, detail_channels=(64, 64, 128), semantic_channels=(16, 32, 64, 128), 
+                 semantic_expansion_ratio=6, bga_channels=128, out_indices=(0, 1, 2, 3, 4), align_corners=False, norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'ReLU', 'inplace': True}, pretrained=False, pretrained_model_path=''):
         super(BiSeNetV2, self).__init__()
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
         self.in_channels = in_channels
         self.out_indices = out_indices
         self.detail_channels = detail_channels
         self.semantic_channels = semantic_channels
         self.semantic_expansion_ratio = semantic_expansion_ratio
         self.bga_channels = bga_channels
         self.align_corners = align_corners
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
-        # define modules
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # set modules
         self.detail = DetailBranch(self.detail_channels, self.in_channels, norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.semantic = SemanticBranch(self.semantic_channels, self.in_channels, self.semantic_expansion_ratio, norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.bga = BGALayer(self.bga_channels, self.align_corners, norm_cfg=norm_cfg, act_cfg=act_cfg)
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         x_detail = self.detail(x)
         x_semantic_lst = self.semantic(x)
         x_head = self.bga(x_detail, x_semantic_lst[-1])
         outs = x_semantic_lst[:-1] + [x_head]
         outs = [outs[i] for i in self.out_indices]
-        return tuple(outs)
-
-
-'''BuildBiSeNetV2'''
-def BuildBiSeNetV2(bisenetv2_cfg):
-    # assert whether support
-    bisenetv2_type = bisenetv2_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3, 
-        'detail_channels': (64, 64, 128), 
-        'semantic_channels': (16, 32, 64, 128), 
-        'semantic_expansion_ratio': 6,
-        'bga_channels': 128, 
-        'out_indices': (0, 1, 2, 3, 4), 
-        'align_corners': False, 
-        'norm_cfg': None, 
-        'act_cfg': {'type': 'relu', 'inplace': True},
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in bisenetv2_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain bisenetv2_cfg
-    bisenetv2_cfg = default_cfg.copy()
-    pretrained = bisenetv2_cfg.pop('pretrained')
-    pretrained_model_path = bisenetv2_cfg.pop('pretrained_model_path')
-    # obtain the instanced bisenetv2
-    model = BiSeNetV2(**bisenetv2_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[bisenetv2_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return tuple(outs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/activation/hardsigmoid.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/activation/hardsigmoid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define the Hard Sigmoid Module
+    Implementation of HardSigmoid
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/apconv.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/apconv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Function:
-    Define Adptive Padding Conv Module
+    Implementation of AdptivePaddingConv2d
 Author:
     Zhenchao Jin
 '''
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..normalization import BuildNormalization, constructnormcfg
+from ..normalization import BuildNormalization
 
 
 '''AdptivePaddingConv2d'''
 class AdptivePaddingConv2d(nn.Conv2d):
     def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, groups=1, bias=True, norm_cfg=None, act_cfg=None):
         super(AdptivePaddingConv2d, self).__init__(
             in_channels=in_channels, 
@@ -21,15 +21,15 @@
             stride=stride, 
             padding=0,
             dilation=dilation, 
             groups=groups, 
             bias=bias
         )
         if norm_cfg is not None: 
-            self.norm = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg))
+            self.norm = BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg)
         if act_cfg is not None: 
             self.activation = BuildActivation(act_cfg)
     '''forward'''
     def forward(self, x):
         img_h, img_w = x.size()[-2:]
         kernel_h, kernel_w = self.weight.size()[-2:]
         stride_h, stride_w = self.stride
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/dsconv.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/dsconv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 '''
 Function:
-    Define Depthwise Separable Convolution Module
+    Implementation of DepthwiseSeparableConv2d
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..activation import BuildActivation
-from ..normalization import BuildNormalization, constructnormcfg
+from ..normalization import BuildNormalization
 
 
 '''DepthwiseSeparableConv2d'''
 class DepthwiseSeparableConv2d(nn.Module):
     def __init__(self, in_channels, out_channels, kernel_size=3, stride=1, padding=1, dilation=1, bias=False, 
                  norm_cfg=None, act_cfg=None, dw_norm_cfg=None, dw_act_cfg=None, pw_norm_cfg=None, pw_act_cfg=None):
         super(DepthwiseSeparableConv2d, self).__init__()
         if dw_norm_cfg is None: dw_norm_cfg = norm_cfg
         if dw_act_cfg is None: dw_act_cfg = act_cfg
         if pw_norm_cfg is None: pw_norm_cfg = norm_cfg
         if pw_act_cfg is None: pw_act_cfg = act_cfg
         self.depthwise_conv = nn.Conv2d(in_channels, in_channels, kernel_size=kernel_size, stride=stride, padding=padding, dilation=dilation, groups=in_channels, bias=bias)
         if dw_norm_cfg is not None:
-            self.depthwise_bn = BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=dw_norm_cfg))
+            self.depthwise_bn = BuildNormalization(placeholder=in_channels, norm_cfg=dw_norm_cfg)
         if dw_act_cfg is not None:
             self.depthwise_activate = BuildActivation(dw_act_cfg)
         self.pointwise_conv = nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=1, groups=1, bias=bias)
         if pw_norm_cfg is not None:
-            self.pointwise_bn = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=pw_norm_cfg))
+            self.pointwise_bn = BuildNormalization(placeholder=out_channels, norm_cfg=pw_norm_cfg)
         if pw_act_cfg is not None:
             self.pointwise_activate = BuildActivation(pw_act_cfg)
     '''forward'''
     def forward(self, x):
         x = self.depthwise_conv(x)
         if hasattr(self, 'depthwise_bn'): x = self.depthwise_bn(x)
         if hasattr(self, 'depthwise_activate'): x = self.depthwise_activate(x)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/dyconv.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/dyconv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Function:
-    Define the dynamic conv2d
+    Implementation of DynamicConv2d
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..activation import BuildActivation
-from ..normalization import BuildNormalization, constructnormcfg
+from ..normalization import BuildNormalization
 
 
 '''Attention2d'''
 class Attention2d(nn.Module):
     def __init__(self, in_channels, out_channels, temperature):
         super(Attention2d, self).__init__()
         assert temperature % 3 == 1
@@ -53,15 +53,15 @@
         self.act_cfg = act_cfg
         # define modules
         self.attention = Attention2d(in_channels, K, temperature)
         self.weight = nn.Parameter(torch.randn(K, out_channels, in_channels//groups, kernel_size, kernel_size), requires_grad=True)
         if bias:
             self.bias = nn.Parameter(torch.randn(K, out_channels))
         if norm_cfg is not None: 
-            self.norm = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg))
+            self.norm = BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg)
         if act_cfg is not None: 
             self.activation = BuildActivation(act_cfg)
     '''update'''
     def update(self):
         self.attention.update()
     '''forward'''
     def forward(self, x):
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/irconv.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/irconv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 '''
 Function:
-    Define InvertedResidual Module
+    Implementation of InvertedResidual and InvertedResidualV3
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..activation import BuildActivation
 from .apconv import AdptivePaddingConv2d
 from .seconv import SqueezeExcitationConv2d
-from ..normalization import BuildNormalization, constructnormcfg
+from ..normalization import BuildNormalization
 
 
 '''InvertedResidual'''
 class InvertedResidual(nn.Module):
     def __init__(self, in_channels, out_channels, stride, expand_ratio, dilation=1, norm_cfg=None, act_cfg=None):
         super(InvertedResidual, self).__init__()
         assert stride in [1, 2], 'stride must in [1, 2], but received %s' % stride
         self.use_res_connect = stride == 1 and in_channels == out_channels
         hidden_dim = int(round(in_channels * expand_ratio))
         layers = []
         if expand_ratio != 1:
             layer = nn.Sequential()
             layer.add_module('conv', nn.Conv2d(in_channels, hidden_dim, kernel_size=1, stride=1, padding=0, bias=False))
             if norm_cfg is not None:
-                layer.add_module('bn', BuildNormalization(constructnormcfg(placeholder=hidden_dim, norm_cfg=norm_cfg)))
+                layer.add_module('bn', BuildNormalization(placeholder=hidden_dim, norm_cfg=norm_cfg))
             if act_cfg is not None:
                 layer.add_module('activation', BuildActivation(act_cfg))
             layers.append(layer)
         layer = nn.Sequential()
         layer.add_module('conv', nn.Conv2d(hidden_dim, hidden_dim, kernel_size=3, stride=stride, padding=dilation, dilation=dilation, groups=hidden_dim, bias=False))
         if norm_cfg is not None:
-            layer.add_module('bn', BuildNormalization(constructnormcfg(placeholder=hidden_dim, norm_cfg=norm_cfg)))
+            layer.add_module('bn', BuildNormalization(placeholder=hidden_dim, norm_cfg=norm_cfg))
         if act_cfg is not None:
             layer.add_module('activation', BuildActivation(act_cfg))
         layers.extend([layer])
         layer = nn.Sequential()
         layer.add_module('conv', nn.Conv2d(hidden_dim, out_channels, kernel_size=1, stride=1, padding=0, bias=False))
         if norm_cfg is not None:
-            layer.add_module('bn', BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)))
+            layer.add_module('bn', BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg))
         layers.extend([layer])
         self.conv = nn.Sequential(*layers)
     '''forward'''
     def forward(self, x):
         if self.use_res_connect:
             return x + self.conv(x)
         else:
@@ -57,36 +57,36 @@
         self.with_res_shortcut = (stride == 1 and in_channels == out_channels)
         self.with_expand_conv = with_expand_conv
         if not self.with_expand_conv: assert mid_channels == in_channels
         if self.with_expand_conv:
             self.expand_conv = nn.Sequential()
             self.expand_conv.add_module('conv', nn.Conv2d(in_channels, mid_channels, kernel_size=1, stride=1, padding=0, bias=False))
             if norm_cfg is not None:
-                self.expand_conv.add_module('bn', BuildNormalization(constructnormcfg(placeholder=mid_channels, norm_cfg=norm_cfg)))
+                self.expand_conv.add_module('bn', BuildNormalization(placeholder=mid_channels, norm_cfg=norm_cfg))
             if act_cfg is not None:
                 self.expand_conv.add_module('activation', BuildActivation(act_cfg))
         self.depthwise_conv = nn.Sequential()
         if stride == 2:
             self.depthwise_conv.add_module('conv', AdptivePaddingConv2d(mid_channels, mid_channels, kernel_size=kernel_size, stride=stride, padding=kernel_size//2, groups=mid_channels, bias=False))
             if norm_cfg is not None:
-                self.depthwise_conv.add_module('bn', BuildNormalization(constructnormcfg(placeholder=mid_channels, norm_cfg=norm_cfg)))
+                self.depthwise_conv.add_module('bn', BuildNormalization(placeholder=mid_channels, norm_cfg=norm_cfg))
             if act_cfg is not None:
                 self.depthwise_conv.add_module('activation', BuildActivation(act_cfg))
         else:
             self.depthwise_conv.add_module('conv', nn.Conv2d(mid_channels, mid_channels, kernel_size=kernel_size, stride=stride, padding=kernel_size//2, groups=mid_channels, bias=False))
             if norm_cfg is not None:
-                self.depthwise_conv.add_module('bn', BuildNormalization(constructnormcfg(placeholder=mid_channels, norm_cfg=norm_cfg)))
+                self.depthwise_conv.add_module('bn', BuildNormalization(placeholder=mid_channels, norm_cfg=norm_cfg))
             if act_cfg is not None:
                 self.depthwise_conv.add_module('activation', BuildActivation(act_cfg))
         if se_cfg is not None:
             self.se = SqueezeExcitationConv2d(**se_cfg)
         self.linear_conv = nn.Sequential()
         self.linear_conv.add_module('conv', nn.Conv2d(mid_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False))
         if norm_cfg is not None:
-            self.linear_conv.add_module('bn', BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)))
+            self.linear_conv.add_module('bn', BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg))
     '''forward'''
     def forward(self, x):
         out = x
         if self.with_expand_conv: out = self.expand_conv(out)
         out = self.depthwise_conv(out)
         if hasattr(self, 'se'): out = self.se(out)
         out = self.linear_conv(out)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/convolution/seconv.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/convolution/seconv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define the Squeeze-and-Excitation Module
+    Implementation of SqueezeExcitationConv2d
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..misc import makedivisible
 from ..activation import BuildActivation
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/dropout/droppath.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/dropout/droppath.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define drop path
+    Implementation of DropPath
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/l2norm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/l2norm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define the l2norm
+    Implementation of L2Norm
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/misc/weightinit.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/misc/weightinit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define weight initialize
+    Implementation of weight initialization methods
 Author:
     Zhenchao Jin
 '''
 import math
 import torch
 import warnings
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/embed.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Function:
-    Patch Embedding or Merging
+    Implementation of AdaptivePadding, PatchEmbed and PatchMerging
 Author:
     Zhenchao Jin
 '''
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..normalization import BuildNormalization, constructnormcfg
+from ..normalization import BuildNormalization
 
 
 '''AdaptivePadding'''
 class AdaptivePadding(nn.Module):
     def __init__(self, kernel_size=1, stride=1, dilation=1, padding='corner'):
         super(AdaptivePadding, self).__init__()
         assert padding in ('same', 'corner')
@@ -64,15 +64,15 @@
             padding = 0
         # projection
         padding = AdaptivePadding.totuple(padding)
         self.projection = nn.Conv2d(in_channels, embed_dims, kernel_size=kernel_size, stride=stride, padding=padding, bias=bias, dilation=dilation)
         # norm
         self.norm = None
         if norm_cfg is not None: 
-            self.norm = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+            self.norm = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         # input size
         self.init_input_size = None
         self.init_out_size = None
         if input_size:
             input_size = AdaptivePadding.totuple(input_size)
             self.init_input_size = input_size
             if self.adap_padding:
@@ -114,15 +114,15 @@
         # sampler
         padding = AdaptivePadding.totuple(padding)
         self.sampler = nn.Unfold(kernel_size=kernel_size, dilation=dilation, padding=padding, stride=stride)
         # norm
         sample_dim = kernel_size[0] * kernel_size[1] * in_channels
         self.norm = None
         if norm_cfg is not None: 
-            self.norm = BuildNormalization(constructnormcfg(placeholder=sample_dim, norm_cfg=norm_cfg))
+            self.norm = BuildNormalization(placeholder=sample_dim, norm_cfg=norm_cfg)
         # reduction
         self.reduction = nn.Linear(sample_dim, out_channels, bias=bias)
     '''forward'''
     def forward(self, x, input_size):
         B, L, C = x.shape
         H, W = input_size
         assert L == H * W, 'input feature has wrong size'
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/ffn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/ffn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define feed-forward networks (FFNs) with identity connection
+    Implementation of FFN
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..dropout import BuildDropout
 from ..activation import BuildActivation
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/mha.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/mha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Multi-head Attention Module
+    Implementation of MultiheadAttention
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..dropout import BuildDropout
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/bricks/transformer/misc.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/bricks/transformer/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define some utils used in transformer backbones
+    Implementation of some utils for transformer backbones
 Author:
     Zhenchao Jin
 '''
 import torch
 
 
 '''nlctonchw'''
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/cgnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/cgnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 Author:
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Global Context Extractor for CGNet'''
 class GlobalContextExtractor(nn.Module):
     def __init__(self, channels, reduction=16):
         super(GlobalContextExtractor, self).__init__()
         assert reduction >= 1 and channels >= reduction
@@ -41,28 +43,28 @@
 class ContextGuidedBlock(nn.Module):
     def __init__(self, in_channels, out_channels, dilation=2, reduction=16, skip_connect=True, downsample=False, norm_cfg=None, act_cfg=None):
         super(ContextGuidedBlock, self).__init__()
         # set attrs
         self.downsample = downsample
         self.skip_connect = skip_connect and not downsample
         channels = out_channels if downsample else out_channels // 2
-        if 'type' in act_cfg and act_cfg['type'] == 'prelu':
+        if 'type' in act_cfg and act_cfg['type'] == 'PReLU':
             act_cfg['num_parameters'] = channels
         kernel_size = 3 if downsample else 1
         stride = 2 if downsample else 1
         padding = (kernel_size - 1) // 2
         # instance modules
         self.conv1x1 = nn.Sequential(
             nn.Conv2d(in_channels, channels, kernel_size=kernel_size, stride=stride, padding=padding, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.f_loc = nn.Conv2d(channels, channels, kernel_size=3, stride=1, padding=1, groups=channels, bias=False)
         self.f_sur = nn.Conv2d(channels, channels, kernel_size=3, stride=1, padding=dilation, dilation=dilation, groups=channels, bias=False)
-        self.bn = BuildNormalization(constructnormcfg(placeholder=channels * 2, norm_cfg=norm_cfg))
+        self.bn = BuildNormalization(placeholder=channels * 2, norm_cfg=norm_cfg)
         self.activate = nn.PReLU(2 * channels)
         if downsample:
             self.bottleneck = nn.Conv2d(2 * channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False)
         self.f_glo = GlobalContextExtractor(out_channels, reduction)
     '''forward'''
     def forward(self, x):
         out = self.conv1x1(x)
@@ -91,49 +93,56 @@
         for pool in self.pools:
             x = pool(x)
         return x
 
 
 '''CGNet'''
 class CGNet(nn.Module):
-    def __init__(self, in_channels=3, num_channels=(32, 64, 128), num_blocks=(3, 21), dilations=(2, 4), reductions=(8, 16), norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, num_channels=(32, 64, 128), num_blocks=(3, 21), dilations=(2, 4), reductions=(8, 16), 
+                 norm_cfg={'type': 'SyncBatchNorm'}, act_cfg={'type': 'PReLU'}, pretrained=False, pretrained_model_path=''):
         super(CGNet, self).__init__()
-        # assert
-        assert isinstance(num_channels, tuple) and len(num_channels) == 3
-        assert isinstance(num_blocks, tuple) and len(num_blocks) == 2
-        assert isinstance(dilations, tuple) and len(dilations) == 2
-        assert isinstance(reductions, tuple) and len(reductions) == 2
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
         self.in_channels = in_channels
         self.num_channels = num_channels
         self.num_blocks = num_blocks
         self.dilations = dilations
         self.reductions = reductions
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
-        if 'type' in self.act_cfg and self.act_cfg['type'] == 'prelu':
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        if 'type' in self.act_cfg and self.act_cfg['type'] == 'PReLU':
             self.act_cfg['num_parameters'] = num_channels[0]
+        # assert
+        assert isinstance(num_channels, tuple) and len(num_channels) == 3
+        assert isinstance(num_blocks, tuple) and len(num_blocks) == 2
+        assert isinstance(dilations, tuple) and len(dilations) == 2
+        assert isinstance(reductions, tuple) and len(reductions) == 2
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # stem
         cur_channels = in_channels
         self.stem = nn.ModuleList()
         for i in range(3):
             self.stem.append(nn.Sequential(
                 nn.Conv2d(cur_channels, num_channels[0], kernel_size=3, stride=2 if i == 0 else 1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=num_channels[0], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=num_channels[0], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
             cur_channels = num_channels[0]
         # down-sample for Input, factor=2
         self.inject_2x = InputInjection(1)
         # down-sample for Input, factor=4
         self.inject_4x = InputInjection(2)
         # norm prelu
         cur_channels += in_channels
         self.norm_prelu_0 = nn.Sequential(
-            BuildNormalization(constructnormcfg(placeholder=cur_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=cur_channels, norm_cfg=norm_cfg),
             nn.PReLU(cur_channels),
         )
         # stage 1
         self.level1 = nn.ModuleList()
         for i in range(num_blocks[0]):
             self.level1.append(ContextGuidedBlock(
                 in_channels=cur_channels if i == 0 else num_channels[1], 
@@ -143,15 +152,15 @@
                 skip_connect=True, 
                 downsample=(i == 0), 
                 norm_cfg=norm_cfg, 
                 act_cfg=act_cfg,
             ))
         cur_channels = 2 * num_channels[1] + in_channels
         self.norm_prelu_1 = nn.Sequential(
-            BuildNormalization(constructnormcfg(placeholder=cur_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=cur_channels, norm_cfg=norm_cfg),
             nn.PReLU(cur_channels),
         )
         # stage 2
         self.level2 = nn.ModuleList()
         for i in range(num_blocks[1]):
             self.level2.append(ContextGuidedBlock(
                 in_channels=cur_channels if i == 0 else num_channels[2],
@@ -161,17 +170,32 @@
                 skip_connect=True, 
                 downsample=(i == 0), 
                 norm_cfg=norm_cfg, 
                 act_cfg=act_cfg,
             ))
         cur_channels = 2 * num_channels[2]
         self.norm_prelu_2 = nn.Sequential(
-            BuildNormalization(constructnormcfg(placeholder=cur_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=cur_channels, norm_cfg=norm_cfg),
             nn.PReLU(cur_channels),
         )
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         output = []
         # stage 0
         inp_2x = self.inject_2x(x)
         inp_4x = self.inject_4x(x)
         for layer in self.stem:
@@ -187,52 +211,8 @@
         # stage 2
         for i, layer in enumerate(self.level2):
             x = layer(x)
             if i == 0: down2 = x
         x = self.norm_prelu_2(torch.cat([down2, x], 1))
         output.append(x)
         # return
-        return output
-
-
-'''BuildCGNet'''
-def BuildCGNet(cgnet_cfg):
-    # assert whether support
-    cgnet_type = cgnet_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3, 
-        'num_channels': (32, 64, 128), 
-        'num_blocks': (3, 21), 
-        'dilations': (2, 4), 
-        'reductions': (8, 16), 
-        'norm_cfg': None, 
-        'act_cfg': {'type': 'prelu'},
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in cgnet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain cgnet_cfg
-    cgnet_cfg = default_cfg.copy()
-    pretrained = cgnet_cfg.pop('pretrained')
-    pretrained_model_path = cgnet_cfg.pop('pretrained_model_path')
-    # obtain the instanced cgnet
-    model = CGNet(**cgnet_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[cgnet_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return output
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/convnext.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/convnext.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,54 +7,38 @@
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 from functools import partial
 from .bricks.dropout.droppath import DropPath
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
+from .bricks.normalization.layernorm2d import LayerNorm2d
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'convnext_tiny': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-tiny_3rdparty_32xb128-noema_in1k_20220301-795e9634.pth',
     'convnext_small': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-small_3rdparty_32xb128-noema_in1k_20220301-303e75e3.pth',
     'convnext_base': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-base_3rdparty_32xb128-noema_in1k_20220301-2a0ee547.pth',
     'convnext_base_21k': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-base_3rdparty_in21k_20220301-262fd037.pth',
     'convnext_large_21k': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-large_3rdparty_in21k_20220301-e6e0ea0a.pth',
     'convnext_xlarge_21k': 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-xlarge_3rdparty_in21k_20220301-08aa5ddc.pth',
 }
-
-
-'''LayerNorm2d'''
-class LayerNorm2d(nn.LayerNorm):
-    def __init__(self, num_channels, **kwargs):
-        super(LayerNorm2d, self).__init__(num_channels, **kwargs)
-        self.num_channels = self.normalized_shape[0]
-    '''forward'''
-    def forward(self, x):
-        assert x.dim() == 4, f'LayerNorm2d only supports inputs with shape (N, C, H, W), but got tensor with shape {x.shape}'
-        x = F.layer_norm(
-            x.permute(0, 2, 3, 1), self.normalized_shape, self.weight, self.bias, self.eps
-        ).permute(0, 3, 1, 2)
-        return x
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''ConvNeXtBlock'''
 class ConvNeXtBlock(nn.Module):
     def __init__(self, in_channels, norm_cfg=None, act_cfg=None, mlp_ratio=4., linear_pw_conv=True, drop_path_rate=0., layer_scale_init_value=1e-6):
         super(ConvNeXtBlock, self).__init__()
         self.depthwise_conv = nn.Conv2d(in_channels, in_channels, kernel_size=7, padding=3, groups=in_channels)
         self.linear_pw_conv = linear_pw_conv
-        if norm_cfg['type'] in ['layernorm2d']:
-            norm_cfg_copy = copy.deepcopy(norm_cfg)
-            norm_cfg_copy.pop('type')
-            self.norm = LayerNorm2d(num_channels=in_channels, **norm_cfg_copy)
-        else:
-            self.norm = BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg))
+        self.norm = BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg)
         mid_channels = int(mlp_ratio * in_channels)
         if self.linear_pw_conv:
             pw_conv = nn.Linear
         else:
             pw_conv = partial(nn.Conv2d, kernel_size=1)
         self.pointwise_conv1 = pw_conv(in_channels, mid_channels)
         self.act = BuildActivation(act_cfg)
@@ -80,55 +64,57 @@
         x = shortcut + self.drop_path(x)
         return x
 
 
 '''ConvNeXt'''
 class ConvNeXt(nn.Module):
     arch_settings = {
-        'tiny': {
-            'depths': [3, 3, 9, 3], 'channels': [96, 192, 384, 768]
-        },
-        'small': {
-            'depths': [3, 3, 27, 3], 'channels': [96, 192, 384, 768]
-        },
-        'base': {
-            'depths': [3, 3, 27, 3], 'channels': [128, 256, 512, 1024]
-        },
-        'large': {
-            'depths': [3, 3, 27, 3], 'channels': [192, 384, 768, 1536]
-        },
-        'xlarge': {
-            'depths': [3, 3, 27, 3], 'channels': [256, 512, 1024, 2048]
-        },
+        'tiny': {'depths': [3, 3, 9, 3], 'channels': [96, 192, 384, 768]},
+        'small': {'depths': [3, 3, 27, 3], 'channels': [96, 192, 384, 768]},
+        'base': {'depths': [3, 3, 27, 3], 'channels': [128, 256, 512, 1024]},
+        'large': {'depths': [3, 3, 27, 3], 'channels': [192, 384, 768, 1536]},
+        'xlarge': {'depths': [3, 3, 27, 3], 'channels': [256, 512, 1024, 2048]},
     }
-    def __init__(self, arch='tiny', in_channels=3, stem_patch_size=4, norm_cfg=None, act_cfg=None, linear_pw_conv=True,
-                 drop_path_rate=0., layer_scale_init_value=1e-6, out_indices=-1, gap_before_final_norm=True):
+    def __init__(self, structure_type, arch='tiny', in_channels=3, stem_patch_size=4, norm_cfg={'type': 'LayerNorm2d', 'eps': 1e-6}, act_cfg={'type': 'GELU'},
+                 linear_pw_conv=True, drop_path_rate=0., layer_scale_init_value=1e-6, out_indices=(0, 1, 2, 3), gap_before_final_norm=True,
+                 pretrained=True, pretrained_model_path=''):
         super(ConvNeXt, self).__init__()
+        # set attributes
+        self.structure_type = structure_type
+        self.arch = arch
+        self.in_channels = in_channels
+        self.stem_patch_size = stem_patch_size
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.linear_pw_conv = linear_pw_conv
+        self.drop_path_rate = drop_path_rate
+        self.layer_scale_init_value = layer_scale_init_value
+        self.gap_before_final_norm = gap_before_final_norm
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
         arch = self.arch_settings[arch]
         self.depths = arch['depths']
         self.channels = arch['channels']
         self.num_stages = len(self.depths)
         if isinstance(out_indices, int):
             out_indices = [out_indices]
         for i, index in enumerate(out_indices):
             if index < 0:
                 out_indices[i] = 4 + index
                 assert out_indices[i] >= 0, f'Invalid out_indices {index}'
         self.out_indices = out_indices
-        self.gap_before_final_norm = gap_before_final_norm
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # stochastic depth decay rule
         dpr = [x.item() for x in torch.linspace(0, drop_path_rate, sum(self.depths))]
         # 4 downsample layers between stages, including the stem layer.
         self.downsample_layers = nn.ModuleList()
-        if norm_cfg['type'] in ['layernorm2d']:
-            norm_cfg_copy = copy.deepcopy(norm_cfg)
-            norm_cfg_copy.pop('type')
-            norm_layer = LayerNorm2d(num_channels=self.channels[0], **norm_cfg_copy)
-        else:
-            norm_layer = BuildNormalization(constructnormcfg(placeholder=self.channels[0], norm_cfg=norm_cfg))
+        norm_layer = BuildNormalization(placeholder=self.channels[0], norm_cfg=norm_cfg)
         stem = nn.Sequential(
             nn.Conv2d(in_channels, self.channels[0], kernel_size=stem_patch_size, stride=stem_patch_size),
             norm_layer,
         )
         self.downsample_layers.append(stem)
         # 4 feature resolution stages, each consisting of multiple residual blocks
         block_idx = 0
@@ -147,21 +133,19 @@
                     in_channels=channels, drop_path_rate=dpr[block_idx + j], norm_cfg=norm_cfg, act_cfg=act_cfg,
                     linear_pw_conv=linear_pw_conv, layer_scale_init_value=layer_scale_init_value
                 ) for j in range(depth)
             ])
             block_idx += depth
             self.stages.append(stage)
             if i in self.out_indices:
-                if norm_cfg['type'] in ['layernorm2d']:
-                    norm_cfg_copy = copy.deepcopy(norm_cfg)
-                    norm_cfg_copy.pop('type')
-                    norm_layer = LayerNorm2d(num_channels=channels, **norm_cfg_copy)
-                else:
-                    norm_layer = BuildNormalization(constructnormcfg(placeholder=channels, norm_cfg=norm_cfg))
+                norm_layer = BuildNormalization(placeholder=channels, norm_cfg=norm_cfg)
                 self.add_module(f'norm{i}', norm_layer)
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''forward'''
     def forward(self, x):
         outs = []
         for i, stage in enumerate(self.stages):
             x = self.downsample_layers[i](x)
             x = stage(x)
             if i in self.out_indices:
@@ -169,57 +153,22 @@
                 if self.gap_before_final_norm:
                     gap = x.mean([-2, -1], keepdim=True)
                     outs.append(norm_layer(gap).flatten(1))
                 else:
                     outs.append(norm_layer(x).contiguous())
         return tuple(outs)
     '''initweights'''
-    def initweights(self, convnext_type, pretrained_model_path=''):
+    def initweights(self, structure_type, pretrained_model_path=''):
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[convnext_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         state_dict_convert = {}
         for key, value in state_dict.items():
             state_dict_convert[key.replace('backbone.', '')] = value
-        self.load_state_dict(state_dict_convert, strict=False)
-
-
-'''BuildConvNeXt'''
-def BuildConvNeXt(convnext_cfg):
-    # assert whether support
-    convnext_type = convnext_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'arch': 'tiny', 
-        'in_channels': 3, 
-        'stem_patch_size': 4, 
-        'norm_cfg': {'type': 'layernorm2d', 'eps': 1e-6},
-        'act_cfg': {'type': 'gelu'},
-        'linear_pw_conv': True,
-        'drop_path_rate': 0., 
-        'layer_scale_init_value': 1e-6, 
-        'out_indices': (0, 1, 2, 3), 
-        'gap_before_final_norm': True,
-        'pretrained': True,
-        'pretrained_model_path': '',
-    }
-    for key, value in convnext_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain convnext_cfg
-    convnext_cfg = default_cfg.copy()
-    pretrained = convnext_cfg.pop('pretrained')
-    pretrained_model_path = convnext_cfg.pop('pretrained_model_path')
-    # obtain the instanced convnext
-    model = ConvNeXt(**convnext_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(convnext_type, pretrained_model_path)
-    # return the model
-    return model
+        self.load_state_dict(state_dict_convert, strict=False)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/erfnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/erfnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,31 @@
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Downsampler block of ERFNet'''
 class DownsamplerBlock(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None):
         super(DownsamplerBlock, self).__init__()
         self.norm_cfg, self.act_cfg = norm_cfg, act_cfg
         self.conv = nn.Conv2d(in_channels, out_channels - in_channels, kernel_size=3, stride=2, padding=1, bias=False)
         self.pool = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.bn = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg))
+        self.bn = BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg)
         self.act = BuildActivation(act_cfg)
     '''forward'''
     def forward(self, x):
         conv_out, pool_out = self.conv(x), self.pool(x)
         pool_out = F.interpolate(pool_out, size=conv_out.size()[2:], mode='bilinear', align_corners=False)
         output = torch.cat([conv_out, pool_out], dim=1)
         output = self.bn(output)
@@ -46,15 +48,15 @@
             first_conv_padding = (1, 0) if conv_layer == 0 else (dilation, 0)
             first_conv_dilation = 1 if conv_layer == 0 else (dilation, 1)
             second_conv_padding = (0, 1) if conv_layer == 0 else (0, dilation)
             second_conv_dilation = 1 if conv_layer == 0 else (1, dilation)
             self.convs_layers.append(nn.Conv2d(channels, channels, kernel_size=(3, 1), stride=1, padding=first_conv_padding, bias=True, dilation=first_conv_dilation))
             self.convs_layers.append(self.act)
             self.convs_layers.append(nn.Conv2d(channels, channels, kernel_size=(1, 3), stride=1, padding=second_conv_padding, bias=True, dilation=second_conv_dilation))
-            self.convs_layers.append(BuildNormalization(constructnormcfg(placeholder=channels, norm_cfg=norm_cfg)))
+            self.convs_layers.append(BuildNormalization(placeholder=channels, norm_cfg=norm_cfg))
             if conv_layer == 0: self.convs_layers.append(self.act)
             else: self.convs_layers.append(nn.Dropout(p=drop_rate))
     '''forward'''
     def forward(self, x):
         output = x
         for conv in self.convs_layers:
             output = conv(output)
@@ -64,50 +66,56 @@
 
 '''Upsampler block of ERFNet'''
 class UpsamplerBlock(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None):
         super(UpsamplerBlock, self).__init__()
         self.norm_cfg, self.act_cfg = norm_cfg, act_cfg
         self.conv = nn.ConvTranspose2d(in_channels, out_channels, kernel_size=3, stride=2, padding=1, output_padding=1, bias=True)
-        self.bn = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg))
+        self.bn = BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg)
         self.act = BuildActivation(act_cfg)
     '''forward'''
     def forward(self, x):
         output = self.conv(x)
         output = self.bn(output)
         output = self.act(output)
         return output
 
 
 '''ERFNet'''
 class ERFNet(nn.Module):
-    def __init__(self, in_channels=3, enc_downsample_channels=(16, 64, 128), enc_stage_non_bottlenecks=(5, 8), enc_non_bottleneck_dilations=(2, 4, 8, 16),
+    def __init__(self, structure_type, in_channels=3, enc_downsample_channels=(16, 64, 128), enc_stage_non_bottlenecks=(5, 8), enc_non_bottleneck_dilations=(2, 4, 8, 16),
                  enc_non_bottleneck_channels=(64, 128), dec_upsample_channels=(64, 16), dec_stages_non_bottleneck=(2, 2), dec_non_bottleneck_channels=(64, 16),
-                 dropout_ratio=0.1, norm_cfg=None, act_cfg=None):
+                 dropout_ratio=0.1, norm_cfg={'type': 'SyncBatchNorm'}, act_cfg={'type': 'PReLU'}, pretrained=False, pretrained_model_path=''):
         super(ERFNet, self).__init__()
-        # check arguments
-        assert len(enc_downsample_channels) == len(dec_upsample_channels) + 1
-        assert len(enc_downsample_channels) == len(enc_stage_non_bottlenecks) + 1
-        assert len(enc_downsample_channels) == len(enc_non_bottleneck_channels) + 1
-        assert enc_stage_non_bottlenecks[-1] % len(enc_non_bottleneck_dilations) == 0
-        assert len(dec_upsample_channels) == len(dec_stages_non_bottleneck)
-        assert len(dec_stages_non_bottleneck) == len(dec_non_bottleneck_channels)
         # set attributes
+        self.structure_type = structure_type
         self.in_channels = in_channels
         self.enc_downsample_channels = enc_downsample_channels
         self.enc_stage_non_bottlenecks = enc_stage_non_bottlenecks
         self.enc_non_bottleneck_dilations = enc_non_bottleneck_dilations
         self.enc_non_bottleneck_channels = enc_non_bottleneck_channels
         self.dec_upsample_channels = dec_upsample_channels
         self.dec_stages_non_bottleneck = dec_stages_non_bottleneck
         self.dec_non_bottleneck_channels = dec_non_bottleneck_channels
         self.dropout_ratio = dropout_ratio
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
-        # define encoder and decoder
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        assert len(enc_downsample_channels) == len(dec_upsample_channels) + 1
+        assert len(enc_downsample_channels) == len(enc_stage_non_bottlenecks) + 1
+        assert len(enc_downsample_channels) == len(enc_non_bottleneck_channels) + 1
+        assert enc_stage_non_bottlenecks[-1] % len(enc_non_bottleneck_dilations) == 0
+        assert len(dec_upsample_channels) == len(dec_stages_non_bottleneck)
+        assert len(dec_stages_non_bottleneck) == len(dec_non_bottleneck_channels)
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # set encoder and decoder
         self.encoder = nn.ModuleList()
         self.decoder = nn.ModuleList()
         # --encoder
         self.encoder.append(DownsamplerBlock(in_channels, enc_downsample_channels[0], norm_cfg=norm_cfg, act_cfg=act_cfg))
         for i in range(len(enc_downsample_channels) - 1):
             self.encoder.append(DownsamplerBlock(enc_downsample_channels[i], enc_downsample_channels[i + 1], norm_cfg=norm_cfg, act_cfg=act_cfg))
             if i == len(enc_downsample_channels) - 2:
@@ -119,60 +127,27 @@
                 for j in range(enc_stage_non_bottlenecks[i]):
                     self.encoder.append(NonBottleneck1d(enc_downsample_channels[i + 1], dropout_ratio, norm_cfg=norm_cfg, act_cfg=act_cfg))
         # --decoder
         for i in range(len(dec_upsample_channels)):
             if i == 0: self.decoder.append(UpsamplerBlock(enc_downsample_channels[-1], dec_non_bottleneck_channels[i], norm_cfg=norm_cfg, act_cfg=act_cfg))
             else: self.decoder.append(UpsamplerBlock(dec_non_bottleneck_channels[i - 1], dec_non_bottleneck_channels[i], norm_cfg=norm_cfg, act_cfg=act_cfg))
             for j in range(dec_stages_non_bottleneck[i]): self.decoder.append(NonBottleneck1d(dec_non_bottleneck_channels[i], norm_cfg=norm_cfg, act_cfg=act_cfg))
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         for enc in self.encoder: x = enc(x)
         for dec in self.decoder: x = dec(x)
-        return [x]
-
-
-'''BuildERFNet'''
-def BuildERFNet(erfnet_cfg):
-    # assert whether support
-    erfnet_type = erfnet_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3, 
-        'enc_downsample_channels': (16, 64, 128),
-        'enc_stage_non_bottlenecks': (5, 8),
-        'enc_non_bottleneck_dilations': (2, 4, 8, 16),
-        'enc_non_bottleneck_channels': (64, 128),
-        'dec_upsample_channels': (64, 16),
-        'dec_stages_non_bottleneck': (2, 2),
-        'dec_non_bottleneck_channels': (64, 16),
-        'dropout_ratio': 0.1,
-        'norm_cfg': None, 
-        'act_cfg': {'type': 'prelu'},
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in erfnet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain erfnet_cfg
-    erfnet_cfg = default_cfg.copy()
-    pretrained = erfnet_cfg.pop('pretrained')
-    pretrained_model_path = erfnet_cfg.pop('pretrained_model_path')
-    # obtain the instanced erfnet
-    model = ERFNet(**erfnet_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[erfnet_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return [x]
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/fastscnn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/fastscnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,21 @@
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, DepthwiseSeparableConv2d, InvertedResidual, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation, DepthwiseSeparableConv2d, InvertedResidual
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Pooling Pyramid Module used in PSPNet'''
 class PoolingPyramidModule(nn.ModuleList):
     def __init__(self, pool_scales, in_channels, out_channels, norm_cfg, act_cfg, align_corners):
         super(PoolingPyramidModule, self).__init__()
         self.pool_scales = pool_scales
@@ -26,15 +28,15 @@
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
         self.align_corners = align_corners
         for pool_scale in pool_scales:
             self.append(nn.Sequential(
                 nn.AdaptiveAvgPool2d(pool_scale),
                 nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
     '''forward'''
     def forward(self, x):
         ppm_outs = []
         for ppm in self:
             ppm_out = ppm(x)
@@ -54,15 +56,15 @@
         super(LearningToDownsample, self).__init__()
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
         self.dw_act_cfg = dw_act_cfg
         dw_channels1, dw_channels2 = dw_channels
         self.conv = nn.Sequential(
             nn.Conv2d(in_channels, dw_channels1, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=dw_channels1, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=dw_channels1, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.dsconv1 = DepthwiseSeparableConv2d(
             in_channels=dw_channels1,
             out_channels=dw_channels2,
             kernel_size=3, 
             stride=2, 
@@ -101,15 +103,15 @@
         # define modules
         self.bottleneck1 = self.makelayer(in_channels, block_channels[0], num_blocks[0], strides[0], expand_ratio)
         self.bottleneck2 = self.makelayer(block_channels[0], block_channels[1], num_blocks[1], strides[1], expand_ratio)
         self.bottleneck3 = self.makelayer(block_channels[1], block_channels[2], num_blocks[2], strides[2], expand_ratio)
         self.ppm = PoolingPyramidModule(pool_scales, block_channels[2], block_channels[2] // 4, norm_cfg=self.norm_cfg, act_cfg=self.act_cfg, align_corners=align_corners)
         self.out = nn.Sequential(
             nn.Conv2d(block_channels[2] * 2, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''make layer'''
     def makelayer(self, in_channels, out_channels, blocks, stride=1, expand_ratio=6):
         layers = [
             InvertedResidual(in_channels, out_channels, stride, expand_ratio, norm_cfg=self.norm_cfg, act_cfg=self.act_cfg)
         ]
@@ -136,60 +138,70 @@
         self.norm_cfg = norm_cfg
         self.dwconv_act_cfg = dwconv_act_cfg
         self.conv_act_cfg = conv_act_cfg
         self.align_corners = align_corners
         # define modules
         self.dwconv = nn.Sequential(
             nn.Conv2d(lower_in_channels, out_channels, kernel_size=3, stride=1, padding=1, groups=out_channels, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(dwconv_act_cfg),
         )
         self.conv_lower_res = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
         )
         self.conv_higher_res = nn.Sequential(
             nn.Conv2d(higher_in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
         )
         self.act = BuildActivation(conv_act_cfg)
     '''forward'''
     def forward(self, higher_res_feature, lower_res_feature):
         lower_res_feature = F.interpolate(lower_res_feature, size=higher_res_feature.size()[2:], mode='bilinear', align_corners=self.align_corners)
         lower_res_feature = self.dwconv(lower_res_feature)
         lower_res_feature = self.conv_lower_res(lower_res_feature)
         higher_res_feature = self.conv_higher_res(higher_res_feature)
         out = higher_res_feature + lower_res_feature
         return self.act(out)
 
 
 '''FastSCNN'''
 class FastSCNN(nn.Module):
-    def __init__(self, in_channels=3, downsample_dw_channels=(32, 48), global_in_channels=64, global_block_channels=(64, 96, 128), global_block_strides=(2, 2, 1), global_out_channels=128, 
-                 higher_in_channels=64, lower_in_channels=128, fusion_out_channels=128, out_indices=(0, 1, 2), norm_cfg=None, act_cfg=None, align_corners=False, dw_act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, downsample_dw_channels=(32, 48), global_in_channels=64, global_block_channels=(64, 96, 128), 
+                 global_block_strides=(2, 2, 1), global_out_channels=128, higher_in_channels=64, lower_in_channels=128, fusion_out_channels=128, 
+                 out_indices=(0, 1, 2), norm_cfg={'type': 'SyncBatchNorm'}, act_cfg={'type': 'ReLU', 'inplace': True}, align_corners=False, 
+                 dw_act_cfg={'type': 'ReLU', 'inplace': True}, pretrained=False, pretrained_model_path=''):
         super(FastSCNN, self).__init__()
-        assert global_in_channels == higher_in_channels, 'Global Input Channels must be the same with Higher Input Channels'
-        assert global_out_channels == lower_in_channels, 'Global Output Channels must be the same with Lower Input Channels'
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
         self.in_channels = in_channels
+        self.downsample_dw_channels = downsample_dw_channels
         self.downsample_dw_channels1 = downsample_dw_channels[0]
         self.downsample_dw_channels2 = downsample_dw_channels[1]
         self.global_in_channels = global_in_channels
         self.global_block_channels = global_block_channels
         self.global_block_strides = global_block_strides
         self.global_out_channels = global_out_channels
         self.higher_in_channels = higher_in_channels
         self.lower_in_channels = lower_in_channels
         self.fusion_out_channels = fusion_out_channels
         self.out_indices = out_indices
         self.norm_cfg = norm_cfg
         self.act_cfg = act_cfg
         self.align_corners = align_corners
         self.dw_act_cfg = dw_act_cfg
-        # define modules
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        assert global_in_channels == higher_in_channels, 'Global Input Channels must be the same with Higher Input Channels'
+        assert global_out_channels == lower_in_channels, 'Global Output Channels must be the same with Lower Input Channels'
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # set modules
         self.learning_to_downsample = LearningToDownsample(
             in_channels=in_channels, 
             dw_channels=downsample_dw_channels, 
             out_channels=global_in_channels,
             norm_cfg=self.norm_cfg,
             act_cfg=self.act_cfg,
             dw_act_cfg=self.dw_act_cfg
@@ -208,66 +220,30 @@
             lower_in_channels=lower_in_channels, 
             out_channels=fusion_out_channels, 
             norm_cfg=self.norm_cfg, 
             dwconv_act_cfg=self.act_cfg, 
             conv_act_cfg=self.act_cfg, 
             align_corners=self.align_corners,
         )
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         higher_res_features = self.learning_to_downsample(x)
         lower_res_features = self.global_feature_extractor(higher_res_features)
         fusion_output = self.feature_fusion(higher_res_features, lower_res_features)
         outs = [higher_res_features, lower_res_features, fusion_output]
         outs = [outs[i] for i in self.out_indices]
-        return tuple(outs)
-
-
-'''BuildFastSCNN'''
-def BuildFastSCNN(fastscnn_cfg):
-    # assert whether support
-    fastscnn_type = fastscnn_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3, 
-        'downsample_dw_channels': (32, 48),
-        'global_in_channels': 64,
-        'global_block_channels': (64, 96, 128),
-        'global_block_strides': (2, 2, 1),
-        'global_out_channels': 128,
-        'higher_in_channels': 64,
-        'lower_in_channels': 128,
-        'fusion_out_channels': 128,
-        'out_indices': (0, 1, 2),
-        'norm_cfg': None,
-        'act_cfg': {'type': 'relu', 'inplace': True},
-        'align_corners': False,
-        'dw_act_cfg': {'type': 'relu', 'inplace': True},
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in fastscnn_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain fastscnn_cfg
-    fastscnn_cfg = default_cfg.copy()
-    pretrained = fastscnn_cfg.pop('pretrained')
-    pretrained_model_path = fastscnn_cfg.pop('pretrained_model_path')
-    # obtain the instanced fastscnn
-    model = FastSCNN(**fastscnn_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[fastscnn_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/hrnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/hrnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 from .resnet import BasicBlock, Bottleneck
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'hrnetv2_w18_small': 'https://download.openmmlab.com/pretrain/third_party/hrnetv2_w18_small-b5a04e21.pth',
     'hrnetv2_w18': 'https://download.openmmlab.com/pretrain/third_party/hrnetv2_w18-00eb2006.pth',
     'hrnetv2_w32': 'https://download.openmmlab.com/pretrain/third_party/hrnetv2_w32-dc9eeb4f.pth',
     'hrnetv2_w40': 'https://download.openmmlab.com/pretrain/third_party/hrnetv2_w40-ed0b031c.pth',
     'hrnetv2_w48': 'https://download.openmmlab.com/pretrain/third_party/hrnetv2_w48-d2186c55.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''HRModule'''
 class HRModule(nn.Module):
     def __init__(self, num_branches, block, num_blocks, in_channels, num_channels, multiscale_output=True, norm_cfg=None, act_cfg=None):
         super(HRModule, self).__init__()
         self.checkbranches(num_branches, num_blocks, in_channels, num_channels)
@@ -65,15 +67,15 @@
         return nn.ModuleList(branches)
     '''make one branch'''
     def makebranch(self, branch_index, block, num_blocks, num_channels, stride=1, norm_cfg=None, act_cfg=None):
         downsample = None
         if stride != 1 or self.in_channels[branch_index] != num_channels[branch_index] * block.expansion:
             downsample = nn.Sequential(
                 nn.Conv2d(self.in_channels[branch_index], num_channels[branch_index] * block.expansion, kernel_size=1, stride=stride, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=num_channels[branch_index] * block.expansion, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=num_channels[branch_index] * block.expansion, norm_cfg=norm_cfg),
             )
         layers = []
         layers.append(block(self.in_channels[branch_index], num_channels[branch_index], stride, downsample=downsample, norm_cfg=norm_cfg, act_cfg=act_cfg))
         self.in_channels[branch_index] = num_channels[branch_index] * block.expansion
         for i in range(1, num_blocks[branch_index]):
             layers.append(block(self.in_channels[branch_index], num_channels[branch_index], norm_cfg=norm_cfg, act_cfg=act_cfg))
         return nn.Sequential(*layers)
@@ -87,55 +89,101 @@
         for i in range(num_out_branches):
             fuse_layer = []
             for j in range(num_branches):
                 if j > i:
                     fuse_layer.append(
                         nn.Sequential(
                             nn.Conv2d(in_channels[j], in_channels[i], kernel_size=1, stride=1, padding=0, bias=False),
-                            BuildNormalization(constructnormcfg(placeholder=in_channels[i], norm_cfg=norm_cfg)),
+                            BuildNormalization(placeholder=in_channels[i], norm_cfg=norm_cfg),
                             nn.Upsample(scale_factor=2**(j-i), mode='bilinear', align_corners=False)
                         )
                     )
                 elif j == i:
                     fuse_layer.append(None)
                 else:
                     conv_downsamples = []
                     for k in range(i - j):
                         if k == i - j - 1:
                             conv_downsamples.append(
                                 nn.Sequential(
                                     nn.Conv2d(in_channels[j], in_channels[i], kernel_size=3, stride=2, padding=1, bias=False),
-                                    BuildNormalization(constructnormcfg(placeholder=in_channels[i], norm_cfg=norm_cfg)),
+                                    BuildNormalization(placeholder=in_channels[i], norm_cfg=norm_cfg),
                                 )
                             )
                         else:
                             conv_downsamples.append(
                                 nn.Sequential(
                                     nn.Conv2d(in_channels[j], in_channels[j], kernel_size=3, stride=2, padding=1, bias=False),
-                                    BuildNormalization(constructnormcfg(placeholder=in_channels[j], norm_cfg=norm_cfg)),
+                                    BuildNormalization(placeholder=in_channels[j], norm_cfg=norm_cfg),
                                     BuildActivation(act_cfg),
                                 )
                             )
                     fuse_layer.append(nn.Sequential(*conv_downsamples))
             fuse_layers.append(nn.ModuleList(fuse_layer))
         return nn.ModuleList(fuse_layers)
 
 
 '''HRNet'''
 class HRNet(nn.Module):
     blocks_dict = {'BASIC': BasicBlock, 'BOTTLENECK': Bottleneck}
-    def __init__(self, in_channels=3, stages_cfg=None, norm_cfg=None, act_cfg=None):
+    arch_settings = {
+        'hrnetv2_w18_small': {
+            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (2,), 'num_channels': (64,),},
+            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (2, 2), 'num_channels': (18, 36),},
+            'stage3': {'num_modules': 3, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (2, 2, 2), 'num_channels': (18, 36, 72),},
+            'stage4': {'num_modules': 2, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (2, 2, 2, 2), 'num_channels': (18, 36, 72, 144),},
+        },
+        'hrnetv2_w18': {
+            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
+            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (18, 36),},
+            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (18, 36, 72),},
+            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (18, 36, 72, 144),},
+        },
+        'hrnetv2_w32': {
+            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
+            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (32, 64),},
+            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (32, 64, 128),},
+            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (32, 64, 128, 256),},
+        },
+        'hrnetv2_w40': {
+            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
+            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (40, 80),},
+            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (40, 80, 160),},
+            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (40, 80, 160, 320),},
+        },
+        'hrnetv2_w48': {
+            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
+            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (48, 96),},
+            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (48, 96, 192),},
+            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (48, 96, 192, 384),},
+        },
+    }
+    def __init__(self, structure_type, arch='hrnetv2_w18_small', in_channels=3, norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'ReLU', 'inplace': True}, pretrained=True, pretrained_model_path=''):
         super(HRNet, self).__init__()
+        # set attributes
+        self.structure_type = structure_type
+        self.arch = arch
+        self.in_channels = in_channels
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # stem net
         self.conv1 = nn.Conv2d(in_channels, 64, kernel_size=3, stride=2, padding=1, bias=False)
-        self.bn1 = BuildNormalization(constructnormcfg(placeholder=64, norm_cfg=norm_cfg))
+        self.bn1 = BuildNormalization(placeholder=64, norm_cfg=norm_cfg)
         self.conv2 = nn.Conv2d(64, 64, kernel_size=3, stride=2, padding=1, bias=False)
-        self.bn2 = BuildNormalization(constructnormcfg(placeholder=64, norm_cfg=norm_cfg))
+        self.bn2 = BuildNormalization(placeholder=64, norm_cfg=norm_cfg)
         self.relu = BuildActivation(act_cfg)
         # stage1
+        stages_cfg = self.arch_settings[arch]
         self.stage1_cfg = stages_cfg['stage1']
         num_channels = self.stage1_cfg['num_channels'][0]
         block_type = self.stage1_cfg['block']
         num_blocks = self.stage1_cfg['num_blocks'][0]
         block = self.blocks_dict[block_type]
         stage1_out_channels = num_channels * block.expansion
         self.layer1 = self.makelayer(block, 64, num_channels, num_blocks, norm_cfg=norm_cfg, act_cfg=act_cfg)
@@ -159,14 +207,29 @@
         self.stage4_cfg = stages_cfg['stage4']
         num_channels = self.stage4_cfg['num_channels']
         block_type = self.stage4_cfg['block']
         block = self.blocks_dict[block_type]
         num_channels = [channel * block.expansion for channel in num_channels]
         self.transition3 = self.maketransitionlayer(pre_stage_channels, num_channels, norm_cfg=norm_cfg, act_cfg=act_cfg)
         self.stage4, pre_stage_channels = self.makestage(self.stage4_cfg, num_channels, norm_cfg=norm_cfg, act_cfg=act_cfg)
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.conv2(x)
         x = self.bn2(x)
         x = self.relu(x)
@@ -213,15 +276,15 @@
         return nn.Sequential(*hr_modules), in_channels
     '''make layer'''
     def makelayer(self, block, inplanes, planes, num_blocks, stride=1, norm_cfg=None, act_cfg=None):
         downsample = None
         if stride != 1 or inplanes != planes * block.expansion:
             downsample = nn.Sequential(
                 nn.Conv2d(inplanes, planes * block.expansion, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=planes * block.expansion, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=planes * block.expansion, norm_cfg=norm_cfg),
             )
         layers = []
         layers.append(
             block(inplanes, planes, stride, downsample=downsample, norm_cfg=norm_cfg, act_cfg=act_cfg)
         )
         inplanes = planes * block.expansion
         for i in range(1, num_blocks):
@@ -236,101 +299,27 @@
         transition_layers = []
         for i in range(num_branches_cur):
             if i < num_branches_pre:
                 if num_channels_cur_layer[i] != num_channels_pre_layer[i]:
                     transition_layers.append(
                         nn.Sequential(
                             nn.Conv2d(num_channels_pre_layer[i], num_channels_cur_layer[i], kernel_size=3, stride=1, padding=1, bias=False),
-                            BuildNormalization(constructnormcfg(placeholder=num_channels_cur_layer[i], norm_cfg=norm_cfg)),
+                            BuildNormalization(placeholder=num_channels_cur_layer[i], norm_cfg=norm_cfg),
                             BuildActivation(act_cfg),
                         )
                      )
                 else:
                     transition_layers.append(None)
             else:
                 conv_downsamples = []
                 for j in range(i + 1 - num_branches_pre):
                     in_channels = num_channels_pre_layer[-1]
                     out_channels = num_channels_cur_layer[i] if j == i - num_branches_pre else in_channels
                     conv_downsamples.append(
                         nn.Sequential(
                             nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=2, padding=1, bias=False),
-                            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                             BuildActivation(act_cfg),
                         )
                     )
                 transition_layers.append(nn.Sequential(*conv_downsamples))
-        return nn.ModuleList(transition_layers)
-
-
-'''BuildHRNet'''
-def BuildHRNet(hrnet_cfg):
-    # assert whether support
-    hrnet_type = hrnet_cfg.pop('type')
-    supported_hrnets = {
-        'hrnetv2_w18_small': {
-            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (2,), 'num_channels': (64,),},
-            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (2, 2), 'num_channels': (18, 36),},
-            'stage3': {'num_modules': 3, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (2, 2, 2), 'num_channels': (18, 36, 72),},
-            'stage4': {'num_modules': 2, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (2, 2, 2, 2), 'num_channels': (18, 36, 72, 144),},
-        },
-        'hrnetv2_w18': {
-            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
-            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (18, 36),},
-            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (18, 36, 72),},
-            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (18, 36, 72, 144),},
-        },
-        'hrnetv2_w32': {
-            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
-            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (32, 64),},
-            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (32, 64, 128),},
-            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (32, 64, 128, 256),},
-        },
-        'hrnetv2_w40': {
-            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
-            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (40, 80),},
-            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (40, 80, 160),},
-            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (40, 80, 160, 320),},
-        },
-        'hrnetv2_w48': {
-            'stage1': {'num_modules': 1, 'num_branches': 1, 'block': 'BOTTLENECK', 'num_blocks': (4,), 'num_channels': (64,),},
-            'stage2': {'num_modules': 1, 'num_branches': 2, 'block': 'BASIC', 'num_blocks': (4, 4), 'num_channels': (48, 96),},
-            'stage3': {'num_modules': 4, 'num_branches': 3, 'block': 'BASIC', 'num_blocks': (4, 4, 4), 'num_channels': (48, 96, 192),},
-            'stage4': {'num_modules': 3, 'num_branches': 4, 'block': 'BASIC', 'num_blocks': (4, 4, 4, 4), 'num_channels': (48, 96, 192, 384),},
-        },
-    }
-    assert hrnet_type in supported_hrnets, 'unsupport the hrnet_type %s' % hrnet_type
-    # parse cfg
-    default_cfg = {
-        'norm_cfg': None,
-        'in_channels': 3,
-        'pretrained': True,
-        'pretrained_model_path': '',
-        'act_cfg': {'type': 'relu', 'inplace': True},
-    }
-    for key, value in hrnet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain hrnet_cfg
-    hrnet_cfg = default_cfg.copy()
-    hrnet_cfg['stages_cfg'] = supported_hrnets[hrnet_type]
-    pretrained = hrnet_cfg.pop('pretrained')
-    pretrained_model_path = hrnet_cfg.pop('pretrained_model_path')
-    # obtain the instanced hrnet
-    model = HRNet(**hrnet_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[hrnet_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return nn.ModuleList(transition_layers)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/mit.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/mit.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,53 @@
 '''
 import math
 import torch
 import torch.nn as nn
 import torch.utils.model_zoo as model_zoo
 import torch.utils.checkpoint as checkpoint
 from .bricks import PatchEmbed as PatchEmbedBase
-from .bricks import BuildNormalization, BuildActivation, BuildDropout, nlctonchw, nchwtonlc, MultiheadAttention, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation, BuildDropout, nlctonchw, nchwtonlc, MultiheadAttention
 
 
-'''model urls, the pretrained weights are stored in https://drive.google.com/drive/folders/1b7bwrInTW4VLEm27YawHOAMSMikga2Ia'''
-model_urls = {
+'''DEFAULT_MODEL_URLS, the pretrained weights are stored in https://drive.google.com/drive/folders/1b7bwrInTW4VLEm27YawHOAMSMikga2Ia'''
+DEFAULT_MODEL_URLS = {
     'mit-b0': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b0.pth',
     'mit-b1': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b1.pth',
     'mit-b2': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b2.pth',
     'mit-b3': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b3.pth',
     'mit-b4': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b4.pth',
     'mit-b5': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_segformer/mit_b5.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {
+    'mit-b0': {
+        'embed_dims': 32, 'num_stages': 4, 'num_layers': [2, 2, 2, 2], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+    'mit-b1': {
+        'embed_dims': 64, 'num_stages': 4, 'num_layers': [2, 2, 2, 2], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+    'mit-b2': {
+        'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 4, 6, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+    'mit-b3': {
+        'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 4, 18, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+    'mit-b4': {
+        'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 8, 27, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+    'mit-b5': {
+        'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 6, 40, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
+        'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
+    },
+}
 
 
 '''PatchEmbed'''
 class PatchEmbed(PatchEmbedBase):
     def __init__(self, **kwargs):
         super(PatchEmbed, self).__init__(**kwargs)
     '''layers with zero weight decay'''
@@ -74,15 +101,15 @@
 '''EfficientMultiheadAttention'''
 class EfficientMultiheadAttention(MultiheadAttention):
     def __init__(self, embed_dims, num_heads, attn_drop=0., proj_drop=0., dropout_cfg=None, batch_first=True, qkv_bias=False, norm_cfg=None, sr_ratio=1):
         super(EfficientMultiheadAttention, self).__init__(embed_dims, num_heads, attn_drop, proj_drop, dropout_cfg=dropout_cfg, batch_first=batch_first, bias=qkv_bias)
         self.sr_ratio = sr_ratio
         if sr_ratio > 1:
             self.sr = nn.Conv2d(embed_dims, embed_dims, kernel_size=sr_ratio, stride=sr_ratio, padding=0)
-            self.norm = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+            self.norm = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
     '''layers with zero weight decay'''
     def zerowdlayers(self):
         if hasattr(self, 'norm'):
             return {'EfficientMultiheadAttention.norm': self.norm}
         return {}
     '''layers with non zero weight decay'''
     def nonzerowdlayers(self):
@@ -110,32 +137,32 @@
 
 
 '''TransformerEncoderLayer'''
 class TransformerEncoderLayer(nn.Module):
     def __init__(self, embed_dims, num_heads, feedforward_channels, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., 
                  qkv_bias=True, act_cfg=None, norm_cfg=None, batch_first=True, sr_ratio=1, use_checkpoint=False):
         super(TransformerEncoderLayer, self).__init__()
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.attn = EfficientMultiheadAttention(
             embed_dims=embed_dims,
             num_heads=num_heads,
             attn_drop=attn_drop_rate,
             proj_drop=drop_rate,
-            dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
             batch_first=batch_first,
             qkv_bias=qkv_bias,
             norm_cfg=norm_cfg,
             sr_ratio=sr_ratio
         )
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm2 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.ffn = MixFFN(
             embed_dims=embed_dims,
             feedforward_channels=feedforward_channels,
             ffn_drop=drop_rate,
-            dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
             act_cfg=act_cfg
         )
         self.use_checkpoint = use_checkpoint
     '''layers with zero weight decay'''
     def zerowdlayers(self):
         layers = {
             'TransformerEncoderLayer.norm1': self.norm1,
@@ -165,31 +192,46 @@
         else:
             x = _forward(x)
         return x
 
 
 '''MixVisionTransformer'''
 class MixVisionTransformer(nn.Module):
-    def __init__(self, in_channels=3, embed_dims=64, num_stages=4, num_layers=[3, 4, 6, 3], num_heads=[1, 2, 4, 8], patch_sizes=[7, 3, 3, 3], strides=[4, 2, 2, 2],
-                 sr_ratios=[8, 4, 2, 1], out_indices=(0, 1, 2, 3), mlp_ratio=4, qkv_bias=True, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., 
-                 act_cfg=None, norm_cfg=None, use_checkpoint=False):
+    def __init__(self, structure_type, in_channels=3, embed_dims=64, num_stages=4, num_layers=[3, 4, 6, 3], num_heads=[1, 2, 4, 8], 
+                 patch_sizes=[7, 3, 3, 3], strides=[4, 2, 2, 2], sr_ratios=[8, 4, 2, 1], out_indices=(0, 1, 2, 3), mlp_ratio=4, qkv_bias=True, 
+                 drop_rate=0., attn_drop_rate=0., drop_path_rate=0., act_cfg={'type': 'GELU'}, norm_cfg={'type': 'LayerNorm', 'eps': 1e-6}, 
+                 use_checkpoint=False, pretrained=True, pretrained_model_path=''):
         super(MixVisionTransformer, self).__init__()
-        # assert
-        assert num_stages == len(num_layers) == len(num_heads) == len(patch_sizes) == len(strides) == len(sr_ratios)
-        assert max(out_indices) < num_stages
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
+        self.in_channels = in_channels
         self.embed_dims = embed_dims
         self.num_stages = num_stages
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.patch_sizes = patch_sizes
         self.strides = strides
         self.sr_ratios = sr_ratios
         self.out_indices = out_indices
+        self.mlp_ratio = mlp_ratio
+        self.qkv_bias = qkv_bias
+        self.drop_rate = drop_rate
+        self.attn_drop_rate = attn_drop_rate
+        self.drop_path_rate = drop_path_rate
+        self.act_cfg = act_cfg
+        self.norm_cfg = norm_cfg
         self.use_checkpoint = use_checkpoint
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        assert num_stages == len(num_layers) == len(num_heads) == len(patch_sizes) == len(strides) == len(sr_ratios)
+        assert max(out_indices) < num_stages
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # transformer encoder
         dpr = [x.item() for x in torch.linspace(0, drop_path_rate, sum(num_layers))]
         cur, self.layers = 0, nn.ModuleList()
         for i, num_layer in enumerate(num_layers):
             embed_dims_i = embed_dims * num_heads[i]
             patch_embed = PatchEmbed(
                 in_channels=in_channels,
@@ -209,17 +251,20 @@
                 qkv_bias=qkv_bias,
                 act_cfg=act_cfg,
                 norm_cfg=norm_cfg,
                 use_checkpoint=use_checkpoint,
                 sr_ratio=sr_ratios[i]) for idx in range(num_layer)
             ])
             in_channels = embed_dims_i
-            norm = BuildNormalization(constructnormcfg(placeholder=embed_dims_i, norm_cfg=norm_cfg))
+            norm = BuildNormalization(placeholder=embed_dims_i, norm_cfg=norm_cfg)
             self.layers.append(nn.ModuleList([patch_embed, layer, norm]))
             cur += num_layer
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''layers with zero weight decay'''
     def zerowdlayers(self):
         zwd_layers = {}
         for layer_idx, layer in enumerate(self.layers):
             assert len(layer) == 3
             for key, value in layer[0].zerowdlayers().items():
                 zwd_layers[f'MixVisionTransformer.{layer_idx}_{key}'] = value
@@ -236,19 +281,19 @@
             for key, value in layer[0].nonzerowdlayers().items():
                 nonzwd_layers[f'MixVisionTransformer.{layer_idx}_{key}'] = value
             for trans_idx, trans in enumerate(layer[1]):
                 for key, value in trans.nonzerowdlayers().items():
                     nonzwd_layers[f'MixVisionTransformer.{layer_idx}_{trans_idx}_{key}'] = value
         return nonzwd_layers
     '''init weights'''
-    def initweights(self, mit_type='', pretrained_model_path=''):
+    def initweights(self, structure_type='', pretrained_model_path=''):
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[mit_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         state_dict = self.mitconvert(state_dict)
@@ -302,67 +347,8 @@
         outs = []
         for i, layer in enumerate(self.layers):
             x, hw_shape = layer[0](x)
             for block in layer[1]: x = block(x, hw_shape)
             x = layer[2](x)
             x = nlctonchw(x, hw_shape)
             if i in self.out_indices: outs.append(x)
-        return outs
-
-
-'''BuildMixVisionTransformer'''
-def BuildMixVisionTransformer(mit_cfg):
-    # assert whether support
-    mit_type = mit_cfg.pop('type')
-    supported_mits = {
-        'mit-b0': {
-            'embed_dims': 32, 'num_stages': 4, 'num_layers': [2, 2, 2, 2], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-        'mit-b1': {
-            'embed_dims': 64, 'num_stages': 4, 'num_layers': [2, 2, 2, 2], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-        'mit-b2': {
-            'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 4, 6, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-        'mit-b3': {
-            'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 4, 18, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-        'mit-b4': {
-            'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 8, 27, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-        'mit-b5': {
-            'embed_dims': 64, 'num_stages': 4, 'num_layers': [3, 6, 40, 3], 'num_heads': [1, 2, 5, 8], 'patch_sizes': [7, 3, 3, 3],
-            'sr_ratios': [8, 4, 2, 1], 'mlp_ratio': 4, 'qkv_bias': True, 'drop_rate': 0.0, 'attn_drop_rate': 0.0, 'drop_path_rate': 0.1,
-        },
-    }
-    assert mit_type in supported_mits, 'unspport the mit_type %s' % mit_type
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3,
-        'strides': [4, 2, 2, 2],
-        'out_indices': (0, 1, 2, 3),
-        'norm_cfg': {'type': 'layernorm', 'eps': 1e-6},
-        'act_cfg': {'type': 'gelu'},
-        'pretrained': True,
-        'pretrained_model_path': '',
-        'use_checkpoint': False,
-    }
-    default_cfg.update(supported_mits[mit_type])
-    for key, value in mit_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain mit_cfg
-    mit_cfg = default_cfg.copy()
-    pretrained = mit_cfg.pop('pretrained')
-    pretrained_model_path = mit_cfg.pop('pretrained_model_path')
-    # obtain the instanced mit
-    model = MixVisionTransformer(**mit_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(mit_type, pretrained_model_path)
-    # return the model
-    return model
+        return outs
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/mobilenet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/mobilenet.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,70 +5,113 @@
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
-from .bricks import makedivisible, BuildNormalization, BuildActivation, AdptivePaddingConv2d, InvertedResidual, InvertedResidualV3, constructnormcfg
+from .bricks import makedivisible, BuildNormalization, BuildActivation, AdptivePaddingConv2d, InvertedResidual, InvertedResidualV3
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'mobilenetv2': 'https://download.openmmlab.com/mmclassification/v0/mobilenet_v2/mobilenet_v2_batch256_imagenet_20200708-3b2dc3af.pth',
     'mobilenetv3_small': 'https://download.openmmlab.com/pretrain/third_party/mobilenet_v3_small-47085aa1.pth',
     'mobilenetv3_large': 'https://download.openmmlab.com/pretrain/third_party/mobilenet_v3_large-bc2c3fd3.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''MobileNetV2'''
 class MobileNetV2(nn.Module):
     arch_settings = [[1, 16, 1], [6, 24, 2], [6, 32, 3], [6, 64, 4], [6, 96, 3], [6, 160, 3], [6, 320, 1]]
-    def __init__(self, in_channels=3, widen_factor=1, outstride=8, out_indices=(1, 2, 4, 6), norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, widen_factor=1, outstride=8, out_indices=(1, 2, 4, 6), norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'ReLU6', 'inplace': True}, pretrained=True, pretrained_model_path=''):
         super(MobileNetV2, self).__init__()
-        # set out_indices
+        # set attributes
         self.out_indices = out_indices
+        self.structure_type = structure_type
+        self.in_channels = in_channels
+        self.widen_factor = widen_factor
+        self.outstride = outstride
+        self.out_indices = out_indices
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # parse outstride
         outstride_to_strides_and_dilations = {
             8: ((1, 2, 2, 1, 1, 1, 1), (1, 1, 1, 2, 2, 4, 4)),
             16: ((1, 2, 2, 2, 1, 1, 1), (1, 1, 1, 1, 1, 2, 2)),
             32: ((1, 2, 2, 2, 1, 2, 1), (1, 1, 1, 1, 1, 1, 1)),
         }
         assert outstride in outstride_to_strides_and_dilations, 'unsupport outstride %s in MobileNetV2' % outstride
         stride_list, dilation_list = outstride_to_strides_and_dilations[outstride]
         # conv1
         self.in_channels = makedivisible(32 * widen_factor, 8)
         self.conv1 = nn.Sequential()
         self.conv1.add_module('conv', nn.Conv2d(in_channels, self.in_channels, kernel_size=3, stride=2, padding=1, bias=False))
-        self.conv1.add_module('bn', BuildNormalization(constructnormcfg(placeholder=self.in_channels, norm_cfg=norm_cfg)))
+        self.conv1.add_module('bn', BuildNormalization(placeholder=self.in_channels, norm_cfg=norm_cfg))
         self.conv1.add_module('activation', BuildActivation(act_cfg))
         # make layers
         self.layers = []
         for i, layer_cfg in enumerate(self.arch_settings):
             expand_ratio, channel, num_blocks = layer_cfg
             stride = stride_list[i]
             dilation = dilation_list[i]
             out_channels = makedivisible(channel * widen_factor, 8)
             inverted_res_layer = self.makelayer(out_channels, num_blocks, stride, dilation, expand_ratio, norm_cfg, act_cfg)
             layer_name = f'layer{i + 1}'
             self.add_module(layer_name, inverted_res_layer)
             self.layers.append(layer_name)
+        # load weights of pretrained model
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            keys = list(state_dict.keys())
+            for key in keys:
+                if key.startswith('backbone.'):
+                    value = state_dict.pop(key)
+                    key = '.'.join(key.split('.')[1:])
+                    state_dict[key] = value
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            keys = list(state_dict.keys())
+            for key in keys:
+                if key.startswith('backbone.'):
+                    value = state_dict.pop(key)
+                    key = '.'.join(key.split('.')[1:])
+                    state_dict[key] = value
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         x = self.conv1(x)
         outs = []
         for i, layer_name in enumerate(self.layers):
             layer = getattr(self, layer_name)
             x = layer(x)
             if i in self.out_indices:
                 outs.append(x)
         return tuple(outs)
     '''make layer'''
     def makelayer(self, out_channels, num_blocks, stride, dilation, expand_ratio, norm_cfg=None, act_cfg=None):
-        if act_cfg is None: act_cfg = {'type': 'relu6', 'inplace': True}
+        if act_cfg is None: act_cfg = {'type': 'ReLU6', 'inplace': True}
         layers = []
         for i in range(num_blocks):
             layers.append(
                 InvertedResidual(
                     self.in_channels, 
                     out_channels, 
                     stride=stride if i == 0 else 1, 
@@ -82,42 +125,86 @@
         return nn.Sequential(*layers)
 
 
 '''MobileNetV3'''
 class MobileNetV3(nn.Module):
     arch_settings = {
         'small': [
-            [3, 16, 16, True, {'type': 'relu'}, 2], [3, 72, 24, False, {'type': 'relu'}, 2], [3, 88, 24, False, {'type': 'relu'}, 1],
-            [5, 96, 40, True, {'type': 'hardswish'}, 2], [5, 240, 40, True, {'type': 'hardswish'}, 1], [5, 240, 40, True, {'type': 'hardswish'}, 1],
-            [5, 120, 48, True, {'type': 'hardswish'}, 1], [5, 144, 48, True, {'type': 'hardswish'}, 1], [5, 288, 96, True, {'type': 'hardswish'}, 2],
-            [5, 576, 96, True, {'type': 'hardswish'}, 1], [5, 576, 96, True, {'type': 'hardswish'}, 1],
+            [3, 16, 16, True, {'type': 'ReLU'}, 2], [3, 72, 24, False, {'type': 'ReLU'}, 2], [3, 88, 24, False, {'type': 'ReLU'}, 1],
+            [5, 96, 40, True, {'type': 'HardSwish'}, 2], [5, 240, 40, True, {'type': 'HardSwish'}, 1], [5, 240, 40, True, {'type': 'HardSwish'}, 1],
+            [5, 120, 48, True, {'type': 'HardSwish'}, 1], [5, 144, 48, True, {'type': 'HardSwish'}, 1], [5, 288, 96, True, {'type': 'HardSwish'}, 2],
+            [5, 576, 96, True, {'type': 'HardSwish'}, 1], [5, 576, 96, True, {'type': 'HardSwish'}, 1],
         ],
         'large': [
-            [3, 16, 16, False, {'type': 'relu'}, 1], [3, 64, 24, False, {'type': 'relu'}, 2], [3, 72, 24, False, {'type': 'relu'}, 1],
-            [5, 72, 40, True, {'type': 'relu'}, 2], [5, 120, 40, True, {'type': 'relu'}, 1], [5, 120, 40, True, {'type': 'relu'}, 1],
-            [3, 240, 80, False, {'type': 'hardswish'}, 2], [3, 200, 80, False, {'type': 'hardswish'}, 1], [3, 184, 80, False, {'type': 'hardswish'}, 1],
-            [3, 184, 80, False, {'type': 'hardswish'}, 1], [3, 480, 112, True, {'type': 'hardswish'}, 1], [3, 672, 112, True, {'type': 'hardswish'}, 1],
-            [5, 672, 160, True, {'type': 'hardswish'}, 2], [5, 960, 160, True, {'type': 'hardswish'}, 1], [5, 960, 160, True, {'type': 'hardswish'}, 1],
+            [3, 16, 16, False, {'type': 'ReLU'}, 1], [3, 64, 24, False, {'type': 'ReLU'}, 2], [3, 72, 24, False, {'type': 'ReLU'}, 1],
+            [5, 72, 40, True, {'type': 'ReLU'}, 2], [5, 120, 40, True, {'type': 'ReLU'}, 1], [5, 120, 40, True, {'type': 'ReLU'}, 1],
+            [3, 240, 80, False, {'type': 'HardSwish'}, 2], [3, 200, 80, False, {'type': 'HardSwish'}, 1], [3, 184, 80, False, {'type': 'HardSwish'}, 1],
+            [3, 184, 80, False, {'type': 'HardSwish'}, 1], [3, 480, 112, True, {'type': 'HardSwish'}, 1], [3, 672, 112, True, {'type': 'HardSwish'}, 1],
+            [5, 672, 160, True, {'type': 'HardSwish'}, 2], [5, 960, 160, True, {'type': 'HardSwish'}, 1], [5, 960, 160, True, {'type': 'HardSwish'}, 1],
         ],
     }
-    def __init__(self, in_channels=3, arch_type='small', outstride=8, out_indices=(0, 1, 12), reduction_factor=1, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, arch_type='large', outstride=8, out_indices=(1, 3, 16), reduction_factor=1, norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'HardSwish'}, pretrained=True, pretrained_model_path=''):
         super(MobileNetV3, self).__init__()
+        # set attributes
+        self.out_indices = out_indices
+        self.structure_type = structure_type
+        self.in_channels = in_channels
+        self.arch_type = arch_type
+        self.outstride = outstride
+        self.out_indices = out_indices
+        self.reduction_factor = reduction_factor
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
         assert arch_type in self.arch_settings
         assert isinstance(reduction_factor, int) and reduction_factor > 0
         assert outstride in [8, 16, 32], 'unsupport outstride %s in MobileNetV3' % outstride
-        self.out_indices = out_indices
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # set layers
         self.layers = self.makelayers(in_channels, arch_type, reduction_factor, outstride, norm_cfg, act_cfg)
+        # load weights of pretrained model
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            keys = list(state_dict.keys())
+            for key in keys:
+                if key.startswith('backbone.'):
+                    value = state_dict.pop(key)
+                    key = '.'.join(key.split('.')[1:])
+                    state_dict[key] = value
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            keys = list(state_dict.keys())
+            for key in keys:
+                if key.startswith('backbone.'):
+                    value = state_dict.pop(key)
+                    key = '.'.join(key.split('.')[1:])
+                    state_dict[key] = value
+            self.load_state_dict(state_dict, strict=False)
     '''make layers'''
     def makelayers(self, in_channels, arch_type, reduction_factor, outstride, norm_cfg=None, act_cfg=None):
         layers, act_cfg_default = [], act_cfg.copy()
         # build the first layer
         in_channels_first_layer, in_channels = in_channels, 16
         layer = nn.Sequential()
         layer.add_module('conv', AdptivePaddingConv2d(in_channels_first_layer, in_channels, kernel_size=3, stride=2, padding=1, bias=False))
-        layer.add_module('bn', BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg)))
+        layer.add_module('bn', BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg))
         layer.add_module('activation', BuildActivation(act_cfg_default))
         self.add_module('layer0', layer)
         layers.append('layer0')
         # build the middle layers
         layer_setting = self.arch_settings[arch_type]
         for i, params in enumerate(layer_setting):
             (kernel_size, mid_channels, out_channels, with_se, act_cfg, stride) = params
@@ -125,15 +212,15 @@
                 mid_channels = mid_channels // reduction_factor
                 out_channels = out_channels // reduction_factor
             se_cfg = None
             if with_se:
                 se_cfg = {
                     'channels': mid_channels,
                     'ratio': 4,
-                    'act_cfgs': ({'type': 'relu'}, {'type': 'hardsigmoid', 'bias': 3.0, 'divisor': 6.0})
+                    'act_cfgs': ({'type': 'ReLU'}, {'type': 'HardSigmoid', 'bias': 3.0, 'divisor': 6.0})
                 }
             layer = InvertedResidualV3(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 mid_channels=mid_channels,
                 kernel_size=kernel_size,
                 stride=stride,
@@ -146,15 +233,15 @@
             layer_name = 'layer{}'.format(i + 1)
             self.add_module(layer_name, layer)
             layers.append(layer_name)
         # build the last layer
         out_channels = 576 if arch_type == 'small' else 960
         layer = nn.Sequential()
         layer.add_module('conv', nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, dilation={8: 4, 16: 2, 32: 1}[outstride], padding=0, bias=False))
-        layer.add_module('bn', BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)))
+        layer.add_module('bn', BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg))
         layer.add_module('activation', BuildActivation(act_cfg_default))
         layer_name = 'layer{}'.format(len(layer_setting) + 1)
         self.add_module(layer_name, layer)
         layers.append(layer_name)
         # convert backbone MobileNetV3 to a semantic segmentation version
         if outstride == 32: return layers
         if arch_type == 'small':
@@ -197,84 +284,8 @@
     def forward(self, x):
         outs = []
         for i, layer_name in enumerate(self.layers):
             layer = getattr(self, layer_name)
             x = layer(x)
             if i in self.out_indices:
                 outs.append(x)
-        return tuple(outs)
-
-
-'''BuildMobileNet'''
-def BuildMobileNet(mobilenet_cfg):
-    # assert whether support
-    mobilenet_type = mobilenet_cfg.pop('type')
-    supported_mobilenets = {
-        'mobilenetv2': MobileNetV2,
-        'mobilenetv3': MobileNetV3,
-    }
-    assert mobilenet_type in supported_mobilenets, 'unsupport the mobilenet_type %s' % mobilenet_type
-    # parse cfg
-    default_cfg = dict()
-    if mobilenet_type == 'mobilenetv2':
-        default_cfg = {
-            'outstride': 8,
-            'norm_cfg': None,
-            'in_channels': 3,
-            'widen_factor': 1,
-            'pretrained': True,
-            'out_indices': (1, 2, 4, 6),
-            'pretrained_model_path': '',
-            'act_cfg': {'type': 'relu6', 'inplace': True},
-        }
-        mobilenet_type_pretrained = mobilenet_type
-    elif mobilenet_type == 'mobilenetv3':
-        default_cfg = {
-            'outstride': 8,
-            'norm_cfg': None,
-            'in_channels': 3,
-            'pretrained': True,
-            'arch_type': 'large',
-            'reduction_factor': 1,
-            'out_indices': (1, 3, 16),
-            'pretrained_model_path': '',
-            'act_cfg': {'type': 'hardswish'},
-        }
-        mobilenet_type_pretrained = 'mobilenetv3_' + mobilenet_cfg.get('arch_type', default_cfg['arch_type'])
-    for key, value in mobilenet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain mobilenet_cfg
-    mobilenet_cfg = default_cfg.copy()
-    pretrained = mobilenet_cfg.pop('pretrained')
-    pretrained_model_path = mobilenet_cfg.pop('pretrained_model_path')
-    # obtain the instanced mobilenet
-    model = supported_mobilenets[mobilenet_type](**mobilenet_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        keys = list(state_dict.keys())
-        for key in keys:
-            if key.startswith('backbone.'):
-                value = state_dict.pop(key)
-                key = '.'.join(key.split('.')[1:])
-                state_dict[key] = value
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[mobilenet_type_pretrained])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        keys = list(state_dict.keys())
-        for key in keys:
-            if key.startswith('backbone.'):
-                value = state_dict.pop(key)
-                key = '.'.join(key.split('.')[1:])
-                state_dict[key] = value
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/resnest.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/resnest.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 from .resnet import ResNet
 from .resnet import Bottleneck as _Bottleneck
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'resnest50': 'https://download.openmmlab.com/pretrain/third_party/resnest50_d2-7497a55b.pth',
     'resnest101': 'https://download.openmmlab.com/pretrain/third_party/resnest101_d2-f3b931b2.pth',
     'resnest200': 'https://download.openmmlab.com/pretrain/third_party/resnest200_d2-ca88e41f.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Radix Softmax module'''
 class RSoftmax(nn.Module):
     def __init__(self, radix, groups):
         super(RSoftmax, self).__init__()
         self.radix = radix
@@ -44,18 +46,18 @@
 '''Split-Attention Conv2d in ResNeSt'''
 class SplitAttentionConv2d(nn.Module):
     def __init__(self, in_channels, channels, kernel_size, stride=1, padding=0, dilation=1, groups=1, radix=2, reduction_factor=4, norm_cfg=None, act_cfg=None):
         super(SplitAttentionConv2d, self).__init__()
         inter_channels = max(in_channels * radix // reduction_factor, 32)
         self.radix = radix
         self.conv = nn.Conv2d(in_channels, channels * radix, kernel_size=kernel_size, stride=stride, padding=padding, dilation=dilation, groups=groups * radix, bias=False)
-        self.bn0 = BuildNormalization(constructnormcfg(placeholder=channels * radix, norm_cfg=norm_cfg))
+        self.bn0 = BuildNormalization(placeholder=channels * radix, norm_cfg=norm_cfg)
         self.relu = BuildActivation(act_cfg)
         self.fc1 = nn.Conv2d(channels, inter_channels, kernel_size=1, stride=1, padding=0, groups=groups)
-        self.bn1 = BuildNormalization(constructnormcfg(placeholder=inter_channels, norm_cfg=norm_cfg))
+        self.bn1 = BuildNormalization(placeholder=inter_channels, norm_cfg=norm_cfg)
         self.fc2 = nn.Conv2d(inter_channels, channels * radix, kernel_size=1, stride=1, padding=0, groups=groups)
         self.rsoftmax = RSoftmax(radix, groups)
     '''forward'''
     def forward(self, x):
         x = self.conv(x)
         x = self.bn0(x)
         x = self.relu(x)
@@ -86,15 +88,15 @@
     def __init__(self, inplanes, planes, groups=1, base_width=4, base_channels=64, radix=2, reduction_factor=4, use_avg_after_block_conv2=True,
                  stride=1, dilation=1, downsample=None, norm_cfg=None, act_cfg=None):
         super(Bottleneck, self).__init__(inplanes, planes, stride, dilation, downsample, norm_cfg, act_cfg)
         if groups == 1: width = planes
         else: width = math.floor(planes * (base_width / base_channels)) * groups
         self.use_avg_after_block_conv2 = use_avg_after_block_conv2 and self.stride > 1
         self.conv1 = nn.Conv2d(inplanes, width, kernel_size=1, stride=1, padding=0, bias=False)
-        self.bn1 = BuildNormalization(constructnormcfg(placeholder=width, norm_cfg=norm_cfg))
+        self.bn1 = BuildNormalization(placeholder=width, norm_cfg=norm_cfg)
         self.conv2 = SplitAttentionConv2d(
             in_channels=width, 
             channels=width, 
             kernel_size=3, 
             stride=1 if self.use_avg_after_block_conv2 else self.stride, 
             padding=dilation,
             dilation=dilation,
@@ -102,15 +104,15 @@
             radix=radix,
             reduction_factor=reduction_factor,
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
         )
         delattr(self, 'bn2')
         self.conv3 = nn.Conv2d(width, planes * self.expansion, kernel_size=1, stride=1, padding=0, bias=False)
-        self.bn3 = BuildNormalization(constructnormcfg(placeholder=planes * self.expansion, norm_cfg=norm_cfg))
+        self.bn3 = BuildNormalization(placeholder=planes * self.expansion, norm_cfg=norm_cfg)
         if self.use_avg_after_block_conv2: 
             self.avg_layer = nn.AvgPool2d(3, self.stride, padding=1)
     '''forward'''
     def forward(self, x):
         identity = x
         out = self.conv1(x)
         out = self.bn1(out)
@@ -131,100 +133,82 @@
 class ResNeSt(ResNet):
     arch_settings = {
         50: (Bottleneck, (3, 4, 6, 3)),
         101: (Bottleneck, (3, 4, 23, 3)),
         152: (Bottleneck, (3, 8, 36, 3)),
         200: (Bottleneck, (3, 24, 36, 3))
     }
-    def __init__(self, groups=1, base_width=4, radix=2, reduction_factor=4, use_avg_after_block_conv2=True,
-                 in_channels=3, base_channels=64, stem_channels=64, depth=101, outstride=8, contract_dilation=True, use_stem=True, 
-                 out_indices=(0, 1, 2, 3), use_avg_for_downsample=False, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, groups=1, base_width=4, radix=2, reduction_factor=4, use_avg_after_block_conv2=True,
+                 in_channels=3, base_channels=64, stem_channels=128, depth=101, outstride=8, contract_dilation=True, use_conv3x3_stem=True, 
+                 out_indices=(0, 1, 2, 3), use_avg_for_downsample=True, norm_cfg={'type': 'SyncBatchNorm'}, act_cfg={'type': 'ReLU', 'inplace': True}, 
+                 pretrained=True, pretrained_model_path=''):
         self.extra_args_for_makelayer = {
             'radix': radix,
             'groups': groups,
             'base_width': base_width,
             'reduction_factor': reduction_factor,
             'base_channels': base_channels,
             'use_avg_after_block_conv2': use_avg_after_block_conv2,
         }
-        super(ResNeSt, self).__init__(in_channels, base_channels, stem_channels, depth, outstride, contract_dilation, use_stem, out_indices, use_avg_for_downsample, norm_cfg, act_cfg)
+        super(ResNeSt, self).__init__(structure_type, in_channels, base_channels, stem_channels, depth, outstride, contract_dilation, use_conv3x3_stem, out_indices, use_avg_for_downsample, norm_cfg, act_cfg, False, '')
+        # set attributes
+        self.structure_type = structure_type
+        self.groups = groups
+        self.base_width = base_width
+        self.radix = radix
+        self.reduction_factor = reduction_factor
+        self.use_avg_after_block_conv2 = use_avg_after_block_conv2
+        self.in_channels = in_channels
+        self.base_channels = base_channels
+        self.stem_channels = stem_channels
+        self.depth = depth
+        self.outstride = outstride
+        self.contract_dilation = contract_dilation
+        self.use_conv3x3_stem = use_conv3x3_stem
+        self.out_indices = out_indices
+        self.use_avg_for_downsample = use_avg_for_downsample
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''make res layer'''
     def makelayer(self, block, inplanes, planes, num_blocks, stride=1, dilation=1, contract_dilation=True, use_avg_for_downsample=False, norm_cfg=None, act_cfg=None):
         downsample = None
         dilations = [dilation] * num_blocks
         if contract_dilation and dilation > 1: dilations[0] = dilation // 2
         if stride != 1 or inplanes != planes * block.expansion:
             if use_avg_for_downsample:
                 downsample = nn.Sequential(
                     nn.AvgPool2d(kernel_size=stride, stride=stride, ceil_mode=True, count_include_pad=False),
                     nn.Conv2d(inplanes, planes * block.expansion, kernel_size=1, stride=1, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=planes * block.expansion, norm_cfg=norm_cfg))
+                    BuildNormalization(placeholder=planes * block.expansion, norm_cfg=norm_cfg)
                 )
             else:
                 downsample = nn.Sequential(
                     nn.Conv2d(inplanes, planes * block.expansion, kernel_size=1, stride=stride, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=planes * block.expansion, norm_cfg=norm_cfg))
+                    BuildNormalization(placeholder=planes * block.expansion, norm_cfg=norm_cfg)
                 )
         layers = []
         layers.append(block(inplanes, planes, stride=stride, dilation=dilations[0], downsample=downsample, norm_cfg=norm_cfg, act_cfg=act_cfg, **self.extra_args_for_makelayer))
         self.inplanes = planes * block.expansion
         for i in range(1, num_blocks): 
             layers.append(block(planes * block.expansion, planes, stride=1, dilation=dilations[i], norm_cfg=norm_cfg, act_cfg=act_cfg, **self.extra_args_for_makelayer))
-        return nn.Sequential(*layers)
-
-
-'''BuildResNeSt'''
-def BuildResNeSt(resnest_cfg):
-    # assert whether support
-    resnest_type = resnest_cfg.pop('type')
-    supported_resnests = {
-        'resnest50': {'depth': 50}, 'resnest101': {'depth': 101},
-        'resnest152': {'depth': 152}, 'resnest200': {'depth': 200},
-    }
-    assert resnest_type in supported_resnests, 'unsupport the resnest_type %s' % resnest_type
-    # parse cfg
-    default_cfg = {
-        'radix': 2,
-        'groups': 1,
-        'outstride': 8,
-        'base_width': 4,
-        'use_stem': True,
-        'norm_cfg': None,
-        'in_channels': 3,
-        'pretrained': True,
-        'base_channels': 64,
-        'stem_channels': 128,
-        'reduction_factor': 4,
-        'contract_dilation': True,
-        'out_indices': (0, 1, 2, 3),
-        'pretrained_model_path': '',
-        'use_avg_for_downsample': True,
-        'use_avg_after_block_conv2': True,
-        'act_cfg': {'type': 'relu', 'inplace': True},
-    }
-    for key, value in resnest_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain resnest_cfg
-    resnest_cfg = default_cfg.copy()
-    resnest_cfg.update(supported_resnests[resnest_type])
-    pretrained = resnest_cfg.pop('pretrained')
-    pretrained_model_path = resnest_cfg.pop('pretrained_model_path')
-    # obtain the instanced resnest
-    model = ResNeSt(**resnest_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[resnest_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return nn.Sequential(*layers)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/resnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/resnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,41 @@
 Author:
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'resnet18': 'https://download.pytorch.org/models/resnet18-5c106cde.pth',
     'resnet34': 'https://download.pytorch.org/models/resnet34-333f7ec4.pth',
     'resnet50': 'https://download.pytorch.org/models/resnet50-19c8e357.pth',
     'resnet101': 'https://download.pytorch.org/models/resnet101-5d3b4d8f.pth',
     'resnet152': 'https://download.pytorch.org/models/resnet152-b121ed2d.pth',
-    'resnet18stem': 'https://download.openmmlab.com/pretrain/third_party/resnet18_v1c-b5776b93.pth',
-    'resnet50stem': 'https://download.openmmlab.com/pretrain/third_party/resnet50_v1c-2cccc1ad.pth',
-    'resnet101stem': 'https://download.openmmlab.com/pretrain/third_party/resnet101_v1c-e67eebb6.pth',
+    'resnet18conv3x3stem': 'https://download.openmmlab.com/pretrain/third_party/resnet18_v1c-b5776b93.pth',
+    'resnet50conv3x3stem': 'https://download.openmmlab.com/pretrain/third_party/resnet50_v1c-2cccc1ad.pth',
+    'resnet101conv3x3stem': 'https://download.openmmlab.com/pretrain/third_party/resnet101_v1c-e67eebb6.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''BasicBlock'''
 class BasicBlock(nn.Module):
     expansion = 1
     def __init__(self, inplanes, planes, stride=1, dilation=1, downsample=None, norm_cfg=None, act_cfg=None):
         super(BasicBlock, self).__init__()
         self.conv1 = nn.Conv2d(inplanes, planes, kernel_size=3, stride=stride, padding=dilation, dilation=dilation, bias=False)
-        self.bn1 = BuildNormalization(constructnormcfg(placeholder=planes, norm_cfg=norm_cfg))
+        self.bn1 = BuildNormalization(placeholder=planes, norm_cfg=norm_cfg)
         self.conv2 = nn.Conv2d(planes, planes, kernel_size=3, stride=1, padding=1, bias=False)
-        self.bn2 = BuildNormalization(constructnormcfg(placeholder=planes, norm_cfg=norm_cfg))
+        self.bn2 = BuildNormalization(placeholder=planes, norm_cfg=norm_cfg)
         self.relu = BuildActivation(act_cfg)
         self.downsample = downsample
         self.stride = stride
         self.dilation = dilation
     '''forward'''
     def forward(self, x):
         identity = x
@@ -53,19 +55,19 @@
 
 '''Bottleneck'''
 class Bottleneck(nn.Module):
     expansion = 4
     def __init__(self, inplanes, planes, stride=1, dilation=1, downsample=None, norm_cfg=None, act_cfg=None):
         super(Bottleneck, self).__init__()
         self.conv1 = nn.Conv2d(inplanes, planes, kernel_size=1, stride=1, padding=0, bias=False)
-        self.bn1 = BuildNormalization(constructnormcfg(placeholder=planes, norm_cfg=norm_cfg))
+        self.bn1 = BuildNormalization(placeholder=planes, norm_cfg=norm_cfg)
         self.conv2 = nn.Conv2d(planes, planes, kernel_size=3, stride=stride, padding=dilation, dilation=dilation, bias=False)
-        self.bn2 = BuildNormalization(constructnormcfg(placeholder=planes, norm_cfg=norm_cfg))
+        self.bn2 = BuildNormalization(placeholder=planes, norm_cfg=norm_cfg)
         self.conv3 = nn.Conv2d(planes, planes * self.expansion, kernel_size=1, stride=1, padding=0, bias=False)
-        self.bn3 = BuildNormalization(constructnormcfg(placeholder=planes * self.expansion, norm_cfg=norm_cfg))
+        self.bn3 = BuildNormalization(placeholder=planes * self.expansion, norm_cfg=norm_cfg)
         self.relu = BuildActivation(act_cfg)
         self.downsample = downsample
         self.stride = stride
         self.dilation = dilation
     '''forward'''
     def forward(self, x):
         identity = x
@@ -88,48 +90,65 @@
     arch_settings = {
         18: (BasicBlock, (2, 2, 2, 2)),
         34: (BasicBlock, (3, 4, 6, 3)),
         50: (Bottleneck, (3, 4, 6, 3)),
         101: (Bottleneck, (3, 4, 23, 3)),
         152: (Bottleneck, (3, 8, 36, 3))
     }
-    def __init__(self, in_channels=3, base_channels=64, stem_channels=64, depth=101, outstride=8, contract_dilation=True, use_stem=True, 
-                 out_indices=(0, 1, 2, 3), use_avg_for_downsample=False, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, base_channels=64, stem_channels=64, depth=101, outstride=8, contract_dilation=True, use_conv3x3_stem=True, 
+                 out_indices=(0, 1, 2, 3), use_avg_for_downsample=False, norm_cfg={'type': 'SyncBatchNorm'}, act_cfg={'type': 'ReLU', 'inplace': True}, 
+                 pretrained=True, pretrained_model_path=''):
         super(ResNet, self).__init__()
-        self.inplanes = stem_channels
-        # set out_indices
+        # set attributes
+        self.structure_type = structure_type
+        self.in_channels = in_channels
+        self.base_channels = base_channels
+        self.stem_channels = stem_channels
+        self.depth = depth
+        self.outstride = outstride
+        self.contract_dilation = contract_dilation
+        self.use_conv3x3_stem = use_conv3x3_stem
         self.out_indices = out_indices
+        self.use_avg_for_downsample = use_avg_for_downsample
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        self.inplanes = stem_channels
         # parse depth settings
         assert depth in self.arch_settings, 'unsupport depth %s' % depth
         block, num_blocks_list = self.arch_settings[depth]
         # parse outstride
         outstride_to_strides_and_dilations = {
             8: ((1, 2, 1, 1), (1, 1, 2, 4)),
             16: ((1, 2, 2, 1), (1, 1, 1, 2)),
             32: ((1, 2, 2, 2), (1, 1, 1, 1)),
         }
         assert outstride in outstride_to_strides_and_dilations, 'unsupport outstride %s' % outstride
         stride_list, dilation_list = outstride_to_strides_and_dilations[outstride]
         # whether replace the 7x7 conv in the input stem with three 3x3 convs
-        self.use_stem = use_stem
-        if use_stem:
+        if use_conv3x3_stem:
             self.stem = nn.Sequential(
                 nn.Conv2d(in_channels, stem_channels // 2, kernel_size=3, stride=2, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=stem_channels // 2, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=stem_channels // 2, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(stem_channels // 2, stem_channels // 2, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=stem_channels // 2, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=stem_channels // 2, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(stem_channels // 2, stem_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=stem_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=stem_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
         else:
             self.conv1 = nn.Conv2d(in_channels, stem_channels, kernel_size=7, stride=2, padding=3, bias=False)
-            self.bn1 = BuildNormalization(constructnormcfg(placeholder=stem_channels, norm_cfg=norm_cfg))
+            self.bn1 = BuildNormalization(placeholder=stem_channels, norm_cfg=norm_cfg)
             self.relu = BuildActivation(act_cfg)
         self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
         # make layers
         self.layer1 = self.makelayer(
             block=block, 
             inplanes=stem_channels, 
             planes=base_channels, 
@@ -173,102 +192,62 @@
             stride=stride_list[3], 
             dilation=dilation_list[3], 
             contract_dilation=contract_dilation, 
             use_avg_for_downsample=use_avg_for_downsample,
             norm_cfg=norm_cfg, 
             act_cfg=act_cfg,
         )
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''make res layer'''
     def makelayer(self, block, inplanes, planes, num_blocks, stride=1, dilation=1, contract_dilation=True, use_avg_for_downsample=False, norm_cfg=None, act_cfg=None):
         downsample = None
         dilations = [dilation] * num_blocks
         if contract_dilation and dilation > 1: dilations[0] = dilation // 2
         if stride != 1 or inplanes != planes * block.expansion:
             if use_avg_for_downsample:
                 downsample = nn.Sequential(
                     nn.AvgPool2d(kernel_size=stride, stride=stride, ceil_mode=True, count_include_pad=False),
                     nn.Conv2d(inplanes, planes * block.expansion, kernel_size=1, stride=1, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=planes * block.expansion, norm_cfg=norm_cfg))
+                    BuildNormalization(placeholder=planes * block.expansion, norm_cfg=norm_cfg)
                 )
             else:
                 downsample = nn.Sequential(
                     nn.Conv2d(inplanes, planes * block.expansion, kernel_size=1, stride=stride, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=planes * block.expansion, norm_cfg=norm_cfg))
+                    BuildNormalization(placeholder=planes * block.expansion, norm_cfg=norm_cfg)
                 )
         layers = []
         layers.append(block(inplanes, planes, stride=stride, dilation=dilations[0], downsample=downsample, norm_cfg=norm_cfg, act_cfg=act_cfg))
         self.inplanes = planes * block.expansion
         for i in range(1, num_blocks): 
             layers.append(block(planes * block.expansion, planes, stride=1, dilation=dilations[i], norm_cfg=norm_cfg, act_cfg=act_cfg))
         return nn.Sequential(*layers)
     '''forward'''
     def forward(self, x):
-        if self.use_stem:
+        if self.use_conv3x3_stem:
             x = self.stem(x)
         else:
             x = self.conv1(x)
             x = self.bn1(x)
             x = self.relu(x)
         x = self.maxpool(x)
         x1 = self.layer1(x)
         x2 = self.layer2(x1)
         x3 = self.layer3(x2)
         x4 = self.layer4(x3)
         outs = []
         for i, feats in enumerate([x1, x2, x3, x4]):
             if i in self.out_indices: outs.append(feats)
-        return tuple(outs)
-
-
-'''BuildResNet'''
-def BuildResNet(resnet_cfg):
-    # assert whether support
-    resnet_type = resnet_cfg.pop('type')
-    supported_resnets = {
-        'resnet18': {'depth': 18}, 'resnet34': {'depth': 34}, 'resnet50': {'depth': 50},
-        'resnet101': {'depth': 101}, 'resnet152': {'depth': 152},
-    }
-    assert resnet_type in supported_resnets, 'unsupport the resnet_type %s' % resnet_type
-    # parse cfg
-    default_cfg = {
-        'outstride': 8,
-        'use_stem': True,
-        'norm_cfg': None,
-        'in_channels': 3,
-        'pretrained': True,
-        'base_channels': 64,
-        'stem_channels': 64,
-        'contract_dilation': True,
-        'out_indices': (0, 1, 2, 3),
-        'pretrained_model_path': '',
-        'use_avg_for_downsample': False,
-        'act_cfg': {'type': 'relu', 'inplace': True},
-    }
-    for key, value in resnet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain resnet_cfg
-    resnet_cfg = default_cfg.copy()
-    resnet_cfg.update(supported_resnets[resnet_type])
-    pretrained = resnet_cfg.pop('pretrained')
-    pretrained_model_path = resnet_cfg.pop('pretrained_model_path')
-    # obtain the instanced resnet
-    model = ResNet(**resnet_cfg)
-    # load weights of pretrained model
-    if resnet_cfg['use_stem']: 
-        resnet_type = resnet_type + 'stem'
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[resnet_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/swin.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/swin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,65 @@
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 import torch.utils.checkpoint as checkpoint
 from collections import OrderedDict
 from .bricks import PatchEmbed as PatchEmbedBase
 from .bricks import PatchMerging as PatchMergingBase
-from .bricks import BuildNormalization, BuildDropout, FFN, constructnormcfg
+from .bricks import BuildNormalization, BuildDropout, FFN
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'swin_tiny_patch4_window7_224': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_tiny_patch4_window7_224.pth',
     'swin_small_patch4_window7_224': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_small_patch4_window7_224.pth',
     'swin_base_patch4_window12_384': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_base_patch4_window12_384.pth',
     'swin_base_patch4_window7_224': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_base_patch4_window7_224.pth',
     'swin_base_patch4_window12_384_22k': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_base_patch4_window12_384_22k.pth',
     'swin_base_patch4_window7_224_22k': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_base_patch4_window7_224_22k.pth',
     'swin_large_patch4_window12_384_22k': 'https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_large_patch4_window12_384_22k.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {
+    'swin_tiny_patch4_window7_224': {
+        'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 96, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4, 
+        'depths': [2, 2, 6, 2], 'num_heads': [3, 6, 12, 24], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True, 
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_small_patch4_window7_224': {
+        'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 96, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [3, 6, 12, 24], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_base_patch4_window12_384': {
+        'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_base_patch4_window7_224': {
+        'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_base_patch4_window12_384_22k': {
+        'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_base_patch4_window7_224_22k': {
+        'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+    'swin_large_patch4_window12_384_22k': {
+        'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 192, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
+        'depths': [2, 2, 18, 2], 'num_heads': [6, 12, 24, 48], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
+        'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
+    },
+}
 
 
 '''PatchMerging'''
 class PatchMerging(PatchMergingBase):
     def __init__(self, **kwargs):
         super(PatchMerging, self).__init__(**kwargs)
     '''layers with zero weight decay'''
@@ -213,24 +251,24 @@
 
 '''SwinBlock'''
 class SwinBlock(nn.Module):
     def __init__(self, embed_dims, num_heads, feedforward_channels, window_size=7, shift=False, qkv_bias=True, qk_scale=None, drop_rate=0., 
                  attn_drop_rate=0., drop_path_rate=0., act_cfg=None, norm_cfg=None, use_checkpoint=False):
         super(SwinBlock, self).__init__()
         self.use_checkpoint = use_checkpoint
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.attn = ShiftWindowMSA(
             embed_dims=embed_dims, num_heads=num_heads, window_size=window_size, shift_size=window_size // 2 if shift else 0,
             qkv_bias=qkv_bias, qk_scale=qk_scale, attn_drop_rate=attn_drop_rate, proj_drop_rate=drop_rate,
-            dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
         )
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm2 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.ffn = FFN(
             embed_dims=embed_dims, feedforward_channels=feedforward_channels, num_fcs=2,
-            ffn_drop=drop_rate, dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            ffn_drop=drop_rate, dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
             act_cfg=act_cfg, add_identity=True,
         )
     '''layers with zero weight decay'''
     def zerowdlayers(self, apply_wd_to_relative_position_bias_table=True):
         # Note: our experiments find that do not set the weight decay of relative_position_bias_table as zero can achieve better segmentation performance
         if apply_wd_to_relative_position_bias_table: return {'SwinBlock.norm1': self.norm1, 'SwinBlock.norm2': self.norm2}
         layers = {'SwinBlock.norm1': self.norm1, 'SwinBlock.norm2': self.norm2}
@@ -325,24 +363,50 @@
             return x_down, down_hw_shape, x, hw_shape
         else:
             return x, hw_shape, x, hw_shape
 
 
 '''SwinTransformer'''
 class SwinTransformer(nn.Module):
-    def __init__(self, pretrain_img_size=224, in_channels=3, embed_dims=96, patch_size=4, window_size=7, mlp_ratio=4, depths=(2, 2, 6, 2), num_heads=(3, 6, 12, 24),
+    def __init__(self, structure_type, pretrain_img_size=224, in_channels=3, embed_dims=96, patch_size=4, window_size=7, mlp_ratio=4, depths=(2, 2, 6, 2), num_heads=(3, 6, 12, 24),
                  strides=(4, 2, 2, 2), out_indices=(0, 1, 2, 3), qkv_bias=True, qk_scale=None, patch_norm=True, drop_rate=0., attn_drop_rate=0., drop_path_rate=0.1,
-                 use_abs_pos_embed=False, act_cfg=None, norm_cfg=None, use_checkpoint=False):
+                 use_abs_pos_embed=False, act_cfg={'type': 'GELU'}, norm_cfg={'type': 'LayerNorm'}, use_checkpoint=False, pretrained=True, pretrained_model_path=''):
         super(SwinTransformer, self).__init__()
-        if isinstance(pretrain_img_size, int):
-            pretrain_img_size = (pretrain_img_size, pretrain_img_size)
-        num_layers = len(depths)
+        # set attributes
+        self.structure_type = structure_type
+        self.pretrain_img_size = pretrain_img_size
+        self.in_channels = in_channels
+        self.embed_dims = embed_dims
+        self.patch_size = patch_size
+        self.window_size = window_size
+        self.mlp_ratio = mlp_ratio
+        self.depths = depths
+        self.num_heads = num_heads
+        self.strides = strides
         self.out_indices = out_indices
+        self.qkv_bias = qkv_bias
+        self.qk_scale = qk_scale
+        self.patch_norm = patch_norm
+        self.drop_rate = drop_rate
+        self.attn_drop_rate = attn_drop_rate
+        self.drop_path_rate = drop_path_rate
+        self.act_cfg = act_cfg
+        self.norm_cfg = norm_cfg
         self.use_abs_pos_embed = use_abs_pos_embed
+        self.use_checkpoint = use_checkpoint
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
         assert strides[0] == patch_size, 'Use non-overlapping patch embed.'
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        if isinstance(pretrain_img_size, int): pretrain_img_size = (pretrain_img_size, pretrain_img_size)
+        self.pretrain_img_size = pretrain_img_size
+        # patch embedding
         self.patch_embed = PatchEmbed(
             in_channels=in_channels,
             embed_dims=embed_dims,
             kernel_size=patch_size,
             stride=strides[0],
             padding='corner',
             norm_cfg=norm_cfg if patch_norm else None,
@@ -354,14 +418,15 @@
             self.absolute_pos_embed = nn.Parameter(torch.zeros((1, num_patches, embed_dims)))
         self.drop_after_pos = nn.Dropout(p=drop_rate)
         # stochastic depth
         total_depth = sum(depths)
         dpr = [x.item() for x in torch.linspace(0, drop_path_rate, total_depth)]
         self.stages = nn.ModuleList()
         in_channels = embed_dims
+        num_layers = len(depths)
         for i in range(num_layers):
             if i < num_layers - 1:
                 downsample = PatchMerging(
                     in_channels=in_channels,
                     out_channels=2 * in_channels,
                     stride=strides[i + 1],
                     norm_cfg=norm_cfg if patch_norm else None,
@@ -376,24 +441,27 @@
             )
             self.stages.append(stage)
             if downsample:
                 in_channels = downsample.out_channels
         self.num_features = [int(embed_dims * 2**i) for i in range(num_layers)]
         # add a norm layer for each output
         for i in out_indices:
-            layer = BuildNormalization(constructnormcfg(placeholder=self.num_features[i], norm_cfg=norm_cfg))
+            layer = BuildNormalization(placeholder=self.num_features[i], norm_cfg=norm_cfg)
             layer_name = f'norm{i}'
             self.add_module(layer_name, layer)
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''initialize backbone'''
-    def initweights(self, swin_type='swin_tiny_patch4_window7_224', pretrained_model_path=''):
+    def initweights(self, structure_type='swin_tiny_patch4_window7_224', pretrained_model_path=''):
         # load
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[swin_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         # be consistent
@@ -516,77 +584,8 @@
         for i, stage in enumerate(self.stages):
             x, hw_shape, out, out_hw_shape = stage(x, hw_shape)
             if i in self.out_indices:
                 norm_layer = getattr(self, f'norm{i}')
                 out = norm_layer(out)
                 out = out.view(-1, *out_hw_shape, self.num_features[i]).permute(0, 3, 1, 2).contiguous()
                 outs.append(out)
-        return outs
-
-
-'''BuildSwinTransformer'''
-def BuildSwinTransformer(swin_cfg):
-    # assert whether support
-    swin_type = swin_cfg.pop('type')
-    supported_swins = {
-        'swin_tiny_patch4_window7_224': {
-            'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 96, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4, 
-            'depths': [2, 2, 6, 2], 'num_heads': [3, 6, 12, 24], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True, 
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_small_patch4_window7_224': {
-            'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 96, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [3, 6, 12, 24], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_base_patch4_window12_384': {
-            'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_base_patch4_window7_224': {
-            'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_base_patch4_window12_384_22k': {
-            'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_base_patch4_window7_224_22k': {
-            'pretrain_img_size': 224, 'in_channels': 3, 'embed_dims': 128, 'patch_size': 4, 'window_size': 7, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [4, 8, 16, 32], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-        'swin_large_patch4_window12_384_22k': {
-            'pretrain_img_size': 384, 'in_channels': 3, 'embed_dims': 192, 'patch_size': 4, 'window_size': 12, 'mlp_ratio': 4,
-            'depths': [2, 2, 18, 2], 'num_heads': [6, 12, 24, 48], 'qkv_bias': True, 'qk_scale': None, 'patch_norm': True,
-            'drop_rate': 0., 'attn_drop_rate': 0., 'drop_path_rate': 0.3, 'use_abs_pos_embed': False,
-        },
-    }
-    assert swin_type in supported_swins, 'unsupport the swin_type %s' % swin_type
-    # parse cfg
-    default_cfg = {
-        'strides': (4, 2, 2, 2),
-        'out_indices': (0, 1, 2, 3),
-        'norm_cfg': {'type': 'layernorm'},
-        'act_cfg': {'type': 'gelu'},
-        'pretrained': True,
-        'pretrained_model_path': '',
-        'use_checkpoint': False,
-    }
-    default_cfg.update(supported_swins[swin_type])
-    for key, value in swin_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain swin_cfg
-    swin_cfg = default_cfg.copy()
-    pretrained = swin_cfg.pop('pretrained')
-    pretrained_model_path = swin_cfg.pop('pretrained_model_path')
-    # obtain the instanced swin
-    model = SwinTransformer(**swin_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(swin_type, pretrained_model_path)
-    # return the model
-    return model
+        return outs
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/twins.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/twins.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,35 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 from collections import OrderedDict
 from .mit import EfficientMultiheadAttention
 from .bricks import PatchEmbed as PatchEmbedBase
-from .bricks import BuildNormalization, FFN, BuildDropout, constructnormcfg
+from .bricks import BuildNormalization, FFN, BuildDropout
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'pcpvt_small': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/pcpvt_small.pth',
     'pcpvt_base': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/pcpvt_base.pth',
     'pcpvt_large': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/pcpvt_large.pth',
     'svt_small': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/alt_gvt_small.pth',
     'svt_base': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/alt_gvt_base.pth',
     'svt_large': 'https://github.com/SegmentationBLWX/modelstore/releases/download/ssseg_twins/alt_gvt_large.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {
+    'pcpvt_small': {'depths': [3, 4, 6, 3], 'drop_path_rate': 0.2},
+    'pcpvt_base': {'depths': [3, 4, 18, 3], 'drop_path_rate': 0.3},
+    'pcpvt_large': {'depths': [3, 8, 27, 3], 'drop_path_rate': 0.3},
+    'svt_small': {'embed_dims': [64, 128, 256, 512], 'num_heads': [2, 4, 8, 16], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 10, 4], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.2},
+    'svt_base': {'embed_dims': [96, 192, 384, 768], 'num_heads': [3, 6, 12, 24], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 18, 2], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.2},
+    'svt_large': {'embed_dims': [128, 256, 512, 1024], 'num_heads': [4, 8, 16, 32], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 18, 2], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.3},
+}
 
 
 '''PatchEmbed'''
 class PatchEmbed(PatchEmbedBase):
     def __init__(self, **kwargs):
         super(PatchEmbed, self).__init__(**kwargs)
     '''layers with zero weight decay'''
@@ -57,21 +66,21 @@
 
 
 '''GSAEncoderLayer'''
 class GSAEncoderLayer(nn.Module):
     def __init__(self, embed_dims, num_heads, feedforward_channels, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., num_fcs=2, 
                  qkv_bias=True, act_cfg=None, norm_cfg=None, sr_ratio=1., dropout_cfg=None):
         super(GSAEncoderLayer, self).__init__()
-        if dropout_cfg is None: dropout_cfg = {'type': 'droppath', 'drop_prob': drop_path_rate}
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        if dropout_cfg is None: dropout_cfg = {'type': 'DropPath', 'drop_prob': drop_path_rate}
+        self.norm1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.attn = GlobalSubsampledAttention(
             embed_dims=embed_dims, num_heads=num_heads, attn_drop=attn_drop_rate, proj_drop=drop_rate, 
             dropout_cfg=dropout_cfg, qkv_bias=qkv_bias, norm_cfg=norm_cfg, sr_ratio=sr_ratio
         )
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm2 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.ffn = FFN(
             embed_dims=embed_dims, feedforward_channels=feedforward_channels, num_fcs=num_fcs, ffn_drop=drop_rate,
             dropout_cfg=dropout_cfg, act_cfg=act_cfg, add_identity=False,
         )
         self.drop_path = BuildDropout(dropout_cfg) if (dropout_cfg and (drop_path_rate > 0.)) else nn.Identity()
     '''forward'''
     def forward(self, x, hw_shape):
@@ -154,18 +163,18 @@
 
 
 '''LSAEncoderLayer'''
 class LSAEncoderLayer(nn.Module):
     def __init__(self, embed_dims, num_heads, feedforward_channels, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., 
                  num_fcs=2, qkv_bias=True, qk_scale=None, act_cfg=None, norm_cfg=None, window_size=1, dropout_cfg=None):
         super(LSAEncoderLayer, self).__init__()
-        if dropout_cfg is None: dropout_cfg = {'type': 'droppath', 'drop_prob': drop_path_rate}
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        if dropout_cfg is None: dropout_cfg = {'type': 'DropPath', 'drop_prob': drop_path_rate}
+        self.norm1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.attn = LocallyGroupedSelfAttention(embed_dims, num_heads, qkv_bias, qk_scale, attn_drop_rate, drop_rate, window_size)
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.norm2 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         self.ffn = FFN(
             embed_dims=embed_dims, feedforward_channels=feedforward_channels, num_fcs=num_fcs, ffn_drop=drop_rate,
             dropout_cfg=dropout_cfg, act_cfg=act_cfg, add_identity=False,
         )
         self.drop_path = BuildDropout(dropout_cfg) if (dropout_cfg and (drop_path_rate > 0.)) else nn.Identity()
     '''forward'''
     def forward(self, x, hw_shape):
@@ -208,22 +217,42 @@
     '''layers with non zero weight decay'''
     def nonzerowdlayers(self):
         return {'ConditionalPositionEncoding.proj': self.proj}
 
 
 '''Twins-PCPVT'''
 class PCPVT(nn.Module):
-    def __init__(self, in_channels=3, embed_dims=[64, 128, 256, 512], patch_sizes=[4, 2, 2, 2], strides=[4, 2, 2, 2], num_heads=[1, 2, 4, 8], mlp_ratios=[4, 4, 4, 4],
-                 out_indices=(0, 1, 2, 3), qkv_bias=False, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., depths=[3, 4, 6, 3], sr_ratios=[8, 4, 2, 1],
-                 norm_after_stage=False, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, embed_dims=[64, 128, 320, 512], patch_sizes=[4, 2, 2, 2], strides=[4, 2, 2, 2], num_heads=[1, 2, 5, 8], 
+                 mlp_ratios=[8, 8, 4, 4], out_indices=(0, 1, 2, 3), qkv_bias=True, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., depths=[3, 4, 6, 3], 
+                 sr_ratios=[8, 4, 2, 1], norm_after_stage=False, norm_cfg={'type': 'LayerNorm'}, act_cfg={'type': 'GELU'}, pretrained=True, pretrained_model_path=''):
         super(PCPVT, self).__init__()
         # set attributes
-        self.depths = depths
+        self.structure_type = structure_type
+        self.in_channels = in_channels
+        self.embed_dims = embed_dims
+        self.patch_sizes = patch_sizes
+        self.strides = strides
+        self.num_heads = num_heads
+        self.mlp_ratios = mlp_ratios
         self.out_indices = out_indices
+        self.qkv_bias = qkv_bias
+        self.drop_rate = drop_rate
+        self.attn_drop_rate = attn_drop_rate
+        self.drop_path_rate = drop_path_rate
+        self.depths = depths
+        self.sr_ratios = sr_ratios
         self.norm_after_stage = norm_after_stage
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # patch embed
         self.patch_embeds = nn.ModuleList()
         self.position_encoding_drops = nn.ModuleList()
         for i in range(len(depths)):
             self.patch_embeds.append(PatchEmbed(
                 in_channels=in_channels if i == 0 else embed_dims[i - 1], embed_dims=embed_dims[i],
                 kernel_size=patch_sizes[i], stride=strides[i], padding='corner', norm_cfg=norm_cfg
@@ -244,15 +273,18 @@
             ])
             self.layers.append(_block)
             cur += depths[k]
         # norm
         if self.norm_after_stage:
             self.norm_list = nn.ModuleList()
             for dim in embed_dims: 
-                self.norm_list.append(BuildNormalization(constructnormcfg(placeholder=dim, norm_cfg=norm_cfg)))
+                self.norm_list.append(BuildNormalization(placeholder=dim, norm_cfg=norm_cfg))
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''forward'''
     def forward(self, x):
         outputs, b = list(), x.shape[0]
         for i in range(len(self.depths)):
             x, hw_shape = self.patch_embeds[i](x)
             h, w = hw_shape
             x = self.position_encoding_drops[i](x)
@@ -296,33 +328,33 @@
                 layers[f'PCPVT.{key}.{layer_idx}'] = value
         for layer_idx, layer in enumerate(self.patch_embeds):
             for key, value in layer.nonzerowdlayers().items():
                 assert f'PCPVT.{key}.{layer_idx}' not in layers
                 layers[f'PCPVT.{key}.{layer_idx}'] = value
         return layers
     '''initialize backbone'''
-    def initweights(self, twins_type='pcpvt_small', pretrained_model_path=''):
+    def initweights(self, structure_type='pcpvt_small', pretrained_model_path=''):
         # load
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[twins_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         # be consistent
-        state_dict = self.twinsconvert(twins_type, state_dict)
+        state_dict = self.twinsconvert(structure_type, state_dict)
         # load state_dict
         self.load_state_dict(state_dict, strict=False)
     '''twins convert'''
     @staticmethod
-    def twinsconvert(twins_type, ckpt):
+    def twinsconvert(structure_type, ckpt):
         new_ckpt = OrderedDict()
         for k, v in list(ckpt.items()):
             new_v = v
             if k.startswith('head'): continue
             elif k.startswith('patch_embeds'):
                 if 'proj.' in k: new_k = k.replace('proj.', 'projection.')
                 else: new_k = k
@@ -330,15 +362,15 @@
                 if 'attn.q.' in k:
                     new_k = k.replace('q.', 'attn.in_proj_')
                     new_v = torch.cat([v, ckpt[k.replace('attn.q.', 'attn.kv.')]], dim=0)
                 elif 'mlp.fc1' in k:
                     new_k = k.replace('mlp.fc1', 'ffn.layers.0.0')
                 elif 'mlp.fc2' in k:
                     new_k = k.replace('mlp.fc2', 'ffn.layers.1')
-                elif twins_type.startswith('pcpvt'):
+                elif structure_type.startswith('pcpvt'):
                     if 'attn.proj.' in k: new_k = k.replace('proj.', 'attn.out_proj.')
                     else: new_k = k
                 else:
                     if 'attn.proj.' in k:
                         k_lst = k.split('.')
                         if int(k_lst[2]) % 2 == 1: new_k = k.replace('proj.', 'attn.out_proj.')
                         else: new_k = k
@@ -352,102 +384,30 @@
                 new_k = k
             if 'attn.kv.' not in k: new_ckpt[new_k] = new_v
         return new_ckpt
 
 
 '''Twins-SVT'''
 class SVT(PCPVT):
-    def __init__(self, in_channels=3, embed_dims=[64, 128, 256], patch_sizes=[4, 2, 2, 2], strides=[4, 2, 2, 2], num_heads=[1, 2, 4], mlp_ratios=[4, 4, 4],
-                 out_indices=(0, 1, 2, 3), qkv_bias=False, drop_rate=0., attn_drop_rate=0., drop_path_rate=0.2, depths=[4, 4, 4], sr_ratios=[4, 2, 1],
-                 windiow_sizes=[7, 7, 7], norm_after_stage=True, norm_cfg=None, act_cfg=None):
+    def __init__(self, structure_type, in_channels=3, embed_dims=[64, 128, 256], patch_sizes=[4, 2, 2, 2], strides=[4, 2, 2, 2], num_heads=[1, 2, 4], mlp_ratios=[4, 4, 4],
+                 out_indices=(0, 1, 2, 3), qkv_bias=True, drop_rate=0., attn_drop_rate=0., drop_path_rate=0.2, depths=[4, 4, 4], sr_ratios=[8, 4, 2, 1],
+                 windiow_sizes=[7, 7, 7], norm_after_stage=True, norm_cfg={'type': 'LayerNorm'}, act_cfg={'type': 'GELU'}, pretrained=True, pretrained_model_path=''):
+        self.windiow_sizes = windiow_sizes
         super(SVT, self).__init__(
             in_channels=in_channels, embed_dims=embed_dims, patch_sizes=patch_sizes, strides=strides, num_heads=num_heads, mlp_ratios=mlp_ratios,
             out_indices=out_indices, qkv_bias=qkv_bias, drop_rate=drop_rate, attn_drop_rate=attn_drop_rate, drop_path_rate=drop_path_rate,
-            depths=depths, sr_ratios=sr_ratios, norm_after_stage=norm_after_stage, norm_cfg=norm_cfg, act_cfg=act_cfg
+            depths=depths, sr_ratios=sr_ratios, norm_after_stage=norm_after_stage, norm_cfg=norm_cfg, act_cfg=act_cfg, pretrained=False, pretrained_model_path='',
+            structure_type=structure_type,
         )
         # transformer encoder, stochastic depth decay rule
         dpr = [x.item() for x in torch.linspace(0, drop_path_rate, sum(depths))]
         for k in range(len(depths)):
             for i in range(depths[k]):
                 if i % 2 == 0:
                     self.layers[k][i] = LSAEncoderLayer(
                         embed_dims=embed_dims[k], num_heads=num_heads[k], feedforward_channels=mlp_ratios[k] * embed_dims[k],
                         drop_rate=drop_rate, attn_drop_rate=attn_drop_rate, drop_path_rate=dpr[sum(depths[:k])+i], num_fcs=2,
                         qkv_bias=qkv_bias, window_size=windiow_sizes[k], norm_cfg=norm_cfg, act_cfg=act_cfg
                     )
-
-
-'''BuildTwins'''
-def BuildTwins(twins_cfg):
-    # assert whether support
-    twins_type = twins_cfg.pop('type')
-    supported_twins = {
-        'pcpvt_small': [
-            PCPVT, {'depths': [3, 4, 6, 3], 'drop_path_rate': 0.2},
-        ],
-        'pcpvt_base': [
-            PCPVT, {'depths': [3, 4, 18, 3], 'drop_path_rate': 0.3},
-        ],
-        'pcpvt_large': [
-            PCPVT, {'depths': [3, 8, 27, 3], 'drop_path_rate': 0.3},
-        ],
-        'svt_small': [
-            SVT, {'embed_dims': [64, 128, 256, 512], 'num_heads': [2, 4, 8, 16], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 10, 4], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.2},
-        ],
-        'svt_base': [
-            SVT, {'embed_dims': [96, 192, 384, 768], 'num_heads': [3, 6, 12, 24], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 18, 2], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.2},
-        ],
-        'svt_large': [
-            SVT, {'embed_dims': [128, 256, 512, 1024], 'num_heads': [4, 8, 16, 32], 'mlp_ratios': [4, 4, 4, 4], 'depths': [2, 2, 18, 2], 'windiow_sizes': [7, 7, 7, 7], 'norm_after_stage': True, 'drop_path_rate': 0.3},
-        ],
-    }
-    assert twins_type in supported_twins, 'unspport the twins_type %s' % twins_type
-    # parse cfg
-    default_cfg = {
-        'pretrained': True,
-        'pretrained_model_path': '',
-    }
-    if twins_type.startswith('pcpvt'):
-        default_cfg.update({
-            'in_channels': 3,
-            'embed_dims': [64, 128, 320, 512],
-            'patch_sizes': [4, 2, 2, 2],
-            'strides': [4, 2, 2, 2],
-            'num_heads': [1, 2, 5, 8],
-            'mlp_ratios': [8, 8, 4, 4],
-            'out_indices': (0, 1, 2, 3),
-            'qkv_bias': True,
-            'drop_rate': 0.0,
-            'attn_drop_rate': 0.0,
-            'sr_ratios': [8, 4, 2, 1],
-            'norm_cfg': {'type': 'layernorm'},
-            'act_cfg': {'type': 'gelu'},
-            'norm_after_stage': False
-        })
-    else:
-        default_cfg.update({
-            'in_channels': 3,
-            'patch_sizes': [4, 2, 2, 2],
-            'strides': [4, 2, 2, 2],
-            'out_indices': (0, 1, 2, 3),
-            'qkv_bias': True,
-            'drop_rate': 0.0,
-            'attn_drop_rate': 0.0,
-            'sr_ratios': [8, 4, 2, 1],
-            'norm_cfg': {'type': 'layernorm'},
-            'act_cfg': {'type': 'gelu'},
-        })
-    default_cfg.update(supported_twins[twins_type][1])
-    for key, value in twins_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain twins_cfg
-    twins_cfg = default_cfg.copy()
-    pretrained = twins_cfg.pop('pretrained')
-    pretrained_model_path = twins_cfg.pop('pretrained_model_path')
-    # obtain the instanced twins
-    model = supported_twins[twins_type][0](**twins_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(twins_type, pretrained_model_path)
-    # return the model
-    return model
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/unet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/unet.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 Author:
     Zhenchao Jin
 '''
 import os
 import torch
 import torch.nn as nn
 import torch.utils.model_zoo as model_zoo
-from .bricks import BuildNormalization, BuildActivation, constructnormcfg
+from .bricks import BuildNormalization, BuildActivation
 
 
-'''model urls'''
-model_urls = {}
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {}
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {}
 
 
 '''Basic convolutional block for UNet'''
 class BasicConvBlock(nn.Module):
     def __init__(self, in_channels, out_channels, num_convs=2, stride=1, dilation=1, norm_cfg=None, act_cfg=None):
         super(BasicConvBlock, self).__init__()
         convs = []
         for i in range(num_convs):
             in_c, out_c = in_channels if i == 0 else out_channels, out_channels
             s, d, p = stride if i == 0 else 1, 1 if i == 0 else dilation, 1 if i == 0 else dilation
             conv = nn.Sequential(
                 nn.Conv2d(in_c, out_c, kernel_size=3, stride=s, padding=p, dilation=d, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_c, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_c, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             convs.append(conv)
         self.convs = nn.Sequential(*convs)
     '''forward'''
     def forward(self, x):
         out = self.convs(x)
@@ -39,15 +41,15 @@
 '''Deconvolution upsample module in decoder for UNet (2X upsample)'''
 class DeconvModule(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None, kernel_size=4, scale_factor=2):
         super(DeconvModule, self).__init__()
         assert (kernel_size - scale_factor >= 0) and (kernel_size - scale_factor) % 2 == 0
         self.deconv_upsamping = nn.Sequential(
             nn.ConvTranspose2d(in_channels, out_channels, kernel_size=kernel_size, stride=scale_factor, padding=(kernel_size - scale_factor) // 2),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         out = self.deconv_upsamping(x)
         return out
 
@@ -55,15 +57,15 @@
 '''Interpolation upsample module in decoder for UNet'''
 class InterpConv(nn.Module):
     def __init__(self, in_channels, out_channels, norm_cfg=None, act_cfg=None, conv_first=False, kernel_size=1, stride=1, padding=0, 
                  upsample_cfg=dict(scale_factor=2, mode='bilinear', align_corners=False)):
         super(InterpConv, self).__init__()
         conv = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=kernel_size, stride=stride, padding=padding, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         upsample = nn.Upsample(**upsample_cfg)
         if conv_first:
             self.interp_upsample = nn.Sequential(conv, upsample)
         else:
             self.interp_upsample = nn.Sequential(upsample, conv)
@@ -98,38 +100,54 @@
                 out_channels=skip_channels,
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg,
             )
         else:
             self.upsample = nn.Sequential(
                 nn.Conv2d(in_channels, skip_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=skip_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=skip_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
     '''forward'''
     def forward(self, skip, x):
         x = self.upsample(x)
         out = torch.cat([skip, x], dim=1)
         out = self.conv_block(out)
         return out
 
 
 '''UNet backbone'''
 class UNet(nn.Module):
-    def __init__(self, in_channels=3, base_channels=64, num_stages=5, strides=(1, 1, 1, 1, 1), enc_num_convs=(2, 2, 2, 2, 2), dec_num_convs=(2, 2, 2, 2),
-                 downsamples=(True, True, True, True), enc_dilations=(1, 1, 1, 1, 1), dec_dilations=(1, 1, 1, 1), norm_cfg=None, act_cfg=None, upsample_type='InterpConv'):
+    def __init__(self, structure_type, in_channels=3, base_channels=64, num_stages=5, strides=(1, 1, 1, 1, 1), enc_num_convs=(2, 2, 2, 2, 2), dec_num_convs=(2, 2, 2, 2),
+                 downsamples=(True, True, True, True), enc_dilations=(1, 1, 1, 1, 1), dec_dilations=(1, 1, 1, 1), norm_cfg={'type': 'SyncBatchNorm'}, 
+                 act_cfg={'type': 'ReLU', 'inplace': True}, upsample_type='InterpConv', pretrained=False, pretrained_model_path=''):
         super(UNet, self).__init__()
-        assert (len(strides) == num_stages) and (len(enc_num_convs) == num_stages) \
-            and (len(dec_num_convs) == (num_stages - 1)) and (len(downsamples) == (num_stages - 1)) \
-            and (len(enc_dilations) == num_stages) and len(dec_dilations) == (num_stages - 1)
-        # set attrs
+        # set attributes
+        self.structure_type = structure_type
+        self.in_channels = in_channels
+        self.enc_num_convs = enc_num_convs
+        self.dec_num_convs = dec_num_convs
         self.num_stages = num_stages
         self.strides = strides
         self.downsamples = downsamples
         self.base_channels = base_channels
+        self.enc_dilations = enc_dilations
+        self.dec_dilations = dec_dilations
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.upsample_type = upsample_type
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
+        # assert
+        assert (len(strides) == num_stages) and (len(enc_num_convs) == num_stages) \
+            and (len(dec_num_convs) == (num_stages - 1)) and (len(downsamples) == (num_stages - 1)) \
+            and (len(enc_dilations) == num_stages) and len(dec_dilations) == (num_stages - 1)
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
         # build encoder and decoder
         self.encoder = nn.ModuleList()
         self.decoder = nn.ModuleList()
         for i in range(num_stages):
             enc_conv_block = []
             if i != 0:
                 if strides[i] == 1 and downsamples[i - 1]:
@@ -158,14 +176,29 @@
                     dilation=enc_dilations[i],
                     norm_cfg=norm_cfg,
                     act_cfg=act_cfg,
                 )
             )
             self.encoder.append((nn.Sequential(*enc_conv_block)))
             in_channels = base_channels * 2**i
+        # load pretrained weights
+        if pretrained and os.path.exists(pretrained_model_path):
+            checkpoint = torch.load(pretrained_model_path, map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
+        elif pretrained:
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
+            if 'state_dict' in checkpoint: 
+                state_dict = checkpoint['state_dict']
+            else: 
+                state_dict = checkpoint
+            self.load_state_dict(state_dict, strict=False)
     '''forward'''
     def forward(self, x):
         self.checkinputdivisible(x)
         enc_outs = []
         for enc in self.encoder:
             x = enc(x)
             enc_outs.append(x)
@@ -177,57 +210,8 @@
     '''check input divisible'''
     def checkinputdivisible(self, x):
         h, w = x.shape[-2:]
         whole_downsample_rate = 1
         for i in range(1, self.num_stages):
             if self.strides[i] == 2 or self.downsamples[i - 1]:
                 whole_downsample_rate *= 2
-        assert (h % whole_downsample_rate == 0) and (w % whole_downsample_rate == 0)
-
-
-'''BuildUNet'''
-def BuildUNet(unet_cfg):
-    # assert whether support
-    unet_type = unet_cfg.pop('type')
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3,
-        'base_channels': 64,
-        'num_stages': 5,
-        'strides': (1, 1, 1, 1, 1),
-        'enc_num_convs': (2, 2, 2, 2, 2),
-        'dec_num_convs': (2, 2, 2, 2),
-        'downsamples': (True, True, True, True),
-        'enc_dilations': (1, 1, 1, 1, 1),
-        'dec_dilations': (1, 1, 1, 1),
-        'norm_cfg': None,
-        'act_cfg': {'type': 'relu', 'inplace': True},
-        'upsample_type': 'InterpConv',
-        'pretrained': False,
-        'pretrained_model_path': '',
-    }
-    for key, value in unet_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain unet_cfg
-    unet_cfg = default_cfg.copy()
-    pretrained = unet_cfg.pop('pretrained')
-    pretrained_model_path = unet_cfg.pop('pretrained_model_path')
-    # obtain the instanced unet
-    model = UNet(**unet_cfg)
-    # load weights of pretrained model
-    if pretrained and os.path.exists(pretrained_model_path):
-        checkpoint = torch.load(pretrained_model_path)
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    elif pretrained:
-        checkpoint = model_zoo.load_url(model_urls[unet_type])
-        if 'state_dict' in checkpoint: 
-            state_dict = checkpoint['state_dict']
-        else: 
-            state_dict = checkpoint
-        model.load_state_dict(state_dict, strict=False)
-    # return the model
-    return model
+        assert (h % whole_downsample_rate == 0) and (w % whole_downsample_rate == 0)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/backbones/vit.py` & `SSSegmentation-1.3.0/ssseg/modules/models/backbones/vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,46 +7,54 @@
 import os
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.model_zoo as model_zoo
 import torch.utils.checkpoint as checkpoint
-from .bricks import BuildNormalization, MultiheadAttention, PatchEmbed, FFN, constructnormcfg
+from .bricks import BuildNormalization, MultiheadAttention, PatchEmbed, FFN
 
 
-'''model urls'''
-model_urls = {
+'''DEFAULT_MODEL_URLS'''
+DEFAULT_MODEL_URLS = {
     'jx_vit_large_p16_384': 'https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_large_p16_384-b3be5167.pth',
 }
+'''AUTO_ASSERT_STRUCTURE_TYPES'''
+AUTO_ASSERT_STRUCTURE_TYPES = {
+    'jx_vit_large_p16_384': {
+        'patch_size': 16, 'embed_dims': 1024, 'num_layers': 24, 'num_heads': 16, 'mlp_ratio': 4,
+        'qkv_bias': True, 'drop_rate': 0.1, 'attn_drop_rate': 0., 'drop_path_rate': 0., 'with_cls_token': True,
+        'output_cls_token': False, 'patch_norm': False, 'final_norm': False, 'num_fcs': 2,
+    }
+}
 
 
 '''TransformerEncoderLayer'''
 class TransformerEncoderLayer(nn.Module):
     def __init__(self, embed_dims, num_heads, feedforward_channels, drop_rate=0., attn_drop_rate=0., drop_path_rate=0., num_fcs=2, 
                  qkv_bias=True, act_cfg=None, norm_cfg=None, batch_first=True, attn_cfg=dict(), ffn_cfg=dict(), use_checkpoint=False):
         super(TransformerEncoderLayer, self).__init__()
-        self.ln1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.ln1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         attn_cfg.update(dict(
             embed_dims=embed_dims,
             num_heads=num_heads,
             attn_drop=attn_drop_rate,
             proj_drop=drop_rate,
-            dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
             batch_first=batch_first,
             bias=qkv_bias,
         ))
         self.attn = MultiheadAttention(**attn_cfg)
-        self.ln2 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+        self.ln2 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
         ffn_cfg.update(dict(
             embed_dims=embed_dims,
             feedforward_channels=feedforward_channels,
             num_fcs=num_fcs,
             ffn_drop=drop_rate,
-            dropout_cfg={'type': 'droppath', 'drop_prob': drop_path_rate},
+            dropout_cfg={'type': 'DropPath', 'drop_prob': drop_path_rate},
             act_cfg=act_cfg,
         ))
         self.ffn = FFN(**ffn_cfg)
         self.use_checkpoint = use_checkpoint
     '''forward'''
     def forward(self, x):
         def _forward(x):
@@ -58,38 +66,60 @@
         else:
             x = _forward(x)
         return x
 
 
 '''VisionTransformer'''
 class VisionTransformer(nn.Module):
-    def __init__(self, img_size=224, patch_size=16, in_channels=3, embed_dims=768, num_layers=12, num_heads=12, mlp_ratio=4, out_indices=-1, qkv_bias=True,
-                 drop_rate=0., attn_drop_rate=0., drop_path_rate=0., with_cls_token=True, output_cls_token=False, norm_cfg=None, act_cfg=None, 
-                 patch_norm=False, final_norm=False, interpolate_mode='bicubic', num_fcs=2, use_checkpoint=False):
+    def __init__(self, structure_type, img_size=224, patch_size=16, in_channels=3, embed_dims=768, num_layers=12, num_heads=12, mlp_ratio=4, out_indices=(9, 14, 19, 23), qkv_bias=True,
+                 drop_rate=0., attn_drop_rate=0., drop_path_rate=0., with_cls_token=True, output_cls_token=False, norm_cfg={'type': 'LayerNorm', 'eps': 1e-6}, act_cfg={'type': 'GELU'}, 
+                 patch_norm=False, final_norm=False, interpolate_mode='bilinear', num_fcs=2, use_checkpoint=False, pretrained=True, pretrained_model_path=''):
         super(VisionTransformer, self).__init__()
-        if isinstance(img_size, int):
-            img_size = (img_size, img_size)
-        if output_cls_token:
-            assert with_cls_token, 'with_cls_token must be True if set output_cls_token to True.'
+        # set attributes
+        self.structure_type = structure_type
         self.img_size = img_size
         self.patch_size = patch_size
+        self.in_channels = in_channels
+        self.embed_dims = embed_dims
+        self.num_layers = num_layers
+        self.num_heads = num_heads
+        self.mlp_ratio = mlp_ratio
+        self.out_indices = out_indices
+        self.qkv_bias = qkv_bias
+        self.drop_rate = drop_rate
+        self.attn_drop_rate = attn_drop_rate
+        self.drop_path_rate = drop_path_rate
+        self.with_cls_token = with_cls_token
+        self.output_cls_token = output_cls_token
+        self.norm_cfg = norm_cfg
+        self.act_cfg = act_cfg
+        self.patch_norm = patch_norm
+        self.num_fcs = num_fcs
+        self.pretrained = pretrained
+        self.pretrained_model_path = pretrained_model_path
         self.interpolate_mode = interpolate_mode
         self.use_checkpoint = use_checkpoint
+        self.final_norm = final_norm
+        # assert
+        if output_cls_token: assert with_cls_token, 'with_cls_token must be True if set output_cls_token to True.'
+        if structure_type in AUTO_ASSERT_STRUCTURE_TYPES:
+            for key, value in AUTO_ASSERT_STRUCTURE_TYPES[structure_type].items():
+                assert hasattr(self, key) and (getattr(self, key) == value)
+        if isinstance(img_size, int): img_size = (img_size, img_size)
+        self.img_size = img_size
         # Image to Patch Embedding
         self.patch_embed = PatchEmbed(
             in_channels=in_channels,
             embed_dims=embed_dims,
             kernel_size=patch_size,
             stride=patch_size,
             padding='corner',
             norm_cfg=norm_cfg if patch_norm else None,
         )
         num_patches = (img_size[0] // patch_size) * (img_size[1] // patch_size)
-        self.with_cls_token = with_cls_token
-        self.output_cls_token = output_cls_token
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dims))
         self.pos_embed = nn.Parameter(torch.zeros(1, num_patches + 1, embed_dims))
         self.drop_after_pos = nn.Dropout(p=drop_rate)
         if isinstance(out_indices, int):
             if out_indices == -1:
                 out_indices = num_layers - 1
             self.out_indices = [out_indices]
@@ -111,23 +141,26 @@
                 num_fcs=num_fcs,
                 qkv_bias=qkv_bias,
                 act_cfg=act_cfg,
                 norm_cfg=norm_cfg,
                 batch_first=True,
                 use_checkpoint=use_checkpoint,
             ))
-        self.final_norm = final_norm
+        
         if final_norm:
-            self.ln1 = BuildNormalization(constructnormcfg(placeholder=embed_dims, norm_cfg=norm_cfg))
+            self.ln1 = BuildNormalization(placeholder=embed_dims, norm_cfg=norm_cfg)
+        # load pretrained weights
+        if pretrained:
+            self.initweights(structure_type, pretrained_model_path)
     '''initialize backbone'''
-    def initweights(self, vit_type='jx_vit_large_p16_384', pretrained_model_path=''):
+    def initweights(self, structure_type='jx_vit_large_p16_384', pretrained_model_path=''):
         if pretrained_model_path:
             checkpoint = torch.load(pretrained_model_path, map_location='cpu')
         else:
-            checkpoint = model_zoo.load_url(model_urls[vit_type], map_location='cpu')
+            checkpoint = model_zoo.load_url(DEFAULT_MODEL_URLS[structure_type], map_location='cpu')
         if 'state_dict' in checkpoint:
             state_dict = checkpoint['state_dict']
         elif 'model' in checkpoint:
             state_dict = checkpoint['model']
         else:
             state_dict = checkpoint
         state_dict = self.vitconvert(state_dict)
@@ -214,48 +247,8 @@
                     out = x[:, 1:]
                 else:
                     out = x
                 B, _, C = out.shape
                 out = out.reshape(B, hw_shape[0], hw_shape[1], C).permute(0, 3, 1, 2).contiguous()
                 if self.output_cls_token: out = [out, x[:, 0]]
                 outs.append(out)
-        return tuple(outs)
-
-
-'''BuildVisionTransformer'''
-def BuildVisionTransformer(vit_cfg):
-    # assert whether support
-    vit_type = vit_cfg.pop('type')
-    supported_vits = {
-        'jx_vit_large_p16_384': {
-            'img_size': 384, 'patch_size': 16, 'embed_dims': 1024, 'num_layers': 24, 'num_heads': 16, 'mlp_ratio': 4,
-            'qkv_bias': True, 'drop_rate': 0.1, 'attn_drop_rate': 0., 'drop_path_rate': 0., 'with_cls_token': True,
-            'output_cls_token': False, 'patch_norm': False, 'final_norm': False, 'num_fcs': 2,
-        }
-    }
-    assert vit_type in supported_vits, 'unspport the vit_type %s' % vit_type
-    # parse cfg
-    default_cfg = {
-        'in_channels': 3,
-        'out_indices': (9, 14, 19, 23),
-        'norm_cfg': {'type': 'layernorm', 'eps': 1e-6},
-        'act_cfg': {'type': 'gelu'},
-        'interpolate_mode': 'bilinear',
-        'pretrained': True,
-        'pretrained_model_path': '',
-        'use_checkpoint': False,
-    }
-    default_cfg.update(supported_vits[vit_type])
-    for key, value in vit_cfg.items():
-        if key in default_cfg: 
-            default_cfg.update({key: value})
-    # obtain vit_cfg
-    vit_cfg = default_cfg.copy()
-    pretrained = vit_cfg.pop('pretrained')
-    pretrained_model_path = vit_cfg.pop('pretrained_model_path')
-    # obtain the instanced vit
-    model = VisionTransformer(**vit_cfg)
-    # load weights of pretrained model
-    if pretrained:
-        model.initweights(vit_type, pretrained_model_path)
-    # return the model
-    return model
+        return tuple(outs)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/losses/accuracy.py` & `SSSegmentation-1.3.0/ssseg/modules/models/losses/accuracy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define the accuracy
+    Implementation of calculateaccuracy
 Author:
     Zhenchao Jin
 '''
 import torch
 
 
 '''calculateaccuracy'''
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/losses/diceloss.py` & `SSSegmentation-1.3.0/ssseg/modules/models/losses/diceloss.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 '''
 Function:
-    Define the dice loss
+    Implementation of DiceLoss
 Author:
     Zhenchao Jin
 '''
 import torch
+import torch.nn as nn
 import torch.nn.functional as F
 
 
-'''
-Function:
-    DiceLoss
-Arguments:
-    --prediction: prediction of the network
-    --target: ground truth
-    --scale_factor: scale the loss for loss balance
-    --lowest_loss_value: added inspired by ICML2020, "Do We Need Zero Training Loss After Achieving Zero Training Error", https://arxiv.org/pdf/2002.08709.pdf
-'''
-def DiceLoss(prediction, target, scale_factor=1.0, smooth=1, exponent=2, reduction='mean', class_weight=None, ignore_index=255, lowest_loss_value=None):
-    '''binary dice loss'''
-    def BinaryDiceLoss(pred, target, valid_mask, smooth=1, exponent=2):
-        assert pred.shape[0] == target.shape[0]
-        pred = pred.reshape(pred.shape[0], -1)
-        target = target.reshape(target.shape[0], -1)
-        valid_mask = valid_mask.reshape(valid_mask.shape[0], -1)
-        num = torch.sum(torch.mul(pred, target) * valid_mask, dim=1) * 2 + smooth
-        den = torch.sum(pred.pow(exponent) + target.pow(exponent), dim=1) + smooth
-        return 1 - num / den
-    '''unwrapped dice loss'''
-    def _DiceLoss(pred, target, valid_mask, smooth=1, exponent=2, class_weight=None, ignore_index=255):
+'''DiceLoss'''
+class DiceLoss(nn.Module):
+    def __init__(self, scale_factor=1.0, smooth=1, exponent=2, reduction='mean', class_weight=None, ignore_index=255, lowest_loss_value=None):
+        super(DiceLoss, self).__init__()
+        self.smooth = smooth
+        self.exponent = exponent
+        self.reduction = reduction
+        self.class_weight = class_weight
+        self.scale_factor = scale_factor
+        self.ignore_index = ignore_index
+        self.lowest_loss_value = lowest_loss_value
+    '''forward'''
+    def forward(self, prediction, target):
+        # fetch attributes
+        smooth, exponent, reduction, ignore_index = self.smooth, self.exponent, self.reduction, self.ignore_index
+        class_weight, scale_factor, lowest_loss_value = self.class_weight, self.scale_factor, self.lowest_loss_value
+        # construct loss_cfg
+        dice_cfg = {
+            'smooth': smooth, 'exponent': exponent, 'reduction': reduction, 'class_weight': class_weight, 'ignore_index': ignore_index,
+        }
+        if dice_cfg['class_weight'] is not None:
+            class_weight = prediction.new_tensor(dice_cfg['class_weight'])
+        else:
+            class_weight = None
+        # calculate loss
+        prediction = F.softmax(prediction, dim=1)
+        num_classes = prediction.shape[1]
+        one_hot_target = F.one_hot(torch.clamp(target.long(), 0, num_classes - 1), num_classes=num_classes)
+        valid_mask = (target != dice_cfg['ignore_index']).long()
+        loss = self.diceloss(prediction, one_hot_target, valid_mask, **dice_cfg)
+        if dice_cfg['reduction'] == 'mean':
+            loss = loss.mean()
+        elif dice_cfg['reduction'] == 'sum':
+            loss = loss.sum()
+        else:
+            assert dice_cfg['reduction'] == 'none', 'only support reduction in [mean, sum, none]'
+        loss = loss * scale_factor
+        if lowest_loss_value is not None:
+            loss = torch.abs(loss - lowest_loss_value) + lowest_loss_value
+        # return
+        return loss
+    '''diceloss'''
+    def diceloss(self, pred, target, valid_mask, smooth=1, exponent=2, class_weight=None, ignore_index=255):
         assert pred.shape[0] == target.shape[0]
         total_loss = 0
         num_classes = pred.shape[1]
         for i in range(num_classes):
             if i != ignore_index:
-                dice_loss = BinaryDiceLoss(pred[:, i], target[..., i], valid_mask=valid_mask, smooth=smooth, exponent=exponent)
+                dice_loss = self.binarydiceloss(pred[:, i], target[..., i], valid_mask=valid_mask, smooth=smooth, exponent=exponent)
                 if class_weight is not None: dice_loss *= class_weight[i]
                 total_loss += dice_loss
         return total_loss / num_classes
-    # calculate the loss
-    dice_cfg = {
-        'smooth': smooth,
-        'exponent': exponent,
-        'reduction': reduction,
-        'class_weight': class_weight,
-        'ignore_index': ignore_index,
-    }
-    if dice_cfg['class_weight'] is not None:
-        class_weight = prediction.new_tensor(dice_cfg['class_weight'])
-    else:
-        class_weight = None
-    prediction = F.softmax(prediction, dim=1)
-    num_classes = prediction.shape[1]
-    one_hot_target = F.one_hot(torch.clamp(target.long(), 0, num_classes - 1), num_classes=num_classes)
-    valid_mask = (target != dice_cfg['ignore_index']).long()
-    loss = _DiceLoss(prediction, one_hot_target, valid_mask, **dice_cfg)
-    if dice_cfg['reduction'] == 'mean':
-        loss = loss.mean()
-    elif dice_cfg['reduction'] == 'sum':
-        loss = loss.sum()
-    else:
-        assert dice_cfg['reduction'] == 'none', 'only support reduction in [mean, sum, none]'
-    # scale the loss
-    loss = loss * scale_factor
-    # return the final loss
-    if lowest_loss_value:
-        return torch.abs(loss - lowest_loss_value) + lowest_loss_value
-    return loss
+    '''binarydiceloss'''
+    @staticmethod
+    def binarydiceloss(pred, target, valid_mask, smooth=1, exponent=2):
+        assert pred.shape[0] == target.shape[0]
+        pred = pred.reshape(pred.shape[0], -1)
+        target = target.reshape(target.shape[0], -1)
+        valid_mask = valid_mask.reshape(valid_mask.shape[0], -1)
+        num = torch.sum(torch.mul(pred, target) * valid_mask, dim=1) * 2 + smooth
+        den = torch.sum(pred.pow(exponent) + target.pow(exponent), dim=1) + smooth
+        return 1 - num / den
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/losses/l1loss.py` & `SSSegmentation-1.3.0/ssseg/modules/models/losses/cosinesimilarityloss.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 '''
 Function:
-    Define the l1 loss
+    Implementation of CosineSimilarityLoss
 Author:
     Zhenchao Jin
 '''
 import torch
+import torch.nn as nn
 import torch.nn.functional as F
 
 
-'''
-Function:
-    L1Loss
-Arguments:
-    --prediction: prediction of the network
-    --target: ground truth
-    --scale_factor: scale the loss for loss balance
-    --lowest_loss_value: added inspired by ICML2020, "Do We Need Zero Training Loss After Achieving Zero Training Error", https://arxiv.org/pdf/2002.08709.pdf
-'''
-def L1Loss(prediction, target, scale_factor=1.0, reduction='mean', lowest_loss_value=None):
-    # calculate the loss
-    loss = F.l1_loss(prediction, target, reduction=reduction)
-    # scale the loss
-    loss = loss * scale_factor
-    # return the final loss
-    if lowest_loss_value:
-        return torch.abs(loss - lowest_loss_value) + lowest_loss_value
-    return loss
+'''CosineSimilarityLoss'''
+class CosineSimilarityLoss(nn.Module):
+    def __init__(self, scale_factor=1.0, reduction='mean', lowest_loss_value=None):
+        super(CosineSimilarityLoss, self).__init__()
+        self.reduction = reduction
+        self.scale_factor = scale_factor
+        self.lowest_loss_value = lowest_loss_value
+    '''forward'''
+    def forward(self, prediction, target):
+        # fetch attributes
+        scale_factor, reduction, lowest_loss_value = self.scale_factor, self.reduction, self.lowest_loss_value
+        # calculate loss
+        assert prediction.shape == target.shape
+        loss = 1 - F.cosine_similarity(prediction, target, dim=1)
+        if reduction == 'mean':
+            loss = loss.mean()
+        elif reduction == 'sum': 
+            loss = loss.sum()
+        loss = loss * scale_factor
+        if lowest_loss_value is not None:
+            loss = torch.abs(loss - lowest_loss_value) + lowest_loss_value
+        # return
+        return loss
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/losses/lovaszloss.py` & `SSSegmentation-1.3.0/ssseg/modules/models/losses/lovaszloss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Function:
-    Define the lovasz loss
+    Implementation of LovaszLoss
 Author:
     Zhenchao Jin
 '''
 import torch
+import torch.nn as nn
 import torch.nn.functional as F
 
 
 '''LovaszGrad: computes gradient of the lovasz extension w.r.t sorted errors'''
 def LovaszGrad(gt_sorted):
     p = len(gt_sorted)
     gts = gt_sorted.sum()
@@ -140,14 +141,28 @@
     # return the final loss
     if lowest_loss_value:
         return torch.abs(loss - lowest_loss_value) + lowest_loss_value
     return loss
 
 
 '''LovaszLoss'''
-def LovaszLoss(mode='multi_class', **kwargs):
-    support_modes = {
-        'binary': LovaszHingeLoss,
-        'multi_class': LovaszSoftmaxLoss,
-    }
-    assert mode in support_modes, 'unsupport mode %s' % mode
-    return support_modes[mode](**kwargs)
+class LovaszLoss(nn.Module):
+    def __init__(self, mode='multi_class', **kwargs):
+        super(LovaszLoss, self).__init__()
+        self.mode = mode
+        self.loss_args = kwargs
+    '''forward'''
+    def forward(self, prediction, target):
+        # fetch attributes
+        mode = self.mode
+        # supported modes
+        supported_modes = {
+            'binary': LovaszHingeLoss,
+            'multi_class': LovaszSoftmaxLoss,
+        }
+        # construct loss_cfg
+        lovasz_args = self.loss_args.copy()
+        lovasz_args.update({'prediction': prediction, 'target': target})
+        # calculate loss
+        loss = supported_modes[mode](**lovasz_args)
+        # return
+        return loss
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/optimizers/builder.py` & `SSSegmentation-1.3.0/ssseg/modules/models/optimizers/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 '''
-Funtion:
-    Build the optimizer
+Function:
+    Implementation of BuildOptimizer
 Author:
     Zhenchao Jin
 '''
 import copy
 import torch.nn as nn
 import torch.optim as optim
 from .paramsconstructor import DefaultParamsConstructor, LayerDecayParamsConstructor
 
 
 '''BuildOptimizer'''
 def BuildOptimizer(model, optimizer_cfg):
     # define the supported optimizers
     supported_optimizers = {
-        'sgd': optim.SGD,
-        'adam': optim.Adam,
-        'adamw': optim.AdamW,
-        'adadelta': optim.Adadelta,
+        'SGD': optim.SGD,
+        'Adam': optim.Adam,
+        'AdamW': optim.AdamW,
+        'Adadelta': optim.Adadelta,
     }
     # parse optimizer_cfg
     optimizer_cfg = copy.deepcopy(optimizer_cfg)
     optimizer_type = optimizer_cfg.pop('type')
     params_rules, filter_params = {}, False
     if 'params_rules' in optimizer_cfg:
         params_rules = optimizer_cfg.pop('params_rules')
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/optimizers/paramsconstructor.py` & `SSSegmentation-1.3.0/ssseg/modules/models/optimizers/paramsconstructor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Define the params constructor
+    Implementation of DefaultParamsConstructor
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/samplers/ohempixelsampler.py` & `SSSegmentation-1.3.0/ssseg/modules/models/samplers/ohempixelsampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    OHEM pixel sampler
+    Implementation of OHEMPixelSampler
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn.functional as F
 from .base import BasePixelSampler
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/schedulers/basescheduler.py` & `SSSegmentation-1.3.0/ssseg/modules/models/schedulers/basescheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Funtion:
-    Define the basescheduler
+    Implementation of BaseScheduler
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from torch.nn.utils import clip_grad
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/schedulers/builder.py` & `SSSegmentation-1.3.0/ssseg/modules/models/schedulers/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 '''
 Funtion:
-    Build the scheduler
+    Implementation of BuildScheduler
 Author:
     Zhenchao Jin
 '''
 import copy
 from .polyscheduler import PolyScheduler
 
 
 '''BuildScheduler'''
 def BuildScheduler(optimizer, scheduler_cfg):
-    # define the supported schedulers
+    scheduler_cfg = copy.deepcopy(scheduler_cfg)
+    # supported schedulers
     supported_schedulers = {
-        'poly': PolyScheduler
+        'PolyScheduler': PolyScheduler
     }
-    # parse scheduler_cfg
-    scheduler_cfg = copy.deepcopy(scheduler_cfg)
+    # build scheduler
     scheduler_type = scheduler_cfg.pop('type')
-    scheduler_cfg['optimizer'] = optimizer
+    scheduler_cfg.pop('optimizer')
+    scheduler = supported_schedulers[scheduler_type](optimizer=optimizer, **scheduler_cfg)
     # return
-    return supported_schedulers[scheduler_type](**scheduler_cfg)
+    return scheduler
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/schedulers/polyscheduler.py` & `SSSegmentation-1.3.0/ssseg/modules/models/schedulers/polyscheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Funtion:
-    Define the polyscheduler
+    Implementation of PolyScheduler
 Author:
     Zhenchao Jin
 '''
 from .basescheduler import BaseScheduler
 
 
 '''PolyScheduler'''
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/afnblock.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/afnblock.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from .ppm import PPMConcat
 from ..base import SelfAttentionBlock
-from ...backbones import BuildNormalization, constructnormcfg
+from ...backbones import BuildNormalization
 
 
 '''Asymmetric Fusion Non-local Block (AFNB)'''
 class AFNBlock(nn.Module):
     def __init__(self, low_in_channels, high_in_channels, transform_channels, out_channels, query_scales, key_pool_scales, norm_cfg=None, act_cfg=None):
         super(AFNBlock, self).__init__()
         self.stages = nn.ModuleList()
@@ -37,15 +37,15 @@
                 matmul_norm=True,
                 with_out_project=True,
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg
             ))
         self.bottleneck = nn.Sequential(
             nn.Conv2d(out_channels+high_in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
         )
     '''forward'''
     def forward(self, low_feats, high_feats):
         priors = [stage(high_feats, low_feats) for stage in self.stages]
         context = torch.stack(priors, dim=0).sum(dim=0)
         output = self.bottleneck(torch.cat([context, high_feats], 1))
         return output
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/annnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/annnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 import copy
 import torch
 import torch.nn as nn
 from .afnblock import AFNBlock
 from .apnblock import APNBlock
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ANNNet'''
 class ANNNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(ANNNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -38,30 +38,30 @@
             key_pool_scales=head_cfg['key_pool_scales'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg),
         )
         # build bottleneck
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels_list'][1], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'afn_block', 'apn_block', 'bottleneck', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         low_feats, high_feats = backbone_outputs[-2], backbone_outputs[-1]
         # feed to AFNBlock
         feats = self.afn_block(low_feats, high_feats)
         feats = self.decoder[0](feats)
@@ -73,12 +73,12 @@
         predictions = self.decoder[1](feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/apnblock.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/apnblock.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from .ppm import PPMConcat
 from ..base import SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''Asymmetric Pyramid Non-local Block (APNB)'''
 class APNBlock(nn.Module):
     def __init__(self, in_channels, transform_channels, out_channels, query_scales, key_pool_scales, norm_cfg=None, act_cfg=None):
         super(APNBlock, self).__init__()
         self.stages = nn.ModuleList()
@@ -37,15 +37,15 @@
                 matmul_norm=True,
                 with_out_project=True,
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg
             ))
         self.bottleneck = nn.Sequential(
             nn.Conv2d(2 * in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, feats):
         priors = [stage(feats, feats) for stage in self.stages]
         context = torch.stack(priors, dim=0).sum(dim=0)
         output = self.bottleneck(torch.cat([context, feats], 1))
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/annnet/ppm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/annnet/ppm.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/acm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/acm.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,47 +3,47 @@
     Implementation of AdaptiveContextModule
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''AdaptiveContextModule'''
 class AdaptiveContextModule(nn.Module):
     def __init__(self, in_channels, out_channels, pool_scale, align_corners, norm_cfg=None, act_cfg=None):
         super(AdaptiveContextModule, self).__init__()
         self.pool_scale = pool_scale
         self.align_corners = align_corners
         self.pooled_redu_conv = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.input_redu_conv = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.global_info = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.gla = nn.Conv2d(out_channels, pool_scale**2, kernel_size=1, stride=1, padding=0)
         self.residual_conv = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.fusion_conv = nn.Sequential(
             nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         batch_size = x.size(0)
         pooled_x = F.adaptive_avg_pool2d(x, self.pool_scale)
         x = self.input_redu_conv(x)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/apcnet/apcnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/apcnet/apcnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
 from .acm import AdaptiveContextModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''APCNet'''
 class APCNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(APCNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -29,27 +29,27 @@
         self.acm_modules = nn.ModuleList()
         for pool_scale in head_cfg['pool_scales']:
             acm_cfg['pool_scale'] = pool_scale
             self.acm_modules.append(AdaptiveContextModule(**acm_cfg))
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * len(head_cfg['pool_scales']) + head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0),
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'acm_modules', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to acm
         acm_outs = [backbone_outputs[-1]]
         for acm_module in self.acm_modules:
             acm_outs.append(acm_module(backbone_outputs[-1]))
@@ -58,12 +58,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/base.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from ...losses import BuildLoss
-from ...backbones import BuildBackbone, BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildBackbone, BuildActivation, BuildNormalization
 
 
 '''BaseSegmentor'''
 class BaseSegmentor(nn.Module):
     def __init__(self, cfg, mode):
         super(BaseSegmentor, self).__init__()
         self.cfg = cfg
@@ -24,15 +24,15 @@
         self.align_corners, self.norm_cfg, self.act_cfg = cfg['align_corners'], cfg['norm_cfg'], cfg['act_cfg']
         # build backbone
         backbone_cfg = copy.deepcopy(cfg['backbone'])
         if 'norm_cfg' not in backbone_cfg:
             backbone_cfg.update({'norm_cfg': copy.deepcopy(self.norm_cfg)})
         self.backbone_net = BuildBackbone(backbone_cfg)
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         raise NotImplementedError('not to be implemented')
     '''forward when mode = `TRAIN`'''
     def forwardtrain(self, predictions, targets, backbone_outputs, losses_cfg, img_size, compute_loss=True):
         predictions = F.interpolate(predictions, size=img_size, mode='bilinear', align_corners=self.align_corners)
         outputs_dict = {'loss_cls': predictions}
         if hasattr(self, 'auxiliary_decoder'):
             backbone_outputs = backbone_outputs[:-1]
@@ -103,15 +103,15 @@
             dec = []
             for idx in range(num_convs):
                 if idx == 0:
                     dec += [nn.Conv2d(aux_cfg['in_channels'], aux_cfg['out_channels'], kernel_size=3, stride=1, padding=1, bias=False),]
                 else:
                     dec += [nn.Conv2d(aux_cfg['out_channels'], aux_cfg['out_channels'], kernel_size=3, stride=1, padding=1, bias=False),]
                 dec += [
-                    BuildNormalization(constructnormcfg(placeholder=aux_cfg['out_channels'], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=aux_cfg['out_channels'], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg)
                 ]
                 if 'upsample' in aux_cfg:
                     dec += [nn.Upsample(**aux_cfg['upsample'])]
             dec.append(nn.Dropout2d(aux_cfg['dropout']))
             if num_convs > 0:
                 dec.append(nn.Conv2d(aux_cfg['out_channels'], num_classes, kernel_size=1, stride=1, padding=0))
@@ -120,38 +120,39 @@
             dec = nn.Sequential(*dec)
             self.auxiliary_decoder.append(dec)
         if len(self.auxiliary_decoder) == 1:
             self.auxiliary_decoder = self.auxiliary_decoder[0]
     '''freeze normalization'''
     def freezenormalization(self):
         for module in self.modules():
-            if type(module) in BuildNormalization(only_get_all_supported=True):
+            if isinstance(module, nn.BatchNorm1d) or isinstance(module, nn.BatchNorm2d) or \
+               isinstance(module, nn.BatchNorm3d) or isinstance(module, SyncBatchNorm):
                 module.eval()
     '''calculate the losses'''
     def calculatelosses(self, predictions, targets, losses_cfg, map_preds_to_tgts_dict=None):
         # parse targets
-        target_seg = targets['segmentation']
-        if 'edge' in targets:
-            target_edge = targets['edge']
-            num_neg_edge, num_pos_edge = torch.sum(target_edge == 0, dtype=torch.float), torch.sum(target_edge == 1, dtype=torch.float)
+        seg_target = targets['seg_target']
+        if 'edge_target' in targets and targets['edge_target'] is not None:
+            edge_target = targets['edge_target']
+            num_neg_edge, num_pos_edge = torch.sum(edge_target == 0, dtype=torch.float), torch.sum(edge_target == 1, dtype=torch.float)
             weight_pos_edge, weight_neg_edge = num_neg_edge / (num_pos_edge + num_neg_edge), num_pos_edge / (num_pos_edge + num_neg_edge)
-            cls_weight_edge = torch.Tensor([weight_neg_edge, weight_pos_edge]).type_as(target_edge)
+            cls_weight_edge = torch.Tensor([weight_neg_edge, weight_pos_edge]).type_as(edge_target)
         # calculate loss according to losses_cfg
-        assert len(predictions) == len(losses_cfg), 'length of losses_cfg should be equal to predictions'
+        assert len(predictions) == len(losses_cfg), 'length of losses_cfg should be equal to the one of predictions'
         losses_log_dict = {}
         for loss_name, loss_cfg in losses_cfg.items():
             if 'edge' in loss_name:
                 loss_cfg = copy.deepcopy(loss_cfg)
                 loss_cfg_keys = loss_cfg.keys()
                 for key in loss_cfg_keys:
                     loss_cfg[key].update({'weight': cls_weight_edge})
             if map_preds_to_tgts_dict is None:
                 losses_log_dict[loss_name] = self.calculateloss(
                     prediction=predictions[loss_name],
-                    target=target_edge if 'edge' in loss_name else target_seg,
+                    target=edge_target if 'edge' in loss_name else seg_target,
                     loss_cfg=loss_cfg,
                 )
             else:
                 losses_log_dict[loss_name] = self.calculateloss(
                     prediction=predictions[loss_name],
                     target=targets[map_preds_to_tgts_dict[loss_name]],
                     loss_cfg=loss_cfg,
@@ -180,24 +181,21 @@
         elif prediction.dim() == 3:
             prediction_format = prediction.permute((0, 2, 1)).contiguous()
         else:
             prediction_format = prediction
         prediction_format = prediction_format.view(-1, prediction_format.size(-1))
         # calculate the loss
         loss = 0
-        for key, value in loss_cfg.items():
-            if (key in ['binaryceloss']) and hasattr(self, 'onehot'):
+        for key in list(loss_cfg.keys()):
+            if (key in ['BinaryCrossEntropyLoss']) and hasattr(self, 'onehot'):
                 prediction_iter = prediction_format
                 target_iter = self.onehot(target, self.cfg['num_classes'])
-            elif key in ['diceloss', 'lovaszloss', 'kldivloss', 'l1loss']:
+            elif key in ['DiceLoss', 'LovaszLoss', 'KLDivLoss', 'L1Loss', 'CosineSimilarityLoss']:
                 prediction_iter = prediction
                 target_iter = target
             else:
                 prediction_iter = prediction_format
                 target_iter = target.view(-1)
-            loss += BuildLoss(key)(
-                prediction=prediction_iter, 
-                target=target_iter, 
-                **value
-            )
+            loss_cfg[key]['type'] = key
+            loss += BuildLoss(loss_cfg[key])(prediction=prediction_iter, target=target_iter)
         # return the loss
         return loss
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/feature2pyramid.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/feature2pyramid.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 Function:
     Implementation of Feature2Pyramid
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
-from ...backbones import BuildNormalization, constructnormcfg
+from ...backbones import BuildNormalization
 
 
 '''Feature2Pyramid'''
 class Feature2Pyramid(nn.Module):
     def __init__(self, embed_dim, rescales=[4, 2, 1, 0.5], norm_cfg=None):
         super(Feature2Pyramid, self).__init__()
         self.rescales = rescales
         self.upsample_4x = None
         for k in self.rescales:
             if k == 4:
                 self.upsample_4x = nn.Sequential(
                     nn.ConvTranspose2d(embed_dim, embed_dim, kernel_size=2, stride=2),
-                    BuildNormalization(constructnormcfg(placeholder=embed_dim, norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=embed_dim, norm_cfg=norm_cfg),
                     nn.GELU(),
                     nn.ConvTranspose2d(embed_dim, embed_dim, kernel_size=2, stride=2),
                 )
             elif k == 2:
                 self.upsample_2x = nn.Sequential(
                     nn.ConvTranspose2d(embed_dim, embed_dim, kernel_size=2, stride=2)
                 )
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/fpn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/fpn.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,35 @@
     Implementation of Feature Pyramid Network
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''Feature Pyramid Network'''
 class FPN(nn.Module):
     def __init__(self, in_channels_list, out_channels, upsample_cfg=dict(mode='nearest'), norm_cfg=None, act_cfg=None):
         super(FPN, self).__init__()
         self.in_channels_list = in_channels_list
         self.upsample_cfg = upsample_cfg
         self.lateral_convs = nn.ModuleList()
         self.fpn_convs = nn.ModuleList()
         if 'inplace' in act_cfg: act_cfg['inplace'] = False
         for i in range(0, len(in_channels_list)):
             l_conv = nn.Sequential(
                 nn.Conv2d(in_channels_list[i], out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             fpn_conv = nn.Sequential(
                 nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.lateral_convs.append(l_conv)
             self.fpn_convs.append(fpn_conv)
     '''forward'''
     def forward(self, inputs):
         assert len(inputs) == len(self.in_channels_list)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/base/selfattention.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/base/selfattention.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Implementation of SelfAttentionBlock
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''SelfAttentionBlock'''
 class SelfAttentionBlock(nn.Module):
     def __init__(self, key_in_channels, query_in_channels, transform_channels, out_channels, share_key_query, 
                  query_downsample, key_downsample, key_query_num_convs, value_out_num_convs, key_query_norm, 
                  value_out_norm, matmul_norm, with_out_project, norm_cfg=None, act_cfg=None):
@@ -89,21 +89,21 @@
             context = self.out_project(context)
         return context
     '''build project'''
     def buildproject(self, in_channels, out_channels, num_convs, use_norm, norm_cfg, act_cfg):
         if use_norm:
             convs = [nn.Sequential(
                 nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )]
             for _ in range(num_convs - 1):
                 convs.append(nn.Sequential(
                     nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 ))
         else:
             convs = [nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False)]
             for _ in range(num_convs - 1):
                 convs.append(
                     nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ccnet/ccnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ccnet/ccnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,51 +3,54 @@
     Implementation of CCNet
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
-from mmcv.ops import CrissCrossAttention
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+try:
+    from mmcv.ops import CrissCrossAttention
+except:
+    CrissCrossAttention = None
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''CCNet'''
 class CCNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(CCNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build criss-cross attention
         self.conv_before_cca = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.cca = CrissCrossAttention(head_cfg['feats_channels'])
         self.conv_after_cca = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels']+head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'conv_before_cca', 'cca', 'conv_after_cca', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to cca
         feats = self.conv_before_cca(backbone_outputs[-1])
         for _ in range(self.cfg['head']['num_recurrence']):
             feats = self.cca(feats)
@@ -57,12 +60,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/ce2p.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/ce2p.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .epm import EdgePerceivingModule
 from ..pspnet import PyramidPoolingModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''CE2P'''
 class CE2P(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(CE2P, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -38,45 +38,45 @@
             'norm_cfg': copy.deepcopy(norm_cfg),
             'act_cfg': copy.deepcopy(act_cfg),
         }
         self.edge_net = EdgePerceivingModule(**epm_cfg)
         # build shortcut
         self.shortcut = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels_list'][0], head_cfg['shortcut_feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['shortcut_feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['shortcut_feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder stage1
         self.decoder_stage1 = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] + head_cfg['shortcut_feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout_stage1']), 
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build decoder stage1
         self.decoder_stage2 = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] + head_cfg['epm_hidden_channels'] * (len(head_cfg['in_channels_list']) - 1), head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout_stage2']), 
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'ppm_net', 'edge_net', 'shortcut', 'decoder_stage1', 'decoder_stage2']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to pyramid pooling module
         ppm_out = self.ppm_net(backbone_outputs[-1])
         ppm_out = F.interpolate(ppm_out, size=backbone_outputs[0].shape[2:], mode='bilinear', align_corners=self.align_corners)
         # feed to edge perceiving module
@@ -94,10 +94,10 @@
             edge = F.interpolate(edge, size=img_size, mode='bilinear', align_corners=self.align_corners)
             preds_stage1 = self.decoder_stage1[-1](feats_stage1)
             preds_stage1 = F.interpolate(preds_stage1, size=img_size, mode='bilinear', align_corners=self.align_corners)
             preds_stage2 = F.interpolate(preds_stage2, size=img_size, mode='bilinear', align_corners=self.align_corners)
             return self.calculatelosses(
                 predictions={'loss_cls_stage1': preds_stage1, 'loss_cls_stage2': preds_stage2, 'loss_edge': edge}, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses'],
             )
         return preds_stage2
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ce2p/epm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ce2p/epm.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     Implementation of EdgePerceivingModule
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''EdgePerceivingModule'''
 class EdgePerceivingModule(nn.Module):
     def __init__(self, in_channels_list=[256, 512, 1024], hidden_channels=256, out_channels=2, align_corners=False, norm_cfg=None, act_cfg=None):
         super(EdgePerceivingModule, self).__init__()
         self.align_corners = align_corners
         self.branches = nn.ModuleList()
         for in_channels in in_channels_list:
             self.branches.append(nn.Sequential(
                 nn.Conv2d(in_channels, hidden_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=hidden_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=hidden_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
         self.edge_conv = nn.Conv2d(hidden_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=True)
         self.fuse_conv = nn.Conv2d(out_channels * len(in_channels_list), out_channels, kernel_size=1, stride=1, padding=0, bias=True)
     '''forward'''
     def forward(self, x):
         assert len(x) == len(self.branches)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/cam.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/cam.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/danet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/danet.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .cam import ChannelAttentionModule
 from .pam import PositionAttentionModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''DANet'''
 class DANet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(DANet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build pam and pam decoder
         self.pam_in_conv = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.pam_net = PositionAttentionModule(head_cfg['feats_channels'], head_cfg['transform_channels'])
         self.pam_out_conv = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.decoder_pam = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build cam and cam decoder
         self.cam_in_conv = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.cam_net = ChannelAttentionModule()
         self.cam_out_conv = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.decoder_cam = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build the pam + cam decoder
@@ -61,15 +61,15 @@
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = [
             'backbone_net', 'pam_in_conv', 'pam_net', 'pam_out_conv', 'decoder_pam', 'cam_in_conv', 'cam_net', 
             'cam_out_conv', 'decoder_cam', 'decoder_pamcam', 'auxiliary_decoder'
         ]
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to pam
         feats_pam = self.pam_in_conv(backbone_outputs[-1])
         feats_pam = self.pam_net(feats_pam)
         feats_pam = self.pam_out_conv(feats_pam)
@@ -82,23 +82,23 @@
         preds_pamcam = self.decoder_pamcam(feats_sum)
         # forward according to the mode
         if self.mode == 'TRAIN':
             outputs_dict = self.forwardtrain(
                 predictions=preds_pamcam,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
                 compute_loss=False,
             )
             preds_pamcam = outputs_dict.pop('loss_cls')
             preds_pam = self.decoder_pam(feats_pam)
             preds_pam = F.interpolate(preds_pam, size=img_size, mode='bilinear', align_corners=self.align_corners)
             preds_cam = self.decoder_cam(feats_cam)
             preds_cam = F.interpolate(preds_cam, size=img_size, mode='bilinear', align_corners=self.align_corners)
             outputs_dict.update({'loss_cls_pam': preds_pam, 'loss_cls_cam': preds_cam, 'loss_cls_pamcam': preds_pamcam})
             return self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return preds_pamcam
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/danet/pam.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/danet/pam.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/aspp.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/aspp.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,46 +3,46 @@
     Implementation of Atrous Spatial Pyramid Pooling (ASPP)
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ASPP'''
 class ASPP(nn.Module):
     def __init__(self, in_channels, out_channels, dilations, align_corners=False, norm_cfg=None, act_cfg=None):
         super(ASPP, self).__init__()
         self.align_corners = align_corners
         self.parallel_branches = nn.ModuleList()
         for idx, dilation in enumerate(dilations):
             if dilation == 1:
                 branch = nn.Sequential(
                     nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=dilation, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                     BuildActivation(act_cfg)
                 )
             else:
                 branch = nn.Sequential(
                     nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=dilation, dilation=dilation, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                     BuildActivation(act_cfg)
                 )
             self.parallel_branches.append(branch)
         self.global_branch = nn.Sequential(
             nn.AdaptiveAvgPool2d((1, 1)),
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg)
         )
         self.bottleneck = nn.Sequential(
             nn.Conv2d(out_channels * (len(dilations) + 1), out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg)
         )
         self.in_channels = in_channels
         self.out_channels = out_channels
     '''forward'''
     def forward(self, x):
         size = x.size()
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3/deeplabv3.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3/deeplabv3.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,26 +34,26 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'aspp_net', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to aspp
         aspp_out = self.aspp_net(backbone_outputs[-1])
         # feed to decoder
         predictions = self.decoder(aspp_out)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/aspp.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/aspp.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,42 +3,42 @@
     Implementation of Depthwise Separable Atrous Spatial Pyramid Pooling (ASPP)
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, DepthwiseSeparableConv2d, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, DepthwiseSeparableConv2d, BuildNormalization
 
 
 '''DepthwiseSeparableASPP'''
 class DepthwiseSeparableASPP(nn.Module):
     def __init__(self, in_channels, out_channels, dilations, align_corners=False, norm_cfg=None, act_cfg=None):
         super(DepthwiseSeparableASPP, self).__init__()
         self.align_corners = align_corners
         self.parallel_branches = nn.ModuleList()
         for idx, dilation in enumerate(dilations):
             if dilation == 1:
                 branch = nn.Sequential(
                     nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, dilation=dilation, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             else:
                 branch = DepthwiseSeparableConv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=dilation, dilation=dilation, bias=False, norm_cfg=norm_cfg, act_cfg=act_cfg)
             self.parallel_branches.append(branch)
         self.global_branch = nn.Sequential(
             nn.AdaptiveAvgPool2d((1, 1)),
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.bottleneck = nn.Sequential(
             nn.Conv2d(out_channels * (len(dilations) + 1), out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.in_channels = in_channels
         self.out_channels = out_channels
     '''forward'''
     def forward(self, x):
         size = x.size()
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/deeplabv3plus/deeplabv3plus.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/deeplabv3plus/deeplabv3plus.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .aspp import DepthwiseSeparableASPP
-from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d
 
 
 '''Deeplabv3plus'''
 class Deeplabv3Plus(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(Deeplabv3Plus, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -27,15 +27,15 @@
             'norm_cfg': copy.deepcopy(norm_cfg),
             'act_cfg': copy.deepcopy(act_cfg),
         }
         self.aspp_net = DepthwiseSeparableASPP(**aspp_cfg)
         # build shortcut
         self.shortcut = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'][0], head_cfg['shortcut_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['shortcut_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['shortcut_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             DepthwiseSeparableConv2d(head_cfg['feats_channels'] + head_cfg['shortcut_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False, act_cfg=act_cfg, norm_cfg=norm_cfg),
             DepthwiseSeparableConv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False, act_cfg=act_cfg, norm_cfg=norm_cfg),
             nn.Dropout2d(head_cfg['dropout']),
@@ -44,15 +44,15 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'aspp_net', 'shortcut', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to aspp
         aspp_out = self.aspp_net(backbone_outputs[-1])
         aspp_out = F.interpolate(aspp_out, size=backbone_outputs[0].shape[2:], mode='bilinear', align_corners=self.align_corners)
         # feed to shortcut
@@ -62,12 +62,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/dcm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/dcm.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,34 @@
     Implementation of Dynamic Convolutional Module
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''DynamicConvolutionalModule'''
 class DynamicConvolutionalModule(nn.Module):
     def __init__(self, filter_size, is_fusion, in_channels, out_channels, norm_cfg=None, act_cfg=None):
         super(DynamicConvolutionalModule, self).__init__()
         self.filter_size, self.is_fusion = filter_size, is_fusion
         self.filter_gen_conv = nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0)
         self.input_redu_conv = nn.Sequential(
             nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
-        self.norm = BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg))
+        self.norm = BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg)
         self.activate = BuildActivation(act_cfg)
         if is_fusion:
             self.fusion_conv = nn.Sequential(
                 nn.Conv2d(out_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
     '''forward'''
     def forward(self, x):
         generated_filter = self.filter_gen_conv(F.adaptive_avg_pool2d(x, self.filter_size))
         x = self.input_redu_conv(x)
         b, c, h, w = x.shape
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/dmnet/dmnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dmnet/dmnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
 from .dcm import DynamicConvolutionalModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''DMNet'''
 class DMNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(DMNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -26,27 +26,27 @@
                 out_channels=head_cfg['feats_channels'],
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg,
             ))
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * len(head_cfg['filter_sizes']) + head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'dcm_modules', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to dcm
         dcm_outs = [backbone_outputs[-1]]
         for dcm_module in self.dcm_modules:
             dcm_outs.append(dcm_module(backbone_outputs[-1]))
@@ -55,12 +55,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/dnlblock.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/dnlblock.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/dnlnet/dnlnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/dnlnet/dnlnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,58 +5,58 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
 from .dnlblock import DisentangledNonLocal2d
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''DNLNet'''
 class DNLNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(DNLNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build disentangled non-local block
         self.conv_before_dnl = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.dnl_block = DisentangledNonLocal2d(
             in_channels=head_cfg['feats_channels'],
             reduction=head_cfg['reduction'],
             use_scale=head_cfg['use_scale'],
             mode=head_cfg['mode'],
             temperature=head_cfg['temperature'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg),
         )
         self.conv_after_dnl = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] + head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'conv_before_dnl', 'dnl_block', 'conv_after_dnl', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to disentangled non-local block
         feats = self.conv_before_dnl(backbone_outputs[-1])
         feats = self.dnl_block(feats)
         feats = self.conv_after_dnl(feats)
@@ -65,12 +65,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/ema.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/ema.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/emanet/emanet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/emanet/emanet.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,62 +5,62 @@
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from .ema import EMAModule
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''EMANet'''
 class EMANet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(EMANet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build the EMA module
         self.ema_in_conv = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.ema_mid_conv = nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0)
         for param in self.ema_mid_conv.parameters():
             param.requires_grad = False
         self.ema_module = EMAModule(
             channels=head_cfg['feats_channels'],
             num_bases=head_cfg['num_bases'],
             num_stages=head_cfg['num_stages'],
             momentum=head_cfg['momentum']
         )
         self.ema_out_conv = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
         )
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] + head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'ema_in_conv', 'ema_module', 'ema_out_conv', 'bottleneck', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to EMA module
         feats = self.ema_in_conv(backbone_outputs[-1])
         identity = feats
         feats = self.ema_mid_conv(feats)
@@ -74,12 +74,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/contextencoding.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/contextencoding.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,31 +5,31 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from .encoding import Encoding
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ContextEncoding'''
 class ContextEncoding(nn.Module):
     def __init__(self, in_channels, num_codes, norm_cfg=None, act_cfg=None):
         super(ContextEncoding, self).__init__()
         self.encoding_project = nn.Sequential(
             nn.Conv2d(in_channels, in_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         encoding_norm_cfg = copy.deepcopy(norm_cfg)
         encoding_norm_cfg['type'] = encoding_norm_cfg['type'].replace('2d', '1d')
         self.encoding = nn.Sequential(
             Encoding(channels=in_channels, num_codes=num_codes),
-            BuildNormalization(constructnormcfg(placeholder=num_codes, norm_cfg=encoding_norm_cfg)),
+            BuildNormalization(placeholder=num_codes, norm_cfg=encoding_norm_cfg),
             BuildActivation(act_cfg),
         )
         self.fc = nn.Sequential(
             nn.Linear(in_channels, in_channels),
             nn.Sigmoid()
         )
     '''forward'''
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/encnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/encnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .contextencoding import ContextEncoding
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ENCNet'''
 class ENCNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(ENCNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build encoding
         # --base structurs
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels_list'][-1], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.enc_module = ContextEncoding(
             in_channels=head_cfg['feats_channels'],
             num_codes=head_cfg['num_codes'],
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
@@ -33,20 +33,20 @@
         # --extra structures
         extra_cfg = head_cfg['extra']
         if extra_cfg['add_lateral']:
             self.lateral_convs = nn.ModuleList()
             for in_channels in head_cfg['in_channels_list'][:-1]:
                 self.lateral_convs.append(
                     nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0),
-                    BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             self.fusion = nn.Sequential(
                 nn.Conv2d(len(head_cfg['in_channels_list']) * head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
         if extra_cfg['use_se_loss']:
             self.se_layer = nn.Linear(head_cfg['feats_channels'], cfg['num_classes'])
         # build decoder
         self.decoder = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
@@ -55,15 +55,15 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'bottleneck', 'enc_module', 'decoder', 'lateral_convs', 'fusion', 'se_layer', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to context encoding
         feats = self.bottleneck(backbone_outputs[-1])
         if hasattr(self, 'lateral_convs'):
             lateral_outs = [
@@ -77,24 +77,24 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             outputs_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
                 compute_loss=False,
             )
             if hasattr(self, 'se_layer'):
                 outputs_dict.update({'loss_se': predictions_se})
             return self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return predictions
     '''convert to onehot labels'''
     def onehot(self, labels, num_classes):
         batch_size = labels.size(0)
         labels_onehot = labels.new_zeros((batch_size, num_classes))
         for i in range(batch_size):
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/encnet/encoding.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/encnet/encoding.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/fastfcn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/fastfcn.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 '''FastFCN'''
 class FastFCN(nn.Module):
     def __init__(self, cfg, mode):
         super(FastFCN, self).__init__()
         self.align_corners, self.norm_cfg, self.act_cfg, head_cfg = cfg['align_corners'], cfg['norm_cfg'], cfg['act_cfg'], cfg['head']
         # build segmentor
         supported_models = {
-            'fcn': FCN,
-            'encnet': ENCNet,
-            'pspnet': PSPNet,
-            'deeplabv3': Deeplabv3,
+            'FCN': FCN,
+            'ENCNet': ENCNet,
+            'PSPNet': PSPNet,
+            'Deeplabv3': Deeplabv3,
         }
         model_type = cfg['segmentor']
         assert model_type in supported_models, 'unsupport model_type %s' % model_type
         self.segmentor = supported_models[model_type](cfg, mode)
         # build jpu neck
         jpu_cfg = head_cfg['jpu']
         if 'act_cfg' not in jpu_cfg: jpu_cfg.update({'act_cfg': self.act_cfg})
         if 'norm_cfg' not in jpu_cfg: jpu_cfg.update({'norm_cfg': self.norm_cfg})
         if 'align_corners' not in jpu_cfg: jpu_cfg.update({'align_corners': self.align_corners})
         self.jpu_neck = JPU(**jpu_cfg)
         self.segmentor.transforminputs = self.transforminputs
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None, **kwargs):
-        return self.segmentor(x, targets, losses_cfg, **kwargs)
+    def forward(self, x, targets=None, **kwargs):
+        return self.segmentor(x, targets, **kwargs)
     '''transform inputs'''
     def transforminputs(self, x_list, selected_indices=None):
         if selected_indices is None:
             if self.cfg['backbone']['series'] in ['hrnet']:
                 selected_indices = (0, 0, 0, 0)
             else:
                 selected_indices = (0, 1, 2, 3)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/fastfcn/jpu.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fastfcn/jpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d
 
 
 '''JPU'''
 class JPU(nn.Module):
     def __init__(self, in_channels_list=(512, 1024, 2048), mid_channels=512, start_level=0, end_level=-1, dilations=(1, 2, 4, 8), 
                  align_corners=False, norm_cfg=None, act_cfg=None):
         super(JPU, self).__init__()
@@ -30,15 +30,15 @@
         self.align_corners = align_corners
         # define modules
         self.conv_layers = nn.ModuleList()
         self.dilation_layers = nn.ModuleList()
         for i in range(self.start_level, self.backbone_end_level):
             conv_layer = nn.Sequential(
                 nn.Conv2d(self.in_channels_list[i], self.mid_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=self.mid_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=self.mid_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.conv_layers.append(conv_layer)
         for idx in range(len(dilations)):
             dilation_layer = DepthwiseSeparableConv2d(
                 in_channels=(self.backbone_end_level - self.start_level) * self.mid_channels,
                 out_channels=self.mid_channels,
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/fcn/fcn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/fcn/fcn.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
     Implementation of FCN
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization, DepthwiseSeparableConv2d
 
 
 '''FCN'''
 class FCN(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(FCN, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build decoder
         convs = []
         for idx in range(head_cfg.get('num_convs', 2)):
             if idx == 0:
                 conv = nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False)
             else:
                 conv = nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False)
-            norm = BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg))
+            norm = BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)
             act = BuildActivation(act_cfg)
             convs += [conv, norm, act]
         convs.append(nn.Dropout2d(head_cfg['dropout']))
         if head_cfg.get('num_convs', 2) > 0:
             convs.append(nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0))
         else:
             convs.append(nn.Conv2d(head_cfg['in_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0))
@@ -34,27 +34,27 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to decoder
         predictions = self.decoder(backbone_outputs[-1])
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
 
 
 '''DepthwiseSeparableFCN'''
@@ -95,24 +95,24 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to decoder
         predictions = self.decoder(backbone_outputs[-1])
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/contextblock.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/contextblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Function:
     Implementation of ContextBlock
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ContextBlock'''
 class ContextBlock(nn.Module):
     def __init__(self, in_channels, ratio, pooling_type='att', fusion_types=('channel_add', ), norm_cfg=None, act_cfg=None):
         super(ContextBlock, self).__init__()
         assert pooling_type in ['avg', 'att']
@@ -27,24 +27,24 @@
             self.conv_mask = nn.Conv2d(in_channels, 1, kernel_size=1, stride=1, padding=0)
             self.softmax = nn.Softmax(dim=2)
         else:
             self.avg_pool = nn.AdaptiveAvgPool2d(1)
         if 'channel_add' in fusion_types:
             self.channel_add_conv = nn.Sequential(
                 nn.Conv2d(self.in_channels, self.planes, kernel_size=1, stride=1, padding=0),
-                BuildNormalization(constructnormcfg(placeholder=[self.planes, 1, 1], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=[self.planes, 1, 1], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(self.planes, self.in_channels, kernel_size=1, stride=1, padding=0)
             )
         else:
             self.channel_add_conv = None
         if 'channel_mul' in fusion_types:
             self.channel_mul_conv = nn.Sequential(
                 nn.Conv2d(self.in_channels, self.planes, kernel_size=1, stride=1, padding=0),
-                BuildNormalization(constructnormcfg(placeholder=[self.planes, 1, 1], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=[self.planes, 1, 1], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(self.planes, self.in_channels, kernel_size=1, stride=1, padding=0)
             )
         else:
             self.channel_mul_conv = None
     '''spatial pool'''
     def spatialpool(self, x):
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/gcnet/gcnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/gcnet/gcnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,57 +5,57 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
 from .contextblock import ContextBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''GCNet'''
 class GCNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(GCNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build context block
         self.conv_before_cb = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.contextblock_net = ContextBlock(
             in_channels=head_cfg['feats_channels'],
             ratio=head_cfg['ratio'],
             pooling_type=head_cfg['pooling_type'],
             fusion_types=head_cfg['fusion_types'],
             norm_cfg=head_cfg.get('norm_cfg', copy.deepcopy(norm_cfg)),
             act_cfg=head_cfg.get('act_cfg', copy.deepcopy(act_cfg)),
         )
         self.conv_after_cb = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'] + head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'conv_before_cb', 'contextblock_net', 'conv_after_cb', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to context block
         feats = self.conv_before_cb(backbone_outputs[-1])
         feats = self.contextblock_net(feats)
         feats = self.conv_after_cb(feats)
@@ -64,12 +64,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icneck.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icneck.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
     Implementation of ICNeck
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildNormalization, BuildActivation, constructnormcfg
+from ...backbones import BuildNormalization, BuildActivation
 
 
 '''CascadeFeatureFusion'''
 class CascadeFeatureFusion(nn.Module):
     def __init__(self, low_channels, high_channels, out_channels, norm_cfg=None, act_cfg=None, align_corners=False):
         super(CascadeFeatureFusion, self).__init__()
         self.align_corners = align_corners
         self.conv_low = nn.Sequential(
             nn.Conv2d(low_channels, out_channels, kernel_size=3, stride=1, padding=2, dilation=2, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.conv_high = nn.Sequential(
             nn.Conv2d(high_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x_low, x_high):
         x_low = F.interpolate(x_low, size=x_high.shape[2:], mode='bilinear', align_corners=self.align_corners)
         x_low = self.conv_low(x_low)
         x_high = self.conv_high(x_high)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from .icneck import ICNeck
 from ..base import BaseSegmentor
 from .icnetencoder import ICNetEncoder
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ICNet'''
 class ICNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(ICNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -33,38 +33,38 @@
             'norm_cfg': norm_cfg.copy(),
             'align_corners': align_corners,
         }
         self.neck = ICNeck(**neck_cfg)
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'neck', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to neck
         backbone_outputs = self.neck(backbone_outputs)
         # feed to decoder
         predictions = self.decoder(backbone_outputs[-1])
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/icnet/icnetencoder.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/icnet/icnetencoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..pspnet import PyramidPoolingModule
-from ...backbones import BuildNormalization, BuildActivation, BuildBackbone, constructnormcfg
+from ...backbones import BuildNormalization, BuildActivation, BuildBackbone
 
 
 '''ICNet-Encoder'''
 class ICNetEncoder(nn.Module):
     def __init__(self, backbone_cfg=None, in_channels=3, layer_channels_list=(512, 2048), light_branch_middle_channels=32, psp_out_channels=512, 
                  out_channels_list=(64, 256, 256), pool_scales=(1, 2, 3, 6), norm_cfg=None, act_cfg=None, align_corners=False):
         super(ICNetEncoder, self).__init__()
@@ -29,31 +29,31 @@
             out_channels=psp_out_channels,
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
             align_corners=align_corners,
         )
         self.conv_sub1 = nn.Sequential(
             nn.Conv2d(in_channels, light_branch_middle_channels, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=light_branch_middle_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=light_branch_middle_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(light_branch_middle_channels, light_branch_middle_channels, kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=light_branch_middle_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=light_branch_middle_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(light_branch_middle_channels, out_channels_list[0], kernel_size=3, stride=2, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels_list[0], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels_list[0], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.conv_sub2 = nn.Sequential(
             nn.Conv2d(layer_channels_list[0], out_channels_list[1], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels_list[1], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels_list[1], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.conv_sub4 = nn.Sequential(
             nn.Conv2d(psp_out_channels, out_channels_list[2], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels_list[2], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels_list[2], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, x):
         output = []
         # sub 1
         output.append(self.conv_sub1(x))
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/isanet/isanet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isanet/isanet.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from ..base import SelfAttentionBlock as _SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''SelfAttentionBlock'''
 class SelfAttentionBlock(_SelfAttentionBlock):
     def __init__(self, in_channels, feats_channels, norm_cfg, act_cfg):
         super(SelfAttentionBlock, self).__init__(
             key_in_channels=in_channels,
@@ -53,15 +53,15 @@
     def __init__(self, cfg, mode):
         super(ISANet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build isa module
         self.down_factor = head_cfg['down_factor']
         self.in_conv = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.global_relation = SelfAttentionBlock(
             in_channels=head_cfg['feats_channels'],
             feats_channels=head_cfg['isa_channels'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg)
@@ -70,30 +70,30 @@
             in_channels=head_cfg['feats_channels'],
             feats_channels=head_cfg['isa_channels'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg)
         )
         self.out_conv = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * 2, head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'in_conv', 'global_relation', 'local_relation', 'out_conv', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to isa module
         feats = self.in_conv(backbone_outputs[-1])
         residual = feats
         n, c, h, w = feats.size()
@@ -128,12 +128,12 @@
         predictions = self.decoder(feats)
         # return according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/imagelevel.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/imagelevel.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ImageLevelContext'''
 class ImageLevelContext(nn.Module):
     def __init__(self, feats_channels, transform_channels, concat_input=False, align_corners=False, norm_cfg=None, act_cfg=None):
         super(ImageLevelContext, self).__init__()
         self.align_corners = align_corners
@@ -33,15 +33,15 @@
             with_out_project=True,
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
         )
         if concat_input:
             self.bottleneck = nn.Sequential(
                 nn.Conv2d(feats_channels * 2, feats_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=feats_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=feats_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
     '''forward'''
     def forward(self, x):
         x_global = self.global_avgpool(x)
         x_global = F.interpolate(x_global, size=x.size()[2:], mode='bilinear', align_corners=self.align_corners)
         feats_il = self.correlate_net(x, torch.cat([x_global, x], dim=1))
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/isnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/isnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .imagelevel import ImageLevelContext
 from .semanticlevel import SemanticLevelContext
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ISNet'''
 class ISNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(ISNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build bottleneck
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build image-level context module
         ilc_cfg = {
             'feats_channels': head_cfg['feats_channels'],
             'transform_channels': head_cfg['transform_channels'],
             'concat_input': head_cfg['concat_input'],
@@ -43,28 +43,28 @@
             'norm_cfg': copy.deepcopy(norm_cfg),
             'act_cfg': copy.deepcopy(act_cfg),
         }
         self.slc_net = SemanticLevelContext(**slc_cfg)
         # build decoder
         self.decoder_stage1 = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         if head_cfg['shortcut']['is_on']:
             self.shortcut = nn.Sequential(
                 nn.Conv2d(head_cfg['shortcut']['in_channels'], head_cfg['shortcut']['feats_channels'], kernel_size=1, stride=1, padding=0),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['shortcut']['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['shortcut']['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.decoder_stage2 = nn.Sequential(
                 nn.Conv2d(head_cfg['feats_channels'] + head_cfg['shortcut']['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Dropout2d(head_cfg['dropout']),
                 nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
             )
         else:
             self.decoder_stage2 = nn.Sequential(
                 nn.Dropout2d(head_cfg['dropout']),
@@ -73,15 +73,15 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'bottleneck', 'ilc_net', 'slc_net', 'shortcut', 'decoder_stage1', 'decoder_stage2', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to bottleneck
         feats = self.bottleneck(backbone_outputs[-1])
         # feed to image-level context module
         feats_il = self.ilc_net(feats)
@@ -100,20 +100,20 @@
         preds_stage2 = self.decoder_stage2(feats_sl)
         # return according to the mode
         if self.mode == 'TRAIN':
             outputs_dict = self.forwardtrain(
                 predictions=preds_stage2,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
                 compute_loss=False,
             )
             preds_stage2 = outputs_dict.pop('loss_cls')
             preds_stage1 = F.interpolate(preds_stage1, size=img_size, mode='bilinear', align_corners=self.align_corners)
             outputs_dict.update({'loss_cls_stage1': preds_stage1, 'loss_cls_stage2': preds_stage2})
             return self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return preds_stage2
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/isnet/semanticlevel.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/isnet/semanticlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''SemanticLevelContext'''
 class SemanticLevelContext(nn.Module):
     def __init__(self, feats_channels, transform_channels, concat_input=False, norm_cfg=None, act_cfg=None):
         super(SemanticLevelContext, self).__init__()
         self.correlate_net = SelfAttentionBlock(
@@ -31,15 +31,15 @@
             with_out_project=True,
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
         )
         if concat_input:
             self.bottleneck = nn.Sequential(
                 nn.Conv2d(feats_channels * 2, feats_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=feats_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=feats_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
     '''forward'''
     def forward(self, x, preds, feats_il):
         inputs = x
         batch_size, num_channels, h, w = x.size()
         num_classes = preds.size(1)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/lrasppnet/lrasppnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/lrasppnet/lrasppnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''LRASPPNet'''
 class LRASPPNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(LRASPPNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -23,41 +23,41 @@
                 f'conv{idx}', 
                 nn.Conv2d(head_cfg['in_channels_list'][idx], branch_channels, kernel_size=1, stride=1, padding=0, bias=False)
             )
             self.branch_ups.add_module(
                 f'conv{idx}', 
                 nn.Sequential(
                     nn.Conv2d(head_cfg['feats_channels'] + branch_channels, head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 )
             )
         self.aspp_conv = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels_list'][-1], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.image_pool = nn.Sequential(
             nn.AvgPool2d(kernel_size=49, stride=(16, 20)),
             nn.Conv2d(head_cfg['in_channels_list'][-1], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             nn.Sigmoid(),
         )
         self.bottleneck = nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False)
         # build decoder
         self.decoder = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'branch_convs', 'branch_ups', 'aspp_conv', 'image_pool', 'bottleneck', 'decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to aspp
         feats = self.aspp_conv(backbone_outputs[-1]) * F.interpolate(self.image_pool(backbone_outputs[-1]), size=backbone_outputs[-1].size()[2:], mode='bilinear', align_corners=self.align_corners)
         feats = self.bottleneck(feats)
         for idx in range(len(self.cfg['head']['branch_channels_list']) - 1, -1, -1):
@@ -68,12 +68,12 @@
         predictions = self.decoder(feats)
         # return according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/maskformer.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/maskformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from ..base import BaseSegmentor
 from ..pspnet import PyramidPoolingModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 from .transformers import Predictor, SetCriterion, Transformer, HungarianMatcher
 
 
 '''MaskFormer'''
 class MaskFormer(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(MaskFormer, self).__init__(cfg, mode)
@@ -33,23 +33,23 @@
         # build lateral convs
         act_cfg_copy = copy.deepcopy(act_cfg)
         if 'inplace' in act_cfg_copy: act_cfg_copy['inplace'] = False
         self.lateral_convs = nn.ModuleList()
         for in_channels in head_cfg['in_channels_list'][:-1]:
             self.lateral_convs.append(nn.Sequential(
                 nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg_copy),
             ))
         # build fpn convs
         self.fpn_convs = nn.ModuleList()
         for in_channels in [head_cfg['feats_channels'], ] * len(self.lateral_convs):
             self.fpn_convs.append(nn.Sequential(
                 nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg_copy),
             ))
         # build decoder
         self.decoder_mask = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['mask_feats_channels'], kernel_size=3, stride=1, padding=1)
         )
         head_cfg['predictor']['num_classes'] = cfg['num_classes']
@@ -68,15 +68,15 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'ppm_net', 'lateral_convs', 'fpn_convs', 'decoder_mask', 'decoder_predictor']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to pyramid pooling module
         ppm_out = self.ppm_net(backbone_outputs[-1])
         # apply fpn
         inputs = backbone_outputs[:-1]
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/criterion.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/criterion.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/matcher.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/matcher.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/predictor.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/predictor.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/maskformer/transformers/transformer.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/maskformer/transformers/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ....backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ....backbones import BuildActivation, BuildNormalization
 
 
 '''TransformerEncoderLayer'''
 class TransformerEncoderLayer(nn.Module):
     def __init__(self, d_model, nhead, dim_feedforward=2048, dropout=0.1, norm_cfg=None, act_cfg=None, norm_before=False):
         super(TransformerEncoderLayer, self).__init__()
         self.norm_before = norm_before
@@ -21,16 +21,16 @@
         self.linear1 = nn.Linear(d_model, dim_feedforward)
         self.linear2 = nn.Linear(dim_feedforward, d_model)
         # dropout
         self.dropout = nn.Dropout(dropout)
         self.dropout1 = nn.Dropout(dropout)
         self.dropout2 = nn.Dropout(dropout)
         # norm
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
+        self.norm1 = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
+        self.norm2 = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
         # act
         self.activation = BuildActivation(act_cfg)
     '''with pos embed'''
     def withposembed(self, tensor, pos=None):
         return tensor if pos is None else tensor + pos
     '''norm_before=False forward'''
     def normafterforward(self, src, src_mask=None, src_key_padding_mask=None, pos=None):
@@ -81,17 +81,17 @@
         self.norm_before = norm_before
         self.self_attn = nn.MultiheadAttention(d_model, nhead, dropout=dropout)
         self.multihead_attn = nn.MultiheadAttention(d_model, nhead, dropout=dropout)
         # linear
         self.linear1 = nn.Linear(d_model, dim_feedforward)
         self.linear2 = nn.Linear(dim_feedforward, d_model)
         # norm
-        self.norm1 = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
-        self.norm2 = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
-        self.norm3 = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
+        self.norm1 = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
+        self.norm2 = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
+        self.norm3 = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
         # dropout
         self.dropout = nn.Dropout(dropout)
         self.dropout1 = nn.Dropout(dropout)
         self.dropout2 = nn.Dropout(dropout)
         self.dropout3 = nn.Dropout(dropout)
         # act
         self.activation = BuildActivation(act_cfg)
@@ -148,19 +148,19 @@
 class Transformer(nn.Module):
     def __init__(self, d_model=512, nhead=8, num_encoder_layers=6, num_decoder_layers=6, dim_feedforward=2048, dropout=0.1, norm_cfg=None, act_cfg=None, norm_before=False, return_intermediate_dec=False):
         super(Transformer, self).__init__()
         self.nhead = nhead
         self.d_model = d_model
         # encoder
         encoder_layer = TransformerEncoderLayer(d_model, nhead, dim_feedforward, dropout, norm_cfg, act_cfg, norm_before)
-        encoder_norm = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg)) if norm_before else None
+        encoder_norm = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg) if norm_before else None
         self.encoder = TransformerEncoder(encoder_layer, num_encoder_layers, encoder_norm)
         # decoder
         decoder_layer = TransformerDecoderLayer(d_model, nhead, dim_feedforward, dropout, norm_cfg, act_cfg, norm_before)
-        decoder_norm = BuildNormalization(constructnormcfg(placeholder=d_model, norm_cfg=norm_cfg))
+        decoder_norm = BuildNormalization(placeholder=d_model, norm_cfg=norm_cfg)
         self.decoder = TransformerDecoder(decoder_layer, num_decoder_layers, decoder_norm, return_intermediate=return_intermediate_dec)
         # reset parameters
         self.resetparameters()
     '''reset parameters'''
     def resetparameters(self):
         for p in self.parameters():
             if p.dim() > 1: nn.init.xavier_uniform_(p)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/initmemory.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/initmemory.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/memory.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from ..base import SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''FeaturesMemory'''
 class FeaturesMemory(nn.Module):
     def __init__(self, num_classes, feats_channels, transform_channels, out_channels, use_context_within_image=True, 
                  num_feats_per_cls=1, use_hard_aggregate=False, norm_cfg=None, act_cfg=None):
         super(FeaturesMemory, self).__init__()
@@ -48,15 +48,15 @@
                     with_out_project=True,
                     norm_cfg=norm_cfg,
                     act_cfg=act_cfg,
                 )
                 self.self_attentions.append(self_attention)
             self.fuse_memory_conv = nn.Sequential(
                 nn.Conv2d(feats_channels * self.num_feats_per_cls, feats_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=feats_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=feats_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
         else:
             self.self_attention = SelfAttentionBlock(
                 key_in_channels=feats_channels,
                 query_in_channels=feats_channels,
                 transform_channels=transform_channels,
@@ -72,15 +72,15 @@
                 with_out_project=True,
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg,
             )
         # whether need to fuse the contextual information within the input image
         self.bottleneck = nn.Sequential(
             nn.Conv2d(feats_channels * 2, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         if use_context_within_image:
             self.self_attention_ms = SelfAttentionBlock(
                 key_in_channels=feats_channels,
                 query_in_channels=feats_channels,
                 transform_channels=transform_channels,
@@ -95,15 +95,15 @@
                 matmul_norm=True,
                 with_out_project=True,
                 norm_cfg=norm_cfg,
                 act_cfg=act_cfg,
             )
             self.bottleneck_ms = nn.Sequential(
                 nn.Conv2d(feats_channels * 2, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
     '''forward'''
     def forward(self, feats, preds=None, feats_ms=None):
         batch_size, num_channels, h, w = feats.size()
         # extract the history features
         # --(B, num_classes, H, W) --> (B*H*W, num_classes)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/memorynet/memorynet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/memorynet/memorynet.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from ..deeplabv3 import ASPP
 from ..base import BaseSegmentor
 from .memory import FeaturesMemory
 from ..pspnet import PyramidPoolingModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''MemoryNet'''
 class MemoryNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(MemoryNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build norm layer
         if 'norm_cfg' in head_cfg:
             self.norm_layers = nn.ModuleList()
             for in_channels in head_cfg['norm_cfg']['in_channels_list']:
                 norm_cfg_copy = head_cfg['norm_cfg'].copy()
                 norm_cfg_copy.pop('in_channels_list')
-                norm_layer = BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg_copy))
+                norm_layer = BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg_copy)
                 self.norm_layers.append(norm_layer)
         # build memory
         if head_cfg['downsample_backbone']['stride'] > 1:
             self.downsample_backbone = nn.Sequential(
                 nn.Conv2d(head_cfg['in_channels'], head_cfg['in_channels'], **head_cfg['downsample_backbone']),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['in_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['in_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
         context_within_image_cfg = head_cfg['context_within_image']
         if context_within_image_cfg['is_on']:
             cwi_cfg = context_within_image_cfg['cfg']
             cwi_cfg.update({
                 'in_channels': head_cfg['in_channels'],
@@ -49,15 +49,15 @@
             supported_context_modules = {
                 'aspp': ASPP,
                 'ppm': PyramidPoolingModule,
             }
             self.context_within_image_module = supported_context_modules[context_within_image_cfg['type']](**cwi_cfg)
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.memory_module = FeaturesMemory(
             num_classes=cfg['num_classes'], 
             feats_channels=head_cfg['feats_channels'], 
             transform_channels=head_cfg['transform_channels'],
             num_feats_per_cls=head_cfg['num_feats_per_cls'],
@@ -66,37 +66,37 @@
             use_hard_aggregate=head_cfg['use_hard_aggregate'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg),
         )
         # build decoder
         self.decoder_stage1 = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0),
         )
         self.decoder_stage2 = nn.Sequential(
             nn.Conv2d(head_cfg['out_channels'], head_cfg['out_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['out_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['out_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['out_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = [
             'backbone_net', 'bottleneck', 'memory_module', 'decoder_stage1', 'decoder_stage2', 'norm_layers',
             'downsample_backbone', 'context_within_image_module', 'auxiliary_decoder'
         ]
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None, **kwargs):
+    def forward(self, x, targets=None, **kwargs):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         if hasattr(self, 'norm_layers'):
             assert len(backbone_outputs) == len(self.norm_layers)
             for idx in range(len(backbone_outputs)):
                 backbone_outputs[idx] = self.norm(backbone_outputs[idx], self.norm_layers[idx])
@@ -113,32 +113,32 @@
         preds_stage2 = self.decoder_stage2(memory_output)
         # forward according to the mode
         if self.mode == 'TRAIN':
             outputs_dict = self.forwardtrain(
                 predictions=preds_stage2,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
                 compute_loss=False,
             )
             preds_stage2 = outputs_dict.pop('loss_cls')
             preds_stage1 = F.interpolate(preds_stage1, size=img_size, mode='bilinear', align_corners=self.align_corners)
             outputs_dict.update({'loss_cls_stage1': preds_stage1, 'loss_cls_stage2': preds_stage2})
             with torch.no_grad():
                 self.memory_module.update(
                     features=F.interpolate(memory_input, size=img_size, mode='bilinear', align_corners=self.align_corners), 
-                    segmentation=targets['segmentation'],
+                    segmentation=targets['seg_target'],
                     learning_rate=kwargs['learning_rate'],
                     **self.cfg['head']['update_cfg']
                 )
             loss, losses_log_dict = self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
             if (kwargs['epoch'] > 1) and self.cfg['head']['use_loss']:
                 loss_memory, loss_memory_log = self.calculatememoryloss(stored_memory)
                 loss += loss_memory
                 losses_log_dict['loss_memory'] = loss_memory_log
                 total = losses_log_dict.pop('total') + losses_log_dict['loss_memory']
                 losses_log_dict['total'] = total
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalblock.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalblock.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Implementation of NonLocal2d, NonLocal3d, NonLocal3d
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 from abc import ABCMeta
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''_NonLocalNd'''
 class _NonLocalNd(nn.Module, metaclass=ABCMeta):
     def __init__(self, in_channels, reduction=2, use_scale=True, mode='embeddedgaussian', norm_cfg=None, act_cfg=None):
         super(_NonLocalNd, self).__init__()
         assert mode in ['gaussian', 'embeddedgaussian', 'dotproduct', 'concatenation']
@@ -21,15 +21,15 @@
         self.inter_channels = max(in_channels // reduction, 1)
         self.mode = mode
         self.g = nn.Sequential(
             nn.Conv2d(self.in_channels, self.inter_channels, kernel_size=1, stride=1, padding=0)
         )
         self.conv_out = nn.Sequential(
             nn.Conv2d(self.inter_channels, self.in_channels, kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=self.in_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=self.in_channels, norm_cfg=norm_cfg),
         )
         if self.mode != 'gaussian':
             self.theta = nn.Sequential(
                 nn.Conv2d(self.in_channels, self.inter_channels, kernel_size=1, stride=1, padding=0)
             )
             self.phi = nn.Sequential(
                 nn.Conv2d(self.in_channels, self.inter_channels, kernel_size=1, stride=1, padding=0)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/nonlocalnet/nonlocalnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,57 +5,57 @@
     Zhenchao Jin
 '''
 import copy
 import torch
 import torch.nn as nn
 from ..base import BaseSegmentor
 from .nonlocalblock import NonLocal2d
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''NonLocalNet'''
 class NonLocalNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(NonLocalNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build non-local block
         self.conv_before_nl = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.nl_block = NonLocal2d(
             in_channels=head_cfg['feats_channels'],
             reduction=head_cfg['reduction'],
             use_scale=head_cfg['use_scale'],
             mode=head_cfg['mode'],
             norm_cfg=copy.deepcopy(norm_cfg),
             act_cfg=copy.deepcopy(act_cfg),
         )
         self.conv_after_nl = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'] + head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'conv_before_nl', 'nl_block', 'conv_after_nl', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to non-local block
         feats = self.conv_before_nl(backbone_outputs[-1])
         feats = self.nl_block(feats)
         feats = self.conv_after_nl(feats)
@@ -64,12 +64,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/objectcontext.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/objectcontext.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import SelfAttentionBlock
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''ObjectContextBlock'''
 class ObjectContextBlock(SelfAttentionBlock):
     def __init__(self, in_channels, transform_channels, scale, align_corners=False, norm_cfg=None, act_cfg=None):
         self.align_corners = align_corners
         if scale > 1:
@@ -34,15 +34,15 @@
             matmul_norm=True, 
             with_out_project=True,
             norm_cfg=norm_cfg,
             act_cfg=act_cfg,
         )
         self.bottleneck = nn.Sequential(
             nn.Conv2d(in_channels*2, in_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
     '''forward'''
     def forward(self, query_feats, key_feats):
         h, w = query_feats.size()[2:]
         context = super(ObjectContextBlock, self).forward(query_feats, key_feats)
         output = self.bottleneck(torch.cat([context, query_feats], dim=1))
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/ocrnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/ocrnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from .objectcontext import ObjectContextBlock
 from .spatialgather import SpatialGatherModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''OCRNet'''
 class OCRNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(OCRNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build auxiliary decoder
         assert (cfg['auxiliary'] is not None) and isinstance(cfg['auxiliary'], dict), 'auxiliary must be given and only support dict type'
         self.setauxiliarydecoder(cfg['auxiliary'])
         # build bottleneck
         self.bottleneck = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build spatial gather module
         spatialgather_cfg = {
             'scale': head_cfg['scale']
         }
         self.spatial_gather_module = SpatialGatherModule(**spatialgather_cfg)
@@ -48,15 +48,15 @@
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'bottleneck', 'spatial_gather_module', 'object_context_block', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to auxiliary decoder
         predictions_aux = self.auxiliary_decoder(backbone_outputs[-2])
         # feed to bottleneck
         feats = self.bottleneck(backbone_outputs[-1])
@@ -68,10 +68,10 @@
         # return according to the mode
         if self.mode == 'TRAIN':
             predictions = F.interpolate(predictions, size=img_size, mode='bilinear', align_corners=self.align_corners)
             predictions_aux = F.interpolate(predictions_aux, size=img_size, mode='bilinear', align_corners=self.align_corners)
             return self.calculatelosses(
                 predictions={'loss_cls': predictions, 'loss_aux': predictions_aux}, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/ocrnet/spatialgather.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/ocrnet/spatialgather.py`

 * *Files identical despite different names*

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/pointrend/pointrend.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pointrend/pointrend.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,19 @@
     Zhenchao Jin
 '''
 import torch
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import FPN, BaseSegmentor
-from mmcv.ops import point_sample as PointSample
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+try:
+    from mmcv.ops import point_sample as PointSample
+except:
+    PointSample = None
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''PointRend'''
 class PointRend(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(PointRend, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -29,15 +32,15 @@
         self.scale_heads, feature_stride_list = nn.ModuleList(), head_cfg['feature_stride_list']
         for i in range(len(feature_stride_list)):
             head_length = max(1, int(np.log2(feature_stride_list[i]) - np.log2(feature_stride_list[0])))
             scale_head = []
             for k in range(head_length):
                 scale_head.append(nn.Sequential(
                     nn.Conv2d(head_cfg['feats_channels'] if k == 0 else head_cfg['scale_head_channels'], head_cfg['scale_head_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=head_cfg['scale_head_channels'], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=head_cfg['scale_head_channels'], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 ))
                 if feature_stride_list[i] != feature_stride_list[0]:
                     scale_head.append(
                         nn.Upsample(scale_factor=2, mode='bilinear', align_corners=align_corners)
                     )
             self.scale_heads.append(nn.Sequential(*scale_head))
@@ -45,15 +48,15 @@
         self.num_fcs, self.coarse_pred_each_layer = head_cfg['num_fcs'], head_cfg['coarse_pred_each_layer']
         fc_in_channels = sum(head_cfg['pointrend_in_channels_list']) + cfg['num_classes']
         fc_channels = head_cfg['feats_channels']
         self.fcs = nn.ModuleList()
         for k in range(self.num_fcs):
             fc = nn.Sequential(
                 nn.Conv1d(fc_in_channels, fc_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=fc_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=fc_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.fcs.append(fc)
             fc_in_channels = fc_channels
             fc_in_channels += cfg['num_classes'] if self.coarse_pred_each_layer else 0
         # build decoder
         self.decoder = nn.Sequential(
@@ -64,15 +67,15 @@
         assert (cfg['auxiliary'] is not None) and isinstance(cfg['auxiliary'], dict), 'auxiliary must be given and only support dict type'
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'fpn_neck', 'scale_heads', 'fcs', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to fpn
         fpn_outs = self.fpn_neck(list(backbone_outputs))
         feats = self.scale_heads[0](fpn_outs[0])
         for i in range(1, len(self.cfg['head']['feature_stride_list'])):
@@ -88,23 +91,23 @@
             coarse_point_feats = self.getcoarsepointfeats(predictions_aux, points)
             outputs = torch.cat([fine_grained_point_feats, coarse_point_feats], dim=1)
             for fc in self.fcs:
                 outputs = fc(outputs)
                 if self.coarse_pred_each_layer:
                     outputs = torch.cat([outputs, coarse_point_feats], dim=1)
             predictions = self.decoder(outputs)
-            point_labels = PointSample(targets['segmentation'].unsqueeze(1).float(), points, mode='nearest', align_corners=self.align_corners)
+            point_labels = PointSample(targets['seg_target'].unsqueeze(1).float(), points, mode='nearest', align_corners=self.align_corners)
             point_labels = point_labels.squeeze(1).long()
             targets['point_labels'] = point_labels
             predictions_aux = F.interpolate(predictions_aux, size=img_size, mode='bilinear', align_corners=self.align_corners)
             return self.calculatelosses(
                 predictions={'loss_cls': predictions, 'loss_aux': predictions_aux}, 
                 targets=targets,
-                losses_cfg=losses_cfg,
-                map_preds_to_tgts_dict={'loss_cls': 'point_labels', 'loss_aux': 'segmentation'}
+                losses_cfg=self.cfg['losses'],
+                map_preds_to_tgts_dict={'loss_cls': 'point_labels', 'loss_aux': 'seg_target'}
             )
         # if mode is TEST
         refined_seg_logits = predictions_aux.clone()
         for _ in range(self.cfg['head']['test']['subdivision_steps']):
             refined_seg_logits = F.interpolate(
                 input=refined_seg_logits, 
                 scale_factor=self.cfg['head']['test']['scale_factor'],
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/psanet/psanet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/psanet/psanet.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,82 +3,85 @@
     Implementation of PSANet
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.ops import PSAMask
+try:
+    from mmcv.ops import PSAMask
+except:
+    PSAMask = None
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''PSANet'''
 class PSANet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(PSANet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build psa
         assert head_cfg['type'] in ['collect', 'distribute', 'bi-direction']
         mask_h, mask_w = head_cfg['mask_size']
         if 'normalization_factor' not in self.cfg['head']:
             self.cfg['head']['normalization_factor'] = mask_h * mask_w
         self.reduce = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         self.attention = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Conv2d(head_cfg['feats_channels'], mask_h * mask_w, kernel_size=1, stride=1, padding=0, bias=False),
         )
         if head_cfg['type'] == 'bi-direction':
             self.reduce_p = nn.Sequential(
                 nn.Conv2d(head_cfg['in_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             )
             self.attention_p = nn.Sequential(
                 nn.Conv2d(head_cfg['feats_channels'], head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(head_cfg['feats_channels'], mask_h * mask_w, kernel_size=1, stride=1, padding=0, bias=False),
             )
             if not head_cfg['compact']:
                 self.psamask_collect = PSAMask('collect', head_cfg['mask_size'])
                 self.psamask_distribute = PSAMask('distribute', head_cfg['mask_size'])
         else:
             if not head_cfg['compact']:
                 self.psamask = PSAMask(head_cfg['type'], head_cfg['mask_size'])
         self.proj = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * (2 if head_cfg['type'] == 'bi-direction' else 1), head_cfg['in_channels'], kernel_size=1, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['in_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['in_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
         )
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['in_channels'] * 2, head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = [
             'backbone_net', 'reduce', 'attention', 'proj', 'decoder', 'auxiliary_decoder', 'reduce_p',
             'attention_p', 'psamask_collect', 'psamask_distribute', 'psamask',
         ]
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to psa
         identity = backbone_outputs[-1]
         shrink_factor, align_corners = self.cfg['head']['shrink_factor'], self.align_corners
         if self.cfg['head']['type'] in ['collect', 'distribute']:
@@ -138,12 +141,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/ppm.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/ppm.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,33 @@
     Implementation of Pyramid Pooling Module
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''PyramidPoolingModule'''
 class PyramidPoolingModule(nn.Module):
     def __init__(self, in_channels, out_channels, pool_scales, align_corners=False, norm_cfg=None, act_cfg=None):
         super(PyramidPoolingModule, self).__init__()
         self.align_corners = align_corners
         self.branches = nn.ModuleList()
         for pool_scale in pool_scales:
             self.branches.append(nn.Sequential(
                 nn.AdaptiveAvgPool2d(output_size=pool_scale),
                 nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg)
             ))
         self.bottleneck = nn.Sequential(
             nn.Conv2d(in_channels + out_channels * len(pool_scales), out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
             BuildActivation(act_cfg)
         )
         self.in_channels = in_channels
         self.out_channels = out_channels
     '''forward'''
     def forward(self, x):
         h, w = x.size(2), x.size(3)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/pspnet/pspnet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/pspnet/pspnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,26 +34,26 @@
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'ppm_net', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to pyramid pooling module
         ppm_out = self.ppm_net(backbone_outputs[-1])
         # feed to decoder
         predictions = self.decoder(ppm_out)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/segformer/segformer.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/segformer/segformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''Segformer'''
 class Segformer(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(Segformer, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build decoder
         self.convs = nn.ModuleList()
         for in_channels in head_cfg['in_channels_list']:
             self.convs.append(nn.Sequential(
                 nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * len(self.convs), head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0),
         )
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'convs', 'decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to decoder
         outs = []
         for idx, feats in enumerate(list(backbone_outputs)):
             outs.append(
@@ -50,12 +50,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/semanticfpn/semanticfpn.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/semanticfpn/semanticfpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Zhenchao Jin
 '''
 import torch
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import FPN, BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''SemanticFPN'''
 class SemanticFPN(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(SemanticFPN, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -28,15 +28,15 @@
         self.scale_heads, feature_stride_list = nn.ModuleList(), head_cfg['feature_stride_list']
         for i in range(len(feature_stride_list)):
             head_length = max(1, int(np.log2(feature_stride_list[i]) - np.log2(feature_stride_list[0])))
             scale_head = []
             for k in range(head_length):
                 scale_head.append(nn.Sequential(
                     nn.Conv2d(head_cfg['feats_channels'] if k == 0 else head_cfg['scale_head_channels'], head_cfg['scale_head_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                    BuildNormalization(constructnormcfg(placeholder=head_cfg['scale_head_channels'], norm_cfg=norm_cfg)),
+                    BuildNormalization(placeholder=head_cfg['scale_head_channels'], norm_cfg=norm_cfg),
                     BuildActivation(act_cfg),
                 ))
                 if feature_stride_list[i] != feature_stride_list[0]:
                     scale_head.append(
                         nn.Upsample(scale_factor=2, mode='bilinear', align_corners=align_corners)
                     )
             self.scale_heads.append(nn.Sequential(*scale_head))
@@ -46,15 +46,15 @@
             nn.Conv2d(head_cfg['scale_head_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'decoder', 'fpn_neck', 'scale_heads']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to fpn
         fpn_outs = self.fpn_neck(list(backbone_outputs))
         feats = self.scale_heads[0](fpn_outs[0])
         for i in range(1, len(self.cfg['head']['feature_stride_list'])):
@@ -63,12 +63,12 @@
         predictions = self.decoder(feats)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/mla.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/mla.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 Function:
     Implementation of Multi-level Feature Aggregation
 Author:
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
-from ...backbones import BuildNormalization, BuildActivation, constructnormcfg
+from ...backbones import BuildNormalization, BuildActivation
 
 
 '''MLAModule'''
 class MLAModule(nn.Module):
     def __init__(self, in_channels_list=[1024, 1024, 1024, 1024], out_channels=256, norm_cfg=None, act_cfg=None):
         super(MLAModule, self).__init__()
         self.channel_proj = nn.ModuleList()
         for i in range(len(in_channels_list)):
             self.channel_proj.append(nn.Sequential(
                 nn.Conv2d(in_channels_list[i], out_channels, kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
         self.feat_extract = nn.ModuleList()
         for i in range(len(in_channels_list)):
             self.feat_extract.append(nn.Sequential(
                 nn.Conv2d(out_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=out_channels, norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=out_channels, norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
             ))
     '''forward'''
     def forward(self, inputs):
         # feat_list -> [p2, p3, p4, p5]
         feat_list = []
         for x, conv in zip(inputs, self.channel_proj):
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/setr/setr.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/setr/setr.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     Zhenchao Jin
 '''
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from .mla import MLANeck
 from ..base import BaseSegmentor
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''Naive upsampling head and Progressive upsampling head of SETR'''
 class SETRUP(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(SETRUP, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build norm layer
         self.norm_layers = nn.ModuleList()
         for in_channels in head_cfg['in_channels_list']:
             norm_cfg_copy = head_cfg['norm_cfg'].copy()
-            norm_layer = BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg_copy))
+            norm_layer = BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg_copy)
             self.norm_layers.append(norm_layer)
         # build decoder
         self.decoder = self.builddecoder({
             'in_channels': head_cfg['in_channels_list'][-1],
             'out_channels': head_cfg['feats_channels'],
             'kernel_size': head_cfg['kernel_size'],
             'scale_factor': head_cfg['scale_factor'],
@@ -40,15 +40,15 @@
             decoder = self.builddecoder(auxiliary_cfg)
             self.auxiliary_decoders.append(decoder)
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'decoder', 'norm_layers', 'auxiliary_decoders']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to norm layer
         assert len(backbone_outputs) == len(self.norm_layers)
         for idx in range(len(backbone_outputs)):
             backbone_outputs[idx] = self.norm(backbone_outputs[idx], self.norm_layers[idx])
@@ -62,15 +62,15 @@
             for idx, (out, dec) in enumerate(zip(backbone_outputs, self.auxiliary_decoders)):
                 predictions_aux = dec(out)
                 predictions_aux = F.interpolate(predictions_aux, size=img_size, mode='bilinear', align_corners=self.align_corners)
                 outputs_dict[f'loss_aux{idx+1}'] = predictions_aux
             return self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return predictions
     '''norm layer'''
     def norm(self, x, norm_layer):
         n, c, h, w = x.shape
         x = x.reshape(n, c, h * w).transpose(2, 1).contiguous()
         x = norm_layer(x)
@@ -80,15 +80,15 @@
     def builddecoder(self, decoder_cfg):
         layers, norm_cfg, act_cfg, num_classes, align_corners, kernel_size = [], self.norm_cfg.copy(), self.act_cfg.copy(), self.cfg['num_classes'], self.align_corners, decoder_cfg['kernel_size']
         for idx in range(decoder_cfg['num_convs']):
             if idx == 0:
                 layers.append(nn.Conv2d(decoder_cfg['in_channels'], decoder_cfg['out_channels'], kernel_size=kernel_size, stride=1, padding=int(kernel_size - 1) // 2, bias=False))
             else:
                 layers.append(nn.Conv2d(decoder_cfg['out_channels'], decoder_cfg['out_channels'], kernel_size=kernel_size, stride=1, padding=int(kernel_size - 1) // 2, bias=False))
-            layers.append(BuildNormalization(constructnormcfg(placeholder=decoder_cfg['out_channels'], norm_cfg=norm_cfg)))
+            layers.append(BuildNormalization(placeholder=decoder_cfg['out_channels'], norm_cfg=norm_cfg))
             layers.append(BuildActivation(act_cfg))
             layers.append(nn.Upsample(scale_factor=decoder_cfg['scale_factor'], mode='bilinear', align_corners=align_corners))
         layers.append(nn.Dropout2d(decoder_cfg['dropout']))
         layers.append(nn.Conv2d(decoder_cfg['out_channels'], num_classes, kernel_size=1, stride=1, padding=0))
         return nn.Sequential(*layers)
 
 
@@ -97,33 +97,33 @@
     def __init__(self, cfg, mode):
         super(SETRMLA, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
         # build mla neck
         norm_layers = nn.ModuleList()
         for in_channels in head_cfg['in_channels_list']:
             norm_cfg_copy = head_cfg['norm_cfg'].copy()
-            norm_layer = BuildNormalization(constructnormcfg(placeholder=in_channels, norm_cfg=norm_cfg_copy))
+            norm_layer = BuildNormalization(placeholder=in_channels, norm_cfg=norm_cfg_copy)
             norm_layers.append(norm_layer)
         self.mla_neck = MLANeck(
             in_channels_list=head_cfg['in_channels_list'], 
             out_channels=head_cfg['mla_feats_channels'], 
             norm_layers=norm_layers, 
             norm_cfg=norm_cfg, 
             act_cfg=act_cfg,
         )
         # build upsample convs and decoder
         assert head_cfg['mla_up_channels'] * len(head_cfg['in_channels_list']) == head_cfg['feats_channels']
         self.up_convs = nn.ModuleList()
         for i in range(len(head_cfg['in_channels_list'])):
             self.up_convs.append(nn.Sequential(
                 nn.Conv2d(head_cfg['mla_feats_channels'], head_cfg['mla_up_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['mla_up_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['mla_up_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Conv2d(head_cfg['mla_up_channels'], head_cfg['mla_up_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['mla_up_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['mla_up_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg),
                 nn.Upsample(scale_factor=head_cfg['scale_factor'], mode='bilinear', align_corners=align_corners)
             ))
         self.decoder = nn.Sequential(
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0),
         )
@@ -135,15 +135,15 @@
             decoder = self.builddecoder(auxiliary_cfg)
             self.auxiliary_decoders.append(decoder)
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'decoder', 'mla_neck', 'auxiliary_decoders', 'up_convs']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to mla neck
         feats_list = self.mla_neck(list(backbone_outputs))
         # feed to decoder
         outputs = []
@@ -160,24 +160,24 @@
             for idx, (out, dec) in enumerate(zip(feats_list, self.auxiliary_decoders)):
                 predictions_aux = dec(out)
                 predictions_aux = F.interpolate(predictions_aux, size=img_size, mode='bilinear', align_corners=self.align_corners)
                 outputs_dict[f'loss_aux{idx+1}'] = predictions_aux
             return self.calculatelosses(
                 predictions=outputs_dict, 
                 targets=targets, 
-                losses_cfg=losses_cfg
+                losses_cfg=self.cfg['losses']
             )
         return predictions
     '''build decoder'''
     def builddecoder(self, decoder_cfg):
         layers, norm_cfg, act_cfg, num_classes, align_corners, kernel_size = [], self.norm_cfg.copy(), self.act_cfg.copy(), self.cfg['num_classes'], self.align_corners, decoder_cfg['kernel_size']
         for idx in range(decoder_cfg['num_convs']):
             if idx == 0:
                 layers.append(nn.Conv2d(decoder_cfg['in_channels'], decoder_cfg['out_channels'], kernel_size=kernel_size, stride=1, padding=int(kernel_size - 1) // 2, bias=False))
             else:
                 layers.append(nn.Conv2d(decoder_cfg['out_channels'], decoder_cfg['out_channels'], kernel_size=kernel_size, stride=1, padding=int(kernel_size - 1) // 2, bias=False))
-            layers.append(BuildNormalization(constructnormcfg(placeholder=decoder_cfg['out_channels'], norm_cfg=norm_cfg)))
+            layers.append(BuildNormalization(placeholder=decoder_cfg['out_channels'], norm_cfg=norm_cfg))
             layers.append(BuildActivation(act_cfg))
             layers.append(nn.Upsample(scale_factor=decoder_cfg['scale_factor'], mode='bilinear', align_corners=align_corners))
         layers.append(nn.Dropout2d(decoder_cfg['dropout']))
         layers.append(nn.Conv2d(decoder_cfg['out_channels'], num_classes, kernel_size=1, stride=1, padding=0))
         return nn.Sequential(*layers)
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/models/segmentors/upernet/upernet.py` & `SSSegmentation-1.3.0/ssseg/modules/models/segmentors/upernet/upernet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 import copy
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import BaseSegmentor
 from ..pspnet import PyramidPoolingModule
-from ...backbones import BuildActivation, BuildNormalization, constructnormcfg
+from ...backbones import BuildActivation, BuildNormalization
 
 
 '''UPerNet'''
 class UPerNet(BaseSegmentor):
     def __init__(self, cfg, mode):
         super(UPerNet, self).__init__(cfg, mode)
         align_corners, norm_cfg, act_cfg, head_cfg = self.align_corners, self.norm_cfg, self.act_cfg, cfg['head']
@@ -36,41 +36,41 @@
         # build lateral convs
         act_cfg_copy = copy.deepcopy(act_cfg)
         if 'inplace' in act_cfg_copy: act_cfg_copy['inplace'] = False
         self.lateral_convs = nn.ModuleList()
         for in_channels in head_cfg['in_channels_list'][:-1]:
             self.lateral_convs.append(nn.Sequential(
                 nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=1, stride=1, padding=0, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg_copy),
             ))
         # build fpn convs
         self.fpn_convs = nn.ModuleList()
         for in_channels in [head_cfg['feats_channels'],] * len(self.lateral_convs):
             self.fpn_convs.append(nn.Sequential(
                 nn.Conv2d(in_channels, head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-                BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+                BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
                 BuildActivation(act_cfg_copy),
             ))
         # build decoder
         self.decoder = nn.Sequential(
             nn.Conv2d(head_cfg['feats_channels'] * len(head_cfg['in_channels_list']), head_cfg['feats_channels'], kernel_size=3, stride=1, padding=1, bias=False),
-            BuildNormalization(constructnormcfg(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg)),
+            BuildNormalization(placeholder=head_cfg['feats_channels'], norm_cfg=norm_cfg),
             BuildActivation(act_cfg),
             nn.Dropout2d(head_cfg['dropout']),
             nn.Conv2d(head_cfg['feats_channels'], cfg['num_classes'], kernel_size=1, stride=1, padding=0)
         )
         # build auxiliary decoder
         self.setauxiliarydecoder(cfg['auxiliary'])
         # freeze normalization layer if necessary
         if cfg.get('is_freeze_norm', False): self.freezenormalization()
         # layer names for training tricks
         self.layer_names = ['backbone_net', 'ppm_net', 'lateral_convs', 'feats_to_pyramid_net', 'decoder', 'auxiliary_decoder']
     '''forward'''
-    def forward(self, x, targets=None, losses_cfg=None):
+    def forward(self, x, targets=None):
         img_size = x.size(2), x.size(3)
         # feed to backbone network
         backbone_outputs = self.transforminputs(self.backbone_net(x), selected_indices=self.cfg['backbone'].get('selected_indices'))
         # feed to feats_to_pyramid_net
         if hasattr(self, 'feats_to_pyramid_net'): backbone_outputs = self.feats_to_pyramid_net(backbone_outputs)
         # feed to pyramid pooling module
         ppm_out = self.ppm_net(backbone_outputs[-1])
@@ -89,12 +89,12 @@
         predictions = self.decoder(fpn_out)
         # forward according to the mode
         if self.mode == 'TRAIN':
             loss, losses_log_dict = self.forwardtrain(
                 predictions=predictions,
                 targets=targets,
                 backbone_outputs=backbone_outputs,
-                losses_cfg=losses_cfg,
+                losses_cfg=self.cfg['losses'],
                 img_size=img_size,
             )
             return loss, losses_log_dict
         return predictions
```

### Comparing `sssegmentation-1.2.0/ssseg/modules/utils/palette.py` & `SSSegmentation-1.3.0/ssseg/modules/datasets/ade20k.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,67 @@
 '''
 Function:
-    Color map for visualizing the segmentation mask
+    Implementation of ADE20kDataset
 Author:
     Zhenchao Jin
 '''
 import os
+import pandas as pd
+from .base import BaseDataset
 
 
-'''lip palette'''
-lip_palette = [
-    (0, 0, 0), (128, 0, 0), (255, 0, 0), (0, 85, 0), (170, 0, 51), (255, 85, 0), (0, 0, 85),
-    (0, 119, 221), (85, 85, 0), (0, 85, 85), (85, 51, 0), (52, 86, 128), (0, 128, 0), (0, 0, 255), 
-    (51, 170, 221), (0, 255, 255), (85, 255, 170), (170, 255, 85), (255, 255, 0), (255, 170, 0)
-]
-assert len(lip_palette) == 20
-
-
-'''cihp palette'''
-cihp_palette = [
-    (0, 0, 0), (128, 0, 0), (255, 0, 0), (0, 85, 0), (170, 0, 51), (255, 85, 0), (0, 0, 85),
-    (0, 119, 221), (85, 85, 0), (0, 85, 85), (85, 51, 0), (52, 86, 128), (0, 128, 0), (0, 0, 255), 
-    (51, 170, 221), (0, 255, 255), (85, 255, 170), (170, 255, 85), (255, 255, 0), (255, 170, 0)
-]
-assert len(cihp_palette) == 20
-
-
-'''pascal context palette'''
-pascalcontext_palette = [
-    (120, 120, 120), (180, 120, 120), (6, 230, 230), (80, 50, 50), (4, 200, 3), (120, 120, 80), (140, 140, 140), (204, 5, 255),
-    (230, 230, 230), (4, 250, 7), (224, 5, 255), (235, 255, 7), (150, 5, 61), (120, 120, 70), (8, 255, 51), (255, 6, 82),
-    (143, 255, 140), (204, 255, 4), (255, 51, 7), (204, 70, 3), (0, 102, 200), (61, 230, 250), (255, 6, 51), (11, 102, 255),
-    (255, 7, 71), (255, 9, 224), (9, 7, 230), (220, 220, 220), (255, 9, 92), (112, 9, 255), (8, 255, 214), (7, 255, 224),
-    (255, 184, 6), (10, 255, 71), (255, 41, 10), (7, 255, 255), (224, 255, 8), (102, 8, 255), (255, 61, 6), (255, 194, 7),
-    (255, 122, 8), (0, 255, 20), (255, 8, 41), (255, 5, 153), (6, 51, 255), (235, 12, 255), (160, 150, 20), (0, 163, 255),
-    (140, 140, 140), (250, 10, 15), (20, 255, 0), (31, 255, 0), (255, 31, 0), (255, 224, 0), (153, 255, 0), (0, 0, 255),
-    (255, 71, 0), (0, 235, 255), (0, 173, 255), (31, 0, 255)
-]
-assert len(pascalcontext_palette) == 60
-
-
-'''pascal context 59 palette'''
-pascalcontext59_palette = [
-    (180, 120, 120), (6, 230, 230), (80, 50, 50), (4, 200, 3), (120, 120, 80), (140, 140, 140), (204, 5, 255),
-    (230, 230, 230), (4, 250, 7), (224, 5, 255), (235, 255, 7), (150, 5, 61), (120, 120, 70), (8, 255, 51), (255, 6, 82),
-    (143, 255, 140), (204, 255, 4), (255, 51, 7), (204, 70, 3), (0, 102, 200), (61, 230, 250), (255, 6, 51), (11, 102, 255),
-    (255, 7, 71), (255, 9, 224), (9, 7, 230), (220, 220, 220), (255, 9, 92), (112, 9, 255), (8, 255, 214), (7, 255, 224),
-    (255, 184, 6), (10, 255, 71), (255, 41, 10), (7, 255, 255), (224, 255, 8), (102, 8, 255), (255, 61, 6), (255, 194, 7),
-    (255, 122, 8), (0, 255, 20), (255, 8, 41), (255, 5, 153), (6, 51, 255), (235, 12, 255), (160, 150, 20), (0, 163, 255),
-    (140, 140, 140), (250, 10, 15), (20, 255, 0), (31, 255, 0), (255, 31, 0), (255, 224, 0), (153, 255, 0), (0, 0, 255),
-    (255, 71, 0), (0, 235, 255), (0, 173, 255), (31, 0, 255)
-]
-assert len(pascalcontext59_palette) == 59
-
-
-'''voc palette'''
-voc_palette = [
-    (0, 0, 0), (128, 0, 0), (0, 128, 0), (128, 128, 0), (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128), (64, 0, 0),
-    (192, 0, 0), (64, 128, 0), (192, 128, 0), (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128), (0, 64, 0),
-    (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)
-]
-assert len(voc_palette) == 21
-
-
-'''ade20k palette'''
-ade20k_palette = [
-    (120, 120, 120), (180, 120, 120), (6, 230, 230), (80, 50, 50), (4, 200, 3), (120, 120, 80), (140, 140, 140), (204, 5, 255), (230, 230, 230), (4, 250, 7), (224, 5, 255),
-    (235, 255, 7), (150, 5, 61), (120, 120, 70), (8, 255, 51), (255, 6, 82), (143, 255, 140), (204, 255, 4), (255, 51, 7), (204, 70, 3), (0, 102, 200), (61, 230, 250),
-    (255, 6, 51), (11, 102, 255), (255, 7, 71), (255, 9, 224), (9, 7, 230), (220, 220, 220), (255, 9, 92), (112, 9, 255), (8, 255, 214), (7, 255, 224), (255, 184, 6),
-    (10, 255, 71), (255, 41, 10), (7, 255, 255), (224, 255, 8), (102, 8, 255), (255, 61, 6), (255, 194, 7), (255, 122, 8), (0, 255, 20), (255, 8, 41), (255, 5, 153),
-    (6, 51, 255), (235, 12, 255), (160, 150, 20), (0, 163, 255), (140, 140, 140), (250,  10,  15), (20, 255, 0), (31, 255, 0), (255, 31, 0), (255, 224, 0), (153, 255, 0),
-    (0, 0, 255), (255, 71, 0), (0, 235, 255), (0, 173, 255), (31, 0, 255), (11, 200, 200), (255, 82, 0), (0, 255, 245), (0,  61, 255), (0, 255, 112), (0, 255, 133),
-    (255, 0, 0), (255, 163, 0), (255, 102, 0), (194, 255, 0), (0, 143, 255), (51, 255, 0), (0, 82, 255), (0, 255, 41), (0, 255, 173), (10, 0, 255), (173, 255, 0),
-    (0, 255, 153), (255, 92, 0), (255, 0, 255), (255, 0, 245), (255, 0, 102), (255, 173, 0), (255, 0, 20), (255, 184, 184), (0, 31, 255), (0, 255, 61), (0, 71, 255),
-    (255, 0, 204), (0, 255, 194), (0, 255, 82), (0, 10, 255), (0, 112, 255), (51, 0, 255), (0, 194, 255), (0, 122, 255), (0, 255, 163), (255, 153, 0), (0, 255, 10),
-    (255, 112, 0), (143, 255, 0), (82, 0, 255), (163, 255, 0), (255, 235, 0), (8, 184, 170), (133, 0, 255), (0, 255, 92), (184, 0, 255), (255, 0, 31), (0, 184, 255),
-    (0, 214, 255), (255, 0, 112), (92, 255, 0), (0, 224, 255), (112, 224, 255), (70, 184, 160), (163, 0, 255), (153, 0, 255), (71, 255, 0), (255, 0, 163), (255, 204, 0),
-    (255, 0, 143), (0, 255, 235), (133, 255, 0), (255, 0, 235), (245, 0, 255), (255, 0, 122), (255, 245, 0), (10, 190, 212), (214, 255, 0), (0, 204, 255), (20, 0, 255),
-    (255, 255, 0), (0, 153, 255), (0, 41, 255), (0, 255, 204), (41, 0, 255), (41, 255, 0), (173, 0, 255), (0, 245, 255), (71, 0, 255), (122, 0, 255), (0, 255, 184),
-    (0, 92, 255), (184, 255, 0), (0, 133, 255), (255, 214, 0), (25, 194, 194), (102, 255, 0), (92, 0, 255)
-]
-assert len(ade20k_palette) == 150
-
-
-'''cityscapes'''
-cityscapes_palette = [
-    (128, 64, 128), (244, 35, 232), (70, 70, 70), (102, 102, 156), (190, 153, 153), (153, 153, 153), (250, 170, 30), (220, 220, 0),
-    (107, 142, 35), (152, 251, 152), (70, 130, 180), (220, 20, 60), (255, 0, 0), (0, 0, 142), (0, 0, 70), (0, 60, 100),
-    (0, 80, 100), (0, 0, 230), (119, 11, 32)
-]
-assert len(cityscapes_palette) == 19
-
-
-'''sbushadow'''
-sbushadow_palette = [(0, 0, 0), (255, 0, 0)]
-assert len(sbushadow_palette) == 2
-
-
-'''supervisely'''
-supervisely_palette = [(0, 0, 0), (255, 0, 0)]
-assert len(supervisely_palette) == 2
-
-
-'''collect the suppoted palettes'''
-supported_palettes = {
-    'voc': voc_palette,
-    'lip': lip_palette,
-    'cihp': cihp_palette,
-    'ade20k': ade20k_palette,
-    'sbushadow': sbushadow_palette,
-    'cityscapes': cityscapes_palette,
-    'supervisely': supervisely_palette,
-    'pascalcontext': pascalcontext_palette,
-    'pascalcontext59': pascalcontext59_palette,
-}
-
-
-'''GeneratePalette'''
-def GeneratePalette(num_classes):
-    palette = [0] * (num_classes * 3)
-    for j in range(0, num_classes):
-        lab = j
-        palette[j * 3 + 0] = 0
-        palette[j * 3 + 1] = 0
-        palette[j * 3 + 2] = 0
-        i = 0
-        while lab:
-            palette[j * 3 + 0] |= (((lab >> 0) & 1) << (7 - i))
-            palette[j * 3 + 1] |= (((lab >> 1) & 1) << (7 - i))
-            palette[j * 3 + 2] |= (((lab >> 2) & 1) << (7 - i))
-            i += 1
-            lab >>= 3
-    import numpy as np
-    palette = np.array(palette).reshape(-1, 3)
-    palette = palette.tolist()
-    return palette
-
-
-'''BuildPalette'''
-def BuildPalette(dataset_type, num_classes=2, logger_handle=None):
-    if dataset_type not in supported_palettes:
-        logger_handle.warning('Unsupport dataset type %s, try to generate the palette according to the number of classes' % dataset_type)
-        return GeneratePalette(num_classes)
-    return supported_palettes[dataset_type]
+'''ADE20kDataset'''
+class ADE20kDataset(BaseDataset):
+    num_classes = 150
+    classnames = [
+        'wall', 'building, edifice', 'sky', 'floor, flooring', 'tree', 'ceiling', 'road, route', 'bed', 'windowpane, window', 'grass',
+        'cabinet', 'sidewalk, pavement', 'person, individual, someone, somebody, mortal, soul', 'earth, ground', 'door, double door', 'table', 'mountain, mount',
+        'plant, flora, plant life', 'curtain, drape, drapery, mantle, pall', 'chair', 'car, auto, automobile, machine, motorcar', 'water', 'painting, picture', 
+        'sofa, couch, lounge', 'shelf', 'house', 'sea', 'mirror', 'rug, carpet, carpeting', 'field', 'armchair', 'seat', 'fence, fencing', 'desk', 'rock, stone', 
+        'wardrobe, closet, press', 'lamp', 'bathtub, bathing tub, bath, tub', 'railing, rail', 'cushion', 'base, pedestal, stand', 'box', 'column, pillar', 'signboard, sign',
+        'chest of drawers, chest, bureau, dresser', 'counter', 'sand', 'sink', 'skyscraper', 'fireplace, hearth, open fireplace', 'refrigerator, icebox',
+        'grandstand, covered stand', 'path', 'stairs, steps', 'runway', 'case, display case, showcase, vitrine', 'pool table, billiard table, snooker table', 'pillow',
+        'screen door, screen', 'stairway, staircase', 'river', 'bridge, span', 'bookcase', 'blind, screen', 'coffee table, cocktail table', 'toilet, can, commode, crapper, pot, potty, stool, throne',
+        'flower', 'book', 'hill', 'bench', 'countertop', 'stove, kitchen stove, range, kitchen range, cooking stove', 'palm, palm tree', 'kitchen island',
+        'computer, computing machine, computing device, data processor, electronic computer, information processing system', 'swivel chair', 'boat', 'bar', 'arcade machine',
+        'hovel, hut, hutch, shack, shanty', 'bus, autobus, coach, charabanc, double-decker, jitney, motorbus, motorcoach, omnibus, passenger vehicle',
+        'towel', 'light, light source', 'truck, motortruck', 'tower', 'chandelier, pendant, pendent', 'awning, sunshade, sunblind', 'streetlight, street lamp', 'booth, cubicle, stall, kiosk',
+        'television receiver, television, television set, tv, tv set, idiot box, boob tube, telly, goggle box', 'airplane, aeroplane, plane', 'dirt track',
+        'apparel, wearing apparel, dress, clothes', 'pole', 'land, ground, soil', 'bannister, banister, balustrade, balusters, handrail', 'escalator, moving staircase, moving stairway',
+        'ottoman, pouf, pouffe, puff, hassock', 'bottle', 'buffet, counter, sideboard', 'poster, posting, placard, notice, bill, card', 'stage', 'van', 'ship', 'fountain',
+        'conveyer belt, conveyor belt, conveyer, conveyor, transporter', 'canopy', 'washer, automatic washer, washing machine', 'plaything, toy', 'swimming pool, swimming bath, natatorium',
+        'stool', 'barrel, cask', 'basket, handbasket', 'waterfall, falls', 'tent, collapsible shelter', 'bag', 'minibike, motorbike', 'cradle', 'oven', 'ball', 'food, solid food', 'step, stair', 'tank, storage tank',
+        'trade name, brand name, brand, marque', 'microwave, microwave oven', 'pot, flowerpot', 'animal, animate being, beast, brute, creature, fauna', 'bicycle, bike, wheel, cycle', 'lake',
+        'dishwasher, dish washer, dishwashing machine', 'screen, silver screen, projection screen', 'blanket, cover', 'sculpture', 'hood, exhaust hood', 'sconce', 'vase',
+        'traffic light, traffic signal, stoplight', 'tray', 'ashcan, trash can, garbage can, wastebin, ash bin, ash-bin, ashbin, dustbin, trash barrel, trash bin',
+        'fan', 'pier, wharf, wharfage, dock', 'crt screen', 'plate', 'monitor, monitoring device', 'bulletin board, notice board', 'shower', 'radiator', 'glass, drinking glass', 'clock', 'flag'
+    ]
+    palette = [
+        (120, 120, 120), (180, 120, 120), (6, 230, 230), (80, 50, 50), (4, 200, 3), (120, 120, 80), (140, 140, 140), (204, 5, 255), (230, 230, 230), (4, 250, 7), (224, 5, 255),
+        (235, 255, 7), (150, 5, 61), (120, 120, 70), (8, 255, 51), (255, 6, 82), (143, 255, 140), (204, 255, 4), (255, 51, 7), (204, 70, 3), (0, 102, 200), (61, 230, 250),
+        (255, 6, 51), (11, 102, 255), (255, 7, 71), (255, 9, 224), (9, 7, 230), (220, 220, 220), (255, 9, 92), (112, 9, 255), (8, 255, 214), (7, 255, 224), (255, 184, 6),
+        (10, 255, 71), (255, 41, 10), (7, 255, 255), (224, 255, 8), (102, 8, 255), (255, 61, 6), (255, 194, 7), (255, 122, 8), (0, 255, 20), (255, 8, 41), (255, 5, 153),
+        (6, 51, 255), (235, 12, 255), (160, 150, 20), (0, 163, 255), (140, 140, 140), (250,  10,  15), (20, 255, 0), (31, 255, 0), (255, 31, 0), (255, 224, 0), (153, 255, 0),
+        (0, 0, 255), (255, 71, 0), (0, 235, 255), (0, 173, 255), (31, 0, 255), (11, 200, 200), (255, 82, 0), (0, 255, 245), (0,  61, 255), (0, 255, 112), (0, 255, 133),
+        (255, 0, 0), (255, 163, 0), (255, 102, 0), (194, 255, 0), (0, 143, 255), (51, 255, 0), (0, 82, 255), (0, 255, 41), (0, 255, 173), (10, 0, 255), (173, 255, 0),
+        (0, 255, 153), (255, 92, 0), (255, 0, 255), (255, 0, 245), (255, 0, 102), (255, 173, 0), (255, 0, 20), (255, 184, 184), (0, 31, 255), (0, 255, 61), (0, 71, 255),
+        (255, 0, 204), (0, 255, 194), (0, 255, 82), (0, 10, 255), (0, 112, 255), (51, 0, 255), (0, 194, 255), (0, 122, 255), (0, 255, 163), (255, 153, 0), (0, 255, 10),
+        (255, 112, 0), (143, 255, 0), (82, 0, 255), (163, 255, 0), (255, 235, 0), (8, 184, 170), (133, 0, 255), (0, 255, 92), (184, 0, 255), (255, 0, 31), (0, 184, 255),
+        (0, 214, 255), (255, 0, 112), (92, 255, 0), (0, 224, 255), (112, 224, 255), (70, 184, 160), (163, 0, 255), (153, 0, 255), (71, 255, 0), (255, 0, 163), (255, 204, 0),
+        (255, 0, 143), (0, 255, 235), (133, 255, 0), (255, 0, 235), (245, 0, 255), (255, 0, 122), (255, 245, 0), (10, 190, 212), (214, 255, 0), (0, 204, 255), (20, 0, 255),
+        (255, 255, 0), (0, 153, 255), (0, 41, 255), (0, 255, 204), (41, 0, 255), (41, 255, 0), (173, 0, 255), (0, 245, 255), (71, 0, 255), (122, 0, 255), (0, 255, 184),
+        (0, 92, 255), (184, 255, 0), (0, 133, 255), (255, 214, 0), (25, 194, 194), (102, 255, 0), (92, 0, 255)
+    ]
+    clsid2label = {0: 255}
+    for i in range(1, num_classes+1): clsid2label[i] = i - 1
+    assert num_classes == len(classnames) and num_classes == len(palette)
+    def __init__(self, mode, logger_handle, dataset_cfg):
+        super(ADE20kDataset, self).__init__(mode=mode, logger_handle=logger_handle, dataset_cfg=dataset_cfg)
+        # obtain the dirs
+        rootdir = dataset_cfg['rootdir']
+        setmap_dict = {'train': 'training', 'val': 'validation', 'test': 'testing'}
+        self.image_dir = os.path.join(rootdir, 'ADEChallengeData2016/images', setmap_dict[dataset_cfg['set']])
+        self.ann_dir = os.path.join(rootdir, 'ADEChallengeData2016/annotations', setmap_dict[dataset_cfg['set']])
+        # obatin imageids
+        df = pd.read_csv(os.path.join(rootdir, 'ADEChallengeData2016', dataset_cfg['set']+'.txt'), names=['imageids'])
+        self.imageids = df['imageids'].values
+        self.imageids = [str(_id) for _id in self.imageids]
```

### Comparing `sssegmentation-1.2.0/ssseg/test.py` & `SSSegmentation-1.3.0/ssseg/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Test the segmentor
+    Implementation of Tester
 Author:
     Zhenchao Jin
 '''
 import os
 import cv2
 import copy
 import torch
@@ -14,96 +14,92 @@
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from tqdm import tqdm
 from configs import BuildConfig
 from modules import (
-    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildOptimizer, BuildScheduler, initslurm,
-    BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, Logger, setRandomSeed, BuildPalette, checkdir, loadcheckpoints, savecheckpoints
+    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, 
+    Logger, initslurm, setrandomseed, touchdir, loadckpts, saveckpts, BuildOptimizer, BuildScheduler
 )
 warnings.filterwarnings('ignore')
 
 
 '''parse arguments in command line'''
 def parseArgs():
     parser = argparse.ArgumentParser(description='SSSegmentation is an open source supervised semantic segmentation toolbox based on PyTorch')
     parser.add_argument('--local_rank', dest='local_rank', help='node rank for distributed testing', default=0, type=int)
     parser.add_argument('--nproc_per_node', dest='nproc_per_node', help='number of process per node', default=8, type=int)
     parser.add_argument('--cfgfilepath', dest='cfgfilepath', help='config file path you want to use', type=str, required=True)
     parser.add_argument('--evalmode', dest='evalmode', help='evaluate mode, support online and offline', default='offline', type=str)
-    parser.add_argument('--checkpointspath', dest='checkpointspath', help='checkpoints you want to resume from', type=str, required=True)
+    parser.add_argument('--ckptspath', dest='ckptspath', help='checkpoints you want to resume from', type=str, required=True)
+    parser.add_argument('--slurm', dest='slurm', help='please add --slurm if you are using slurm', default=False, action='store_true')
     args = parser.parse_args()
-    initslurm(args, '28000')
+    if args.slurm: initslurm(args, '28000')
     return args
 
 
 '''Tester'''
 class Tester():
     def __init__(self, cfg, ngpus_per_node, logger_handle, cmd_args, cfg_file_path):
         # set attribute
         self.cfg = cfg
         self.ngpus_per_node = ngpus_per_node
         self.logger_handle = logger_handle
         self.cmd_args = cmd_args
         self.cfg_file_path = cfg_file_path
         assert torch.cuda.is_available(), 'cuda is not available'
         # init distributed training
-        self.cfg.DATALOADER_CFG['test']['batch_size'] = self.cmd_args.nproc_per_node
         dist.init_process_group(backend=self.cfg.SEGMENTOR_CFG.get('backend', 'nccl'))
+        # open full fp32
+        torch.backends.cuda.matmul.allow_tf32 = False
+        torch.backends.cudnn.allow_tf32 = False
     '''start tester'''
     def start(self, all_preds, all_gts):
         cfg, ngpus_per_node, logger_handle, cmd_args, cfg_file_path = self.cfg, self.ngpus_per_node, self.logger_handle, self.cmd_args, self.cfg_file_path
         rank_id = int(os.environ['SLURM_PROCID']) if 'SLURM_PROCID' in os.environ else cmd_args.local_rank
         # build dataset and dataloader
-        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=copy.deepcopy(cfg.DATASET_CFG))
+        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=cfg.SEGMENTOR_CFG['dataset'])
         assert dataset.num_classes == cfg.SEGMENTOR_CFG['num_classes'], 'parsed config file %s error' % cfg_file_path
-        dataloader_cfg = copy.deepcopy(cfg.DATALOADER_CFG)
-        batch_size, num_workers = dataloader_cfg['test']['batch_size'], dataloader_cfg['test']['num_workers']
-        batch_size_per_node = batch_size // ngpus_per_node
-        num_workers_per_node = num_workers // ngpus_per_node
-        dataloader_cfg['test'].update({'batch_size': batch_size_per_node, 'num_workers': num_workers_per_node})
+        dataloader_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['dataloader'])
+        expected_total_train_bs_for_assert = dataloader_cfg.pop('expected_total_train_bs_for_assert')
+        dataloader_cfg['train']['batch_size'], dataloader_cfg['train']['num_workers'] = dataloader_cfg['train'].pop('batch_size_per_gpu'), dataloader_cfg['train'].pop('num_workers_per_gpu')
+        dataloader_cfg['test']['batch_size'], dataloader_cfg['test']['num_workers'] = dataloader_cfg['test'].pop('batch_size_per_gpu'), dataloader_cfg['test'].pop('num_workers_per_gpu')
+        assert expected_total_train_bs_for_assert == dataloader_cfg['train']['batch_size'] * ngpus_per_node
         dataloader = BuildDistributedDataloader(dataset=dataset, dataloader_cfg=dataloader_cfg['test'])
         # build segmentor
         cfg.SEGMENTOR_CFG['backbone']['pretrained'] = False
         segmentor = BuildSegmentor(segmentor_cfg=copy.deepcopy(cfg.SEGMENTOR_CFG), mode='TEST')
         torch.cuda.set_device(cmd_args.local_rank)
         segmentor.cuda(cmd_args.local_rank)
-        # load checkpoints
-        checkpoints = loadcheckpoints(cmd_args.checkpointspath, logger_handle=logger_handle, cmd_args=cmd_args)
+        # load ckpts
+        ckpts = loadckpts(cmd_args.ckptspath)
         try:
-            segmentor.load_state_dict(checkpoints['model'])
+            segmentor.load_state_dict(ckpts['model'])
         except Exception as e:
-            logger_handle.warning(str(e) + '\n' + 'Try to load checkpoints by using strict=False')
-            segmentor.load_state_dict(checkpoints['model'], strict=False)
+            logger_handle.warning(str(e) + '\n' + 'Try to load ckpts by using strict=False')
+            segmentor.load_state_dict(ckpts['model'], strict=False)
         # parallel
         segmentor = BuildDistributedModel(segmentor, {'device_ids': [cmd_args.local_rank]})
         # print information
         if (cmd_args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
             logger_handle.info(f'Config file path: {cfg_file_path}')
-            logger_handle.info(f'DATASET_CFG: \n{cfg.DATASET_CFG}')
-            logger_handle.info(f'DATALOADER_CFG: \n{cfg.DATALOADER_CFG}')
-            logger_handle.info(f'OPTIMIZER_CFG: \n{cfg.OPTIMIZER_CFG}')
-            logger_handle.info(f'SCHEDULER_CFG: \n{cfg.SCHEDULER_CFG}')
-            logger_handle.info(f'LOSSES_CFG: \n{cfg.LOSSES_CFG}')
-            logger_handle.info(f'SEGMENTOR_CFG: \n{cfg.SEGMENTOR_CFG}')
-            logger_handle.info(f'INFERENCE_CFG: \n{cfg.INFERENCE_CFG}')
-            logger_handle.info(f'COMMON_CFG: \n{cfg.COMMON_CFG}')
-            logger_handle.info(f'Resume from: {cmd_args.checkpointspath}')
+            logger_handle.info(f'Config details: \n{cfg.SEGMENTOR_CFG}')
+            logger_handle.info(f'Resume from: {cmd_args.ckptspath}')
         # set eval
         segmentor.eval()
         # start to test
         FloatTensor = torch.cuda.FloatTensor
-        inference_cfg = copy.deepcopy(cfg.INFERENCE_CFG)
+        inference_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['inference'])
         with torch.no_grad():
             dataloader.sampler.set_epoch(0)
             pbar = tqdm(enumerate(dataloader))
-            for batch_idx, samples in pbar:
+            for batch_idx, samples_meta in pbar:
                 pbar.set_description('Processing %s/%s in rank %s' % (batch_idx+1, len(dataloader), rank_id))
-                imageids, images, widths, heights, gts = samples['id'], samples['image'], samples['width'], samples['height'], samples['groundtruth']
+                imageids, images, widths, heights, gts = samples_meta['id'], samples_meta['image'], samples_meta['width'], samples_meta['height'], samples_meta['seg_target']
                 infer_tricks, align_corners = inference_cfg['tricks'], segmentor.module.align_corners
                 cascade_cfg = infer_tricks.get('cascade', {'key_for_pre_output': 'memory_gather_logits', 'times': 1, 'forward_default_args': None})
                 for idx in range(cascade_cfg['times']):
                     forward_args = None
                     if idx > 0: 
                         outputs_list = [
                             F.interpolate(outputs, size=outputs_list[-1].shape[2:], mode='bilinear', align_corners=align_corners) for outputs in outputs_list
@@ -148,22 +144,22 @@
                 outputs_flip = self.inference(
                     segmentor=segmentor, 
                     images=images_flip.type(FloatTensor), 
                     inference_cfg=inference_cfg, 
                     num_classes=num_classes, 
                     forward_args=forward_args,
                 )
-                fix_ann_pairs = inference_cfg.get('fix_ann_pairs', None)
-                if fix_ann_pairs is None:
-                    for aug_opt in self.cfg.DATASET_CFG['train']['aug_opts']:
-                        if 'RandomFlip' in aug_opt: 
-                            fix_ann_pairs = aug_opt[-1].get('fix_ann_pairs', None)
-                if fix_ann_pairs is not None:
+                fixed_seg_target_pairs = inference_cfg.get('fixed_seg_target_pairs', None)
+                if fixed_seg_target_pairs is None:
+                    for data_pipeline in self.cfg.SEGMENTOR_CFG['dataset']['train']['data_pipelines']:
+                        if 'RandomFlip' in data_pipeline: 
+                            fixed_seg_target_pairs = data_pipeline[-1].get('fixed_seg_target_pairs', None)
+                if fixed_seg_target_pairs is not None:
                     outputs_flip_clone = outputs_flip.data.clone()
-                    for (pair_a, pair_b) in fix_ann_pairs:
+                    for (pair_a, pair_b) in fixed_seg_target_pairs:
                         outputs_flip[:, pair_a, :, :] = outputs_flip_clone[:, pair_b, :, :]
                         outputs_flip[:, pair_b, :, :] = outputs_flip_clone[:, pair_a, :, :]
                 outputs_flip = torch.from_numpy(np.flip(outputs_flip.cpu().numpy(), axis=3).copy()).type_as(outputs)
                 outputs_list.append(outputs_flip)
         return outputs_list
     '''inference'''
     def inference(self, segmentor, images, inference_cfg, num_classes, forward_args=None):
@@ -207,68 +203,68 @@
 
 
 '''main'''
 def main():
     # parse arguments
     args = parseArgs()
     cfg, cfg_file_path = BuildConfig(args.cfgfilepath)
-    # check work dir
-    checkdir(cfg.COMMON_CFG['work_dir'])
+    # touch work dir
+    touchdir(cfg.SEGMENTOR_CFG['work_dir'])
     # initialize logger_handle
-    logger_handle = Logger(cfg.COMMON_CFG['logfilepath'])
+    logger_handle = Logger(cfg.SEGMENTOR_CFG['logfilepath'])
     # number of gpus, for distribued testing, only support a process for a GPU
     ngpus_per_node = torch.cuda.device_count()
     if ngpus_per_node != args.nproc_per_node:
         if (args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
             logger_handle.warning('ngpus_per_node is not equal to nproc_per_node, force ngpus_per_node = nproc_per_node by default')
         ngpus_per_node = args.nproc_per_node
     # instanced Tester
     all_preds, all_gts = [], []
     client = Tester(cfg=cfg, ngpus_per_node=ngpus_per_node, logger_handle=logger_handle, cmd_args=args, cfg_file_path=cfg_file_path)
     client.start(all_preds, all_gts)
     # save results and evaluate
     rank_id = int(os.environ['SLURM_PROCID']) if 'SLURM_PROCID' in os.environ else args.local_rank
-    work_dir = cfg.COMMON_CFG['work_dir']
-    filename = cfg.COMMON_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank_id}.' + cfg.COMMON_CFG['resultsavepath'].split('.')[-1]
+    work_dir = cfg.SEGMENTOR_CFG['work_dir']
+    filename = cfg.SEGMENTOR_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank_id}.' + cfg.SEGMENTOR_CFG['resultsavepath'].split('.')[-1]
     with open(os.path.join(work_dir, filename), 'wb') as fp:
         pickle.dump([all_preds, all_gts], fp)
     rank = torch.tensor([rank_id], device='cuda')
     rank_list = [rank.clone() for _ in range(args.nproc_per_node)]
     dist.all_gather(rank_list, rank)
     logger_handle.info('Rank %s finished' % int(rank.item()))
     if (args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
         all_preds_gather, all_gts_gather = [], []
         for rank in rank_list:
             rank = str(int(rank.item()))
-            filename = cfg.COMMON_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank}.' + cfg.COMMON_CFG['resultsavepath'].split('.')[-1]
+            filename = cfg.SEGMENTOR_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank}.' + cfg.SEGMENTOR_CFG['resultsavepath'].split('.')[-1]
             fp = open(os.path.join(work_dir, filename), 'rb')
             all_preds, all_gts = pickle.load(fp)
             all_preds_gather += all_preds
             all_gts_gather += all_gts
         all_preds, all_gts = all_preds_gather, all_gts_gather
         all_preds_filtered, all_gts_filtered, all_ids = [], [], []
         for idx, pred in enumerate(all_preds):
             if pred[0] in all_ids: 
                 continue
             all_ids.append(pred[0])
             all_preds_filtered.append(pred[1])
             all_gts_filtered.append(all_gts[idx])
         all_preds, all_gts = all_preds_filtered, all_gts_filtered
         logger_handle.info('All Finished, all_preds: %s, all_gts: %s' % (len(all_preds), len(all_gts)))
-        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=copy.deepcopy(cfg.DATASET_CFG))
+        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=cfg.SEGMENTOR_CFG['dataset'])
         if args.evalmode == 'offline':
             result = dataset.evaluate(
-                predictions=all_preds, 
-                groundtruths=all_gts, 
-                metric_list=cfg.INFERENCE_CFG.get('metric_list', ['iou', 'miou']),
+                seg_preds=all_preds, 
+                seg_targets=all_gts, 
+                metric_list=cfg.SEGMENTOR_CFG['inference'].get('metric_list', ['iou', 'miou']),
                 num_classes=cfg.SEGMENTOR_CFG['num_classes'],
                 ignore_index=-1,
             )
             logger_handle.info(result)
         else:
-            dataset.formatresults(all_preds, all_ids)
+            dataset.formatresults(all_preds, all_ids, savedir=os.path.join(work_dir, 'results'))
 
 
 '''debug'''
 if __name__ == '__main__':
     with torch.no_grad():
         main()
```

### Comparing `sssegmentation-1.2.0/ssseg/train.py` & `SSSegmentation-1.3.0/ssseg/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 Function:
-    Train the segmentor
+    Implementation of Trainer
 Author:
     Zhenchao Jin
 '''
 import os
 import copy
 import torch
 import pickle
@@ -13,29 +13,30 @@
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
 from tqdm import tqdm
 from configs import BuildConfig
 from modules import (
-    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildOptimizer, BuildScheduler, initslurm,
-    BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, Logger, setRandomSeed, BuildPalette, checkdir, loadcheckpoints, savecheckpoints
+    BuildDataset, BuildDistributedDataloader, BuildDistributedModel, BuildLoss, BuildBackbone, BuildSegmentor, BuildPixelSampler, 
+    Logger, initslurm, setrandomseed, touchdir, loadckpts, saveckpts, BuildOptimizer, BuildScheduler
 )
 warnings.filterwarnings('ignore')
 
 
 '''parse arguments in command line'''
 def parseArgs():
     parser = argparse.ArgumentParser(description='SSSegmentation is an open source supervised semantic segmentation toolbox based on PyTorch')
     parser.add_argument('--local_rank', dest='local_rank', help='node rank for distributed training', default=0, type=int)
     parser.add_argument('--nproc_per_node', dest='nproc_per_node', help='number of process per node', default=8, type=int)
     parser.add_argument('--cfgfilepath', dest='cfgfilepath', help='config file path you want to use', type=str, required=True)
-    parser.add_argument('--checkpointspath', dest='checkpointspath', help='checkpoints you want to resume from', default='', type=str)
+    parser.add_argument('--ckptspath', dest='ckptspath', help='checkpoints you want to resume from', default='', type=str)
+    parser.add_argument('--slurm', dest='slurm', help='please add --slurm if you are using slurm', default=False, action='store_true')
     args = parser.parse_args()
-    initslurm(args, '29000')
+    if args.slurm: initslurm(args, '29000')
     return args
 
 
 '''Trainer'''
 class Trainer():
     def __init__(self, cfg, ngpus_per_node, logger_handle, cmd_args, cfg_file_path):
         # set attribute
@@ -43,159 +44,157 @@
         self.ngpus_per_node = ngpus_per_node
         self.logger_handle = logger_handle
         self.cmd_args = cmd_args
         self.cfg_file_path = cfg_file_path
         assert torch.cuda.is_available(), 'cuda is not available'
         # init distributed training
         dist.init_process_group(backend=self.cfg.SEGMENTOR_CFG.get('backend', 'nccl'))
+        # open full fp32
+        torch.backends.cuda.matmul.allow_tf32 = False
+        torch.backends.cudnn.allow_tf32 = False
     '''start trainer'''
     def start(self):
         cfg, ngpus_per_node, logger_handle, cmd_args, cfg_file_path = self.cfg, self.ngpus_per_node, self.logger_handle, self.cmd_args, self.cfg_file_path
         # build dataset and dataloader
-        dataset = BuildDataset(mode='TRAIN', logger_handle=logger_handle, dataset_cfg=copy.deepcopy(cfg.DATASET_CFG))
+        dataset = BuildDataset(mode='TRAIN', logger_handle=logger_handle, dataset_cfg=cfg.SEGMENTOR_CFG['dataset'])
         assert dataset.num_classes == cfg.SEGMENTOR_CFG['num_classes'], 'parsed config file %s error' % cfg_file_path
-        dataloader_cfg = copy.deepcopy(cfg.DATALOADER_CFG)
-        batch_size, num_workers = dataloader_cfg['train']['batch_size'], dataloader_cfg['train']['num_workers']
-        batch_size_per_node = batch_size // ngpus_per_node
-        num_workers_per_node = num_workers // ngpus_per_node
-        dataloader_cfg['train'].update({'batch_size': batch_size_per_node, 'num_workers': num_workers_per_node})
+        dataloader_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['dataloader'])
+        expected_total_train_bs_for_assert = dataloader_cfg.pop('expected_total_train_bs_for_assert')
+        dataloader_cfg['train']['batch_size'], dataloader_cfg['train']['num_workers'] = dataloader_cfg['train'].pop('batch_size_per_gpu'), dataloader_cfg['train'].pop('num_workers_per_gpu')
+        dataloader_cfg['test']['batch_size'], dataloader_cfg['test']['num_workers'] = dataloader_cfg['test'].pop('batch_size_per_gpu'), dataloader_cfg['test'].pop('num_workers_per_gpu')
+        assert expected_total_train_bs_for_assert == dataloader_cfg['train']['batch_size'] * ngpus_per_node
         dataloader = BuildDistributedDataloader(dataset=dataset, dataloader_cfg=dataloader_cfg['train'])
         # build segmentor
         segmentor = BuildSegmentor(segmentor_cfg=copy.deepcopy(cfg.SEGMENTOR_CFG), mode='TRAIN')
         torch.cuda.set_device(cmd_args.local_rank)
         segmentor.cuda(cmd_args.local_rank)
         torch.backends.cudnn.benchmark = cfg.SEGMENTOR_CFG['benchmark']
         # build optimizer
-        optimizer_cfg = copy.deepcopy(cfg.OPTIMIZER_CFG)
-        optimizer = BuildOptimizer(segmentor, optimizer_cfg)
+        optimizer = BuildOptimizer(segmentor, cfg.SEGMENTOR_CFG['scheduler']['optimizer'])
         # build fp16
         fp16_cfg = self.cfg.SEGMENTOR_CFG.get('fp16_cfg', {'type': None})
         fp16_type = fp16_cfg.pop('type')
         assert fp16_type in [None, 'apex']
         if fp16_type is not None:
             import apex
             segmentor, optimizer = apex.amp.initialize(segmentor, optimizer, **fp16_cfg)
-            for m in segmentor.modules():
-                if hasattr(m, 'fp16_enabled'):
-                    m.fp16_enabled = True
         # build scheduler
-        scheduler_cfg = copy.deepcopy(cfg.SCHEDULER_CFG)
+        scheduler_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['scheduler'])
         scheduler_cfg.update({
-            'lr': cfg.OPTIMIZER_CFG['lr'],
+            'lr': cfg.SEGMENTOR_CFG['scheduler']['optimizer']['lr'],
             'iters_per_epoch': len(dataloader),
-            'params_rules': cfg.OPTIMIZER_CFG['params_rules'],
+            'params_rules': cfg.SEGMENTOR_CFG['scheduler']['optimizer']['params_rules'],
         })
         scheduler = BuildScheduler(optimizer=optimizer, scheduler_cfg=scheduler_cfg)
         start_epoch, end_epoch = 1, scheduler_cfg['max_epochs']
-        # load checkpoints
-        if cmd_args.checkpointspath and os.path.exists(cmd_args.checkpointspath):
-            checkpoints = loadcheckpoints(cmd_args.checkpointspath, logger_handle=logger_handle, cmd_args=cmd_args)
+        # load ckpts
+        if cmd_args.ckptspath and os.path.exists(cmd_args.ckptspath):
+            ckpts = loadckpts(cmd_args.ckptspath)
             try:
-                segmentor.load_state_dict(checkpoints['model'])
+                segmentor.load_state_dict(ckpts['model'])
             except Exception as e:
-                logger_handle.warning(str(e) + '\n' + 'Try to load checkpoints by using strict=False')
-                segmentor.load_state_dict(checkpoints['model'], strict=False)
-            if 'optimizer' in checkpoints: 
-                optimizer.load_state_dict(checkpoints['optimizer'])
-            if 'cur_epoch' in checkpoints: 
-                start_epoch = checkpoints['cur_epoch'] + 1
-                scheduler.setstate({'cur_epoch': checkpoints['cur_epoch'], 'cur_iter': checkpoints['cur_iter']})
-                assert checkpoints['cur_iter'] == len(dataloader) * checkpoints['cur_epoch']
-            if 'amp' in checkpoints and fp16_type is not None:
-                apex.amp.load_state_dict(checkpoints['amp'])
+                logger_handle.warning(str(e) + '\n' + 'Try to load ckpts by using strict=False')
+                segmentor.load_state_dict(ckpts['model'], strict=False)
+            if 'optimizer' in ckpts: 
+                optimizer.load_state_dict(ckpts['optimizer'])
+            if 'cur_epoch' in ckpts: 
+                start_epoch = ckpts['cur_epoch'] + 1
+                scheduler.setstate({'cur_epoch': ckpts['cur_epoch'], 'cur_iter': ckpts['cur_iter']})
+                assert ckpts['cur_iter'] == len(dataloader) * ckpts['cur_epoch']
+            if 'amp' in ckpts and fp16_type is not None:
+                apex.amp.load_state_dict(ckpts['amp'])
         else:
-            cmd_args.checkpointspath = ''
+            cmd_args.ckptspath = ''
         # parallel segmentor
-        segmentor = BuildDistributedModel(segmentor, {'device_ids': [cmd_args.local_rank]})
+        build_dist_model_cfg = self.cfg.SEGMENTOR_CFG.get('build_dist_model_cfg', {})
+        build_dist_model_cfg.update({'device_ids': [cmd_args.local_rank]})
+        segmentor = BuildDistributedModel(segmentor, build_dist_model_cfg)
         # print config
         if (cmd_args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
             logger_handle.info(f'Config file path: {cfg_file_path}')
-            logger_handle.info(f'DATASET_CFG: \n{cfg.DATASET_CFG}')
-            logger_handle.info(f'DATALOADER_CFG: \n{cfg.DATALOADER_CFG}')
-            logger_handle.info(f'OPTIMIZER_CFG: \n{cfg.OPTIMIZER_CFG}')
-            logger_handle.info(f'SCHEDULER_CFG: \n{cfg.SCHEDULER_CFG}')
-            logger_handle.info(f'LOSSES_CFG: \n{cfg.LOSSES_CFG}')
-            logger_handle.info(f'SEGMENTOR_CFG: \n{cfg.SEGMENTOR_CFG}')
-            logger_handle.info(f'INFERENCE_CFG: \n{cfg.INFERENCE_CFG}')
-            logger_handle.info(f'COMMON_CFG: \n{cfg.COMMON_CFG}')
-            logger_handle.info(f'Resume from: {cmd_args.checkpointspath}')
+            logger_handle.info(f'Config details: \n{cfg.SEGMENTOR_CFG}')
+            logger_handle.info(f'Resume from: {cmd_args.ckptspath}')
         # start to train the segmentor
         FloatTensor, losses_log_dict_memory = torch.cuda.FloatTensor, {}
         for epoch in range(start_epoch, end_epoch+1):
             # --set train
             segmentor.train()
             dataloader.sampler.set_epoch(epoch)
             # --train epoch
-            for batch_idx, samples in enumerate(dataloader):
+            for batch_idx, samples_meta in enumerate(dataloader):
                 learning_rate = scheduler.updatelr()
-                images, targets = samples['image'].type(FloatTensor), {'segmentation': samples['segmentation'].type(FloatTensor), 'edge': samples['edge'].type(FloatTensor)}
+                images = samples_meta['image'].type(FloatTensor)
+                targets = {'seg_target': samples_meta['seg_target'].type(FloatTensor)}
+                if 'edge_target' in samples_meta: targets['edge_target'] = samples_meta['edge_target'].type(FloatTensor)
                 optimizer.zero_grad()
-                if cfg.SEGMENTOR_CFG['type'] in ['memorynet', 'memorynetv2']:
-                    loss, losses_log_dict = segmentor(images, targets, cfg.LOSSES_CFG, learning_rate=learning_rate, epoch=epoch)
+                if cfg.SEGMENTOR_CFG['type'] in ['MemoryNet', 'MemoryNetV2']:
+                    loss, losses_log_dict = segmentor(images, targets, learning_rate=learning_rate, epoch=epoch)
                 else:
-                    loss, losses_log_dict = segmentor(images, targets, cfg.LOSSES_CFG)
+                    loss, losses_log_dict = segmentor(images, targets)
                 for key, value in losses_log_dict.items():
                     if key in losses_log_dict_memory: 
                         losses_log_dict_memory[key].append(value)
                     else: 
                         losses_log_dict_memory[key] = [value]
                 if fp16_type is not None:
                     with apex.amp.scale_loss(loss, optimizer) as scaled_loss:
                         scaled_loss.backward()
                 else:
                     loss.backward()
                 scheduler.step()
-                if (cmd_args.local_rank == 0) and (scheduler.cur_iter % cfg.COMMON_CFG['log_interval_iterations'] == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
-                    loss_log = ''
-                    for key, value in losses_log_dict_memory.items():
-                        loss_log += '%s %.4f, ' % (key, sum(value) / len(value))
+                if (cmd_args.local_rank == 0) and (scheduler.cur_iter % cfg.SEGMENTOR_CFG['log_interval_iterations'] == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
+                    print_log = {
+                        'epoch': epoch, 'batch': batch_idx+1, 'segmentor': cfg.SEGMENTOR_CFG['type'], 'backbone': cfg.SEGMENTOR_CFG['backbone']['structure_type'],
+                        'dataset': cfg.SEGMENTOR_CFG['dataset']['type'], 'learning_rate': learning_rate,
+                    }
+                    for key in list(losses_log_dict_memory.keys()):
+                        print_log[key] = sum(losses_log_dict_memory[key]) / len(losses_log_dict_memory[key])
+                    logger_handle.info(print_log)
                     losses_log_dict_memory = dict()
-                    logger_handle.info(
-                        f'[Epoch]: {epoch}/{end_epoch}, [Batch]: {batch_idx+1}/{len(dataloader)}, [Segmentor]: {cfg.SEGMENTOR_CFG["type"]}-{cfg.SEGMENTOR_CFG["backbone"]["type"]}, '
-                        f'[DATASET]: {cfg.DATASET_CFG["type"]}, [LEARNING_RATE]: {learning_rate}\n\t[LOSS]: {loss_log}'
-                    )
             scheduler.cur_epoch = epoch
-            # --save checkpoints
-            if (epoch % cfg.COMMON_CFG['save_interval_epochs'] == 0) or (epoch == end_epoch):
+            # --save ckpts
+            if (epoch % cfg.SEGMENTOR_CFG['save_interval_epochs'] == 0) or (epoch == end_epoch):
                 state_dict = scheduler.state()
                 state_dict['model'] = segmentor.module.state_dict()
                 if fp16_type is not None:
                     state_dict['amp'] = apex.amp.state_dict()
-                savepath = os.path.join(cfg.COMMON_CFG['work_dir'], 'epoch_%s.pth' % epoch)
+                savepath = os.path.join(cfg.SEGMENTOR_CFG['work_dir'], 'epoch_%s.pth' % epoch)
                 if (cmd_args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0):
-                    savecheckpoints(state_dict, savepath, logger_handle, cmd_args=cmd_args)
-            # --eval checkpoints
-            if (epoch % cfg.COMMON_CFG['eval_interval_epochs'] == 0) or (epoch == end_epoch):
+                    saveckpts(state_dict, savepath)
+            # --eval ckpts
+            if (epoch % cfg.SEGMENTOR_CFG['eval_interval_epochs'] == 0) or (epoch == end_epoch):
                 self.evaluate(segmentor)
     '''evaluate'''
     def evaluate(self, segmentor):
         cfg, ngpus_per_node, cmd_args, logger_handle = self.cfg, self.ngpus_per_node, self.cmd_args, self.logger_handle
+        # TODO: bug occurs if use --pyt bash
         rank_id = int(os.environ['SLURM_PROCID']) if 'SLURM_PROCID' in os.environ else cmd_args.local_rank
         # build dataset and dataloader
-        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=copy.deepcopy(cfg.DATASET_CFG))
-        dataloader_cfg = copy.deepcopy(cfg.DATALOADER_CFG)
-        batch_size, num_workers = ngpus_per_node, dataloader_cfg['test']['num_workers']
-        batch_size_per_node = batch_size // ngpus_per_node
-        num_workers_per_node = num_workers // ngpus_per_node
-        dataloader_cfg['test'].update({'batch_size': batch_size_per_node, 'num_workers': num_workers_per_node})
+        dataset = BuildDataset(mode='TEST', logger_handle=logger_handle, dataset_cfg=cfg.SEGMENTOR_CFG['dataset'])
+        assert dataset.num_classes == cfg.SEGMENTOR_CFG['num_classes'], 'parsed config file %s error' % cfg_file_path
+        dataloader_cfg = copy.deepcopy(cfg.SEGMENTOR_CFG['dataloader'])
+        expected_total_train_bs_for_assert = dataloader_cfg.pop('expected_total_train_bs_for_assert')
+        dataloader_cfg['train']['batch_size'], dataloader_cfg['train']['num_workers'] = dataloader_cfg['train'].pop('batch_size_per_gpu'), dataloader_cfg['train'].pop('num_workers_per_gpu')
+        dataloader_cfg['test']['batch_size'], dataloader_cfg['test']['num_workers'] = dataloader_cfg['test'].pop('batch_size_per_gpu'), dataloader_cfg['test'].pop('num_workers_per_gpu')
+        assert expected_total_train_bs_for_assert == dataloader_cfg['train']['batch_size'] * ngpus_per_node
         dataloader = BuildDistributedDataloader(dataset=dataset, dataloader_cfg=dataloader_cfg['test'])
         # start to eval
         segmentor.eval()
         segmentor.module.mode = 'TEST'
-        inference_cfg, all_preds, all_gts = cfg.INFERENCE_CFG, [], []
+        inference_cfg, all_preds, all_gts = cfg.SEGMENTOR_CFG['inference'], [], []
         align_corners = segmentor.module.align_corners
         FloatTensor = torch.cuda.FloatTensor
         use_probs_before_resize = inference_cfg['tricks']['use_probs_before_resize']
         assert inference_cfg['mode'] in ['whole', 'slide']
         with torch.no_grad():
             dataloader.sampler.set_epoch(0)
             pbar = tqdm(enumerate(dataloader))
-            for batch_idx, samples in pbar:
+            for batch_idx, samples_meta in pbar:
                 pbar.set_description('Processing %s/%s in rank %s' % (batch_idx+1, len(dataloader), rank_id))
-                imageids, images, widths, heights, gts = samples['id'], samples['image'].type(FloatTensor), samples['width'], samples['height'], samples['groundtruth']
+                imageids, images, widths, heights, gts = samples_meta['id'], samples_meta['image'].type(FloatTensor), samples_meta['width'], samples_meta['height'], samples_meta['seg_target']
                 if inference_cfg['mode'] == 'whole':
                     outputs = segmentor(images)
                     if use_probs_before_resize:
                         outputs = F.softmax(outputs, dim=1)
                 else:
                     opts = inference_cfg['opts']
                     stride_h, stride_w = opts['stride']
@@ -223,61 +222,61 @@
                     output = F.interpolate(outputs[idx: idx+1], size=(heights[idx], widths[idx]), mode='bilinear', align_corners=align_corners)
                     pred = (torch.argmax(output[0], dim=0)).cpu().numpy().astype(np.int32)
                     all_preds.append([imageids[idx], pred])
                     gt = gts[idx].cpu().numpy().astype(np.int32)
                     gt[gt >= dataset.num_classes] = -1
                     all_gts.append(gt)
         # collect eval results and calculate the metric
-        filename = cfg.COMMON_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank_id}.' + cfg.COMMON_CFG['resultsavepath'].split('.')[-1]
-        with open(os.path.join(cfg.COMMON_CFG['work_dir'], filename), 'wb') as fp:
+        filename = cfg.SEGMENTOR_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank_id}.' + cfg.SEGMENTOR_CFG['resultsavepath'].split('.')[-1]
+        with open(os.path.join(cfg.SEGMENTOR_CFG['work_dir'], filename), 'wb') as fp:
             pickle.dump([all_preds, all_gts], fp)
         rank = torch.tensor([rank_id], device='cuda')
         rank_list = [rank.clone() for _ in range(ngpus_per_node)]
         dist.all_gather(rank_list, rank)
         logger_handle.info('Rank %s finished' % int(rank.item()))
         if rank_id == 0:
             all_preds_gather, all_gts_gather = [], []
             for rank in rank_list:
                 rank = str(int(rank.item()))
-                filename = cfg.COMMON_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank}.' + cfg.COMMON_CFG['resultsavepath'].split('.')[-1]
-                fp = open(os.path.join(cfg.COMMON_CFG['work_dir'], filename), 'rb')
+                filename = cfg.SEGMENTOR_CFG['resultsavepath'].split('/')[-1].split('.')[0] + f'_{rank}.' + cfg.SEGMENTOR_CFG['resultsavepath'].split('.')[-1]
+                fp = open(os.path.join(cfg.SEGMENTOR_CFG['work_dir'], filename), 'rb')
                 all_preds, all_gts = pickle.load(fp)
                 all_preds_gather += all_preds
                 all_gts_gather += all_gts
             all_preds, all_gts = all_preds_gather, all_gts_gather
             all_preds_filtered, all_gts_filtered, all_ids = [], [], []
             for idx, pred in enumerate(all_preds):
                 if pred[0] in all_ids: 
                     continue
                 all_ids.append(pred[0])
                 all_preds_filtered.append(pred[1])
                 all_gts_filtered.append(all_gts[idx])
             all_preds, all_gts = all_preds_filtered, all_gts_filtered
             logger_handle.info('All Finished, all_preds: %s, all_gts: %s' % (len(all_preds), len(all_gts)))
             result = dataset.evaluate(
-                predictions=all_preds, 
-                groundtruths=all_gts, 
-                metric_list=cfg.INFERENCE_CFG.get('metric_list', ['iou', 'miou']),
+                seg_preds=all_preds, 
+                seg_targets=all_gts, 
+                metric_list=inference_cfg.get('metric_list', ['iou', 'miou']),
                 num_classes=cfg.SEGMENTOR_CFG['num_classes'],
                 ignore_index=-1,
             )
             logger_handle.info(result)
         segmentor.train()
         segmentor.module.mode = 'TRAIN'
 
 
 '''main'''
 def main():
     # parse arguments
     args = parseArgs()
     cfg, cfg_file_path = BuildConfig(args.cfgfilepath)
-    # check work dir
-    checkdir(cfg.COMMON_CFG['work_dir'])
+    # touch work dir
+    touchdir(cfg.SEGMENTOR_CFG['work_dir'])
     # initialize logger_handle
-    logger_handle = Logger(cfg.COMMON_CFG['logfilepath'])
+    logger_handle = Logger(cfg.SEGMENTOR_CFG['logfilepath'])
     # number of gpus, for distribued training, only support a process for a GPU
     ngpus_per_node = torch.cuda.device_count()
     if ngpus_per_node != args.nproc_per_node:
         if (args.local_rank == 0) and (int(os.environ.get('SLURM_PROCID', 0)) == 0): 
             logger_handle.warning('ngpus_per_node is not equal to nproc_per_node, force ngpus_per_node = nproc_per_node by default')
         ngpus_per_node = args.nproc_per_node
     # instanced Trainer
```

### Comparing `sssegmentation-1.2.0/sssegmentation.egg-info/SOURCES.txt` & `SSSegmentation-1.3.0/SSSegmentation.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 LICENSE
 README.md
 setup.py
+SSSegmentation.egg-info/PKG-INFO
+SSSegmentation.egg-info/SOURCES.txt
+SSSegmentation.egg-info/dependency_links.txt
+SSSegmentation.egg-info/requires.txt
+SSSegmentation.egg-info/top_level.txt
+SSSegmentation.egg-info/zip-safe
 ssseg/__init__.py
 ssseg/inference.py
 ssseg/test.py
 ssseg/train.py
 ssseg/configs/__init__.py
 ssseg/configs/builder.py
+ssseg/configs/_base_/__init__.py
+ssseg/configs/_base_/dataloaders/__init__.py
+ssseg/configs/_base_/dataloaders/default_dataloader_bs16.py
+ssseg/configs/_base_/dataloaders/default_dataloader_bs32.py
+ssseg/configs/_base_/dataloaders/default_dataloader_bs40.py
+ssseg/configs/_base_/dataloaders/default_dataloader_bs8.py
+ssseg/configs/_base_/datasets/__init__.py
+ssseg/configs/_base_/datasets/ade20k_512x512.py
+ssseg/configs/_base_/datasets/ade20k_640x640.py
+ssseg/configs/_base_/datasets/atr_473x473.py
+ssseg/configs/_base_/datasets/chasedb1_128x128.py
+ssseg/configs/_base_/datasets/cihp_473x473.py
+ssseg/configs/_base_/datasets/cityscapes_1024x1024.py
+ssseg/configs/_base_/datasets/cityscapes_512x1024.py
+ssseg/configs/_base_/datasets/cityscapes_832x832.py
+ssseg/configs/_base_/datasets/cocostuff10k_512x512.py
+ssseg/configs/_base_/datasets/drive_64x64.py
+ssseg/configs/_base_/datasets/hrf_256x256.py
+ssseg/configs/_base_/datasets/lip_473x473.py
+ssseg/configs/_base_/datasets/pascalcontext59_480x480.py
+ssseg/configs/_base_/datasets/pascalcontext_480x480.py
+ssseg/configs/_base_/datasets/stare_128x128.py
+ssseg/configs/_base_/datasets/vocaug_512x512.py
+ssseg/configs/_base_/datasets/vspw_512x512.py
 ssseg/modules/__init__.py
 ssseg/modules/datasets/__init__.py
 ssseg/modules/datasets/ade20k.py
 ssseg/modules/datasets/atr.py
 ssseg/modules/datasets/base.py
 ssseg/modules/datasets/builder.py
 ssseg/modules/datasets/chasedb1.py
 ssseg/modules/datasets/cihp.py
 ssseg/modules/datasets/cityscapes.py
 ssseg/modules/datasets/coco.py
+ssseg/modules/datasets/darkzurich.py
 ssseg/modules/datasets/drive.py
 ssseg/modules/datasets/hrf.py
 ssseg/modules/datasets/lip.py
 ssseg/modules/datasets/mhp.py
+ssseg/modules/datasets/nighttimedriving.py
 ssseg/modules/datasets/sbushadow.py
 ssseg/modules/datasets/stare.py
 ssseg/modules/datasets/supervisely.py
 ssseg/modules/datasets/voc.py
 ssseg/modules/datasets/vspw.py
 ssseg/modules/datasets/pipelines/__init__.py
 ssseg/modules/datasets/pipelines/evaluation.py
@@ -66,24 +98,25 @@
 ssseg/modules/models/backbones/bricks/misc/__init__.py
 ssseg/modules/models/backbones/bricks/misc/l2norm.py
 ssseg/modules/models/backbones/bricks/misc/scale.py
 ssseg/modules/models/backbones/bricks/misc/utils.py
 ssseg/modules/models/backbones/bricks/misc/weightinit.py
 ssseg/modules/models/backbones/bricks/normalization/__init__.py
 ssseg/modules/models/backbones/bricks/normalization/builder.py
-ssseg/modules/models/backbones/bricks/normalization/utils.py
+ssseg/modules/models/backbones/bricks/normalization/layernorm2d.py
 ssseg/modules/models/backbones/bricks/transformer/__init__.py
 ssseg/modules/models/backbones/bricks/transformer/embed.py
 ssseg/modules/models/backbones/bricks/transformer/ffn.py
 ssseg/modules/models/backbones/bricks/transformer/mha.py
 ssseg/modules/models/backbones/bricks/transformer/misc.py
 ssseg/modules/models/losses/__init__.py
 ssseg/modules/models/losses/accuracy.py
 ssseg/modules/models/losses/builder.py
 ssseg/modules/models/losses/celoss.py
+ssseg/modules/models/losses/cosinesimilarityloss.py
 ssseg/modules/models/losses/diceloss.py
 ssseg/modules/models/losses/focalloss.py
 ssseg/modules/models/losses/klloss.py
 ssseg/modules/models/losses/l1loss.py
 ssseg/modules/models/losses/lovaszloss.py
 ssseg/modules/models/optimizers/__init__.py
 ssseg/modules/models/optimizers/builder.py
@@ -166,14 +199,17 @@
 ssseg/modules/models/segmentors/maskformer/transformers/matcher.py
 ssseg/modules/models/segmentors/maskformer/transformers/predictor.py
 ssseg/modules/models/segmentors/maskformer/transformers/transformer.py
 ssseg/modules/models/segmentors/memorynet/__init__.py
 ssseg/modules/models/segmentors/memorynet/initmemory.py
 ssseg/modules/models/segmentors/memorynet/memory.py
 ssseg/modules/models/segmentors/memorynet/memorynet.py
+ssseg/modules/models/segmentors/memorynetv2/__init__.py
+ssseg/modules/models/segmentors/memorynetv2/memorynetv2.py
+ssseg/modules/models/segmentors/memorynetv2/memoryv2.py
 ssseg/modules/models/segmentors/nonlocalnet/__init__.py
 ssseg/modules/models/segmentors/nonlocalnet/nonlocalblock.py
 ssseg/modules/models/segmentors/nonlocalnet/nonlocalnet.py
 ssseg/modules/models/segmentors/ocrnet/__init__.py
 ssseg/modules/models/segmentors/ocrnet/objectcontext.py
 ssseg/modules/models/segmentors/ocrnet/ocrnet.py
 ssseg/modules/models/segmentors/ocrnet/spatialgather.py
@@ -196,15 +232,8 @@
 ssseg/modules/parallel/__init__.py
 ssseg/modules/parallel/dataloader.py
 ssseg/modules/parallel/model.py
 ssseg/modules/utils/__init__.py
 ssseg/modules/utils/io.py
 ssseg/modules/utils/logger.py
 ssseg/modules/utils/misc.py
-ssseg/modules/utils/palette.py
-ssseg/modules/utils/slurm.py
-sssegmentation.egg-info/PKG-INFO
-sssegmentation.egg-info/SOURCES.txt
-sssegmentation.egg-info/dependency_links.txt
-sssegmentation.egg-info/requires.txt
-sssegmentation.egg-info/top_level.txt
-sssegmentation.egg-info/zip-safe
+ssseg/modules/utils/slurm.py
```

