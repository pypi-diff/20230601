# Comparing `tmp/imscript-0.6.tar.gz` & `tmp/imscript-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imscript-0.6.tar", last modified: Thu Jun  1 15:21:42 2023, max compression
+gzip compressed data, was "imscript-0.7.tar", last modified: Thu Jun  1 15:26:35 2023, max compression
```

## Comparing `imscript-0.6.tar` & `imscript-0.7.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:21:42.848180 imscript-0.6/
--rw-rw-r--   0 coco      (1000) coco      (1000)    41635 2022-05-24 08:55:55.000000 imscript-0.6/.deps.mk
--rw-rw-r--   0 coco      (1000) coco      (1000)       76 2023-06-01 12:58:57.000000 imscript-0.6/MANIFEST.in
--rw-rw-r--   0 coco      (1000) coco      (1000)     6261 2023-06-01 15:20:53.000000 imscript-0.6/Makefile
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 15:21:42.848180 imscript-0.6/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.6/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:21:42.828180 imscript-0.6/imscript.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 15:21:42.000000 imscript-0.6/imscript.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     2043 2023-06-01 15:21:42.000000 imscript-0.6/imscript.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 15:21:42.000000 imscript-0.6/imscript.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 15:21:42.000000 imscript-0.6/imscript.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-01 15:21:42.848180 imscript-0.6/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      806 2023-06-01 15:21:27.000000 imscript-0.6/setup.py
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:21:42.848180 imscript-0.6/src/
--rw-rw-r--   0 coco      (1000) coco      (1000)      911 2017-10-23 14:34:44.000000 imscript-0.6/src/abstract_dsf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      689 2017-10-23 14:34:44.000000 imscript-0.6/src/abstract_dsf.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     5374 2017-10-23 14:34:44.000000 imscript-0.6/src/abstract_heap.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     8946 2022-11-07 09:50:33.000000 imscript-0.6/src/amle.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2129 2018-02-16 16:28:06.000000 imscript-0.6/src/autotrim.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4987 2019-05-07 13:07:56.000000 imscript-0.6/src/backflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      825 2022-02-25 16:40:51.000000 imscript-0.6/src/bandslice.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5426 2022-11-07 09:50:33.000000 imscript-0.6/src/bdint.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2510 2017-10-23 14:34:44.000000 imscript-0.6/src/bicubic.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1471 2017-10-23 14:34:44.000000 imscript-0.6/src/bicubic_gray.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3011 2017-10-23 14:34:44.000000 imscript-0.6/src/bilinear_interpolation.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14174 2023-05-16 09:57:29.000000 imscript-0.6/src/blur.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     9431 2018-02-16 16:26:37.000000 imscript-0.6/src/bmms.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5726 2021-04-23 16:53:33.000000 imscript-0.6/src/carve.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    18033 2018-12-02 15:33:58.000000 imscript-0.6/src/ccproc.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      783 2017-10-23 14:34:44.000000 imscript-0.6/src/ccproc.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     2529 2017-10-23 14:34:44.000000 imscript-0.6/src/censust.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7642 2019-12-18 13:54:29.000000 imscript-0.6/src/cleant_cgpois.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2238 2017-11-12 08:49:58.000000 imscript-0.6/src/colorcoordsf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4044 2017-11-24 18:26:29.000000 imscript-0.6/src/colormatch.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14726 2022-11-07 09:50:33.000000 imscript-0.6/src/contihist.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1535 2018-04-25 10:33:08.000000 imscript-0.6/src/crop.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      141 2020-04-06 13:26:01.000000 imscript-0.6/src/d5.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    13607 2018-02-16 16:03:22.000000 imscript-0.6/src/dataconv.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2113 2017-10-23 14:34:44.000000 imscript-0.6/src/dct.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1956 2017-10-23 14:34:44.000000 imscript-0.6/src/dht.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5142 2022-11-02 07:40:05.000000 imscript-0.6/src/dither.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5017 2020-01-10 14:33:49.000000 imscript-0.6/src/downsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3508 2019-07-16 11:46:25.000000 imscript-0.6/src/drawsegment.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2448 2017-10-23 14:34:44.000000 imscript-0.6/src/drawtriangle.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2591 2018-11-17 18:44:45.000000 imscript-0.6/src/eucdist.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8492 2017-10-23 14:34:44.000000 imscript-0.6/src/exterior_algebra.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1794 2017-10-23 14:34:44.000000 imscript-0.6/src/extrapolators.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1628 2022-11-07 15:14:20.000000 imscript-0.6/src/fail.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1418 2018-02-16 16:27:35.000000 imscript-0.6/src/fancy_crop.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3506 2018-02-16 16:27:51.000000 imscript-0.6/src/fancy_downsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    20717 2022-07-13 12:27:58.000000 imscript-0.6/src/fancy_image.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4280 2018-10-19 07:13:31.000000 imscript-0.6/src/fancy_image.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     7059 2023-04-07 10:19:22.000000 imscript-0.6/src/fft.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1379 2017-10-23 14:34:44.000000 imscript-0.6/src/fftshift.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    84778 2021-06-03 13:20:54.000000 imscript-0.6/src/flambda.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3235 2018-07-10 14:32:43.000000 imscript-0.6/src/flowarrows.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3618 2018-02-16 16:16:06.000000 imscript-0.6/src/flowinv.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    24129 2023-03-20 09:45:46.000000 imscript-0.6/src/fontu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    32612 2021-06-28 07:40:10.000000 imscript-0.6/src/geomedian.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1604 2021-07-23 15:12:25.000000 imscript-0.6/src/getbands.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4854 2019-04-15 16:46:40.000000 imscript-0.6/src/getpixel.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5688 2022-11-02 07:40:05.000000 imscript-0.6/src/ghisto.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8043 2018-01-03 11:41:10.000000 imscript-0.6/src/gntiply.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1702 2017-10-23 14:34:44.000000 imscript-0.6/src/gram_schmidt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3144 2017-10-23 14:34:44.000000 imscript-0.6/src/grid.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3798 2018-03-22 08:54:00.000000 imscript-0.6/src/heatd.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1127 2018-02-16 18:36:16.000000 imscript-0.6/src/help_stuff.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2848 2017-10-23 14:34:44.000000 imscript-0.6/src/homographies.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6286 2022-02-23 15:28:45.000000 imscript-0.6/src/homwarp.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1039 2018-02-07 17:22:02.000000 imscript-0.6/src/idump.c
--rw-rw-r--   0 coco      (1000) coco      (1000)   183486 2022-11-24 17:47:57.000000 imscript-0.6/src/iio.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8888 2022-05-24 10:44:02.000000 imscript-0.6/src/iio.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     3023 2023-01-23 08:50:42.000000 imscript-0.6/src/iion.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      626 2020-02-07 12:37:20.000000 imscript-0.6/src/iion_int.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      753 2022-11-07 09:50:33.000000 imscript-0.6/src/iion_pure.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      824 2017-10-23 14:34:44.000000 imscript-0.6/src/iion_u16.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      253 2021-03-16 15:08:51.000000 imscript-0.6/src/im.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5683 2020-01-10 14:32:38.000000 imscript-0.6/src/imflip.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      338 2020-01-30 09:53:05.000000 imscript-0.6/src/imhalve.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    23117 2020-01-10 14:32:44.000000 imscript-0.6/src/imprintf.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2968 2021-06-15 10:19:21.000000 imscript-0.6/src/linalg.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3661 2022-11-02 07:40:05.000000 imscript-0.6/src/lrcat.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6290 2018-02-16 16:14:16.000000 imscript-0.6/src/marching_interpolation.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2962 2017-10-23 14:34:44.000000 imscript-0.6/src/marching_squares.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7313 2019-01-08 11:10:02.000000 imscript-0.6/src/mdither.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7482 2019-01-08 11:10:15.000000 imscript-0.6/src/mdither2.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7327 2018-11-23 08:20:02.000000 imscript-0.6/src/mdither3.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      193 2017-11-30 11:51:08.000000 imscript-0.6/src/means.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6215 2017-11-01 15:45:05.000000 imscript-0.6/src/mediator.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1756 2017-10-23 14:34:44.000000 imscript-0.6/src/minicg.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    11894 2018-07-10 14:32:17.000000 imscript-0.6/src/modes_detector.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17399 2022-11-07 14:49:50.000000 imscript-0.6/src/moistiv_epipolar.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    15593 2023-02-16 15:39:37.000000 imscript-0.6/src/morsi.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7493 2022-11-02 08:49:14.000000 imscript-0.6/src/nnint.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1938 2017-12-30 15:31:26.000000 imscript-0.6/src/nonmaxsup.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      765 2017-10-23 14:34:44.000000 imscript-0.6/src/ntiply.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      162 2017-12-12 13:31:10.000000 imscript-0.6/src/numbersio.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    12436 2017-10-23 14:34:44.000000 imscript-0.6/src/ok_list.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17774 2023-01-24 10:59:47.000000 imscript-0.6/src/palette.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4036 2020-12-06 18:05:01.000000 imscript-0.6/src/parsenumbers.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1252 2017-11-13 14:55:57.000000 imscript-0.6/src/pickopt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      450 2020-02-13 08:44:15.000000 imscript-0.6/src/pixdump.c
--rw-rw-r--   0 coco      (1000) coco      (1000)   104894 2023-05-24 13:57:34.000000 imscript-0.6/src/plambda.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4668 2021-06-23 14:55:11.000000 imscript-0.6/src/points.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8894 2020-03-09 14:57:59.000000 imscript-0.6/src/ppsmooth.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    29708 2021-12-09 13:36:31.000000 imscript-0.6/src/pview.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    96888 2021-06-14 15:31:43.000000 imscript-0.6/src/pλ.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5168 2022-04-21 08:24:03.000000 imscript-0.6/src/qauto.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     2227 2022-11-02 08:48:01.000000 imscript-0.6/src/qeasy.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3944 2023-02-21 16:29:17.000000 imscript-0.6/src/random.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17472 2017-10-23 14:34:44.000000 imscript-0.6/src/ransac.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    24327 2019-05-07 10:03:01.000000 imscript-0.6/src/ransac_cases.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1265 2018-05-31 18:07:33.000000 imscript-0.6/src/redim.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4984 2017-10-23 14:34:44.000000 imscript-0.6/src/registration.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    21672 2023-03-20 12:53:49.000000 imscript-0.6/src/rpc2.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6501 2019-02-23 19:54:59.000000 imscript-0.6/src/rpcfit33.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    11740 2023-05-24 13:58:13.000000 imscript-0.6/src/rpctk.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    12960 2019-02-08 09:45:19.000000 imscript-0.6/src/rpctk_old.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      460 2017-10-23 14:34:44.000000 imscript-0.6/src/seconds.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      464 2023-04-18 11:08:49.000000 imscript-0.6/src/setpixel.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    40509 2022-11-07 15:00:57.000000 imscript-0.6/src/siftie.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    15912 2017-10-23 14:34:44.000000 imscript-0.6/src/siftu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    13108 2022-11-07 09:50:33.000000 imscript-0.6/src/simpois.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1349 2018-08-24 10:55:52.000000 imscript-0.6/src/smapa.h
--rw-rw-r--   0 coco      (1000) coco      (1000)    10832 2018-02-16 16:10:48.000000 imscript-0.6/src/spline.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     6230 2020-12-04 11:17:12.000000 imscript-0.6/src/srmatch.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     5886 2017-10-23 14:34:44.000000 imscript-0.6/src/strt.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     1376 2017-10-23 14:34:44.000000 imscript-0.6/src/synflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    29109 2018-02-16 16:35:04.000000 imscript-0.6/src/synflow_core.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     3652 2022-11-02 07:40:05.000000 imscript-0.6/src/tbcat.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    23780 2022-11-07 15:01:37.000000 imscript-0.6/src/tiff_octaves_rw.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    73306 2022-11-07 14:55:30.000000 imscript-0.6/src/tiffu.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     4488 2018-07-11 18:56:13.000000 imscript-0.6/src/upsa.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    17626 2021-07-19 17:20:01.000000 imscript-0.6/src/veco.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    14287 2020-01-10 14:33:16.000000 imscript-0.6/src/vecoh.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     7890 2020-01-10 14:33:18.000000 imscript-0.6/src/vecov.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      482 2018-01-11 09:37:54.000000 imscript-0.6/src/vector.c
--rw-rw-r--   0 coco      (1000) coco      (1000)     8319 2022-12-15 15:23:14.000000 imscript-0.6/src/viewflow.c
--rw-rw-r--   0 coco      (1000) coco      (1000)    37651 2017-10-23 14:34:44.000000 imscript-0.6/src/vvector.h
--rw-rw-r--   0 coco      (1000) coco      (1000)     5234 2018-03-10 17:30:58.000000 imscript-0.6/src/warp.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      780 2017-10-23 14:34:44.000000 imscript-0.6/src/xfopen.c
--rw-rw-r--   0 coco      (1000) coco      (1000)      847 2022-07-13 12:24:19.000000 imscript-0.6/src/xmalloc.c
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:26:35.979080 imscript-0.7/
+-rw-rw-r--   0 coco      (1000) coco      (1000)    41635 2022-05-24 08:55:55.000000 imscript-0.7/.deps.mk
+-rw-rw-r--   0 coco      (1000) coco      (1000)       76 2023-06-01 12:58:57.000000 imscript-0.7/MANIFEST.in
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6264 2023-06-01 15:24:46.000000 imscript-0.7/Makefile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 15:26:35.979080 imscript-0.7/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.7/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:26:35.963080 imscript-0.7/imscript.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-06-01 15:26:35.000000 imscript-0.7/imscript.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2043 2023-06-01 15:26:35.000000 imscript-0.7/imscript.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 15:26:35.000000 imscript-0.7/imscript.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-01 15:26:35.000000 imscript-0.7/imscript.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-01 15:26:35.979080 imscript-0.7/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      806 2023-06-01 15:26:31.000000 imscript-0.7/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-01 15:26:35.979080 imscript-0.7/src/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      911 2017-10-23 14:34:44.000000 imscript-0.7/src/abstract_dsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      689 2017-10-23 14:34:44.000000 imscript-0.7/src/abstract_dsf.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5374 2017-10-23 14:34:44.000000 imscript-0.7/src/abstract_heap.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8946 2022-11-07 09:50:33.000000 imscript-0.7/src/amle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2129 2018-02-16 16:28:06.000000 imscript-0.7/src/autotrim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4987 2019-05-07 13:07:56.000000 imscript-0.7/src/backflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      825 2022-02-25 16:40:51.000000 imscript-0.7/src/bandslice.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5426 2022-11-07 09:50:33.000000 imscript-0.7/src/bdint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2510 2017-10-23 14:34:44.000000 imscript-0.7/src/bicubic.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1471 2017-10-23 14:34:44.000000 imscript-0.7/src/bicubic_gray.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3011 2017-10-23 14:34:44.000000 imscript-0.7/src/bilinear_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14174 2023-05-16 09:57:29.000000 imscript-0.7/src/blur.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     9431 2018-02-16 16:26:37.000000 imscript-0.7/src/bmms.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5726 2021-04-23 16:53:33.000000 imscript-0.7/src/carve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    18033 2018-12-02 15:33:58.000000 imscript-0.7/src/ccproc.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      783 2017-10-23 14:34:44.000000 imscript-0.7/src/ccproc.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2529 2017-10-23 14:34:44.000000 imscript-0.7/src/censust.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7642 2019-12-18 13:54:29.000000 imscript-0.7/src/cleant_cgpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2238 2017-11-12 08:49:58.000000 imscript-0.7/src/colorcoordsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4044 2017-11-24 18:26:29.000000 imscript-0.7/src/colormatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14726 2022-11-07 09:50:33.000000 imscript-0.7/src/contihist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1535 2018-04-25 10:33:08.000000 imscript-0.7/src/crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      141 2020-04-06 13:26:01.000000 imscript-0.7/src/d5.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13607 2018-02-16 16:03:22.000000 imscript-0.7/src/dataconv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2113 2017-10-23 14:34:44.000000 imscript-0.7/src/dct.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1956 2017-10-23 14:34:44.000000 imscript-0.7/src/dht.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5142 2022-11-02 07:40:05.000000 imscript-0.7/src/dither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5017 2020-01-10 14:33:49.000000 imscript-0.7/src/downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3508 2019-07-16 11:46:25.000000 imscript-0.7/src/drawsegment.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2448 2017-10-23 14:34:44.000000 imscript-0.7/src/drawtriangle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2591 2018-11-17 18:44:45.000000 imscript-0.7/src/eucdist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8492 2017-10-23 14:34:44.000000 imscript-0.7/src/exterior_algebra.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1794 2017-10-23 14:34:44.000000 imscript-0.7/src/extrapolators.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1628 2022-11-07 15:14:20.000000 imscript-0.7/src/fail.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1418 2018-02-16 16:27:35.000000 imscript-0.7/src/fancy_crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3506 2018-02-16 16:27:51.000000 imscript-0.7/src/fancy_downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    20717 2022-07-13 12:27:58.000000 imscript-0.7/src/fancy_image.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4280 2018-10-19 07:13:31.000000 imscript-0.7/src/fancy_image.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7059 2023-04-07 10:19:22.000000 imscript-0.7/src/fft.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1379 2017-10-23 14:34:44.000000 imscript-0.7/src/fftshift.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    84778 2021-06-03 13:20:54.000000 imscript-0.7/src/flambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3235 2018-07-10 14:32:43.000000 imscript-0.7/src/flowarrows.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3618 2018-02-16 16:16:06.000000 imscript-0.7/src/flowinv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24129 2023-03-20 09:45:46.000000 imscript-0.7/src/fontu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    32612 2021-06-28 07:40:10.000000 imscript-0.7/src/geomedian.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1604 2021-07-23 15:12:25.000000 imscript-0.7/src/getbands.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4854 2019-04-15 16:46:40.000000 imscript-0.7/src/getpixel.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5688 2022-11-02 07:40:05.000000 imscript-0.7/src/ghisto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8043 2018-01-03 11:41:10.000000 imscript-0.7/src/gntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1702 2017-10-23 14:34:44.000000 imscript-0.7/src/gram_schmidt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3144 2017-10-23 14:34:44.000000 imscript-0.7/src/grid.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3798 2018-03-22 08:54:00.000000 imscript-0.7/src/heatd.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1127 2018-02-16 18:36:16.000000 imscript-0.7/src/help_stuff.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2848 2017-10-23 14:34:44.000000 imscript-0.7/src/homographies.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6286 2022-02-23 15:28:45.000000 imscript-0.7/src/homwarp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1039 2018-02-07 17:22:02.000000 imscript-0.7/src/idump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   183486 2022-11-24 17:47:57.000000 imscript-0.7/src/iio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8888 2022-05-24 10:44:02.000000 imscript-0.7/src/iio.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3023 2023-01-23 08:50:42.000000 imscript-0.7/src/iion.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      626 2020-02-07 12:37:20.000000 imscript-0.7/src/iion_int.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      753 2022-11-07 09:50:33.000000 imscript-0.7/src/iion_pure.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      824 2017-10-23 14:34:44.000000 imscript-0.7/src/iion_u16.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      253 2021-03-16 15:08:51.000000 imscript-0.7/src/im.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5683 2020-01-10 14:32:38.000000 imscript-0.7/src/imflip.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      338 2020-01-30 09:53:05.000000 imscript-0.7/src/imhalve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23117 2020-01-10 14:32:44.000000 imscript-0.7/src/imprintf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2968 2021-06-15 10:19:21.000000 imscript-0.7/src/linalg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3661 2022-11-02 07:40:05.000000 imscript-0.7/src/lrcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6290 2018-02-16 16:14:16.000000 imscript-0.7/src/marching_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2962 2017-10-23 14:34:44.000000 imscript-0.7/src/marching_squares.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7313 2019-01-08 11:10:02.000000 imscript-0.7/src/mdither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7482 2019-01-08 11:10:15.000000 imscript-0.7/src/mdither2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7327 2018-11-23 08:20:02.000000 imscript-0.7/src/mdither3.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      193 2017-11-30 11:51:08.000000 imscript-0.7/src/means.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6215 2017-11-01 15:45:05.000000 imscript-0.7/src/mediator.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1756 2017-10-23 14:34:44.000000 imscript-0.7/src/minicg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    11894 2018-07-10 14:32:17.000000 imscript-0.7/src/modes_detector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17399 2022-11-07 14:49:50.000000 imscript-0.7/src/moistiv_epipolar.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15593 2023-02-16 15:39:37.000000 imscript-0.7/src/morsi.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7493 2022-11-02 08:49:14.000000 imscript-0.7/src/nnint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1938 2017-12-30 15:31:26.000000 imscript-0.7/src/nonmaxsup.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      765 2017-10-23 14:34:44.000000 imscript-0.7/src/ntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      162 2017-12-12 13:31:10.000000 imscript-0.7/src/numbersio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12436 2017-10-23 14:34:44.000000 imscript-0.7/src/ok_list.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17774 2023-01-24 10:59:47.000000 imscript-0.7/src/palette.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4036 2020-12-06 18:05:01.000000 imscript-0.7/src/parsenumbers.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1252 2017-11-13 14:55:57.000000 imscript-0.7/src/pickopt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      450 2020-02-13 08:44:15.000000 imscript-0.7/src/pixdump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   104894 2023-05-24 13:57:34.000000 imscript-0.7/src/plambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4668 2021-06-23 14:55:11.000000 imscript-0.7/src/points.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8894 2020-03-09 14:57:59.000000 imscript-0.7/src/ppsmooth.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29708 2021-12-09 13:36:31.000000 imscript-0.7/src/pview.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    96888 2021-06-14 15:31:43.000000 imscript-0.7/src/pλ.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5168 2022-04-21 08:24:03.000000 imscript-0.7/src/qauto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2227 2022-11-02 08:48:01.000000 imscript-0.7/src/qeasy.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3944 2023-02-21 16:29:17.000000 imscript-0.7/src/random.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17472 2017-10-23 14:34:44.000000 imscript-0.7/src/ransac.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24327 2019-05-07 10:03:01.000000 imscript-0.7/src/ransac_cases.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1265 2018-05-31 18:07:33.000000 imscript-0.7/src/redim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4984 2017-10-23 14:34:44.000000 imscript-0.7/src/registration.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    21672 2023-03-20 12:53:49.000000 imscript-0.7/src/rpc2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6501 2019-02-23 19:54:59.000000 imscript-0.7/src/rpcfit33.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    11740 2023-05-24 13:58:13.000000 imscript-0.7/src/rpctk.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12960 2019-02-08 09:45:19.000000 imscript-0.7/src/rpctk_old.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      460 2017-10-23 14:34:44.000000 imscript-0.7/src/seconds.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      464 2023-04-18 11:08:49.000000 imscript-0.7/src/setpixel.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    40509 2022-11-07 15:00:57.000000 imscript-0.7/src/siftie.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15912 2017-10-23 14:34:44.000000 imscript-0.7/src/siftu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13108 2022-11-07 09:50:33.000000 imscript-0.7/src/simpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1349 2018-08-24 10:55:52.000000 imscript-0.7/src/smapa.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)    10832 2018-02-16 16:10:48.000000 imscript-0.7/src/spline.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6230 2020-12-04 11:17:12.000000 imscript-0.7/src/srmatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5886 2017-10-23 14:34:44.000000 imscript-0.7/src/strt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1376 2017-10-23 14:34:44.000000 imscript-0.7/src/synflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29109 2018-02-16 16:35:04.000000 imscript-0.7/src/synflow_core.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3652 2022-11-02 07:40:05.000000 imscript-0.7/src/tbcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23780 2022-11-07 15:01:37.000000 imscript-0.7/src/tiff_octaves_rw.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    73306 2022-11-07 14:55:30.000000 imscript-0.7/src/tiffu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4488 2018-07-11 18:56:13.000000 imscript-0.7/src/upsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17626 2021-07-19 17:20:01.000000 imscript-0.7/src/veco.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14287 2020-01-10 14:33:16.000000 imscript-0.7/src/vecoh.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7890 2020-01-10 14:33:18.000000 imscript-0.7/src/vecov.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      482 2018-01-11 09:37:54.000000 imscript-0.7/src/vector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8319 2022-12-15 15:23:14.000000 imscript-0.7/src/viewflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    37651 2017-10-23 14:34:44.000000 imscript-0.7/src/vvector.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5234 2018-03-10 17:30:58.000000 imscript-0.7/src/warp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      780 2017-10-23 14:34:44.000000 imscript-0.7/src/xfopen.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      847 2022-07-13 12:24:19.000000 imscript-0.7/src/xmalloc.c
```

### Comparing `imscript-0.6/.deps.mk` & `imscript-0.7/.deps.mk`

 * *Files identical despite different names*

### Comparing `imscript-0.6/Makefile` & `imscript-0.7/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # CONFIGURABLE DEPENDENCIES
 # XXX: comment (or not) the following lines to disable (enable) image formats
 # Note: just comment the lines, do NOT change the ones to zeros!
 
 ENABLE_PNG  = 1
 ENABLE_TIFF = 1
 ENABLE_JPEG = 1
