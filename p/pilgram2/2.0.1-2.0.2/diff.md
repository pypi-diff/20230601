# Comparing `tmp/pilgram2-2.0.1.tar.gz` & `tmp/pilgram2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilgram2-2.0.1.tar", max compression
+gzip compressed data, was "pilgram2-2.0.2.tar", max compression
```

## Comparing `pilgram2-2.0.1.tar` & `pilgram2-2.0.2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11558 2023-04-19 04:50:10.095416 pilgram2-2.0.1/LICENSE
--rw-r--r--   0        0        0     1021 2023-05-31 18:38:25.638514 pilgram2-2.0.1/pilgram2/_1977.py
--rw-r--r--   0        0        0     2634 2023-05-31 18:38:25.638514 pilgram2-2.0.1/pilgram2/__init__.py
--rw-r--r--   0        0        0      617 2023-06-01 05:57:04.772670 pilgram2-2.0.1/pilgram2/_version.py
--rw-r--r--   0        0        0     1141 2023-05-31 18:38:25.639516 pilgram2-2.0.1/pilgram2/aden.py
--rw-r--r--   0        0        0     1005 2023-05-31 18:38:25.639516 pilgram2-2.0.1/pilgram2/amaro.py
--rw-r--r--   0        0        0     1002 2023-05-31 18:38:25.639516 pilgram2-2.0.1/pilgram2/ashby.py
--rw-r--r--   0        0        0      988 2023-05-31 18:38:25.640515 pilgram2-2.0.1/pilgram2/brannan.py
--rw-r--r--   0        0        0     1236 2023-05-31 18:38:25.640515 pilgram2-2.0.1/pilgram2/brooklyn.py
--rw-r--r--   0        0        0     1074 2023-05-31 18:38:25.640515 pilgram2-2.0.1/pilgram2/charmes.py
--rw-r--r--   0        0        0      998 2023-05-31 18:38:25.640515 pilgram2-2.0.1/pilgram2/clarendon.py
--rw-r--r--   0        0        0     1070 2023-05-31 18:38:25.641514 pilgram2-2.0.1/pilgram2/crema.py
--rw-r--r--   0        0        0      993 2023-05-31 18:38:25.641514 pilgram2-2.0.1/pilgram2/css/__init__.py
--rw-r--r--   0        0        0     1580 2023-05-31 18:38:25.641514 pilgram2-2.0.1/pilgram2/css/blending/__init__.py
--rw-r--r--   0        0        0     3696 2023-05-31 18:38:25.642514 pilgram2-2.0.1/pilgram2/css/blending/alpha.py
--rw-r--r--   0        0        0     2235 2023-05-31 18:38:25.642514 pilgram2-2.0.1/pilgram2/css/blending/color.py
--rw-r--r--   0        0        0     1989 2023-05-31 18:38:25.642514 pilgram2-2.0.1/pilgram2/css/blending/color_burn.py
--rw-r--r--   0        0        0     2137 2023-05-31 18:38:25.643510 pilgram2-2.0.1/pilgram2/css/blending/color_dodge.py
--rw-r--r--   0        0        0     1378 2023-05-31 18:38:25.643510 pilgram2-2.0.1/pilgram2/css/blending/darken.py
--rw-r--r--   0        0        0     1432 2023-05-31 18:38:25.643510 pilgram2-2.0.1/pilgram2/css/blending/difference.py
--rw-r--r--   0        0        0     1558 2023-05-31 18:38:25.643510 pilgram2-2.0.1/pilgram2/css/blending/exclusion.py
--rw-r--r--   0        0        0     1956 2023-05-31 18:38:25.644511 pilgram2-2.0.1/pilgram2/css/blending/hard_light.py
--rw-r--r--   0        0        0     2285 2023-05-31 18:38:25.644511 pilgram2-2.0.1/pilgram2/css/blending/hue.py
--rw-r--r--   0        0        0     1386 2023-05-31 18:38:25.644511 pilgram2-2.0.1/pilgram2/css/blending/lighten.py
--rw-r--r--   0        0        0     1424 2023-05-31 18:38:25.645510 pilgram2-2.0.1/pilgram2/css/blending/multiply.py
--rw-r--r--   0        0        0     6124 2023-05-31 18:38:25.645510 pilgram2-2.0.1/pilgram2/css/blending/nonseparable.py
--rw-r--r--   0        0        0     1315 2023-05-31 18:38:25.645510 pilgram2-2.0.1/pilgram2/css/blending/normal.py
--rw-r--r--   0        0        0     1113 2023-05-31 18:38:25.646512 pilgram2-2.0.1/pilgram2/css/blending/overlay.py
--rw-r--r--   0        0        0     1481 2023-05-31 18:38:25.646512 pilgram2-2.0.1/pilgram2/css/blending/screen.py
--rw-r--r--   0        0        0     2606 2023-05-31 18:38:25.646512 pilgram2-2.0.1/pilgram2/css/blending/soft_light.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.647512 pilgram2-2.0.1/pilgram2/css/blending/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-05-31 18:38:25.647512 pilgram2-2.0.1/pilgram2/css/blending/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-31 18:38:25.647512 pilgram2-2.0.1/pilgram2/css/blending/tests/helpers/alpha_support.py
--rw-r--r--   0        0        0     4250 2023-05-31 18:38:25.648511 pilgram2-2.0.1/pilgram2/css/blending/tests/test_alpha.py
--rw-r--r--   0        0        0     1384 2023-05-31 18:38:25.648511 pilgram2-2.0.1/pilgram2/css/blending/tests/test_color.py
--rw-r--r--   0        0        0     1408 2023-05-31 18:38:25.648511 pilgram2-2.0.1/pilgram2/css/blending/tests/test_color_burn.py
--rw-r--r--   0        0        0     1419 2023-05-31 18:38:25.649515 pilgram2-2.0.1/pilgram2/css/blending/tests/test_color_dodge.py
--rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.649515 pilgram2-2.0.1/pilgram2/css/blending/tests/test_darken.py
--rw-r--r--   0        0        0     1061 2023-05-31 18:38:25.649515 pilgram2-2.0.1/pilgram2/css/blending/tests/test_difference.py
--rw-r--r--   0        0        0     1412 2023-05-31 18:38:25.650510 pilgram2-2.0.1/pilgram2/css/blending/tests/test_exclusion.py
--rw-r--r--   0        0        0     1434 2023-05-31 18:38:25.650510 pilgram2-2.0.1/pilgram2/css/blending/tests/test_hard_light.py
--rw-r--r--   0        0        0     1863 2023-05-31 18:38:25.650510 pilgram2-2.0.1/pilgram2/css/blending/tests/test_hue.py
--rw-r--r--   0        0        0     1049 2023-05-31 18:38:25.650510 pilgram2-2.0.1/pilgram2/css/blending/tests/test_lighten.py
--rw-r--r--   0        0        0     1053 2023-05-31 18:38:25.651513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_multiply.py
--rw-r--r--   0        0        0     5166 2023-05-31 18:38:25.651513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_nonseparable.py
--rw-r--r--   0        0        0     1529 2023-05-31 18:38:25.651513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_normal.py
--rw-r--r--   0        0        0     1654 2023-05-31 18:38:25.652513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_overlay.py
--rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.652513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_screen.py
--rw-r--r--   0        0        0     1413 2023-05-31 18:38:25.652513 pilgram2-2.0.1/pilgram2/css/blending/tests/test_soft_light.py
--rw-r--r--   0        0        0     1304 2023-05-31 18:38:25.653514 pilgram2-2.0.1/pilgram2/css/brightness.py
--rw-r--r--   0        0        0     1473 2023-05-31 18:38:25.653514 pilgram2-2.0.1/pilgram2/css/contrast.py
--rw-r--r--   0        0        0     2036 2023-05-31 18:38:25.653514 pilgram2-2.0.1/pilgram2/css/grayscale.py
--rw-r--r--   0        0        0     2578 2023-05-31 18:38:25.653514 pilgram2-2.0.1/pilgram2/css/hue_rotate.py
--rw-r--r--   0        0        0     2019 2023-05-31 18:38:25.654512 pilgram2-2.0.1/pilgram2/css/saturate.py
--rw-r--r--   0        0        0     2024 2023-05-31 18:38:25.654512 pilgram2-2.0.1/pilgram2/css/sepia.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.654512 pilgram2-2.0.1/pilgram2/css/tests/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-31 18:38:25.654512 pilgram2-2.0.1/pilgram2/css/tests/test_brightness.py
--rw-r--r--   0        0        0     2401 2023-05-31 18:38:25.655512 pilgram2-2.0.1/pilgram2/css/tests/test_contrast.py
--rw-r--r--   0        0        0     2313 2023-05-31 18:38:25.655512 pilgram2-2.0.1/pilgram2/css/tests/test_grayscale.py
--rw-r--r--   0        0        0     2741 2023-05-31 18:38:25.655512 pilgram2-2.0.1/pilgram2/css/tests/test_hue_rotate.py
--rw-r--r--   0        0        0     2321 2023-05-31 18:38:25.655512 pilgram2-2.0.1/pilgram2/css/tests/test_saturate.py
--rw-r--r--   0        0        0     2170 2023-05-31 18:38:25.656514 pilgram2-2.0.1/pilgram2/css/tests/test_sepia.py
--rw-r--r--   0        0        0      920 2023-05-31 18:38:25.656514 pilgram2-2.0.1/pilgram2/dogpatch.py
--rw-r--r--   0        0        0     1043 2023-05-31 18:38:25.656514 pilgram2-2.0.1/pilgram2/earlybird.py
--rw-r--r--   0        0        0      996 2023-05-31 18:38:25.657513 pilgram2-2.0.1/pilgram2/gingham.py
--rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.657513 pilgram2-2.0.1/pilgram2/ginza.py
--rw-r--r--   0        0        0     1157 2023-05-31 18:38:25.657513 pilgram2-2.0.1/pilgram2/hefe.py
--rw-r--r--   0        0        0     1040 2023-05-31 18:38:25.657513 pilgram2-2.0.1/pilgram2/helena.py
--rw-r--r--   0        0        0     1129 2023-05-31 18:38:25.658513 pilgram2-2.0.1/pilgram2/hudson.py
--rw-r--r--   0        0        0      960 2023-05-31 18:38:25.658513 pilgram2-2.0.1/pilgram2/inkwell.py
--rw-r--r--   0        0        0     1036 2023-05-31 18:38:25.658513 pilgram2-2.0.1/pilgram2/juno.py
--rw-r--r--   0        0        0     1011 2023-05-31 18:38:25.659513 pilgram2-2.0.1/pilgram2/kelvin.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.659513 pilgram2-2.0.1/pilgram2/lark.py
--rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.659513 pilgram2-2.0.1/pilgram2/lofi.py
--rw-r--r--   0        0        0     1037 2023-05-31 18:38:25.659513 pilgram2-2.0.1/pilgram2/ludwig.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.660513 pilgram2-2.0.1/pilgram2/maven.py
--rw-r--r--   0        0        0     1519 2023-05-31 18:38:25.660513 pilgram2-2.0.1/pilgram2/mayfair.py
--rw-r--r--   0        0        0     1103 2023-05-31 18:38:25.660513 pilgram2-2.0.1/pilgram2/moon.py
--rw-r--r--   0        0        0     1156 2023-05-31 18:38:25.661513 pilgram2-2.0.1/pilgram2/nashville.py
--rw-r--r--   0        0        0     1029 2023-05-31 18:38:25.661513 pilgram2-2.0.1/pilgram2/perpetua.py
--rw-r--r--   0        0        0     1047 2023-05-31 18:38:25.661513 pilgram2-2.0.1/pilgram2/poprocket.py
--rw-r--r--   0        0        0     1124 2023-05-31 18:38:25.661513 pilgram2-2.0.1/pilgram2/reyes.py
--rw-r--r--   0        0        0     1561 2023-05-31 18:38:25.662514 pilgram2-2.0.1/pilgram2/rise.py
--rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.662514 pilgram2-2.0.1/pilgram2/sierra.py
--rw-r--r--   0        0        0      953 2023-05-31 18:38:25.662514 pilgram2-2.0.1/pilgram2/skyline.py
--rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.662514 pilgram2-2.0.1/pilgram2/slumber.py
--rw-r--r--   0        0        0     1033 2023-05-31 18:38:25.663513 pilgram2-2.0.1/pilgram2/stinson.py
--rw-r--r--   0        0        0     1127 2023-05-31 18:38:25.663513 pilgram2-2.0.1/pilgram2/sutro.py
--rw-r--r--   0        0        0      592 2023-05-31 18:38:25.664526 pilgram2-2.0.1/pilgram2/tests/__init__.py
--rw-r--r--   0        0        0    63895 2023-05-31 18:38:25.664526 pilgram2-2.0.1/pilgram2/tests/assets/mtjimba.jpg
--rw-r--r--   0        0        0      840 2023-05-31 18:38:25.665525 pilgram2-2.0.1/pilgram2/tests/test_1977.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.1/pilgram2/tests/test_aden.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.1/pilgram2/tests/test_amaro.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.666524 pilgram2-2.0.1/pilgram2/tests/test_ashby.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.666524 pilgram2-2.0.1/pilgram2/tests/test_brannan.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.666524 pilgram2-2.0.1/pilgram2/tests/test_brooklyn.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.667523 pilgram2-2.0.1/pilgram2/tests/test_charmes.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.667523 pilgram2-2.0.1/pilgram2/tests/test_clarendon.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.668521 pilgram2-2.0.1/pilgram2/tests/test_crema.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.1/pilgram2/tests/test_dogpatch.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.668521 pilgram2-2.0.1/pilgram2/tests/test_earlybird.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.1/pilgram2/tests/test_gingham.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.669524 pilgram2-2.0.1/pilgram2/tests/test_ginza.py
--rw-r--r--   0        0        0      832 2023-05-31 18:38:25.669524 pilgram2-2.0.1/pilgram2/tests/test_hefe.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.669524 pilgram2-2.0.1/pilgram2/tests/test_helena.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.1/pilgram2/tests/test_hudson.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.670522 pilgram2-2.0.1/pilgram2/tests/test_inkwell.py
--rw-r--r--   0        0        0      832 2023-05-31 18:38:25.670522 pilgram2-2.0.1/pilgram2/tests/test_juno.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.1/pilgram2/tests/test_kelvin.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.1/pilgram2/tests/test_lark.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.1/pilgram2/tests/test_lofi.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.671522 pilgram2-2.0.1/pilgram2/tests/test_ludwig.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.672523 pilgram2-2.0.1/pilgram2/tests/test_maven.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.672523 pilgram2-2.0.1/pilgram2/tests/test_mayfair.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.672523 pilgram2-2.0.1/pilgram2/tests/test_moon.py
--rw-r--r--   0        0        0      862 2023-05-31 18:38:25.672523 pilgram2-2.0.1/pilgram2/tests/test_nashville.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.1/pilgram2/tests/test_perpetua.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.1/pilgram2/tests/test_poprocket.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.673522 pilgram2-2.0.1/pilgram2/tests/test_reyes.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.673522 pilgram2-2.0.1/pilgram2/tests/test_rise.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.674524 pilgram2-2.0.1/pilgram2/tests/test_sierra.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.674524 pilgram2-2.0.1/pilgram2/tests/test_skyline.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.674524 pilgram2-2.0.1/pilgram2/tests/test_slumber.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.1/pilgram2/tests/test_stinson.py
--rw-r--r--   0        0        0      837 2023-05-31 18:38:25.675526 pilgram2-2.0.1/pilgram2/tests/test_sutro.py
--rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.1/pilgram2/tests/test_toaster.py
--rw-r--r--   0        0        0      857 2023-05-31 18:38:25.676521 pilgram2-2.0.1/pilgram2/tests/test_valencia.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.1/pilgram2/tests/test_walden.py
--rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.1/pilgram2/tests/test_willow.py
--rw-r--r--   0        0        0      842 2023-05-31 18:38:25.677524 pilgram2-2.0.1/pilgram2/tests/test_xpro2.py
--rw-r--r--   0        0        0     1013 2023-05-31 18:38:25.677524 pilgram2-2.0.1/pilgram2/toaster.py
--rw-r--r--   0        0        0     1278 2023-05-31 18:38:25.677524 pilgram2-2.0.1/pilgram2/util/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.677524 pilgram2-2.0.1/pilgram2/util/add.py
--rw-r--r--   0        0        0     1010 2023-05-31 18:38:25.678524 pilgram2-2.0.1/pilgram2/util/apply_lut.py
--rw-r--r--   0        0        0      972 2023-05-31 18:38:25.679038 pilgram2-2.0.1/pilgram2/util/clip.py
--rw-r--r--   0        0        0     1439 2023-05-31 18:38:25.679038 pilgram2-2.0.1/pilgram2/util/fill.py
--rw-r--r--   0        0        0      899 2023-05-31 18:38:25.679038 pilgram2-2.0.1/pilgram2/util/invert.py
--rw-r--r--   0        0        0     2832 2023-05-31 18:38:25.679038 pilgram2-2.0.1/pilgram2/util/linear_gradient.py
--rw-r--r--   0        0        0      869 2023-05-31 18:38:25.680050 pilgram2-2.0.1/pilgram2/util/or_convert.py
--rw-r--r--   0        0        0     3801 2023-05-31 18:38:25.680050 pilgram2-2.0.1/pilgram2/util/radial_gradient.py
--rw-r--r--   0        0        0     1098 2023-05-31 18:38:25.680050 pilgram2-2.0.1/pilgram2/util/subtract.py
--rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.681046 pilgram2-2.0.1/pilgram2/util/tests/test_add.py
--rw-r--r--   0        0        0     1226 2023-05-31 18:38:25.681046 pilgram2-2.0.1/pilgram2/util/tests/test_apply_lut.py
--rw-r--r--   0        0        0     1122 2023-05-31 18:38:25.681046 pilgram2-2.0.1/pilgram2/util/tests/test_clip.py
--rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.682048 pilgram2-2.0.1/pilgram2/util/tests/test_fill.py
--rw-r--r--   0        0        0     1020 2023-05-31 18:38:25.682048 pilgram2-2.0.1/pilgram2/util/tests/test_invert.py
--rw-r--r--   0        0        0     2603 2023-05-31 18:38:25.682048 pilgram2-2.0.1/pilgram2/util/tests/test_linear_gradient.py
--rw-r--r--   0        0        0     1097 2023-05-31 18:38:25.683048 pilgram2-2.0.1/pilgram2/util/tests/test_or_convert.py
--rw-r--r--   0        0        0     4730 2023-05-31 18:38:25.683048 pilgram2-2.0.1/pilgram2/util/tests/test_radial_gradient.py
--rw-r--r--   0        0        0     1115 2023-05-31 18:38:25.683048 pilgram2-2.0.1/pilgram2/util/tests/test_subtract.py
--rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.683048 pilgram2-2.0.1/pilgram2/valencia.py
--rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.684047 pilgram2-2.0.1/pilgram2/walden.py
--rw-r--r--   0        0        0     1150 2023-05-31 18:38:25.684047 pilgram2-2.0.1/pilgram2/willow.py
--rw-r--r--   0        0        0     1344 2023-05-31 18:38:25.684047 pilgram2-2.0.1/pilgram2/xpro2.py
--rw-r--r--   0        0        0     2177 2023-06-01 05:57:06.334143 pilgram2-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3134 2023-05-31 19:10:30.206244 pilgram2-2.0.1/README.md
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pilgram2-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-04-19 04:50:10.095416 pilgram2-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1021 2023-05-31 18:38:25.638514 pilgram2-2.0.2/pilgram2/_1977.py
+-rw-r--r--   0        0        0     2634 2023-05-31 18:38:25.638514 pilgram2-2.0.2/pilgram2/__init__.py
+-rw-r--r--   0        0        0      617 2023-06-01 17:46:56.534914 pilgram2-2.0.2/pilgram2/_version.py
+-rw-r--r--   0        0        0     1141 2023-05-31 18:38:25.639516 pilgram2-2.0.2/pilgram2/aden.py
+-rw-r--r--   0        0        0     1005 2023-05-31 18:38:25.639516 pilgram2-2.0.2/pilgram2/amaro.py
+-rw-r--r--   0        0        0     1002 2023-05-31 18:38:25.639516 pilgram2-2.0.2/pilgram2/ashby.py
+-rw-r--r--   0        0        0      988 2023-05-31 18:38:25.640515 pilgram2-2.0.2/pilgram2/brannan.py
+-rw-r--r--   0        0        0     1236 2023-05-31 18:38:25.640515 pilgram2-2.0.2/pilgram2/brooklyn.py
+-rw-r--r--   0        0        0     1074 2023-05-31 18:38:25.640515 pilgram2-2.0.2/pilgram2/charmes.py
+-rw-r--r--   0        0        0      998 2023-05-31 18:38:25.640515 pilgram2-2.0.2/pilgram2/clarendon.py
+-rw-r--r--   0        0        0     1070 2023-05-31 18:38:25.641514 pilgram2-2.0.2/pilgram2/crema.py
+-rw-r--r--   0        0        0      993 2023-05-31 18:38:25.641514 pilgram2-2.0.2/pilgram2/css/__init__.py
+-rw-r--r--   0        0        0     1580 2023-05-31 18:38:25.641514 pilgram2-2.0.2/pilgram2/css/blending/__init__.py
+-rw-r--r--   0        0        0     3696 2023-05-31 18:38:25.642514 pilgram2-2.0.2/pilgram2/css/blending/alpha.py
+-rw-r--r--   0        0        0     2235 2023-05-31 18:38:25.642514 pilgram2-2.0.2/pilgram2/css/blending/color.py
+-rw-r--r--   0        0        0     1989 2023-05-31 18:38:25.642514 pilgram2-2.0.2/pilgram2/css/blending/color_burn.py
+-rw-r--r--   0        0        0     2137 2023-05-31 18:38:25.643510 pilgram2-2.0.2/pilgram2/css/blending/color_dodge.py
+-rw-r--r--   0        0        0     1378 2023-05-31 18:38:25.643510 pilgram2-2.0.2/pilgram2/css/blending/darken.py
+-rw-r--r--   0        0        0     1432 2023-05-31 18:38:25.643510 pilgram2-2.0.2/pilgram2/css/blending/difference.py
+-rw-r--r--   0        0        0     1558 2023-05-31 18:38:25.643510 pilgram2-2.0.2/pilgram2/css/blending/exclusion.py
+-rw-r--r--   0        0        0     1956 2023-05-31 18:38:25.644511 pilgram2-2.0.2/pilgram2/css/blending/hard_light.py
+-rw-r--r--   0        0        0     2285 2023-05-31 18:38:25.644511 pilgram2-2.0.2/pilgram2/css/blending/hue.py
+-rw-r--r--   0        0        0     1386 2023-05-31 18:38:25.644511 pilgram2-2.0.2/pilgram2/css/blending/lighten.py
+-rw-r--r--   0        0        0     1424 2023-05-31 18:38:25.645510 pilgram2-2.0.2/pilgram2/css/blending/multiply.py
+-rw-r--r--   0        0        0     6124 2023-05-31 18:38:25.645510 pilgram2-2.0.2/pilgram2/css/blending/nonseparable.py
+-rw-r--r--   0        0        0     1315 2023-05-31 18:38:25.645510 pilgram2-2.0.2/pilgram2/css/blending/normal.py
+-rw-r--r--   0        0        0     1113 2023-05-31 18:38:25.646512 pilgram2-2.0.2/pilgram2/css/blending/overlay.py
+-rw-r--r--   0        0        0     1481 2023-05-31 18:38:25.646512 pilgram2-2.0.2/pilgram2/css/blending/screen.py
+-rw-r--r--   0        0        0     2606 2023-05-31 18:38:25.646512 pilgram2-2.0.2/pilgram2/css/blending/soft_light.py
+-rw-r--r--   0        0        0      592 2023-05-31 18:38:25.647512 pilgram2-2.0.2/pilgram2/css/blending/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-31 18:38:25.647512 pilgram2-2.0.2/pilgram2/css/blending/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-31 18:38:25.647512 pilgram2-2.0.2/pilgram2/css/blending/tests/helpers/alpha_support.py
+-rw-r--r--   0        0        0     4250 2023-05-31 18:38:25.648511 pilgram2-2.0.2/pilgram2/css/blending/tests/test_alpha.py
+-rw-r--r--   0        0        0     1384 2023-05-31 18:38:25.648511 pilgram2-2.0.2/pilgram2/css/blending/tests/test_color.py
+-rw-r--r--   0        0        0     1408 2023-05-31 18:38:25.648511 pilgram2-2.0.2/pilgram2/css/blending/tests/test_color_burn.py
+-rw-r--r--   0        0        0     1419 2023-05-31 18:38:25.649515 pilgram2-2.0.2/pilgram2/css/blending/tests/test_color_dodge.py
+-rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.649515 pilgram2-2.0.2/pilgram2/css/blending/tests/test_darken.py
+-rw-r--r--   0        0        0     1061 2023-05-31 18:38:25.649515 pilgram2-2.0.2/pilgram2/css/blending/tests/test_difference.py
+-rw-r--r--   0        0        0     1412 2023-05-31 18:38:25.650510 pilgram2-2.0.2/pilgram2/css/blending/tests/test_exclusion.py
+-rw-r--r--   0        0        0     1434 2023-05-31 18:38:25.650510 pilgram2-2.0.2/pilgram2/css/blending/tests/test_hard_light.py
+-rw-r--r--   0        0        0     1863 2023-05-31 18:38:25.650510 pilgram2-2.0.2/pilgram2/css/blending/tests/test_hue.py
+-rw-r--r--   0        0        0     1049 2023-05-31 18:38:25.650510 pilgram2-2.0.2/pilgram2/css/blending/tests/test_lighten.py
+-rw-r--r--   0        0        0     1053 2023-05-31 18:38:25.651513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_multiply.py
+-rw-r--r--   0        0        0     5166 2023-05-31 18:38:25.651513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_nonseparable.py
+-rw-r--r--   0        0        0     1529 2023-05-31 18:38:25.651513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_normal.py
+-rw-r--r--   0        0        0     1654 2023-05-31 18:38:25.652513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_overlay.py
+-rw-r--r--   0        0        0     1045 2023-05-31 18:38:25.652513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_screen.py
+-rw-r--r--   0        0        0     1413 2023-05-31 18:38:25.652513 pilgram2-2.0.2/pilgram2/css/blending/tests/test_soft_light.py
+-rw-r--r--   0        0        0     1304 2023-05-31 18:38:25.653514 pilgram2-2.0.2/pilgram2/css/brightness.py
+-rw-r--r--   0        0        0     1473 2023-05-31 18:38:25.653514 pilgram2-2.0.2/pilgram2/css/contrast.py
+-rw-r--r--   0        0        0     2036 2023-05-31 18:38:25.653514 pilgram2-2.0.2/pilgram2/css/grayscale.py
+-rw-r--r--   0        0        0     2578 2023-05-31 18:38:25.653514 pilgram2-2.0.2/pilgram2/css/hue_rotate.py
+-rw-r--r--   0        0        0     2019 2023-05-31 18:38:25.654512 pilgram2-2.0.2/pilgram2/css/saturate.py
+-rw-r--r--   0        0        0     2024 2023-05-31 18:38:25.654512 pilgram2-2.0.2/pilgram2/css/sepia.py
+-rw-r--r--   0        0        0      592 2023-05-31 18:38:25.654512 pilgram2-2.0.2/pilgram2/css/tests/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-31 18:38:25.654512 pilgram2-2.0.2/pilgram2/css/tests/test_brightness.py
+-rw-r--r--   0        0        0     2401 2023-05-31 18:38:25.655512 pilgram2-2.0.2/pilgram2/css/tests/test_contrast.py
+-rw-r--r--   0        0        0     2313 2023-05-31 18:38:25.655512 pilgram2-2.0.2/pilgram2/css/tests/test_grayscale.py
+-rw-r--r--   0        0        0     2741 2023-05-31 18:38:25.655512 pilgram2-2.0.2/pilgram2/css/tests/test_hue_rotate.py
+-rw-r--r--   0        0        0     2321 2023-05-31 18:38:25.655512 pilgram2-2.0.2/pilgram2/css/tests/test_saturate.py
+-rw-r--r--   0        0        0     2170 2023-05-31 18:38:25.656514 pilgram2-2.0.2/pilgram2/css/tests/test_sepia.py
+-rw-r--r--   0        0        0      920 2023-05-31 18:38:25.656514 pilgram2-2.0.2/pilgram2/dogpatch.py
+-rw-r--r--   0        0        0     1043 2023-05-31 18:38:25.656514 pilgram2-2.0.2/pilgram2/earlybird.py
+-rw-r--r--   0        0        0      996 2023-05-31 18:38:25.657513 pilgram2-2.0.2/pilgram2/gingham.py
+-rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.657513 pilgram2-2.0.2/pilgram2/ginza.py
+-rw-r--r--   0        0        0     1157 2023-05-31 18:38:25.657513 pilgram2-2.0.2/pilgram2/hefe.py
+-rw-r--r--   0        0        0     1040 2023-05-31 18:38:25.657513 pilgram2-2.0.2/pilgram2/helena.py
+-rw-r--r--   0        0        0     1129 2023-05-31 18:38:25.658513 pilgram2-2.0.2/pilgram2/hudson.py
+-rw-r--r--   0        0        0      960 2023-05-31 18:38:25.658513 pilgram2-2.0.2/pilgram2/inkwell.py
+-rw-r--r--   0        0        0     1036 2023-05-31 18:38:25.658513 pilgram2-2.0.2/pilgram2/juno.py
+-rw-r--r--   0        0        0     1011 2023-05-31 18:38:25.659513 pilgram2-2.0.2/pilgram2/kelvin.py
+-rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.659513 pilgram2-2.0.2/pilgram2/lark.py
+-rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.659513 pilgram2-2.0.2/pilgram2/lofi.py
+-rw-r--r--   0        0        0     1037 2023-05-31 18:38:25.659513 pilgram2-2.0.2/pilgram2/ludwig.py
+-rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.660513 pilgram2-2.0.2/pilgram2/maven.py
+-rw-r--r--   0        0        0     1519 2023-05-31 18:38:25.660513 pilgram2-2.0.2/pilgram2/mayfair.py
+-rw-r--r--   0        0        0     1103 2023-05-31 18:38:25.660513 pilgram2-2.0.2/pilgram2/moon.py
+-rw-r--r--   0        0        0     1156 2023-05-31 18:38:25.661513 pilgram2-2.0.2/pilgram2/nashville.py
+-rw-r--r--   0        0        0     1029 2023-05-31 18:38:25.661513 pilgram2-2.0.2/pilgram2/perpetua.py
+-rw-r--r--   0        0        0     1047 2023-05-31 18:38:25.661513 pilgram2-2.0.2/pilgram2/poprocket.py
+-rw-r--r--   0        0        0     1124 2023-05-31 18:38:25.661513 pilgram2-2.0.2/pilgram2/reyes.py
+-rw-r--r--   0        0        0     1561 2023-05-31 18:38:25.662514 pilgram2-2.0.2/pilgram2/rise.py
+-rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.662514 pilgram2-2.0.2/pilgram2/sierra.py
+-rw-r--r--   0        0        0      953 2023-05-31 18:38:25.662514 pilgram2-2.0.2/pilgram2/skyline.py
+-rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.662514 pilgram2-2.0.2/pilgram2/slumber.py
+-rw-r--r--   0        0        0     1033 2023-05-31 18:38:25.663513 pilgram2-2.0.2/pilgram2/stinson.py
+-rw-r--r--   0        0        0     1127 2023-05-31 18:38:25.663513 pilgram2-2.0.2/pilgram2/sutro.py
+-rw-r--r--   0        0        0      592 2023-05-31 18:38:25.664526 pilgram2-2.0.2/pilgram2/tests/__init__.py
+-rw-r--r--   0        0        0    63895 2023-05-31 18:38:25.664526 pilgram2-2.0.2/pilgram2/tests/assets/mtjimba.jpg
+-rw-r--r--   0        0        0      840 2023-05-31 18:38:25.665525 pilgram2-2.0.2/pilgram2/tests/test_1977.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.2/pilgram2/tests/test_aden.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.665525 pilgram2-2.0.2/pilgram2/tests/test_amaro.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.666524 pilgram2-2.0.2/pilgram2/tests/test_ashby.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.666524 pilgram2-2.0.2/pilgram2/tests/test_brannan.py
+-rw-r--r--   0        0        0      857 2023-05-31 18:38:25.666524 pilgram2-2.0.2/pilgram2/tests/test_brooklyn.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.667523 pilgram2-2.0.2/pilgram2/tests/test_charmes.py
+-rw-r--r--   0        0        0      862 2023-05-31 18:38:25.667523 pilgram2-2.0.2/pilgram2/tests/test_clarendon.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.668521 pilgram2-2.0.2/pilgram2/tests/test_crema.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.2/pilgram2/tests/test_dogpatch.py
+-rw-r--r--   0        0        0      862 2023-05-31 18:38:25.668521 pilgram2-2.0.2/pilgram2/tests/test_earlybird.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.668521 pilgram2-2.0.2/pilgram2/tests/test_gingham.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.669524 pilgram2-2.0.2/pilgram2/tests/test_ginza.py
+-rw-r--r--   0        0        0      832 2023-05-31 18:38:25.669524 pilgram2-2.0.2/pilgram2/tests/test_hefe.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.669524 pilgram2-2.0.2/pilgram2/tests/test_helena.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.2/pilgram2/tests/test_hudson.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.670522 pilgram2-2.0.2/pilgram2/tests/test_inkwell.py
+-rw-r--r--   0        0        0      832 2023-05-31 18:38:25.670522 pilgram2-2.0.2/pilgram2/tests/test_juno.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.670522 pilgram2-2.0.2/pilgram2/tests/test_kelvin.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.2/pilgram2/tests/test_lark.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.671522 pilgram2-2.0.2/pilgram2/tests/test_lofi.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.671522 pilgram2-2.0.2/pilgram2/tests/test_ludwig.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.672523 pilgram2-2.0.2/pilgram2/tests/test_maven.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.672523 pilgram2-2.0.2/pilgram2/tests/test_mayfair.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.672523 pilgram2-2.0.2/pilgram2/tests/test_moon.py
+-rw-r--r--   0        0        0      862 2023-05-31 18:38:25.672523 pilgram2-2.0.2/pilgram2/tests/test_nashville.py
+-rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.2/pilgram2/tests/test_perpetua.py
+-rw-r--r--   0        0        0      857 2023-05-31 18:38:25.673522 pilgram2-2.0.2/pilgram2/tests/test_poprocket.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.673522 pilgram2-2.0.2/pilgram2/tests/test_reyes.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.673522 pilgram2-2.0.2/pilgram2/tests/test_rise.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.674524 pilgram2-2.0.2/pilgram2/tests/test_sierra.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.674524 pilgram2-2.0.2/pilgram2/tests/test_skyline.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.674524 pilgram2-2.0.2/pilgram2/tests/test_slumber.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.2/pilgram2/tests/test_stinson.py
+-rw-r--r--   0        0        0      837 2023-05-31 18:38:25.675526 pilgram2-2.0.2/pilgram2/tests/test_sutro.py
+-rw-r--r--   0        0        0      852 2023-05-31 18:38:25.675526 pilgram2-2.0.2/pilgram2/tests/test_toaster.py
+-rw-r--r--   0        0        0      857 2023-05-31 18:38:25.676521 pilgram2-2.0.2/pilgram2/tests/test_valencia.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.2/pilgram2/tests/test_walden.py
+-rw-r--r--   0        0        0      847 2023-05-31 18:38:25.676521 pilgram2-2.0.2/pilgram2/tests/test_willow.py
+-rw-r--r--   0        0        0      842 2023-05-31 18:38:25.677524 pilgram2-2.0.2/pilgram2/tests/test_xpro2.py
+-rw-r--r--   0        0        0     1013 2023-05-31 18:38:25.677524 pilgram2-2.0.2/pilgram2/toaster.py
+-rw-r--r--   0        0        0     1278 2023-05-31 18:38:25.677524 pilgram2-2.0.2/pilgram2/util/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-31 18:38:25.677524 pilgram2-2.0.2/pilgram2/util/add.py
+-rw-r--r--   0        0        0     1010 2023-05-31 18:38:25.678524 pilgram2-2.0.2/pilgram2/util/apply_lut.py
+-rw-r--r--   0        0        0      972 2023-05-31 18:38:25.679038 pilgram2-2.0.2/pilgram2/util/clip.py
+-rw-r--r--   0        0        0     1439 2023-05-31 18:38:25.679038 pilgram2-2.0.2/pilgram2/util/fill.py
+-rw-r--r--   0        0        0      899 2023-05-31 18:38:25.679038 pilgram2-2.0.2/pilgram2/util/invert.py
+-rw-r--r--   0        0        0     2832 2023-05-31 18:38:25.679038 pilgram2-2.0.2/pilgram2/util/linear_gradient.py
+-rw-r--r--   0        0        0      869 2023-05-31 18:38:25.680050 pilgram2-2.0.2/pilgram2/util/or_convert.py
+-rw-r--r--   0        0        0     3801 2023-05-31 18:38:25.680050 pilgram2-2.0.2/pilgram2/util/radial_gradient.py
+-rw-r--r--   0        0        0     1098 2023-05-31 18:38:25.680050 pilgram2-2.0.2/pilgram2/util/subtract.py
+-rw-r--r--   0        0        0     1092 2023-05-31 18:38:25.681046 pilgram2-2.0.2/pilgram2/util/tests/test_add.py
+-rw-r--r--   0        0        0     1226 2023-05-31 18:38:25.681046 pilgram2-2.0.2/pilgram2/util/tests/test_apply_lut.py
+-rw-r--r--   0        0        0     1122 2023-05-31 18:38:25.681046 pilgram2-2.0.2/pilgram2/util/tests/test_clip.py
+-rw-r--r--   0        0        0     1048 2023-05-31 18:38:25.682048 pilgram2-2.0.2/pilgram2/util/tests/test_fill.py
+-rw-r--r--   0        0        0     1020 2023-05-31 18:38:25.682048 pilgram2-2.0.2/pilgram2/util/tests/test_invert.py
+-rw-r--r--   0        0        0     2603 2023-05-31 18:38:25.682048 pilgram2-2.0.2/pilgram2/util/tests/test_linear_gradient.py
+-rw-r--r--   0        0        0     1097 2023-05-31 18:38:25.683048 pilgram2-2.0.2/pilgram2/util/tests/test_or_convert.py
+-rw-r--r--   0        0        0     4730 2023-05-31 18:38:25.683048 pilgram2-2.0.2/pilgram2/util/tests/test_radial_gradient.py
+-rw-r--r--   0        0        0     1115 2023-05-31 18:38:25.683048 pilgram2-2.0.2/pilgram2/util/tests/test_subtract.py
+-rw-r--r--   0        0        0     1093 2023-05-31 18:38:25.683048 pilgram2-2.0.2/pilgram2/valencia.py
+-rw-r--r--   0        0        0     1118 2023-05-31 18:38:25.684047 pilgram2-2.0.2/pilgram2/walden.py
+-rw-r--r--   0        0        0     1150 2023-05-31 18:38:25.684047 pilgram2-2.0.2/pilgram2/willow.py
+-rw-r--r--   0        0        0     1344 2023-05-31 18:38:25.684047 pilgram2-2.0.2/pilgram2/xpro2.py
+-rw-r--r--   0        0        0     2001 2023-06-01 17:46:57.982312 pilgram2-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2993 2023-06-01 18:14:18.605151 pilgram2-2.0.2/README.md
+-rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 pilgram2-2.0.2/PKG-INFO
```

### Comparing `pilgram2-2.0.1/LICENSE` & `pilgram2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/_1977.py` & `pilgram2-2.0.2/pilgram2/_1977.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/__init__.py` & `pilgram2-2.0.2/pilgram2/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/_version.py` & `pilgram2-2.0.2/pilgram2/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
```

### Comparing `pilgram2-2.0.1/pilgram2/aden.py` & `pilgram2-2.0.2/pilgram2/aden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/amaro.py` & `pilgram2-2.0.2/pilgram2/amaro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/ashby.py` & `pilgram2-2.0.2/pilgram2/ashby.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/brannan.py` & `pilgram2-2.0.2/pilgram2/brannan.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/brooklyn.py` & `pilgram2-2.0.2/pilgram2/brooklyn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/charmes.py` & `pilgram2-2.0.2/pilgram2/charmes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/clarendon.py` & `pilgram2-2.0.2/pilgram2/clarendon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/crema.py` & `pilgram2-2.0.2/pilgram2/crema.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/__init__.py` & `pilgram2-2.0.2/pilgram2/css/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/__init__.py` & `pilgram2-2.0.2/pilgram2/css/blending/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/alpha.py` & `pilgram2-2.0.2/pilgram2/css/blending/alpha.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/color.py` & `pilgram2-2.0.2/pilgram2/css/blending/color.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/color_burn.py` & `pilgram2-2.0.2/pilgram2/css/blending/color_burn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/color_dodge.py` & `pilgram2-2.0.2/pilgram2/css/blending/color_dodge.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/darken.py` & `pilgram2-2.0.2/pilgram2/css/blending/darken.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/difference.py` & `pilgram2-2.0.2/pilgram2/css/blending/difference.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/exclusion.py` & `pilgram2-2.0.2/pilgram2/css/blending/exclusion.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/hard_light.py` & `pilgram2-2.0.2/pilgram2/css/blending/hard_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/hue.py` & `pilgram2-2.0.2/pilgram2/css/blending/hue.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/lighten.py` & `pilgram2-2.0.2/pilgram2/css/blending/lighten.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/multiply.py` & `pilgram2-2.0.2/pilgram2/css/blending/multiply.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/nonseparable.py` & `pilgram2-2.0.2/pilgram2/css/blending/nonseparable.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/normal.py` & `pilgram2-2.0.2/pilgram2/css/blending/normal.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/overlay.py` & `pilgram2-2.0.2/pilgram2/css/blending/overlay.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/screen.py` & `pilgram2-2.0.2/pilgram2/css/blending/screen.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/soft_light.py` & `pilgram2-2.0.2/pilgram2/css/blending/soft_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/__init__.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/helpers/__init__.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/helpers/alpha_support.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/helpers/alpha_support.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_alpha.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_color.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_color_burn.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_color_burn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_color_dodge.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_color_dodge.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_darken.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_darken.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_difference.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_exclusion.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_hard_light.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_hard_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_hue.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_lighten.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_lighten.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_multiply.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_multiply.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_nonseparable.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_nonseparable.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_normal.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_overlay.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_screen.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/blending/tests/test_soft_light.py` & `pilgram2-2.0.2/pilgram2/css/blending/tests/test_soft_light.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/brightness.py` & `pilgram2-2.0.2/pilgram2/css/brightness.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/contrast.py` & `pilgram2-2.0.2/pilgram2/css/contrast.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/grayscale.py` & `pilgram2-2.0.2/pilgram2/css/grayscale.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/hue_rotate.py` & `pilgram2-2.0.2/pilgram2/css/hue_rotate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/saturate.py` & `pilgram2-2.0.2/pilgram2/css/saturate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/sepia.py` & `pilgram2-2.0.2/pilgram2/css/sepia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/__init__.py` & `pilgram2-2.0.2/pilgram2/css/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_brightness.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_brightness.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_contrast.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_contrast.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_grayscale.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_hue_rotate.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_hue_rotate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_saturate.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_saturate.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/css/tests/test_sepia.py` & `pilgram2-2.0.2/pilgram2/css/tests/test_sepia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/dogpatch.py` & `pilgram2-2.0.2/pilgram2/dogpatch.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/earlybird.py` & `pilgram2-2.0.2/pilgram2/earlybird.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/gingham.py` & `pilgram2-2.0.2/pilgram2/gingham.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/ginza.py` & `pilgram2-2.0.2/pilgram2/ginza.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/hefe.py` & `pilgram2-2.0.2/pilgram2/hefe.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/helena.py` & `pilgram2-2.0.2/pilgram2/helena.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/hudson.py` & `pilgram2-2.0.2/pilgram2/hudson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/inkwell.py` & `pilgram2-2.0.2/pilgram2/inkwell.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/juno.py` & `pilgram2-2.0.2/pilgram2/juno.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/kelvin.py` & `pilgram2-2.0.2/pilgram2/kelvin.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/lark.py` & `pilgram2-2.0.2/pilgram2/lark.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/lofi.py` & `pilgram2-2.0.2/pilgram2/lofi.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/ludwig.py` & `pilgram2-2.0.2/pilgram2/ludwig.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/maven.py` & `pilgram2-2.0.2/pilgram2/maven.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/mayfair.py` & `pilgram2-2.0.2/pilgram2/mayfair.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/moon.py` & `pilgram2-2.0.2/pilgram2/moon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/nashville.py` & `pilgram2-2.0.2/pilgram2/nashville.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/perpetua.py` & `pilgram2-2.0.2/pilgram2/perpetua.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/poprocket.py` & `pilgram2-2.0.2/pilgram2/poprocket.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/reyes.py` & `pilgram2-2.0.2/pilgram2/reyes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/rise.py` & `pilgram2-2.0.2/pilgram2/rise.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/sierra.py` & `pilgram2-2.0.2/pilgram2/sierra.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/skyline.py` & `pilgram2-2.0.2/pilgram2/skyline.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/slumber.py` & `pilgram2-2.0.2/pilgram2/slumber.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/stinson.py` & `pilgram2-2.0.2/pilgram2/stinson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/sutro.py` & `pilgram2-2.0.2/pilgram2/sutro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/__init__.py` & `pilgram2-2.0.2/pilgram2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/assets/mtjimba.jpg` & `pilgram2-2.0.2/pilgram2/tests/assets/mtjimba.jpg`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_1977.py` & `pilgram2-2.0.2/pilgram2/tests/test_1977.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_aden.py` & `pilgram2-2.0.2/pilgram2/tests/test_aden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_amaro.py` & `pilgram2-2.0.2/pilgram2/tests/test_amaro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_ashby.py` & `pilgram2-2.0.2/pilgram2/tests/test_ashby.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_brannan.py` & `pilgram2-2.0.2/pilgram2/tests/test_brannan.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_brooklyn.py` & `pilgram2-2.0.2/pilgram2/tests/test_brooklyn.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_charmes.py` & `pilgram2-2.0.2/pilgram2/tests/test_charmes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_clarendon.py` & `pilgram2-2.0.2/pilgram2/tests/test_clarendon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_crema.py` & `pilgram2-2.0.2/pilgram2/tests/test_crema.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_dogpatch.py` & `pilgram2-2.0.2/pilgram2/tests/test_dogpatch.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_earlybird.py` & `pilgram2-2.0.2/pilgram2/tests/test_earlybird.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_gingham.py` & `pilgram2-2.0.2/pilgram2/tests/test_gingham.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_ginza.py` & `pilgram2-2.0.2/pilgram2/tests/test_ginza.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_hefe.py` & `pilgram2-2.0.2/pilgram2/tests/test_hefe.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_helena.py` & `pilgram2-2.0.2/pilgram2/tests/test_helena.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_hudson.py` & `pilgram2-2.0.2/pilgram2/tests/test_hudson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_inkwell.py` & `pilgram2-2.0.2/pilgram2/tests/test_inkwell.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_juno.py` & `pilgram2-2.0.2/pilgram2/tests/test_juno.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_kelvin.py` & `pilgram2-2.0.2/pilgram2/tests/test_kelvin.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_lark.py` & `pilgram2-2.0.2/pilgram2/tests/test_lark.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_lofi.py` & `pilgram2-2.0.2/pilgram2/tests/test_lofi.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_ludwig.py` & `pilgram2-2.0.2/pilgram2/tests/test_ludwig.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_maven.py` & `pilgram2-2.0.2/pilgram2/tests/test_maven.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_mayfair.py` & `pilgram2-2.0.2/pilgram2/tests/test_mayfair.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_moon.py` & `pilgram2-2.0.2/pilgram2/tests/test_moon.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_nashville.py` & `pilgram2-2.0.2/pilgram2/tests/test_nashville.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_perpetua.py` & `pilgram2-2.0.2/pilgram2/tests/test_perpetua.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_poprocket.py` & `pilgram2-2.0.2/pilgram2/tests/test_poprocket.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_reyes.py` & `pilgram2-2.0.2/pilgram2/tests/test_reyes.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_rise.py` & `pilgram2-2.0.2/pilgram2/tests/test_rise.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_sierra.py` & `pilgram2-2.0.2/pilgram2/tests/test_sierra.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_skyline.py` & `pilgram2-2.0.2/pilgram2/tests/test_skyline.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_slumber.py` & `pilgram2-2.0.2/pilgram2/tests/test_slumber.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_stinson.py` & `pilgram2-2.0.2/pilgram2/tests/test_stinson.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_sutro.py` & `pilgram2-2.0.2/pilgram2/tests/test_sutro.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_toaster.py` & `pilgram2-2.0.2/pilgram2/tests/test_toaster.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_valencia.py` & `pilgram2-2.0.2/pilgram2/tests/test_valencia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_walden.py` & `pilgram2-2.0.2/pilgram2/tests/test_walden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_willow.py` & `pilgram2-2.0.2/pilgram2/tests/test_willow.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/tests/test_xpro2.py` & `pilgram2-2.0.2/pilgram2/tests/test_xpro2.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/toaster.py` & `pilgram2-2.0.2/pilgram2/toaster.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/__init__.py` & `pilgram2-2.0.2/pilgram2/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/add.py` & `pilgram2-2.0.2/pilgram2/util/add.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/apply_lut.py` & `pilgram2-2.0.2/pilgram2/util/apply_lut.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/clip.py` & `pilgram2-2.0.2/pilgram2/util/clip.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/fill.py` & `pilgram2-2.0.2/pilgram2/util/fill.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/invert.py` & `pilgram2-2.0.2/pilgram2/util/invert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/linear_gradient.py` & `pilgram2-2.0.2/pilgram2/util/linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/or_convert.py` & `pilgram2-2.0.2/pilgram2/util/or_convert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/radial_gradient.py` & `pilgram2-2.0.2/pilgram2/util/radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/subtract.py` & `pilgram2-2.0.2/pilgram2/util/subtract.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_add.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_apply_lut.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_apply_lut.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_clip.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_fill.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_invert.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_linear_gradient.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_or_convert.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_or_convert.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_radial_gradient.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/util/tests/test_subtract.py` & `pilgram2-2.0.2/pilgram2/util/tests/test_subtract.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/valencia.py` & `pilgram2-2.0.2/pilgram2/valencia.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/walden.py` & `pilgram2-2.0.2/pilgram2/walden.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/willow.py` & `pilgram2-2.0.2/pilgram2/willow.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/pilgram2/xpro2.py` & `pilgram2-2.0.2/pilgram2/xpro2.py`

 * *Files identical despite different names*

