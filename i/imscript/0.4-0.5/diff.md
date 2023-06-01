# Comparing `tmp/imscript-0.4.tar.gz` & `tmp/imscript-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imscript-0.4.tar", last modified: Thu Jun  1 12:54:14 2023, max compression
+gzip compressed data, was "imscript-0.5.tar", last modified: Thu Jun  1 13:01:03 2023, max compression
```

## Comparing `imscript-0.4.tar` & `imscript-0.5.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 12:54:14.430418 imscript-0.4/
--rw-rw-r--   0 coco      (1000) coco      (1000)       59 2023-04-18 09:51:25.000000 imscript-0.4/MANIFEST.in
--rw-rw-r--   0 coco      (1000) coco      (1000)     6218 2023-03-20 09:48:02.000000 imscript-0.4/Makefile
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 12:54:14.430418 imscript-0.4/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.4/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 12:54:14.402417 imscript-0.4/imscript.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 12:54:14.000000 imscript-0.4/imscript.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     2034 2023-06-01 12:54:14.000000 imscript-0.4/imscript.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 12:54:14.000000 imscript-0.4/imscript.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 12:54:14.000000 imscript-0.4/imscript.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-01 12:54:14.430418 imscript-0.4/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      803 2023-06-01 12:53:37.000000 imscript-0.4/setup.py
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 12:54:14.430418 imscript-0.4/src/
--rw-rw-r--   0 coco      (1000) coco      (1000)      911 2017-10-23 14:34:44.000000 imscript-0.4/src/abstract_dsf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      689 2017-10-23 14:34:44.000000 imscript-0.4/src/abstract_dsf.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     5374 2017-10-23 14:34:44.000000 imscript-0.4/src/abstract_heap.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     8946 2022-11-07 09:50:33.000000 imscript-0.4/src/amle.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2129 2018-02-16 16:28:06.000000 imscript-0.4/src/autotrim.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4987 2019-05-07 13:07:56.000000 imscript-0.4/src/backflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      825 2022-02-25 16:40:51.000000 imscript-0.4/src/bandslice.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5426 2022-11-07 09:50:33.000000 imscript-0.4/src/bdint.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2510 2017-10-23 14:34:44.000000 imscript-0.4/src/bicubic.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1471 2017-10-23 14:34:44.000000 imscript-0.4/src/bicubic_gray.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3011 2017-10-23 14:34:44.000000 imscript-0.4/src/bilinear_interpolation.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14174 2023-05-16 09:57:29.000000 imscript-0.4/src/blur.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     9431 2018-02-16 16:26:37.000000 imscript-0.4/src/bmms.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5726 2021-04-23 16:53:33.000000 imscript-0.4/src/carve.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    18033 2018-12-02 15:33:58.000000 imscript-0.4/src/ccproc.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      783 2017-10-23 14:34:44.000000 imscript-0.4/src/ccproc.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     2529 2017-10-23 14:34:44.000000 imscript-0.4/src/censust.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7642 2019-12-18 13:54:29.000000 imscript-0.4/src/cleant_cgpois.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2238 2017-11-12 08:49:58.000000 imscript-0.4/src/colorcoordsf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4044 2017-11-24 18:26:29.000000 imscript-0.4/src/colormatch.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14726 2022-11-07 09:50:33.000000 imscript-0.4/src/contihist.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1535 2018-04-25 10:33:08.000000 imscript-0.4/src/crop.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      141 2020-04-06 13:26:01.000000 imscript-0.4/src/d5.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    13607 2018-02-16 16:03:22.000000 imscript-0.4/src/dataconv.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2113 2017-10-23 14:34:44.000000 imscript-0.4/src/dct.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1956 2017-10-23 14:34:44.000000 imscript-0.4/src/dht.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5142 2022-11-02 07:40:05.000000 imscript-0.4/src/dither.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5017 2020-01-10 14:33:49.000000 imscript-0.4/src/downsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3508 2019-07-16 11:46:25.000000 imscript-0.4/src/drawsegment.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2448 2017-10-23 14:34:44.000000 imscript-0.4/src/drawtriangle.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2591 2018-11-17 18:44:45.000000 imscript-0.4/src/eucdist.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8492 2017-10-23 14:34:44.000000 imscript-0.4/src/exterior_algebra.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1794 2017-10-23 14:34:44.000000 imscript-0.4/src/extrapolators.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1628 2022-11-07 15:14:20.000000 imscript-0.4/src/fail.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1418 2018-02-16 16:27:35.000000 imscript-0.4/src/fancy_crop.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3506 2018-02-16 16:27:51.000000 imscript-0.4/src/fancy_downsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    20717 2022-07-13 12:27:58.000000 imscript-0.4/src/fancy_image.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4280 2018-10-19 07:13:31.000000 imscript-0.4/src/fancy_image.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     7059 2023-04-07 10:19:22.000000 imscript-0.4/src/fft.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1379 2017-10-23 14:34:44.000000 imscript-0.4/src/fftshift.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    84778 2021-06-03 13:20:54.000000 imscript-0.4/src/flambda.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3235 2018-07-10 14:32:43.000000 imscript-0.4/src/flowarrows.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3618 2018-02-16 16:16:06.000000 imscript-0.4/src/flowinv.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    24129 2023-03-20 09:45:46.000000 imscript-0.4/src/fontu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    32612 2021-06-28 07:40:10.000000 imscript-0.4/src/geomedian.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1604 2021-07-23 15:12:25.000000 imscript-0.4/src/getbands.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4854 2019-04-15 16:46:40.000000 imscript-0.4/src/getpixel.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5688 2022-11-02 07:40:05.000000 imscript-0.4/src/ghisto.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8043 2018-01-03 11:41:10.000000 imscript-0.4/src/gntiply.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1702 2017-10-23 14:34:44.000000 imscript-0.4/src/gram_schmidt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3144 2017-10-23 14:34:44.000000 imscript-0.4/src/grid.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3798 2018-03-22 08:54:00.000000 imscript-0.4/src/heatd.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1127 2018-02-16 18:36:16.000000 imscript-0.4/src/help_stuff.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2848 2017-10-23 14:34:44.000000 imscript-0.4/src/homographies.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6286 2022-02-23 15:28:45.000000 imscript-0.4/src/homwarp.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1039 2018-02-07 17:22:02.000000 imscript-0.4/src/idump.c
--rw-rw-r--   0 coco      (1000) coco      (1000)   183486 2022-11-24 17:47:57.000000 imscript-0.4/src/iio.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8888 2022-05-24 10:44:02.000000 imscript-0.4/src/iio.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     3023 2023-01-23 08:50:42.000000 imscript-0.4/src/iion.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      626 2020-02-07 12:37:20.000000 imscript-0.4/src/iion_int.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      753 2022-11-07 09:50:33.000000 imscript-0.4/src/iion_pure.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      824 2017-10-23 14:34:44.000000 imscript-0.4/src/iion_u16.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      253 2021-03-16 15:08:51.000000 imscript-0.4/src/im.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5683 2020-01-10 14:32:38.000000 imscript-0.4/src/imflip.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      338 2020-01-30 09:53:05.000000 imscript-0.4/src/imhalve.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    23117 2020-01-10 14:32:44.000000 imscript-0.4/src/imprintf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2968 2021-06-15 10:19:21.000000 imscript-0.4/src/linalg.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3661 2022-11-02 07:40:05.000000 imscript-0.4/src/lrcat.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6290 2018-02-16 16:14:16.000000 imscript-0.4/src/marching_interpolation.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2962 2017-10-23 14:34:44.000000 imscript-0.4/src/marching_squares.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7313 2019-01-08 11:10:02.000000 imscript-0.4/src/mdither.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7482 2019-01-08 11:10:15.000000 imscript-0.4/src/mdither2.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7327 2018-11-23 08:20:02.000000 imscript-0.4/src/mdither3.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      193 2017-11-30 11:51:08.000000 imscript-0.4/src/means.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6215 2017-11-01 15:45:05.000000 imscript-0.4/src/mediator.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1756 2017-10-23 14:34:44.000000 imscript-0.4/src/minicg.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    11894 2018-07-10 14:32:17.000000 imscript-0.4/src/modes_detector.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17399 2022-11-07 14:49:50.000000 imscript-0.4/src/moistiv_epipolar.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    15593 2023-02-16 15:39:37.000000 imscript-0.4/src/morsi.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7493 2022-11-02 08:49:14.000000 imscript-0.4/src/nnint.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1938 2017-12-30 15:31:26.000000 imscript-0.4/src/nonmaxsup.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      765 2017-10-23 14:34:44.000000 imscript-0.4/src/ntiply.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      162 2017-12-12 13:31:10.000000 imscript-0.4/src/numbersio.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    12436 2017-10-23 14:34:44.000000 imscript-0.4/src/ok_list.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17774 2023-01-24 10:59:47.000000 imscript-0.4/src/palette.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4036 2020-12-06 18:05:01.000000 imscript-0.4/src/parsenumbers.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1252 2017-11-13 14:55:57.000000 imscript-0.4/src/pickopt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      450 2020-02-13 08:44:15.000000 imscript-0.4/src/pixdump.c
--rw-rw-r--   0 coco      (1000) coco      (1000)   104894 2023-05-24 13:57:34.000000 imscript-0.4/src/plambda.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4668 2021-06-23 14:55:11.000000 imscript-0.4/src/points.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8894 2020-03-09 14:57:59.000000 imscript-0.4/src/ppsmooth.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    29708 2021-12-09 13:36:31.000000 imscript-0.4/src/pview.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    96888 2021-06-14 15:31:43.000000 imscript-0.4/src/pλ.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5168 2022-04-21 08:24:03.000000 imscript-0.4/src/qauto.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2227 2022-11-02 08:48:01.000000 imscript-0.4/src/qeasy.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3944 2023-02-21 16:29:17.000000 imscript-0.4/src/random.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17472 2017-10-23 14:34:44.000000 imscript-0.4/src/ransac.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    24327 2019-05-07 10:03:01.000000 imscript-0.4/src/ransac_cases.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1265 2018-05-31 18:07:33.000000 imscript-0.4/src/redim.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4984 2017-10-23 14:34:44.000000 imscript-0.4/src/registration.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    21672 2023-03-20 12:53:49.000000 imscript-0.4/src/rpc2.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6501 2019-02-23 19:54:59.000000 imscript-0.4/src/rpcfit33.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    11740 2023-05-24 13:58:13.000000 imscript-0.4/src/rpctk.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    12960 2019-02-08 09:45:19.000000 imscript-0.4/src/rpctk_old.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      460 2017-10-23 14:34:44.000000 imscript-0.4/src/seconds.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      464 2023-04-18 11:08:49.000000 imscript-0.4/src/setpixel.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    40509 2022-11-07 15:00:57.000000 imscript-0.4/src/siftie.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    15912 2017-10-23 14:34:44.000000 imscript-0.4/src/siftu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    13108 2022-11-07 09:50:33.000000 imscript-0.4/src/simpois.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1349 2018-08-24 10:55:52.000000 imscript-0.4/src/smapa.h
--rw-rw-r--   0 coco      (1000) coco      (1000)    10832 2018-02-16 16:10:48.000000 imscript-0.4/src/spline.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6230 2020-12-04 11:17:12.000000 imscript-0.4/src/srmatch.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5886 2017-10-23 14:34:44.000000 imscript-0.4/src/strt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1376 2017-10-23 14:34:44.000000 imscript-0.4/src/synflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    29109 2018-02-16 16:35:04.000000 imscript-0.4/src/synflow_core.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3652 2022-11-02 07:40:05.000000 imscript-0.4/src/tbcat.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    23780 2022-11-07 15:01:37.000000 imscript-0.4/src/tiff_octaves_rw.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    73306 2022-11-07 14:55:30.000000 imscript-0.4/src/tiffu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4488 2018-07-11 18:56:13.000000 imscript-0.4/src/upsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17626 2021-07-19 17:20:01.000000 imscript-0.4/src/veco.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14287 2020-01-10 14:33:16.000000 imscript-0.4/src/vecoh.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7890 2020-01-10 14:33:18.000000 imscript-0.4/src/vecov.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      482 2018-01-11 09:37:54.000000 imscript-0.4/src/vector.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8319 2022-12-15 15:23:14.000000 imscript-0.4/src/viewflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    37651 2017-10-23 14:34:44.000000 imscript-0.4/src/vvector.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     5234 2018-03-10 17:30:58.000000 imscript-0.4/src/warp.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      780 2017-10-23 14:34:44.000000 imscript-0.4/src/xfopen.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      847 2022-07-13 12:24:19.000000 imscript-0.4/src/xmalloc.c
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 13:01:03.254272 imscript-0.5/
+-rw-rw-r--   0 coco      (1000) coco      (1000)    41635 2022-05-24 08:55:55.000000 imscript-0.5/.deps.mk
+-rw-rw-r--   0 coco      (1000) coco      (1000)       76 2023-06-01 12:58:57.000000 imscript-0.5/MANIFEST.in
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6218 2023-03-20 09:48:02.000000 imscript-0.5/Makefile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 13:01:03.254272 imscript-0.5/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.5/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 13:01:03.238271 imscript-0.5/imscript.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 13:01:03.000000 imscript-0.5/imscript.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2043 2023-06-01 13:01:03.000000 imscript-0.5/imscript.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 13:01:03.000000 imscript-0.5/imscript.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 13:01:03.000000 imscript-0.5/imscript.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-01 13:01:03.254272 imscript-0.5/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      806 2023-06-01 13:00:06.000000 imscript-0.5/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 13:01:03.254272 imscript-0.5/src/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      911 2017-10-23 14:34:44.000000 imscript-0.5/src/abstract_dsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      689 2017-10-23 14:34:44.000000 imscript-0.5/src/abstract_dsf.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5374 2017-10-23 14:34:44.000000 imscript-0.5/src/abstract_heap.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8946 2022-11-07 09:50:33.000000 imscript-0.5/src/amle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2129 2018-02-16 16:28:06.000000 imscript-0.5/src/autotrim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4987 2019-05-07 13:07:56.000000 imscript-0.5/src/backflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      825 2022-02-25 16:40:51.000000 imscript-0.5/src/bandslice.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5426 2022-11-07 09:50:33.000000 imscript-0.5/src/bdint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2510 2017-10-23 14:34:44.000000 imscript-0.5/src/bicubic.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1471 2017-10-23 14:34:44.000000 imscript-0.5/src/bicubic_gray.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3011 2017-10-23 14:34:44.000000 imscript-0.5/src/bilinear_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14174 2023-05-16 09:57:29.000000 imscript-0.5/src/blur.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     9431 2018-02-16 16:26:37.000000 imscript-0.5/src/bmms.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5726 2021-04-23 16:53:33.000000 imscript-0.5/src/carve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    18033 2018-12-02 15:33:58.000000 imscript-0.5/src/ccproc.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      783 2017-10-23 14:34:44.000000 imscript-0.5/src/ccproc.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2529 2017-10-23 14:34:44.000000 imscript-0.5/src/censust.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7642 2019-12-18 13:54:29.000000 imscript-0.5/src/cleant_cgpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2238 2017-11-12 08:49:58.000000 imscript-0.5/src/colorcoordsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4044 2017-11-24 18:26:29.000000 imscript-0.5/src/colormatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14726 2022-11-07 09:50:33.000000 imscript-0.5/src/contihist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1535 2018-04-25 10:33:08.000000 imscript-0.5/src/crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      141 2020-04-06 13:26:01.000000 imscript-0.5/src/d5.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13607 2018-02-16 16:03:22.000000 imscript-0.5/src/dataconv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2113 2017-10-23 14:34:44.000000 imscript-0.5/src/dct.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1956 2017-10-23 14:34:44.000000 imscript-0.5/src/dht.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5142 2022-11-02 07:40:05.000000 imscript-0.5/src/dither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5017 2020-01-10 14:33:49.000000 imscript-0.5/src/downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3508 2019-07-16 11:46:25.000000 imscript-0.5/src/drawsegment.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2448 2017-10-23 14:34:44.000000 imscript-0.5/src/drawtriangle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2591 2018-11-17 18:44:45.000000 imscript-0.5/src/eucdist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8492 2017-10-23 14:34:44.000000 imscript-0.5/src/exterior_algebra.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1794 2017-10-23 14:34:44.000000 imscript-0.5/src/extrapolators.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1628 2022-11-07 15:14:20.000000 imscript-0.5/src/fail.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1418 2018-02-16 16:27:35.000000 imscript-0.5/src/fancy_crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3506 2018-02-16 16:27:51.000000 imscript-0.5/src/fancy_downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    20717 2022-07-13 12:27:58.000000 imscript-0.5/src/fancy_image.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4280 2018-10-19 07:13:31.000000 imscript-0.5/src/fancy_image.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7059 2023-04-07 10:19:22.000000 imscript-0.5/src/fft.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1379 2017-10-23 14:34:44.000000 imscript-0.5/src/fftshift.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    84778 2021-06-03 13:20:54.000000 imscript-0.5/src/flambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3235 2018-07-10 14:32:43.000000 imscript-0.5/src/flowarrows.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3618 2018-02-16 16:16:06.000000 imscript-0.5/src/flowinv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24129 2023-03-20 09:45:46.000000 imscript-0.5/src/fontu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    32612 2021-06-28 07:40:10.000000 imscript-0.5/src/geomedian.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1604 2021-07-23 15:12:25.000000 imscript-0.5/src/getbands.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4854 2019-04-15 16:46:40.000000 imscript-0.5/src/getpixel.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5688 2022-11-02 07:40:05.000000 imscript-0.5/src/ghisto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8043 2018-01-03 11:41:10.000000 imscript-0.5/src/gntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1702 2017-10-23 14:34:44.000000 imscript-0.5/src/gram_schmidt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3144 2017-10-23 14:34:44.000000 imscript-0.5/src/grid.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3798 2018-03-22 08:54:00.000000 imscript-0.5/src/heatd.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1127 2018-02-16 18:36:16.000000 imscript-0.5/src/help_stuff.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2848 2017-10-23 14:34:44.000000 imscript-0.5/src/homographies.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6286 2022-02-23 15:28:45.000000 imscript-0.5/src/homwarp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1039 2018-02-07 17:22:02.000000 imscript-0.5/src/idump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   183486 2022-11-24 17:47:57.000000 imscript-0.5/src/iio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8888 2022-05-24 10:44:02.000000 imscript-0.5/src/iio.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3023 2023-01-23 08:50:42.000000 imscript-0.5/src/iion.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      626 2020-02-07 12:37:20.000000 imscript-0.5/src/iion_int.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      753 2022-11-07 09:50:33.000000 imscript-0.5/src/iion_pure.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      824 2017-10-23 14:34:44.000000 imscript-0.5/src/iion_u16.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      253 2021-03-16 15:08:51.000000 imscript-0.5/src/im.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5683 2020-01-10 14:32:38.000000 imscript-0.5/src/imflip.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      338 2020-01-30 09:53:05.000000 imscript-0.5/src/imhalve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23117 2020-01-10 14:32:44.000000 imscript-0.5/src/imprintf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2968 2021-06-15 10:19:21.000000 imscript-0.5/src/linalg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3661 2022-11-02 07:40:05.000000 imscript-0.5/src/lrcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6290 2018-02-16 16:14:16.000000 imscript-0.5/src/marching_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2962 2017-10-23 14:34:44.000000 imscript-0.5/src/marching_squares.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7313 2019-01-08 11:10:02.000000 imscript-0.5/src/mdither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7482 2019-01-08 11:10:15.000000 imscript-0.5/src/mdither2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7327 2018-11-23 08:20:02.000000 imscript-0.5/src/mdither3.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      193 2017-11-30 11:51:08.000000 imscript-0.5/src/means.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6215 2017-11-01 15:45:05.000000 imscript-0.5/src/mediator.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1756 2017-10-23 14:34:44.000000 imscript-0.5/src/minicg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    11894 2018-07-10 14:32:17.000000 imscript-0.5/src/modes_detector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17399 2022-11-07 14:49:50.000000 imscript-0.5/src/moistiv_epipolar.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15593 2023-02-16 15:39:37.000000 imscript-0.5/src/morsi.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7493 2022-11-02 08:49:14.000000 imscript-0.5/src/nnint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1938 2017-12-30 15:31:26.000000 imscript-0.5/src/nonmaxsup.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      765 2017-10-23 14:34:44.000000 imscript-0.5/src/ntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      162 2017-12-12 13:31:10.000000 imscript-0.5/src/numbersio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12436 2017-10-23 14:34:44.000000 imscript-0.5/src/ok_list.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17774 2023-01-24 10:59:47.000000 imscript-0.5/src/palette.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4036 2020-12-06 18:05:01.000000 imscript-0.5/src/parsenumbers.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1252 2017-11-13 14:55:57.000000 imscript-0.5/src/pickopt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      450 2020-02-13 08:44:15.000000 imscript-0.5/src/pixdump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   104894 2023-05-24 13:57:34.000000 imscript-0.5/src/plambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4668 2021-06-23 14:55:11.000000 imscript-0.5/src/points.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8894 2020-03-09 14:57:59.000000 imscript-0.5/src/ppsmooth.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29708 2021-12-09 13:36:31.000000 imscript-0.5/src/pview.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    96888 2021-06-14 15:31:43.000000 imscript-0.5/src/pλ.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5168 2022-04-21 08:24:03.000000 imscript-0.5/src/qauto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2227 2022-11-02 08:48:01.000000 imscript-0.5/src/qeasy.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3944 2023-02-21 16:29:17.000000 imscript-0.5/src/random.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17472 2017-10-23 14:34:44.000000 imscript-0.5/src/ransac.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24327 2019-05-07 10:03:01.000000 imscript-0.5/src/ransac_cases.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1265 2018-05-31 18:07:33.000000 imscript-0.5/src/redim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4984 2017-10-23 14:34:44.000000 imscript-0.5/src/registration.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    21672 2023-03-20 12:53:49.000000 imscript-0.5/src/rpc2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6501 2019-02-23 19:54:59.000000 imscript-0.5/src/rpcfit33.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    11740 2023-05-24 13:58:13.000000 imscript-0.5/src/rpctk.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12960 2019-02-08 09:45:19.000000 imscript-0.5/src/rpctk_old.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      460 2017-10-23 14:34:44.000000 imscript-0.5/src/seconds.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      464 2023-04-18 11:08:49.000000 imscript-0.5/src/setpixel.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    40509 2022-11-07 15:00:57.000000 imscript-0.5/src/siftie.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15912 2017-10-23 14:34:44.000000 imscript-0.5/src/siftu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13108 2022-11-07 09:50:33.000000 imscript-0.5/src/simpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1349 2018-08-24 10:55:52.000000 imscript-0.5/src/smapa.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)    10832 2018-02-16 16:10:48.000000 imscript-0.5/src/spline.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6230 2020-12-04 11:17:12.000000 imscript-0.5/src/srmatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5886 2017-10-23 14:34:44.000000 imscript-0.5/src/strt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1376 2017-10-23 14:34:44.000000 imscript-0.5/src/synflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29109 2018-02-16 16:35:04.000000 imscript-0.5/src/synflow_core.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3652 2022-11-02 07:40:05.000000 imscript-0.5/src/tbcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23780 2022-11-07 15:01:37.000000 imscript-0.5/src/tiff_octaves_rw.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    73306 2022-11-07 14:55:30.000000 imscript-0.5/src/tiffu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4488 2018-07-11 18:56:13.000000 imscript-0.5/src/upsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17626 2021-07-19 17:20:01.000000 imscript-0.5/src/veco.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14287 2020-01-10 14:33:16.000000 imscript-0.5/src/vecoh.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7890 2020-01-10 14:33:18.000000 imscript-0.5/src/vecov.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      482 2018-01-11 09:37:54.000000 imscript-0.5/src/vector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8319 2022-12-15 15:23:14.000000 imscript-0.5/src/viewflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    37651 2017-10-23 14:34:44.000000 imscript-0.5/src/vvector.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5234 2018-03-10 17:30:58.000000 imscript-0.5/src/warp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      780 2017-10-23 14:34:44.000000 imscript-0.5/src/xfopen.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      847 2022-07-13 12:24:19.000000 imscript-0.5/src/xmalloc.c
```

### Comparing `imscript-0.4/Makefile` & `imscript-0.5/Makefile`

 * *Files identical despite different names*

### Comparing `imscript-0.4/imscript.egg-info/SOURCES.txt` & `imscript-0.5/imscript.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.deps.mk
 MANIFEST.in
 Makefile
 README
 setup.py
 imscript.egg-info/PKG-INFO
 imscript.egg-info/SOURCES.txt
 imscript.egg-info/dependency_links.txt
