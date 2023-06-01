# Comparing `tmp/pyplotter-0.3.4.tar.gz` & `tmp/pyplotter-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotter-0.3.4.tar", last modified: Wed Sep  7 08:21:11 2022, max compression
+gzip compressed data, was "pyplotter-0.3.5.tar", last modified: Thu Jun  1 11:56:06 2023, max compression
```

## Comparing `pyplotter-0.3.4.tar` & `pyplotter-0.3.5.tar`

### file list

```diff
@@ -1,100 +1,103 @@
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.947191 pyplotter-0.3.4/
--rw-rw-rw-   0        0        0     1182 2022-04-06 10:43:16.000000 pyplotter-0.3.4/LICENSE
--rw-rw-rw-   0        0        0       35 2022-05-10 10:10:11.000000 pyplotter-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7757 2022-09-07 08:21:11.948192 pyplotter-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     7076 2022-09-07 08:19:20.000000 pyplotter-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.767190 pyplotter-0.3.4/pyplotter/
--rw-rw-rw-   0        0        0        0 2022-05-10 10:10:11.000000 pyplotter-0.3.4/pyplotter/__init__.py
--rw-rw-rw-   0        0        0      836 2022-08-01 13:37:57.000000 pyplotter-0.3.4/pyplotter/pyplotter.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.803194 pyplotter-0.3.4/pyplotter/sources/
--rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/sources/__init__.py
--rw-rw-rw-   0        0        0    14695 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/config.py
--rw-rw-rw-   0        0        0    16825 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/functions.py
--rw-rw-rw-   0        0        0    32749 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/main.py
--rw-rw-rw-   0        0        0    95768 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/sources/palettes.py
--rw-rw-rw-   0        0        0     8496 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/pyqtgraph.py
--rw-rw-rw-   0        0        0    17626 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/qcodesDatabase.py
--rw-rw-rw-   0        0        0    10681 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/runPropertiesExtra.py
--rw-rw-rw-   0        0        0     8357 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/widgetBlueFors.py
--rw-rw-rw-   0        0        0    10524 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/widgetCSV.py
--rw-rw-rw-   0        0        0    16164 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/widgetPlot.py
--rw-rw-rw-   0        0        0    70015 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/widgetPlot1d.py
--rw-rw-rw-   0        0        0    69186 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/widgetPlot2d.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.814191 pyplotter-0.3.4/pyplotter/sources/workers/
--rw-rw-rw-   0        0        0        0 2022-03-01 13:15:08.000000 pyplotter-0.3.4/pyplotter/sources/workers/__init__.py
--rw-rw-rw-   0        0        0     3025 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/workers/checkNbRunDatabase.py
--rw-rw-rw-   0        0        0     7192 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/workers/loadDataBase.py
--rw-rw-rw-   0        0        0     4315 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/workers/loadDataFromCache.py
--rw-rw-rw-   0        0        0     9334 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/workers/loadDataFromRun.py
--rw-rw-rw-   0        0        0     2197 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/sources/workers/loadRunInfo.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.853191 pyplotter-0.3.4/pyplotter/ui/
--rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/__init__.py
--rw-rw-rw-   0        0        0     1784 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/checkBoxHidden.py
--rw-rw-rw-   0        0        0     1578 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/checkBoxStared.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.868191 pyplotter-0.3.4/pyplotter/ui/dialogs/
--rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/__init__.py
--rw-rw-rw-   0        0        0     1500 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogColormap.py
--rw-rw-rw-   0        0        0     3668 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogColormapUi.py
--rw-rw-rw-   0        0        0     1816 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogComment.py
--rw-rw-rw-   0        0        0      988 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogFontsize.py
--rw-rw-rw-   0        0        0     4192 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogFontsizeUi.py
--rw-rw-rw-   0        0        0    23043 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogLiveplot.py
--rw-rw-rw-   0        0        0    20446 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/dialogs/dialogLiveplotUi.py
--rw-rw-rw-   0        0        0     1785 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/hBoxLayoutLabelPath.py
--rw-rw-rw-   0        0        0      388 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/histogramLUTWidget.py
--rw-rw-rw-   0        0        0      531 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/labelSnapshot.py
--rw-rw-rw-   0        0        0     1284 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/lineEditSnapshot.py
--rw-rw-rw-   0        0        0    20963 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/mainWindow.py
--rw-rw-rw-   0        0        0     8406 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/menuBar.py
--rw-rw-rw-   0        0        0     1772 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/menuDb.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.897191 pyplotter-0.3.4/pyplotter/ui/pictures/
--rw-rw-rw-   0        0        0     1895 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/pictures/bluefors.png
--rw-rw-rw-   0        0        0     2992 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/csv.png
--rw-rw-rw-   0        0        0     2791 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/database.png
--rw-rw-rw-   0        0        0     1998 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/databaseOpened.png
--rw-rw-rw-   0        0        0     3294 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/databaseOpenedStared.png
--rw-rw-rw-   0        0        0     4684 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/databaseStared.png
--rw-rw-rw-   0        0        0      170 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/empty.png
--rw-rw-rw-   0        0        0     1788 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/folder.png
--rw-rw-rw-   0        0        0     1384 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/folderEnhanced.png
--rw-rw-rw-   0        0        0   192524 2022-01-17 07:35:16.000000 pyplotter-0.3.4/pyplotter/ui/pictures/icon.png
--rw-rw-rw-   0        0        0     1346 2022-01-17 07:35:16.000000 pyplotter-0.3.4/pyplotter/ui/pictures/icon.py
--rw-rw-rw-   0        0        0     2915 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/s2p.png
--rw-rw-rw-   0        0        0     1723 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/star.png
--rw-rw-rw-   0        0        0     1173 2020-11-30 15:51:41.000000 pyplotter-0.3.4/pyplotter/ui/pictures/trash.png
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.944191 pyplotter-0.3.4/pyplotter/ui/plot1d/
--rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/__init__.py
--rw-rw-rw-   0        0        0     5098 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/dialogFiltering.py
--rw-rw-rw-   0        0        0    35713 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/dialogFit.py
--rw-rw-rw-   0        0        0     8502 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxCalculus.py
--rw-rw-rw-   0        0        0     2241 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxCalculusUi.py
--rw-rw-rw-   0        0        0    10977 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFFT.py
--rw-rw-rw-   0        0        0     2625 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFFTUi.py
--rw-rw-rw-   0        0        0     7117 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFiltering.py
--rw-rw-rw-   0        0        0     7132 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFit.py
--rw-rw-rw-   0        0        0     8152 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxNormalize.py
--rw-rw-rw-   0        0        0     2448 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxNormalizeUi.py
--rw-rw-rw-   0        0        0     6588 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxStatistics.py
--rw-rw-rw-   0        0        0     3663 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxStatisticsUi.py
--rw-rw-rw-   0        0        0     8083 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/widgetTabCurve.py
--rw-rw-rw-   0        0        0     3423 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1d/widgetTabCurveUi.py
--rw-rw-rw-   0        0        0      244 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plot1dWidget.py
--rw-rw-rw-   0        0        0      356 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/plotWidget.py
--rw-rw-rw-   0        0        0     1334 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/pushButtonOpenFolder.py
--rw-rw-rw-   0        0        0     6857 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/statusBar.py
--rw-rw-rw-   0        0        0    22218 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/tableWidgetDatabase.py
--rw-rw-rw-   0        0        0    13708 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/tableWidgetFolder.py
--rw-rw-rw-   0        0        0      495 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/tableWidgetItemNumOrdered.py
--rw-rw-rw-   0        0        0    18014 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/tableWidgetParameter.py
--rw-rw-rw-   0        0        0     3940 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/treeViewSnapshot.py
--rw-rw-rw-   0        0        0    15046 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/widgetPlot1d.py
--rw-rw-rw-   0        0        0    26264 2022-09-07 08:19:21.000000 pyplotter-0.3.4/pyplotter/ui/widgetPlot2d.py
-drwxrwxrwx   0        0        0        0 2022-09-07 08:21:11.777190 pyplotter-0.3.4/pyplotter.egg-info/
--rw-rw-rw-   0        0        0     7757 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-07 08:21:11.000000 pyplotter-0.3.4/pyplotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2022-09-07 08:21:11.951198 pyplotter-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      128 2022-05-10 10:10:11.000000 pyplotter-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.969824 pyplotter-0.3.5/
+-rw-rw-rw-   0        0        0     1182 2022-04-06 10:43:16.000000 pyplotter-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-05-10 10:10:11.000000 pyplotter-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7710 2023-06-01 11:56:06.970824 pyplotter-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7076 2022-09-07 08:19:20.000000 pyplotter-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.591823 pyplotter-0.3.5/pyplotter/
+-rw-rw-rw-   0        0        0        0 2022-05-10 10:10:11.000000 pyplotter-0.3.5/pyplotter/__init__.py
+-rw-rw-rw-   0        0        0      836 2022-08-01 13:37:57.000000 pyplotter-0.3.5/pyplotter/pyplotter.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.662822 pyplotter-0.3.5/pyplotter/sources/
+-rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/sources/__init__.py
+-rw-rw-rw-   0        0        0    17575 2023-03-29 14:12:42.000000 pyplotter-0.3.5/pyplotter/sources/config.py
+-rw-rw-rw-   0        0        0    16825 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/functions.py
+-rw-rw-rw-   0        0        0    32935 2023-04-18 10:08:58.000000 pyplotter-0.3.5/pyplotter/sources/main.py
+-rw-rw-rw-   0        0        0    95768 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/sources/palettes.py
+-rw-rw-rw-   0        0        0     8496 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/pyqtgraph.py
+-rw-rw-rw-   0        0        0    29407 2023-04-18 10:04:38.000000 pyplotter-0.3.5/pyplotter/sources/qcodesDatabase.py
+-rw-rw-rw-   0        0        0    10681 2023-03-14 10:33:09.000000 pyplotter-0.3.5/pyplotter/sources/runPropertiesExtra.py
+-rw-rw-rw-   0        0        0     8475 2023-04-18 11:41:03.000000 pyplotter-0.3.5/pyplotter/sources/widgetBlueFors.py
+-rw-rw-rw-   0        0        0    10751 2023-04-18 11:39:49.000000 pyplotter-0.3.5/pyplotter/sources/widgetCSV.py
+-rw-rw-rw-   0        0        0    16164 2023-03-17 13:40:51.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot.py
+-rw-rw-rw-   0        0        0    70638 2023-02-17 09:02:20.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot1d.py
+-rw-rw-rw-   0        0        0    69186 2023-04-18 08:41:49.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot2d.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.681823 pyplotter-0.3.5/pyplotter/sources/workers/
+-rw-rw-rw-   0        0        0        0 2022-03-01 13:15:08.000000 pyplotter-0.3.5/pyplotter/sources/workers/__init__.py
+-rw-rw-rw-   0        0        0     3025 2023-01-04 16:03:39.000000 pyplotter-0.3.5/pyplotter/sources/workers/checkNbRunDatabase.py
+-rw-rw-rw-   0        0        0     7870 2023-03-29 14:10:57.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataBase.py
+-rw-rw-rw-   0        0        0     4315 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromCache.py
+-rw-rw-rw-   0        0        0     9334 2023-01-04 16:03:29.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromRun.py
+-rw-rw-rw-   0        0        0     2290 2023-04-18 10:06:03.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadRunInfo.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.768826 pyplotter-0.3.5/pyplotter/ui/
+-rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/__init__.py
+-rw-rw-rw-   0        0        0     1784 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/checkBoxHidden.py
+-rw-rw-rw-   0        0        0     1578 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/checkBoxStared.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.814826 pyplotter-0.3.5/pyplotter/ui/dialogs/
+-rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-03-17 13:40:19.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormap.py
+-rw-rw-rw-   0        0        0     3668 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormapUi.py
+-rw-rw-rw-   0        0        0     1816 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogComment.py
+-rw-rw-rw-   0        0        0      988 2023-03-17 13:40:13.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsize.py
+-rw-rw-rw-   0        0        0     4192 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsizeUi.py
+-rw-rw-rw-   0        0        0    23043 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplot.py
+-rw-rw-rw-   0        0        0    20446 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplotUi.py
+-rw-rw-rw-   0        0        0     4067 2023-03-29 14:05:07.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py
+-rw-rw-rw-   0        0        0     2859 2023-03-29 13:20:18.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py
+-rw-rw-rw-   0        0        0     1785 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/hBoxLayoutLabelPath.py
+-rw-rw-rw-   0        0        0      388 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/histogramLUTWidget.py
+-rw-rw-rw-   0        0        0      531 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/labelSnapshot.py
+-rw-rw-rw-   0        0        0     1284 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/lineEditSnapshot.py
+-rw-rw-rw-   0        0        0    16326 2023-04-18 10:27:14.000000 pyplotter-0.3.5/pyplotter/ui/mainWindow.py
+-rw-rw-rw-   0        0        0     9055 2023-03-29 13:43:20.000000 pyplotter-0.3.5/pyplotter/ui/menuBar.py
+-rw-rw-rw-   0        0        0     1772 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/menuDb.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.889824 pyplotter-0.3.5/pyplotter/ui/pictures/
+-rw-rw-rw-   0        0        0     1895 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/pictures/bluefors.png
+-rw-rw-rw-   0        0        0     2992 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/csv.png
+-rw-rw-rw-   0        0        0     2791 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/database.png
+-rw-rw-rw-   0        0        0     1998 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpened.png
+-rw-rw-rw-   0        0        0     3294 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpenedStared.png
+-rw-rw-rw-   0        0        0     4684 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseStared.png
+-rw-rw-rw-   0        0        0      170 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/empty.png
+-rw-rw-rw-   0        0        0     1788 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/folder.png
+-rw-rw-rw-   0        0        0     1384 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/folderEnhanced.png
+-rw-rw-rw-   0        0        0   192524 2022-01-17 07:35:16.000000 pyplotter-0.3.5/pyplotter/ui/pictures/icon.png
+-rw-rw-rw-   0        0        0     1346 2022-01-17 07:35:16.000000 pyplotter-0.3.5/pyplotter/ui/pictures/icon.py
+-rw-rw-rw-   0        0        0     2915 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/s2p.png
+-rw-rw-rw-   0        0        0     1723 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/star.png
+-rw-rw-rw-   0        0        0     1173 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/trash.png
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.965824 pyplotter-0.3.5/pyplotter/ui/plot1d/
+-rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/__init__.py
+-rw-rw-rw-   0        0        0     5098 2022-09-13 06:53:17.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFiltering.py
+-rw-rw-rw-   0        0        0    35713 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFit.py
+-rw-rw-rw-   0        0        0     8502 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculus.py
+-rw-rw-rw-   0        0        0     2241 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculusUi.py
+-rw-rw-rw-   0        0        0    10977 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFT.py
+-rw-rw-rw-   0        0        0     2625 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFTUi.py
+-rw-rw-rw-   0        0        0     7117 2022-09-13 06:51:57.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFiltering.py
+-rw-rw-rw-   0        0        0     7132 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFit.py
+-rw-rw-rw-   0        0        0     8152 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalize.py
+-rw-rw-rw-   0        0        0     2448 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalizeUi.py
+-rw-rw-rw-   0        0        0     6588 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatistics.py
+-rw-rw-rw-   0        0        0     3663 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatisticsUi.py
+-rw-rw-rw-   0        0        0     8111 2023-02-17 09:02:20.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurve.py
+-rw-rw-rw-   0        0        0     3423 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurveUi.py
+-rw-rw-rw-   0        0        0      244 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1dWidget.py
+-rw-rw-rw-   0        0        0      356 2023-04-17 13:19:05.000000 pyplotter-0.3.5/pyplotter/ui/plotWidget.py
+-rw-rw-rw-   0        0        0     1334 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/pushButtonOpenFolder.py
+-rw-rw-rw-   0        0        0     6914 2023-04-24 13:35:52.000000 pyplotter-0.3.5/pyplotter/ui/statusBar.py
+-rw-rw-rw-   0        0        0    25592 2023-04-18 10:23:07.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetDatabase.py
+-rw-rw-rw-   0        0        0    13729 2023-03-09 16:16:50.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetFolder.py
+-rw-rw-rw-   0        0        0      495 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetItemNumOrdered.py
+-rw-rw-rw-   0        0        0    21386 2023-04-18 11:41:13.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetParameter.py
+-rw-rw-rw-   0        0        0     3940 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/treeViewSnapshot.py
+-rw-rw-rw-   0        0        0    15046 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/widgetPlot1d.py
+-rw-rw-rw-   0        0        0    26264 2023-04-18 08:42:34.000000 pyplotter-0.3.5/pyplotter/ui/widgetPlot2d.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.614822 pyplotter-0.3.5/pyplotter.egg-info/
+-rw-rw-rw-   0        0        0     7710 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3202 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-06-01 11:56:02.000000 pyplotter-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1064 2023-06-01 11:56:06.973824 pyplotter-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      128 2022-05-10 10:10:11.000000 pyplotter-0.3.5/setup.py
```

### Comparing `pyplotter-0.3.4/LICENSE` & `pyplotter-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/PKG-INFO` & `pyplotter-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pyplotter
-Version: 0.3.4
+Version: 0.3.5
 Summary: A data browser and vizualizer for QCoDes database, csv, s2p and BlueFors logging files.
 Home-page: https://github.com/pyplotter/pyplotter
