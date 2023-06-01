# Comparing `tmp/scicm-1.0.3.tar.gz` & `tmp/scicm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicm-1.0.3.tar", last modified: Wed Nov 23 23:16:12 2022, max compression
+gzip compressed data, was "scicm-1.0.4.tar", last modified: Thu Jun  1 17:25:29 2023, max compression
```

## Comparing `scicm-1.0.3.tar` & `scicm-1.0.4.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2022-11-23 23:16:12.727609 scicm-1.0.3/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1527 2021-02-12 11:28:41.000000 scicm-1.0.3/LICENSE
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      104 2021-12-09 09:00:33.000000 scicm-1.0.3/MANIFEST.in
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2255 2022-11-23 23:16:12.727609 scicm-1.0.3/PKG-INFO
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1904 2021-12-09 09:00:23.000000 scicm-1.0.3/README.md
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       90 2021-02-23 07:25:28.000000 scicm-1.0.3/pyproject.toml
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2022-11-23 23:16:10.879619 scicm-1.0.3/scicm/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      319 2021-08-18 07:54:27.000000 scicm-1.0.3/scicm/__init__.py
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2086 2022-10-11 20:15:05.000000 scicm-1.0.3/scicm/cm.py
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2022-11-23 23:16:12.726609 scicm-1.0.3/scicm/cm_data/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 09:02:00.000000 scicm-1.0.3/scicm/cm_data/B2P.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8421 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/B2T.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/BY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8369 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BgreyY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BkG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BkO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BkR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BkT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8343 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BkY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Blue.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Blue2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-02 08:54:55.000000 scicm-1.0.3/scicm/cm_data/BwG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BwM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/BwO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 09:01:22.000000 scicm-1.0.3/scicm/cm_data/BwR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Cyan.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    13797 2021-02-26 13:01:23.000000 scicm-1.0.3/scicm/cm_data/Day.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:59:16.000000 scicm-1.0.3/scicm/cm_data/G2Y.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/GB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/GP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/GT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-03-24 08:46:31.000000 scicm-1.0.3/scicm/cm_data/Garnet.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/GkM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:59:58.000000 scicm-1.0.3/scicm/cm_data/GkP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Green.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Green2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/GwM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/GwP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:58:20.000000 scicm-1.0.3/scicm/cm_data/M2R.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/MB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/MO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/MR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/MY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Magenta.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Magenta2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    13797 2021-02-26 13:01:23.000000 scicm-1.0.3/scicm/cm_data/Night.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:57:39.000000 scicm-1.0.3/scicm/cm_data/O2Y.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/OB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/OP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/OT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/OkM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Orange.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Orange2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:56:31.000000 scicm-1.0.3/scicm/cm_data/P2M.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/PY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8365 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/PgreyG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/PkM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:57:18.000000 scicm-1.0.3/scicm/cm_data/PkO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/PkR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/PkY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 07:35:08.000000 scicm-1.0.3/scicm/cm_data/Purple.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Purple2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/PwM.txt
--rw-r--r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:56:10.000000 scicm-1.0.3/scicm/cm_data/Quartile.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:55:01.000000 scicm-1.0.3/scicm/cm_data/R2O.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/RB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/RP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/RT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 07:34:53.000000 scicm-1.0.3/scicm/cm_data/Red.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Red2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8363 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/RgreyB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-03-23 05:27:25.000000 scicm-1.0.3/scicm/cm_data/Ripe.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/RwM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/RwP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftBlue.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftGreen.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftMagenta.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftOrange.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftPurple.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftRed.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftTeal.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-26 06:15:41.000000 scicm-1.0.3/scicm/cm_data/SoftYellow.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Stone.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/T2G.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/TB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/TO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/TR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/TY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Teal.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Teal2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    11520 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TgreyM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TkG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/TkO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TkP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TkR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TkY.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-03-04 06:48:47.000000 scicm-1.0.3/scicm/cm_data/Tropical.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TwG.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TwO.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/TwR.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/YB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/YP.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2022-06-26 06:21:15.000000 scicm-1.0.3/scicm/cm_data/YT.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-08-25 08:18:51.000000 scicm-1.0.3/scicm/cm_data/Yellow.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/Yellow2080.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-07-15 12:26:29.000000 scicm-1.0.3/scicm/cm_data/YkB.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-02-23 08:53:13.000000 scicm-1.0.3/scicm/cm_data/YkM.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/iso_1.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2021-12-03 06:17:56.000000 scicm-1.0.3/scicm/cm_data/iso_2.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     6185 2022-07-10 05:14:22.000000 scicm-1.0.3/scicm/tools.py
-drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2022-11-23 23:16:10.880619 scicm-1.0.3/scicm.egg-info/
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2255 2022-11-23 23:16:10.000000 scicm-1.0.3/scicm.egg-info/PKG-INFO
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2759 2022-11-23 23:16:10.000000 scicm-1.0.3/scicm.egg-info/SOURCES.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2022-11-23 23:16:10.000000 scicm-1.0.3/scicm.egg-info/dependency_links.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       54 2022-11-23 23:16:10.000000 scicm-1.0.3/scicm.egg-info/requires.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        6 2022-11-23 23:16:10.000000 scicm-1.0.3/scicm.egg-info/top_level.txt
--rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      540 2022-11-23 23:16:12.729609 scicm-1.0.3/setup.cfg
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2023-06-01 17:25:29.086557 scicm-1.0.4/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     1527 2023-01-11 21:44:26.000000 scicm-1.0.4/LICENSE
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      104 2023-01-11 21:44:26.000000 scicm-1.0.4/MANIFEST.in
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     5381 2023-06-01 17:25:29.086557 scicm-1.0.4/PKG-INFO
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     5030 2023-06-01 17:21:34.000000 scicm-1.0.4/README.md
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       90 2023-01-11 21:44:29.000000 scicm-1.0.4/pyproject.toml
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2023-06-01 17:25:28.423559 scicm-1.0.4/scicm/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      319 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/__init__.py
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2156 2023-06-01 17:21:34.000000 scicm-1.0.4/scicm/cm.py
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2023-06-01 17:25:29.085557 scicm-1.0.4/scicm/cm_data/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/B2P.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8421 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/B2T.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8369 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BgreyY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BkG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BkO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BkR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BkT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8343 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BkY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Blue.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Blue2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BwG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BwM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BwO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/BwR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Cyan.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    13797 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Day.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/G2Y.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Garnet.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GkM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GkP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Green.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Green2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GwM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/GwP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/M2R.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/MB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/MO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/MR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/MY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Magenta.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Magenta2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    13797 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Night.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/O2Y.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/OB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/OP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/OT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/OkM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Orange.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Orange2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/P2M.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8365 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PgreyG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PkM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PkO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PkR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PkY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Purple.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Purple2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/PwM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Quartile.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/R2O.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Red.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Red2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8363 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RgreyB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Ripe.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RwM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/RwP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftBlue.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftGreen.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftMagenta.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftOrange.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftPurple.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftRed.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftTeal.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/SoftYellow.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Stone.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/T2G.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Teal.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Teal2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)    11520 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TgreyM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TkG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TkO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TkP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TkR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TkY.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Tropical.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TwG.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TwO.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/TwR.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/YB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/YP.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/YT.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Yellow.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/Yellow2080.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/YkB.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/YkM.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/iso_1.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     8448 2023-01-11 21:44:29.000000 scicm-1.0.4/scicm/cm_data/iso_2.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     6185 2023-05-31 20:38:49.000000 scicm-1.0.4/scicm/tools.py
+drwxrwxr-x   0 mbravo    (1000) mbravo    (1000)        0 2023-06-01 17:25:28.425559 scicm-1.0.4/scicm.egg-info/
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     5381 2023-06-01 17:25:28.000000 scicm-1.0.4/scicm.egg-info/PKG-INFO
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)     2759 2023-06-01 17:25:28.000000 scicm-1.0.4/scicm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        1 2023-06-01 17:25:28.000000 scicm-1.0.4/scicm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)       54 2023-06-01 17:25:28.000000 scicm-1.0.4/scicm.egg-info/requires.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)        6 2023-06-01 17:25:28.000000 scicm-1.0.4/scicm.egg-info/top_level.txt
+-rw-rw-r--   0 mbravo    (1000) mbravo    (1000)      540 2023-06-01 17:25:29.087557 scicm-1.0.4/setup.cfg
```

### Comparing `scicm-1.0.3/LICENSE` & `scicm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm.py` & `scicm-1.0.4/scicm/cm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 '''This module reads the colour map data from the cm folder, set ups the corresponding colour
 maps and their corresponding reverse order maps, and registers them with matplotlib'''
 
