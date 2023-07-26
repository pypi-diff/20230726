# Comparing `tmp/pyplotter-0.3.5.tar.gz` & `tmp/pyplotter-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotter-0.3.5.tar", last modified: Thu Jun  1 11:56:06 2023, max compression
+gzip compressed data, was "pyplotter-0.3.6.tar", last modified: Wed Jul 26 13:10:14 2023, max compression
```

## Comparing `pyplotter-0.3.5.tar` & `pyplotter-0.3.6.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.969824 pyplotter-0.3.5/
--rw-rw-rw-   0        0        0     1182 2022-04-06 10:43:16.000000 pyplotter-0.3.5/LICENSE
--rw-rw-rw-   0        0        0       35 2022-05-10 10:10:11.000000 pyplotter-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7710 2023-06-01 11:56:06.970824 pyplotter-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     7076 2022-09-07 08:19:20.000000 pyplotter-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.591823 pyplotter-0.3.5/pyplotter/
--rw-rw-rw-   0        0        0        0 2022-05-10 10:10:11.000000 pyplotter-0.3.5/pyplotter/__init__.py
--rw-rw-rw-   0        0        0      836 2022-08-01 13:37:57.000000 pyplotter-0.3.5/pyplotter/pyplotter.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.662822 pyplotter-0.3.5/pyplotter/sources/
--rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/sources/__init__.py
--rw-rw-rw-   0        0        0    17575 2023-03-29 14:12:42.000000 pyplotter-0.3.5/pyplotter/sources/config.py
--rw-rw-rw-   0        0        0    16825 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/functions.py
--rw-rw-rw-   0        0        0    32935 2023-04-18 10:08:58.000000 pyplotter-0.3.5/pyplotter/sources/main.py
--rw-rw-rw-   0        0        0    95768 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/sources/palettes.py
--rw-rw-rw-   0        0        0     8496 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/pyqtgraph.py
--rw-rw-rw-   0        0        0    29407 2023-04-18 10:04:38.000000 pyplotter-0.3.5/pyplotter/sources/qcodesDatabase.py
--rw-rw-rw-   0        0        0    10681 2023-03-14 10:33:09.000000 pyplotter-0.3.5/pyplotter/sources/runPropertiesExtra.py
--rw-rw-rw-   0        0        0     8475 2023-04-18 11:41:03.000000 pyplotter-0.3.5/pyplotter/sources/widgetBlueFors.py
--rw-rw-rw-   0        0        0    10751 2023-04-18 11:39:49.000000 pyplotter-0.3.5/pyplotter/sources/widgetCSV.py
--rw-rw-rw-   0        0        0    16164 2023-03-17 13:40:51.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot.py
--rw-rw-rw-   0        0        0    70638 2023-02-17 09:02:20.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot1d.py
--rw-rw-rw-   0        0        0    69186 2023-04-18 08:41:49.000000 pyplotter-0.3.5/pyplotter/sources/widgetPlot2d.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.681823 pyplotter-0.3.5/pyplotter/sources/workers/
--rw-rw-rw-   0        0        0        0 2022-03-01 13:15:08.000000 pyplotter-0.3.5/pyplotter/sources/workers/__init__.py
--rw-rw-rw-   0        0        0     3025 2023-01-04 16:03:39.000000 pyplotter-0.3.5/pyplotter/sources/workers/checkNbRunDatabase.py
--rw-rw-rw-   0        0        0     7870 2023-03-29 14:10:57.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataBase.py
--rw-rw-rw-   0        0        0     4315 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromCache.py
--rw-rw-rw-   0        0        0     9334 2023-01-04 16:03:29.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromRun.py
--rw-rw-rw-   0        0        0     2290 2023-04-18 10:06:03.000000 pyplotter-0.3.5/pyplotter/sources/workers/loadRunInfo.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.768826 pyplotter-0.3.5/pyplotter/ui/
--rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/__init__.py
--rw-rw-rw-   0        0        0     1784 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/checkBoxHidden.py
--rw-rw-rw-   0        0        0     1578 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/checkBoxStared.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.814826 pyplotter-0.3.5/pyplotter/ui/dialogs/
--rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-03-17 13:40:19.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormap.py
--rw-rw-rw-   0        0        0     3668 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormapUi.py
--rw-rw-rw-   0        0        0     1816 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogComment.py
--rw-rw-rw-   0        0        0      988 2023-03-17 13:40:13.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsize.py
--rw-rw-rw-   0        0        0     4192 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsizeUi.py
--rw-rw-rw-   0        0        0    23043 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplot.py
--rw-rw-rw-   0        0        0    20446 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplotUi.py
--rw-rw-rw-   0        0        0     4067 2023-03-29 14:05:07.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py
--rw-rw-rw-   0        0        0     2859 2023-03-29 13:20:18.000000 pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py
--rw-rw-rw-   0        0        0     1785 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/hBoxLayoutLabelPath.py
--rw-rw-rw-   0        0        0      388 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/histogramLUTWidget.py
--rw-rw-rw-   0        0        0      531 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/labelSnapshot.py
--rw-rw-rw-   0        0        0     1284 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/lineEditSnapshot.py
--rw-rw-rw-   0        0        0    16326 2023-04-18 10:27:14.000000 pyplotter-0.3.5/pyplotter/ui/mainWindow.py
--rw-rw-rw-   0        0        0     9055 2023-03-29 13:43:20.000000 pyplotter-0.3.5/pyplotter/ui/menuBar.py
--rw-rw-rw-   0        0        0     1772 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/menuDb.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.889824 pyplotter-0.3.5/pyplotter/ui/pictures/
--rw-rw-rw-   0        0        0     1895 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/pictures/bluefors.png
--rw-rw-rw-   0        0        0     2992 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/csv.png
--rw-rw-rw-   0        0        0     2791 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/database.png
--rw-rw-rw-   0        0        0     1998 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpened.png
--rw-rw-rw-   0        0        0     3294 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpenedStared.png
--rw-rw-rw-   0        0        0     4684 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/databaseStared.png
--rw-rw-rw-   0        0        0      170 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/empty.png
--rw-rw-rw-   0        0        0     1788 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/folder.png
--rw-rw-rw-   0        0        0     1384 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/folderEnhanced.png
--rw-rw-rw-   0        0        0   192524 2022-01-17 07:35:16.000000 pyplotter-0.3.5/pyplotter/ui/pictures/icon.png
--rw-rw-rw-   0        0        0     1346 2022-01-17 07:35:16.000000 pyplotter-0.3.5/pyplotter/ui/pictures/icon.py
--rw-rw-rw-   0        0        0     2915 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/s2p.png
--rw-rw-rw-   0        0        0     1723 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/star.png
--rw-rw-rw-   0        0        0     1173 2020-11-30 15:51:41.000000 pyplotter-0.3.5/pyplotter/ui/pictures/trash.png
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.965824 pyplotter-0.3.5/pyplotter/ui/plot1d/
--rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/__init__.py
--rw-rw-rw-   0        0        0     5098 2022-09-13 06:53:17.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFiltering.py
--rw-rw-rw-   0        0        0    35713 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFit.py
--rw-rw-rw-   0        0        0     8502 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculus.py
--rw-rw-rw-   0        0        0     2241 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculusUi.py
--rw-rw-rw-   0        0        0    10977 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFT.py
--rw-rw-rw-   0        0        0     2625 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFTUi.py
--rw-rw-rw-   0        0        0     7117 2022-09-13 06:51:57.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFiltering.py
--rw-rw-rw-   0        0        0     7132 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFit.py
--rw-rw-rw-   0        0        0     8152 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalize.py
--rw-rw-rw-   0        0        0     2448 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalizeUi.py
--rw-rw-rw-   0        0        0     6588 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatistics.py
--rw-rw-rw-   0        0        0     3663 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatisticsUi.py
--rw-rw-rw-   0        0        0     8111 2023-02-17 09:02:20.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurve.py
--rw-rw-rw-   0        0        0     3423 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurveUi.py
--rw-rw-rw-   0        0        0      244 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/plot1dWidget.py
--rw-rw-rw-   0        0        0      356 2023-04-17 13:19:05.000000 pyplotter-0.3.5/pyplotter/ui/plotWidget.py
--rw-rw-rw-   0        0        0     1334 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/pushButtonOpenFolder.py
--rw-rw-rw-   0        0        0     6914 2023-04-24 13:35:52.000000 pyplotter-0.3.5/pyplotter/ui/statusBar.py
--rw-rw-rw-   0        0        0    25592 2023-04-18 10:23:07.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetDatabase.py
--rw-rw-rw-   0        0        0    13729 2023-03-09 16:16:50.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetFolder.py
--rw-rw-rw-   0        0        0      495 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetItemNumOrdered.py
--rw-rw-rw-   0        0        0    21386 2023-04-18 11:41:13.000000 pyplotter-0.3.5/pyplotter/ui/tableWidgetParameter.py
--rw-rw-rw-   0        0        0     3940 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/treeViewSnapshot.py
--rw-rw-rw-   0        0        0    15046 2022-09-07 08:19:21.000000 pyplotter-0.3.5/pyplotter/ui/widgetPlot1d.py
--rw-rw-rw-   0        0        0    26264 2023-04-18 08:42:34.000000 pyplotter-0.3.5/pyplotter/ui/widgetPlot2d.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:56:06.614822 pyplotter-0.3.5/pyplotter.egg-info/
--rw-rw-rw-   0        0        0     7710 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 11:56:06.000000 pyplotter-0.3.5/pyplotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-06-01 11:56:02.000000 pyplotter-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0     1064 2023-06-01 11:56:06.973824 pyplotter-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      128 2022-05-10 10:10:11.000000 pyplotter-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.329777 pyplotter-0.3.6/
+-rw-rw-rw-   0        0        0     1182 2022-04-06 10:43:16.000000 pyplotter-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-05-10 10:10:11.000000 pyplotter-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7734 2023-07-26 13:10:14.329777 pyplotter-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7076 2022-09-07 08:19:20.000000 pyplotter-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.139801 pyplotter-0.3.6/pyplotter/
+-rw-rw-rw-   0        0        0        0 2022-05-10 10:10:11.000000 pyplotter-0.3.6/pyplotter/__init__.py
+-rw-rw-rw-   0        0        0      836 2022-08-01 13:37:57.000000 pyplotter-0.3.6/pyplotter/pyplotter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.193445 pyplotter-0.3.6/pyplotter/sources/
+-rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/sources/__init__.py
+-rw-rw-rw-   0        0        0    17647 2023-07-25 15:09:26.000000 pyplotter-0.3.6/pyplotter/sources/config.py
+-rw-rw-rw-   0        0        0    16825 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/sources/functions.py
+-rw-rw-rw-   0        0        0    33263 2023-06-07 11:58:57.000000 pyplotter-0.3.6/pyplotter/sources/main.py
+-rw-rw-rw-   0        0        0    95768 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/sources/palettes.py
+-rw-rw-rw-   0        0        0     8496 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/sources/pyqtgraph.py
+-rw-rw-rw-   0        0        0    29407 2023-04-18 10:04:38.000000 pyplotter-0.3.6/pyplotter/sources/qcodesDatabase.py
+-rw-rw-rw-   0        0        0    10685 2023-06-07 11:54:39.000000 pyplotter-0.3.6/pyplotter/sources/runPropertiesExtra.py
+-rw-rw-rw-   0        0        0     8826 2023-07-26 12:32:10.000000 pyplotter-0.3.6/pyplotter/sources/widgetBlueFors.py
+-rw-rw-rw-   0        0        0    10754 2023-07-25 15:12:57.000000 pyplotter-0.3.6/pyplotter/sources/widgetCSV.py
+-rw-rw-rw-   0        0        0    16164 2023-03-17 13:40:51.000000 pyplotter-0.3.6/pyplotter/sources/widgetPlot.py
+-rw-rw-rw-   0        0        0    70638 2023-02-17 09:02:20.000000 pyplotter-0.3.6/pyplotter/sources/widgetPlot1d.py
+-rw-rw-rw-   0        0        0    69186 2023-04-18 08:41:49.000000 pyplotter-0.3.6/pyplotter/sources/widgetPlot2d.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.206596 pyplotter-0.3.6/pyplotter/sources/workers/
+-rw-rw-rw-   0        0        0        0 2022-03-01 13:15:08.000000 pyplotter-0.3.6/pyplotter/sources/workers/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-07 10:22:01.000000 pyplotter-0.3.6/pyplotter/sources/workers/checkNbRunDatabase.py
+-rw-rw-rw-   0        0        0     8219 2023-07-25 15:07:54.000000 pyplotter-0.3.6/pyplotter/sources/workers/loadDataBase.py
+-rw-rw-rw-   0        0        0     4315 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/sources/workers/loadDataFromCache.py
+-rw-rw-rw-   0        0        0     9371 2023-07-25 15:07:23.000000 pyplotter-0.3.6/pyplotter/sources/workers/loadDataFromRun.py
+-rw-rw-rw-   0        0        0     2290 2023-04-18 10:06:03.000000 pyplotter-0.3.6/pyplotter/sources/workers/loadRunInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.246599 pyplotter-0.3.6/pyplotter/ui/
+-rw-rw-rw-   0        0        0        0 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-06-07 11:45:47.000000 pyplotter-0.3.6/pyplotter/ui/checkBoxHidden.py
+-rw-rw-rw-   0        0        0     1603 2023-06-07 11:45:55.000000 pyplotter-0.3.6/pyplotter/ui/checkBoxStared.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.277429 pyplotter-0.3.6/pyplotter/ui/dialogs/
+-rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-03-17 13:40:19.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogColormap.py
+-rw-rw-rw-   0        0        0     3668 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogColormapUi.py
+-rw-rw-rw-   0        0        0     1816 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogComment.py
+-rw-rw-rw-   0        0        0      988 2023-03-17 13:40:13.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogFontsize.py
+-rw-rw-rw-   0        0        0     4192 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogFontsizeUi.py
+-rw-rw-rw-   0        0        0    23046 2023-06-07 09:52:39.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogLiveplot.py
+-rw-rw-rw-   0        0        0    20446 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogLiveplotUi.py
+-rw-rw-rw-   0        0        0     4067 2023-03-29 14:05:07.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py
+-rw-rw-rw-   0        0        0     2859 2023-03-29 13:20:18.000000 pyplotter-0.3.6/pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py
+-rw-rw-rw-   0        0        0     1785 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/hBoxLayoutLabelPath.py
+-rw-rw-rw-   0        0        0      388 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/histogramLUTWidget.py
+-rw-rw-rw-   0        0        0      531 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/labelSnapshot.py
+-rw-rw-rw-   0        0        0     1284 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/lineEditSnapshot.py
+-rw-rw-rw-   0        0        0    16326 2023-04-18 10:27:14.000000 pyplotter-0.3.6/pyplotter/ui/mainWindow.py
+-rw-rw-rw-   0        0        0     9055 2023-03-29 13:43:20.000000 pyplotter-0.3.6/pyplotter/ui/menuBar.py
+-rw-rw-rw-   0        0        0     1772 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/menuDb.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.299776 pyplotter-0.3.6/pyplotter/ui/pictures/
+-rw-rw-rw-   0        0        0     1895 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/pictures/bluefors.png
+-rw-rw-rw-   0        0        0     2992 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/csv.png
+-rw-rw-rw-   0        0        0     2791 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/database.png
+-rw-rw-rw-   0        0        0     1998 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/databaseOpened.png
+-rw-rw-rw-   0        0        0     3294 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/databaseOpenedStared.png
+-rw-rw-rw-   0        0        0     4684 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/databaseStared.png
+-rw-rw-rw-   0        0        0      170 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/empty.png
+-rw-rw-rw-   0        0        0     1788 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/folder.png
+-rw-rw-rw-   0        0        0     1384 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/folderEnhanced.png
+-rw-rw-rw-   0        0        0    51769 2023-07-20 08:46:54.000000 pyplotter-0.3.6/pyplotter/ui/pictures/icon.png
+-rw-rw-rw-   0        0        0     1346 2022-01-17 07:35:16.000000 pyplotter-0.3.6/pyplotter/ui/pictures/icon.py
+-rw-rw-rw-   0        0        0     2915 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/s2p.png
+-rw-rw-rw-   0        0        0     1723 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/star.png
+-rw-rw-rw-   0        0        0     1173 2020-11-30 15:51:41.000000 pyplotter-0.3.6/pyplotter/ui/pictures/trash.png
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.329777 pyplotter-0.3.6/pyplotter/ui/plot1d/
+-rw-rw-rw-   0        0        0        0 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/__init__.py
+-rw-rw-rw-   0        0        0     5098 2022-09-13 06:53:17.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/dialogFiltering.py
+-rw-rw-rw-   0        0        0    35713 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/dialogFit.py
+-rw-rw-rw-   0        0        0     8502 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxCalculus.py
+-rw-rw-rw-   0        0        0     2241 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxCalculusUi.py
+-rw-rw-rw-   0        0        0    10977 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFFT.py
+-rw-rw-rw-   0        0        0     2625 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFFTUi.py
+-rw-rw-rw-   0        0        0     7117 2022-09-13 06:51:57.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFiltering.py
+-rw-rw-rw-   0        0        0     7132 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFit.py
+-rw-rw-rw-   0        0        0     8152 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxNormalize.py
+-rw-rw-rw-   0        0        0     2448 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxNormalizeUi.py
+-rw-rw-rw-   0        0        0     6588 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxStatistics.py
+-rw-rw-rw-   0        0        0     3663 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxStatisticsUi.py
+-rw-rw-rw-   0        0        0     8111 2023-02-17 09:02:20.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/widgetTabCurve.py
+-rw-rw-rw-   0        0        0     3423 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1d/widgetTabCurveUi.py
+-rw-rw-rw-   0        0        0      244 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/plot1dWidget.py
+-rw-rw-rw-   0        0        0      356 2023-04-17 13:19:05.000000 pyplotter-0.3.6/pyplotter/ui/plotWidget.py
+-rw-rw-rw-   0        0        0     1334 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/pushButtonOpenFolder.py
+-rw-rw-rw-   0        0        0     7245 2023-07-25 15:10:49.000000 pyplotter-0.3.6/pyplotter/ui/statusBar.py
+-rw-rw-rw-   0        0        0    26311 2023-07-25 15:08:15.000000 pyplotter-0.3.6/pyplotter/ui/tableWidgetDatabase.py
+-rw-rw-rw-   0        0        0    15511 2023-06-07 12:05:29.000000 pyplotter-0.3.6/pyplotter/ui/tableWidgetFolder.py
+-rw-rw-rw-   0        0        0      495 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/tableWidgetItemNumOrdered.py
+-rw-rw-rw-   0        0        0    21391 2023-07-25 15:08:23.000000 pyplotter-0.3.6/pyplotter/ui/tableWidgetParameter.py
+-rw-rw-rw-   0        0        0     3940 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/treeViewSnapshot.py
+-rw-rw-rw-   0        0        0    15046 2022-09-07 08:19:21.000000 pyplotter-0.3.6/pyplotter/ui/widgetPlot1d.py
+-rw-rw-rw-   0        0        0    26264 2023-04-18 08:42:34.000000 pyplotter-0.3.6/pyplotter/ui/widgetPlot2d.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:10:14.161445 pyplotter-0.3.6/pyplotter.egg-info/
+-rw-rw-rw-   0        0        0     7734 2023-07-26 13:10:13.000000 pyplotter-0.3.6/pyplotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3202 2023-07-26 13:10:14.000000 pyplotter-0.3.6/pyplotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:10:13.000000 pyplotter-0.3.6/pyplotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-07-26 13:10:13.000000 pyplotter-0.3.6/pyplotter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2023-07-26 13:10:13.000000 pyplotter-0.3.6/pyplotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 13:10:13.000000 pyplotter-0.3.6/pyplotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-07-25 15:17:08.000000 pyplotter-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1089 2023-07-26 13:10:14.329777 pyplotter-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      128 2022-05-10 10:10:11.000000 pyplotter-0.3.6/setup.py
```

### Comparing `pyplotter-0.3.5/LICENSE` & `pyplotter-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/PKG-INFO` & `pyplotter-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyplotter
-Version: 0.3.5
+Version: 0.3.6
 Summary: A data browser and vizualizer for QCoDes database, csv, s2p and BlueFors logging files.
 Home-page: https://github.com/pyplotter/pyplotter