-Author: Étienne Dumur
 Author-email: etienne.dumur@cea.fr
 Maintainer: Étienne Dumur
 Maintainer-email: etienne.dumur@cea.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -206,9 +204,7 @@
 
 ## 🙏 Acknowledgments
 
 * [plottr](https://github.com/toolsforexperiments/plottr), for the inspiration of some interfaces.
 * [pyqtgraph](http://www.pyqtgraph.org/), for the amazing and **fast** plotting library.
 * [bokeh](https://github.com/bokeh/bokeh/blob/7cc500601cdb688c4b6b2153704097f3345dd91c/bokeh/palettes.py), for their work on the colormap palette reused here.
 * [qb style](https://github.com/quantumblacklabs/qbstyles), for its color codes of lines.
-
-
```

### Comparing `pyplotter-0.3.4/README.md` & `pyplotter-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/pyplotter.py` & `pyplotter-0.3.5/pyplotter/pyplotter.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/config.py` & `pyplotter-0.3.5/pyplotter/sources/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # This Python file uses the following encoding: utf-8
 import json
 import os
 from platformdirs import user_config_dir
 from typing import List, Union, Any
-import collections
+# For python < 3.10
+try:
+    from collections import Mapping
+except:
+    from collections.abc import Mapping # type: ignore
 
 # This file create a python dict containing all personalized parameters
 configPackage = {
 
 # Do not put "/" after ":" in the two following paths
 # The soft will not allowed to go above that path
 'root' : 'C:/',
@@ -133,43 +137,141 @@
                             'pyqtgraphyLabelTextColor' : '#ffffff',
                             'pyqtgraphzLabelTextColor' : '#ffffff',
                             'pyqtgraphxAxisTicksColor' : '#ffffff',
                             'pyqtgraphyAxisTicksColor' : '#ffffff',
                             'pyqtgraphzAxisTicksColor' : '#ffffff',
                             'pyqtgraphxAxisTickLabelsColor': '#ffffff',
                             'pyqtgraphyAxisTickLabelsColor': '#ffffff',
-                            'pyqtgraphzAxisTickLabelsColor': '#ffffff'},
+                            'pyqtgraphzAxisTickLabelsColor': '#ffffff',
+
+                            # Font color for the duration column of the tableWidgetDatabase
+                            'tableWidgetDatabaseDuration' : {
+                                'hour'        : '#9292ff',
+                                'minute'      : '#008080',
+                                'second'      : '#a221de',
+                                'millisecond' : '#e01f1f'
+                                },
+                           },
             'qbstyles' : {'dialogBackgroundColor'    : '#0c1c23',
-                            'pyqtgraphBackgroundColor' : '#0c1c23',
-                            'dialogTextColor'          : '#dadcdd',
-                            'plot1dSelectionLineColor' : '#dadcdd',
-                            'pyqtgraphTitleTextColor'  : '#dadcdd',
-                            'pyqtgraphxLabelTextColor' : '#dadcdd',
-                            'pyqtgraphyLabelTextColor' : '#dadcdd',
-                            'pyqtgraphzLabelTextColor' : '#dadcdd',
-                            'pyqtgraphxAxisTicksColor' : '#dadcdd',
-                            'pyqtgraphyAxisTicksColor' : '#dadcdd',
-                            'pyqtgraphzAxisTicksColor' : '#dadcdd',
-                            'pyqtgraphxAxisTickLabelsColor': '#dadcdd',
-                            'pyqtgraphyAxisTickLabelsColor': '#dadcdd',
-                            'pyqtgraphzAxisTickLabelsColor': '#dadcdd'},
+                          'pyqtgraphBackgroundColor' : '#0c1c23',
+                          'dialogTextColor'          : '#dadcdd',
+                          'plot1dSelectionLineColor' : '#dadcdd',
+                          'pyqtgraphTitleTextColor'  : '#dadcdd',
+                          'pyqtgraphxLabelTextColor' : '#dadcdd',
+                          'pyqtgraphyLabelTextColor' : '#dadcdd',
+                          'pyqtgraphzLabelTextColor' : '#dadcdd',
+                          'pyqtgraphxAxisTicksColor' : '#dadcdd',
+                          'pyqtgraphyAxisTicksColor' : '#dadcdd',
+                          'pyqtgraphzAxisTicksColor' : '#dadcdd',
+                          'pyqtgraphxAxisTickLabelsColor': '#dadcdd',
+                          'pyqtgraphyAxisTickLabelsColor': '#dadcdd',
+                          'pyqtgraphzAxisTickLabelsColor': '#dadcdd',
+
+                          # Font color for the duration column of the tableWidgetDatabase
+                          'tableWidgetDatabaseDuration' : {
+                              'hour'        : '#9292ff',
+                              'minute'      : '#008080',
+                              'second'      : '#a221de',
+                              'millisecond' : '#e01f1f'
+                              },
+                         },
             'white' : {'dialogBackgroundColor'    : '#ffffff',
                        'pyqtgraphBackgroundColor' : '#ffffff',
                        'dialogTextColor'          : '#000000',
                        'plot1dSelectionLineColor' : '#000000',
                        'pyqtgraphTitleTextColor'  : '#000000',
                        'pyqtgraphxLabelTextColor' : '#000000',
                        'pyqtgraphyLabelTextColor' : '#000000',
                        'pyqtgraphzLabelTextColor' : '#000000',
                        'pyqtgraphxAxisTicksColor' : '#000000',
                        'pyqtgraphyAxisTicksColor' : '#000000',
                        'pyqtgraphzAxisTicksColor' : '#000000',
                        'pyqtgraphxAxisTickLabelsColor': '#000000',
                        'pyqtgraphyAxisTickLabelsColor': '#000000',
-                       'pyqtgraphzAxisTickLabelsColor': '#000000'}},
+                       'pyqtgraphzAxisTickLabelsColor': '#000000',
+
+                        # Font color for the duration column of the tableWidgetDatabase
+                        'tableWidgetDatabaseDuration' : {
+                            'hour'        : '#1111dd',
+                            'minute'      : '#008080',
+                            'second'      : '#a221de',
+                            'millisecond' : '#e01f1f'
+                            },
+                      },
+           },
+
+# Columns of tableWidgetDatabase
+'DatabaseDisplayColumn' : {
+    'databaseAbsPath' : {
+        'index' : 0,
+        'name' : '',
+        'visible' : False
+    },
+    'itemRunId' : {
+        'index' : 1,
+        'name' : 'run id',
+        'visible' : True
+    },
+    'dimension' : {
+        'index' : 2,
+        'name' : 'dim',
+        'visible' : True
+    },
+    'experimentName' : {
+        'index' : 3,
+        'name' : 'experiment',
+        'visible' : True
+    },
+    'sampleName' : {
+        'index' : 4,
+        'name' : 'sample',
+        'visible' : True
+    },
+    'runName' : {
+        'index' : 5,
+        'name' : 'name',
+        'visible' : True
+    },
+    'captured_run_id' : {
+        'index' : 6,
+        'name' : 'captured_run_id',
+        'visible' : True
+    },
+    'guid' : {
+        'index' : 7,
+        'name' : 'guid',
+        'visible' : True
+    },
+    'started' : {
+        'index' : 8,
+        'name' : 'started',
+        'visible' : True
+    },
+    'completed' : {
+        'index' : 9,
+        'name' : 'completed',
+        'visible' : True
+    },
+    'duration' : {
+        'index' : 10,
+        'name' : 'duration',
+        'visible' : True
+    },
+    'runRecords' : {
+        'index' : 11,
+        'name' : 'records',
+        'visible' : True
+    },
+    'comment' : {
+        'index' : 12,
+        'name' : 'comment',
+        'visible' : True
+    },
+},
+
 # Font size of the axis and tick labels
 # Handy if user wants to have larger font
 'axisLabelFontSize' : 12,
 'tickLabelFontSize' : 12,
 
 # Plot parameters
 # To avoid heavy calculations and consequently lag, we limit the colormap to a
@@ -250,15 +352,15 @@
     Modify ``source`` in place.
 
     From:
     https://stackoverflow.com/questions/3232943/update-value-of-a-nested-dictionary-of-varying-depth
     """
 
     for key, value in overrides.items():
-        if isinstance(value, collections.Mapping) and value:
+        if isinstance(value, Mapping) and value:
             returned = deep_update(source.get(key, {}), value)
             source[key] = returned
         else:
             source[key] = overrides[key]
     return source
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/functions.py` & `pyplotter-0.3.5/pyplotter/sources/functions.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/main.py` & `pyplotter-0.3.5/pyplotter/sources/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class MainApp(QtWidgets.QMainWindow, mainWindow.Ui_MainWindow):
 
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
     signalRemoveProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     signalEnableCheck          = QtCore.pyqtSignal(QtWidgets.QCheckBox)
-    signalAddRow               = QtCore.pyqtSignal(int, dict, str, str, str, str, str, str, str, int, bool)
+    signalAddRow               = QtCore.pyqtSignal(int, dict, str, str, str, str, str, str, str, str, int, bool)
 
     signalRunClickDone = QtCore.pyqtSignal()
 
 
     def __init__(self, QApplication,
                        parent=None):
 
@@ -55,14 +55,15 @@
 
 
         self.lineEditFilterSnapshot.signallineEditFilterSnapshotTextEdited.connect(self.treeViewSnapshot.searchItem)
 
 
         # Connect menuBar signal
         self.menuBarMain.signalUpdateStyle.connect(self.updateStyle)
+        self.menuBarMain.signalUpdateTableWidgetDatabase.connect(self.tableWidgetDataBase.slotUpdate)
         self.menuBarMain.signal2MainWindowAddPlot.connect(self.slotFromPlotAddPlot)
         self.menuBarMain.signalUpdateCurve.connect(self.slotUpdateCurve)
         self.menuBarMain.signalUpdate2d.connect(self.slotUpdate2d)
         self.menuBarMain.signalSendStatusBarMessage.connect(self.statusBarMain.setStatusBarMessage)
         self.menuBarMain.signalUpdatePlotProperty.connect(self.slotUpdatePlotProperty)
 
 
@@ -178,18 +179,19 @@
     #                           GUI
     #
     #
     ###########################################################################
 
 
 
-    @QtCore.pyqtSlot(int, dict, str, str, str, str, str, str, str, int)
+    @QtCore.pyqtSlot(int, dict, str, str, str, str, str, str, str, str, int)
     def addRow(self, runId: int,
                      paramDependent: dict,
                      experimentName: str,
+                     shape: str,
                      curveId: str,
                      plotRef: str,
                      plotTitle: str,
                      windowTitle: str,
                      databaseAbsPath: str,
                      dataType: str,
                      rowPosition: int) -> None:
@@ -211,14 +213,15 @@
                     if plotRef in plot.plotRef:
                         if plot.zLabelText==paramDependent['label']:
                             parameterPlotted = True
 
         self.signalAddRow.emit(runId,
                                paramDependent,
                                experimentName,
+                               shape,
                                curveId,
                                plotRef,
                                plotTitle,
                                windowTitle,
                                databaseAbsPath,
                                dataType,
                                rowPosition,
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/palettes.py` & `pyplotter-0.3.5/pyplotter/sources/palettes.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/pyqtgraph.py` & `pyplotter-0.3.5/pyplotter/sources/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/qcodesDatabase.py` & `pyplotter-0.3.5/pyplotter/sources/qcodesDatabase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # This Python file uses the following encoding: utf-8
 import io
 import time
 import sqlite3
 import json
 import numpy as np
-from typing import Tuple, List, Union, Any, Sequence
+from typing import Dict, Tuple, List, Union, Optional
 import multiprocess as mp
+try:
+    from importlib.metadata import version
+except ImportError: # for Python<3.8
+    from importlib_metadata import version
 
 from .config import loadConfigCurrent
 config = loadConfigCurrent()
 
 
 def timestamp2string(timestamp :int,
                      fmt :str="%Y-%m-%d %H:%M:%S") -> str:
@@ -17,14 +21,60 @@
     Returns timestamp in a human-readable format.
     """
 
     return time.strftime(fmt, time.localtime(timestamp))
 
 
 
+def timestamps2duration(timestamp_after: Optional[int],
+                        timestamp_before: Optional[int]) -> str:
+    """
+    Returns duration between two timestamps in a human-readable format.
+    """
+
+    if timestamp_before is None or timestamp_after is None:
+        return ''
+
+    s = timestamp_after - timestamp_before
+    hours, remainder = divmod(s, 3600)
+    minutes, seconds = divmod(remainder, 60)
+
+    if hours!=0:
+        return '<span style="color:{};">{:02.0f}h</span>'\
+               '<span style="color:{};">{:02.0f}m</span>'\
+               '<span style="color:{};">{:02.0f}s</span>'\
+               '<span style="color:{};">{:03.0f}ms</span>'.format(config['styles'][config['style']]['tableWidgetDatabaseDuration']['hour'],
+                                                                  hours,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['minute'],
+                                                                  minutes,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['second'],
+                                                                  seconds,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['millisecond'],
+                                                                  (seconds-int(seconds))*1000)
+    elif minutes!=0:
+        return '<span style="color:{};">{:02.0f}m</span>'\
+               '<span style="color:{};">{:02.0f}s</span>'\
+               '<span style="color:{};">{:03.0f}ms</span>'.format(config['styles'][config['style']]['tableWidgetDatabaseDuration']['minute'],
+                                                                  minutes,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['second'],
+                                                                  seconds,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['millisecond'],
+                                                                  (seconds-int(seconds))*1000)
+    elif seconds!=0:
+        return '<span style="color:{};">{:02.0f}s</span>'\
+               '<span style="color:{};">{:03.0f}ms</span>'.format(config['styles'][config['style']]['tableWidgetDatabaseDuration']['second'],
+                                                                  seconds,
+                                                                  config['styles'][config['style']]['tableWidgetDatabaseDuration']['millisecond'],
+                                                                  (seconds-int(seconds))*1000)
+    else:
+        return '<span style="color:{};">{:03.0f}ms</span>'.format(config['styles'][config['style']]['tableWidgetDatabaseDuration']['millisecond'],
+                                                                  (seconds-int(seconds))*1000)
+
+
+
 def openDatabase(databaseAbsPath: str,
                  returnDict: bool=False) -> Tuple[sqlite3.Connection,
                                                   sqlite3.Cursor]:
     """
     Open connection to database using qcodes functions.
 
     Args:
@@ -144,14 +194,32 @@
     # Create nice dict object from a string
     d = json.loads(row['run_description'])
 
     return len([i for i in d['interdependencies']['paramspecs'] if len(i['depends_on'])!=0])
 
 
 
+def getShapeFromRunDescription(runDescription : dict) -> Dict[str, Optional[Tuple[int]]]:
+    """
+        dict of the dependent parameter shape.
+        {dependent parameter name : shape}
+    """
+
+    dependentNames = [i['name'] for i in runDescription['interdependencies']['paramspecs'] if len(i['depends_on'])!=0]
+    # No shapes stored
+    if runDescription['version']<3:
+        return {name : None for name in dependentNames}
+    else:
+        if runDescription['shapes'] is None:
+            return {name : None for name in dependentNames}
+        else:
+            return runDescription['shapes']
+
+
+
 def getDependentSnapshotFromRunId(databaseAbsPath: str,
                                   runId: int) -> Tuple[list, dict]:
     """
     Get the list of dependent parameters from a runId.
     Return a tuple of dependent parameters, each parameter
     being a dict.
 