### Comparing `pilgram2-2.0.1/README.md` & `pilgram2-2.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # pilgram2
 
 [![PyPI](https://img.shields.io/pypi/v/pilgram2.svg)](https://python.org/pypi/pilgram2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pilgram2.svg)](https://python.org/pypi/pilgram2)
 [![Python CI](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml/badge.svg)](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml)
-[![codecov](https://codecov.io/gh/mgrl/pilgram2/branch/master/graph/badge.svg)](https://codecov.io/gh/mgrl/pilgram2)
+[![codecov](https://codecov.io/gh/mgrl/pilgram2/branch/main/graph/badge.svg)](https://codecov.io/gh/mgrl/pilgram2)
 
 A python library for instagram filters.
 
-![screenshot](https://raw.githubusercontent.com/mgrl/pilgram2/v2/screenshots/screenshot.png)
+![screenshot](https://raw.githubusercontent.com/mgrl/pilgram2/main/screenshots/screenshot.png)
 
 The filter implementations are inspired by [CSSgram](https://una.im/CSSgram/).
 Pilgram2 was forked from [pilgram](https://github.com/akiomik/pilgram).
 Pilgram2 features more filter and supports non-quadratic images.
 
 ## Requirements
 
-- Python >= 3.4
+- Python >= 3.8
 - [Pillow](https://pillow.readthedocs.io/en/stable/) or [pillow-simd](https://github.com/uploadcare/pillow-simd)
 - [NumPy](https://numpy.org)
 
 ## Install
 
 ```sh
-pip install pillow>=4.1.0 # or pip install pillow-simd
+pip install pillow # or pip install pillow-simd
 pip install numpy
 pip install pilgram2
 ```
 
 ## Usage
 
 39 available instagram filters on `pilgram2`, 14 filters new to pilgram2 compared to pilgram:
@@ -120,18 +120,13 @@
 import pilgram2.css.blending
 
 backdrop = Image.open('backdrop.jpg')
 source = Image.open('source.jpg')
 pilgram2.css.blending.color(backdrop, source).save('blending.jpg')
 ```
 
-## Performance
-
-![filter performance comparison](screenshots/filter-performance-comparison.png)
-
 ## Test
 
 ```sh
 pipenv install --dev
 make test     # pytest
-make test-tox # pytest with tox
 ```
```

### Comparing `pilgram2-2.0.1/PKG-INFO` & `pilgram2-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilgram2
-Version: 2.0.1
+Version: 2.0.2
 Summary: library for instagram filters
 License: Apache-2.0
 Author: Michael G
 Author-email: me@mgrl.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,34 +16,34 @@
 Description-Content-Type: text/markdown
 
 # pilgram2
 
 [![PyPI](https://img.shields.io/pypi/v/pilgram2.svg)](https://python.org/pypi/pilgram2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pilgram2.svg)](https://python.org/pypi/pilgram2)
 [![Python CI](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml/badge.svg)](https://github.com/mgrl/pilgram2/actions/workflows/ci.yml)
-[![codecov](https://codecov.io/gh/mgrl/pilgram2/branch/master/graph/badge.svg)](https://codecov.io/gh/mgrl/pilgram2)
+[![codecov](https://codecov.io/gh/mgrl/pilgram2/branch/main/graph/badge.svg)](https://codecov.io/gh/mgrl/pilgram2)
 
 A python library for instagram filters.
 
-![screenshot](https://raw.githubusercontent.com/mgrl/pilgram2/v2/screenshots/screenshot.png)
+![screenshot](https://raw.githubusercontent.com/mgrl/pilgram2/main/screenshots/screenshot.png)
 
 The filter implementations are inspired by [CSSgram](https://una.im/CSSgram/).
 Pilgram2 was forked from [pilgram](https://github.com/akiomik/pilgram).
 Pilgram2 features more filter and supports non-quadratic images.
 
 ## Requirements
 
-- Python >= 3.4
+- Python >= 3.8
 - [Pillow](https://pillow.readthedocs.io/en/stable/) or [pillow-simd](https://github.com/uploadcare/pillow-simd)
 - [NumPy](https://numpy.org)
 
 ## Install
 
 ```sh
-pip install pillow>=4.1.0 # or pip install pillow-simd
+pip install pillow # or pip install pillow-simd
 pip install numpy
 pip install pilgram2
 ```
 
 ## Usage
 
 39 available instagram filters on `pilgram2`, 14 filters new to pilgram2 compared to pilgram:
@@ -137,19 +137,14 @@
 import pilgram2.css.blending
 
 backdrop = Image.open('backdrop.jpg')
 source = Image.open('source.jpg')
 pilgram2.css.blending.color(backdrop, source).save('blending.jpg')
 ```
 
-## Performance
-
-![filter performance comparison](screenshots/filter-performance-comparison.png)
-
 ## Test
 
 ```sh
 pipenv install --dev
 make test     # pytest
-make test-tox # pytest with tox
 ```
```