+Author: Étienne Dumur
 Author-email: etienne.dumur@cea.fr
 Maintainer: Étienne Dumur
 Maintainer-email: etienne.dumur@cea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `pyplotter-0.3.5/README.md` & `pyplotter-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/pyplotter.py` & `pyplotter-0.3.6/pyplotter/pyplotter.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/config.py` & `pyplotter-0.3.6/pyplotter/sources/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 'displayRunNameInPlotTitle' : True,
 
 # Maximum number of runs being treated on the same SQL request
 # Should be somwhere below 2020
 'maximumRunPerRequest' : 2000, # int
 # Gives the downloading file percentage must progressed to be displayed
 'displayedDownloadQcodesPercentage' : 5, # int
+# Number of decimal for the progress bar
+'progressBarDecimal' : 100, # int
 # The delay in ms between to check of a run download
 'delayBetweenProgressBarUpdate' : 100, # int
 # Number of runs to be transferred at the same time when displaying a database
 'NbRunEmit' : 100, # int
 # Delay between to consecutive check of the total nb of run in a database
 'delayBetweendataBaseNbRunCheck' : 5, # in s
 # Message to display when station has not been defined in a qcodes experiment
@@ -120,15 +122,15 @@
                'ch5' : {'labelText'  : 'Mixture tank',
                         'labelUnits' : 'Bar'},
                'ch6' : {'labelText'  : 'Venting line',
                         'labelUnits' : 'Bar'}},
 
 
 # Layout parameters
-'dialogWindowSize' : (1.618*750, 500),
+'dialogWindowSize' : (1314, 500),
 'sweptParameterSeparator' : " <span style='font-weight: bold; color: #eb272e;'>vs</span> ",
 
 'style' : 'qbstyles', # Must match an available style below
 'styles' : {'qdarkstyle' : {'dialogBackgroundColor'    : '#272822',
                             'pyqtgraphBackgroundColor' : '#272822',
                             'dialogTextColor'          : '#ffffff',
                             'plot1dSelectionLineColor' : '#ffffff',
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/functions.py` & `pyplotter-0.3.6/pyplotter/sources/functions.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/main.py` & `pyplotter-0.3.6/pyplotter/sources/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,21 @@
         self.widgetBlueFors.signalUpdateProgressBar.connect(self.statusBarMain.updateProgressBar)
         self.widgetBlueFors.signalRemoveProgressBar.connect(self.statusBarMain.removeProgressBar)
         self.widgetBlueFors.signalLoadedDataFull.connect(self.loadedDataFull)
 
         self.statusBarMain.signalCsvLoad.connect(self.widgetCSV.csvLoad)
         self.statusBarMain.signalBlueForsLoad.connect(self.widgetBlueFors.blueForsLoad)
         self.statusBarMain.signalDatabaseLoad.connect(self.tableWidgetDataBase.databaseClick)
+        self.statusBarMain.signalDatabaseLoadingStop.connect(self.tableWidgetDataBase.databaseLoadingStop)
         self.statusBarMain.signalAddCurve.connect(self.tableWidgetParameter.getData)
 
         self.tableWidgetFolder.signalSendStatusBarMessage.connect(self.statusBarMain.setStatusBarMessage)
         self.tableWidgetFolder.signalBlueForsClick.connect(self.statusBarMain.blueForsLoad)
         self.tableWidgetFolder.signalCSVClick.connect(self.statusBarMain.csvLoad)
+        self.tableWidgetFolder.signalDatabaseLoadingStop.connect(self.statusBarMain.databaseLoadingStop)
         self.tableWidgetFolder.signalDatabaseClick.connect(self.statusBarMain.databaseLoad)
         self.tableWidgetFolder.signalDatabaseClick.connect(self.checkBoxHidden.databaseClick)
         self.tableWidgetFolder.signalDatabaseClick.connect(self.checkBoxStared.databaseClick)
         self.tableWidgetFolder.signalUpdateLabelPath.connect(self.hBoxLayoutPath.updateLabelPath)
         self.tableWidgetFolder.signalDatabasePathUpdate.connect(self.tableWidgetDataBase.updateDatabasePath)
         self.tableWidgetFolder.first_call()
 
@@ -137,14 +139,16 @@
         self.tableWidgetDataBase.signalDatabaseClickDone.connect(self.checkBoxStared.databaseClickDone)
         self.tableWidgetDataBase.signalCheckBoxHiddenChecked.connect(self.checkBoxStared.checkBoxHiddenChecked)
 
         self.tableWidgetDataBase.signalUpdateCurrentDatabase.connect(self.labelCurrentDataBase.setText)
 
         self.tableWidgetDataBase.signalRunClick.connect(self.tableWidgetParameter.slotFillTableWidgetParameter)
 
+        self.tableWidgetDataBase.signalDatabaseLoadingStop.connect(self.tableWidgetFolder.databaseLoadingStop)
+
         self.tableWidgetDataBase.first_call()
 
 
 
         self.tableWidgetParameter.signalSendStatusBarMessage.connect(self.statusBarMain.setStatusBarMessage)
         self.tableWidgetParameter.signalRemoveProgressBar.connect(self.statusBarMain.removeProgressBar)
         self.tableWidgetParameter.signalUpdateProgressBar.connect(self.statusBarMain.updateProgressBar)
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/palettes.py` & `pyplotter-0.3.6/pyplotter/sources/palettes.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/pyqtgraph.py` & `pyplotter-0.3.6/pyplotter/sources/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/qcodesDatabase.py` & `pyplotter-0.3.6/pyplotter/sources/qcodesDatabase.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/runPropertiesExtra.py` & `pyplotter-0.3.6/pyplotter/sources/runPropertiesExtra.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,24 +244,24 @@
                     if len(val['stared'])>0:
                         databaseNames.append(key)
 
             return [os.path.basename(os.path.normpath(databaseName)) for databaseName in databaseNames]
 
 
 
-    def isDatabaseStared(self) -> bool:
+    def isDatabaseStared(self, databaseName: str) -> bool:
         """
         Return True if the databaseName has at least one run stared in
         the json file.
         False otherwise.
         """
 
-        if self.databaseName in self.json:
-            if 'stared' in self.json[self.databaseName]:
-                if len(self.json[self.databaseName]['stared'])>0:
+        if databaseName in self.json:
+            if 'stared' in self.json[databaseName]:
+                if len(self.json[databaseName]['stared'])>0:
 
                     return True
                 else:
                     return False
             else:
                 return False
         else:
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/widgetBlueFors.py` & `pyplotter-0.3.6/pyplotter/sources/widgetBlueFors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     signalUpdateLabelCurrentSnapshot = QtCore.pyqtSignal(str)
     signalUpdateLabelCurrentRun = QtCore.pyqtSignal(str)
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
 
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
 
-    signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     signalRemoveProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     signalLoadedDataFull = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
 
     def __init__(self, parent):
         """
         Class handling the reading of csv file.
@@ -105,16 +105,23 @@
                                      delimiter = ',',
                                      names     = ['date', 'time', 'y'],
                                      header    = None)
 
                     self.signalUpdateProgressBar.emit(progressBar, progress, 'Downloading data: {:.0f}%'.format(progress*100))
                     progress += progressIteration
 
-                    # There is a space before the day
-                    x = pandasTimestamp2Int(pd.to_datetime(df['date']+'-'+df['time'], format=' %d-%m-%y-%H:%M:%S'))
+                    try:
+                        # Old BlueFors log files
+                        # There is a space before the day
+                        x = pandasTimestamp2Int(pd.to_datetime(df['date']+'-'+df['time'], format=' %d-%m-%y-%H:%M:%S'))
+                    except:
+                        # Recent BlueFors log files
+                        # There is no space before the day
+                        x = pandasTimestamp2Int(pd.to_datetime(df['date']+'-'+df['time'], format='%d-%m-%y-%H:%M:%S'))
+
                     y = df['y'].to_numpy()*1e-3
 
                     self.paramDependentList.append({'depends_on' : ['time'],
                                                     'name'  : config[fileName]['labelText'],
                                                     'label' : config[fileName]['labelText'],
                                                     'x' : x,
                                                     'y' : y,
@@ -141,15 +148,15 @@
                        plotRef: str,
                        plotTitle: str,
                        runId: int,
                        windowTitle: str,
                        cb: QtWidgets.QCheckBox,
                        progressBar: QtWidgets.QProgressBar) -> None:
 
-        self.signalUpdateProgressBar.emit(progressBar, 100, 'Downloading data: 100%')
+        self.signalUpdateProgressBar.emit(progressBar, 100., 'Downloading data: 100%')
 
         xLabelText  = 'Time'
         xLabelUnits = ''
         zLabelText  = ''
         zLabelUnits = ''
 
         for paramDependent in self.paramDependentList:
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/widgetCSV.py` & `pyplotter-0.3.6/pyplotter/sources/widgetCSV.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     signalUpdateLabelCurrentRun = QtCore.pyqtSignal(str)
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
 
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
     signalAddSnapshot = QtCore.pyqtSignal(dict)
 
-    signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    signalUpdateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     signalRemoveProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     signalFillTableWidgetParameter = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     signalLoadedDataFull = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
 
     def __init__(self, parent):
         """
         Class handling the reading of csv file.
@@ -225,15 +225,15 @@
                        plotRef: str,
                        plotTitle: str,
                        runId: int,
                        windowTitle: str,
                        cb: QtWidgets.QCheckBox,
                        progressBar: QtWidgets.QProgressBar) -> None:
 
-        self.signalUpdateProgressBar.emit(progressBar, 100, 'Downloading data: 100%')
+        self.signalUpdateProgressBar.emit(progressBar, 100., 'Downloading data: 100%')
 
         for paramDependent in self.paramDependentList:
             if paramDependent['name'] == dependentParamName:
                 data = (paramDependent['x'], paramDependent['y'])
 
         xLabelText  = self.independentParameter
         xLabelUnits = ''
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/widgetPlot.py` & `pyplotter-0.3.6/pyplotter/sources/widgetPlot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/widgetPlot1d.py` & `pyplotter-0.3.6/pyplotter/sources/widgetPlot1d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/widgetPlot2d.py` & `pyplotter-0.3.6/pyplotter/sources/widgetPlot2d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/workers/checkNbRunDatabase.py` & `pyplotter-0.3.6/pyplotter/sources/workers/checkNbRunDatabase.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         for twait in range(config['delayBetweendataBaseNbRunCheck']):
             # We check if the thread ias being stopped
             if self._stop:
                 return
             elapsedTime = config['delayBetweendataBaseNbRunCheck']-twait
             self.signal.addStatusBarMessage.emit(' (Check for new run in {}s)'.format(elapsedTime),
                                                   'green')
-            QtTest.QTest.qWait(1000)
+            QtCore.QThread.msleep(1000)
 
         # We check if the thread ias being stopped
         if self._stop:
             return
         # Queue will contain the nb of run in the database
         queueNbRun: mp.Queue = mp.Queue()
 
@@ -73,23 +73,25 @@
 
 
         nbTotalRun: int = queueNbRun.get()
 
         queueNbRun.close()
         queueNbRun.join_thread()
 
+        self.worker.join()
+
         # We check if the thread ias being stopped
         if self._stop:
             return
 
         if self.nbTotalRun<nbTotalRun:
             self.signal.addStatusBarMessage.emit(' (New run detected)',
                                                   'orange')
-            QtTest.QTest.qWait(500)
+            QtCore.QThread.msleep(500)
             self.signal.dataBaseUpdate.emit(self.databaseAbsPath)
         else:
             self.signal.addStatusBarMessage.emit(' (No run detected)',
                                                   'black')
-            QtTest.QTest.qWait(500)
+            QtCore.QThread.msleep(500)
             # In any case, we rerun the thread
             self.signal.dataBaseCheckNbRun.emit(self.databaseAbsPath,
                                                 nbTotalRun)
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/workers/loadDataBase.py` & `pyplotter-0.3.6/pyplotter/sources/workers/loadDataBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     # Signal used to update the status bar
     sendStatusBarMessage = QtCore.pyqtSignal(str, str)
     # Signal used to add n rows in the database table
     addRows = QtCore.pyqtSignal(list, list, list, list, list, list, list, list, list, list, list, int, str)
     # Signal used to update the progress bar
-    updateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    updateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     # When the run method is done
     databaseClickDone = QtCore.pyqtSignal(QtWidgets.QProgressBar, bool, str, int)
 
 class LoadDataBaseThread(QtCore.QRunnable):
 
 
     def __init__(self, databaseAbsPath:str,
@@ -39,14 +39,17 @@
 
         self.signal = LoadDataBaseSignal()
 
 
         self.databaseAbsPath = databaseAbsPath
         self.progressBar     = progressBar
 
+        # If set to True, stop the run
+        self._stop = False
+
 
 
     @QtCore.pyqtSlot()
     def run(self):
         """
         Method launched by the worker.
         Go through the runs and send a signal for each new entry.
@@ -73,38 +76,47 @@
         self.worker.start()
 
         # Here, we loop until the data transfer is done.
         # In each loop, we check the transfer progression and update the progress
         # bar
         done = False
         while not done:
-            QtTest.QTest.qWait(config['delayBetweenProgressBarUpdate'])
+            QtCore.QThread.msleep(config['delayBetweenProgressBarUpdate'])
+
+            # We check if the thread ias being stopped
+            if self._stop:
+                return
 
             progressBar = queueProgressBar.get()
             queueProgressBar.put(progressBar)
 
-            self.signal.updateProgressBar.emit(self.progressBar, progressBar, '')
+            self.signal.updateProgressBar.emit(self.progressBar, progressBar, 'Loading database: {:.0f}%'.format(progressBar))
 
             done = queueDone.get()
             queueDone.put(done)
 
         runInfos: dict = queueData.get()
         queueData.close()
         queueData.join_thread()
         queueProgressBar.close()
         queueProgressBar.join_thread()
         queueDone.close()
         queueDone.join_thread()
 
+        self.worker.join()
+
+        # We check if the thread ias being stopped
+        if self._stop:
+            return
 
 
         # If database is empty
         if runInfos is None:
             self.signal.sendStatusBarMessage.emit('Database empty', 'red')
-            QtTest.QTest.qWait(1000) # To let user see the error message
+            QtCore.QThread.msleep(1000) # To let user see the error message
             self.signal.databaseClickDone.emit(self.progressBar, # progressBar
                                                True, #error
                                                '', # databaseAbsPath
                                                0) #nbTotalRun
             return
 
         # Going through the database here
@@ -151,15 +163,15 @@
                                           guid,
                                           started,
                                           completed,
                                           duration,
                                           runRecords,
                                           nbTotalRun,
                                           self.databaseAbsPath)
-                self.signal.updateProgressBar.emit(self.progressBar, int(runId[0]/nbTotalRun*100), 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
+                self.signal.updateProgressBar.emit(self.progressBar, runId[0]/nbTotalRun*100, 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
 
 
                 runId           = []
                 dim             = []
                 experimentName  = []
                 sampleName      = []
                 runName         = []
@@ -181,14 +193,14 @@
                                       guid,
                                       started,
                                       completed,
                                       duration,
                                       runRecords,
                                       nbTotalRun,
                                       self.databaseAbsPath)
-            self.signal.updateProgressBar.emit(self.progressBar, int(runId[0]/nbTotalRun*100), 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
+            self.signal.updateProgressBar.emit(self.progressBar, runId[0]/nbTotalRun*100, 'Displaying database: run '+str(runId[0])+'/'+str(nbTotalRun))
 
         # Signal that the whole database has been looked at
         self.signal.databaseClickDone.emit(self.progressBar, # progressBar
                                            False, #error
                                            self.databaseAbsPath, # databaseAbsPath
                                            nbTotalRun) #nbTotalRun
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromCache.py` & `pyplotter-0.3.6/pyplotter/sources/workers/loadDataFromCache.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/sources/workers/loadDataFromRun.py` & `pyplotter-0.3.6/pyplotter/sources/workers/loadDataFromRun.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # xLabelText: str, xLabelUnits: str,
     # yLabelText: str, yLabelUnits: str,
     # zLabelText: str, zLabelUnits: str,
     loadedDataFull = QtCore.pyqtSignal(int, str, str, str, str, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar, tuple, str, str, str, str, str, str, bool)
     # Signal used to update the status bar
     sendStatusBarMessage = QtCore.pyqtSignal(str, str)
     # Signal to update the progress bar
-    updateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    updateProgressBar = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     # Signal when the data download is done but the database is empty
     # Useful for the starting of the liveplot
     loadedDataEmpty = QtCore.pyqtSignal(QtWidgets.QCheckBox, QtWidgets.QProgressBar)
 
 
 
 
@@ -129,15 +129,15 @@
         # Here, we loop until the data transfer is done.
         # In each loop, we check the transfer progression and update the progress
         # bar
         # We display information only if different than the previous iteration
         # to avoid blinking
         done = False
         while not done:
-            QtTest.QTest.qWait(config['delayBetweenProgressBarUpdate'])
+            QtCore.QThread.msleep(config['delayBetweenProgressBarUpdate'])
 
             progressBarNew = queueProgressBar.get()
             queueProgressBar.put(progressBarNew)
             if progressBarNew!=progressBar:
                 progressBar = progressBarNew
                 self.signal.updateProgressBar.emit(self.progressBar, progressBar, 'Downloading data: {:.0f}%'.format(progressBar))
 
@@ -154,14 +154,17 @@
         queueData.close()
         queueData.join_thread()
         queueProgressBar.close()
         queueProgressBar.join_thread()
         queueDone.close()
         queueDone.join_thread()
 
+
+        self.worker.join()
+
         # If getParameterDatamp failed, or the database is empty we emit a specific
         # signal which will flag the data download as done without launching a
         # new plot window
         if d is None:
             self.signal.sendStatusBarMessage.emit('Extracting data failed...', 'red')
             self.signal.loadedDataEmpty.emit(self.cb,
                                              self.progressBar)
```