@@ -189,14 +257,62 @@
 
     dependents = [i for i in d['interdependencies']['paramspecs'] if len(i['depends_on'])!=0]
 
     return dependents, snapshotDict
 
 
 
+def getDependentSnapshotShapeFromRunId(databaseAbsPath: str,
+                                       runId: int) -> Tuple[list, dict, dict]:
+    """
+    Get the list of dependent parameters from a runId.
+    Return a tuple of dependent parameters, each parameter
+    being a dict.
+
+    Parameters
+    ----------
+    runId: int
+        id of the run.
+
+    Return
+    ------
+    (dependent, snapshotDict) : tuple
+        dependents : list
+            list of dict of all dependents parameters.
+        snapshotDict : dict
+            Snapshot of the run.
+        shape : Dict[str, Optional[Tuple[int]]]
+            list of the dependent parameter shape.
+    """
+
+    conn, cur = openDatabase(databaseAbsPath,
+                             returnDict=True)
+
+    # Get runs infos
+    cur.execute("SELECT run_description, snapshot FROM 'runs' WHERE run_id="+str(runId))
+    row = cur.fetchall()[0]
+
+    # Create nice dict object from a string
+    d = json.loads(row['run_description'])
+
+    # If there is no station, the snapshot is None
+    if row['snapshot'] is None:
+        snapshotDict = {'': config['defaultSnapshot']}
+    else:
+        snapshotDict = json.loads(row['snapshot'])
+
+    closeDatabase(conn, cur)
+
+    dependents = [i for i in d['interdependencies']['paramspecs'] if len(i['depends_on'])!=0]
+    shapes = getShapeFromRunDescription(d)
+
+    return dependents, snapshotDict, shapes
+
+
+
 def getNbTotalRun(databaseAbsPath: str) -> int:
     """
     Return the number of run in the database
     """
 
     conn, cur = openDatabase(databaseAbsPath,
                              returnDict=True)
@@ -282,14 +398,120 @@
 #                           but placing them in mutiprocessing queue
 #
 #
 ###########################################################################
 
 
 
+def getParameterDbRow(databaseAbsPath: str,
+                      table_name: str,
+                      param_name: str) -> int:
+    """
+    Get the total number of not-null values of a parameter
+
+    Args:
+        conn: Connection to the database
+        table_name: Name of the table that holds the data
+        param_name: Name of the parameter to get the setpoints of
+
+    Returns:
+        The total number of not-null values
+    """
+    conn, cur = openDatabase(databaseAbsPath,
+                             returnDict=True)
+    sql = f"""
+           SELECT COUNT({param_name}) FROM "{table_name}"
+           WHERE {param_name} IS NOT NULL
+           """
+    cur.execute(sql)
+    rows = cur.fetchall()
+    closeDatabase(conn, cur)
+
+    return rows[0][f'COUT({param_name})']
+
+
+
+def getTableMaxId(databaseAbsPath: str,
+                     table_name: str) -> int:
+    """
+    Get the max id of a table
+
+    Args:
+        databaseAbsPath: database absolute path
+        table_name: Name of the table that holds the data
+
+    Returns:
+        The max id of a table
+    """
+    conn, cur = openDatabase(databaseAbsPath,
+                             returnDict=True)
+    sql = f"""
+           SELECT MAX(run_id)
+           FROM "{table_name}"
+           """
+    cur.execute(sql)
+    rows = cur.fetchall()
+
+    return rows[0]['max(run_id)']
+
+
+
+def getOffsetLimitForCallback(databaseAbsPath: str,
+                              table_name: str,
+                              param_name: str) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Since sqlite3 does not allow to keep track of the data loading progress,
+    we compute how many sqlite request correspond to a progress of
+    config['displayedDownloadQcodesPercentage'].
+    This function return a list of offset and a integer value of limit to
+    be used to run such SQL requests.
+
+    Args:
+        conn: Connection to the database
+        table_name: Name of the table that holds the data
+        param_name: Name of the parameter to get the setpoints of
+
+    Returns:
+        offset: list of SQL offset corresponding to a progress of
+            config['displayedDownloadQcodesPercentage']
+        limit: SQL limit corresponding to a progress of
+            config['displayedDownloadQcodesPercentage']
+    """
+
+    # First, we get the number of row to be downloaded for the wanted
+    # dependent parameter
+    nb_row = getParameterDbRow(databaseAbsPath,
+                               table_name,
+                               param_name)
+
+    # Second, we get the max id of the table
+    max_id = getTableMaxId(databaseAbsPath,
+                           table_name)
+
+    # Third, we create a list of offset corresponding to a progress of
+    # config['displayedDownloadQcodesPercentage']
+    if nb_row >= 100:
+
+        # Using linspace with dtype=int ensure of having an array finishing
+        # by max_id
+        offset = np.linspace(0, max_id, int(100 / config['displayedDownloadQcodesPercentage']) + 1, dtype=int)
+
+    else:
+        # If there is less than 100 row to be downloaded, we overwrite the
+        # config['displayedDownloadQcodesPercentage'] to avoid many calls for small download
+        offset = np.array([0, nb_row // 2, nb_row])
+
+    # The number of row downloaded between two iterations may vary
+    # We compute the limit corresponding to each offset
+    limit = offset[1:] - offset[:-1]
+
+    return offset, limit
+
+
+
 def getRunInfosmp(databaseAbsPath: str,
                   queueData: mp.Queue,
                   queueProgressBar: mp.Queue,
                   queueDone: mp.Queue) -> None:
     """
     Get a handfull of information about all the run of a database.
     Return None if database is empty.
@@ -329,15 +551,15 @@
     callEvery = int(total/100*config['displayedDownloadQcodesPercentage'])
 
     # For small database
     if callEvery==0:
         callEvery = total
 
     ## Get runs infos
-    request = "SELECT run_id, exp_id, name, completed_timestamp, run_timestamp, result_table_name, run_description FROM 'runs'"
+    request = "SELECT run_id, exp_id, name, completed_timestamp, run_timestamp, result_table_name, run_description, captured_run_id, guid FROM 'runs'"
     runInfos: List[dict] = [{}]*total
     ids = np.arange(0, total, callEvery)
     if ids[-1]!=total:
         ids = np.append(ids, total)
     iteration = 100/len(ids)
     for i in range(len(ids)-1):
         cur.execute('{0} LIMIT {1} OFFSET {2}'.format(request,
@@ -391,16 +613,19 @@
     for slice in range(len(result_table_names)//config['maximumRunPerRequest']+1):
         for runInfo, runRecords in zip(runInfos[slice*config['maximumRunPerRequest']:(slice+1)*config['maximumRunPerRequest']], records[slice]):
             infos[runInfo['run_id']] = {'nb_independent_parameter' : getNbIndependentFromRow(runInfo),
                                         'nb_dependent_parameter' : getNbDependentFromRow(runInfo),
                                         'experiment_name' : experimentInfos[runInfo['exp_id']-1]['name'],
                                         'sample_name' : experimentInfos[runInfo['exp_id']-1]['sample_name'],
                                         'run_name' : runInfo['name'],
+                                        'captured_run_id' : str(runInfo['captured_run_id']),
+                                        'guid' : runInfo['guid'],
                                         'started' : timestamp2string(runInfo['run_timestamp']),
                                         'completed' : timestamp2string(runInfo['completed_timestamp']),
+                                        'duration'  : timestamps2duration(runInfo['completed_timestamp'], runInfo['run_timestamp']),
                                         'records' : runRecords}
 
 
     # stop = time.time()
     # print(stop-start)
     # start = time.time()
     queueData.put(infos)
@@ -477,63 +702,118 @@
     # for 2d
     elif len(paramIndependentName)==2:
         request = 'SELECT {0},{1},{2} FROM "{3}" WHERE {2} IS NOT NULL'.format(paramIndependentName[0],
                                                                                paramIndependentName[1],
                                                                                paramDependentName,
                                                                                table_name)
 
-    conn, cur = openDatabase(databaseAbsPath)
-    # For small run, we download all at once
-    if nbPoint<=100:
-        cur.execute(request)
-        d = np.array(cur.fetchall())
-
-        queueProgressBar.put(queueProgressBar.get() + 100)
-    else:
-        # We download the data while updating the progress bar
-        # First, we compute the id limits to download the data in
-        # 100/config['displayedDownloadQcodesPercentage'] request
-        d = np.empty((nbPoint, len(paramIndependentName)+1))
-        ids = np.arange(0, nbPoint, callEvery)
-        if ids[-1]!=nbPoint:
-            ids = np.append(ids, nbPoint)
-        iteration = 100/len(ids)
-        for i in range(len(ids)-1):
-            cur.execute('{0} LIMIT {1} OFFSET {2}'.format(request,
-                                                        callEvery,
-                                                        ids[i]))
-            d[ids[i]:ids[i+1],] = np.array(cur.fetchall())
+    # First, we try to download the data ourself
+    try:
+        conn, cur = openDatabase(databaseAbsPath)
+        # For small run, we download all at once
+        if nbPoint<=100:
+            cur.execute(request)
+            d = np.array(cur.fetchall())
+
+            queueProgressBar.put(queueProgressBar.get() + 100)
+        else:
+            # We download the data while updating the progress bar
+            # First, we compute the id limits to download the data in
+            # 100/config['displayedDownloadQcodesPercentage'] request
+            d = np.empty((nbPoint, len(paramIndependentName)+1))
+            ids = np.arange(0, nbPoint, callEvery)
+            if ids[-1]!=nbPoint:
+                ids = np.append(ids, nbPoint)
+            iteration = 100/len(ids)
+            for i in range(len(ids)-1):
+                cur.execute('{0} LIMIT {1} OFFSET {2}'.format(request,
+                                                            callEvery,
+                                                            ids[i]))
+                d[ids[i]:ids[i+1],] = np.array(cur.fetchall())
 
-            queueProgressBar.put(queueProgressBar.get() + iteration)
+                queueProgressBar.put(queueProgressBar.get() + iteration)
 
-    queueProgressBar.get()
-    queueProgressBar.put(100)
+        queueProgressBar.get()
+        queueProgressBar.put(100)
 
-    closeDatabase(conn, cur)
+        closeDatabase(conn, cur)
 
-    # We do not handle bytes data yet
-    if isinstance(d[0][0], np.bytes_):
+        # We do not handle bytes data yet
+        if isinstance(d[0][0], np.bytes_):
 
-        queueProgressBar.get()
-        queueProgressBar.put(0)
-        queueMessage.get()
-        queueMessage.put('Binary data detected, give me time here...')
-
-        # We transform the binary data to float
-        for i in range(d.shape[1]):
-            out = io.BytesIO(d[0][i])
-            out.seek(0)
-            if i==0:
-                t = np.load(out)
-            else:
-                t = np.vstack((t, np.load(out))).T
-        d = t
+            queueProgressBar.get()
+            queueProgressBar.put(0)
+            queueMessage.get()
+            queueMessage.put('Binary data detected, give me time here...')
+
+            # We transform the binary data to float
+            for i in range(d.shape[1]):
+                out = io.BytesIO(d[0][i])
+                out.seek(0)
+                if i==0:
+                    t = np.load(out)
+                else:
+                    t = np.vstack((t, np.load(out))).T
+            d = t
+            queueProgressBar.get()
+            queueProgressBar.put(100)
+    # If error, we load qcodes (slow)
+    except:
+        # If the callack argument is available on qcodes
+        if int(version('qcodes').split('.')[1])>=36:
+            def callback(progress):
+                queueProgressBar.get()
+                queueProgressBar.put(progress)
+                return callback
+
+            from qcodes import initialise_or_create_database_at, load_by_id
+            initialise_or_create_database_at(databaseAbsPath)
+            ds = load_by_id(runId).get_parameter_data(paramDependentName,
+                                                      callback=callback)[paramDependentName]
+
+            # for empty dataset
+            if len(ds)==0:
+                d = np.array([])
+            # for 1d
+            elif len(paramIndependentName)==1:
+                d = np.vstack((np.ravel(ds[paramIndependentName[0]]),
+                               np.ravel(ds[paramDependentName]))).T
+            # for 2d
+            elif len(paramIndependentName)==2:
+                d = np.vstack((np.ravel(ds[paramIndependentName[0]]),
+                               np.ravel(ds[paramIndependentName[1]]),
+                               np.ravel(ds[paramDependentName]))).T
+        else:
+            queueProgressBar.get()
+            queueProgressBar.put(0)
+            queueMessage.get()
+            queueMessage.put('Format not handled, have to load QCoDeS...')
+
+            from qcodes import initialise_or_create_database_at, load_by_id
+            initialise_or_create_database_at(databaseAbsPath)
+
+            queueProgressBar.get()
+            queueProgressBar.put(50)
+            ds = load_by_id(runId).get_parameter_data()[paramDependentName]
+
+            # for empty dataset
+            if len(ds)==0:
+                d = np.array([])
+            # for 1d
+            elif len(paramIndependentName)==1:
+                d = np.vstack((np.ravel(ds[paramIndependentName[0]]),
+                               np.ravel(ds[paramDependentName]))).T
+            # for 2d
+            elif len(paramIndependentName)==2:
+                d = np.vstack((np.ravel(ds[paramIndependentName[0]]),
+                               np.ravel(ds[paramIndependentName[1]]),
+                               np.ravel(ds[paramDependentName]))).T
+            queueProgressBar.get()
+            queueProgressBar.put(100)
 
-        queueProgressBar.get()
-        queueProgressBar.put(100)
 
     queueData.put(d)
     queueDone.put(True)
 
 
 
 def getNbTotalRunmp(databaseAbsPath: str,
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/runPropertiesExtra.py` & `pyplotter-0.3.5/pyplotter/sources/runPropertiesExtra.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/widgetBlueFors.py` & `pyplotter-0.3.5/pyplotter/sources/widgetBlueFors.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
 
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
 
     signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
     signalRemoveProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar)
-    signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, str, str, str, str, bool)
+    signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     signalLoadedDataFull = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
 
     def __init__(self, parent):
         """
         Class handling the reading of csv file.
         """
 
@@ -120,14 +120,15 @@
                                                     'y' : y,
                                                     'unit' : config[fileName]['labelUnits']})
 
 
         self.signalFillTableWidgetParameter.emit(0, # runId
                                                  self.paramDependentList, # dependentList,
                                                  {}, # snapshotDict,
+                                                 {i['name'] : None for i in self.paramDependentList}, # shapes
                                                  '', # experimentName
                                                  '', # runName
                                                  absPath, # fileAbsPath
                                                  'bluefors', # dataType
                                                  doubleClick) # doubleClick
 
         self.signalRemoveProgressBar.emit(progressBar)
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/widgetCSV.py` & `pyplotter-0.3.5/pyplotter/sources/widgetCSV.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
     signalAddSnapshot = QtCore.pyqtSignal(dict)
 
     signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
     signalRemoveProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar)
