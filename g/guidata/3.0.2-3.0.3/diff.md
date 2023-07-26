# Comparing `tmp/guidata-3.0.2.tar.gz` & `tmp/guidata-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-3.0.2.tar", last modified: Wed Jul 26 11:38:44 2023, max compression
+gzip compressed data, was "guidata-3.0.3.tar", last modified: Wed Jul 26 12:43:40 2023, max compression
```

## Comparing `guidata-3.0.2.tar` & `guidata-3.0.3.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.992524 guidata-3.0.2/
--rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.2/LICENSE
--rw-rw-rw-   0        0        0        9 2023-07-26 09:34:47.000000 guidata-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5248 2023-07-26 11:38:44.990517 guidata-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-07-18 08:47:02.000000 guidata-3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.386199 guidata-3.0.2/doc/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.388199 guidata-3.0.2/doc/_static/
--rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.2/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.2/doc/basic_example.py
--rw-rw-rw-   0        0        0     1659 2023-07-21 12:45:55.000000 guidata-3.0.2/doc/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.400197 guidata-3.0.2/doc/dev/
--rw-rw-rw-   0        0        0     2675 2023-07-21 10:37:23.000000 guidata-3.0.2/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.2/doc/dev/howto.rst
--rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.2/doc/dev/index.rst
--rw-rw-rw-   0        0        0     2171 2023-07-19 10:06:27.000000 guidata-3.0.2/doc/dev/v2_to_v3.csv
--rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.0.2/doc/dev/v2_to_v3.rst
--rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.2/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.409198 guidata-3.0.2/doc/images/
--rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.2/doc/images/basic_example.png
--rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.2/doc/images/guidata-banner.png
--rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.2/doc/images/guidata-vertical.png
--rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.2/doc/images/layout_example.png
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.430199 guidata-3.0.2/doc/images/screenshots/
--rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.2/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.2/doc/images/screenshots/activable_dataset.png
--rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.2/doc/images/screenshots/all_features.png
--rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.2/doc/images/screenshots/all_items.png
--rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.2/doc/images/screenshots/bool_selector.png
--rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.2/doc/images/screenshots/datasetgroup.png
--rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.2/doc/images/screenshots/editgroupbox.png
--rw-rw-rw-   0        0        0      933 2023-07-18 09:00:42.000000 guidata-3.0.2/doc/index.rst
--rw-rw-rw-   0        0        0      181 2023-07-21 12:29:31.000000 guidata-3.0.2/doc/installation.rst
--rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.2/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.441199 guidata-3.0.2/doc/reference/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.456199 guidata-3.0.2/doc/reference/dataset/
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.2/doc/reference/dataset/dataitems.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.2/doc/reference/dataset/datatypes.rst
--rw-rw-rw-   0        0        0      144 2023-07-07 14:10:24.000000 guidata-3.0.2/doc/reference/dataset/index.rst
--rw-rw-rw-   0        0        0       34 2023-07-19 09:25:53.000000 guidata-3.0.2/doc/reference/dataset/io.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.2/doc/reference/dataset/qtwidgets.rst
--rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.2/doc/reference/guitest.rst
--rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.0.2/doc/reference/index.rst
--rw-rw-rw-   0        0        0       34 2023-07-07 14:22:12.000000 guidata-3.0.2/doc/reference/userconfig.rst
--rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.2/doc/reference/utils.rst
--rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.2/doc/reference/widgets.rst
--rw-rw-rw-   0        0        0     2460 2023-07-26 11:38:27.000000 guidata-3.0.2/doc/requirements.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.476204 guidata-3.0.2/guidata/
--rw-rw-rw-   0        0        0     3004 2023-07-26 09:52:33.000000 guidata-3.0.2/guidata/__init__.py
--rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.2/guidata/config.py
--rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.2/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.505202 guidata-3.0.2/guidata/dataset/
--rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.2/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.2/guidata/dataset/datatypes.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.518204 guidata-3.0.2/guidata/dataset/io/
--rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.2/guidata/dataset/io/__init__.py
--rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.2/guidata/dataset/io/base.py
--rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.2/guidata/dataset/io/h5fmt.py
--rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.2/guidata/dataset/io/inifmt.py
--rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.2/guidata/dataset/io/jsonfmt.py
--rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.2/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.2/guidata/env.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.520204 guidata-3.0.2/guidata/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.532204 guidata-3.0.2/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0   394832 2023-07-26 11:38:25.000000 guidata-3.0.2/guidata/guidata.chm
--rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.2/guidata/guitest.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.727964 guidata-3.0.2/guidata/images/
--rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.777967 guidata-3.0.2/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.812974 guidata-3.0.2/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.2/guidata/images/guidata-banner.svg
--rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.2/guidata/images/guidata-vertical.svg
--rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.2/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/xmin.png
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.352196 guidata-3.0.2/guidata/locale/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.352196 guidata-3.0.2/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.815968 guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.2/guidata/qthelpers.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.902513 guidata-3.0.2/guidata/tests/
--rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.2/guidata/tests/_all_tests.py
--rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.2/guidata/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.355198 guidata-3.0.2/guidata/tests/data/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.909528 guidata-3.0.2/guidata/tests/data/genreqs/
--rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.2/guidata/tests/data/genreqs/pyproject.toml
--rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.2/guidata/tests/data/genreqs/setup.cfg
--rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.2/guidata/tests/test_activable_dataset.py
--rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.2/guidata/tests/test_activable_items.py
--rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.2/guidata/tests/test_all_features.py
--rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.2/guidata/tests/test_all_items.py
--rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.2/guidata/tests/test_arrayeditor.py
--rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.2/guidata/tests/test_bool_selector.py
--rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.2/guidata/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.2/guidata/tests/test_codeeditor.py
--rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.2/guidata/tests/test_collectionseditor.py
--rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/test_config.py
--rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.2/guidata/tests/test_console.py
--rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.2/guidata/tests/test_data.py
--rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.2/guidata/tests/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/test_datasetgroup.py
--rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.2/guidata/tests/test_disthelpers.py
--rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.2/guidata/tests/test_editgroupbox.py
--rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.2/guidata/tests/test_genreqs.py
--rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.2/guidata/tests/test_importwizard.py
--rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.2/guidata/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.2/guidata/tests/test_item_order.py
--rw-rw-rw-   0        0        0     1142 2023-07-26 11:35:40.000000 guidata-3.0.2/guidata/tests/test_loadsave_hdf5.py
--rw-rw-rw-   0        0        0     1078 2023-07-26 11:35:40.000000 guidata-3.0.2/guidata/tests/test_loadsave_json.py
--rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.2/guidata/tests/test_no_qt.py
--rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.2/guidata/tests/test_objecteditor.py
--rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.2/guidata/tests/test_rotatedlabel.py
--rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.2/guidata/tests/test_text.py
--rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.2/guidata/tests/test_translations.py
--rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.2/guidata/tests/test_userconfig_app.py
--rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.2/guidata/userconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.925519 guidata-3.0.2/guidata/utils/
--rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.2/guidata/utils/__init__.py
--rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.2/guidata/utils/disthelpers.py
--rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/utils/encoding.py
--rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.2/guidata/utils/genreqs.py
--rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.2/guidata/utils/gettext_helpers.py
--rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.2/guidata/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.962516 guidata-3.0.2/guidata/widgets/
--rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.2/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.2/guidata/widgets/arrayeditor.py
--rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.2/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.2/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.988517 guidata-3.0.2/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.2/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.2/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.2/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.2/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.2/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.2/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.2/guidata/widgets/dockable.py
--rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.2/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.2/guidata/widgets/rotatedlabel.py
--rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/texteditor.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.489202 guidata-3.0.2/guidata.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5799 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1949 2023-07-26 09:34:07.000000 guidata-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 11:38:44.992524 guidata-3.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.597999 guidata-3.0.3/
+-rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0        9 2023-07-26 09:34:47.000000 guidata-3.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6016 2023-07-26 12:43:40.597000 guidata-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2977 2023-07-26 12:41:54.000000 guidata-3.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.025030 guidata-3.0.3/doc/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.027030 guidata-3.0.3/doc/_static/
+-rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.3/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.3/doc/basic_example.py
+-rw-rw-rw-   0        0        0     1659 2023-07-21 12:45:55.000000 guidata-3.0.3/doc/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.039031 guidata-3.0.3/doc/dev/
+-rw-rw-rw-   0        0        0     2675 2023-07-21 10:37:23.000000 guidata-3.0.3/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.3/doc/dev/howto.rst
+-rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.3/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     2171 2023-07-19 10:06:27.000000 guidata-3.0.3/doc/dev/v2_to_v3.csv
+-rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.0.3/doc/dev/v2_to_v3.rst
+-rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.3/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.048046 guidata-3.0.3/doc/images/
+-rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.3/doc/images/basic_example.png
+-rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.3/doc/images/guidata-banner.png
+-rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.3/doc/images/guidata-vertical.png
+-rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.3/doc/images/layout_example.png
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.069030 guidata-3.0.3/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.3/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.3/doc/images/screenshots/activable_dataset.png
+-rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.3/doc/images/screenshots/all_features.png
+-rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.3/doc/images/screenshots/all_items.png
+-rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.3/doc/images/screenshots/bool_selector.png
+-rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.3/doc/images/screenshots/datasetgroup.png
+-rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.3/doc/images/screenshots/editgroupbox.png
+-rw-rw-rw-   0        0        0      933 2023-07-18 09:00:42.000000 guidata-3.0.3/doc/index.rst
+-rw-rw-rw-   0        0        0      181 2023-07-21 12:29:31.000000 guidata-3.0.3/doc/installation.rst
+-rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.3/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.086038 guidata-3.0.3/doc/reference/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.096032 guidata-3.0.3/doc/reference/dataset/
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.3/doc/reference/dataset/dataitems.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.3/doc/reference/dataset/datatypes.rst
+-rw-rw-rw-   0        0        0      144 2023-07-07 14:10:24.000000 guidata-3.0.3/doc/reference/dataset/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-19 09:25:53.000000 guidata-3.0.3/doc/reference/dataset/io.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.3/doc/reference/dataset/qtwidgets.rst
+-rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.3/doc/reference/guitest.rst
+-rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.0.3/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-07 14:22:12.000000 guidata-3.0.3/doc/reference/userconfig.rst
+-rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.3/doc/reference/utils.rst
+-rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.3/doc/reference/widgets.rst
+-rw-rw-rw-   0        0        0     2460 2023-07-26 12:43:21.000000 guidata-3.0.3/doc/requirements.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.114032 guidata-3.0.3/guidata/
+-rw-rw-rw-   0        0        0     3004 2023-07-26 12:34:51.000000 guidata-3.0.3/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.3/guidata/config.py
+-rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.3/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.145033 guidata-3.0.3/guidata/dataset/
+-rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.3/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.3/guidata/dataset/datatypes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.159032 guidata-3.0.3/guidata/dataset/io/
+-rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.3/guidata/dataset/io/__init__.py
+-rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.3/guidata/dataset/io/base.py
+-rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.3/guidata/dataset/io/h5fmt.py
+-rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.3/guidata/dataset/io/inifmt.py
+-rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.3/guidata/dataset/io/jsonfmt.py
+-rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.3/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.3/guidata/env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.161033 guidata-3.0.3/guidata/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.176037 guidata-3.0.3/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0   394832 2023-07-26 12:43:19.000000 guidata-3.0.3/guidata/guidata.chm
+-rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.3/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.298038 guidata-3.0.3/guidata/images/
+-rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.342877 guidata-3.0.3/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.390044 guidata-3.0.3/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.3/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.3/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.3/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.979028 guidata-3.0.3/guidata/locale/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.984030 guidata-3.0.3/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.394045 guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.3/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.497996 guidata-3.0.3/guidata/tests/
+-rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.3/guidata/tests/_all_tests.py
+-rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.3/guidata/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:39.989056 guidata-3.0.3/guidata/tests/data/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.501996 guidata-3.0.3/guidata/tests/data/genreqs/
+-rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.3/guidata/tests/data/genreqs/pyproject.toml
+-rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.3/guidata/tests/data/genreqs/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.3/guidata/tests/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.3/guidata/tests/test_activable_items.py
+-rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.3/guidata/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.3/guidata/tests/test_all_items.py
+-rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.3/guidata/tests/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.3/guidata/tests/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.3/guidata/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.3/guidata/tests/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.3/guidata/tests/test_collectionseditor.py
+-rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/test_config.py
+-rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.3/guidata/tests/test_console.py
+-rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.3/guidata/tests/test_data.py
+-rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.3/guidata/tests/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.3/guidata/tests/test_datasetgroup.py
+-rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.3/guidata/tests/test_disthelpers.py
+-rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.3/guidata/tests/test_editgroupbox.py
+-rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.3/guidata/tests/test_genreqs.py
+-rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.3/guidata/tests/test_importwizard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.3/guidata/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.3/guidata/tests/test_item_order.py
+-rw-rw-rw-   0        0        0     1142 2023-07-26 11:35:40.000000 guidata-3.0.3/guidata/tests/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1078 2023-07-26 11:35:40.000000 guidata-3.0.3/guidata/tests/test_loadsave_json.py
+-rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.3/guidata/tests/test_no_qt.py
+-rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.3/guidata/tests/test_objecteditor.py
+-rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.3/guidata/tests/test_rotatedlabel.py
+-rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.3/guidata/tests/test_text.py
+-rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.3/guidata/tests/test_translations.py
+-rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.3/guidata/tests/test_userconfig_app.py
+-rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.3/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.526996 guidata-3.0.3/guidata/utils/
+-rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.3/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.3/guidata/utils/disthelpers.py
+-rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.3/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.3/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.3/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.562998 guidata-3.0.3/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.3/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.3/guidata/widgets/arrayeditor.py
+-rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.3/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.3/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.594999 guidata-3.0.3/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.3/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.3/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.3/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.3/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.3/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.3/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.3/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.3/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.3/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.3/guidata/widgets/texteditor.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:40.129033 guidata-3.0.3/guidata.egg-info/
+-rw-rw-rw-   0        0        0     6016 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5799 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 12:43:39.000000 guidata-3.0.3/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1974 2023-07-26 12:28:44.000000 guidata-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:43:40.597999 guidata-3.0.3/setup.cfg
```

### Comparing `guidata-3.0.2/LICENSE` & `guidata-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/PKG-INFO` & `guidata-3.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.2
-Summary: Signal and image processing software
+Version: 3.0.3
+Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -55,15 +55,14 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # guidata: Automatic GUI generation for easy dataset editing and display with Python
 