-from os import path
+from os import path, sep
 import pkg_resources
 from glob import glob
 from numpy import loadtxt
 from matplotlib.colors import LinearSegmentedColormap as LSC
 
 # Check for matplotlib version
-mpl_ver=pkg_resources.get_distribution('matplotlib').version
-mpl_ver=[int(s) for s in mpl_ver.split('.')]
-mpl_ver=mpl_ver[0]*10+mpl_ver[1]
-if mpl_ver>=35:
+mpl_ver = pkg_resources.get_distribution('matplotlib').version
+mpl_ver = [int(s) for s in mpl_ver.split('.')]
+mpl_ver = mpl_ver[0]*10+mpl_ver[1]
+if mpl_ver >= 35:
     from matplotlib import colormaps as cm
 else:
     from matplotlib import cm
 
 # Grab the path to the colour map data
-data_path=path.join(path.split(__file__)[0],'cm_data')
+data_path = path.join(path.split(__file__)[0], 'cm_data')
 
 # List of all colour maps in scicm
-cmaps=[c.split('/')[-1].split('.')[0] for c in sorted(glob(f'{data_path}/*.txt'))]
+cmaps = [c.split(sep)[-1].split('.')[0] for c in sorted(glob(f'{data_path}{sep}*.txt'))]
 
 # List of diverging colour maps, this separate list is used
 # to generate the mirror name copies (i.e. RwB)