-    signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, str, str, str, str, bool)
+    signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     signalLoadedDataFull = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
 
     def __init__(self, parent):
         """
         Class handling the reading of csv file.
         """
 
@@ -145,27 +145,30 @@
                 header: Union[None, int]=None
                 if c is None:
                     header = None
                 else:
                     f = open(fileAbsPath, 'r')
                     header = 0
                     d = f.readline()
-                    while d[0]==c:
+                    while d[0]==comment:
                         d = f.readline()
                         header += 1
                 f.close()
 
                 ## Guess delimiter character
                 f = open(fileAbsPath, 'r')
-                for i in range(10):
-                    d = f.readline()
+                d = f.readline()
+                for i in range(9):
+                    d += f.readline()
                 f.close()
                 delimiter = None
                 if ',' in d:
                     delimiter = ','
+                elif ';' in d:
+                    delimiter = ';'
                 else:
                     delimiter = ' '
 
                 # Get the data as panda dataframe
                 df = pd.read_csv(fileAbsPath, comment=comment, sep=delimiter, header=header)
 
                 # Get the column name as string
@@ -201,14 +204,15 @@
                                             'y' : y,
                                             'unit' : '',
                                             'name' : columnName})
 
         self.signalFillTableWidgetParameter.emit(0, # runId
                                                  self.paramDependentList, # dependentList,
                                                  {}, # snapshotDict,
+                                                 {i['name'] : None for i in self.paramDependentList}, # shapes
                                                  '', # experimentName
                                                  '', # runName
                                                  fileAbsPath, # fileAbsPath
                                                  'csv', # dataType
                                                  doubleClick) # doubleClick
 
         self.signalRemoveProgressBar.emit(progressBar)
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/widgetPlot.py` & `pyplotter-0.3.5/pyplotter/sources/widgetPlot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/widgetPlot1d.py` & `pyplotter-0.3.5/pyplotter/sources/widgetPlot1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,42 +532,45 @@
 
         self.comboBoxXAxis.setCurrentIndex(self.comboBoxXAxis.findText(self.plotItem.getAxis('bottom').labelText))
 
 
 
     def comboBoxXAxisActivated(self, autoRange: bool=False) -> None:
 
-        # Get a curve containing the data to update the plot
-        # Either in its x or y axis
-        for curve in self.curves.values():
-            # During liveplot, dataset may be None for the first iteration
-            if curve._dataset is not None:
-                if curve.curveXLabel==self.comboBoxXAxis.currentText():
-                    newXData  = curve._dataset.x
-                    newXLabel = curve.curveXLabel
-                    newXUnits = curve.curveXUnits
-                    break
-                if curve.curveYLabel==self.comboBoxXAxis.currentText():
-                    newXData  = curve._dataset.y
-                    newXLabel = curve.curveYLabel
-                    newXUnits = curve.curveYUnits
-                    break
+        # The change of x axis is enable only if there is no fit or filtering
+        # being done
+        if self.comboBoxXAxis.isEnabled():
+            # Get a curve containing the data to update the plot
+            # Either in its x or y axis
+            for curve in self.curves.values():
+                # During liveplot, dataset may be None for the first iteration
+                if curve._dataset is not None:
+                    if curve.curveXLabel==self.comboBoxXAxis.currentText():
+                        newXData  = curve.x
+                        newXLabel = curve.curveXLabel
+                        newXUnits = curve.curveXUnits
+                        break
+                    if curve.curveYLabel==self.comboBoxXAxis.currentText():
+                        newXData  = curve.y
+                        newXLabel = curve.curveYLabel
+                        newXUnits = curve.curveYUnits
+                        break
 
-        # We update the curve
-        for curve in self.curves.values():
-            # During liveplot, dataset may be None for the first iteration
-            if curve._dataset is not None:
-                # During liveplot, [:len(newXData)] handles update of the y axis
-                curve.setData(x=newXData[:len(curve._dataset.y)],
-                            y=curve._dataset.y[:len(newXData)])
-
-        # We update the x label
-        self.plotItem.setLabel(axis ='bottom',
-                               text =newXLabel,
-                               units=newXUnits)
+            # We update the curve
+            for curve in self.curves.values():
+                # During liveplot, dataset may be None for the first iteration
+                if curve._dataset is not None:
+                    # During liveplot, [:len(newXData)] handles update of the y axis
+                    curve.setData(x=newXData[:len(curve.y)],
+                                  y=curve.y[:len(newXData)])
+
+            # We update the x label
+            self.plotItem.setLabel(axis ='bottom',
+                                text =newXLabel,
+                                units=newXUnits)
 
         if autoRange:
             self.autoRange()
 
 
 
     ####################################
@@ -653,17 +656,17 @@
         the colors in config files
         """
 
         colorIndex = getCurveColorIndex([curve.colorIndex for curve in self.curves.values()],
                                         self.config)
         color = self.config['plot1dColors'][colorIndex]
 
-        mkpen = pg.mkPen(color=color, width=self.config['plotDataItemWidth'])
+        pen = pg.mkPen(color=color, width=self.config['plotDataItemWidth'])
 
-        return colorIndex, mkpen
+        return colorIndex, pen
 
 
 
     def updatePlotDataItem(self, x                  : np.ndarray,
                                  y                  : np.ndarray,
                                  curveId            : str,
                                  curveLegend        : str,
@@ -753,20 +756,24 @@
             Default True.
         hidden : bool
             If the plotDataItem is hidden.
             Default False.
         """
 
         # Get the dataPlotItem color
-        colorIndex, mkpen = self.getLineColor()
+        colorIndex, pen = self.getLineColor()
+
+        # If there is only one point, the Pen is incorrect
+        if len(x)==1:
+            pen = None
 
         # Create plotDataItem and save its reference
         self.curves[curveId] = self.plotItem.plot(x,
                                                   y,
-                                                  pen=mkpen,
+                                                  pen=pen,
                                                   useCache=True, # Improve performance
                                                   autoDownsample=True, # Improve performance
                                                 #   clipToView = True, # Improve performance
                                                   )
 
         # Create usefull attribute
         self.curves[curveId].x                  = x
@@ -775,19 +782,24 @@
         self.curves[curveId].curveXLabel        = curveXLabel
         self.curves[curveId].curveXUnits        = curveXUnits
         self.curves[curveId].curveYLabel        = curveYLabel
         self.curves[curveId].curveYUnits        = curveYUnits
         self.curves[curveId].curveLegend        = curveLegend
         self.curves[curveId].showInLegend       = showInLegend
         self.curves[curveId].hidden             = hidden
-        self.curves[curveId].mkpen              = mkpen
+        self.curves[curveId].pen                = pen
 
         self.updateListDataPlotItem(curveId)
         self.updateListXAxis()
 
+        # If there is only one point, we show symbols
+        if len(x)==1:
+            self.checkBoxSymbol.setChecked(False)
+            self.checkBoxSymbol.setChecked(True)
+
 
 
     def removePlotDataItem(self, curveId: str) -> None:
         """
         Remove a PlotDataItem identified via its "curveId".
 
         Parameters
@@ -1037,16 +1049,16 @@
             #     self.tableWidgetCurves.setItem(row, 4, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveYLabel))
             #     self.tableWidgetCurves.setItem(row, 5, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveXLabel))
             #     self.tableWidgetCurves.setItem(row, 4, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveYLabel))
             #     self.tableWidgetCurves.setItem(row, 5, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveXLabel))
 
             # self.tableWidgetCurves.setSortingEnabled(True)
             # self.tableWidgetCurves.sortByColumn(3, QtCore.Qt.DescendingOrder)
-            # self.tableWidgetCurves.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-            # self.tableWidgetCurves.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            # self.tableWidgetCurves.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            # self.tableWidgetCurves.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
 
         # else:
         #     if hasattr(self, 'tabCurves'):
         #         self.tabWidget.removeTab(1)
         #         del(self.tabCurves)
 
@@ -1181,15 +1193,15 @@
             rightCurveId = list(self.curves.keys())[1]
 
             if self.checkBoxSplitYAxis.isChecked():
 
                 self.groupBoxCurveInteraction.setEnabled(False)
 
                 # Create an empty plotDataItem which will contain the right curve
-                self.curveRight = pg.PlotDataItem(pen=self.curves[rightCurveId].mkpen)
+                self.curveRight = pg.PlotDataItem(pen=self.curves[rightCurveId].pen)
 
                 # Create and set links for a second viewbox which will contains the right curve
                 self.vbRight = pg.ViewBox()
                 self.vbRight.setXLink(self.plotItem)
                 self.plotItem.scene().addItem(self.vbRight)
                 self.plotItem.showAxis('right')
                 self.plotItem.getAxis('right').linkToView(self.vbRight)
@@ -1482,30 +1494,30 @@
             If None, put back the default plotDataItem style.
             See getCurveId from MainApp
         """
 
         if curveId is not None:
             if curveId+'-selection' not in self.curves.keys():
                 # Create new style
-                mkPen = pg.mkPen(color=self.config['plot1dColorsComplementary'][self.curves[curveId].colorIndex],
-                                style=QtCore.Qt.SolidLine ,
-                                width=self.config['plotDataItemWidth'])
+                Pen = pg.mkPen(color=self.config['plot1dColorsComplementary'][self.curves[curveId].colorIndex],
+                               style=QtCore.Qt.SolidLine ,
+                               width=self.config['plotDataItemWidth'])
 
                 self.addPlotDataItem(x            = self.selectedX,
                                      y            = self.selectedY,
                                      curveId      = curveId+'-selection',
                                      curveXLabel  = self.curves[curveId].curveXLabel,
                                      curveXUnits  = self.curves[curveId].curveXUnits,
                                      curveYLabel  = self.curves[curveId].curveYLabel,
                                      curveYUnits  = self.curves[curveId].curveYUnits,
                                      curveLegend  = 'Selection',
                                      showInLegend = True)
 
                 # Apply new style
-                self.curves[curveId+'-selection'].setPen(mkPen)
+                self.curves[curveId+'-selection'].setPen(Pen)
             else:
                 # Update the curve
                 self.curves[curveId+'-selection'].setData(x=self.selectedX,
                                                           y=self.selectedY)
         else:
             # Remove the curve
             curveIdToBeRemoved = None
@@ -1592,14 +1604,17 @@
         self.groupBoxFFT.setEnabled(enable)
         self.groupBoxCalculus.setEnabled(enable)
         self.groupBoxStatistics.setEnabled(enable)
         self.groupBoxFiltering.setEnabled(enable)
         self.groupBoxFit.setEnabled(enable)
         self.groupBoxNormalize.setEnabled(enable)
 
+        # The change of x-axis is enable only when no interaction is done
+        self.comboBoxXAxis.setEnabled(not enable)
+
 
 
     def interactionCloseAll(self) -> None:
 
         self.signalFilteringClose.emit()
         self.signalFitClose.emit()
         self.signalFFTClosePlot.emit()
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/widgetPlot2d.py` & `pyplotter-0.3.5/pyplotter/sources/widgetPlot2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         self.checkBoxDrawIsoCurve.clicked.connect(self.cbIsoCurve)
         self.checkBoxInvert.clicked.connect(lambda : self.cbcmInvert(self.checkBoxInvert))
         self.checkBoxMaximum.clicked.connect(self.checkBoxMaximumClicked)
         self.checkBoxMinimum.clicked.connect(self.checkBoxMinimumClicked)
         self.checkBoxSwapxy.clicked.connect(self.checkBoxSwapxyState)
         self.checkBoxAspectEqual.clicked.connect(self.checkBoxAspectEqualState)
         self.checkBoxSubtractAverageX.clicked.connect(self.zDataTransformation)