### Comparing `pyplotter-0.3.5/pyplotter/sources/workers/loadRunInfo.py` & `pyplotter-0.3.6/pyplotter/sources/workers/loadRunInfo.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/checkBoxHidden.py` & `pyplotter-0.3.6/pyplotter/ui/checkBoxHidden.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,11 +58,11 @@
     def databaseClick(self):
         # Disable interactivity
         self.setChecked(False)
         self.setEnabled(False)
 
 
 
-    @QtCore.pyqtSlot()
-    def databaseClickDone(self):
+    @QtCore.pyqtSlot(str)
+    def databaseClickDone(self, databaseAbsPath: str):
         # Enable database interaction
         self.setEnabled(True)
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/checkBoxStared.py` & `pyplotter-0.3.6/pyplotter/ui/checkBoxStared.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,11 +49,11 @@
     def databaseClick(self) -> None:
         # Disable interactivity
         self.setChecked(False)
         self.setEnabled(False)
 
 
 
-    @QtCore.pyqtSlot()
-    def databaseClickDone(self) -> None:
+    @QtCore.pyqtSlot(str)
+    def databaseClickDone(self, databaseAbsPath: str) -> None:
         # Enable database interaction
         self.setEnabled(True)
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormap.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogColormap.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogColormapUi.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogColormapUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogComment.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogComment.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsize.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogFontsize.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogFontsizeUi.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogFontsizeUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplot.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogLiveplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
         Call when user click on the 'LivePlot' button.
         Allow user to chose any available qcodes database in his computer.
         This database will be monitored and any new run will be plotted.
         """
 
         self.pushButtonLivePlot.setText('Loading QCoDeS...')
         # self.setStatusBarMessage()
-        QtTest.QTest.qWait(100)
+        QtCore.QThread.msleep(100)
         from qcodes import initialise_or_create_database_at, load_by_run_spec
         self.pushButtonLivePlot.setText('Select database...')
         self.loadDataset = load_by_run_spec
         # self.setStatusBarMessage('Ready')
 
         fname = QtWidgets.QFileDialog.getOpenFileName(self,
                                                       'Open QCoDeS database',
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogLiveplotUi.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogLiveplotUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogMenuDatabaseDisplay.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py` & `pyplotter-0.3.6/pyplotter/ui/dialogs/dialogMenuDatabaseDisplayUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/hBoxLayoutLabelPath.py` & `pyplotter-0.3.6/pyplotter/ui/hBoxLayoutLabelPath.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/labelSnapshot.py` & `pyplotter-0.3.6/pyplotter/ui/labelSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/lineEditSnapshot.py` & `pyplotter-0.3.6/pyplotter/ui/lineEditSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/mainWindow.py` & `pyplotter-0.3.6/pyplotter/ui/mainWindow.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/menuBar.py` & `pyplotter-0.3.6/pyplotter/ui/menuBar.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/menuDb.py` & `pyplotter-0.3.6/pyplotter/ui/menuDb.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/bluefors.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/bluefors.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/csv.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/csv.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/database.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/database.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpened.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/databaseOpened.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/databaseOpenedStared.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/databaseOpenedStared.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/databaseStared.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/databaseStared.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/folder.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/folder.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/folderEnhanced.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/folderEnhanced.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/icon.py` & `pyplotter-0.3.6/pyplotter/ui/pictures/icon.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/s2p.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/s2p.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/star.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/star.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pictures/trash.png` & `pyplotter-0.3.6/pyplotter/ui/pictures/trash.png`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFiltering.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/dialogFiltering.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/dialogFit.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/dialogFit.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculus.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxCalculus.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxCalculusUi.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxCalculusUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFT.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFFT.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFFTUi.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFFTUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFiltering.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFiltering.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxFit.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxFit.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalize.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxNormalize.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxNormalizeUi.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxNormalizeUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatistics.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxStatistics.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/groupBoxStatisticsUi.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/groupBoxStatisticsUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurve.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/widgetTabCurve.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/plot1d/widgetTabCurveUi.py` & `pyplotter-0.3.6/pyplotter/ui/plot1d/widgetTabCurveUi.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/pushButtonOpenFolder.py` & `pyplotter-0.3.6/pyplotter/ui/pushButtonOpenFolder.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/statusBar.py` & `pyplotter-0.3.6/pyplotter/ui/statusBar.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 from ..sources.config import loadConfigCurrent
 config = loadConfigCurrent()
 
 
 class StatusBar(QtWidgets.QStatusBar):
 
-    signalUpdateStyle        = QtCore.pyqtSignal(dict)
-    signalOpenDialogLivePlot = QtCore.pyqtSignal()
-    signalDatabaseLoad      = QtCore.pyqtSignal(str, QtWidgets.QProgressBar)
-    signalCsvLoad      = QtCore.pyqtSignal(str, bool, QtWidgets.QProgressBar)
-    signalBlueForsLoad      = QtCore.pyqtSignal(str, bool, QtWidgets.QProgressBar)
-    signalAddCurve     = QtCore.pyqtSignal(str, str, str, str, str, str, int, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar)
+    signalUpdateStyle         = QtCore.pyqtSignal(dict)
+    signalOpenDialogLivePlot  = QtCore.pyqtSignal()
+    signalDatabaseLoadingStop = QtCore.pyqtSignal()
+    signalDatabaseLoad        = QtCore.pyqtSignal(str, QtWidgets.QProgressBar)
+    signalCsvLoad             = QtCore.pyqtSignal(str, bool, QtWidgets.QProgressBar)
+    signalBlueForsLoad        = QtCore.pyqtSignal(str, bool, QtWidgets.QProgressBar)
+    signalAddCurve            = QtCore.pyqtSignal(str, str, str, str, str, str, int, str, QtWidgets.QCheckBox, QtWidgets.QProgressBar)
 
     def __init__(self, parent: Optional[Any]=None) -> None:
         super(StatusBar, self).__init__(parent)
 
         self.labelMessage = QtWidgets.QLabel()
         self.addPermanentWidget(self.labelMessage)
 
@@ -69,39 +70,51 @@
 
 
 
     @QtCore.pyqtSlot(str, bool)
     def csvLoad(self, databaseAbsPath: str,
                       doubleClick: bool) -> None:
 
-        progressBar = self.addProgressBar()
+        self.progressBarDatabaseLoad = self.addProgressBar()
         self.signalCsvLoad.emit(databaseAbsPath,
                                 doubleClick,
-                                progressBar)
+                                self.progressBarDatabaseLoad)
 
 
 
     @QtCore.pyqtSlot(str, bool)
     def blueForsLoad(self, databaseAbsPath: str,
                            doubleClick: bool) -> None:
 
-        progressBar = self.addProgressBar()
+        self.progressBarDatabaseLoad = self.addProgressBar()
         self.signalBlueForsLoad.emit(databaseAbsPath,
                                      doubleClick,
-                                     progressBar)
+                                     self.progressBarDatabaseLoad)
+
+
+
+    @QtCore.pyqtSlot()
+    def databaseLoadingStop(self) -> None:
+        """
+        Called from tableWidgetFolder to interupt the loading of a database.
+        Remove the progress bar of the database loading and propagate the
+        event to tableWidgetDatabase.
+        """
+
+        self.removeProgressBar(self.progressBarDatabaseLoad)
+        self.signalDatabaseLoadingStop.emit()
 
 
 
     @QtCore.pyqtSlot(str)
     def databaseLoad(self, databaseAbsPath: str) -> None:
 
-        progressBar = self.addProgressBar()
+        self.progressBarDatabaseLoad = self.addProgressBar()
         self.signalDatabaseLoad.emit(databaseAbsPath,
-                                      progressBar)
-
+                                     self.progressBarDatabaseLoad)
 
 
     @QtCore.pyqtSlot(str, str, str, str, str, str, int, str, QtWidgets.QCheckBox)
     def addCurve(self, curveId: str,
                        databaseAbsPath: str,
                        dataType: str,
                        dependentParamName: str,
@@ -134,33 +147,30 @@
     ###########################################################################
 
 
 
     @QtCore.pyqtSlot()
     def addProgressBar(self) -> QtWidgets.QProgressBar:
         """