-ENABLE_WEBP = 1
-ENABLE_HEIF = 1
-ENABLE_PGSL = 1
+#ENABLE_WEBP = 1
+#ENABLE_HEIF = 1
+#ENABLE_PGSL = 1
 
 # CAVEAT: if you want to use HDF5, make sure that no "mpich" packages
 # are installed on your computer.  If they are, all programs that link
 # to libdf5 become really slow due to dynamic linking initialization.
 #
 #ENABLE_HDF5 = 1
```

### Comparing `imscript-0.6/imscript.egg-info/SOURCES.txt` & `imscript-0.7/imscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imscript-0.6/setup.py` & `imscript-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 		os.system("make -j bin/plambda bin/qauto bin/morsi")
 		install.run(self)
 
 
 import setuptools
 setuptools.setup(
 	name = "imscript",
-	version = "0.6",
+	version = "0.7",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@fastmail.com",
 	description = "Image Processing with Unix Pipes",
 	url = "https://github.com/mnhrdt/imscript",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

### Comparing `imscript-0.6/src/abstract_dsf.c` & `imscript-0.7/src/abstract_dsf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/abstract_dsf.h` & `imscript-0.7/src/abstract_dsf.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/abstract_heap.h` & `imscript-0.7/src/abstract_heap.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/amle.c` & `imscript-0.7/src/amle.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/autotrim.c` & `imscript-0.7/src/autotrim.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/backflow.c` & `imscript-0.7/src/backflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bandslice.c` & `imscript-0.7/src/bandslice.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bdint.c` & `imscript-0.7/src/bdint.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bicubic.c` & `imscript-0.7/src/bicubic.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bicubic_gray.c` & `imscript-0.7/src/bicubic_gray.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bilinear_interpolation.c` & `imscript-0.7/src/bilinear_interpolation.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/blur.c` & `imscript-0.7/src/blur.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/bmms.c` & `imscript-0.7/src/bmms.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/carve.c` & `imscript-0.7/src/carve.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ccproc.c` & `imscript-0.7/src/ccproc.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ccproc.h` & `imscript-0.7/src/ccproc.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/censust.c` & `imscript-0.7/src/censust.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/cleant_cgpois.c` & `imscript-0.7/src/cleant_cgpois.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/colorcoordsf.c` & `imscript-0.7/src/colorcoordsf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/colormatch.c` & `imscript-0.7/src/colormatch.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/contihist.c` & `imscript-0.7/src/contihist.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/crop.c` & `imscript-0.7/src/crop.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/dataconv.c` & `imscript-0.7/src/dataconv.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/dct.c` & `imscript-0.7/src/dct.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/dht.c` & `imscript-0.7/src/dht.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/dither.c` & `imscript-0.7/src/dither.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/downsa.c` & `imscript-0.7/src/downsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/drawsegment.c` & `imscript-0.7/src/drawsegment.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/drawtriangle.c` & `imscript-0.7/src/drawtriangle.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/eucdist.c` & `imscript-0.7/src/eucdist.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/exterior_algebra.c` & `imscript-0.7/src/exterior_algebra.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/extrapolators.c` & `imscript-0.7/src/extrapolators.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fail.c` & `imscript-0.7/src/fail.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fancy_crop.c` & `imscript-0.7/src/fancy_crop.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fancy_downsa.c` & `imscript-0.7/src/fancy_downsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fancy_image.c` & `imscript-0.7/src/fancy_image.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fancy_image.h` & `imscript-0.7/src/fancy_image.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fft.c` & `imscript-0.7/src/fft.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fftshift.c` & `imscript-0.7/src/fftshift.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/flambda.c` & `imscript-0.7/src/flambda.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/flowarrows.c` & `imscript-0.7/src/flowarrows.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/flowinv.c` & `imscript-0.7/src/flowinv.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/fontu.c` & `imscript-0.7/src/fontu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/geomedian.c` & `imscript-0.7/src/geomedian.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/getbands.c` & `imscript-0.7/src/getbands.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/getpixel.c` & `imscript-0.7/src/getpixel.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ghisto.c` & `imscript-0.7/src/ghisto.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/gntiply.c` & `imscript-0.7/src/gntiply.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/gram_schmidt.c` & `imscript-0.7/src/gram_schmidt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/grid.c` & `imscript-0.7/src/grid.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/heatd.c` & `imscript-0.7/src/heatd.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/help_stuff.c` & `imscript-0.7/src/help_stuff.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/homographies.c` & `imscript-0.7/src/homographies.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/homwarp.c` & `imscript-0.7/src/homwarp.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/idump.c` & `imscript-0.7/src/idump.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iio.c` & `imscript-0.7/src/iio.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iio.h` & `imscript-0.7/src/iio.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iion.c` & `imscript-0.7/src/iion.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iion_int.c` & `imscript-0.7/src/iion_int.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iion_pure.c` & `imscript-0.7/src/iion_pure.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/iion_u16.c` & `imscript-0.7/src/iion_u16.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/imflip.c` & `imscript-0.7/src/imflip.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/imprintf.c` & `imscript-0.7/src/imprintf.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/linalg.c` & `imscript-0.7/src/linalg.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/lrcat.c` & `imscript-0.7/src/lrcat.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/marching_interpolation.c` & `imscript-0.7/src/marching_interpolation.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/marching_squares.c` & `imscript-0.7/src/marching_squares.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/mdither.c` & `imscript-0.7/src/mdither.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/mdither2.c` & `imscript-0.7/src/mdither2.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/mdither3.c` & `imscript-0.7/src/mdither3.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/mediator.c` & `imscript-0.7/src/mediator.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/minicg.c` & `imscript-0.7/src/minicg.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/modes_detector.c` & `imscript-0.7/src/modes_detector.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/moistiv_epipolar.c` & `imscript-0.7/src/moistiv_epipolar.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/morsi.c` & `imscript-0.7/src/morsi.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/nnint.c` & `imscript-0.7/src/nnint.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/nonmaxsup.c` & `imscript-0.7/src/nonmaxsup.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ntiply.c` & `imscript-0.7/src/ntiply.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ok_list.c` & `imscript-0.7/src/ok_list.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/palette.c` & `imscript-0.7/src/palette.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/parsenumbers.c` & `imscript-0.7/src/parsenumbers.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/pickopt.c` & `imscript-0.7/src/pickopt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/plambda.c` & `imscript-0.7/src/plambda.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/points.c` & `imscript-0.7/src/points.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ppsmooth.c` & `imscript-0.7/src/ppsmooth.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/pview.c` & `imscript-0.7/src/pview.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/pλ.c` & `imscript-0.7/src/pλ.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/qauto.c` & `imscript-0.7/src/qauto.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/qeasy.c` & `imscript-0.7/src/qeasy.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/random.c` & `imscript-0.7/src/random.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ransac.c` & `imscript-0.7/src/ransac.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/ransac_cases.c` & `imscript-0.7/src/ransac_cases.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/redim.c` & `imscript-0.7/src/redim.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/registration.c` & `imscript-0.7/src/registration.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/rpc2.c` & `imscript-0.7/src/rpc2.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/rpcfit33.c` & `imscript-0.7/src/rpcfit33.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/rpctk.c` & `imscript-0.7/src/rpctk.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/rpctk_old.c` & `imscript-0.7/src/rpctk_old.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/siftie.c` & `imscript-0.7/src/siftie.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/siftu.c` & `imscript-0.7/src/siftu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/simpois.c` & `imscript-0.7/src/simpois.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/smapa.h` & `imscript-0.7/src/smapa.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/spline.c` & `imscript-0.7/src/spline.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/srmatch.c` & `imscript-0.7/src/srmatch.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/strt.c` & `imscript-0.7/src/strt.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/synflow.c` & `imscript-0.7/src/synflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/synflow_core.c` & `imscript-0.7/src/synflow_core.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/tbcat.c` & `imscript-0.7/src/tbcat.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/tiff_octaves_rw.c` & `imscript-0.7/src/tiff_octaves_rw.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/tiffu.c` & `imscript-0.7/src/tiffu.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/upsa.c` & `imscript-0.7/src/upsa.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/veco.c` & `imscript-0.7/src/veco.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/vecoh.c` & `imscript-0.7/src/vecoh.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/vecov.c` & `imscript-0.7/src/vecov.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/viewflow.c` & `imscript-0.7/src/viewflow.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/vvector.h` & `imscript-0.7/src/vvector.h`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/warp.c` & `imscript-0.7/src/warp.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/xfopen.c` & `imscript-0.7/src/xfopen.c`

 * *Files identical despite different names*

### Comparing `imscript-0.6/src/xmalloc.c` & `imscript-0.7/src/xmalloc.c`

 * *Files identical despite different names*