-        self.checkBoxSubtractAverageX.clicked.connect(self.zDataTransformation)
+        self.checkBoxSubtractAverageY.clicked.connect(self.zDataTransformation)
         self.spinBoxSubtractPolyX.valueChanged.connect(self.zDataTransformation)
         self.spinBoxSubtractPolyY.valueChanged.connect(self.zDataTransformation)
         self.checkBoxUnwrapX.clicked.connect(self.zDataTransformation)
         self.checkBoxUnwrapY.clicked.connect(self.zDataTransformation)
         self.pushButton3d.clicked.connect(self.launched3d)
         self.plotItem.scene().sigMouseClicked.connect(self.plotItemdoubleClick)
         self.radioButtonSliceSingleAny.toggled.connect(self.radioBoxSliceChanged)
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/workers/checkNbRunDatabase.py` & `pyplotter-0.3.5/pyplotter/sources/workers/checkNbRunDatabase.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/workers/loadDataBase.py` & `pyplotter-0.3.5/pyplotter/sources/workers/loadDataBase.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     Class containing the signal of the loadDataBaseThread, see below
     """
 
     # Signal used to update the status bar
     sendStatusBarMessage = QtCore.pyqtSignal(str, str)
     # Signal used to add n rows in the database table
-    addRows = QtCore.pyqtSignal(list, list, list, list, list, list, list, list, int, str)
+    addRows = QtCore.pyqtSignal(list, list, list, list, list, list, list, list, list, list, list, int, str)
     # Signal used to update the progress bar
     updateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
     # When the run method is done
     databaseClickDone = QtCore.pyqtSignal(QtWidgets.QProgressBar, bool, str, int)
 
 class LoadDataBaseThread(QtCore.QRunnable):
 
@@ -116,61 +116,76 @@
         # thread. Every config['NbRunEmit'] a signal is emitted and the list are
         # empty and the process starts again until all info have been stransferred.
         runId           = []
         dim             = []
         experimentName  = []
         sampleName      = []
         runName         = []
+        captured_run_id = []
+        guid            = []
         started         = []
         completed       = []
+        duration        = []
         runRecords      = []
         for key, val in runInfos.items():
 
             runId.append(key)
             dim.append('-'.join(str(i) for i in val['nb_independent_parameter'])+'d')
             experimentName.append(val['experiment_name'])
             sampleName.append(val['sample_name'])
             runName.append(val['run_name'])
+            captured_run_id.append(val['captured_run_id'])
+            guid.append(val['guid'])
             started.append(val['started'])
             completed.append(val['completed'])
+            duration.append(val['duration'])
             runRecords.append(str(val['records']))
 
             # If we reach enough data, we emit the signal.
             if key%config['NbRunEmit']==0:
                 self.signal.addRows.emit(runId,
                                           dim,
                                           experimentName,
                                           sampleName,
                                           runName,
+                                          captured_run_id,
+                                          guid,
                                           started,
                                           completed,
+                                          duration,
                                           runRecords,
                                           nbTotalRun,
                                           self.databaseAbsPath)
                 self.signal.updateProgressBar.emit(self.progressBar, int(runId[0]/nbTotalRun*100), 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
 
 
                 runId           = []
                 dim             = []
                 experimentName  = []
                 sampleName      = []
                 runName         = []
+                captured_run_id = []
+                guid            = []
                 started         = []
                 completed       = []
+                duration        = []
                 runRecords      = []
 
         # If there is still information to be transferred, we do so
         if len(runId)!=0:
             self.signal.addRows.emit(runId,
                                       dim,
                                       experimentName,
                                       sampleName,
                                       runName,
+                                      captured_run_id,
+                                      guid,
                                       started,
                                       completed,
+                                      duration,
                                       runRecords,
                                       nbTotalRun,
                                       self.databaseAbsPath)
             self.signal.updateProgressBar.emit(self.progressBar, int(runId[0]/nbTotalRun*100), 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
 
         # Signal that the whole database has been looked at
         self.signal.databaseClickDone.emit(self.progressBar, # progressBar
```

### Comparing `pyplotter-0.3.4/pyplotter/sources/workers/loadDataFromCache.py` & `pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromCache.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/workers/loadDataFromRun.py` & `pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromRun.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/sources/workers/loadRunInfo.py` & `pyplotter-0.3.5/pyplotter/sources/workers/loadRunInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This Python file uses the following encoding: utf-8
 from PyQt5 import QtCore
 
 from ..config import loadConfigCurrent
 config = loadConfigCurrent()
-from ..qcodesDatabase import getDependentSnapshotFromRunId
+from ..qcodesDatabase import getDependentSnapshotShapeFromRunId
 
 
 class LoadRunInfoSignal(QtCore.QObject):
     """
     Class containing the signal of the loadRunInfoThread, see below
     """
 
     # When the run method is done
-    updateRunInfo = QtCore.pyqtSignal(int, list,dict, str, str, str, str, bool)
+    updateRunInfo = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
 
 class LoadRunInfoThread(QtCore.QRunnable):
 
 
 
     def __init__(self, databaseAbsPath: str,
                        runId: int,
@@ -52,18 +52,21 @@
 
     @QtCore.pyqtSlot()
     def run(self):
         """
         Method launched by the worker.
         """
 
-        dependentList, snapshotDict = getDependentSnapshotFromRunId(self.databaseAbsPath,
-                                                                    self.runId)
+        (dependentList,
+         snapshotDict,
+         shapesDict) = getDependentSnapshotShapeFromRunId(self.databaseAbsPath,
+                                                          self.runId)
 
         self.signal.updateRunInfo.emit(self.runId,
                                        dependentList,
                                        snapshotDict,
+                                       shapesDict,
                                        self.experimentName,
                                        self.runName,
                                        self.databaseAbsPath,
                                        'qcodes', # dataType
                                        self.doubleClicked)
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/checkBoxHidden.py` & `pyplotter-0.3.5/pyplotter/ui/checkBoxHidden.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/checkBoxStared.py` & `pyplotter-0.3.5/pyplotter/ui/checkBoxStared.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogColormap.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormap.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogColormapUi.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormapUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogComment.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogComment.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogFontsize.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsize.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogFontsizeUi.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsizeUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogLiveplot.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/dialogs/dialogLiveplotUi.py` & `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplotUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/hBoxLayoutLabelPath.py` & `pyplotter-0.3.5/pyplotter/ui/hBoxLayoutLabelPath.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/labelSnapshot.py` & `pyplotter-0.3.5/pyplotter/ui/labelSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/lineEditSnapshot.py` & `pyplotter-0.3.5/pyplotter/ui/lineEditSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/mainWindow.py` & `pyplotter-0.3.5/pyplotter/ui/mainWindow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file '.\scripts\pyplotter\pyplotter\ui\mainWindow.ui'
 #
-# Created by: PyQt5 UI code generator 5.12.3
+# Created by: PyQt5 UI code generator 5.15.7
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
@@ -124,34 +125,16 @@
         self.tableWidgetParameter.setFont(font)
         self.tableWidgetParameter.setLineWidth(0)
         self.tableWidgetParameter.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.tableWidgetParameter.setAlternatingRowColors(True)
         self.tableWidgetParameter.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.tableWidgetParameter.setShowGrid(False)
         self.tableWidgetParameter.setObjectName("tableWidgetParameter")
-        self.tableWidgetParameter.setColumnCount(9)
+        self.tableWidgetParameter.setColumnCount(0)
         self.tableWidgetParameter.setRowCount(0)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(4, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(5, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(6, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(7, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetParameter.setHorizontalHeaderItem(8, item)
         self.tableWidgetParameter.horizontalHeader().setStretchLastSection(True)
         self.tableWidgetParameter.verticalHeader().setVisible(False)
         self.verticalLayout_6.addWidget(self.tableWidgetParameter)
         self.verticalLayoutWidget_2 = QtWidgets.QWidget(self.splitter)
         self.verticalLayoutWidget_2.setObjectName("verticalLayoutWidget_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.verticalLayoutWidget_2)
         self.verticalLayout_7.setContentsMargins(0, 0, 0, 0)
@@ -233,42 +216,20 @@
         self.horizontalLayout.addWidget(self.checkBoxStared)
         self.verticalLayout_11.addLayout(self.horizontalLayout)
         self.tableWidgetDataBase = TableWidgetDatabase(self.layoutWidget_3)
         font = QtGui.QFont()
         font.setPointSize(8)
         self.tableWidgetDataBase.setFont(font)
         self.tableWidgetDataBase.setLineWidth(0)
-        self.tableWidgetDataBase.setSizeAdjustPolicy(QtWidgets.QAbstractScrollArea.AdjustIgnored)
-        self.tableWidgetDataBase.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.tableWidgetDataBase.setAlternatingRowColors(True)
         self.tableWidgetDataBase.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.tableWidgetDataBase.setShowGrid(False)
-        self.tableWidgetDataBase.setColumnCount(10)
         self.tableWidgetDataBase.setObjectName("tableWidgetDataBase")
+        self.tableWidgetDataBase.setColumnCount(0)
         self.tableWidgetDataBase.setRowCount(0)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(4, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(5, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(6, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(7, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(8, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.tableWidgetDataBase.setHorizontalHeaderItem(9, item)
         self.tableWidgetDataBase.horizontalHeader().setDefaultSectionSize(80)
         self.tableWidgetDataBase.horizontalHeader().setMinimumSectionSize(32)
         self.tableWidgetDataBase.horizontalHeader().setStretchLastSection(True)
         self.tableWidgetDataBase.verticalHeader().setVisible(False)
         self.verticalLayout_11.addWidget(self.tableWidgetDataBase)
         self.verticalLayout_4.addWidget(self.splitter_2)
         MainWindow.setCentralWidget(self.centralwidget)
@@ -293,58 +254,20 @@
         self.tableWidgetFolder.setSortingEnabled(True)
         item = self.tableWidgetFolder.horizontalHeaderItem(0)
         item.setText(_translate("MainWindow", "item"))
         item = self.tableWidgetFolder.horizontalHeaderItem(1)
         item.setText(_translate("MainWindow", "size"))
         self.labelRun.setText(_translate("MainWindow", "Browse parameters run:"))
         self.tableWidgetParameter.setSortingEnabled(True)
-        item = self.tableWidgetParameter.horizontalHeaderItem(0)
-        item.setText(_translate("MainWindow", "run id"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(1)
-        item.setText(_translate("MainWindow", "experiment name"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(2)
-        item.setText(_translate("MainWindow", "parameter name"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(3)
-        item.setText(_translate("MainWindow", "databaseAbsPath"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(4)
-        item.setText(_translate("MainWindow", "dataType"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(5)
-        item.setText(_translate("MainWindow", "plotted"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(6)
-        item.setText(_translate("MainWindow", "axis"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(7)
-        item.setText(_translate("MainWindow", "unit"))
-        item = self.tableWidgetParameter.horizontalHeaderItem(8)
-        item.setText(_translate("MainWindow", "swept parameters"))
         self.labelMetadata.setText(_translate("MainWindow", "Browse metadata run:"))
         self.labelSnapshot.setText(_translate("MainWindow", "Filter:"))
         self.labelDataBase.setText(_translate("MainWindow", "Browse database:"))
         self.checkBoxHidden.setText(_translate("MainWindow", "Show hidden"))
         self.checkBoxStared.setText(_translate("MainWindow", "Show only stared run"))
         self.tableWidgetDataBase.setSortingEnabled(True)
-        item = self.tableWidgetDataBase.horizontalHeaderItem(0)
-        item.setText(_translate("MainWindow", "dataBaseAbsPath"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(1)
-        item.setText(_translate("MainWindow", "run id"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(2)
-        item.setText(_translate("MainWindow", "dim"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(3)
-        item.setText(_translate("MainWindow", "experiment"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(4)
-        item.setText(_translate("MainWindow", "sample"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(5)
-        item.setText(_translate("MainWindow", "run name"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(6)
-        item.setText(_translate("MainWindow", "started"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(7)
-        item.setText(_translate("MainWindow", "completed"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(8)
-        item.setText(_translate("MainWindow", "records"))
-        item = self.tableWidgetDataBase.horizontalHeaderItem(9)
-        item.setText(_translate("MainWindow", "Comments"))
 from ..ui.checkBoxHidden import CheckBoxHidden
 from ..ui.checkBoxStared import CheckBoxStared
 from ..ui.labelSnapshot import LabelSnapshot
 from ..ui.lineEditSnapshot import LineEditSnapshot
 from ..ui.menuBar import MenuBar
 from ..ui.pushButtonOpenFolder import pushButtonOpenFolder
 from ..ui.statusBar import StatusBar
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/menuBar.py` & `pyplotter-0.3.5/pyplotter/ui/menuBar.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 
 from ..sources.config import loadConfigCurrent, updateUserConfig
 config = loadConfigCurrent()
 
 from .dialogs.dialogFontsize import DialogFontSize
 from .dialogs.dialogColormap import DialogMenuColormap
 from .dialogs.dialogLiveplot import DialogLiveplot
+from .dialogs.dialogMenuDatabaseDisplay import DialogMenuDatabaseDisplay
 
 
 class MenuBar(QtWidgets.QMenuBar):
 
-    signalUpdateStyle        = QtCore.pyqtSignal(dict)
-    signalOpenDialogLivePlot = QtCore.pyqtSignal()
+    signalUpdateStyle               = QtCore.pyqtSignal(dict)
+    signalUpdateTableWidgetDatabase = QtCore.pyqtSignal(dict)
+    signalOpenDialogLivePlot        = QtCore.pyqtSignal()
 
     signal2MainWindowAddPlot   = QtCore.pyqtSignal(int, str, str, str, str, str, tuple, str, str, str, str, str, str)
 
     signalUpdateCurve          = QtCore.pyqtSignal(str, str, str, np.ndarray, np.ndarray, bool, bool)
     signalUpdate2d             = QtCore.pyqtSignal(str, np.ndarray, np.ndarray, np.ndarray)
     signalUpdatePlotProperty   = QtCore.pyqtSignal(str, str, str)
 
@@ -46,26 +48,30 @@
         self.actionFontsize = self.menuPlot.addAction('Fontsize')
         self.actionColormap = self.menuPlot.addAction('Colormap')
         self.menuPreferences.addAction(self.menuPlot.menuAction())
 
         self.menuLiveplot    = self.addMenu('Liveplot')
         self.actionOpenliveplot = self.menuLiveplot.addAction('Open liveplot')
 
+        self.actionDatabase = self.menuPreferences.addAction('Database display')
+
         self.actionqb.triggered.connect(self.menuBackgroundQb)
         self.actionqdark.triggered.connect(self.menuBackgroundQdark)
         self.actionwhite.triggered.connect(self.menuBackgroundWhite)
         self.actionDefaultPath.triggered.connect(self.menuDefaultPath)
+        self.actionDatabase.triggered.connect(self.menuDatabase)
         self.actionAxisLabelColor.triggered.connect(self.menuAxisLabelColor)
         self.actionAxisTickLabelsColor.triggered.connect(self.menuAxisTickLabelsColor)
         self.actionAxisTicksColor.triggered.connect(self.menuAxisTicksColor)
         self.actionTitleColor.triggered.connect(self.menuTitleColor)
         self.actionFontsize.triggered.connect(self.menuFontsize)
         self.actionColormap.triggered.connect(self.menuColormap)
         self.actionOpenliveplot.triggered.connect(self.menuOpenLiveplot)
 
+
         if config['style']=='qbstyles':
             self.actionqb.setChecked(True)
             self.actionqb.setEnabled(False)
         elif config['style']=='qdarkstyle':
             self.actionqdark.setChecked(True)
             self.actionqdark.setEnabled(False)
         elif config['style']=='white':
@@ -135,14 +141,22 @@
         if path != '':
 
             updateUserConfig('path', os.path.abspath(path))
             updateUserConfig('root', os.path.splitdrive(path)[0])
 
 
 
+    def menuDatabase(self):
+
+        self.dialogMenuDatabaseDisplay = DialogMenuDatabaseDisplay(self.parent(), config)
+        self.dialogMenuDatabaseDisplay.signalUpdateTableWidgetDatabase.connect(self.signalUpdateTableWidgetDatabase.emit)
+        self.dialogMenuDatabaseDisplay.signalUpdateStyle.connect(self.signalUpdateStyle.emit)
+
+
+
     def menuAxisLabelColor(self):
 
         color = QtWidgets.QColorDialog.getColor()
 
         if color.isValid():
 
             for label in ('pyqtgraphxLabelTextColor',
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/menuDb.py` & `pyplotter-0.3.5/pyplotter/ui/menuDb.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/bluefors.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/bluefors.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/csv.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/csv.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/database.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/database.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/databaseOpened.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpened.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/databaseOpenedStared.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpenedStared.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/databaseStared.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/databaseStared.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/folder.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/folder.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/folderEnhanced.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/folderEnhanced.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/icon.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/icon.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/icon.py` & `pyplotter-0.3.5/pyplotter/ui/pictures/icon.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/s2p.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/s2p.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/star.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/star.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pictures/trash.png` & `pyplotter-0.3.5/pyplotter/ui/pictures/trash.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/dialogFiltering.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFiltering.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/dialogFit.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFit.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxCalculus.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculus.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxCalculusUi.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculusUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFFT.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFT.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFFTUi.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFTUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFiltering.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFiltering.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxFit.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFit.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxNormalize.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalize.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxNormalizeUi.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalizeUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxStatistics.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatistics.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/groupBoxStatisticsUi.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatisticsUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/widgetTabCurve.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         self.tabWidget = tabWidget
         self.plotRef = plotRef
 
         ## Only used to propagate information
         # curveId
         self.tableWidgetCurves.setColumnHidden(0, True)
 
-        self.tableWidgetCurves.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-        self.tableWidgetCurves.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.tableWidgetCurves.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.tableWidgetCurves.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
 
 
     def updateList1dCurvesLabels(self, plotRef: str,
                                        plotCurvesId: List[str],
                                        plots: list) -> None:
 
@@ -121,16 +121,16 @@
                 self.tableWidgetCurves.setItem(row, 4, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveYLabel))
                 self.tableWidgetCurves.setItem(row, 5, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveXLabel))
                 self.tableWidgetCurves.setItem(row, 4, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveYLabel))
                 self.tableWidgetCurves.setItem(row, 5, QtWidgets.QTableWidgetItem(currentPlot.curves[curveId2Build].curveXLabel))
 
             self.tableWidgetCurves.setSortingEnabled(True)
             self.tableWidgetCurves.sortByColumn(3, QtCore.Qt.DescendingOrder)
-            self.tableWidgetCurves.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-            self.tableWidgetCurves.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            self.tableWidgetCurves.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            self.tableWidgetCurves.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
             # Remove the curve
             for curveId2Remove in curveId2Removes:
                 self.signalRemovePlotDataItem.emit(plotRef,
                                                    curveId2Remove)
 
             if self.tabWidget.count()==1:
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/plot1d/widgetTabCurveUi.py` & `pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurveUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/pushButtonOpenFolder.py` & `pyplotter-0.3.5/pyplotter/ui/pushButtonOpenFolder.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/statusBar.py` & `pyplotter-0.3.5/pyplotter/ui/statusBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,16 +171,18 @@
     def removeProgressBar(self, progressBar: QtWidgets.QProgressBar) -> None:
         """
         Remove the progress bar in the status bar.
         Usually called after a thread has loaded something.
         """
         self.removeWidget(progressBar)
         del(progressBar)
-        self.removeWidget(self.progressBarLabel)
-        del(self.progressBarLabel)
+
+        if hasattr(self, 'progressBarLabel'):
+            self.removeWidget(self.progressBarLabel)
+            del(self.progressBarLabel)
 
 
 
     @QtCore.pyqtSlot(QtWidgets.QProgressBar, int, str)
     def updateProgressBar(self, progressBar: QtWidgets.QProgressBar,
                                 val: int,
                                 text: str) -> None:
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/tableWidgetDatabase.py` & `pyplotter-0.3.5/pyplotter/ui/tableWidgetDatabase.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,25 +13,14 @@
 from ..sources.workers.checkNbRunDatabase import dataBaseCheckNbRunThread
 from ..sources.functions import clearTableWidget, getDatabaseNameFromAbsPath
 from ..ui.dialogs.dialogComment import DialogComment
 
 # Get the folder path for pictures
 PICTURESPATH = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'pictures')
 
-# Column index
-COLUMNDATABASEABSPATH = 0
-COLUMNITEMRUNID       = 1
-COLUMNDIM             = 2
-COLUMNEXPERIMENTNAME  = 3
-COLUMNSAMPLENAME      = 4
-COLUMNRUNNAME         = 5
-COLUMNSTARTED         = 6
-COLUMNCOMPLETED       = 7
-COLUMNRUNRECORDS      = 8
-COLUMNCOMMENT         = 9
 
 class TableWidgetDatabase(QtWidgets.QTableWidget):
     """
     Custom class to be able to sort numerical table column
     """
 
     # Propagated to statusBarMain
@@ -40,15 +29,15 @@
     signalUpdateProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
     signalRemoveProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     # Propagated to tableWidgetFolder, checkBoxHidden, checkBoxStared
     signalDatabaseClickDone = QtCore.pyqtSignal()
     # Propagated to labelCurrentDataBase
     signalUpdateCurrentDatabase = QtCore.pyqtSignal(str)
     # Propagated to tableWidgetParameter
-    signalRunClick = QtCore.pyqtSignal(int, list, dict, str, str, str, str, bool)
+    signalRunClick = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     # Propagated to tableWidgetFolder
     signalDatabaseStars   = QtCore.pyqtSignal()
     signalDatabaseUnstars = QtCore.pyqtSignal()
     # Propagated to checkBoxStared
     signalCheckBoxHiddenChecked = QtCore.pyqtSignal(bool)
     # Propagated to checkBoxHidden
     signalCheckBoxStaredChecked = QtCore.pyqtSignal(bool)
@@ -60,14 +49,16 @@
     # Internal event, see keyPressEvent
     keyPressed = QtCore.pyqtSignal(str, int)
 
 
     def __init__(self, parent=None) -> None:
         super(TableWidgetDatabase, self).__init__(parent)
 
+        # Forbid editing of the cells
+        self.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
 
         # When user wants to look at a run
         self.cellClicked.connect(self.runClick)
 
         # When user wants to hide or stars a run
         self.keyPressed.connect(self.tableWidgetDataBasekeyPress)
 
@@ -82,17 +73,31 @@
 
         self.properties = RunPropertiesExtra()
         self.threadpool = QtCore.QThreadPool()
 
 
 
     def first_call(self):
-        ## Only used to propagate information
-        # Contain the databaseAbsPath
-        self.setColumnHidden(COLUMNDATABASEABSPATH, True)
+        """
+        Call when the widget is initially display
+        Build the columns foolowing the config file
+        """
+        self.setColumnCount(len(config['DatabaseDisplayColumn']))
+
+        for val in config['DatabaseDisplayColumn'].values():
+
+            # Add a column
+            item = QtWidgets.QTableWidgetItem()
+
+            # Set its header
+            self.setHorizontalHeaderItem(val['index'], item)
+            item.setText(val['name'])
+
+            # Hide or display some column
+            self.setColumnHidden(val['index'], False==val['visible'])
 
 
 
     def keyPressEvent(self, event):
         super(TableWidgetDatabase, self).keyPressEvent(event)
 
         # Emit the pressed key in human readable format in lower case
@@ -112,16 +117,16 @@
                                  os.path.basename(databaseAbsPath))
 
         # Remove all previous row in the table
         clearTableWidget(self)
 
         # Modify the resize mode so that the initial view has an optimized
         # column width
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.Fixed)
-        self.verticalHeader().setResizeMode(QtWidgets.QHeaderView.Fixed)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
+        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
 
         # Create a thread which will read the database
         worker = LoadDataBaseThread(databaseAbsPath,
                                     progressBar)
 
         # Connect signals
         worker.signal.sendStatusBarMessage.connect(self.signalSendStatusBarMessage)
@@ -130,70 +135,92 @@
         worker.signal.databaseClickDone.connect(self.databaseClickDone)
 
         # Execute the thread
         self.threadpool.start(worker)
 
 
 
-    QtCore.pyqtSlot(list, list, list, list, list, list, list, list, int, str)
-    def databaseClickAddRows(self, lrunId          : List[int],
-                                   ldim            : List[str],
-                                   lexperimentName : List[str],
-                                   lsampleName     : List[str],
-                                   lrunName        : List[str],
-                                   lstarted        : List[str],
-                                   lcompleted      : List[str],
-                                   lrunRecords     : List[str],
-                                   nbTotalRun      : int,
-                                   databaseAbsPath : str) -> None:
+    QtCore.pyqtSlot(list, list, list, list, list, list, list, list, list, list, list, int, str)
+    def databaseClickAddRows(self, lrunId           : List[int],
+                                   ldim             : List[str],
+                                   lexperimentName  : List[str],
+                                   lsampleName      : List[str],
+                                   lrunName         : List[str],
+                                   lcaptured_run_id : List[str],
+                                   lguid            : List[str],
+                                   lstarted         : List[str],
+                                   lcompleted       : List[str],
+                                   lduration        : List[str],
+                                   lrunRecords      : List[str],
+                                   nbTotalRun       : int,
+                                   databaseAbsPath  : str) -> None:
         """
         Called by another thread to fill the database table.
         Each call add n rows into the table.
         """
 
 
         if lrunId[0]==1:
             # self.statusBarMain.clearMessage()
             self.setRowCount(nbTotalRun)
 
         # We go through all lists of parameters and for each list element, we add
         # a row in the table
-        for (runId, dim, experimentName, sampleName, runName, started, completed,
-             runRecords) in zip(lrunId,
-             ldim, lexperimentName, lsampleName, lrunName, lstarted, lcompleted,
-             lrunRecords):
+        for (runId, dim, experimentName, sampleName, runName, captured_run_id,
+             guid, started, completed, duration, runRecords) in zip(lrunId,
+             ldim, lexperimentName, lsampleName, lrunName, lcaptured_run_id,
+             lguid, lstarted, lcompleted, lduration, lrunRecords):
 
             itemRunId = TableWidgetItemNumOrdered(str(runId))
 
             # If the run has been stared by an user
             if runId in self.properties.getRunStared():
                 itemRunId.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'star.png')))
                 itemRunId.setForeground(QtGui.QBrush(QtGui.QColor(*config['runStaredColor'])))
             # If the user has hidden a row
             elif runId in self.properties.getRunHidden():
                 itemRunId.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'trash.png')))
                 itemRunId.setForeground(QtGui.QBrush(QtGui.QColor(*config['runHiddenColor'])))
             else:
                 itemRunId.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'empty.png')))
 
-            self.setItem(runId-1, COLUMNDATABASEABSPATH, QtWidgets.QTableWidgetItem(databaseAbsPath))
-            self.setItem(runId-1, COLUMNITEMRUNID, itemRunId)
-            self.item(runId-1, COLUMNITEMRUNID).setToolTip('Type "s" to star a run and "h" to hide it.')
-            self.setItem(runId-1, COLUMNDIM, QtWidgets.QTableWidgetItem(dim))
-            self.setItem(runId-1, COLUMNEXPERIMENTNAME, QtWidgets.QTableWidgetItem(experimentName))
-            self.setItem(runId-1, COLUMNSAMPLENAME, QtWidgets.QTableWidgetItem(sampleName))
-            self.setItem(runId-1, COLUMNRUNNAME, QtWidgets.QTableWidgetItem(runName))
-            self.setItem(runId-1, COLUMNSTARTED, QtWidgets.QTableWidgetItem(started))
-            self.setItem(runId-1, COLUMNCOMPLETED, QtWidgets.QTableWidgetItem(completed))
-            self.setItem(runId-1, COLUMNRUNRECORDS, TableWidgetItemNumOrdered(runRecords))
-            self.setItem(runId-1, COLUMNCOMMENT, QtWidgets.QTableWidgetItem(self.properties.getRunComment(runId)))
-            self.item(runId-1, COLUMNCOMMENT).setToolTip('Double-click on the "Comments" column to add or modify a comment attached to a run')
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['databaseAbsPath']['index'], QtWidgets.QTableWidgetItem(databaseAbsPath))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['itemRunId']['index'],       itemRunId)
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['dimension']['index'],       QtWidgets.QTableWidgetItem(dim))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['experimentName']['index'],  QtWidgets.QTableWidgetItem(experimentName))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['sampleName']['index'],      QtWidgets.QTableWidgetItem(sampleName))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['runName']['index'],         QtWidgets.QTableWidgetItem(runName))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['captured_run_id']['index'], QtWidgets.QTableWidgetItem(captured_run_id))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['guid']['index'],            QtWidgets.QTableWidgetItem(guid))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['started']['index'],         QtWidgets.QTableWidgetItem(started))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['completed']['index'],       QtWidgets.QTableWidgetItem(completed))
+
+            # All of that to get colored duration
+            widgetText =  QtWidgets.QLabel()
+            widgetText.setTextFormat(QtCore.Qt.RichText)
+            widgetText.setText(duration)
+            self.setCellWidget(runId-1, config['DatabaseDisplayColumn']['duration']['index'], widgetText)
+
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['runRecords']['index'],      TableWidgetItemNumOrdered(runRecords))
+            self.setItem(runId-1, config['DatabaseDisplayColumn']['comment']['index'],         QtWidgets.QTableWidgetItem(self.properties.getRunComment(runId)))
+
+            # Hide some run
             if runId in self.properties.getRunHidden():
                 self.setRowHidden(runId-1, True)
 
+            # Set vertical and horizontal alignment
+            for i in range(config['DatabaseDisplayColumn']['comment']['index']):
+                if i!=config['DatabaseDisplayColumn']['duration']['index']:
+                    self.item(runId-1, i).setTextAlignment(QtCore.Qt.AlignVCenter)
+                else:
+                    self.cellWidget(runId-1, i).setAlignment(QtCore.Qt.AlignVCenter|QtCore.Qt.AlignRight)
+
+            # Set some tooltip
+            self.item(runId-1,    config['DatabaseDisplayColumn']['itemRunId']['index']).setToolTip('Type "s" to star a run and "h" to hide it.')
+            self.item(runId-1, config['DatabaseDisplayColumn']['comment']['index']).setToolTip('Double-click on the "Comments" column to add or modify a comment attached to a run')
 
 
     @QtCore.pyqtSlot(QtWidgets.QProgressBar, bool, str, int)
     def databaseClickDone(self,progressBar    : QtWidgets.QProgressBar,
                                error          : bool,
                                databaseAbsPath: str,
                                nbTotalRun     : int) -> None:
@@ -211,17 +238,17 @@
             Simply stored for other purposes and to avoid other sql queries.
         """
 
         self.signalRemoveProgressBar.emit(progressBar)
 
         if not error:
             self.setSortingEnabled(True)