-        Add a progress bar in the status bar.
-
-        Return
-        ------
-        progressBarKey : str
-            An unique key coming from uuid.uuid4().
+        Add a progress bar in the status bar and return it
         """
 
         # Add a progress bar in the statusbar
-        progressBarKey = str(uuid.uuid4())
         progressBar = QtWidgets.QProgressBar()
         progressBar.setMinimumWidth(400)
-        progressBar.decimal = 100
-        progressBar.decimal = 100
         progressBar.setAlignment(QtCore.Qt.AlignCenter)
         progressBar.setValue(0)
-        # setting maximum value for 2 decimal points
-        progressBar.setMaximum(100*progressBar.decimal)
+        progressBar.setMaximum(100*config['progressBarDecimal'])
         progressBar.setTextVisible(True)
+
+        palette = QtGui.QPalette()
+        palette.setColor(QtGui.QPalette.Text, QtGui.QColor(255, 165, 0)) # text, not highlight
+        palette.setColor(QtGui.QPalette.HighlightedText, QtGui.QColor(255, 165, 0)) # text, not highlight
+        progressBar.setPalette(palette)
+
         self.setSizeGripEnabled(False)
         self.addPermanentWidget(progressBar)
         self.progressBarLabel = QtWidgets.QLabel('   ')
         self.addPermanentWidget(progressBar)
         self.addPermanentWidget(self.progressBarLabel)
 
         return progressBar
@@ -178,32 +188,27 @@
 
         if hasattr(self, 'progressBarLabel'):
             self.removeWidget(self.progressBarLabel)
             del(self.progressBarLabel)
 
 
 
-    @QtCore.pyqtSlot(QtWidgets.QProgressBar, int, str)
+    @QtCore.pyqtSlot(QtWidgets.QProgressBar, float, str)
     def updateProgressBar(self, progressBar: QtWidgets.QProgressBar,
-                                val: int,
+                                val: float,
                                 text: str) -> None:
         """
         Update the progress bar in the status bar
 
         Parameters
         ----------
         progressBar : str
             progressBar from addProgressBar.