```

### Comparing `imscript-0.4/setup.py` & `imscript-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from setuptools.command.install import install
 class myinstall(install):
 	def run(self):
 		import os
 		os.system("mkdir -p bin")
-		os.system("make bin/plambda bin/qauto bin/morsi")
+		os.system("make -j bin/plambda bin/qauto bin/morsi")
 		install.run(self)
 
 
 import setuptools
 setuptools.setup(
 	name = "imscript",
-	version = "0.4",
+	version = "0.5",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@fastmail.com",
 	description = "Image Processing with Unix Pipes",
 	url = "https://github.com/mnhrdt/imscript",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

### Comparing `imscript-0.4/src/abstract_dsf.c` & `imscript-0.5/src/abstract_dsf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/abstract_dsf.h` & `imscript-0.5/src/abstract_dsf.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/abstract_heap.h` & `imscript-0.5/src/abstract_heap.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/amle.c` & `imscript-0.5/src/amle.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/autotrim.c` & `imscript-0.5/src/autotrim.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/backflow.c` & `imscript-0.5/src/backflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bandslice.c` & `imscript-0.5/src/bandslice.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bdint.c` & `imscript-0.5/src/bdint.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bicubic.c` & `imscript-0.5/src/bicubic.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bicubic_gray.c` & `imscript-0.5/src/bicubic_gray.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bilinear_interpolation.c` & `imscript-0.5/src/bilinear_interpolation.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/blur.c` & `imscript-0.5/src/blur.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/bmms.c` & `imscript-0.5/src/bmms.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/carve.c` & `imscript-0.5/src/carve.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ccproc.c` & `imscript-0.5/src/ccproc.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ccproc.h` & `imscript-0.5/src/ccproc.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/censust.c` & `imscript-0.5/src/censust.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/cleant_cgpois.c` & `imscript-0.5/src/cleant_cgpois.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/colorcoordsf.c` & `imscript-0.5/src/colorcoordsf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/colormatch.c` & `imscript-0.5/src/colormatch.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/contihist.c` & `imscript-0.5/src/contihist.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/crop.c` & `imscript-0.5/src/crop.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/dataconv.c` & `imscript-0.5/src/dataconv.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/dct.c` & `imscript-0.5/src/dct.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/dht.c` & `imscript-0.5/src/dht.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/dither.c` & `imscript-0.5/src/dither.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/downsa.c` & `imscript-0.5/src/downsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/drawsegment.c` & `imscript-0.5/src/drawsegment.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/drawtriangle.c` & `imscript-0.5/src/drawtriangle.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/eucdist.c` & `imscript-0.5/src/eucdist.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/exterior_algebra.c` & `imscript-0.5/src/exterior_algebra.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/extrapolators.c` & `imscript-0.5/src/extrapolators.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fail.c` & `imscript-0.5/src/fail.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fancy_crop.c` & `imscript-0.5/src/fancy_crop.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fancy_downsa.c` & `imscript-0.5/src/fancy_downsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fancy_image.c` & `imscript-0.5/src/fancy_image.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fancy_image.h` & `imscript-0.5/src/fancy_image.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fft.c` & `imscript-0.5/src/fft.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fftshift.c` & `imscript-0.5/src/fftshift.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/flambda.c` & `imscript-0.5/src/flambda.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/flowarrows.c` & `imscript-0.5/src/flowarrows.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/flowinv.c` & `imscript-0.5/src/flowinv.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/fontu.c` & `imscript-0.5/src/fontu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/geomedian.c` & `imscript-0.5/src/geomedian.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/getbands.c` & `imscript-0.5/src/getbands.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/getpixel.c` & `imscript-0.5/src/getpixel.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ghisto.c` & `imscript-0.5/src/ghisto.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/gntiply.c` & `imscript-0.5/src/gntiply.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/gram_schmidt.c` & `imscript-0.5/src/gram_schmidt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/grid.c` & `imscript-0.5/src/grid.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/heatd.c` & `imscript-0.5/src/heatd.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/help_stuff.c` & `imscript-0.5/src/help_stuff.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/homographies.c` & `imscript-0.5/src/homographies.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/homwarp.c` & `imscript-0.5/src/homwarp.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/idump.c` & `imscript-0.5/src/idump.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iio.c` & `imscript-0.5/src/iio.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iio.h` & `imscript-0.5/src/iio.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iion.c` & `imscript-0.5/src/iion.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iion_int.c` & `imscript-0.5/src/iion_int.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iion_pure.c` & `imscript-0.5/src/iion_pure.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/iion_u16.c` & `imscript-0.5/src/iion_u16.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/imflip.c` & `imscript-0.5/src/imflip.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/imprintf.c` & `imscript-0.5/src/imprintf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/linalg.c` & `imscript-0.5/src/linalg.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/lrcat.c` & `imscript-0.5/src/lrcat.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/marching_interpolation.c` & `imscript-0.5/src/marching_interpolation.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/marching_squares.c` & `imscript-0.5/src/marching_squares.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/mdither.c` & `imscript-0.5/src/mdither.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/mdither2.c` & `imscript-0.5/src/mdither2.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/mdither3.c` & `imscript-0.5/src/mdither3.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/mediator.c` & `imscript-0.5/src/mediator.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/minicg.c` & `imscript-0.5/src/minicg.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/modes_detector.c` & `imscript-0.5/src/modes_detector.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/moistiv_epipolar.c` & `imscript-0.5/src/moistiv_epipolar.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/morsi.c` & `imscript-0.5/src/morsi.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/nnint.c` & `imscript-0.5/src/nnint.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/nonmaxsup.c` & `imscript-0.5/src/nonmaxsup.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ntiply.c` & `imscript-0.5/src/ntiply.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ok_list.c` & `imscript-0.5/src/ok_list.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/palette.c` & `imscript-0.5/src/palette.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/parsenumbers.c` & `imscript-0.5/src/parsenumbers.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/pickopt.c` & `imscript-0.5/src/pickopt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/plambda.c` & `imscript-0.5/src/plambda.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/points.c` & `imscript-0.5/src/points.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ppsmooth.c` & `imscript-0.5/src/ppsmooth.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/pview.c` & `imscript-0.5/src/pview.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/pλ.c` & `imscript-0.5/src/pλ.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/qauto.c` & `imscript-0.5/src/qauto.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/qeasy.c` & `imscript-0.5/src/qeasy.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/random.c` & `imscript-0.5/src/random.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ransac.c` & `imscript-0.5/src/ransac.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/ransac_cases.c` & `imscript-0.5/src/ransac_cases.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/redim.c` & `imscript-0.5/src/redim.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/registration.c` & `imscript-0.5/src/registration.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/rpc2.c` & `imscript-0.5/src/rpc2.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/rpcfit33.c` & `imscript-0.5/src/rpcfit33.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/rpctk.c` & `imscript-0.5/src/rpctk.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/rpctk_old.c` & `imscript-0.5/src/rpctk_old.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/siftie.c` & `imscript-0.5/src/siftie.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/siftu.c` & `imscript-0.5/src/siftu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/simpois.c` & `imscript-0.5/src/simpois.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/smapa.h` & `imscript-0.5/src/smapa.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/spline.c` & `imscript-0.5/src/spline.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/srmatch.c` & `imscript-0.5/src/srmatch.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/strt.c` & `imscript-0.5/src/strt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/synflow.c` & `imscript-0.5/src/synflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/synflow_core.c` & `imscript-0.5/src/synflow_core.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/tbcat.c` & `imscript-0.5/src/tbcat.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/tiff_octaves_rw.c` & `imscript-0.5/src/tiff_octaves_rw.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/tiffu.c` & `imscript-0.5/src/tiffu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/upsa.c` & `imscript-0.5/src/upsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/veco.c` & `imscript-0.5/src/veco.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/vecoh.c` & `imscript-0.5/src/vecoh.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/vecov.c` & `imscript-0.5/src/vecov.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/viewflow.c` & `imscript-0.5/src/viewflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/vvector.h` & `imscript-0.5/src/vvector.h`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/warp.c` & `imscript-0.5/src/warp.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/xfopen.c` & `imscript-0.5/src/xfopen.c`

 * *Files identical despite different names*

### Comparing `imscript-0.4/src/xmalloc.c` & `imscript-0.5/src/xmalloc.c`

 * *Files identical despite different names*