-            self.sortItems(COLUMNITEMRUNID, QtCore.Qt.DescendingOrder)
-            self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-            self.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            self.sortItems(config['DatabaseDisplayColumn']['itemRunId']['index'], QtCore.Qt.DescendingOrder)
+            self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+            self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
 
             self.signalSendStatusBarMessage.emit('Ready', 'green')
 
 
         # We store the total number of run
         self.nbTotalRun = nbTotalRun
@@ -296,26 +323,26 @@
         # When the user click on another database while having already clicked
         # on a run, the runClick event is happenning even if no run have been clicked
         # This is due to the "currentCellChanged" event handler.
         # We catch that false event and return nothing
         if self._databaseClicking:
             return
 
-        databaseAbsPath = self.item(currentRow, COLUMNDATABASEABSPATH).text()
-        runId           = int(self.item(currentRow, COLUMNITEMRUNID).text())
-        experimentName  = self.item(currentRow, COLUMNEXPERIMENTNAME).text()
-        runName         = self.item(currentRow, COLUMNRUNNAME).text()
+        databaseAbsPath = self.item(currentRow, config['DatabaseDisplayColumn']['databaseAbsPath']['index']).text()
+        runId           = int(self.item(currentRow, config['DatabaseDisplayColumn']['itemRunId']['index']).text())
+        experimentName  = self.item(currentRow, config['DatabaseDisplayColumn']['experimentName']['index']).text()
+        runName         = self.item(currentRow, config['DatabaseDisplayColumn']['runName']['index']).text()
 
         # We check if use click or doubleClick
         doubleClick = False
         if currentRow==self.lastClickRow:
             if time() - self.lastClickTime<0.5:
                 # If we detect a double click on the "Comments" column
                 # We do not launch a plot but open a comment dialog
-                if currentColumn==COLUMNCOMMENT:
+                if currentColumn==config['DatabaseDisplayColumn']['comment']['index']:
                     self.dialogComment = DialogComment(runId,
                                                        self.properties.getRunComment(runId))
                     self.dialogComment.signalCloseDialogComment.connect(self.slotCloseCommentDialog)
                     self.dialogComment.signalUpdateDialogComment.connect(self.slotUpdateCommentDialog)
                 else:
                     doubleClick = True
                     # When user doubleclick on a run, we disable the row to avoid
@@ -339,16 +366,14 @@
         worker.signal.updateRunInfo.connect(self.signalRunClick)
 
         # Execute the thread
         self.threadpool.start(worker)
 
 
 
-
-
     def tableWidgetDataBasekeyPress(self, key: str,
                                           row : int) -> None:
         """
         Call when user presses a key while having the focus on the database table.
         Towo keys are handle:
             "h" to hide/unhide a run
             "s" to star/unstar a run
@@ -357,28 +382,28 @@
         ----------
         key : str
             Pressed key in human readable format.
         row : int
             Row of the database table in which the key happened.
         """
 
-        runId = int(self.item(row, COLUMNITEMRUNID).text())
+        runId = int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text())
 
         # If user wants to star a run
         if key==config['keyPressedStared'].lower():
 
             # If the run was already stared
             # We remove the star of the table
             # We remove the runId from the json
             if runId in self.properties.getRunStared():
 
                 # We remove the star from the row
                 item = TableWidgetItemNumOrdered(str(runId))
                 item.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'empty.png')))
-                self.setItem(row, COLUMNITEMRUNID, item)
+                self.setItem(row, config['DatabaseDisplayColumn']['itemRunId']['index'], item)
 
                 # We update the json
                 self.properties.jsonRemoveStaredRun(runId)
 
                 # If the database does not contain stared run anymore, we modify
                 # its icon
                 if len(self.properties.getRunStared())==0:
@@ -387,15 +412,15 @@
             # If the user wants to stared the run
             else:
 
                 # We put a star in the row
                 item = TableWidgetItemNumOrdered(str(runId))
                 item.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'star.png')))
                 item.setForeground(QtGui.QBrush(QtGui.QColor(*config['runStaredColor'])))
-                self.setItem(row, COLUMNITEMRUNID, item)
+                self.setItem(row, config['DatabaseDisplayColumn']['itemRunId']['index'], item)
 
                 # We update the json
                 self.properties.jsonAddStaredRun(runId)
 
                 # If the database containing the stared run is displayed, we star it
                 self.signalDatabaseStars.emit()
 