-diverging=[c for c in cmaps if len(c)==3 and c[1]=='k']
-diverging+=[c for c in cmaps if len(c)==3 and c[1]=='w']
-diverging={c:c[::-1] for c in diverging}
+diverging = [c for c in cmaps if len(c) == 3 and c[1] == 'k']
+diverging += [c for c in cmaps if len(c) == 3 and c[1] == 'w']
+diverging = {c: c[::-1] for c in diverging}
 
 # Reading in the colour map data and setting up the cm objects
-cmap_dict={}
+cmap_dict = {}
 for cmap in cmaps:
-    cmap_path=path.join(data_path,f'{cmap}.txt')
-    cmap_data=loadtxt(cmap_path)
-    cmap_dict[cmap]=LSC.from_list(f'scicm.{cmap}',cmap_data,N=cmap_data.shape[0])
-    cmap_dict[f'{cmap}_r']=LSC.from_list(f'scicm.{cmap}_r',cmap_data[::-1,:],
-                                         N=cmap_data.shape[0])
-    if cmap in diverging.keys():
-        cmap_name=diverging[cmap]
-        cmap_dict[cmap_name]=LSC.from_list(f'scicm.{cmap_name}',cmap_data[::-1,:],
+    cmap_path = path.join(data_path, f'{cmap}.txt')
+    cmap_data = loadtxt(cmap_path)
+    cmap_dict[cmap] = LSC.from_list(f'scicm.{cmap}', cmap_data, N=cmap_data.shape[0])
+    cmap_dict[f'{cmap}_r'] = LSC.from_list(f'scicm.{cmap}_r', cmap_data[::-1, :],
                                            N=cmap_data.shape[0])
-        cmap_dict[f'{cmap_name}_r']=LSC.from_list(f'scicm.{cmap_name}_r',cmap_data,
-                                                  N=cmap_data.shape[0])
+    if cmap in diverging.keys():
+        cmap_name = diverging[cmap]
+        cmap_dict[cmap_name] = LSC.from_list(f'scicm.{cmap_name}', cmap_data[::-1, :],
+                                             N=cmap_data.shape[0])
+        cmap_dict[f'{cmap_name}_r'] = LSC.from_list(f'scicm.{cmap_name}_r', cmap_data,
+                                                    N=cmap_data.shape[0])
 
 # Registering the maps with matplotlib
-if mpl_ver>=35:
+if mpl_ver >= 35:
     for cmap in cmap_dict:
         cm.register(cmap_dict[cmap])
 else:
     for cmap in cmap_dict:
-        cm.register_cmap(f'scicm.{cmap}',cmap_dict[cmap])
+        cm.register_cmap(f'scicm.{cmap}', cmap_dict[cmap])
 
 locals().update(cmap_dict)
```

### Comparing `scicm-1.0.3/scicm/cm_data/B2P.txt` & `scicm-1.0.4/scicm/cm_data/B2P.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/B2T.txt` & `scicm-1.0.4/scicm/cm_data/B2T.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BG.txt` & `scicm-1.0.4/scicm/cm_data/BG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BM.txt` & `scicm-1.0.4/scicm/cm_data/BM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BO.txt` & `scicm-1.0.4/scicm/cm_data/BO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BR.txt` & `scicm-1.0.4/scicm/cm_data/BR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BT.txt` & `scicm-1.0.4/scicm/cm_data/BT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BY.txt` & `scicm-1.0.4/scicm/cm_data/BY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BgreyY.txt` & `scicm-1.0.4/scicm/cm_data/BgreyY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BkG.txt` & `scicm-1.0.4/scicm/cm_data/BkG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BkO.txt` & `scicm-1.0.4/scicm/cm_data/BkO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BkR.txt` & `scicm-1.0.4/scicm/cm_data/BkR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BkT.txt` & `scicm-1.0.4/scicm/cm_data/BkT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BkY.txt` & `scicm-1.0.4/scicm/cm_data/BkY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Blue.txt` & `scicm-1.0.4/scicm/cm_data/Blue.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Blue2080.txt` & `scicm-1.0.4/scicm/cm_data/Blue2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BwG.txt` & `scicm-1.0.4/scicm/cm_data/BwG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BwM.txt` & `scicm-1.0.4/scicm/cm_data/BwM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BwO.txt` & `scicm-1.0.4/scicm/cm_data/BwO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/BwR.txt` & `scicm-1.0.4/scicm/cm_data/BwR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Cyan.txt` & `scicm-1.0.4/scicm/cm_data/Cyan.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Day.txt` & `scicm-1.0.4/scicm/cm_data/Day.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/G2Y.txt` & `scicm-1.0.4/scicm/cm_data/G2Y.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GB.txt` & `scicm-1.0.4/scicm/cm_data/GB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GP.txt` & `scicm-1.0.4/scicm/cm_data/GP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GT.txt` & `scicm-1.0.4/scicm/cm_data/GT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Garnet.txt` & `scicm-1.0.4/scicm/cm_data/Garnet.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GkM.txt` & `scicm-1.0.4/scicm/cm_data/GkM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GkP.txt` & `scicm-1.0.4/scicm/cm_data/GkP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Green.txt` & `scicm-1.0.4/scicm/cm_data/Green.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Green2080.txt` & `scicm-1.0.4/scicm/cm_data/Green2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GwM.txt` & `scicm-1.0.4/scicm/cm_data/GwM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/GwP.txt` & `scicm-1.0.4/scicm/cm_data/GwP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/M2R.txt` & `scicm-1.0.4/scicm/cm_data/M2R.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/MB.txt` & `scicm-1.0.4/scicm/cm_data/MB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/MO.txt` & `scicm-1.0.4/scicm/cm_data/MO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/MR.txt` & `scicm-1.0.4/scicm/cm_data/MR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/MY.txt` & `scicm-1.0.4/scicm/cm_data/MY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Magenta.txt` & `scicm-1.0.4/scicm/cm_data/Magenta.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Magenta2080.txt` & `scicm-1.0.4/scicm/cm_data/Magenta2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Night.txt` & `scicm-1.0.4/scicm/cm_data/Night.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/O2Y.txt` & `scicm-1.0.4/scicm/cm_data/O2Y.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/OB.txt` & `scicm-1.0.4/scicm/cm_data/OB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/OP.txt` & `scicm-1.0.4/scicm/cm_data/OP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/OT.txt` & `scicm-1.0.4/scicm/cm_data/OT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/OkM.txt` & `scicm-1.0.4/scicm/cm_data/OkM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Orange.txt` & `scicm-1.0.4/scicm/cm_data/Orange.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Orange2080.txt` & `scicm-1.0.4/scicm/cm_data/Orange2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/P2M.txt` & `scicm-1.0.4/scicm/cm_data/P2M.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PG.txt` & `scicm-1.0.4/scicm/cm_data/PG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PM.txt` & `scicm-1.0.4/scicm/cm_data/PM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PO.txt` & `scicm-1.0.4/scicm/cm_data/PO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PR.txt` & `scicm-1.0.4/scicm/cm_data/PR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PT.txt` & `scicm-1.0.4/scicm/cm_data/PT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PY.txt` & `scicm-1.0.4/scicm/cm_data/PY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PgreyG.txt` & `scicm-1.0.4/scicm/cm_data/PgreyG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PkM.txt` & `scicm-1.0.4/scicm/cm_data/PkM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PkO.txt` & `scicm-1.0.4/scicm/cm_data/PkO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PkR.txt` & `scicm-1.0.4/scicm/cm_data/PkR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PkY.txt` & `scicm-1.0.4/scicm/cm_data/PkY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Purple.txt` & `scicm-1.0.4/scicm/cm_data/Purple.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Purple2080.txt` & `scicm-1.0.4/scicm/cm_data/Purple2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/PwM.txt` & `scicm-1.0.4/scicm/cm_data/PwM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Quartile.txt` & `scicm-1.0.4/scicm/cm_data/Quartile.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/R2O.txt` & `scicm-1.0.4/scicm/cm_data/R2O.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RB.txt` & `scicm-1.0.4/scicm/cm_data/RB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RP.txt` & `scicm-1.0.4/scicm/cm_data/RP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RT.txt` & `scicm-1.0.4/scicm/cm_data/RT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Red.txt` & `scicm-1.0.4/scicm/cm_data/Red.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Red2080.txt` & `scicm-1.0.4/scicm/cm_data/Red2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RgreyB.txt` & `scicm-1.0.4/scicm/cm_data/RgreyB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Ripe.txt` & `scicm-1.0.4/scicm/cm_data/Ripe.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RwM.txt` & `scicm-1.0.4/scicm/cm_data/RwM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/RwP.txt` & `scicm-1.0.4/scicm/cm_data/RwP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftBlue.txt` & `scicm-1.0.4/scicm/cm_data/SoftBlue.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftGreen.txt` & `scicm-1.0.4/scicm/cm_data/SoftGreen.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftMagenta.txt` & `scicm-1.0.4/scicm/cm_data/SoftMagenta.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftOrange.txt` & `scicm-1.0.4/scicm/cm_data/SoftOrange.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftPurple.txt` & `scicm-1.0.4/scicm/cm_data/SoftPurple.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftRed.txt` & `scicm-1.0.4/scicm/cm_data/SoftRed.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftTeal.txt` & `scicm-1.0.4/scicm/cm_data/SoftTeal.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/SoftYellow.txt` & `scicm-1.0.4/scicm/cm_data/SoftYellow.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Stone.txt` & `scicm-1.0.4/scicm/cm_data/Stone.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/T2G.txt` & `scicm-1.0.4/scicm/cm_data/T2G.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TB.txt` & `scicm-1.0.4/scicm/cm_data/TB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TO.txt` & `scicm-1.0.4/scicm/cm_data/TO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TR.txt` & `scicm-1.0.4/scicm/cm_data/TR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TY.txt` & `scicm-1.0.4/scicm/cm_data/TY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Teal.txt` & `scicm-1.0.4/scicm/cm_data/Teal.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Teal2080.txt` & `scicm-1.0.4/scicm/cm_data/Teal2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TgreyM.txt` & `scicm-1.0.4/scicm/cm_data/TgreyM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TkG.txt` & `scicm-1.0.4/scicm/cm_data/TkG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TkO.txt` & `scicm-1.0.4/scicm/cm_data/TkO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TkP.txt` & `scicm-1.0.4/scicm/cm_data/TkP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TkR.txt` & `scicm-1.0.4/scicm/cm_data/TkR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TkY.txt` & `scicm-1.0.4/scicm/cm_data/TkY.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Tropical.txt` & `scicm-1.0.4/scicm/cm_data/Tropical.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TwG.txt` & `scicm-1.0.4/scicm/cm_data/TwG.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TwO.txt` & `scicm-1.0.4/scicm/cm_data/TwO.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/TwR.txt` & `scicm-1.0.4/scicm/cm_data/TwR.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/YB.txt` & `scicm-1.0.4/scicm/cm_data/YB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/YP.txt` & `scicm-1.0.4/scicm/cm_data/YP.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/YT.txt` & `scicm-1.0.4/scicm/cm_data/YT.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Yellow.txt` & `scicm-1.0.4/scicm/cm_data/Yellow.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/Yellow2080.txt` & `scicm-1.0.4/scicm/cm_data/Yellow2080.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/YkB.txt` & `scicm-1.0.4/scicm/cm_data/YkB.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/YkM.txt` & `scicm-1.0.4/scicm/cm_data/YkM.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/iso_1.txt` & `scicm-1.0.4/scicm/cm_data/iso_1.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/cm_data/iso_2.txt` & `scicm-1.0.4/scicm/cm_data/iso_2.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm/tools.py` & `scicm-1.0.4/scicm/tools.py`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/scicm.egg-info/SOURCES.txt` & `scicm-1.0.4/scicm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scicm-1.0.3/setup.cfg` & `scicm-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scicm
-version = 1.0.3
+version = 1.0.4
 description = Science Colour Maps is a small package containing several colour maps created using viscm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MBravoS/scicm
 author = Matías A. Bravo Santa Cruz
 author_email = matias.bravo@icrar.org
 license = BSD-3-Clause
```