-        val : int
+        val : float
             Value of the progress.
-            Must be an int between 0 and 100.
+            Must be an float between 0 and 100.
         text : str
             Text to be shown on the progress bar.
         """
-        palette = QtGui.QPalette()
-        palette.setColor(QtGui.QPalette.Text, QtGui.QColor(255, 165, 0)) # text, not highlight
-        palette.setColor(QtGui.QPalette.HighlightedText, QtGui.QColor(255, 165, 0)) # text, not highlight
-
-        progressBar.setPalette(palette)
+        progressBar.setValue(int(val*config['progressBarDecimal']))
         progressBar.setFormat(text)
-        progressBar.setValue(int(val*progressBar.decimal))
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/tableWidgetDatabase.py` & `pyplotter-0.3.6/pyplotter/ui/tableWidgetDatabase.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,20 @@
     """
     Custom class to be able to sort numerical table column
     """
 
     # Propagated to statusBarMain
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
     signalAddStatusBarMessage  = QtCore.pyqtSignal(str, str)
-    signalUpdateProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    signalUpdateProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     signalRemoveProgressBar    = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     # Propagated to tableWidgetFolder, checkBoxHidden, checkBoxStared
-    signalDatabaseClickDone = QtCore.pyqtSignal()
+    signalDatabaseClickDone = QtCore.pyqtSignal(str)
+    # Propagated to tableWidgetFolder
+    signalDatabaseLoadingStop = QtCore.pyqtSignal(str)
     # Propagated to labelCurrentDataBase
     signalUpdateCurrentDatabase = QtCore.pyqtSignal(str)
     # Propagated to tableWidgetParameter
     signalRunClick = QtCore.pyqtSignal(int, list, dict, dict, str, str, str, str, bool)
     # Propagated to tableWidgetFolder
     signalDatabaseStars   = QtCore.pyqtSignal()
     signalDatabaseUnstars = QtCore.pyqtSignal()
@@ -101,14 +103,27 @@
         super(TableWidgetDatabase, self).keyPressEvent(event)
 
         # Emit the pressed key in human readable format in lower case
         self.keyPressed.emit(QtGui.QKeySequence(event.key()).toString().lower(), self.currentRow())
 
 
 
+    @QtCore.pyqtSlot()
+    def databaseLoadingStop(self) -> None:
+        """
+        Called from tableWidgetFolder to interupt the loading of a database.
+        """
+        if hasattr(self, 'workerLoadDatabase'):
+            # This will stop the thread
+            self.workerLoadDatabase._stop = True
+            # Propage the database absolute path to the table widget folder
+            self.signalDatabaseLoadingStop.emit(self.workerLoadDatabase.databaseAbsPath)
+
+
+
     @QtCore.pyqtSlot(str, QtWidgets.QProgressBar)
     def databaseClick(self, databaseAbsPath: str,
                             progressBar: QtWidgets.QProgressBar) -> None:
         """
         Called from the statusBarMain, when user clicks on a database.
         """
 
@@ -121,25 +136,25 @@
 
         # Modify the resize mode so that the initial view has an optimized
         # column width
         self.horizontalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
         self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Fixed)
 
         # Create a thread which will read the database
-        worker = LoadDataBaseThread(databaseAbsPath,
-                                    progressBar)
+        self.workerLoadDatabase = LoadDataBaseThread(databaseAbsPath,
+                                                     progressBar)
 
         # Connect signals
-        worker.signal.sendStatusBarMessage.connect(self.signalSendStatusBarMessage)
-        worker.signal.addRows.connect(self.databaseClickAddRows)
-        worker.signal.updateProgressBar.connect(self.signalUpdateProgressBar)
-        worker.signal.databaseClickDone.connect(self.databaseClickDone)
+        self.workerLoadDatabase.signal.sendStatusBarMessage.connect(self.signalSendStatusBarMessage)
+        self.workerLoadDatabase.signal.addRows.connect(self.databaseClickAddRows)
+        self.workerLoadDatabase.signal.updateProgressBar.connect(self.signalUpdateProgressBar)
+        self.workerLoadDatabase.signal.databaseClickDone.connect(self.databaseClickDone)
 
         # Execute the thread
-        self.threadpool.start(worker)
+        self.threadpool.start(self.workerLoadDatabase)
 
 
 
     QtCore.pyqtSlot(list, list, list, list, list, list, list, list, list, list, list, int, str)
     def databaseClickAddRows(self, lrunId           : List[int],
                                    ldim             : List[str],
                                    lexperimentName  : List[str],
@@ -251,15 +266,15 @@
 
 
         # We store the total number of run
         self.nbTotalRun = nbTotalRun
 
         # Done
         self._databaseClicking = False
-        self.signalDatabaseClickDone.emit()
+        self.signalDatabaseClickDone.emit(databaseAbsPath)
         self.signalUpdateCurrentDatabase.emit(getDatabaseNameFromAbsPath(databaseAbsPath))
 
         # We periodically check if there is not a new run to display
         self.databaseAbsPath = databaseAbsPath
         self.dataBaseCheckNbRun(databaseAbsPath,
                                 nbTotalRun)
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/tableWidgetFolder.py` & `pyplotter-0.3.6/pyplotter/ui/tableWidgetFolder.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 import os
 from time import time
 
 from ..sources.config import loadConfigCurrent
 config = loadConfigCurrent()
 from ..ui.menuDb import MenuDb
 from ..sources.runPropertiesExtra import RunPropertiesExtra
-from ..sources.functions import clearTableWidget, isBlueForsFolder, sizeof_fmt
+from ..sources.functions import (
+    clearTableWidget,
+    isBlueForsFolder,
+    sizeof_fmt,
+    getDatabaseNameFromAbsPath
+)
 
 # Get the folder path for pictures
 PICTURESPATH = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'pictures')
 
 class TableWidgetFolder(QtWidgets.QTableWidget):
     """
     Custom class to be able to sort numerical table column
     """
 
     signalSendStatusBarMessage = QtCore.pyqtSignal(str, str)
     signalDatabaseClick    = QtCore.pyqtSignal(str)
+    signalDatabaseLoadingStop    = QtCore.pyqtSignal()
     signalCSVClick         = QtCore.pyqtSignal(str, bool)
     signalBlueForsClick         = QtCore.pyqtSignal(str, bool)
     signalDatabasePathUpdate         = QtCore.pyqtSignal(str)
     signalUpdateLabelPath    = QtCore.pyqtSignal(str)
 
 
 
@@ -275,52 +281,101 @@
 
         # Load runs extra properties
         self.properties.jsonLoad(self.currentPath,
                                  self.databaseName)
 
         # To avoid the opening of two databases as once
         if self._flagDatabaseClicking:
-            return
+            # Emit signal to stop loading the previous database
+            self.signalDatabaseLoadingStop.emit()
+
         self._flagDatabaseClicking = True
 
+
+        row = self.rowNumberFromText(getDatabaseNameFromAbsPath(self.databaseAbsPath))
+
         # We show the database is now opened
-        if self.properties.isDatabaseStared():
-            self.databaseUpdateIcon('databaseOpenedStared.png')
+        if self.properties.isDatabaseStared(self.databaseName):
+            self.databaseUpdateIcon(row, 'databaseOpenedStared.png')
         else:
-            self.databaseUpdateIcon('databaseOpened.png')
+            self.databaseUpdateIcon(row, 'databaseOpened.png')
 
 
         self.signalDatabaseClick.emit(self.databaseAbsPath)
 
 
 
-    @QtCore.pyqtSlot()
-    def databaseClickDone(self) -> None:
+    @QtCore.pyqtSlot(str)
+    def databaseClickDone(self, databaseAbsPath: str) -> None:
         """
         Display the content of the clicked dataBase into the database table
         which will then contain all runs.
         """
 
+        databaseName = getDatabaseNameFromAbsPath(databaseAbsPath)
+        row = self.rowNumberFromText(databaseName)
+
         # We show the database is now closed
-        if self.properties.isDatabaseStared():
-            self.databaseUpdateIcon('databaseStared.png')
+        if self.properties.isDatabaseStared(databaseName):
+            self.databaseUpdateIcon(row, 'databaseStared.png')
         else:
-            self.databaseUpdateIcon('database.png')
+            self.databaseUpdateIcon(row, 'database.png')
 
         # To avoid the opening of two databases as once
         self._flagDatabaseClicking = False
 
 
 
-    def databaseUpdateIcon(self, iconName: str) -> None:
+    @QtCore.pyqtSlot(str)
+    def databaseLoadingStop(self, databaseAbsPath: str) -> None:
+        """
+        Called by tableWidgetDatabase when a database is stopped being loaded.
+        Basically, put back standard database icon
+        """
+
+        databaseName = getDatabaseNameFromAbsPath(databaseAbsPath)
+        row = self.rowNumberFromText(databaseName)
+
+        # We show the database is now closed
+        if self.properties.isDatabaseStared(databaseName):
+            self.databaseUpdateIcon(row, 'databaseStared.png')
+        else:
+            self.databaseUpdateIcon(row, 'database.png')
+
+
+
+    def databaseUpdateIcon(self, row: int,
+                                 iconName: str) -> None:
+        """
+        Change the icon of a database of row to the new iconName.
+
+        Args:
+            row: Row of the database to the change the icon
+            iconName: New icon name
+        """
+
+        self.item(row, 0).setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, iconName)))
 
-        item = self.item(self.currentIndex().row(), 0)
-        item.setIcon(QtGui.QIcon(os.path.join(PICTURESPATH, iconName)))
 
 
+    def rowNumberFromText(self, text: str) -> int:
+        """
+        Return the row number where the displayed text corresponds to the input
+        text.
+        If no correspondance is found, return 0.
+
+        Args:
+            text: text you want the row
+        """
+
+        for row in range(self.rowCount()):
+            if text==getDatabaseNameFromAbsPath(self.item(row, 0).text()):
+                return row
+
+        return 0
 
 
     ############################################################################
     #
     #
     #                           Called from other widgets
     #
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/tableWidgetParameter.py` & `pyplotter-0.3.6/pyplotter/ui/tableWidgetParameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class TableWidgetParameter(QtWidgets.QTableWidget):
     """
     Custom class to be able to sort numerical table column
     """
 
     signalSendStatusBarMessage       = QtCore.pyqtSignal(str, str)
-    signalUpdateProgressBar          = QtCore.pyqtSignal(QtWidgets.QProgressBar, int, str)
+    signalUpdateProgressBar          = QtCore.pyqtSignal(QtWidgets.QProgressBar, float, str)
     signalRemoveProgressBar          = QtCore.pyqtSignal(QtWidgets.QProgressBar)
     signalAddCurve                   = QtCore.pyqtSignal(str, str, str, str, str, str, int, str, QtWidgets.QCheckBox)
     signalRemoveCurve                = QtCore.pyqtSignal(str, str)
     signalCleanSnapshot              = QtCore.pyqtSignal()
     signalAddSnapshot                = QtCore.pyqtSignal(dict)
     signalLineEditSnapshotEnabled    = QtCore.pyqtSignal(bool)
     signalLabelSnapshotEnabled       = QtCore.pyqtSignal(bool)
@@ -238,15 +238,15 @@
             either "qcodes", "csv", "bluefors"
         """
 
         # Flag
         self._dataDowloadingFlag = True
 
         cb.setEnabled(False)