@@ -407,25 +432,25 @@
             # We unhide the row
             # We remove the runId from the json
             if runId in self.properties.getRunHidden():
 
                 item = TableWidgetItemNumOrdered(str(runId))
                 item.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'empty.png')))
                 item.setForeground(QtGui.QBrush(QtGui.QColor(255, 255, 255)))
-                self.setItem(row, COLUMNITEMRUNID, item)
+                self.setItem(row, config['DatabaseDisplayColumn']['itemRunId']['index'], item)
 
                 # We update the json
                 self.properties.jsonRemoveHiddenRun(runId)
             else:
 
                 # We modify the item and hide the row
                 item = TableWidgetItemNumOrdered(str(runId))
                 item.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, 'trash.png')))
                 item.setForeground(QtGui.QBrush(QtGui.QColor(*config['runHiddenColor'])))
-                self.setItem(row, COLUMNITEMRUNID, item)
+                self.setItem(row, config['DatabaseDisplayColumn']['itemRunId']['index'], item)
 
                 # We update the json
                 self.properties.jsonAddHiddenRun(runId)
 
 
             # We hide the row only if the user didn't check the checkboxhidden
             self.signalCheckBoxHiddenHideRow.emit()
@@ -445,15 +470,15 @@
     def slotRunClickDone(self) -> None:
         """
         Called by MainWindow when user has doubleClicked on a row.
         Enable the row again if the use didn't change the database in the meantime.
         """
 
         if hasattr(self, 'doubleClickCurrentRow'):
-            if self.doubleClickDatabaseAbsPath==self.item(self.doubleClickCurrentRow, COLUMNDATABASEABSPATH).text():
+            if self.doubleClickDatabaseAbsPath==self.item(self.doubleClickCurrentRow, config['DatabaseDisplayColumn']['databaseAbsPath']['index']).text():
                 self.cellClicked.connect(self.runClick)
             del(self.doubleClickCurrentRow)
             del(self.doubleClickDatabaseAbsPath)
 
 
 
     @QtCore.pyqtSlot(int)
@@ -470,25 +495,25 @@
         # If user wants to see hidden run
         if state==2:
 
             self.signalCheckBoxHiddenChecked.emit(True)
 
             for row in range(nbTotalRow):
 
-                if int(self.item(row, COLUMNITEMRUNID).text()) in runHidden:
+                if int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text()) in runHidden:
                     self.setRowHidden(row, False)
 
         # Hide hidden run again
         elif state==0:
 
             self.signalCheckBoxHiddenChecked.emit(False)
 
             for row in range(nbTotalRow):
 
-                if int(self.item(row, COLUMNITEMRUNID).text()) in runHidden:
+                if int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text()) in runHidden:
                     self.setRowHidden(row, True)
                 else:
                     self.setRowHidden(row, False)
 
 
 
     @QtCore.pyqtSlot(int)
@@ -505,26 +530,26 @@
 
         # If user wants to see only stared run
         if state==2:
 
             self.signalCheckBoxStaredChecked.emit(True)
 
             for row in range(nbTotalRow):
-                if int(self.item(row, COLUMNITEMRUNID).text()) not in runStared:
+                if int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text()) not in runStared:
                     self.setRowHidden(row, True)
                 else:
                     self.setRowHidden(row, False)
 
         # Show all
         elif state==0:
 
             self.signalCheckBoxStaredChecked.emit(False)
 
             for row in range(nbTotalRow):
-                if int(self.item(row, COLUMNITEMRUNID).text()) in runHidden:
+                if int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text()) in runHidden:
                     self.setRowHidden(row, True)
                 else:
                     self.setRowHidden(row, False)
 
 
 
     @QtCore.pyqtSlot()
@@ -540,27 +565,44 @@
         # We close the plot
         self.dialogComment._allowClosing = True
         self.dialogComment.deleteLater()
         del(self.dialogComment)
 
 
 
+    @QtCore.pyqtSlot(dict)
+    def slotUpdate(self, config: dict) -> None:
+        """
+        Called from DialogMenuDatabaseDisplay when user clicks on a checkbox
+        Show or hide column dependending on the config dictionnary.
+
+        Args:
+            config: dict of the current config file
+        """
+
+        for val in config['DatabaseDisplayColumn'].values():
+
+            # Hide or display some column
+            self.setColumnHidden(val['index'], False==val['visible'])
+
+
+
     @QtCore.pyqtSlot(int, str)
     def slotUpdateCommentDialog(self, runId: int,
                                       comment: str) -> None:
         """
         Called from the dialogComment when user change its text
 
         Args:
             runId: Id of the commented run
             comment: comment to be added to the run
         """
 
         # Add the comment on the GUI
         for row in range(self.rowCount()):
-            if int(self.item(row, COLUMNITEMRUNID).text())==runId:
-                self.setItem(row, COLUMNCOMMENT, QtWidgets.QTableWidgetItem(comment))
+            if int(self.item(row, config['DatabaseDisplayColumn']['itemRunId']['index']).text())==runId:
+                self.setItem(row, config['DatabaseDisplayColumn']['comment']['index'], QtWidgets.QTableWidgetItem(comment))
                 break
 
         # Save the comment in the json file
         self.properties.jsonAddCommentRun(runId,
                                           comment)
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/tableWidgetFolder.py` & `pyplotter-0.3.5/pyplotter/ui/tableWidgetFolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.lastClickTime = time()
         self.lastClickRow  = 100
 
 
 
     def first_call(self):
 
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
         self.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
 
         # If we are unable to detect the config folder, we switch in local mode
         if not os.path.isdir(os.path.normpath(config['path'])):
 
             # Ask user to chose a path
             self.currentPath = QtWidgets.QFileDialog.getExistingDirectory(self,
@@ -164,16 +164,16 @@
                         fileSizeItem = QtWidgets.QTableWidgetItem(sizeof_fmt(os.path.getsize(abs_filename)))
                         fileSizeItem.setTextAlignment(QtCore.Qt.AlignRight)
                         fileSizeItem.setTextAlignment(QtCore.Qt.AlignVCenter)
                         self.setItem(row, 1, fileSizeItem)
                         row += 1
 
         self.setSortingEnabled(True)
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-        self.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
         # Allow item event again
         self._folderUpdating = False
 
 
 
     def itemClicked(self, b: Union[int, QtCore.QPoint]) -> None:
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/tableWidgetParameter.py` & `pyplotter-0.3.5/pyplotter/ui/tableWidgetParameter.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,51 +28,99 @@
     signalRemoveCurve                = QtCore.pyqtSignal(str, str)
     signalCleanSnapshot              = QtCore.pyqtSignal()
     signalAddSnapshot                = QtCore.pyqtSignal(dict)
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
     signalUpdateLabelCurrentSnapshot = QtCore.pyqtSignal(str)
     signalUpdateLabelCurrentRun      = QtCore.pyqtSignal(str)
-    signaladdRow                     = QtCore.pyqtSignal(int, dict, str, str, str, str, str, str, str, int)
+    signaladdRow                     = QtCore.pyqtSignal(int, dict, str, str, str, str, str, str, str, str, int)
 
     signalLoadedDataEmpty  = QtCore.pyqtSignal(QtWidgets.QCheckBox, QtWidgets.QProgressBar)
     signalLoadedDataFull   = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
     signalCSVLoadData      = QtCore.pyqtSignal(str, str, str, str, str, int, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar)
     signalBlueForsLoadData = QtCore.pyqtSignal(str, str, str, str, str, int, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar)
 
 
 
     def __init__(self, parent=None) -> None:
         super(TableWidgetParameter, self).__init__(parent)
 
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
         self.cellClicked.connect(self.parameterCellClicked)
 
         self.threadpool = QtCore.QThreadPool()
 
         # Flag
         self._dataDowloadingFlag = False
 
 
     def first_call(self):
+
+        self._columnIndexes = {'runId' : 0,
+                               'experimentName' : 1,
+                               'parameterName' : 2,
+                               'databaseAbsPath' : 3,
+                               'dataType' : 4,
+                               'plotted' : 5,
+                               'axis' : 6,
+                               'unit' : 7,
+                               'shape' : 8,
+                               'sweptParameters' : 9,
+                               }
+        self.setColumnCount(len(self._columnIndexes))
+
         ## Only used to propagate information
         # runId
-        self.setColumnHidden(0, True)
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('runId')
+        self.setHorizontalHeaderItem(self._columnIndexes['runId'], item)
+        self.setColumnHidden(self._columnIndexes['runId'], True)
         # experimentName
-        self.setColumnHidden(1, True)
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('experimentName')
+        self.setHorizontalHeaderItem(self._columnIndexes['experimentName'], item)
+        self.setColumnHidden(self._columnIndexes['experimentName'], True)
         # parameterName
-        self.setColumnHidden(2, True)
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('parameterName')
+        self.setHorizontalHeaderItem(self._columnIndexes['parameterName'], item)
+        self.setColumnHidden(self._columnIndexes['parameterName'], True)
         # databaseAbsPath
-        self.setColumnHidden(3, True)
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('databaseAbsPath')
+        self.setHorizontalHeaderItem(self._columnIndexes['databaseAbsPath'], item)
+        self.setColumnHidden(self._columnIndexes['databaseAbsPath'], True)
         # dataType
-        self.setColumnHidden(4, True)
-
-        # Should be last column above + 1
-        self.cbColumn = 5
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('dataType')
+        self.setHorizontalHeaderItem(self._columnIndexes['dataType'], item)
+        self.setColumnHidden(self._columnIndexes['dataType'], True)
+
+        ## Column display
+        # plotted
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('plotted')
+        self.setHorizontalHeaderItem(self._columnIndexes['plotted'], item)
+        # axis
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('axis')
+        self.setHorizontalHeaderItem(self._columnIndexes['axis'], item)
+        # unit
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('unit')
+        self.setHorizontalHeaderItem(self._columnIndexes['unit'], item)
+        # shaoe
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('shape')
+        self.setHorizontalHeaderItem(self._columnIndexes['shape'], item)
+        # swept parameters
+        item = QtWidgets.QTableWidgetItem()
+        item.setText('swept parameters')
+        self.setHorizontalHeaderItem(self._columnIndexes['sweptParameters'], item)
 
 
 
     def parameterCellClicked(self, row: int,
                                    column: int) -> None:
         """
         Handle event when user click on the cell containing the checkbox.
@@ -82,16 +130,16 @@
         Parameters
         ----------
             row, column : int, int
             Row and column where the user clicked
         """
 
         # If user clicks on the cell containing the checkbox
-        if column==self.cbColumn:
-            cb = self.cellWidget(row, self.cbColumn)
+        if column==self._columnIndexes['plotted']:
+            cb = self.cellWidget(row, self._columnIndexes['plotted'])
             cb.toggle()
 
 
 
     def parameterClicked(self,
                          state              : bool,
                          cb                 : QtWidgets.QCheckBox,
@@ -123,21 +171,24 @@
         windowTitle : str
             Window title, see getWindowTitle.
         paramDependent : dict
             Dependent parameter the user wants to see the data.
             This should be a qcodes dependent parameter dict.
         plotRef : str
             Reference to a plot window, see getPlotRef.
+        dataType : str
+            either "qcodes", "csv", "bluefors"
         """
 
         if state:
 
             if len(paramDependent['depends_on'])>2:
 
                 self.signalSendStatusBarMessage.emit('Plotter does not handle data whose dim>2', 'red')
+                cb.toggle()
                 return
             else:
                 self.signalAddCurve.emit(curveId,
                                          databaseAbsPath,
                                          dataType,
                                          dependentParamName,
                                          plotRef,
@@ -179,14 +230,16 @@
             Plot title, see getPlotTitle.
         windowTitle : str
             Window title, see getWindowTitle.
         plotRef : str
             Reference of the plot window.
         dependentParamName : str
             Name of the dependent parameter from which data will be downloaded.
+        dataType : str
+            either "qcodes", "csv", "bluefors"
         """
 
         # Flag
         self._dataDowloadingFlag = True
 
         cb.setEnabled(False)
         QtTest.QTest.qWait(100)
@@ -261,28 +314,29 @@
     #                           Called from other widgets
     #
     #
     ############################################################################
 
 
 
-    @QtCore.pyqtSlot(int, list, dict, str, str, str, str, bool)
+    @QtCore.pyqtSlot(int, list, dict, dict, str, str, str, str, bool)
     def slotFillTableWidgetParameter(self, runId: int,
                                            paramDependentList: list,
                                            snapshotDict: dict,
+                                           shapesDict: dict,
                                            experimentName: str,
                                            runName: str,
                                            databaseAbsPath: str,
                                            dataType: str,
                                            doubleClick: bool) -> None:
 
         ## Fill the tableWidgetParameters with the run parameters
         clearTableWidget(self)
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.Fixed)
-        self.verticalHeader().setResizeMode(QtWidgets.QHeaderView.Fixed)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
+        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
 
 
         plotTitle       = getPlotTitle(databaseAbsPath=databaseAbsPath,
                                        runId=runId,
                                        experimentName=experimentName)
         windowTitle     = getWindowTitle(databaseAbsPath=databaseAbsPath,
                                          runId=runId,
@@ -297,27 +351,28 @@
                                         paramDependent=paramDependent,
                                         runId=runId)
 
             rowPosition = self.rowCount()
             self.insertRow(rowPosition)
             self.signaladdRow.emit(runId,
                                    paramDependent,
+                                   str(shapesDict[paramDependent['name']]).replace('[', '').replace(']', ''),
                                    experimentName,
                                    curveId,
                                    plotRef,
                                    plotTitle,
                                    windowTitle,
                                    databaseAbsPath,
                                    dataType,
                                    rowPosition)
 
 
         self.setSortingEnabled(True)
-        self.horizontalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
-        self.verticalHeader().setResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
+        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeToContents)
 
         ## Fill the listWidgetMetada with the station snapshot
         self.signalLineEditSnapshotEnabled.emit(True)
         self.signalLabelSnapshotEnabled.emit(True)
 
         # Update the run snapshot
         self.signalCleanSnapshot.emit()
@@ -327,52 +382,55 @@
 
 
         ## Update label
         self.signalSendStatusBarMessage.emit('Ready', 'green')
 
         # If a double click is detected, we launch a plot of the first parameter
         if doubleClick:
-            self.parameterCellClicked(0, self.cbColumn)
+            self.parameterCellClicked(0, self._columnIndexes['plotted'])
 
 
 
-    @QtCore.pyqtSlot(int, dict, str, str, str, str, str, str, str, int, bool)
+    @QtCore.pyqtSlot(int, dict, str, str, str, str, str, str, str, str, int, bool)
     def slotAddRow(self, runId: int,
                          paramDependent: dict,
+                         shape: str,
                          experimentName: str,
                          curveId: str,
                          plotRef: str,
                          plotTitle: str,
                          windowTitle: str,
                          databaseAbsPath: str,
                          dataType: str,
                          rowPosition: int,
                          isParameterPlotted: bool) -> None:
         """
+        dataType : str
+            either "qcodes", "csv", "bluefors"
         """
 
         runIdStr = str(runId)
 
         cb = QtWidgets.QCheckBox()
 
         if isParameterPlotted:
             cb.setChecked(True)
 