-[![license](https://img.shields.io/pypi/l/guidata.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/guidata.svg)](https://pypi.org/project/guidata/)
 [![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/CODRA-Ingenierie-Informatique/guidata/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/guidata.svg)](https://pypi.python.org/pypi/guidata/)
 [![download count](https://img.shields.io/conda/dn/conda-forge/guidata.svg)](https://www.anaconda.com/download/)
 
 Simple example of ``guidata`` datasets embedded in an application window:
 
@@ -97,20 +96,38 @@
 * HDF5 I/O helpers
 * misc. utils
 
 ## Dependencies
 
 ### Requirements
 
-* Python 3.7+
+* Python 3.8+
 * [PyQt5](https://pypi.python.org/pypi/PyQt5) (Python Qt bindings)
 * [QtPy](https://pypi.org/project/QtPy/) (abstraction layer for Python-Qt binding libraries)
 * [h5py](https://pypi.org/project/h5py/) (interface to the HDF5 data format)
 * [NumPy](https://pypi.org/project/numpy/) (operations on multidimensional arrays)
+* [requests](https://pypi.org/project/requests/) (HTTP library)
+* [tomli](https://pypi.org/project/tomli/) (TOML parser)
+
+### Optional dependencies
+
+For some editing widgets:
+
+* [pillow](https://pypi.org/project/Pillow/) (image processing library)
+* [pandas](https://pypi.org/project/pandas/) (data analysis library)
+
+For documentation generation:
+
+* [sphinx](https://pypi.org/project/Sphinx/) (Python documentation generator)
+* [sphinx-copybutton](https://pypi.org/project/sphinx-copybutton/) (add a copy button to each of your code cells)
+* [sphinx_qt_documentation](https://pypi.org/project/sphinx-qt-documentation/) (plugin for proper resolve intersphinx references for Qt elements)
+* [python-docs-theme](https://pypi.org/project/python-docs-theme/) (Python documentation theme)
 
 ## Installation
 
 ### From the source package
 
+Using ``build``:
+
 ```bash
-python setup.py install
+python -m build
 ```
```

### Comparing `guidata-3.0.2/README.md` & `guidata-3.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # guidata: Automatic GUI generation for easy dataset editing and display with Python
 
-[![license](https://img.shields.io/pypi/l/guidata.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/guidata.svg)](https://pypi.org/project/guidata/)
 [![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/CODRA-Ingenierie-Informatique/guidata/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/guidata.svg)](https://pypi.python.org/pypi/guidata/)
 [![download count](https://img.shields.io/conda/dn/conda-forge/guidata.svg)](https://www.anaconda.com/download/)
 
 Simple example of ``guidata`` datasets embedded in an application window:
 
@@ -38,20 +37,38 @@
 * HDF5 I/O helpers
 * misc. utils
 
 ## Dependencies
 
 ### Requirements
 
-* Python 3.7+
+* Python 3.8+
 * [PyQt5](https://pypi.python.org/pypi/PyQt5) (Python Qt bindings)
 * [QtPy](https://pypi.org/project/QtPy/) (abstraction layer for Python-Qt binding libraries)
 * [h5py](https://pypi.org/project/h5py/) (interface to the HDF5 data format)
 * [NumPy](https://pypi.org/project/numpy/) (operations on multidimensional arrays)
+* [requests](https://pypi.org/project/requests/) (HTTP library)
+* [tomli](https://pypi.org/project/tomli/) (TOML parser)
+
+### Optional dependencies
+
+For some editing widgets:
+
+* [pillow](https://pypi.org/project/Pillow/) (image processing library)
+* [pandas](https://pypi.org/project/pandas/) (data analysis library)
+
+For documentation generation:
+
+* [sphinx](https://pypi.org/project/Sphinx/) (Python documentation generator)
+* [sphinx-copybutton](https://pypi.org/project/sphinx-copybutton/) (add a copy button to each of your code cells)
+* [sphinx_qt_documentation](https://pypi.org/project/sphinx-qt-documentation/) (plugin for proper resolve intersphinx references for Qt elements)
+* [python-docs-theme](https://pypi.org/project/python-docs-theme/) (Python documentation theme)
 
 ## Installation
 
 ### From the source package
 
+Using ``build``:
+
 ```bash
-python setup.py install
+python -m build
 ```
```

### Comparing `guidata-3.0.2/doc/_static/favicon.ico` & `guidata-3.0.3/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/basic_example.py` & `guidata-3.0.3/doc/basic_example.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/conf.py` & `guidata-3.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/dev/contribute.rst` & `guidata-3.0.3/doc/dev/contribute.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/dev/howto.rst` & `guidata-3.0.3/doc/dev/howto.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/dev/v2_to_v3.csv` & `guidata-3.0.3/doc/dev/v2_to_v3.csv`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/dev/v2_to_v3.rst` & `guidata-3.0.3/doc/dev/v2_to_v3.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/examples.rst` & `guidata-3.0.3/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/basic_example.png` & `guidata-3.0.3/doc/images/basic_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/guidata-banner.png` & `guidata-3.0.3/doc/images/guidata-banner.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/guidata-vertical.png` & `guidata-3.0.3/doc/images/guidata-vertical.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/layout_example.png` & `guidata-3.0.3/doc/images/layout_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/__init__.png` & `guidata-3.0.3/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/activable_dataset.png` & `guidata-3.0.3/doc/images/screenshots/activable_dataset.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/all_features.png` & `guidata-3.0.3/doc/images/screenshots/all_features.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/all_items.png` & `guidata-3.0.3/doc/images/screenshots/all_items.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/bool_selector.png` & `guidata-3.0.3/doc/images/screenshots/bool_selector.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/datasetgroup.png` & `guidata-3.0.3/doc/images/screenshots/datasetgroup.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/images/screenshots/editgroupbox.png` & `guidata-3.0.3/doc/images/screenshots/editgroupbox.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/index.rst` & `guidata-3.0.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/overview.rst` & `guidata-3.0.3/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/doc/requirements.rst` & `guidata-3.0.3/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/__init__.py` & `guidata-3.0.3/guidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 =======
 
 Based on the Qt library :mod:`guidata` is a Python library generating graphical
 user interfaces for easy dataset editing and display. It also provides helpers
 and application development tools for Qt.
 """
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (images) and translations:
 DATAPATH = LOCALEPATH = ""
```

### Comparing `guidata-3.0.2/guidata/config.py` & `guidata-3.0.3/guidata/config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/configtools.py` & `guidata-3.0.3/guidata/configtools.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/__init__.py` & `guidata-3.0.3/guidata/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/dataitems.py` & `guidata-3.0.3/guidata/dataset/dataitems.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/datatypes.py` & `guidata-3.0.3/guidata/dataset/datatypes.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/io/__init__.py` & `guidata-3.0.3/guidata/dataset/io/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/io/base.py` & `guidata-3.0.3/guidata/dataset/io/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/io/h5fmt.py` & `guidata-3.0.3/guidata/dataset/io/h5fmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/io/inifmt.py` & `guidata-3.0.3/guidata/dataset/io/inifmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/io/jsonfmt.py` & `guidata-3.0.3/guidata/dataset/io/jsonfmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/qtitemwidgets.py` & `guidata-3.0.3/guidata/dataset/qtitemwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/qtwidgets.py` & `guidata-3.0.3/guidata/dataset/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/dataset/textedit.py` & `guidata-3.0.3/guidata/dataset/textedit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/env.py` & `guidata-3.0.3/guidata/env.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/external/darkdetect/__init__.py` & `guidata-3.0.3/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.0.3/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.0.3/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.0.3/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/guidata.chm` & `guidata-3.0.3/guidata/guidata.chm`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 4954 5346 0300 0000 6000 0000 0100 0000  ITSF....`.......
-00000010: 4017 d5af 0c04 0000 10fd 017c aa7b d011  @..........|.{..
+00000010: ebb4 37c1 0c04 0000 10fd 017c aa7b d011  ..7........|.{..
 00000020: 9e0c 00a0 c922 e6ec 11fd 017c aa7b d011  .....".....|.{..
 00000030: 9e0c 00a0 c922 e6ec 6000 0000 0000 0000  ....."..`.......
 00000040: 1800 0000 0000 0000 7800 0000 0000 0000  ........x.......
 00000050: 5410 0000 0000 0000 cc10 0000 0000 0000  T...............
 00000060: fe01 0000 0000 0000 5006 0600 0000 0000  ........P.......
 00000070: 0000 0000 0000 0000 4954 5350 0100 0000  ........ITSP....
 00000080: 5400 0000 0a00 0000 0010 0000 0200 0000  T...............
@@ -297,25 +297,25 @@
 00001280: 0000 6aa9 0100 0000 0000 78af 0100 0000  ..j.......x.....
 00001290: 0000 26dd 0100 0000 0000 7e55 0200 0000  ..&.......~U....
 000012a0: 0000 52ce 0200 0000 0000 1842 0300 0000  ..R........B....
 000012b0: 0000 b0b5 0300 0000 0000 f62c 0400 0000  ...........,....
 000012c0: 0000 3ea1 0400 0000 0000 f019 0500 0000  ..>.............
 000012d0: 0000 243e 0500 0000 0000 1245 0500 0000  ..$>.......E....
 000012e0: 0000 109c 0500 0000 0000 a2d2 0500 0000  ................
-000012f0: 0000 0300 0000 0a00 0400 b105 c164 0900  .............d..
+000012f0: 0000 0300 0000 0a00 0400 e714 c164 0900  .............d..
 00001300: 1600 4848 4120 5665 7273 696f 6e20 342e  ..HHA Version 4.
 00001310: 3734 2e38 3730 3200 0400 2400 0904 0000  74.8702...$.....
 00001320: 0000 0000 0100 0000 0100 0000 0000 0000  ................
-00001330: 8553 d4af b5bf d901 0000 0000 0000 0000  .S..............
+00001330: 46f1 36c1 bebf d901 0000 0000 0000 0000  F.6.............
 00001340: 0200 0b00 696e 6465 782e 6874 6d6c 0003  ....index.html..
 00001350: 0013 0067 7569 6461 7461 2033 2e30 204d  ...guidata 3.0 M
 00001360: 616e 7561 6c00 0600 0800 6775 6964 6174  anual.....guidat
 00001370: 6100 0500 0800 6775 6964 6174 6100 0c00  a.....guidata...
-00001380: 0400 0000 0000 0d00 0010 5423 534d 1d32  ..........T#SM.2
-00001390: 3501 0100 0000 5b01 0000 0000 0000 ffff  5.....[.........
+00001380: 0400 0000 0000 0d00 0010 5423 534d 7e9f  ..........T#SM~.
+00001390: 7001 0100 0000 5b01 0000 0000 0000 ffff  p.....[.........
 000013a0: ffff 0000 0000 0100 0000 ffff ffff ffff  ................
 000013b0: ffff ffff ffff 2712 8000 ffff ffff ffff  ......'.........
 000013c0: ffff ffff ffff ffff ffff 0000 0000 0100  ................
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -24072,356 +24072,356 @@
 0005e070: fd95 92eb cc62 f87d 3085 7dfb f1fa 18a6  .....b.}0.}.....
 0005e080: b71f bc0b 7055 574c 7fef 8035 f562 c7e4  ....pUWL...5.b..
 0005e090: 857c 7cf1 175f f1c5 5f7c dd3f 5010 2f3e  .||.._.._|.?P./>
 0005e0a0: fd38 2506 a0a3 97fd e273 1508 2f1d 3cc0  .8%......s../.<.
 0005e0b0: 04f7 4e37 3558 3efe 3ea5 ff1d f7a4 2ddb  ..N75X>.>.....-.
 0005e0c0: 873c f338 0139 7a09 ea63 c189 d7de 7a1b  .<.8.9z..c....z.
 0005e0d0: ddcf 17f2 f1c5 5f7c c517 7cf1 175f f1c5  ......_|..|.._..
-0005e0e0: 5f7c c517 7cf1 46fb d191 3168 6cf9 78bc  _|..|.F...1hl.x.
-0005e0f0: a9f1 c583 86ef 07f0 dfbf 49b0 46a3 1f4e  ..........I.F..N
-0005e100: f3a9 fb49 e20b bef8 8b2f f8e2 2fbe e28b  ...I...../../...
-0005e110: bef8 8b2f f8e2 7ebe 4253 b47d c903 0a51  .../..~.BS.}...Q
-0005e120: 146c 8411 4164 e0f6 00ff e126 209c 792a  .l..Ad.....& .y*
-0005e130: c8b0 895d 940a b015 1e6a 182a 0354 fc29  ...].....j.*.T.)
-0005e140: 3a56 cc30 923d 888c 0be6 8543 1b48 07bb  :V.0.=.....C.H..
-0005e150: d82d 355f f96c 81c0 88bf d001 0f0f 6e0c  .-5_.l........n.
-0005e160: a80e 0728 b2c2 ba1a e8fc 163c 0bec 9dc6  ...(.......<....
-0005e170: d65e a286 071b 8a20 0ac6 d080 5758 d058  .^..... ....WX.X
-0005e180: f299 1a11 81c3 d6c0 bf5f 2d24 d10c 2e70  ........._-$...p
-0005e190: 5240 b151 b61d a173 084e 910d 22e2 4326  R@.Q...s.N..".C&
-0005e1a0: ef83 0e14 88e6 5d3e db63 174a 79ca c437  ......]>.c.Jy..7
-0005e1b0: 9be0 50f4 c26c 2103 7241 8b81 d204 ba02  ..P..l!.rA......
-0005e1c0: 5086 8f13 ce45 790d 4502 17bc 6e70 7107  P....Ey.E...npq.
-0005e1d0: 92c2 d719 42c9 110c 460d 5943 04bf 64b3  ....B...F.YC..d.
-0005e1e0: 18c0 858f 1d2e 6518 8b07 0a46 7f5f 85bf  ......e....F._..
-0005e1f0: 9691 fc80 56fc e920 b5c1 5600 ba40 4483  ....V.. ..V..@D.
-0005e200: 5b60 60b0 f082 5638 c6c0 c903 5321 c4d0  [``...V8....S!..
-0005e210: 2273 5122 3cf4 4411 95ce 0c1a d21d af04  "sQ"<.D.........
-0005e220: c21f 3864 4809 b584 1b1b 6e87 d7c0 df7f  ..8dH.....n.....
-0005e230: 1c08 0c14 14da 2f62 64c3 8642 f849 106d  ....../bd..B.I.m
-0005e240: a124 0d3f 03de 5769 8fe1 9a60 43a6 3260  .$.?..Wi...`C.2`
-0005e250: b129 e85d c9d0 de40 f859 f064 3c51 c015  .).]...@.Y.d<Q..
-0005e260: 2128 e06b c881 706a 0e22 e015 602b bbcf  !(.k..pj."..`+..
-0005e270: ba05 2d11 8700 040f 6573 13d8 d0a1 129b  ..-.....es......
-0005e280: 8446 1f1a 2093 2006 2018 40e1 97d9 e406  .F.. . . .@.....
-0005e290: 5411 4fc3 70fc 5550 8fa1 8d61 8375 2103  T.O.p.UP...a.u!.
-0005e2a0: 3521 df43 ac85 e064 41d6 e0c5 0328 c335  5!.C...dA....(.5
-0005e2b0: 86c2 6a8a 4b03 50f0 6ada 089e 185e 15e2  ..j.K.P.j....^..
-0005e2c0: 4bf0 1540 2ed0 c0a0 1d52 7108 1138 3089  K..@.....Rq..80.
-0005e2d0: c28e 080a 8296 314f c983 50ac 2126 7f0a  ......1O..P.!&..
-0005e2e0: 1323 0834 f070 8163 8011 8764 4442 d400  .#.4.p.c...dDB..
-0005e2f0: e102 293f 6103 8f68 a15d 76c1 1181 59e0  ..)?a..h.]v...Y.
-0005e300: 83df b261 1648 7408 812f 5132 1c10 802b  ...a.Ht../Q2...+
-0005e310: 064b 43cc c8c1 c026 48d4 8357 f864 4b13  .KC....&H..W.dK.
-0005e320: a20a 8634 0712 a143 a00b 8e12 1935 5504  ...4...C.....5U.
-0005e330: a541 c980 0907 0070 33c0 158e 2770 8d01  .A.....p3...'p..
-0005e340: 7e3d 6019 771c 60e1 2005 dd4c 4486 2431  ~=`.w.`. ..LD.$1
-0005e350: 2f1f df3f b8c2 7c2e 28e8 4c2b 9300 2182  /..?..|.(.L+..!.
-0005e360: acf8 c200 e50b 6645 5419 ca12 c1ee acb2  ......fET.......
-0005e370: 430e c0fc ba06 3380 40e5 35dc 1da4 d161  C.....3.@.5....a
-0005e380: 0694 4270 c7f0 6b50 a30d 75f0 8f81 7205  ..Bp..kP..u...r.
-0005e390: b562 4541 2898 187c 2421 f6ed 0ff1 9304  .bEA(..|$!......
-0005e3a0: 8464 081b 9c0a 3013 df62 3686 1321 5710  .d....0..b6..!W.
-0005e3b0: 18f3 0d38 056f ea47 0804 02a7 947f b142  ...8.o.G.......B
-0005e3c0: b0b2 cf0d e16b 0465 3078 1b63 02ac f844  .....k.e0x.c...D
-0005e3d0: 8220 b48e 071c e90a 1309 5690 e041 6ba0  . ........V..Ak.
-0005e3e0: 37e8 1514 319c 5860 a8a8 c288 cb60 c840  7...1.X`.....`.@
-0005e3f0: 1d30 121c 0d90 049b 6fb4 1dac 2554 10e5  .0......o...%T..
-0005e400: f593 aab8 b03b 69de 13d8 85d0 8247 780a  .....;i......Gx.
-0005e410: 2167 a2e0 4036 fc11 3033 6234 0533 7090  !g..@6..03b4.3p.
-0005e420: 12ec cf98 ae10 eebc ecf3 d8f0 40e2 3054  ............@.0T
-0005e430: 03a7 da7b d9b8 76b0 153d 002a 4157 60cb  ...{..v..=.*AW`.
-0005e440: d364 26a8 1514 2d3c c5c0 0a0e a619 bb90  .d&...-<........
-0005e450: 7b15 1a1b 870b b0c2 a003 1e19 9c2d c035  {............-.5
-0005e460: 57a8 82ca 3b10 47c0 2b2c 2440 a1c6 8213  W...;.G.+,$@....
-0005e470: e804 d9e1 2f1f df78 64c3 2408 0479 1c9c  ..../..xd.$..y..
-0005e480: 9a35 082e 0544 9ac6 1ba1 ff15 42ed 2004  .5...D......B. .
-0005e490: c403 333a b680 e035 ae88 01f0 1b10 3806  ..3:...5......8.
-0005e4a0: b41a 4702 28d8 8992 347c f5ed 3630 6076  ..G.(...4|..60`v
-0005e4b0: bfc7 b184 80bb df68 fa81 503c 5010 f69d  .......h..P<P...
-0005e4c0: 220a 5c01 f204 a482 0940 25a0 c0ef 1fb8  ".\......@%.....
-0005e4d0: e046 0bb1 0d76 2674 ddc6 4fc0 1381 74c0  .F...v&t..O...t.
-0005e4e0: 2ef4 8a0d c440 b9fc 1608 6920 577e 5419  .....@....i W~T.
-0005e4f0: a112 c0e0 aa6c 0385 1670 0261 0d68 c504  .....l...p.a.h..
-0005e500: 3562 03d2 db1b 2c20 4102 6d21 4070 09c2  5b...., A.m!@p..
-0005e510: 85e3 07bb 164a 7408 e359 ef86 0d11 35fc  .....Jt..Y....5.
-0005e520: 8405 fc18 1ba2 b406 b086 57fc bb00 6303  ..........W...c.
-0005e530: 90db 4061 00b2 03af 4164 7647 490b d184  ..@a....AdvGI...
-0005e540: 6702 2386 b486 f81b 4c28 3c1a 0f86 03ca  g.#.....L(<.....
-0005e550: 814a 0e0e c614 839c ec51 1138 91e1 42e4  .J.......Q.8..B.
-0005e560: 160c 9882 6f0d 46c6 01ac eb77 cc58 dd60  ....o.F....w.X.`
-0005e570: bcb0 c805 ebd8 0db8 d7a1 4b83 88f3 3b64  ..........K...;d
-0005e580: 02f2 06ba 1c8c c120 3be4 8cef 5358 a1f4  ....... ;...SX..
-0005e590: 6311 4891 df13 ce86 3cec 84fe 5d21 b161  c.H.....<...]!.a
-0005e5a0: 056e 080e 2012 6042 bf3a 9b26 2027 50a2  .n.. .`B.:.& 'P.
-0005e5b0: 1055 0153 6acf 5a81 b706 c0b5 0564 a292  .U.Sj.Z......d..
-0005e5c0: 02d8 0cf6 f0db 0c66 5150 c1be d900 5690  .......fQP....V.
-0005e5d0: 6e7b 280d 123b 2817 2305 2fa2 51ff fc88  n{(..;(.#./.Q...
-0005e5e0: 1056 6ad8 e040 6980 0004 3e6f 5817 bc34  .Vj..@i...>oX..4
-0005e5f0: 60d9 2a22 9c14 084a 3667 2609 c195 d033  `.*"...J6g&....3
-0005e600: 1800 16c8 2d1e 2e00 c100 0a06 81c1 1707  ....-...........
-0005e610: f0b5 83c7 e05e 8331 3398 19ec 58c3 b216  .....^.13...X...
-0005e620: b7c2 1bc4 82da e07e 4424 fc02 870c b5e2  .......~D$......
-0005e630: 8440 f068 7b10 4a36 3183 1bb7 6918 27d0  .@.h{.J61...i.'.
-0005e640: 7070 35ec 1d2c c71e 044a 055c 7838 9b21  pp5..,...J.\x8.!
-0005e650: c118 f024 a054 83ba ecbe 8327 1760 a17b  ...$.T.....'.`.{
-0005e660: 8883 6e2b b802 2077 18b9 8015 110f 5004  ..n+.. w......P.
-0005e670: 8340 8008 4161 0469 385b 06c9 1187 a015  .@..Aa.i8[......
-0005e680: c4d4 7ed8 d6f6 2014 dd70 688c 022c 21c9  ..~... ..ph..,!.
-0005e690: 8173 82d3 db23 5bb8 2401 a4a0 22a5 c15f  .s...#[.$...".._
-0005e6a0: 60af 3688 133c f0e1 3696 1788 e0e0 dab8  `.6..<..6.......
-0005e6b0: 48e0 2b1e 5094 600e 7888 982a 4076 bfe1  H.+.P.`.x..*@v..
-0005e6c0: 300a d147 b44e 0583 2e90 536c 18f4 a806  0..G.N....Sl....
-0005e6d0: d905 f801 a06e 2113 bff0 1905 a070 1616  .....n!......p..
-0005e6e0: 17ec 5a20 bb29 0310 0f46 e830 1b6c 02b1  ..Z .)...F.0.l..
-0005e6f0: a2c7 23eb 719f ce7d 8341 084c fb1d fb74  ..#.q..}.A.L...t
-0005e700: 70c1 c213 ad34 03c1 b091 41a7 8410 5e11  p....4....A...^.
-0005e710: 9406 e402 1618 114b 6548 7818 8c23 17ba  .......KeHx..#..
-0005e720: 7068 0c26 0eca 8131 0254 dffd f293 1b90  ph.&...1.T......
-0005e730: 0b26 b0fb 0fb4 c420 5340 8c20 768c 3cc4  .&..... S@. v.<.
-0005e740: b031 8dd8 3e03 3ec1 f437 adce 8143 3a12  .1..>.>..7...C:.
-0005e750: 7122 b933 eb3e d9e0 073e 1d74 40fc 9889  q".3.>...>.t@...
-0005e760: ec1f 9a0b 03a6 0032 c8b9 4940 8f04 770c  .......2..I@..w.
-0005e770: 6809 3867 2520 8220 4d83 e830 8254 a005  h.8g% . M..0.T..
-0005e780: b825 8108 054d b477 65b3 194c 8a87 0cbf  .%...M.we..L....
-0005e790: 580a 8f51 6005 f005 2ee0 4487 6208 7207  X..Q`.....D.b.r.
-0005e7a0: d122 968d 4330 b4fb ae81 be20 fc80 f835  ."..C0..... ...5
-0005e7b0: 1018 865f 85c4 019d 6cf8 3a88 7e11 341b  ..._....l.:.~.4.
-0005e7c0: c30a 7085 4007 3dcc e1da d491 b682 39ec  ..p.@.=.......9.
-0005e7d0: b803 0f27 e015 c407 943a 7f5b 0811 01ae  ...'.....:.[....
-0005e7e0: 4292 05b5 35c8 c58f 22a4 c022 3786 73b4  B...5...".."7.s.
-0005e7f0: 9c64 b71b 3001 2026 a864 01aa 073d b09f  .d..0. &.d...=..
-0005e800: 05e1 7017 7db0 0648 03a3 fe6e 8616 0b59  ..p.}..H...n...Y
-0005e810: 183c c03a 108c 3f2a 1a19 0cb8 cd9f ac01  .<.:..?*........
-0005e820: 9280 4afc 263c 6718 7888 025e 07de 05e5  ..J.&<g.x..^....
-0005e830: 0b6d 3bd8 62f8 ac41 1960 717e 081b 3f0f  .m;.b..A.`q~..?.
-0005e840: 1076 3c36 bb31 c90d e7be b341 98d0 6936  .v<6.1.....A..i6
-0005e850: 7d44 7b3f be1b 3104 c3ef 6d1e 3eaa a6c1  }D{?..1...m.>...
-0005e860: 0b27 5a08 eec9 3004 403b dd4b 188a c147  .'Z...0.@;.K...G
-0005e870: a8a8 e6aa 38c9 c126 0083 40d3 8c78 670b  ....8..&..@..xg.
-0005e880: f809 6c24 021a 0a90 bc65 21ac 3403 280a  ..l$.....e!.4.(.
-0005e890: b522 a882 870e 34c6 432a d67e 38bf a015  ."....4.C*.~8...
-0005e8a0: f474 212e 71b1 c205 c60f 90c6 0d47 dd78  .t!.q........G.x
-0005e8b0: 5988 a8ff 2444 c169 f981 d28c 4809 2094  Y...$D.i....H. .
-0005e8c0: 9ce1 88d4 b031 6af8 6d1a c1df 7883 0c2b  .....1j.m...x..+
-0005e8d0: f6b5 0618 0a61 f91f b506 2201 c80f 5991  .....a...."...Y.
-0005e8e0: 334d 7e15 101b 6150 63cf c264 82f0 33fc  3M~...aPc..d..3.
-0005e8f0: 33b8 7e12 0619 4b07 cd6b 4a1a 0306 81fd  3.~...K..kJ.....
-0005e900: 90a9 9326 ce16 4014 dd72 8086 85aa ed81  ...&..@..r......
-0005e910: 18ac 4081 b878 66d0 2304 4fe1 fdd0 9b30  ..@..xf.#.O....0
-0005e920: fb98 41c0 2ab3 4f09 c8d9 8111 4805 7730  ..A.*.O.....H.w0
-0005e930: 580c fa26 080b 64a2 fd8a 462d 2dff 1b1d  X..&..d...F--...
-0005e940: 8b8a 0f0c 54d7 3b36 7c0f 012a 7c43 40b5  ....T.;6|..*|C@.
-0005e950: 0ea3 2b7c a700 7c18 0218 78f0 74f8 67e1  ..+|..|...x.t.g.
-0005e960: 7c3d 412c 7c76 80b6 0eb0 2d7c 8d61 7c40  |=A,|v....-|.a|@
-0005e970: 002e 78e0 5df8 b940 7768 3972 f221 57e0  ..x.]..@wh9r.!W.
-0005e980: 09a4 454b 4020 ceb6 d090 ea0e 14db 4b89  ..EK@ ........K.
-0005e990: 65cd 6660 6d5e 2572 2d17 1464 33b1 98ed  e.f`m^%r-..d3...
-0005e9a0: 4a32 5163 9123 225a 49da c1dc 2c6d 4646  J2Qc.#"ZI...,mFF
-0005e9b0: e572 3b2b 9f3a 1320 1d4b 94c3 a48b 75b8  .r;+.:. .K....u.
-0005e9c0: a258 be3a 2419 9d1d a090 6189 b03f 937e  .X.:$.....a..?.~
-0005e9d0: ba06 94cf 3cae 0be5 fe4c a789 4fc2 3d73  ....<....L..O.=s
-0005e9e0: e5d9 7824 092b 7491 3f69 6c90 27ea 2248  ..x$.+t.?il.'."H
-0005e9f0: 6674 816a f347 a8d2 4b62 13f1 0984 d120  ft.j.G..Kb..... 
-0005ea00: 62a2 990f a02b 8250 1a81 5212 8ac5 4a8c  b....+.P..R...J.
-0005ea10: 6802 2652 2ccd 0671 15ae 7144 3a2a d433  h.&R,..q..qD:*.3
-0005ea20: 2124 15e2 b680 4a9d 652c fb77 aa79 4cd5  !$....J.e,.w.yL.
-0005ea30: 695c d41c 8cf0 5b26 5163 bdb8 3b1b 8240  i\....[&Qc..;..@
-0005ea40: 9dca 0ff5 b319 33b5 1211 25de c411 1da8  ......3...%.....
-0005ea50: d1b9 8c44 d959 aea3 6f81 252e b2fb 47ad  ...D.Y..o.%...G.
-0005ea60: 3ea5 b143 8c4f 265d 9128 9cad 08b7 b911  >..C.O&].(......
-0005ea70: e50c 4411 f565 8d48 366e 4e74 6590 8fe8  ..D..e.H6nNte...
-0005ea80: 8e7b 34e3 408b 950a 4b34 28fe 41cf bec2  .{4.@...K4(.A...
-0005ea90: 98fb 4a6a a194 e419 b334 1bd1 d273 6f94  ..Jj.....4...so.
-0005eaa0: ba69 d1ab e567 71bd 621a 243e 25ed 8df5  .i...gq.b.$>%...
-0005eab0: 793d a618 bace c44f c856 e8f5 7bd1 b357  y=.....O.V..{..W
-0005eac0: 089e def1 2325 6afc ab59 bbb6 1f27 739e  ....#%j..Y...'s.
-0005ead0: d65d 320b d24e a719 ac91 e951 b51e 2175  .]2..N.....Q..!u
-0005eae0: 6920 052c 5cb8 a9ab bb0a e639 243a cee1  i .,\......9$:..
-0005eaf0: 22f9 9aa1 1b9a 6976 1a1e a445 61e2 133a  ".....iv...Ea..:
-0005eb00: 7427 74c4 6033 d2b3 a784 b830 d9a4 7a01  t't.`3.....0..z.
-0005eb10: 7227 d915 4932 db30 d812 2864 5c4f ad12  r'..I2.0..(d\O..
-0005eb20: 46e3 2265 5732 c989 47d1 607a ffd4 4b11  F."eW2..G.`z..K.
-0005eb30: c693 d486 4c40 cd13 4fb6 1a1f 44be 7d4c  ....L@..O...D.}L
-0005eb40: eb0e 4c27 9109 0761 e0a1 f2e4 b2c0 eb6c  ..L'...a.......l
-0005eb50: 9aad 974a 8b2f 0ecc a7b8 0852 b5ca 6a5e  ...J./.....R..j^
-0005eb60: 1105 ed13 65c6 814c 93a3 8909 554a b2e8  ....e..L....UJ..
-0005eb70: 393b e934 b61e 8fd5 a6e8 4c43 a20f bbb8  9;.4......LC....
-0005eb80: 13ca 0330 606b ed9c 422a d496 c286 9b22  ...0`k..B*....."
-0005eb90: 542f 6b99 d110 10d9 5b96 d2bd d25b 1586  T/k.....[....[..
-0005eba0: 4e20 83b9 2d55 1220 a5a1 0cd9 ba34 376a  N ..-U. .....47j
-0005ebb0: 7e56 7525 2eb7 749b 4a0d 8e58 a49a 8ef9  ~Vu%..t.J..X....
-0005ebc0: 2f6c 5853 e311 63be 199c d6e0 887d d84e  /lXS..c......}.N
-0005ebd0: b332 3b61 011d cafc 3e42 9d23 4824 8adc  .2;a....>B.#H$..
-0005ebe0: cf0c dbb8 d30d 1291 ea98 4ef3 cfd3 c39a  ..........N.....
-0005ebf0: 6747 be68 1e4d 2c0d 1345 d0c5 73b2 b144  gG.h.M,..E..s..D
-0005ec00: 72bb 4a82 4b32 f1e9 1d98 d09c 32a1 ca3e  r.J.K2......2..>
-0005ec10: ac9f 0906 9af0 ada4 7e5a 2734 c269 f05e  ........~Z'4.i.^
-0005ec20: 9367 f056 9d8d 207d d9ac a335 8c0c 2686  .g.V.. }...5..&.
-0005ec30: af5a 4ddf 3e7b 9024 a980 c346 ac4d bfe0  .ZM.>{.$...F.M..
-0005ec40: 1225 db4f 26eb f0d8 27cd 2a40 6a95 1e6f  .%.O&...'.*@j..o
-0005ec50: c41a 26a4 768a 37d3 859d 044d c9ed 2aa5  ..&.v.7....M..*.
-0005ec60: a470 4c1d ec51 ffe4 383f 0d8c a06b 8bed  .pL..Q..8?...k..
-0005ec70: a473 f0e0 456a 1302 e4b3 ccb9 6470 0b88  .s..Ej......dp..
-0005ec80: 26b3 a7cb a133 538b c404 b310 a14e 7d4c  &....3S......N}L
-0005ec90: 0fea 6b44 2a6c 72a1 a404 4eb8 d2f5 06c5  ..kD*lr...N.....
-0005eca0: ed1f e3c2 96ae 0b55 ab51 50da 6a8b 45d9  .......U.QP.j.E.
-0005ecb0: ce08 c7ce aef9 ea3b f33c e2c9 5568 2ff5  .......;.<..Uh/.
-0005ecc0: a72c 5f3c 1c35 4390 5f42 9e37 86e7 cdb2  .,_<.5C._B.7....
-0005ecd0: 4e84 a06f 5ccf 48c1 dbb9 5a09 ef99 ada3  N..o\.H...Z.....
-0005ece0: 28ef 5147 0d66 2c4a 9e7f c774 0edd 967d  (.QG.f,J...t...}
-0005ecf0: 397d 1ddb de79 5dbd e90a 223e 7f31 2df5  9}...y]...">.1-.
-0005ed00: 0e16 878e ecf2 43f4 6f14 9e19 188d 262f  ......C.o.....&/
-0005ed10: 7ddb df09 92a3 9d0d 09a2 3f4d a075 e376  }.........?M.u.v
-0005ed20: b684 04ce afc1 d02d 80a7 0ce8 1556 911e  .......-.....V..
-0005ed30: 1eb8 e225 5960 7d2a 9424 8426 9ac4 2ce5  ...%Y`}*.$.&..,.
-0005ed40: 5ab4 14b0 1247 df71 285b e0b1 10b3 7b8a  Z....G.q([....{.
-0005ed50: aa96 9851 a206 6248 7058 a355 c7cf d19d  ...Q..bHpX.U....
-0005ed60: 124d 6e93 51aa 7be7 9a39 b20a 6dca 8f86  .Mn.Q.{..9..m...
-0005ed70: 0c7d 60a2 7d8e 2dcb 041f f919 436c d42f  .}`.}.-.....Cl./
-0005ed80: 4b4a daa8 c4b9 5b23 d28c 016a fb77 4b4a  KJ....[#...j.wKJ
-0005ed90: c2c5 d193 bb86 a694 d276 513a 5593 848e  .........vQ:U...
-0005eda0: d74e 1f0b 5ca6 b643 8994 d769 f476 40c9  .N..\..C...i.v@.
-0005edb0: 1d23 b30b 52f5 46d5 5673 9bc0 cc26 b729  .#..R.F.Vs...&.)
-0005edc0: b0f1 c112 7212 9a18 d86d 221b 6577 3295  ....r....m".ew2.
-0005edd0: db54 d2c8 5889 7693 3ad7 a46e b32c 6ed8  .T..X.v.:..n.,n.
-0005ede0: 3551 da54 d2d8 8008 4d75 e532 a156 2096  5Q.T....Mu.2.V .
-0005edf0: a877 6eef b60a d330 8824 abd5 2ac9 42e1  .wn....0.$..*.B.
-0005ee00: 9a52 7527 73a2 9155 860f efd4 7549 64a1  .Ru's..U....uId.
-0005ee10: 78c2 b8ef 3cd4 7854 7256 431a 1337 8213  x...<.xTrVC..7..
-0005ee20: d3a4 70ba 3448 abef 5233 0d65 5172 56df  ..p.4H..R3.eQrV.
-0005ee30: 5504 208c 2568 59c2 1b30 102b f814 319d  U. .%hY..0.+..1.
-0005ee40: b75a c0de 602f c2e5 b044 35ec 7562 b615  .Z..`/...D5.ub..
-0005ee50: 1881 5059 a802 5c22 eb0f 3a35 da08 a8d3  ..PY..\"..:5....
-0005ee60: 1bc4 756a 4f44 29a3 2c01 b768 a50a 322c  ..ujOD).,..h..2,
-0005ee70: c1d1 741e aa7a 0ba5 ee94 0145 943f aa48  ..t..z.....E.?.H
-0005ee80: 63b8 494c 39bb abbe 5c55 420d 553c f68c  c.IL9...\UB.U<..
-0005ee90: ae9a 6988 4fcc 8e5e 20b7 6bab e742 113e  ..i.O..^ .k..B.>
-0005eea0: 3b76 ab55 c146 8010 ac92 edc2 a15b e0f3  ;v.U.F.......[..
-0005eeb0: 4aa7 db68 756c 0079 9471 9317 ca36 60bd  J..hul.y.q...6`.
-0005eec0: f126 35f1 5b5a 5dbd f047 da4c fbe4 5741  .&5.[Z]..G.L..WA
-0005eed0: c095 8a85 543c 7a8d ba45 7f6f 111d 2f55  ....T<z..E.o../U
-0005eee0: b846 199c b4bf bb46 17df 8250 01e9 2a2d  .F.....F...P..*-
-0005eef0: d783 c6a6 93bb 2ff1 bc97 f502 8c83 c82a  ....../........*
-0005ef00: 93c4 e938 2dab 63a3 7e93 ba53 d6b3 0695  ...8-.c.~..S....
-0005ef10: 41a5 5d25 9e55 88b4 8c3f c485 ecc5 d5e4  A.]%.U...?......
-0005ef20: 7db4 ec9c 140e 45da 6e6e 5a19 9650 662c  }.....E.nnZ..Pf,
-0005ef30: b70e 1b5e 1319 bdd7 e29e 3858 6dd5 e874  ...^......8Xm..t
-0005ef40: 77e9 2b2d ac04 061d f4be 86f8 9e19 52d8  w.+-..........R.
-0005ef50: 1253 305f ebe8 c184 f873 25e1 f4b3 37a4  .S0_.....s%...7.
-0005ef60: 0bc4 927a 3a47 485b 59d6 d531 ea94 178b  ...z:GH[Y..1....
-0005ef70: 35ff 63b5 7945 4662 5204 5a22 7592 548c  5.c.yEFbR.Z"u.T.
-0005ef80: efe0 c223 9514 ddf4 8435 4727 574a 54e7  ...#.....5G'WJT.
-0005ef90: ecda 036e dcaf 895a fd8a 4f07 02d2 4d5c  ...n...Z..O...M\
-0005efa0: f26a 60b7 9666 5a37 13ad 1db7 af48 2377  .j`..fZ7.....H#w
-0005efb0: c523 2b61 ef6b c92b 619b 8fa6 0810 96dc  .#+a.k.+a.......
-0005efc0: 65bf f906 4c24 db5e 6007 00d4 e0f9 dd99  e...L$.^`.......
-0005efd0: 7a6d b0c2 ce11 4280 fd49 865d 343a 4bf5  zm....B..I.]4:K.
-0005efe0: 0fe5 d625 0127 6697 dc50 6a50 20b1 5f8d  ...%.'f..PjP ._.
-0005eff0: 59db be9c 6379 1a6b 2dd7 cb8a b846 edd8  Y...cy.k-....F..
-0005f000: 6403 a2e4 7558 bbb5 b424 2533 cf84 57b4  d...uX...$%3..W.
-0005f010: 94ac 2890 d474 5295 6757 8cd2 a0cc 5222  ..(..tR.gW....R"
-0005f020: 8e56 add0 7bc4 c610 bc3b a9df 0c8b 621c  .V..{....;....b.
-0005f030: 3206 56d9 d1b4 7a07 d772 a750 b47a 82d2  2.V...z..r.P.z..
-0005f040: 1dea 6f8c 6905 9ad0 2e76 c669 c9e6 a6ca  ..o.i....v.i....
-0005f050: 13ad 2941 6d1d 94e7 2155 3a4d 3c9b 8f9a  ..)Am...!U:M<...
-0005f060: aaea ab9c ed23 357a 5668 70a9 4774 2382  .....#5zVhp.Gt#.
-0005f070: aac8 a2f6 c4a3 4fd0 31c4 6355 d365 360d  ......O.1.cU.e6.
-0005f080: 889d a1b4 b730 f91f 03fd b4ce 0fc9 27b8  .....0........'.
-0005f090: bb7c 0d0b 5c77 aa43 34b8 b871 b1d4 9728  .|..\w.C4..q...(
-0005f0a0: 5ba6 fb84 00cd 2584 1327 b3d4 07cc 787a  [.....%..'....xz
-0005f0b0: 7d34 e8e2 46cf 741a 4d60 7b24 715d 162e  }4..F.t.M`{$q]..
-0005f0c0: 01f4 972d db24 5495 8828 50d1 2556 3a57  ...-.$T..(P.%V:W
-0005f0d0: f350 b1aa d515 ea6c 3e57 678f 4e46 d8d9  .P.....l>Wg.NF..
-0005f0e0: 31d2 3b97 a36f 9405 c83e 760b 110d 55c3  1.;..o...>v...U.
-0005f0f0: 1002 1ac4 153a a7b0 e7df 4e17 25e8 026a  .....:....N.%..j
-0005f100: 534c 6e97 bea7 c58b 4700 0a8d 59df 84d4  SLn.....G...Y...
-0005f110: 4c9e 2f23 8d49 5abb 72fe c449 3f27 eb43  L./#.IZ.r..I?'.C
-0005f120: 007a 0978 a133 b78e 1406 90d8 ad6b 6b32  .z.x.3.......kk2
-0005f130: b8ba 51c5 1b61 2dd8 e35d 4ae3 74a2 9170  ..Q..a-..]J.t..p
-0005f140: 2ede 70f2 93d1 2e13 adf3 f6bb 3621 4198  ..p.........6!A.
-0005f150: a304 d70b e048 8215 3528 5f05 d723 f651  .....H..5(_..#.Q
-0005f160: a075 92c0 c68a aeaf 9ac3 4b8f 51f9 7bf6  .u........K.Q.{.
-0005f170: a479 8a0d f231 4a94 e635 b1f7 6b79 318f  .y...1J..5..ky1.
-0005f180: 9d52 ad5e 4f9c b620 f75a bd54 06d2 a1c1  .R.^O.. .Z.T....
-0005f190: 6089 9853 c8b4 8082 6169 bca3 57be 374d  `..S....ai..W.7M
-0005f1a0: 6c9b 05b3 84af ab15 ecff ba89 51df 8278  l...........Q..x
-0005f1b0: af79 2933 4e2d 43fe 1eb1 9298 da4b c1a7  .y)3N-C......K..
-0005f1c0: 548a 3a12 5bcf 936a 988d 88a2 7f83 35bd  T.:.[..j......5.
-0005f1d0: 8649 93a7 bf12 bfad 4a35 c7b6 4665 2be5  .I......J5..Fe+.
-0005f1e0: 9b93 58fe 0926 56e2 5d2f fcc5 e3fb 860f  ..X..&V.]/......
-0005f1f0: 4d27 c037 cd64 ce51 f49a 8beb 0278 797e  M'.7.d.Q.....xy~
-0005f200: 7e16 7675 1ec7 af6b 938c 1023 03f1 8211  ~.vu...k...#....
-0005f210: 8e90 9efb 0cea 29eb ba82 2c8d 0895 2757  ......)...,...'W
-0005f220: 60db d0bb 28c2 1dc5 28c7 7536 4f43 8492  `...(...(.u6OC..
-0005f230: 25a1 5b5a f908 70b6 f348 9c56 3ce1 92b4  %.[Z..p..H.V<...
-0005f240: 6718 fd70 abbe 8a09 740c 064d 5d64 13ee  g..p....t..M]d..
-0005f250: c61d 53bb ae8e 36d5 6457 b30a 2811 1aac  ..S...6.dW..(...
-0005f260: 2a4c 7a00 593e c6ca 0d07 1a66 254b b611  *Lz.Y>.....f%K..
-0005f270: 3cfd 966d b29b 9748 25d9 ee55 a74d a27a  <..m...H%..U.M.z
-0005f280: c545 e626 4cdb 860e b62e e3ce 7918 0234  .E.&L.......y..4
-0005f290: 79ab 4a22 fb98 b80e 7a19 342e 551b d06e  y.J"....z.4.U..n
-0005f2a0: fe0e ddcc ad3f b7b0 fc5d 6d8a 3a85 339e  .....?...]m.:.3.
-0005f2b0: 52b1 1519 e854 2a2e 8963 9acb 27af 11c3  R....T*..c..'...
-0005f2c0: c7d9 9e12 c233 9698 021d 7a23 ce86 7aa3  .....3....z#..z.
-0005f2d0: 5934 2b92 f47c c564 3441 7a55 6567 1990  Y4+..|.d4AzUeg..
-0005f2e0: 64e2 6025 b7a3 ab65 1c09 4df8 0a35 8b9b  d.`%...e..M..5..
-0005f2f0: 85a8 ea28 8aca fe62 f82e 9935 4430 a7aa  ...(...b...5D0..
-0005f300: 7e85 0409 18b2 0b5c 04ee f227 30d1 6acd  ~......\...'0.j.
-0005f310: e718 6110 8999 ee5d ed84 fe40 6b28 c664  ..a....]...@k(.d
-0005f320: 8e77 8dca 0ca4 2245 e1dc 02d6 aae4 0c1a  .w...."E........
-0005f330: bd8f 0f68 a0e8 3277 7afb e905 9858 f408  ...h..2wz....X..
-0005f340: b4bb 3e1e 2f2a dbd7 f259 3b86 d749 459e  ..>./*...Y;..IE.
-0005f350: 098c 5bd6 d96c 960c c4ce 05c2 4b1e c86f  ..[..l......K..o
-0005f360: 4166 6a22 9625 8152 9a91 82c0 a1f4 5e3b  Afj".%.R......^;
-0005f370: 5b95 5323 ff0b 1041 dec3 23cb f629 6546  [.S#...A..#..)eF
-0005f380: 9b56 7120 f33e b4fb 9508 4ab7 894b a981  .Vq .>....J..K..
-0005f390: e891 b1a0 769a 0049 3a65 9708 3134 baf0  ....v..I:e..14..
-0005f3a0: ee6c 1392 2f30 5c15 8c9e 4e0c d444 5c46  .l../0\...N..D\F
-0005f3b0: 78b2 b290 214c a601 94a1 8591 90e4 369d  x...!L........6.
-0005f3c0: 5967 5394 3d19 4258 2698 a93c 79e0 1773  YgS.=.BX&..<y..s
-0005f3d0: 3ad5 a9ac dae8 ac41 8d69 5999 5bfc 8c05  :......A.iY.[...
-0005f3e0: 5889 b891 d265 c547 4469 8918 64f6 9697  X....e.GDi..d...
-0005f3f0: 6d33 86a3 d932 4798 7087 44fa ab7a cd6b  m3...2G.p.D..z.k
-0005f400: 6c2d 94e6 2668 5e9f 49f3 bd43 1b35 d089  l-..&h^.I..C.5..
-0005f410: e6b5 23a8 44e2 c2a6 a576 cd9d 064e 20d3  ..#.D....v...N .
-0005f420: d809 9218 eee6 4501 af88 630e 9d23 8ca2  ......E...c..#..
-0005f430: c454 3a40 ce3c 6479 613a 36ac 77e9 986d  .T:@.<dya:6.w..m
-0005f440: 8a0c 8a78 1d8f 7d0e 6e98 509e 6d26 8c72  ...x..}.n.P.m&.r
-0005f450: d2e8 0135 4630 39a5 85de 6334 0331 ed75  ...5F09...c4.1.u
-0005f460: 5aee 9114 499d dd09 0ef6 bd7d 32b8 2250  Z...I......}2."P
-0005f470: e756 754e 075e f828 4c8a 47f6 c05b 6267  .VuN.^.(L.G..[bg
-0005f480: b59e 1cd6 7b1d 95c0 444f 7660 68c8 06c8  ....{...DOv`h...
-0005f490: 2618 5cb8 8da6 2eb0 e132 d335 37ec d173  &.\......2.57..s
-0005f4a0: 441a 9ba3 552a d2ef ad8a 6344 4bc4 970e  D...U*....cDK...
-0005f4b0: 34be 0287 3d2b 1ee3 4e97 f30c 8cb8 5357  4...=+..N.....SW
-0005f4c0: e6dd 7a40 e576 99ae 777b 8dc5 9878 079b  ..z@.v..w{...x..
-0005f4d0: 3bb5 86d8 c3b5 4147 8d44 a5e9 7783 5550  ;.....AG.D..w.UP
-0005f4e0: 24a2 3446 50f4 46c8 1ae1 43a4 b650 5e37  $.4FP.F...C..P^7
-0005f4f0: 138f 3e43 516f 0a9a d2a1 3a88 7f09 7e76  ..>CQo....:...~v
-0005f500: d811 adad bd48 77df 07d0 434b b313 6ccb  .....Hw...CK..l.
-0005f510: e3a1 a871 be5a 718a 57de 5506 1248 55f9  ...q.Zq.W.U..HU.
-0005f520: f7b4 8d93 a9b3 e252 d962 da6a f89c a655  .......R.b.j...U
-0005f530: 35f1 e873 332f 9c41 848f 10cc bcaa 42e7  5..s3/.A......B.
-0005f540: 366d 0288 964a a0a8 3f59 2d8e daab d1a4  6m...J..?Y-.....
-0005f550: f9bc 611f ec88 7a75 b3e1 e133 5cb9 22e6  ..a...zu...3\.".
-0005f560: acc1 82a7 2092 5996 47de d759 a0f1 94d8  .... .Y.G..Y....
-0005f570: 6bbd 1706 d55b b7f9 e224 ea26 6d7b 446f  k....[...$.&m{Do
-0005f580: 2933 8558 f673 772d e60a 7aeb fbea 7d9f  )3.X.sw-..z...}.
-0005f590: 0c5a 8034 e8e9 f3ef 5854 df29 5d01 ba97  .Z.4....XT.)]...
-0005f5a0: 9f25 f8cc ebe7 54ac f56a ba3a 89bf 6d7c  .%....T..j.:..m|
-0005f5b0: f72f ffe4 6ceb 097f bc37 7f6d 16e6 e0d7  ./..l....7.m....
-0005f5c0: 175a a48d c3b8 ab2a ab2d 16ff 762d 58a3  .Z.....*.-..v-X.
-0005f5d0: d4ac 40ff bff5 e4c9 1fdf 522b 80bf 7fdd  ..@.......R+....
-0005f5e0: 11ff 8d27 59c5 ad5b adaf dcf8 fc77 beb0  ...'Y..[.....w..
-0005f5f0: 6a05 ee5b f24e 2eb5 4dfe f185 9a39 b156  j..[.N..M....9.V
-0005f600: 570a 56b9 379f b7d3 f1ba d5b9 ed95 ee8f  W.V.7...........
-0005f610: 3b9d f4e6 12fe 4b8b 37de dd3b e7a9 e9cd  ;.....K.7..;....
-0005f620: 10df 4a7e eafd 7cd6 97df 9cf9 fdb5 7f5f  ..J~..|........_
-0005f630: daf3 80c3 0810 0200 0000 4363 3033 0000  ..........Cc03..
+0005e0e0: 5f7c c517 7cf1 46fb d191 3568 9adb f1e0  _|..|.F...5h....
+0005e0f0: 53e3 8b07 0ddf 0fe0 bf7f 9360 8c46 3f9c  S..........`.F?.
+0005e100: e653 f693 c517 7cf1 175f f1c5 5f7c c517  .S....|.._.._|..
+0005e110: 7cf1 175f f1c5 fc7c 84a6 68fb 9207 14a2  |.._...|..h.....
+0005e120: 28d8 0823 83c8 c1ed 00fe c34d 4038 f354  (..#.......M@8.T
+0005e130: 9061 12bb 2815 602b 3cd4 3054 06a8 f853  .a..(.`+<.0T...S
+0005e140: 74ac 9861 257b 1119 16cc 0a87 3790 0e76  t..a%{......7..v
+0005e150: b05b 6abe f3d9 0381 107f a003 1e1e dc18  .[j.............
+0005e160: 501d 0f50 6485 7535 d0f9 2d78 17d8 3a8d  P..Pd.u5..-x..:.
+0005e170: adbd 440d 0e36 1541 158c a001 aeb0 a1b1  ..D..6.A........
+0005e180: e433 3522 0387 ac81 7ebf 5a48 a219 5ce0  .35"....~.ZH..\.
+0005e190: a480 62a3 6c3b 42e7 109c 231b 44c4 874c  ..b.l;B...#.D..L
+0005e1a0: de07 1d28 10cd ba7c b6c7 2f94 f294 896f  ...(...|../....o
+0005e1b0: 37c1 a0e8 84d9 4206 e582 1603 a409 7505  7.....B.......u.
+0005e1c0: a00c 1e27 9c8b f21a 8b04 2e78 dce0 e30e  ...'.......x....
+0005e1d0: 2485 af33 8492 2218 8c1a b386 097e c966  $..3.."......~.f
+0005e1e0: 3180 0a1f 3a5c ca30 160f 148c ffbe 0b7f  1...:\.0........
+0005e1f0: 2d23 f901 acf8 d341 6a83 ac00 7581 8806  -#.....Aj...u...
+0005e200: b7c0 c160 e005 ad70 8c81 9207 a742 88a1  ...`...p.....B..
+0005e210: 44e6 a344 78e8 8922 2a9d 1834 a43b 5e09  D..Dx.."*..4.;^.
+0005e220: 843f 70c8 9112 6a09 3736 dd0e ae81 beff  .?p...j.76......
+0005e230: 3810 1928 28b4 5fc4 c886 0c85 f093 20da  8..((._....... .
+0005e240: 4249 1b7e 06bc afd2 1ec3 35c1 864c 64c0  BI.~......5..Ld.
+0005e250: 6253 d1bb 92a1 bc81 f0b3 e0c9 78a2 802b  bS..........x..+
+0005e260: 4250 c1d7 9003 e0d4 1c44 c02b c156 769f  BP.......D.+.Vv.
+0005e270: 740b 5a22 0e01 081e cbe6 27b0 a143 2436  t.Z"......'..C$6
+0005e280: 088d 3f34 4026 400c 4130 81c2 2eb3 c80d  ..?4@&@.A0......
+0005e290: a922 9f86 e0f8 aba0 1e43 1ac3 06eb 4206  .".......C....B.
+0005e2a0: 6a42 bf87 580b c1c9 83ac c08b 0650 876b  jB..X........P.k
+0005e2b0: 0d85 d414 9706 a1e0 d5b4 103c 31bc 2bc4  ...........<1.+.
+0005e2c0: 96e0 2b80 5da0 8041 3aa4 e210 2370 6112  ..+.]..A:...#pa.
+0005e2d0: 841d 1114 042d 639e 9307 a058 424c fe14  .....-c....XBL..
+0005e2e0: 2646 1068 e0e1 02c7 0023 0ec9 8884 a801  &F.h.....#......
+0005e2f0: c205 527e c206 1ed1 43bb ed82 2302 b3c0  ..R~....C...#...
+0005e300: 06bf 64c3 2c90 e810 025f a264 3820 0057  ..d.,...._.d8 .W
+0005e310: 0d96 8798 9083 814d 90a8 06af f0c9 9626  .......M.......&
+0005e320: 4415 0c69 0e24 4287 4017 1c25 326a aa08  D..i.$B.@..%2j..
+0005e330: 4b83 9201 120e 01e0 6780 2a1c 4ee0 1a03  K.......g.*.N...
+0005e340: fc7a c032 ef38 c0c2 400a bb99 880c 4862  .z.2.8..@.....Hb
+0005e350: 5e3e bf7f 7085 f95c 50d0 9856 2701 4304  ^>..p..\P..V'.C.
+0005e360: 58f1 8401 ca17 cc8a a832 9525 83dd 5865  X........2.%..Xe
+0005e370: 871c 80f9 750d 6700 81ca 6bb8 3a48 a3c3  ....u.g...k.:H..
+0005e380: 0c28 85e0 8ee1 d6a0 471b ebe0 1e03 e40a  .(......G.......
+0005e390: 6ac5 8b82 5030 30f8 4942 eddb 1ee2 2609  j...P00.IB....&.
+0005e3a0: 08c9 1036 3815 6026 bfc5 6c0c 2642 af20  ...68.`&..l.&B. 
+0005e3b0: 30e6 1a70 0ade d48f 1108 044e 28ff 6385  0..p.......N(.c.
+0005e3c0: 6065 9e1b c2d7 08ca 60f0 37c6 0458 f089  `e......`.7..X..
+0005e3d0: 0541 681d 0e38 d215 2712 ac20 c183 d740  .Ah..8..'.. ...@
+0005e3e0: 6ed0 2b28 6238 b1c0 5151 8411 96c1 9081  n.+(b8..QQ......
+0005e3f0: 3a60 2538 1b20 0936 df68 3a58 4ba8 21ca  :`%8. .6.h:XK.!.
+0005e400: eb27 5471 6177 d3bc 27b0 0aa1 048f f014  .'Tqaw..'.......
+0005e410: 43ce 44c1 806c f823 6066 c468 0b66 e120  C.D..l.#`f.h.f. 
+0005e420: 25d8 9e31 5d21 dd79 d9e7 b1e1 80c4 61a8  %..1]!.y......a.
+0005e430: 064e b5f7 b371 ec60 2a7a 0054 83ae c096  .N...q.`*z.T....
+0005e440: a7c9 4c50 2a28 5b78 8a81 141c 4d33 7621  ..LP*([x....M3v!
+0005e450: f62a 3436 0f17 6085 4007 3c32 385b 816b  .*46..`.@.<28[.k
+0005e460: af50 0495 7720 8e80 5658 4980 428d 0427  .P..w ..VXI.B..'
+0005e470: d109 b2c3 5e3e bff1 c886 4810 09f2 3838  ....^>....H...88
+0005e480: 346b 105c 0b88 358d 3642 ff2b 84da 4008  4k.\..5.6B.+..@.
+0005e490: 8807 6774 6c01 c16b 5d11 02e0 3620 700c  ..gtl..k]...6 p.
+0005e4a0: 6835 8f04 51b0 1225 69f8 eadb 6c60 c1ec  h5..Q..%i...l`..
+0005e4b0: 7f8f 6309 0077 bfd1 f403 a078 a120 ec3b  ..c..w.....x. .;
+0005e4c0: 4414 b802 e509 4805 1380 4b40 81df 3e70  D.....H...K@..>p
+0005e4d0: c18d 1662 1aec 4de8 bb8d 9f80 2702 e980  ...b..M.....'...
+0005e4e0: 5ce8 141b 8981 72f9 2c10 d240 aefc a832  \.....r.,..@...2
+0005e4f0: 4325 80c1 55d9 060a 2ce0 04c2 1ad0 8a09  C%..U...,.......
+0005e500: 6bc4 06a4 b637 5840 8204 da42 81e0 1384  k....7X@...B....
+0005e510: 0bc7 0e76 2c94 e810 c7b3 de0d 1b22 6af8  ...v,........"j.
+0005e520: 080b f931 3644 690d 610d aef8 7601 c706  ...16Di.a...v...
+0005e530: 20b7 81c2 0164 065e 82c8 ec8e 9316 a209   ....d.^........
+0005e540: cf04 470c 680d f037 9850 7934 1f0c 0694  ..G.h..7.Py4....
+0005e550: 0295 1c1c 8d29 0639 d8a3 2370 23c3 84c8  .....).9..#p#...
+0005e560: 2d18 3005 df1a 8d8c 0258 d6ef 98b1 bbc1  -.0......X......
+0005e570: 7861 910b d7b1 1b70 af43 9706 10e7 77c8  xa.....p.C....w.
+0005e580: 05e4 0d74 3818 8341 77c8 18df a7b0 42e9  ...t8..Aw.....B.
+0005e590: c722 9022 bf27 9d0d 79d8 08fd ba42 62c3  .".".'..y....Bb.
+0005e5a0: 0adc 101c 4024 c084 7e75 364d 414e a044  ....@$..~u6MAN.D
+0005e5b0: 20aa 03a6 d59e b402 6f0d 806b 0bc8 4525   .......o..k..E%
+0005e5c0: 05b0 19ec e0b7 18cc a3a0 827d b301 ac20  ...........}... 
+0005e5d0: dcf6 501a 2476 502e 470a 5f44 a3fe f811  ..P.$vP.G._D....
+0005e5e0: 21ac d4b0 c181 d200 0008 7cde b02e 7969  !.........|...yi
+0005e5f0: c0b2 5444 3829 1094 6cce 4d12 822b a067  ..TD8)..l.M..+.g
+0005e600: 3100 2c90 5a3c 5c00 8201 150c 0283 2f0e  1.,.Z<\......./.
+0005e610: e16b 068f c0bd 0763 6730 33d8 b086 652d  .k.....cg03...e-
+0005e620: 6f85 3788 04b5 c0fd 8848 f805 0f19 6ac5  o.7......H....j.
+0005e630: 0881 e0d1 f620 956c 6306 366e d330 4ea0  ..... .lc.6n.0N.
+0005e640: e1e0 6ad8 3a58 8e3d 0894 0ab8 f070 3643  ..j.:X.=.....p6C
+0005e650: 8231 e049 41a9 0775 d87d 064f 2ec0 43f7  .1.IA..u.}.O..C.
+0005e660: 1007 dc56 7005 41ee 3072 002b 221e a008  ...Vp.A.0r.+"...
+0005e670: 0681 0011 82c2 08d2 71b6 0d92 220e 412b  ........q...".A+
+0005e680: 89a9 fdb0 aced 4028 bbe1 d018 0558 4292  ......@(.....XB.
+0005e690: 03e7 04a7 b747 b670 4902 4941 444a 83bf  .....G.pI.IADJ..
+0005e6a0: c15e 6c10 2778 e1c3 6d2c 2f10 c1c1 b571  .^l.'x..m,/....q
+0005e6b0: 90c0 573c a028 c11c f010 3055 81ec 7ec3  ..W<.(....0U..~.
+0005e6c0: 6014 a28f 699d 0b06 5c20 a7d8 30e8 500d  `...i...\ ..0.P.
+0005e6d0: b20b f003 40dd 4326 7ee1 320a 40e1 2d2c  ....@.C&~.2.@.-,
+0005e6e0: 2ed8 b440 7653 0620 1e8c d061 37d8 0562  ...@vS. ...a7..b
+0005e6f0: 458f 47d6 e23e 9cfb 0683 1098 f63b f7e9  E.G..>.......;..
+0005e700: e082 8427 5b69 0782 6123 824e 0821 bc22  ...'[i..a#.N.!."
+0005e710: 280d c805 2c30 2296 ca90 f030 1947 2e74  (...,0"....0.G.t
+0005e720: e0d0 194c 1c94 0263 05a8 bffb e527 3620  ...L...c.....'6 
+0005e730: 174c 61f7 1e68 8841 a680 1941 ed18 7888  .La..h.A...A..x.
+0005e740: 6163 1ab1 7d06 7c82 e96f 5a9d 0287 7424  ac..}.|..oZ...t$
+0005e750: e244 7267 d77d b2c1 0e7c 3be8 81f8 3013  .Drg.}...|;...0.
+0005e760: d83f 3517 064c 0164 9073 9280 1e09 ee18  .?5..L.d.s......
+0005e770: d012 70ce 4a40 0541 9a06 d061 04a9 400b  ..p.J@.A...a..@.
+0005e780: 704b 0211 0a9a 69ef ca66 3398 150f 187e  pK....i..f3....~
+0005e790: b014 1ea3 c00a e10b 5dc0 880e c410 e40e  ........].......
+0005e7a0: a345 2c1b 8760 69f7 5c03 7d41 f801 f06b  .E,..`i.\.}A...k
+0005e7b0: 2030 0dbf 0b89 033a d9f0 7410 fc22 6836   0.....:..t.."h6
+0005e7c0: 8715 e00a 810e 7b98 c3b5 a923 6d05 72d8  ......{....#m.r.
+0005e7d0: 7007 1e4e c02b 880f 2875 feb6 1122 035c  p..N.+..(u...".\
+0005e7e0: 8524 0b6a 6b90 8b1f 4448 8145 6f0c e668  .$.jk...DH.Eo..h
+0005e7f0: 38c9 6e37 6002 404c 51c9 0254 0f7a 613f  8.n7`.@LQ..T.za?
+0005e800: 0ac2 e12e fa60 0d90 0646 fcdd 0c2d 16b2  .....`...F...-..
+0005e810: 3078 8175 2018 7e54 3532 1970 9a3f 5903  0x.u .~T52.p.?Y.
+0005e820: 2501 94f8 4c78 cf30 f010 05bc 0fbc 0aca  %...Lx.0........
+0005e830: 17da 77b0 c4f0 5883 32c0 e2fc 1036 7e1e  ..w...X.2....6~.
+0005e840: 20ec 786c 7663 931b ce7d 6783 30a1 d26c   .xlvc...}g.0..l
+0005e850: fa88 f67e 7c37 6308 86df db3c 7d54 4c83  ...~|7c....<}TL.
+0005e860: 164e b510 dc93 6008 8076 bb97 3014 838f  .N....`..v..0...
+0005e870: 5151 cd55 7092 834d 0106 80a6 18f1 ce16  QQ.Up..M........
+0005e880: f013 d848 0534 1420 79cb 4258 6806 5014  ...H.4. y.BXh.P.
+0005e890: 6b45 5005 0f1d 688c 8654 adfd 707e 402b  kEP...h..T..p~@+
+0005e8a0: e8e9 435c e262 840b 8d1f 208d 1a8e bbf1  ..C\.b.... .....
+0005e8b0: b310 50ff 4888 83d3 f303 a419 9112 4128  ..P.H.........A(
+0005e8c0: 39c3 10a9 6163 d4f0 db34 83bf f006 1956  9...ac...4.....V
+0005e8d0: ec6b 0c30 14c2 f23f 6a0d 4402 911f b222  .k.0...?j.D...."
+0005e8e0: 669a fc2a 2036 c3a0 c69e 85c9 05e1 67f8  f..* 6........g.
+0005e8f0: 6670 fc24 0c32 960e 9ad7 9434 070c 03fb  fp.$.2.....4....
+0005e900: 2053 264d 9c2d 8028 bbe5 010d 0b55 db03   S&M.-.(.....U..
+0005e910: 3158 8002 71f1 cca0 4708 9fc2 faa1 3761  1X..q...G.....7a
+0005e920: f731 8380 5466 9f12 90b3 0223 900a ee60  .1..Tf.....#...`
+0005e930: b018 f44d 1116 c944 fa15 8d5a 5afe 373a  ...M...D...ZZ.7:
+0005e940: 1615 1f18 a8ae 766c f81e 0254 f986 816a  ......vl...T...j
+0005e950: 1c46 56f8 4e01 f830 0530 f1e0 e9f0 cec2  .FV.N..0.0......
+0005e960: f87a 8258 f9ec 016d 1c60 5af8 1ac3 f880  .z.X...m.`Z.....
+0005e970: 015c f1c0 baf0 7281 eed0 72e4 e543 afc0  .\....r...r..C..
+0005e980: 1248 8a96 8140 9d6d a021 d51d 29b6 9712  .H...@.m.!..)...
+0005e990: ca9a ccc0 dabc 4ae4 5a2e 29c8 6762 30db  ......J.Z.).gb0.
+0005e9a0: 9464 a2c6 2247 45b4 93b4 82b9 58da 8c8c  .d.."GE.....X...
+0005e9b0: cae5 7656 3e75 2640 3b96 2987 4917 ea70  ..vV>u&@;.).I..p
+0005e9c0: 44b1 7c75 4832 3b3b 4121 c212 607f 26fd  D.|uH2;;A!..`.&.
+0005e9d0: 750d 299f 795c 16ca fd99 4f13 9e84 7be6  u.).y\....O...{.
+0005e9e0: cab3 f048 1356 e822 7fd2 d920 4ed4 4490  ...H.V."... N.D.
+0005e9f0: cce8 02d5 e78f 50a5 97c4 27e2 1208 a341  ......P...'....A
+0005ea00: c444 321f 4057 05a1 3402 a524 158b 9418  .D2.@W..4..$....
+0005ea10: d004 4da4 589a 0de2 2a5c e288 7454 a867  ..M.X...*\..tT.g
+0005ea20: 4348 2bc4 6d01 943a ca58 f6ef 55f3 98aa  CH+.m..:.X..U...
+0005ea30: d2b8 a939 18e1 b64c a3c6 7a71 7636 0581  ...9...L..zqv6..
+0005ea40: 3b95 1eea 6733 666a 2522 4abc 8923 3b50  ;...g3fj%"J..#;P
+0005ea50: a273 1889 b3b3 5d47 de02 4b5c 65f7 8f5a  .s....]G..K\e..Z
+0005ea60: 7c4a 6287 189f 4cba 2351 395b 106e 7223  |Jb...L.#Q9[.nr#
+0005ea70: ca19 8822 eacb 1a91 6cdc 9de8 cb20 1ed1  ..."....l.... ..
+0005ea80: 1df7 69c6 8016 2a15 9768 51fc 839e 7d85  ..i...*..hQ...}.
+0005ea90: 30f7 95d4 4229 c833 6769 36a2 a5e7 de28  0...B).3gi6....(
+0005eaa0: 75d3 a257 cbcf e27a c434 497c 4bda 1aeb  u..W...z.4I|K...
+0005eab0: f27a 4d31 749d 889f 91ad d1eb f6a2 67af  .zM1t.........g.
+0005eac0: 113c bce3 474a d4f8 57b3 766d 3f4e e63c  .<..GJ..W.vm?N.<
+0005ead0: acbb 6416 a49d 4f33 5823 d2a3 6a3d 42ea  ..d...O3X#..j=B.
+0005eae0: d240 0b58 b970 5257 7615 cc73 4974 9dc3  .@.X.pRWv..sIt..
+0005eaf0: 45f2 3543 3634 d2ec 343c 498b c2c4 2674  E.5C64..4<I...&t
+0005eb00: e94e e888 c166 a567 4e09 7161 b249 f402  .N...f.gN.qa.I..
+0005eb10: e44e b22b 9264 b661 b025 50c8 b89e 5b25  .N.+.d.a.%P...[%
+0005eb20: 8cc6 44ca af64 9313 8ea2 c1f4 fea9 9722  ..D..d........."
+0005eb30: 8d27 a80d 9880 9b27 9e6c 353e 887c fa98  .'.....'.l5>.|..
+0005eb40: d61d 984e 2213 0fc2 c143 e5c9 6481 d7d9  ...N"....C..d...
+0005eb50: 345b 2e95 175f 1d98 4e71 11a4 6a95 d4bc  4[..._..Nq..j...
+0005eb60: 220a db27 ca8c 0399 2647 1213 ab94 64d1  "..'....&G....d.
+0005eb70: 7276 d269 6d3d 1fab 4cd1 9886 451f 7771  rv.im=..L...E.wq
+0005eb80: 2694 0660 c1d6 da39 8554 a92d 840d 3645  &..`...9.T.-..6E
+0005eb90: a95e d632 a321 21b2 b72c a47b a5b7 2a0c  .^.2.!!..,.{..*.
+0005eba0: 9d40 0673 5aaa 2540 4b43 18b2 7469 6ed4  .@.sZ.%@KC..tin.
+0005ebb0: fcac eb4a 5d6e e836 941a 1db1 4935 1cf3  ...J]n.6....I5..
+0005ebc0: 5ed8 b0a6 c723 c77c 3338 acc1 10fb b09d  ^....#.|38......
+0005ebd0: 6665 76c2 033a 94f9 7c84 3a47 9148 14b9  fev..:..|.:G.H..
+0005ebe0: 9f19 b671 a71b 2522 d531 9de6 9fa7 8635  ...q..%".1.....5
+0005ebf0: ce8e 7cd1 3c9a 581a 278a a18b e664 6389  ..|.<.X.'....dc.
+0005ec00: e576 9404 9764 e3d3 3b30 a139 6442 957d  .v...d..;0.9dB.}
+0005ec10: 583f 130c 35e1 5a49 fcb4 4e68 84d3 e0bd  X?..5.ZI..Nh....
+0005ec20: 26cf e1ad 3a1b 41fa b259 466b 1919 4c0c  &...:.A..YFk..L.
+0005ec30: 5fb5 9abe 7cf6 2149 5201 868d 599b 7ec1  _...|.!IR...Y.~.
+0005ec40: 244a b79f 4dd6 e1b1 4e9a 5580 d42a 3cde  $J..M...N.U..*<.
+0005ec50: 8935 4d48 ed14 6fa6 0a3b 099a 93db 544a  .5MH..o..;....TJ
+0005ec60: 48e1 983a d9a3 fec9 717e 1a18 41d7 16db  H..:....q~..A...
+0005ec70: 49e7 e0c1 8ad4 2704 c967 9873 c9e0 1710  I.....'..g.s....
+0005ec80: 4d66 4e97 4367 a616 8809 6621 429d fb98  MfN.Cg....f!B...
+0005ec90: 1ed4 d688 55d8 e442 4909 9d70 a5eb 0c8a  ....U..BI..p....
+0005eca0: db3f c785 2c5d 16aa 57a3 a1b4 d516 8ab2  .?..,]..W.......
+0005ecb0: 9d11 8f9d 5cf3 d477 e779 c493 abd0 5eea  ....\..w.y....^.
+0005ecc0: 4e59 be78 396a 8620 be84 3d6f 0dcf 9b65  NY.x9j. ..=o...e
+0005ecd0: 9c08 41df b99e 9182 b673 b512 df33 5b47  ..A......s...3[G
+0005ece0: 50de a28e 1acc 5894 3cff 8fe9 1cba 2cfb  P.....X.<.....,.
+0005ecf0: 73fa 3ab6 bdf3 ba7a d215 447c ff62 5aea  s.:....z..D|.bZ.
+0005ed00: 1d2c 0f1d d9e5 86e8 de28 3d33 301a 4d5e  .,.......(=30.M^
+0005ed10: fab6 bf13 2447 3b1b 1244 7e9a 40eb c7ed  ....$G;..D~.@...
+0005ed20: 6d09 099c 5e83 a15b 014f 18d0 2aac 233d  m...^..[.O..*.#=
+0005ed30: 3c70 c44b b2c0 fa54 2849 094d 3589 59ca  <p.K...T(I.M5.Y.
+0005ed40: b568 2860 248e bee3 51b6 c163 2166 f714  .h(`$...Q..c!f..
+0005ed50: 542d 30a3 440d c490 e0b0 47ab 8f9f a23b  T-0.D.....G....;
+0005ed60: 259a dd26 a354 f6ce 3473 6515 db94 1e0d  %..&.T..4se.....
+0005ed70: 19fa c144 fb1c 5a96 083e f233 86d8 a85f  ...D..Z..>.3..._
+0005ed80: 9794 b551 8873 b746 a419 02d4 f6ef 9794  ...Q.s.F........
+0005ed90: 858b a327 770d 4c29 a4ed a374 ab26 081d  ...'w.L)...t.&..
+0005eda0: ae9d 3f16 b84c 6d87 1229 aed3 e9ed 8092  ..?..Lm..)......
+0005edb0: 3a46 6717 a5ea 8caa ade6 3681 984d 6f53  :Fg.......6..MoS
+0005edc0: 60e3 8225 e424 3431 b0db 4436 cbee 642a  `..%.$41..D6..d*
+0005edd0: b7a9 a591 b112 ed26 74ae 48dd 6759 dcb0  .......&t.H.gY..
+0005ede0: 6aa2 b5a9 a4b1 0011 9aea ca65 43ad 402c  j..........eC.@,
+0005edf0: 51ef dcde 6c15 a661 1149 57ab 5592 84c2  Q...l..a.IW.U...
+0005ee00: 34a5 eb4e e644 22ab 0d1f dea9 eb92 c942  4..N.D"........B
+0005ee10: f184 71df 78a8 f0a8 e4ac 8634 266e 0527  ..q.x......4&n.'
+0005ee20: a749 e074 6990 56df a466 1aca a3e4 acbe  .I.ti.V..f......
+0005ee30: ab08 4018 4bd0 b284 3660 2056 f129 623a  ..@.K...6` V.)b:
+0005ee40: 6fb5 80bd c15e 84cb 6189 6ad8 eac4 6d2b  o....^..a.j...m+
+0005ee50: 3002 a0b2 5005 b844 d61f 746a b511 51a7  0...P..D..tj..Q.
+0005ee60: 3688 ead4 9f88 5246 5802 6ed1 4a15 6558  6.....RFX.n.J.eX
+0005ee70: 82a3 e83c 55f5 174a dc29 028a 287f 5591  ...<U..J.)..(.U.
+0005ee80: c670 9398 7376 567d b8aa 841a ab78 ed19  .p..svV}.....x..
+0005ee90: 5d35 d310 9e98 1dbd 416e d656 ce85 227c  ]5......An.V.."|
+0005eea0: 76ec 56ab 828d 0121 5925 da85 43b7 c1e7  v.V....!Y%..C...
+0005eeb0: 944e b6d1 ead8 00f2 28e3 262f 956d c07a  .N......(.&/.m.z
+0005eec0: e34d 6ae2 b7b4 ba7a e08f b599 f6c9 af82  .Mj....z........
+0005eed0: 812b 140b a978 f41a 748b fede 223a 5eaa  .+...x..t...":^.
+0005eee0: 718d 3338 687f 778d 2ebe 05a1 02d2 555a  q.38h.w.......UZ
+0005eef0: af07 8d4d 2777 5fe2 782f eb05 1807 9155  ...M'w_.x/.....U
+0005ef00: 2689 d371 5b56 c746 fc26 75a7 ad67 0d2a  &..q[V.F.&u..g.*
+0005ef10: 824a ba4a 3dab 1069 197f 890b d98b abc9  .J.J=..i........
+0005ef20: fb68 d839 291c 8ab4 dcdc b432 2ca1 cc58  .h.9)......2,..X
+0005ef30: 6e1d 36bc 2732 7baf c43d 71b0 daaa d1e9  n.6.'2{..=q.....
+0005ef40: eed2 565a 5809 0d3a e97d 0cf1 3d33 a4b0  ..VZX..:.}..=3..
+0005ef50: 24a6 61be d7d1 8209 f1e7 4bc2 e967 6f48  $.a.......K..goH
+0005ef60: 1688 24f5 748e 91b6 b2ac ab63 d529 2f16  ..$.t......c.)/.
+0005ef70: 6bfe c66a f28a 8cc4 a408 b544 eb24 a918  k..j.......D.$..
+0005ef80: dec1 8447 2b29 bae9 086b 8e4e af94 a9ce  ...G+)...k.N....
+0005ef90: d8b5 07dc b85f 13b5 fa15 9f0e 04a4 9ab8  ....._..........
+0005efa0: e5d5 c06e 2ccd b56e 275a 3a6e 5e91 46ee  ...n,..n'Z:n^.F.
+0005efb0: 8a47 56c2 ded7 9357 c336 1e4d 1120 2db9  .GV....W.6.M. -.
+0005efc0: ca7e f20d 9848 b6bd c10e 01a8 c1f3 ba33  .~...H.........3
+0005efd0: f5da 6085 9d23 8400 fa93 0cbb 6974 97ea  ..`..#......it..
+0005efe0: 1eca ac4b 034e cc2e b8a1 d5a0 4162 bf1a  ...K.N......Ab..
+0005eff0: b3b6 7c39 c6f2 35d6 5bae 9615 718d dab1  ..|9..5.[...q...
+0005f000: c906 44c9 ebb0 766b 6849 4b66 9f09 af68  ..D...vkhIKf...h
+0005f010: 2959 5020 a9e9 a42a cfae 19a5 4099 a444  )YP ...*....@..D
+0005f020: 1dad 5ba1 f688 8c21 7977 53bf 1816 c438  ..[....!ywS....8
+0005f030: 650c adb2 a269 f40e aee5 4ea1 69f5 05a5  e....i....N.i...
+0005f040: 3bd4 de18 d30a 34a1 5cec 8dd3 93cd 4d95  ;.....4.\.....M.
+0005f050: 265a 5282 db3a 28cf 42aa 759a 7936 1f35  &ZR..:(.B.u.y6.5
+0005f060: 55d5 5639 da47 6af4 add0 e052 8fe8 4704  U.V9.Gj....R..G.
+0005f070: 5591 45ed 8947 9fa0 6288 c6aa a6cb 6d1a  U.E..G..b.....m.
+0005f080: 113b 4269 6e61 f33f 07fa 699d 1f92 4e70  .;Bina.?..i...Np
+0005f090: 76f9 1a16 b8ee 5587 6870 71e3 62a9 2f51  v.....U.hpq.b./Q
+0005f0a0: b74c f709 019a 4a08 274e 67a9 0e98 f0f4  .L....J.'Ng.....
+0005f0b0: fb68 d1c5 8c9e e834 9ac0 f648 e2ba 2d5c  .h.....4...H..-\
+0005f0c0: 02e8 2e5b b749 a82a 1151 a0a2 4aac 74ae  ...[.I.*.Q..J.t.
+0005f0d0: e7a1 6255 aa2b d4d9 7dae ce1e 9d8c b1b3  ..bU.+..}.......
+0005f0e0: 63a4 762e 46df 280b 907d ec16 231a aa86  c.v.F.(..}..#...
+0005f0f0: 2104 3488 2b74 4f61 cebf 9d2e 4ad0 04d4  !.4.+tOa....J...
+0005f100: a798 dd2e 7d4f 8a17 8f00 151a b3be 09a9  ....}O..........
+0005f110: 983c 5e46 1b93 b576 e4fc 8893 7e4e d687  .<^F...v....~N..
+0005f120: 00f4 12f0 4367 6e1d 290c 20b1 5ad7 d764  ....Cgn.). .Z..d
+0005f130: 7175 a28a 37c2 5ab0 c7bb 95c6 e844 23e1  qu..7.Z......D#.
+0005f140: 5dbc e1e4 26a3 5d26 5be7 ec77 6d42 8230  ]...&.]&[..wmB.0
+0005f150: 4609 ae17 c091 042b 6a50 be0a ae47 eca3  F......+jP...G..
+0005f160: 41eb 2581 8d15 5d5f 3587 971e a3f2 f6ec  A.%...]_5.......
+0005f170: 48f3 141b e563 9428 cd6b 62ef d7f2 621e  H....c.(.kb...b.
+0005f180: 3aa5 5bbd 9e38 6c41 eeb5 7ba9 0da4 4383  :.[..8lA..{...C.
+0005f190: c012 31a7 9169 0005 c3d2 7947 ae7c 6f9a  ..1..i....yG.|o.
+0005f1a0: d936 0b66 085f 572b d9ff 7513 a2be 04f1  .6.f._W+..u.....
+0005f1b0: 5ef3 5266 9d5a 87fc 3d62 2431 b597 834f  ^.Rf.Z..=b$1...O
+0005f1c0: a814 7524 b69e 27d5 311b 1145 ff06 6a7a  ..u$..'.1..E..jz
+0005f1d0: 0d93 264f 7f25 7e5b 956a 8e6d 8dca 57ca  ..&O.%~[.j.m..W.
+0005f1e0: 3727 b0fc 134c acc4 bb5e f98b c6f7 0c1f  7'...L...^......
+0005f1f0: 9a4e 806f 9ac9 9da3 e935 16d7 04f0 f2fc  .N.o.....5......
+0005f200: d129 5b17 791c beae 3209 0f31 3110 2918  .)[.y...2..11.).
+0005f210: ef08 eeb9 cea0 98b2 a92b 64a9 42a8 3eb9  .........+d.B.>.
+0005f220: 05db 86de 4611 ee28 4139 aab3 7c1a 2594  ....F..(A9..|.%.
+0005f230: 2a09 d8d2 cd47 82b3 9a47 e7b4 e509 90a4  *....G...G......
+0005f240: 3bc3 ed87 58f5 504c a263 3368 ef22 9870  ;...X.PL.c3h.".p
+0005f250: 35ee 9cda 7675 b2a9 20bb 9855 4589 d260  5...vu.. ..UE..`
+0005f260: 5061 d103 cef2 3056 6b38 d230 2859 b78d  Pa....0Vk8.0(Y..
+0005f270: e3e9 b46c 92dd be44 2ac9 72af 3b6d 12d5  ...l...D*.r.;m..
+0005f280: 292e 3637 60da 3174 b675 1877 c9c3 15a0  ).67`.1t.u.w....
+0005f290: c95b 5412 d8c7 c075 d1cb a071 abda 8076  .[T....u...q...v
+0005f2a0: f677 e966 6dfd ba85 e4ef 6c53 d429 9df1  .w.fm.....lS.)..
+0005f2b0: 908a aac8 41a7 5371 4e1c d55c 3e79 8e18  ....A.SqN..\>y..
+0005f2c0: 38ce f194 149e b0c4 11e8 d41b 7536 d11b  8...........u6..
+0005f2d0: cca2 5b91 a3e7 2a26 a209 d3ab 2c3b cf80  ..[...*&....,;..
+0005f2e0: 2113 052b bb1d 582d e748 69c2 54a8 5ddc  !..+..X-.Hi.T.].
+0005f2f0: 2944 5647 5354 f117 c177 c9ac 2582 3c55  )DVGST...w..%.<U
+0005f300: f02b 2548 c290 5fe0 3e70 744a f7b5 d60c  .+%H.._.>ptJ....
+0005f310: 8ea1 0671 9819 de95 4ee8 0fd4 86e2 4cb6  ...q....N.....L.
+0005f320: 7867 a8ec 40da 52c4 ce2d 601d 4a2e a0a1  xg..@.R..-`.J...
+0005f330: fbc8 80d6 8afe 7307 b72f 5ea0 8995 8f80  ......s../^.....
+0005f340: bb4b e341 a2e2 7dfd 9fb5 6328 9db4 e479  .K.A..}...c(...y
+0005f350: c058 659d cdb6 c990 ec6c 204c e451 fcb6  .Xe......l L.Q..
+0005f360: 6486 2612 59a2 2865 1919 08ac 4a2f b513  d.&.Y.(e....J/..
+0005f370: 55e9 35b2 bf30 11f4 3d0c b2ec 9f32 6664  U.5..0..=....2fd
+0005f380: 6955 07b2 ef13 bb3f 8940 745b b8a4 1a98  iU.....?.@t[....
+0005f390: 1e99 0b8a a719 9064 5306 89a0 4373 0b1f  .......dS...Cs..
+0005f3a0: cea6 21e9 0233 55f1 e8c9 c4c0 4de4 6544  ..!..3U.....M.eD
+0005f3b0: 27cb 0b89 c224 1a10 196a 1849 495e d309  '....$...j.II^..
+0005f3c0: 7566 4599 9331 84d5 8229 ca63 079e 3197  ufE..1...).c..1.
+0005f3d0: 537d caaa 8d9e 1aa4 98c6 95d9 c59f 58b0  S}............X.
+0005f3e0: 95c8 1b89 5d86 7c24 9456 8841 669f 7949  ....].|$.V.Af.yI
+0005f3f0: 3663 38da 2d63 8499 7778 a40f aa47 bcb6  6c8.-c..wx...G..
+0005f400: d6d2 69ce 8246 f569 34ef 3b94 51d3 9db8  ..i..F.i4.;.Q...
+0005f410: 5e0b 826a 243e 6c4a 6a27 dc59 e0d4 326d  ^..j$>lJj'.Y..2m
+0005f420: 9d00 8981 6e2e 14e0 8a58 e6f0 3932 28da  ....n....X..92(.
+0005f430: 4cc5 0344 cca3 96e7 a643 c31a 976e d976  L..D.....C...n.v
+0005f440: c880 88a7 f1a8 e7d0 86d9 e5e9 6602 28d7  ............f.(.
+0005f450: 8dce 5023 0413 536a e89d 4653 1033 5e37  ..P#..Sj..FS.3^7
+0005f460: e5de 49a1 d419 9d90 60df dbe7 83db 0225  ..I.....`......%
+0005f470: 6e25 e774 e055 8f72 a488 64cf bc75 7606  n%.t.U.r..d..uv.
+0005f480: eb29 615d d7c1 09bc f454 0746 866c 808c  .)a].....T.F.l..
+0005f490: 8261 856b 68ca 02db 2ee3 5d13 c33e 3d77  .a.kh.....]..>=w
+0005f4a0: a411 394a a5b2 fd5e aa28 46d4 443c e9b0  ..9J...^.(F.D<..
+0005f4b0: e37b 7048 b322 31de 74e9 cfe0 883b 75c5  .{pH."1.t....;u.
+0005f4c0: de3d 0764 6ea7 e95a b797 587c 89d7 b089  .=.dn..Z..X|....
+0005f4d0: 537b 88bd 5c6b 7434 4814 9ade 3758 0575  S{..\kt4H...7X.u
+0005f4e0: 225a 6344 454f 840c 116e 44aa 0b35 7563  "ZcDEO...nD..5uc
+0005f4f0: f1e8 3334 f5e6 a019 1daa 8328 97a0 67f7  ..34.......(..g.
+0005f500: 1de1 da8a 8bd4 f7dd 007d b474 3b31 b63c  .........}.t;1.<
+0005f510: 1eca 1a37 ab85 a7e8 e51d 6570 8154 952f  ...7......ep.T./
+0005f520: 4f5b 3879 3adb 2e95 2d26 ad96 cfa9 5a85  O[8y:...-&....Z.
+0005f530: 136f 3e57 f382 1934 f8c8 c14c ab0a 74ce  .o>W...4...L..t.
+0005f540: d326 8068 a924 8a6a 9305 e2f8 bdda 4daa  .&.h.$.j......M.
+0005f550: cf1b f691 8e18 57c7 1bae 3e33 951b 62ce  ......W...>3..b.
+0005f560: 1a2c 78ca 2229 6509 e49d 9d75 1a7f 890d  .,x.")e....u....
+0005f570: d64b 61b0 bd75 9b5f 4e72 6e22 b6a7 f4d6  .Ka..u._Nrn"....
+0005f580: 3243 8895 3f57 d762 ae70 b76e afae f7b9  2C..?W.b.p.n....
+0005f590: a0d5 48c3 9e0e ff8e 4535 9d82 15f0 7bd9  ..H.....E5....{.
+0005f5a0: 59a2 cffc 7e8e c5ba af46 ab53 f8ab c697  Y...~....F.S....
+0005f5b0: ffd2 4f7e b6fe f0c7 7b93 d7c6 61fe 7e6d  ..O~....{...a.~m
+0005f5c0: a105 da78 8c4b aa32 dab2 f1bf d762 356a  ...x.K.2.....b5j
+0005f5d0: cd8a f44f 5b0f 9efc f14d b5f2 f82b d70d  ...O[....M...+..
+0005f5e0: f1ff 7812 55dc ba95 fada 8ddf 7fc7 0bcb  ..x.U...........
+0005f5f0: 56e0 bea5 efe4 522b e4ef 5fd8 9913 6ba5  V.....R+.._...k.
+0005f600: a510 957b f369 3b7d af7b 9d1b 5e59 fed8  ...{.i;}.{..^Y..
+0005f610: d3e9 6fbe e14f b428 e3bd bd73 9eda de7c  ..o..O.(...s...|
+0005f620: f19d e407 deaf 67ad f9cd 997f 5fcb f7d5  ......g....._...
+0005f630: 3dff 38ac 0810 0200 0000 4363 3033 0000  =.8.......Cc03..
 0005f640: 0b65 19e5 001f 0277 a4d5 7fb8 f089 3982  .e.....w......9.
 0005f650: 7d1c 9b10 386d 77f9 63e4 745b 7397 eab6  }...8mw.c.t[s...
 0005f660: d6ee 3b47 17c2 efbf 41fe 0080 9101 2b1a  ..;G....A.....+.
 0005f670: 0080 3930 2961 9484 4974 be69 3718 89e2  ..90)a..It.i7...
 0005f680: c4f0 2d0b 0972 917b d8fe 7b17 2b70 60d9  ..-..r.{..{.+p`.
 0005f690: eede 6df7 65bf f701 0f2a 51b1 e5de 7dcd  ..m.e....*Q...}.
 0005f6a0: d096 d8f4 d143 3ec2 6d99 98be 9e96 c899  .....C>.m.......
```

### Comparing `guidata-3.0.2/guidata/guitest.py` & `guidata-3.0.3/guidata/guitest.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/apply.png` & `guidata-3.0.3/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/arredit.png` & `guidata-3.0.3/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/busy.png` & `guidata-3.0.3/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/cell_edit.png` & `guidata-3.0.3/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/copy.png` & `guidata-3.0.3/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/delete.png` & `guidata-3.0.3/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/dictedit.png` & `guidata-3.0.3/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/dtype.png` & `guidata-3.0.3/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/edit.png` & `guidata-3.0.3/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/copywop.png` & `guidata-3.0.3/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/edit.png` & `guidata-3.0.3/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/edit_add.png` & `guidata-3.0.3/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/editclear.png` & `guidata-3.0.3/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/editcopy.png` & `guidata-3.0.3/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/editcut.png` & `guidata-3.0.3/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/editdelete.png` & `guidata-3.0.3/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/editpaste.png` & `guidata-3.0.3/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/fileimport.png` & `guidata-3.0.3/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/filesave.png` & `guidata-3.0.3/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/imshow.png` & `guidata-3.0.3/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/insert.png` & `guidata-3.0.3/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/plot.png` & `guidata-3.0.3/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/rename.png` & `guidata-3.0.3/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/editors/selectall.png` & `guidata-3.0.3/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/exit.png` & `guidata-3.0.3/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/file.png` & `guidata-3.0.3/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/fileclose.png` & `guidata-3.0.3/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/fileimport.png` & `guidata-3.0.3/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/fileopen.png` & `guidata-3.0.3/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filesave.png` & `guidata-3.0.3/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filesaveas.png` & `guidata-3.0.3/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/doc.png` & `guidata-3.0.3/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/gif.png` & `guidata-3.0.3/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/html.png` & `guidata-3.0.3/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/jpg.png` & `guidata-3.0.3/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/pdf.png` & `guidata-3.0.3/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/png.png` & `guidata-3.0.3/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/pps.png` & `guidata-3.0.3/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/ps.png` & `guidata-3.0.3/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/tar.png` & `guidata-3.0.3/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/tgz.png` & `guidata-3.0.3/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/tif.png` & `guidata-3.0.3/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/txt.png` & `guidata-3.0.3/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/xls.png` & `guidata-3.0.3/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/filetypes/zip.png` & `guidata-3.0.3/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/guidata-banner.svg` & `guidata-3.0.3/guidata/images/guidata-banner.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/guidata-vertical.svg` & `guidata-3.0.3/guidata/images/guidata-vertical.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/guidata.svg` & `guidata-3.0.3/guidata/images/guidata.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/not_found.png` & `guidata-3.0.3/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/python.png` & `guidata-3.0.3/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/quickview.png` & `guidata-3.0.3/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/save_all.png` & `guidata-3.0.3/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/selection.png` & `guidata-3.0.3/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/images/settings.png` & `guidata-3.0.3/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.0.3/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/qthelpers.py` & `guidata-3.0.3/guidata/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/_all_tests.py` & `guidata-3.0.3/guidata/tests/_all_tests.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/data/genreqs/pyproject.toml` & `guidata-3.0.3/guidata/tests/data/genreqs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/data/genreqs/setup.cfg` & `guidata-3.0.3/guidata/tests/data/genreqs/setup.cfg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_activable_dataset.py` & `guidata-3.0.3/guidata/tests/test_activable_dataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_activable_items.py` & `guidata-3.0.3/guidata/tests/test_activable_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_all_features.py` & `guidata-3.0.3/guidata/tests/test_all_features.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_all_items.py` & `guidata-3.0.3/guidata/tests/test_all_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_arrayeditor.py` & `guidata-3.0.3/guidata/tests/test_arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_bool_selector.py` & `guidata-3.0.3/guidata/tests/test_bool_selector.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_callbacks.py` & `guidata-3.0.3/guidata/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_codeeditor.py` & `guidata-3.0.3/guidata/tests/test_codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_collectionseditor.py` & `guidata-3.0.3/guidata/tests/test_collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_config.py` & `guidata-3.0.3/guidata/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_console.py` & `guidata-3.0.3/guidata/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_data.py` & `guidata-3.0.3/guidata/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_dataframeeditor.py` & `guidata-3.0.3/guidata/tests/test_dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_datasetgroup.py` & `guidata-3.0.3/guidata/tests/test_datasetgroup.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_disthelpers.py` & `guidata-3.0.3/guidata/tests/test_disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_editgroupbox.py` & `guidata-3.0.3/guidata/tests/test_editgroupbox.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_genreqs.py` & `guidata-3.0.3/guidata/tests/test_genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_importwizard.py` & `guidata-3.0.3/guidata/tests/test_importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_inheritance.py` & `guidata-3.0.3/guidata/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_item_order.py` & `guidata-3.0.3/guidata/tests/test_item_order.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_loadsave_hdf5.py` & `guidata-3.0.3/guidata/tests/test_loadsave_hdf5.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_loadsave_json.py` & `guidata-3.0.3/guidata/tests/test_loadsave_json.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_no_qt.py` & `guidata-3.0.3/guidata/tests/test_no_qt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_objecteditor.py` & `guidata-3.0.3/guidata/tests/test_objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_rotatedlabel.py` & `guidata-3.0.3/guidata/tests/test_rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_text.py` & `guidata-3.0.3/guidata/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/tests/test_userconfig_app.py` & `guidata-3.0.3/guidata/tests/test_userconfig_app.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/userconfig.py` & `guidata-3.0.3/guidata/userconfig.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/__init__.py` & `guidata-3.0.3/guidata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/disthelpers.py` & `guidata-3.0.3/guidata/utils/disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/encoding.py` & `guidata-3.0.3/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/genreqs.py` & `guidata-3.0.3/guidata/utils/genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/gettext_helpers.py` & `guidata-3.0.3/guidata/utils/gettext_helpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/utils/misc.py` & `guidata-3.0.3/guidata/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/__init__.py` & `guidata-3.0.3/guidata/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/arrayeditor.py` & `guidata-3.0.3/guidata/widgets/arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/codeeditor.py` & `guidata-3.0.3/guidata/widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/collectionseditor.py` & `guidata-3.0.3/guidata/widgets/collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/__init__.py` & `guidata-3.0.3/guidata/widgets/console/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/base.py` & `guidata-3.0.3/guidata/widgets/console/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/calltip.py` & `guidata-3.0.3/guidata/widgets/console/calltip.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/dochelpers.py` & `guidata-3.0.3/guidata/widgets/console/dochelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/internalshell.py` & `guidata-3.0.3/guidata/widgets/console/internalshell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/interpreter.py` & `guidata-3.0.3/guidata/widgets/console/interpreter.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/mixins.py` & `guidata-3.0.3/guidata/widgets/console/mixins.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/shell.py` & `guidata-3.0.3/guidata/widgets/console/shell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/console/terminal.py` & `guidata-3.0.3/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/dataframeeditor.py` & `guidata-3.0.3/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/dockable.py` & `guidata-3.0.3/guidata/widgets/dockable.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/importwizard.py` & `guidata-3.0.3/guidata/widgets/importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/nsview.py` & `guidata-3.0.3/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/objecteditor.py` & `guidata-3.0.3/guidata/widgets/objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/rotatedlabel.py` & `guidata-3.0.3/guidata/widgets/rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/syntaxhighlighters.py` & `guidata-3.0.3/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata/widgets/texteditor.py` & `guidata-3.0.3/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/guidata.egg-info/PKG-INFO` & `guidata-3.0.3/guidata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.2
-Summary: Signal and image processing software
+Version: 3.0.3
+Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -55,15 +55,14 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # guidata: Automatic GUI generation for easy dataset editing and display with Python
 
-[![license](https://img.shields.io/pypi/l/guidata.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/guidata.svg)](https://pypi.org/project/guidata/)
 [![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/CODRA-Ingenierie-Informatique/guidata/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/guidata.svg)](https://pypi.python.org/pypi/guidata/)
 [![download count](https://img.shields.io/conda/dn/conda-forge/guidata.svg)](https://www.anaconda.com/download/)
 
 Simple example of ``guidata`` datasets embedded in an application window:
 
@@ -97,20 +96,38 @@
 * HDF5 I/O helpers
 * misc. utils
 
 ## Dependencies
 
 ### Requirements
 
-* Python 3.7+
+* Python 3.8+
 * [PyQt5](https://pypi.python.org/pypi/PyQt5) (Python Qt bindings)
 * [QtPy](https://pypi.org/project/QtPy/) (abstraction layer for Python-Qt binding libraries)
 * [h5py](https://pypi.org/project/h5py/) (interface to the HDF5 data format)
 * [NumPy](https://pypi.org/project/numpy/) (operations on multidimensional arrays)
+* [requests](https://pypi.org/project/requests/) (HTTP library)
+* [tomli](https://pypi.org/project/tomli/) (TOML parser)
+
+### Optional dependencies
+
+For some editing widgets:
+
+* [pillow](https://pypi.org/project/Pillow/) (image processing library)
+* [pandas](https://pypi.org/project/pandas/) (data analysis library)
+
+For documentation generation:
+
+* [sphinx](https://pypi.org/project/Sphinx/) (Python documentation generator)
+* [sphinx-copybutton](https://pypi.org/project/sphinx-copybutton/) (add a copy button to each of your code cells)
+* [sphinx_qt_documentation](https://pypi.org/project/sphinx-qt-documentation/) (plugin for proper resolve intersphinx references for Qt elements)
+* [python-docs-theme](https://pypi.org/project/python-docs-theme/) (Python documentation theme)
 
 ## Installation
 
 ### From the source package
 
+Using ``build``:
+
 ```bash
-python setup.py install
+python -m build
 ```
```

### Comparing `guidata-3.0.2/guidata.egg-info/SOURCES.txt` & `guidata-3.0.3/guidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guidata-3.0.2/pyproject.toml` & `guidata-3.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "guidata"
 authors = [{ name = "Codra", email = "p.raybaut@codra.fr" }]
-description = "Signal and image processing software"
+description = "Automatic GUI generation for easy dataset editing and display"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering",
```