-        QtTest.QTest.qWait(100)
+        QtCore.QThread.msleep(100)
 
         if dataType=='qcodes':
             worker = LoadDataFromRunThread(curveId,
                                            databaseAbsPath,
                                            dependentParamName,
                                            plotRef,
                                            plotTitle,
```

### Comparing `pyplotter-0.3.5/pyplotter/ui/treeViewSnapshot.py` & `pyplotter-0.3.6/pyplotter/ui/treeViewSnapshot.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/widgetPlot1d.py` & `pyplotter-0.3.6/pyplotter/ui/widgetPlot1d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter/ui/widgetPlot2d.py` & `pyplotter-0.3.6/pyplotter/ui/widgetPlot2d.py`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/pyplotter.egg-info/PKG-INFO` & `pyplotter-0.3.6/pyplotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyplotter
-Version: 0.3.5
+Version: 0.3.6
 Summary: A data browser and vizualizer for QCoDes database, csv, s2p and BlueFors logging files.
 Home-page: https://github.com/pyplotter/pyplotter
+Author: Étienne Dumur
 Author-email: etienne.dumur@cea.fr
 Maintainer: Étienne Dumur
 Maintainer-email: etienne.dumur@cea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `pyplotter-0.3.5/pyplotter.egg-info/SOURCES.txt` & `pyplotter-0.3.6/pyplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplotter-0.3.5/setup.cfg` & `pyplotter-0.3.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7970 6c6f 7474 6572 0d0a 7665   = pyplotter..ve
-00000020: 7273 696f 6e20 3d20 302e 332e 350d 0a61  rsion = 0.3.5..a
-00000030: 7574 686f 725f 656d 6169 6c20 3d20 6574  uthor_email = et
-00000040: 6965 6e6e 652e 6475 6d75 7240 6365 612e  ienne.dumur@cea.
-00000050: 6672 0d0a 6d61 696e 7461 696e 6572 203d  fr..maintainer =
-00000060: 20c3 8974 6965 6e6e 6520 4475 6d75 720d   ..tienne Dumur.
-00000070: 0a6d 6169 6e74 6169 6e65 725f 656d 6169  .maintainer_emai
-00000080: 6c20 3d20 6574 6965 6e6e 652e 6475 6d75  l = etienne.dumu
-00000090: 7240 6365 612e 6672 0d0a 6465 7363 7269  r@cea.fr..descri
-000000a0: 7074 696f 6e20 3d20 4120 6461 7461 2062  ption = A data b
-000000b0: 726f 7773 6572 2061 6e64 2076 697a 7561  rowser and vizua
-000000c0: 6c69 7a65 7220 666f 7220 5143 6f44 6573  lizer for QCoDes
-000000d0: 2064 6174 6162 6173 652c 2063 7376 2c20   database, csv, 
-000000e0: 7332 7020 616e 6420 426c 7565 466f 7273  s2p and BlueFors
-000000f0: 206c 6f67 6769 6e67 2066 696c 6573 2e0d   logging files..
-00000100: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000110: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000120: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000130: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000140: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000150: 776e 3b20 6368 6172 7365 743d 5554 462d  wn; charset=UTF-
-00000160: 383b 2076 6172 6961 6e74 3d47 464d 0d0a  8; variant=GFM..
-00000170: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000180: 7468 7562 2e63 6f6d 2f70 7970 6c6f 7474  thub.com/pyplott
-00000190: 6572 2f70 7970 6c6f 7474 6572 0d0a 636c  er/pyplotter..cl
-000001a0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-000001b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001d0: 2033 0d0a 0949 6e74 656e 6465 6420 4175   3...Intended Au
-000001e0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-000001f0: 652f 5265 7365 6172 6368 0d0a 094f 7065  e/Research...Ope
-00000200: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000210: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000220: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
-00000230: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000240: 670d 0a6c 6963 656e 7365 203d 204d 4954  g..license = MIT
-00000250: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000260: 645f 7061 636b 6167 6573 2829 2c0d 0a0d  d_packages(),...
-00000270: 0a5b 6f70 7469 6f6e 735d 0d0a 7079 7468  .[options]..pyth
-00000280: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000290: 332e 360d 0a69 6e63 6c75 6465 5f70 6163  3.6..include_pac
-000002a0: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-000002b0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000002c0: 6573 203d 200d 0a09 7164 6172 6b73 7479  es = ...qdarksty
-000002d0: 6c65 0d0a 096c 6d66 6974 0d0a 096d 756c  le...lmfit...mul
-000002e0: 7469 7072 6f63 6573 730d 0a09 6e75 6d70  tiprocess...nump
-000002f0: 793e 3d31 2e31 372e 300d 0a09 7061 6e64  y>=1.17.0...pand
-00000300: 6173 3e3d 312e 302e 300d 0a09 706c 6174  as>=1.0.0...plat
-00000310: 666f 726d 6469 7273 0d0a 0970 796f 7065  formdirs...pyope
-00000320: 6e67 6c0d 0a09 7079 7174 350d 0a09 7079  ngl...pyqt5...py
-00000330: 7174 352d 7369 700d 0a09 7079 7174 7765  qt5-sip...pyqtwe
-00000340: 6265 6e67 696e 650d 0a09 7079 7174 6772  bengine...pyqtgr
-00000350: 6170 683e 3d30 2e31 322e 330d 0a09 7163  aph>=0.12.3...qc
-00000360: 6f64 6573 3e3d 302e 3236 2e30 0d0a 0973  odes>=0.26.0...s
-00000370: 6369 6b69 742d 7266 0d0a 0973 6369 7079  cikit-rf...scipy
-00000380: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000390: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-000003a0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-000003b0: 0970 6c6f 7474 6572 203d 2070 7970 6c6f  .plotter = pyplo
-000003c0: 7474 6572 2e70 7970 6c6f 7474 6572 3a6d  tter.pyplotter:m
-000003d0: 6169 6e0d 0a09 7079 706c 6f74 7465 7220  ain...pyplotter 
-000003e0: 3d20 7079 706c 6f74 7465 722e 7079 706c  = pyplotter.pypl
-000003f0: 6f74 7465 723a 6d61 696e 0d0a 0d0a 5b65  otter:main....[e
-00000400: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000410: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000420: 203d 2030 0d0a 0d0a                       = 0....
+00000020: 7273 696f 6e20 3d20 302e 332e 360d 0a61  rsion = 0.3.6..a
+00000030: 7574 686f 7220 3d20 c389 7469 656e 6e65  uthor = ..tienne
+00000040: 2044 756d 7572 0d0a 6175 7468 6f72 5f65   Dumur..author_e
+00000050: 6d61 696c 203d 2065 7469 656e 6e65 2e64  mail = etienne.d
+00000060: 756d 7572 4063 6561 2e66 720d 0a6d 6169  umur@cea.fr..mai
+00000070: 6e74 6169 6e65 7220 3d20 c389 7469 656e  ntainer = ..tien
+00000080: 6e65 2044 756d 7572 0d0a 6d61 696e 7461  ne Dumur..mainta
+00000090: 696e 6572 5f65 6d61 696c 203d 2065 7469  iner_email = eti
+000000a0: 656e 6e65 2e64 756d 7572 4063 6561 2e66  enne.dumur@cea.f
+000000b0: 720d 0a64 6573 6372 6970 7469 6f6e 203d  r..description =
+000000c0: 2041 2064 6174 6120 6272 6f77 7365 7220   A data browser 
+000000d0: 616e 6420 7669 7a75 616c 697a 6572 2066  and vizualizer f
+000000e0: 6f72 2051 436f 4465 7320 6461 7461 6261  or QCoDes databa
+000000f0: 7365 2c20 6373 762c 2073 3270 2061 6e64  se, csv, s2p and
+00000100: 2042 6c75 6546 6f72 7320 6c6f 6767 696e   BlueFors loggin
+00000110: 6720 6669 6c65 732e 0d0a 6c6f 6e67 5f64  g files...long_d
+00000120: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000130: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+00000140: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000150: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000160: 7874 2f6d 6172 6b64 6f77 6e3b 2063 6861  xt/markdown; cha
+00000170: 7273 6574 3d55 5446 2d38 3b20 7661 7269  rset=UTF-8; vari
+00000180: 616e 743d 4746 4d0d 0a75 726c 203d 2068  ant=GFM..url = h
+00000190: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001a0: 6d2f 7079 706c 6f74 7465 722f 7079 706c  m/pyplotter/pypl
+000001b0: 6f74 7465 720d 0a63 6c61 7373 6966 6965  otter..classifie
+000001c0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+000001d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001e0: 5079 7468 6f6e 203a 3a20 330d 0a09 496e  Python :: 3...In
+000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000200: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
+00000210: 7263 680d 0a09 4f70 6572 6174 696e 6720  rch...Operating 
+00000220: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000230: 6570 656e 6465 6e74 0d0a 0954 6f70 6963  ependent...Topic
+00000240: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+00000250: 6e67 696e 6565 7269 6e67 0d0a 6c69 6365  ngineering..lice
+00000260: 6e73 6520 3d20 4d49 540d 0a70 6163 6b61  nse = MIT..packa
+00000270: 6765 7320 3d20 6669 6e64 5f70 6163 6b61  ges = find_packa
+00000280: 6765 7328 292c 0d0a 0d0a 5b6f 7074 696f  ges(),....[optio
+00000290: 6e73 5d0d 0a70 7974 686f 6e5f 7265 7175  ns]..python_requ
+000002a0: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
+000002b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+000002c0: 7461 203d 2054 7275 650d 0a69 6e73 7461  ta = True..insta
+000002d0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+000002e0: 0971 6461 726b 7374 796c 650d 0a09 6c6d  .qdarkstyle...lm
+000002f0: 6669 740d 0a09 6d75 6c74 6970 726f 6365  fit...multiproce
+00000300: 7373 0d0a 096e 756d 7079 3e3d 312e 3137  ss...numpy>=1.17
+00000310: 2e30 0d0a 0970 616e 6461 733e 3d31 2e30  .0...pandas>=1.0
+00000320: 2e30 0d0a 0970 6c61 7466 6f72 6d64 6972  .0...platformdir
+00000330: 730d 0a09 7079 6f70 656e 676c 0d0a 0970  s...pyopengl...p
+00000340: 7971 7435 0d0a 0970 7971 7435 2d73 6970  yqt5...pyqt5-sip
+00000350: 0d0a 0970 7971 7477 6562 656e 6769 6e65  ...pyqtwebengine
+00000360: 0d0a 0970 7971 7467 7261 7068 3e3d 302e  ...pyqtgraph>=0.
+00000370: 3132 2e33 0d0a 0971 636f 6465 733e 3d30  12.3...qcodes>=0
+00000380: 2e32 362e 300d 0a09 7363 696b 6974 2d72  .26.0...scikit-r
+00000390: 660d 0a09 7363 6970 790d 0a0d 0a5b 6f70  f...scipy....[op
+000003a0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000003b0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000003c0: 6970 7473 203d 200d 0a09 706c 6f74 7465  ipts = ...plotte
+000003d0: 7220 3d20 7079 706c 6f74 7465 722e 7079  r = pyplotter.py
+000003e0: 706c 6f74 7465 723a 6d61 696e 0d0a 0970  plotter:main...p
+000003f0: 7970 6c6f 7474 6572 203d 2070 7970 6c6f  yplotter = pyplo
+00000400: 7474 6572 2e70 7970 6c6f 7474 6572 3a6d  tter.pyplotter:m
+00000410: 6169 6e0d 0a0d 0a5b 6567 675f 696e 666f  ain....[egg_info
+00000420: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000430: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000440: 0a                                       .
```