-        self.setItem(rowPosition, 0, QtWidgets.QTableWidgetItem(runIdStr))
-        self.setItem(rowPosition, 1, QtWidgets.QTableWidgetItem(experimentName))
-        self.setItem(rowPosition, 2, QtWidgets.QTableWidgetItem(paramDependent['name']))
-        self.setItem(rowPosition, 3, QtWidgets.QTableWidgetItem(databaseAbsPath))
-        self.setItem(rowPosition, 4, QtWidgets.QTableWidgetItem(dataType))
-        self.setCellWidget(rowPosition, 5, cb)
-        self.setItem(rowPosition, 6, QtWidgets.QTableWidgetItem(paramDependent['label']))
-        self.setItem(rowPosition, 7, QtWidgets.QTableWidgetItem(paramDependent['unit']))
-
+        self.setItem(rowPosition, self._columnIndexes['runId'], QtWidgets.QTableWidgetItem(runIdStr))
+        self.setItem(rowPosition, self._columnIndexes['experimentName'], QtWidgets.QTableWidgetItem(experimentName))
+        self.setItem(rowPosition, self._columnIndexes['parameterName'], QtWidgets.QTableWidgetItem(paramDependent['name']))
+        self.setItem(rowPosition, self._columnIndexes['databaseAbsPath'], QtWidgets.QTableWidgetItem(databaseAbsPath))
+        self.setItem(rowPosition, self._columnIndexes['dataType'], QtWidgets.QTableWidgetItem(dataType))
+        self.setCellWidget(rowPosition, self._columnIndexes['plotted'], cb)
+        self.setItem(rowPosition, self._columnIndexes['axis'], QtWidgets.QTableWidgetItem(paramDependent['label']))
+        self.setItem(rowPosition, self._columnIndexes['unit'], QtWidgets.QTableWidgetItem(paramDependent['unit']))
+        self.setItem(rowPosition, self._columnIndexes['shape'], QtWidgets.QTableWidgetItem(shape))
 
         independentString = config['sweptParameterSeparator'].join(paramDependent['depends_on'])
-        self.setCellWidget(rowPosition, 8, QtWidgets.QLabel(independentString))
+        self.setCellWidget(rowPosition, self._columnIndexes['sweptParameters'], QtWidgets.QLabel(independentString))
 
         # Each checkbox at its own event attached to it
         cb.toggled.connect(lambda state,
                                   cb                    = cb,
                                   dependentParamName    = paramDependent['name'],
                                   runId                 = runId,
                                   curveId               = curveId,
@@ -411,17 +469,17 @@
 
             rowCurveId = getCurveId(databaseAbsPath=databaseAbsPath,
                                     name=parameterName,
                                     runId=runId)
 
             if rowCurveId==curveId:
                 # Uncheck the checkBox without triggering an event
-                self.cellWidget(row, self.cbColumn).setCheckable(False)
-                self.cellWidget(row, self.cbColumn).setChecked(False)
-                self.cellWidget(row, self.cbColumn).setCheckable(True)
+                self.cellWidget(row, self._columnIndexes['plotted']).setCheckable(False)
+                self.cellWidget(row, self._columnIndexes['plotted']).setChecked(False)
+                self.cellWidget(row, self._columnIndexes['plotted']).setCheckable(True)
 
 
 
     @QtCore.pyqtSlot()
     def slotClearTable(self) -> None:
 
         clearTableWidget(self)
```

### Comparing `pyplotter-0.3.4/pyplotter/ui/treeViewSnapshot.py` & `pyplotter-0.3.5/pyplotter/ui/treeViewSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/widgetPlot1d.py` & `pyplotter-0.3.5/pyplotter/ui/widgetPlot1d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter/ui/widgetPlot2d.py` & `pyplotter-0.3.5/pyplotter/ui/widgetPlot2d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.4/pyplotter.egg-info/PKG-INFO` & `pyplotter-0.3.5/pyplotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pyplotter
-Version: 0.3.4
+Version: 0.3.5
 Summary: A data browser and vizualizer for QCoDes database, csv, s2p and BlueFors logging files.
 Home-page: https://github.com/pyplotter/pyplotter
-Author: Étienne Dumur
 Author-email: etienne.dumur@cea.fr
 Maintainer: Étienne Dumur
 Maintainer-email: etienne.dumur@cea.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -206,9 +204,7 @@
 
 ## 🙏 Acknowledgments
 
 * [plottr](https://github.com/toolsforexperiments/plottr), for the inspiration of some interfaces.
 * [pyqtgraph](http://www.pyqtgraph.org/), for the amazing and **fast** plotting library.
 * [bokeh](https://github.com/bokeh/bokeh/blob/7cc500601cdb688c4b6b2153704097f3345dd91c/bokeh/palettes.py), for their work on the colormap palette reused here.
 * [qb style](https://github.com/quantumblacklabs/qbstyles), for its color codes of lines.
-
-
```

### Comparing `pyplotter-0.3.4/pyplotter.egg-info/SOURCES.txt` & `pyplotter-0.3.5/pyplotter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 pyplotter/__init__.py
 pyplotter/pyplotter.py
 pyplotter.egg-info/PKG-INFO
 pyplotter.egg-info/SOURCES.txt
 pyplotter.egg-info/dependency_links.txt
@@ -57,14 +58,16 @@
 pyplotter/ui/dialogs/dialogColormap.py
 pyplotter/ui/dialogs/dialogColormapUi.py
 pyplotter/ui/dialogs/dialogComment.py
 pyplotter/ui/dialogs/dialogFontsize.py
 pyplotter/ui/dialogs/dialogFontsizeUi.py
 pyplotter/ui/dialogs/dialogLiveplot.py
 pyplotter/ui/dialogs/dialogLiveplotUi.py
+pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py
+pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py
 pyplotter/ui/pictures/bluefors.png
 pyplotter/ui/pictures/csv.png
 pyplotter/ui/pictures/database.png
 pyplotter/ui/pictures/databaseOpened.png
 pyplotter/ui/pictures/databaseOpenedStared.png
 pyplotter/ui/pictures/databaseStared.png
 pyplotter/ui/pictures/empty.png
```

### Comparing `pyplotter-0.3.4/setup.cfg` & `pyplotter-0.3.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7970 6c6f 7474 6572 0d0a 7665   = pyplotter..ve
-00000020: 7273 696f 6e20 3d20 302e 332e 340d 0a61  rsion = 0.3.4..a
-00000030: 7574 686f 7220 3d20 c389 7469 656e 6e65  uthor = ..tienne
-00000040: 2044 756d 7572 0d0a 6175 7468 6f72 5f65   Dumur..author_e
-00000050: 6d61 696c 203d 2065 7469 656e 6e65 2e64  mail = etienne.d
-00000060: 756d 7572 4063 6561 2e66 720d 0a6d 6169  umur@cea.fr..mai
-00000070: 6e74 6169 6e65 7220 3d20 c389 7469 656e  ntainer = ..tien
-00000080: 6e65 2044 756d 7572 0d0a 6d61 696e 7461  ne Dumur..mainta
-00000090: 696e 6572 5f65 6d61 696c 203d 2065 7469  iner_email = eti
-000000a0: 656e 6e65 2e64 756d 7572 4063 6561 2e66  enne.dumur@cea.f
-000000b0: 720d 0a64 6573 6372 6970 7469 6f6e 203d  r..description =
-000000c0: 2041 2064 6174 6120 6272 6f77 7365 7220   A data browser 
-000000d0: 616e 6420 7669 7a75 616c 697a 6572 2066  and vizualizer f
-000000e0: 6f72 2051 436f 4465 7320 6461 7461 6261  or QCoDes databa
-000000f0: 7365 2c20 6373 762c 2073 3270 2061 6e64  se, csv, s2p and
-00000100: 2042 6c75 6546 6f72 7320 6c6f 6767 696e   BlueFors loggin
-00000110: 6720 6669 6c65 732e 0d0a 6c6f 6e67 5f64  g files...long_d
-00000120: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000130: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-00000140: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000150: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000160: 7874 2f6d 6172 6b64 6f77 6e3b 2063 6861  xt/markdown; cha
-00000170: 7273 6574 3d55 5446 2d38 3b20 7661 7269  rset=UTF-8; vari
-00000180: 616e 743d 4746 4d0d 0a75 726c 203d 2068  ant=GFM..url = h
-00000190: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001a0: 6d2f 7079 706c 6f74 7465 722f 7079 706c  m/pyplotter/pypl
-000001b0: 6f74 7465 720d 0a63 6c61 7373 6966 6965  otter..classifie
-000001c0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-000001d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001e0: 5079 7468 6f6e 203a 3a20 330d 0a09 496e  Python :: 3...In
-000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000200: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-00000210: 7263 680d 0a09 4f70 6572 6174 696e 6720  rch...Operating 
-00000220: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000230: 6570 656e 6465 6e74 0d0a 0954 6f70 6963  ependent...Topic
-00000240: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-00000250: 6e67 696e 6565 7269 6e67 0d0a 6c69 6365  ngineering..lice
-00000260: 6e73 6520 3d20 4d49 540d 0a70 6163 6b61  nse = MIT..packa
-00000270: 6765 7320 3d20 6669 6e64 5f70 6163 6b61  ges = find_packa
-00000280: 6765 7328 292c 0d0a 0d0a 5b6f 7074 696f  ges(),....[optio
-00000290: 6e73 5d0d 0a70 7974 686f 6e5f 7265 7175  ns]..python_requ
-000002a0: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
-000002b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000002c0: 7461 203d 2054 7275 650d 0a69 6e73 7461  ta = True..insta
-000002d0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-000002e0: 0971 6461 726b 7374 796c 650d 0a09 6c6d  .qdarkstyle...lm
-000002f0: 6669 740d 0a09 6d75 6c74 6970 726f 6365  fit...multiproce
-00000300: 7373 0d0a 096e 756d 7079 3e3d 312e 3137  ss...numpy>=1.17
-00000310: 2e30 0d0a 0970 616e 6461 733e 3d31 2e30  .0...pandas>=1.0
-00000320: 2e30 0d0a 0970 6c61 7466 6f72 6d64 6972  .0...platformdir
-00000330: 730d 0a09 7079 6f70 656e 676c 0d0a 0970  s...pyopengl...p
-00000340: 7971 7435 0d0a 0970 7971 7435 2d73 6970  yqt5...pyqt5-sip
-00000350: 0d0a 0970 7971 7477 6562 656e 6769 6e65  ...pyqtwebengine
-00000360: 0d0a 0970 7971 7467 7261 7068 3e3d 302e  ...pyqtgraph>=0.
-00000370: 3132 2e33 0d0a 0971 636f 6465 733e 3d30  12.3...qcodes>=0
-00000380: 2e32 362e 300d 0a09 7363 696b 6974 2d72  .26.0...scikit-r
-00000390: 660d 0a09 7363 6970 790d 0a0d 0a5b 6f70  f...scipy....[op
-000003a0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000003b0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-000003c0: 6970 7473 203d 200d 0a09 706c 6f74 7465  ipts = ...plotte
-000003d0: 7220 3d20 7079 706c 6f74 7465 722e 7079  r = pyplotter.py
-000003e0: 706c 6f74 7465 723a 6d61 696e 0d0a 0970  plotter:main...p
-000003f0: 7970 6c6f 7474 6572 203d 2070 7970 6c6f  yplotter = pyplo
-00000400: 7474 6572 2e70 7970 6c6f 7474 6572 3a6d  tter.pyplotter:m
-00000410: 6169 6e0d 0a0d 0a5b 6567 675f 696e 666f  ain....[egg_info
-00000420: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000430: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000440: 0a                                       .
+00000020: 7273 696f 6e20 3d20 302e 332e 350d 0a61  rsion = 0.3.5..a
+00000030: 7574 686f 725f 656d 6169 6c20 3d20 6574  uthor_email = et
+00000040: 6965 6e6e 652e 6475 6d75 7240 6365 612e  ienne.dumur@cea.
+00000050: 6672 0d0a 6d61 696e 7461 696e 6572 203d  fr..maintainer =
+00000060: 20c3 8974 6965 6e6e 6520 4475 6d75 720d   ..tienne Dumur.
+00000070: 0a6d 6169 6e74 6169 6e65 725f 656d 6169  .maintainer_emai
+00000080: 6c20 3d20 6574 6965 6e6e 652e 6475 6d75  l = etienne.dumu
+00000090: 7240 6365 612e 6672 0d0a 6465 7363 7269  r@cea.fr..descri
+000000a0: 7074 696f 6e20 3d20 4120 6461 7461 2062  ption = A data b
+000000b0: 726f 7773 6572 2061 6e64 2076 697a 7561  rowser and vizua
+000000c0: 6c69 7a65 7220 666f 7220 5143 6f44 6573  lizer for QCoDes
+000000d0: 2064 6174 6162 6173 652c 2063 7376 2c20   database, csv, 
+000000e0: 7332 7020 616e 6420 426c 7565 466f 7273  s2p and BlueFors
+000000f0: 206c 6f67 6769 6e67 2066 696c 6573 2e0d   logging files..
+00000100: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000110: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+00000120: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+00000130: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000140: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000150: 776e 3b20 6368 6172 7365 743d 5554 462d  wn; charset=UTF-
+00000160: 383b 2076 6172 6961 6e74 3d47 464d 0d0a  8; variant=GFM..
+00000170: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000180: 7468 7562 2e63 6f6d 2f70 7970 6c6f 7474  thub.com/pyplott
+00000190: 6572 2f70 7970 6c6f 7474 6572 0d0a 636c  er/pyplotter..cl
+000001a0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+000001b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001d0: 2033 0d0a 0949 6e74 656e 6465 6420 4175   3...Intended Au
+000001e0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+000001f0: 652f 5265 7365 6172 6368 0d0a 094f 7065  e/Research...Ope
+00000200: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000210: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000220: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
+00000230: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000240: 670d 0a6c 6963 656e 7365 203d 204d 4954  g..license = MIT
+00000250: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000260: 645f 7061 636b 6167 6573 2829 2c0d 0a0d  d_packages(),...
+00000270: 0a5b 6f70 7469 6f6e 735d 0d0a 7079 7468  .[options]..pyth
+00000280: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000290: 332e 360d 0a69 6e63 6c75 6465 5f70 6163  3.6..include_pac
+000002a0: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
+000002b0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000002c0: 6573 203d 200d 0a09 7164 6172 6b73 7479  es = ...qdarksty
+000002d0: 6c65 0d0a 096c 6d66 6974 0d0a 096d 756c  le...lmfit...mul
+000002e0: 7469 7072 6f63 6573 730d 0a09 6e75 6d70  tiprocess...nump
+000002f0: 793e 3d31 2e31 372e 300d 0a09 7061 6e64  y>=1.17.0...pand
+00000300: 6173 3e3d 312e 302e 300d 0a09 706c 6174  as>=1.0.0...plat
+00000310: 666f 726d 6469 7273 0d0a 0970 796f 7065  formdirs...pyope
+00000320: 6e67 6c0d 0a09 7079 7174 350d 0a09 7079  ngl...pyqt5...py
+00000330: 7174 352d 7369 700d 0a09 7079 7174 7765  qt5-sip...pyqtwe
+00000340: 6265 6e67 696e 650d 0a09 7079 7174 6772  bengine...pyqtgr
+00000350: 6170 683e 3d30 2e31 322e 330d 0a09 7163  aph>=0.12.3...qc
+00000360: 6f64 6573 3e3d 302e 3236 2e30 0d0a 0973  odes>=0.26.0...s
+00000370: 6369 6b69 742d 7266 0d0a 0973 6369 7079  cikit-rf...scipy
+00000380: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+00000390: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
+000003a0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
+000003b0: 0970 6c6f 7474 6572 203d 2070 7970 6c6f  .plotter = pyplo
+000003c0: 7474 6572 2e70 7970 6c6f 7474 6572 3a6d  tter.pyplotter:m
+000003d0: 6169 6e0d 0a09 7079 706c 6f74 7465 7220  ain...pyplotter 
+000003e0: 3d20 7079 706c 6f74 7465 722e 7079 706c  = pyplotter.pypl
+000003f0: 6f74 7465 723a 6d61 696e 0d0a 0d0a 5b65  otter:main....[e
+00000400: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000410: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000420: 203d 2030 0d0a 0d0a                       = 0....
```

