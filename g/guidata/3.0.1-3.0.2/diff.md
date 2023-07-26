# Comparing `tmp/guidata-3.0.1.tar.gz` & `tmp/guidata-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-3.0.1.tar", last modified: Fri Jul 21 16:08:50 2023, max compression
+gzip compressed data, was "guidata-3.0.2.tar", last modified: Wed Jul 26 11:38:44 2023, max compression
```

## Comparing `guidata-3.0.1.tar` & `guidata-3.0.2.tar`

### file list

```diff
@@ -1,178 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.687090 guidata-3.0.1/
--rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-07-21 16:08:50.685076 guidata-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-07-18 08:47:02.000000 guidata-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.272077 guidata-3.0.1/guidata/
--rw-rw-rw-   0        0        0     3004 2023-07-07 13:55:43.000000 guidata-3.0.1/guidata/__init__.py
--rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.1/guidata/config.py
--rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.1/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.299077 guidata-3.0.1/guidata/dataset/
--rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.1/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.1/guidata/dataset/datatypes.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.310080 guidata-3.0.1/guidata/dataset/io/
--rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.1/guidata/dataset/io/__init__.py
--rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.1/guidata/dataset/io/base.py
--rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.1/guidata/dataset/io/h5fmt.py
--rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.1/guidata/dataset/io/inifmt.py
--rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.1/guidata/dataset/io/jsonfmt.py
--rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.1/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.1/guidata/env.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.313093 guidata-3.0.1/guidata/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.325077 guidata-3.0.1/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0   394832 2023-07-21 16:08:26.000000 guidata-3.0.1/guidata/guidata.chm
--rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.1/guidata/guitest.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.408076 guidata-3.0.1/guidata/images/
--rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.446075 guidata-3.0.1/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.518077 guidata-3.0.1/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.1/guidata/images/guidata-banner.svg
--rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.1/guidata/images/guidata-vertical.svg
--rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.1/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/xmin.png
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.224078 guidata-3.0.1/guidata/locale/
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.225076 guidata-3.0.1/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.521093 guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.1/guidata/qthelpers.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.601078 guidata-3.0.1/guidata/tests/
--rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.1/guidata/tests/_all_tests.py
--rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.1/guidata/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.229076 guidata-3.0.1/guidata/tests/data/
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.606075 guidata-3.0.1/guidata/tests/data/genreqs/
--rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.1/guidata/tests/data/genreqs/pyproject.toml
--rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.1/guidata/tests/data/genreqs/setup.cfg
--rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.1/guidata/tests/test_activable_dataset.py
--rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.1/guidata/tests/test_activable_items.py
--rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.1/guidata/tests/test_all_features.py
--rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.1/guidata/tests/test_all_items.py
--rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.1/guidata/tests/test_arrayeditor.py
--rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.1/guidata/tests/test_bool_selector.py
--rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.1/guidata/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.1/guidata/tests/test_codeeditor.py
--rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.1/guidata/tests/test_collectionseditor.py
--rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/test_config.py
--rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.1/guidata/tests/test_console.py
--rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.1/guidata/tests/test_data.py
--rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.1/guidata/tests/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/test_datasetgroup.py
--rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.1/guidata/tests/test_disthelpers.py
--rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.1/guidata/tests/test_editgroupbox.py
--rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.1/guidata/tests/test_genreqs.py
--rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.1/guidata/tests/test_importwizard.py
--rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.1/guidata/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.1/guidata/tests/test_item_order.py
--rw-rw-rw-   0        0        0     1108 2023-07-19 09:56:40.000000 guidata-3.0.1/guidata/tests/test_loadsave_hdf5.py
--rw-rw-rw-   0        0        0     1042 2023-07-19 09:55:37.000000 guidata-3.0.1/guidata/tests/test_loadsave_json.py
--rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.1/guidata/tests/test_no_qt.py
--rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.1/guidata/tests/test_objecteditor.py
--rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.1/guidata/tests/test_rotatedlabel.py
--rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.1/guidata/tests/test_text.py
--rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.1/guidata/tests/test_translations.py
--rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.1/guidata/tests/test_userconfig_app.py
--rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.1/guidata/userconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.628077 guidata-3.0.1/guidata/utils/
--rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.1/guidata/utils/__init__.py
--rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.1/guidata/utils/disthelpers.py
--rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/utils/encoding.py
--rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.1/guidata/utils/genreqs.py
--rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.1/guidata/utils/gettext_helpers.py
--rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.1/guidata/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.661076 guidata-3.0.1/guidata/widgets/
--rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.1/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.1/guidata/widgets/arrayeditor.py
--rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.1/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.1/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.684075 guidata-3.0.1/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.1/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.1/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.1/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.1/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.1/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.1/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.1/guidata/widgets/dockable.py
--rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.1/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.1/guidata/widgets/rotatedlabel.py
--rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/texteditor.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.285075 guidata-3.0.1/guidata.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4841 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1957 2023-07-21 16:08:07.000000 guidata-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 16:08:50.688087 guidata-3.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.992524 guidata-3.0.2/
+-rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0        9 2023-07-26 09:34:47.000000 guidata-3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5248 2023-07-26 11:38:44.990517 guidata-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2023-07-18 08:47:02.000000 guidata-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.386199 guidata-3.0.2/doc/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.388199 guidata-3.0.2/doc/_static/
+-rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.2/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.2/doc/basic_example.py
+-rw-rw-rw-   0        0        0     1659 2023-07-21 12:45:55.000000 guidata-3.0.2/doc/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.400197 guidata-3.0.2/doc/dev/
+-rw-rw-rw-   0        0        0     2675 2023-07-21 10:37:23.000000 guidata-3.0.2/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.2/doc/dev/howto.rst
+-rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.2/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     2171 2023-07-19 10:06:27.000000 guidata-3.0.2/doc/dev/v2_to_v3.csv
+-rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.0.2/doc/dev/v2_to_v3.rst
+-rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.2/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.409198 guidata-3.0.2/doc/images/
+-rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.2/doc/images/basic_example.png
+-rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.2/doc/images/guidata-banner.png
+-rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.2/doc/images/guidata-vertical.png
+-rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.2/doc/images/layout_example.png
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.430199 guidata-3.0.2/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.2/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.2/doc/images/screenshots/activable_dataset.png
+-rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.2/doc/images/screenshots/all_features.png
+-rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.2/doc/images/screenshots/all_items.png
+-rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.2/doc/images/screenshots/bool_selector.png
+-rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.2/doc/images/screenshots/datasetgroup.png
+-rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.2/doc/images/screenshots/editgroupbox.png
+-rw-rw-rw-   0        0        0      933 2023-07-18 09:00:42.000000 guidata-3.0.2/doc/index.rst
+-rw-rw-rw-   0        0        0      181 2023-07-21 12:29:31.000000 guidata-3.0.2/doc/installation.rst
+-rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.2/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.441199 guidata-3.0.2/doc/reference/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.456199 guidata-3.0.2/doc/reference/dataset/
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.2/doc/reference/dataset/dataitems.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.2/doc/reference/dataset/datatypes.rst
+-rw-rw-rw-   0        0        0      144 2023-07-07 14:10:24.000000 guidata-3.0.2/doc/reference/dataset/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-19 09:25:53.000000 guidata-3.0.2/doc/reference/dataset/io.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.2/doc/reference/dataset/qtwidgets.rst
+-rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.2/doc/reference/guitest.rst
+-rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.0.2/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       34 2023-07-07 14:22:12.000000 guidata-3.0.2/doc/reference/userconfig.rst
+-rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.2/doc/reference/utils.rst
+-rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.2/doc/reference/widgets.rst
+-rw-rw-rw-   0        0        0     2460 2023-07-26 11:38:27.000000 guidata-3.0.2/doc/requirements.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.476204 guidata-3.0.2/guidata/
+-rw-rw-rw-   0        0        0     3004 2023-07-26 09:52:33.000000 guidata-3.0.2/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.2/guidata/config.py
+-rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.2/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.505202 guidata-3.0.2/guidata/dataset/
+-rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.2/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.2/guidata/dataset/datatypes.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.518204 guidata-3.0.2/guidata/dataset/io/
+-rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.2/guidata/dataset/io/__init__.py
+-rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.2/guidata/dataset/io/base.py
+-rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.2/guidata/dataset/io/h5fmt.py
+-rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.2/guidata/dataset/io/inifmt.py
+-rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.2/guidata/dataset/io/jsonfmt.py
+-rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.2/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.2/guidata/env.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.520204 guidata-3.0.2/guidata/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.532204 guidata-3.0.2/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0   394832 2023-07-26 11:38:25.000000 guidata-3.0.2/guidata/guidata.chm
+-rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.2/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.727964 guidata-3.0.2/guidata/images/
+-rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.777967 guidata-3.0.2/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.812974 guidata-3.0.2/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.2/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.2/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.2/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.352196 guidata-3.0.2/guidata/locale/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.352196 guidata-3.0.2/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.815968 guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.2/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.902513 guidata-3.0.2/guidata/tests/
+-rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.2/guidata/tests/_all_tests.py
+-rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.2/guidata/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.355198 guidata-3.0.2/guidata/tests/data/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.909528 guidata-3.0.2/guidata/tests/data/genreqs/
+-rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.2/guidata/tests/data/genreqs/pyproject.toml
+-rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.2/guidata/tests/data/genreqs/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.2/guidata/tests/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.2/guidata/tests/test_activable_items.py
+-rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.2/guidata/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.2/guidata/tests/test_all_items.py
+-rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.2/guidata/tests/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.2/guidata/tests/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.2/guidata/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.2/guidata/tests/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.2/guidata/tests/test_collectionseditor.py
+-rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/test_config.py
+-rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.2/guidata/tests/test_console.py
+-rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.2/guidata/tests/test_data.py
+-rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.2/guidata/tests/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.2/guidata/tests/test_datasetgroup.py
+-rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.2/guidata/tests/test_disthelpers.py
+-rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.2/guidata/tests/test_editgroupbox.py
+-rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.2/guidata/tests/test_genreqs.py
+-rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.2/guidata/tests/test_importwizard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.2/guidata/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.2/guidata/tests/test_item_order.py
+-rw-rw-rw-   0        0        0     1142 2023-07-26 11:35:40.000000 guidata-3.0.2/guidata/tests/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1078 2023-07-26 11:35:40.000000 guidata-3.0.2/guidata/tests/test_loadsave_json.py
+-rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.2/guidata/tests/test_no_qt.py
+-rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.2/guidata/tests/test_objecteditor.py
+-rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.2/guidata/tests/test_rotatedlabel.py
+-rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.2/guidata/tests/test_text.py
+-rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.2/guidata/tests/test_translations.py
+-rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.2/guidata/tests/test_userconfig_app.py
+-rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.2/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.925519 guidata-3.0.2/guidata/utils/
+-rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.2/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.2/guidata/utils/disthelpers.py
+-rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.2/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.2/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.2/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.962516 guidata-3.0.2/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.2/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.2/guidata/widgets/arrayeditor.py
+-rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.2/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.2/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.988517 guidata-3.0.2/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.2/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.2/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.2/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.2/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.2/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.2/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.2/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.2/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.2/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.2/guidata/widgets/texteditor.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:38:44.489202 guidata-3.0.2/guidata.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5799 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 11:38:44.000000 guidata-3.0.2/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1949 2023-07-26 09:34:07.000000 guidata-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:38:44.992524 guidata-3.0.2/setup.cfg
```

### Comparing `guidata-3.0.1/LICENSE` & `guidata-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/PKG-INFO` & `guidata-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.1
+Version: 3.0.2
 Summary: Signal and image processing software
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `guidata-3.0.1/README.md` & `guidata-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/__init__.py` & `guidata-3.0.2/guidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 =======
 
 Based on the Qt library :mod:`guidata` is a Python library generating graphical
 user interfaces for easy dataset editing and display. It also provides helpers
 and application development tools for Qt.
 """
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (images) and translations:
 DATAPATH = LOCALEPATH = ""
```

### Comparing `guidata-3.0.1/guidata/config.py` & `guidata-3.0.2/guidata/config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/configtools.py` & `guidata-3.0.2/guidata/configtools.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/__init__.py` & `guidata-3.0.2/guidata/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/dataitems.py` & `guidata-3.0.2/guidata/dataset/dataitems.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/datatypes.py` & `guidata-3.0.2/guidata/dataset/datatypes.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/io/__init__.py` & `guidata-3.0.2/guidata/dataset/io/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/io/base.py` & `guidata-3.0.2/guidata/dataset/io/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/io/h5fmt.py` & `guidata-3.0.2/guidata/dataset/io/h5fmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/io/inifmt.py` & `guidata-3.0.2/guidata/dataset/io/inifmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/io/jsonfmt.py` & `guidata-3.0.2/guidata/dataset/io/jsonfmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/qtitemwidgets.py` & `guidata-3.0.2/guidata/dataset/qtitemwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/qtwidgets.py` & `guidata-3.0.2/guidata/dataset/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/dataset/textedit.py` & `guidata-3.0.2/guidata/dataset/textedit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/env.py` & `guidata-3.0.2/guidata/env.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/external/darkdetect/__init__.py` & `guidata-3.0.2/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.0.2/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.0.2/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.0.2/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/guidata.chm` & `guidata-3.0.2/guidata/guidata.chm`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 4954 5346 0300 0000 6000 0000 0100 0000  ITSF....`.......
-00000010: 9787 9594 0c04 0000 10fd 017c aa7b d011  ...........|.{..
+00000010: 4017 d5af 0c04 0000 10fd 017c aa7b d011  @..........|.{..
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
-000012f0: 0000 0300 0000 0a00 0400 7aad ba64 0900  ..........z..d..
+000012f0: 0000 0300 0000 0a00 0400 b105 c164 0900  .............d..
 00001300: 1600 4848 4120 5665 7273 696f 6e20 342e  ..HHA Version 4.
 00001310: 3734 2e38 3730 3200 0400 2400 0904 0000  74.8702...$.....
 00001320: 0000 0000 0100 0000 0100 0000 0000 0000  ................
-00001330: d79c 9494 edbb d901 0000 0000 0000 0000  ................
+00001330: 8553 d4af b5bf d901 0000 0000 0000 0000  .S..............
 00001340: 0200 0b00 696e 6465 782e 6874 6d6c 0003  ....index.html..
 00001350: 0013 0067 7569 6461 7461 2033 2e30 204d  ...guidata 3.0 M
 00001360: 616e 7561 6c00 0600 0800 6775 6964 6174  anual.....guidat
 00001370: 6100 0500 0800 6775 6964 6174 6100 0c00  a.....guidata...
-00001380: 0400 0000 0000 0d00 0010 5423 534d ca02  ..........T#SM..
-00001390: 8902 0100 0000 5b01 0000 0000 0000 ffff  ......[.........
+00001380: 0400 0000 0000 0d00 0010 5423 534d 1d32  ..........T#SM.2
+00001390: 3501 0100 0000 5b01 0000 0000 0000 ffff  5.....[.........
 000013a0: ffff 0000 0000 0100 0000 ffff ffff ffff  ................
 000013b0: ffff ffff ffff 2712 8000 ffff ffff ffff  ......'.........
 000013c0: ffff ffff ffff ffff ffff 0000 0000 0100  ................
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -23746,682 +23746,682 @@
 0005cc10: 0d29 834c 94f5 5906 2f42 e8a9 efbf bc23  .).L..Y./B.....#
 0005cc20: 69d8 1571 6742 c373 699c f6fd dac1 cc17  i..qgB.si.......
 0005cc30: 2f14 6e61 42b4 e648 07d0 284a 6b3e c799  /.naB..H..(Jk>..
 0005cc40: 4963 7ffb 0e74 7c34 498b 1319 ca77 be31  Ic...t|4I....w.1
 0005cc50: 259e 84be 9a4b 7ff6 f305 79c9 fc00 5406  %....K....y...T.
 0005cc60: df00 e23e b671 a026 0000 0000 0a00 0940  ...>.q.&.......@
 0005cc70: 38d8 0115 2aac 81b0 8caa 4401 1901 adab  8...*.....D.....
-0005cc80: 5f80 10a5 4108 aa4a e1a0 00f9 95e8 6683  _...A..J......f.
-0005cc90: bd50 18a6 dfaf e1df 5d24 5574 f315 aaf2  .P......]$Ut....
-0005cca0: 099a 3302 5544 0060 6465 6053 a205 9453  ..3.UD.`de`S...S
-0005ccb0: 2d58 d00c 7a1a bc8c 4c58 f5e1 ca9c c0bf  -X..z...LX......
-0005ccc0: e117 7688 f4a2 c097 4671 1fa1 9692 ca87  ..v.....Fq......
-0005ccd0: 012b 2899 1c83 8f70 4f09 7185 11c4 eaab  .+(....pO.q.....
-0005cce0: a108 a6d4 c14a d093 13c1 42e8 3d1d 1dae  .....J....B.=...
-0005ccf0: 253b 8300 2530 9b25 9008 4026 c09d 8e80  %;..%0.%..@&....
-0005cd00: 48fc 8193 68cb c76c bce6 c3de 767b 1b58  H...h..l....v{.X
-0005cd10: 05b0 0080 0018 010d 1995 3f4c dd38 f8f0  ..........?L.8..
-0005cd20: ce4c 1e92 fbcb 3af3 4029 4995 6d7e 9c3f  .L....:.@)I.m~.?
-0005cd30: 39da d31d c51e 8fef e4bf dc4d 5af6 ca10  9..........MZ...
-0005cd40: d06b 100b 53a8 fed7 cfcf 7340 f23b 516e  .k..S.....s@.;Qn
-0005cd50: 7e40 f7c6 d414 20c8 fab1 be9f f3bf 44ae  ~@.... .......D.
-0005cd60: f563 de09 7dd1 ddad 6319 3e7b 632a b2ee  .c..}...c.>{c*..
-0005cd70: 11c4 c28e 4885 542d 3e58 a717 c7a3 5c5c  ....H.T->X....\\
-0005cd80: 6f91 fab3 4e4a 96ad dc47 3160 96df f23d  o...NJ...G1`...=
-0005cd90: 2750 8e29 ee2c 2e7f 463a d337 3cf6 4f2d  'P.).,..F:.7<.O-
-0005cda0: 3c74 702e cfc1 bdb6 3bf0 f7fb 82ca 4df6  <tp.....;.....M.
-0005cdb0: a108 a288 c1fc 3ebc 6811 7146 0de1 15bd  ......>.h.qF....
-0005cdc0: ba2a e9bd f582 8d21 b1ec c75f dc1b 6b63  .*.....!..._..kc
-0005cdd0: f9fc 53aa c8cd 4082 5d65 de8f 8d5d b9e3  ..S...@.]e...]..
-0005cde0: b108 6a8b c3f9 7f70 b54b c15f b795 05b2  ..j....p.K._....
-0005cdf0: 917c d1bc 3365 cbf1 387e ac41 50bb f791  .|..3e..8~.AP...
-0005ce00: d1f2 ef99 419c ffcc adcd af5a 7fcf abed  ....A......Z....
-0005ce10: e7c0 d10a 6b1b d91b 5532 271f 8bbc df4b  ....k...U2'....K
-0005ce20: 2121 eb92 c88d 3c5e 63e4 cd66 90e9 fa89  !!....<^c..f....
-0005ce30: 6bf9 03f8 4864 103c 95bc b49b 4ab1 f5df  k...Hd.<....J...
-0005ce40: d71b 2b57 5911 f35d 28df ae4a fcbf 9cb3  ..+WY..](..J....
-0005ce50: f91e 0920 e187 2e67 e72b 26ca a99f 5fa7  ... ...g.+&..._.
-0005ce60: 4f7b fcd4 fe54 f9a7 b23d 125c 06cb cc57  O{...T...=.\...W
-0005ce70: 2322 bbbc 9981 cb6c 1bdd 599a 2708 bd56  #".....l..Y.'..V
-0005ce80: 4fb6 b2fa 75dc c372 a4bc ddcc d941 5a71  O...u..r.....AZq
-0005ce90: cbdb b35a bf56 5724 ab22 6386 79ab 1c52  ...Z.VW$."c.y..R
-0005cea0: 1fd5 7e5a 3239 ea83 308c c291 6c85 92db  ..~Z29..0...l...
-0005ceb0: f508 1fd6 c72c 4ea8 1bae fb7a 757b 7bd3  .....,N....zu{{.
-0005cec0: 892f fe20 6fb4 487a 062f c4e2 7a78 6ea1  ./. o.Hz./..zxn.
-0005ced0: 1bbf 0fd2 7fbc 617b 72a3 278e 0462 9158  ......a{r.'..b.X
-0005cee0: f2e4 e1e2 358f 4c3d c413 c232 73a1 8663  ....5.L=...2s..c
-0005cef0: fffa d15f 4ed1 3f4f f55a 670d 8f2e 688a  ..._N.?O.Zg...h.
-0005cf00: f28e f921 5f1f 7a92 3f91 86a9 7008 3585  ...!_.z.?...p.5.
-0005cf10: 698f ff23 1f69 f6a5 dfd4 77cb 07a9 2e51  i..#.i....w....Q
-0005cf20: 356b 8f13 d19b 05e1 7930 c47d 632c 2c62  5k......y0.}c,,b
-0005cf30: fac2 fba1 4e81 165b 6e9a fc8c 3a7d 79a2  ....N..[n...:}y.
-0005cf40: 95ef b809 77fd 437b 4bee dadd 005e 6217  ....w.C{K....^b.
-0005cf50: 291e fd6d 17c9 e8f5 1499 abf6 deea 8d4f  )..m...........O
-0005cf60: 7ec4 7f09 e2d7 103a de54 85fb 1c07 7b23  ~......:.T....{#
-0005cf70: 2a5b 8f77 83bf de15 b0f8 577f 9d54 ef34  *[.w......W..T.4
-0005cf80: 9428 ed2b e5c4 e9c4 2dce 9fab 62fb 981c  .(.+....-...b...
-0005cf90: 75c5 95d7 4622 caa9 e333 8e7f 17be f0ba  u...F"...3......
-0005cfa0: f761 67b8 3fe5 a5a4 f7f9 84c0 e45d e0b7  .ag.?........]..
-0005cfb0: 8ce0 a146 86e3 7ced 65cb 0bf9 1e6a d9fc  ...F..|.e....j..
-0005cfc0: 33fd c0d5 f4ee e7eb 7c60 b37e 7f7b f121  3.......|`.~.{.!
-0005cfd0: 640f d4f6 d4eb 856c 884e 2428 eb3d 3d51  d......l.N$(.==Q
-0005cfe0: 7fc6 2271 420f 907d 0ab2 2458 e866 12f1  .."qB..}..$X.f..
-0005cff0: 8f5c c9e4 47e5 e8f2 3345 9aab 10e9 a6a7  .\..G...3E......
-0005d000: 1ee3 89d3 4d5e d0a4 9888 7da6 12ff fa72  ....M^....}....r
-0005d010: f6c8 4d80 ff83 7b16 b503 8edf 7fe2 b50b  ..M...{.........
-0005d020: 86ff fe55 e6c7 2448 b996 1eb5 ea31 6cbd  ...U..$H.....1l.
-0005d030: 8a5f 0aa1 5d5e 1b85 7bb4 d0f1 ed9f f9d1  ._..]^..{.......
-0005d040: aa8d e63e 8e95 4a41 a023 103b c4b7 7fac  ...>..JA.#.;....
-0005d050: aa7d bc69 fe13 6271 09f2 8b7c ded6 c4a2  .}.i..bq...|....
-0005d060: c769 eb91 e6fb d5fb 1387 bbe9 28f2 a264  .i..........(..d
-0005d070: ef9e b0c9 3855 b95b 2420 161e 5ff1 909a  ....8U.[$ .._...
-0005d080: 01b2 44ba 903c 09f2 d2c6 8967 bfdc 96ff  ..D..<.....g....
-0005d090: 7bed bd91 1ed3 cc9b f704 e925 f936 f999  {..........%.6..
-0005d0a0: 723e 721d aa12 d69e 2995 53ea 0a32 5f87  r>r.....).S..2_.
-0005d0b0: a109 4e1f f275 f829 177d 427b cbc7 fbbf  ..N..u.).}B{....
-0005d0c0: 2979 403f 87c2 e2df f0e0 5efa fcdd e3d4  )y@?......^.....
-0005d0d0: 15e5 6eba 7dd4 845b 65f8 d3ad f4b8 73c9  ..n.}..[e.....s.
-0005d0e0: aa6d 684f 773c c3f5 e55d 56c6 6f3a 7d31  .mhOw<...]V.o:}1
-0005d0f0: 78e7 bc53 9881 d0de 160b d3fb 3e9c b7bd  x..S........>...
-0005d100: 574e fa5d 16ea aa13 4236 6d12 2ef1 e806  WN.]....B6m.....
-0005d110: 1ebf ad31 72fb 7cdb e43b f88f bd7e 49bd  ...1r.|..;...~I.
-0005d120: 2e10 2ffe bda6 6089 a4ce 0422 4fa2 46f1  ../...`...."O.F.
-0005d130: 7ee4 675e db76 7d7a f2ab 337b 87ee 8de9  ~.g^.v}z..3{....
-0005d140: f546 cb83 acea 3163 dbe9 14e3 cce3 d29c  .F....1c........
-0005d150: 77f3 8bfa b13f f1d5 af60 f46c fa82 38e0  w....?...`.l..8.
-0005d160: 03b9 33bd 31d9 f339 2b8e d7a8 38c6 de51  ..3.1..9+...8..Q
-0005d170: ec89 b7fa 0ff8 e796 a3fc 8086 8f77 11ff  .............w..
-0005d180: 3ce0 1a49 c637 0f4a 36e7 0419 a4c3 da5f  <..I.7.J6......_
-0005d190: b162 03f3 1777 505f ac61 3eff 9669 96d5  .b...wP_.a>..i..
-0005d1a0: ff20 c0dc 9924 fdd6 46ed eec0 f66c 4e58  . ...$..F....lNX
-0005d1b0: 6e16 1c48 7ff1 6f7d 0b45 a7b1 dcfb c72b  n..H..o}.E.....+
-0005d1c0: ead6 1677 ce8f 6e3a 3a01 4785 b880 bdd6  ...w..n::.G.....
-0005d1d0: 721f 6bee 4671 5dba 7879 43c1 6615 0b13  r.k.Fq].xyC.f...
-0005d1e0: b42b 7cef e7bf 3b15 f275 a550 bd43 0bd8  .+|...;..u.P.C..
-0005d1f0: 5fbc 6a23 2776 5251 becf 5777 a4e0 2c71  _.j#'vRQ..Ww..,q
-0005d200: df61 e643 c1b4 6df9 7bd6 8ab5 1bcd dafd  .a.C..m.{.......
-0005d210: 677f 757f de91 ce2b 7dfa 7f34 ef15 bb48  g.u....+}..4...H
-0005d220: 0ffd f33f d6d5 946e 2e89 761a 1dc4 ffd3  ...?...n..v.....
-0005d230: c5c5 070f 9cb6 1078 d0a9 8997 efaa 40ff  .......x......@.
-0005d240: 39f0 38d3 bebe 5824 7eef 5707 f917 399f  9.8...X$~.W...9.
-0005d250: c35d 7fd1 1076 afa7 7b72 f6ae 54bf 3dba  .]...v..{r..T.=.
-0005d260: f1b8 a8eb f995 c707 8a40 64d2 4d13 bdc5  .........@d.M...
-0005d270: cf4a 3a4f 7e88 f9ce a50f 78cf 1c92 399a  .J:O~.....x...9.
-0005d280: 5eca 66cc b87f 23b2 e750 553d cf70 48b2  ^.f...#..PU=.pH.
-0005d290: 8cff c052 7475 925f ad26 7987 5f17 db8c  ...Rtu._.&y._...
-0005d2a0: 32d9 ecbe 76a0 5e86 77f8 147f aa8f 5dff  2...v.^.w.....].
-0005d2b0: b26b 8e5c 48f9 399c fb1c b52b d6e7 2d3f  .k.\H.9....+..-?
-0005d2c0: 3693 fb67 3df9 3d4d 6fcc 082b 3b2d 70da  6..g=.=Mo..+;-p.
-0005d2d0: eef3 f88f f85b 1f67 6fbc 7fdc 04cc 76ff  .....[.go.....v.
-0005d2e0: ec65 ffa9 b1a0 daa9 cbbd 10ea c486 7157  .e............qW
-0005d2f0: fa04 e44c aab6 1388 7dae a53d b23e 6a81  ...L....}..=.>j.
-0005d300: d9e3 1ff1 057c 11f2 43d8 3ff1 efa2 1e2e  .....|..C.?.....
-0005d310: 430f f73a 3f94 5331 9ef6 6848 dfc9 4e87  C..:?.S1..hH..N.
-0005d320: caa1 4399 f6d1 c3bd a81f 85ff a389 d2fb  ..C.............
-0005d330: af70 83f8 dc4d 0805 417a b4ef e4e4 a1c3  .p...M..Az......
-0005d340: 2eff e5df 4970 1708 4e1a a126 d0f1 d579  ....Ip..N..&...y
-0005d350: 523e faf9 607d 4ff4 676a a457 eb57 3111  R>..`}O.gj.W.W1.
-0005d360: 3fa8 5448 ec21 ca7b 35f0 86f5 ddab 55bc  ?.TH.!.{5.....U.
-0005d370: 820f 0ee1 3a28 aa15 dc33 c84e d55c 9c60  ....:(...3.N.\.`
-0005d380: f947 2bdb ec6d dafb ddbf 98de 70dc d8e3  .G+..m......p...
-0005d390: c7d4 cbdf 85aa 37d5 8b40 4aec e345 e179  ......7..@J..E.y
-0005d3a0: 37f5 679b bbdf f108 3126 417f fff2 06fd  7.g.....1&A.....
-0005d3b0: f556 dee7 4595 6053 c312 feb7 50f3 d783  .V..E.`S....P...
-0005d3c0: 6a96 bb27 3fd6 818e 7fbc 7898 5e7d 8ae8  j..'?.....x.^}..
-0005d3d0: f612 5b0f 12d2 9cce b7e7 5d20 f30d 442f  ..[.......] ..D/
-0005d3e0: 9cc7 4ef1 5f7f eff9 4699 f309 bd6c fde4  ..N._...F....l..
-0005d3f0: a7fc b432 401f 12e4 939e 5077 dae7 9eb3  ...2@.....Pw....
-0005d400: ff29 8a8a fa73 7024 bdd2 8b91 c972 8df1  .)...sp$.....r..
-0005d410: f1cd 3e89 8e30 de79 e2ff 5110 03fd bf1e  ..>..0.y..Q.....
-0005d420: 0b59 cfe1 be5f bf6c f3ab 0909 89f9 d1e7  .Y..._.l........
-0005d430: dfd5 46c3 02d9 5127 bf22 3ae0 cca3 5f47  ..F...Q'.":..._G
-0005d440: def4 8cef 436e 10f6 acb8 de74 53a4 3b81  ....Cn.....tS.;.
-0005d450: 6098 c394 63a1 7ef2 ab97 a756 e572 85fc  `...c.~....V.r..
-0005d460: ed44 f929 014a ed2e f2db 2e03 77b2 4990  .D.).J......w.I.
-0005d470: 777d 388f ea8f a20e 141e a248 f315 3d79  w}8........H..=y
-0005d480: 7cf3 9028 0bff 0bde 85fc 7b9b c95f 0c7a  |..(......{.._.z
-0005d490: 43ff 3a3f b318 e7c9 d8bb a9f8 d655 2578  C.:?.........U%x
-0005d4a0: 7d88 d3a7 cd8a 6ae9 d49b e727 5629 f996  }.....j....'V)..
-0005d4b0: fd26 98bf 35fe bc1e b7f8 fffa 2f45 4a7f  .&..5......./EJ.
-0005d4c0: 08ff f5b7 9bb3 7dbe 0721 7144 8688 8730  ......}..!qD...0
-0005d4d0: 96ae f3da 3dc7 711e 793c 28d5 aff6 5593  ....=.q.y<(...U.
-0005d4e0: dfbd a9ac f17e 49bd 0e6b 2dc4 83cc ff61  .....~I..k-....a
-0005d4f0: fd51 ffbb 0f0c 8577 5b68 c057 9e2b a43a  .Q.....w[h.W.+.:
-0005d500: a843 db9f f179 71a3 2bfc 905e 8f0f cf9b  .C...yq.+..^....
-0005d510: ea2b 2a3b 2c42 df22 4382 9de4 a440 c9f5  .+*;,B."C....@..
-0005d520: 54b0 4ee1 1ee2 fc94 656f a59d 47bd ede1  T.N.....eo..G...
-0005d530: 6836 f5ec e564 f552 7b06 e640 544b 26b9  h6...d.R{..@TK&.
-0005d540: 304f 65ec 1e98 5be9 caef 98fb 26d2 3419  0Oe...[.....&.4.
-0005d550: ded4 67d4 da43 bdba 745a 37d3 5b1f 74e9  ..g..C..tZ7.[.t.
-0005d560: 6bb8 c1bb 0c85 6c51 1dd6 0fe3 9592 506a  k.....lQ......Pj
-0005d570: d6a7 fa82 ba4e 57a2 91b1 9714 a5e7 3393  .....NW.......3.
-0005d580: a7ee c930 ce2e 750e 3374 7384 599e a65b  ...0..u.3ts.Y..[
-0005d590: cc68 8c54 6a93 1263 721d 662c 99b3 ac63  .h.Tj..cr.f,...c
-0005d5a0: f064 0c53 f50a 5a6d d675 a94b 2a8e d8cb  .d.S..Zm.u.K*...
-0005d5b0: 8c96 8931 2d13 891a fbb2 0c6c d699 42ef  ...1-......l..B.
-0005d5c0: 9f79 6fe2 d815 2bb1 767e 652f d7ce c931  .yo...+.v~e/...1
-0005d5d0: 554c 6c9a bdf0 0e73 d4a6 a3cf ddac 5507  ULl....s......U.
-0005d5e0: 5412 ff9b 1219 ece9 5761 5e35 3bb7 fb28  T.......Wa^5;..(
-0005d5f0: d3f1 ef6e ba4d 9e39 4249 a6ad ca5e 9851  ...n.M.9BI...^.Q
-0005d600: 69ba 49fe 638e 9b16 1155 aa52 a2dd 119b  i.I.c....U.R....
-0005d610: be9e d0ed 72ac 5184 067c 999a 6f99 b58e  ....r.Q..|..o...
-0005d620: 2abc 6863 39f5 bf25 b4a6 7628 3bde addb  *.hc9..%..v(;...
-0005d630: b70b fa39 01f7 bdbb 55f6 bf9a d033 ccf0  ...9....U....3..
-0005d640: e67d 9e6d b558 c339 ea46 b813 1db3 ad52  .}.m.X.9.F.....R
-0005d650: ec83 fada 6329 449a 736c 0713 1a45 a8ca  ....c)D.sl...E..
-0005d660: 2e64 32b8 4e53 8ed5 3ea1 cd96 473a c428  .d2.NS..>...G:.(
-0005d670: f9c0 e4ce ba62 ee88 b28c 63cf f2ab 6dd3  .....b....c...m.
-0005d680: 9aa3 9aaa 8f0a 3bb9 9974 ca2e 899d 9741  ......;..t.....A
-0005d690: 6f5a 29d4 64e4 7d9a 5211 ec3c aed2 3be0  oZ).d.}.R..<..;.
-0005d6a0: 18e4 0ca9 a4fa 9fb7 2cd3 3b65 ab97 27ea  ........,.;e..'.
-0005d6b0: 6724 9d59 b126 e5fc 9cd6 c862 e1d2 6b3c  g$.Y.&.....b..k<
-0005d6c0: 26cf 73dc 194f 247d 7ad0 f15d f83a ef94  &.s..O$}z..].:..
-0005d6d0: 99ac ea3b 3854 5a61 72b4 f92c 7c9c 2ed6  ...;8TZar..,|...
-0005d6e0: b3d0 4a81 f58f 2f6d 3915 7252 8b8b 7e9b  ..J.../m9.rR..~.
-0005d6f0: 457a a35e e197 ab07 0f77 ee53 b903 192d  Ez.^.....w.S...-
-0005d700: db9c 3cb5 8ccd 91bc bbd7 ee58 c71d ec54  ..<........X...T
-0005d710: 271c 31c6 7d57 1e2e b13b fd32 a6ca 9b5d  '.1.}W...;.2...]
-0005d720: bd62 773b 6526 598f cebc 3d2d c6c8 2b2d  .bw;e&Y...=-..+-
-0005d730: f4c4 23b9 4ea5 eb6e 1da4 c2a1 5767 e8d9  ..#.N..n....Wg..
-0005d740: f74d 53fa 259e fa2e e7e0 cc67 59b3 d6f3  .MS.%......gY...
-0005d750: d9f1 0ed5 27e9 84ac f39c be8c 47df f55b  ....'.......G..[
-0005d760: 3c18 6fc5 fda4 1b07 e842 92d9 17cc 9aea  <.o......B......
-0005d770: 3487 2c62 15d6 3717 2b16 3652 c78e 5225  4.,b..7.+.6R..R%
-0005d780: 2f62 5195 2e9a acd7 1dd1 d60c e8e8 1ac5  /bQ.............
-0005d790: 7214 28e9 9bd2 f501 baf2 415d a312 c253  r.(.......A]...S
-0005d7a0: 3a63 0912 7e52 c9a0 ea22 275f 2a47 7cc4  :c..~R..."'_*G|.
-0005d7b0: ce3c 4725 b935 adab 9cd2 41cd 5590 eb9a  .<G%.5....A.U...
-0005d7c0: 934c 1365 5a34 2562 f23a c3c5 a33c 5388  .L.eZ4%b.:...<S.
-0005d7d0: d032 cf5c d4f7 82a6 23e3 b688 a5eb 7573  .2.\....#.....us
-0005d7e0: 19d3 34f9 26e9 c560 60e5 68c7 4bf5 5766  ..4.&..``.h.K.Wf
-0005d7f0: d5bc d665 c5a5 e564 a67e 88ad 31ed fa18  ...e...d.~..1...
-0005d800: e984 921a c464 caa4 fab9 81b2 5e89 bdc8  .....d......^...
-0005d810: 7d8e bb2e cadc b135 0d86 5f3d 850a b7a9  }......5.._=....
-0005d820: 3dab c818 0ce3 a04b 8cbe f0b7 379f b170  =......K....7..p
-0005d830: f534 b62a eb79 659b 9aa5 7ab7 3932 cddc  .4.*.ye...z.92..
-0005d840: 4af1 9ff8 bcda d159 de18 ceb2 0c32 5f87  J......Y.....2_.
-0005d850: a71c 2ba2 d4d5 bdaf c51e 9033 68c5 96a9  ..+........3h...
-0005d860: 4f04 6bc7 5402 97f3 ff45 99e7 63c5 54f1  O.k.T....E..c.T.
-0005d870: 09ac ebfd 75e8 e94e c9ec b6d9 5db5 af2e  ....u..N....]...
-0005d880: e00e 71cb ada3 abd1 e4ff c8c1 2824 d829  ..q.........($.)
-0005d890: 2d94 ae04 98c2 61bf ae4d b2fc 98c6 bcf0  -.....a..M......
-0005d8a0: 23e7 60b1 e8d3 2b19 9a86 9462 df92 6c89  #.`...+....b..l.
-0005d8b0: bd74 6ee5 8e1a ee15 5048 80b5 5d98 74fa  .tn.....PH..].t.
-0005d8c0: f882 10ee 380a 270d fd8f 9433 ebba 4837  ....8.'....3..H7
-0005d8d0: cdb8 16e7 1be5 491d 854e 2227 6590 234b  ......I..N"'e.#K
-0005d8e0: 458a 3293 a9d9 8911 42dd 4ead a69f e4ea  E.2.....B.N.....
-0005d8f0: dc24 b9e7 ead4 2959 24ba 208f 5c8b d060  .$....)Y$. .\..`
-0005d900: 9362 6e7a a5fa 8fa1 7625 1237 86d3 af54  .bnz....v%.7...T
-0005d910: 9593 af17 f534 a508 47ba 6604 bd99 01cb  .....4..G.f.....
-0005d920: 9ca3 13c9 7368 5ed4 b2d7 bf4f ff4f 7ad7  ....sh^....O.Oz.
-0005d930: 8d75 ea6e fa7f d6b9 2320 66cc 38f6 5692  .u.n....# f.8.V.
-0005d940: e52f a62b 16a2 bf4a 6976 3c37 556a 3dd1  ./.+...Jiv<7Uj=.
-0005d950: 692e 4b36 4d8c ad94 121b 3c37 444b 0831  i.K6M.....<7DK.1
-0005d960: efd8 9291 0b9d 7b9b d37a 739f fc6d 1e43  ......{..zs..m.C
-0005d970: d632 b23b b7c8 662c f6ae dfbb 946a 9edb  .2.;..f,.....j..
-0005d980: 2fba 0753 6555 6e6b b676 6bba 7171 5ddc  /..SeUnk.vk.qq].
-0005d990: 1cc5 54d6 53bb a992 2b9b 7337 eb31 19d9  ..T.S...+.s7.1..
-0005d9a0: 51d2 ba17 cfba 3944 63b6 d9c7 e82f fa85  Q.....9Dc..../..
-0005d9b0: 9456 e14a 862e 3735 4c49 3090 3297 a0dc  .V.J..75LI0.2...
-0005d9c0: 853c 197b 8b73 6679 0b44 2f49 6318 18f3  .<.{.sfy.D/Ic...
-0005d9d0: 9db6 d624 8d5d 3b32 bb7c c473 dbaa 31a7  ...$.];2.|.s..1.
-0005d9e0: ad7f ccd7 33ed 7597 b2de 172d 1d4f ca9a  ....3.u....-.O..
-0005d9f0: 7817 c574 7a14 7253 f7d0 6f06 fa6d 6634  x..tz.rS..o..mf4
-0005da00: 9c43 f4e0 cdaa 779b 8e92 6656 ed73 e9db  .C....w...fV.s..
-0005da10: 2ed7 bba4 0185 4613 82c6 de88 c062 9cd3  ......F......b..
-0005da20: 4ad0 d24f f35c 2eb2 cbea c45d f7f5 ab94  J..O.\.....]....
-0005da30: ce4d 5d58 7494 5b91 2dbb c2a5 738e 706c  .M]Xt.[.-...s.pl
-0005da40: f493 d477 6635 cffe d23e a9d1 aed6 3960  ...wf5...>....9`
-0005da50: 692a c6d8 bb0c 913d c7b8 63c1 8367 de18  i*.....=..c..g..
-0005da60: a7ba 1c8b 8be1 debf 3587 ce0e e6d6 ab4e  ........5......N
-0005da70: 89f4 7b71 a763 2f7d bcce face 7655 cccf  ..{q.c/}....vU..
-0005da80: f967 cf31 0915 f47e a4cd f6cf ee4b 482b  .g.1...~.....KH+
-0005da90: 05bc a289 6b50 4ee9 3c58 689e 0673 872f  ....kPN.<Xh..s./
-0005daa0: 745f aad6 5d97 b64c 5968 789b d306 c54b  t_..]..LYhx....K
-0005dab0: 1805 f6cd f2f0 ff98 de64 b5c6 2182 c769  .........d..!..i
-0005dac0: 18f5 f5be 66b2 ac82 6bdb b28e d2a9 fb5c  ....f...k......\
-0005dad0: 8547 a15b ad9e b680 7a1a 6e87 53ef 5668  .G.[....z.n.S.Vh
-0005dae0: a23a ce6c 79f3 7c33 6e2d 402f 4267 d970  .:.ly.|3n-@/Bg.p
-0005daf0: e21c 33b6 2d8e e0a3 e34a 6f5e c058 a75c  ..3.-....Jo^.X.\
-0005db00: 9250 265f 8b2b 4c72 7ae4 2aff eb7a 181d  .P&_.+Lrz.*..z..
-0005db10: ccdb 5af7 eca5 804b 03ec 5e5a 7989 045b  ..Z....K..^Zy..[
-0005db20: ebeb 1302 cd34 842b dff6 ccc7 6eac 8a5f  .....4.+....n.._
-0005db30: d771 38b7 7fee 1d0e c995 a295 9713 45b4  .q8...........E.
-0005db40: 7aac 438b 9dbe fd61 c7d6 4728 2c54 ef85  z.C....a..G(,T..
-0005db50: f52d 8502 13b4 2e32 ee85 974a 6996 7904  .-.....2...Ji.y.
-0005db60: 1f6d b6aa a37f 746b b2cf d2f9 dd67 854a  .m....tk.....g.J
-0005db70: 1ccf 7393 1371 6462 d171 d1a8 8f6f 39bc  ..s..qdb.q...o9.
-0005db80: 4a6f c562 b587 ecbc 61c7 932d 3e45 2fef  Jo.b....a..->E/.
-0005db90: 86c2 d972 2cae 2def 13fe c4b3 8cd1 39c6  ...r,.-.......9.
-0005dba0: 681b 6a75 cdf4 5d3e a0f5 aa4e 5ab7 99d3  h.ju..]>...NZ...
-0005dbb0: d931 b79c eb76 9a5b eb83 a3ea 617f 07c3  .1...v.[....a...
-0005dbc0: deb1 9236 1ee1 d440 982d 5e71 0dd9 cb3a  ...6...@.-^q...:
-0005dbd0: 5976 43a4 eb96 549c 97cb 1ee0 cdcb f552  YvC...T........R
-0005dbe0: de7d 9571 bb40 a41e 72b5 1b67 e292 9115  .}.q.@..r..g....
-0005dbf0: c373 8fad 560b 1965 512e d793 d5e5 59a7  .s..V..eQ.....Y.
-0005dc00: 544f d165 1843 e9b0 cd62 f1d9 3cfd b8e8  TO.e.C...b..<...
-0005dc10: 2eed e403 aff4 cf58 fbeb 3aee c45c b3ce  .......X..:..\..
-0005dc20: 4a8c 1dda 1ed6 f5b1 5da4 95c6 fa12 7da3  J.......].....}.
-0005dc30: c050 995b 1670 5bc6 ceec 30fb 34da ebac  .P.[.p[...0.4...
-0005dc40: 350a a073 5e44 afcc af58 6fa5 56a4 b173  5..s^D...Xo.V..s
-0005dc50: 14bc 4ad3 3bde 4ab7 478b 2bf1 3b1e 9e93  ..J.;.J.G.+.;...
-0005dc60: 0328 1ff1 2df7 15c9 3b2c 64e0 0dd3 8e47  .(..-...;,d....G
-0005dc70: 4b42 fbd9 11f9 1b02 5939 a7ec 85ad c45e  KB......Y9.....^
-0005dc80: 53df de59 91ca b0aa 137b 3e4c e19f e3b3  S..Y.....{>L....
-0005dc90: dd1f 1061 dd5b 3e99 0f3a 558d da7b 832f  ...a.[>..:U..{./
-0005dca0: e6d0 a73d 3d30 fc90 cee0 ab0f 0bff 9696  ...==0..........
-0005dcb0: f1a9 2159 2d06 117a 1512 cf7d abcf 75ef  ..!Y-..z...}..u.
-0005dcc0: 693e bc0a a31b cf1e 889b 7d5a 539a c5ab  i>........}ZS...
-0005dcd0: ed02 4ee7 7ff4 c09e b334 6771 cada cbee  ..N......4gq....
-0005dce0: 7b4d 242a 2351 3e96 19f3 dccf 2a2e bc04  {M$*#Q>.....*...
-0005dcf0: adea 16fb c03e 909b bef7 e120 62ba aa03  .....>..... b...
-0005dd00: 17fe 2966 fff8 0eca 87f8 766a 2894 9a42  ..)f......vj(..B
-0005dd10: f9b9 ffc2 f765 84b8 8f43 eb63 ffcb 54e9  .....e...C.c..T.
-0005dd20: 3f58 f6e0 7f6f 0f71 5763 fc9c ae08 cc9b  ?X...o.qWc......
-0005dd30: c148 9bee 0051 1faf a28f efa9 9fd9 3b74  .H...Q........;t
-0005dd40: fb5d 4031 44ab 406f 11e5 0f52 323f e3f7  .]@1D.@o...R2?..
-0005dd50: 3baf 4feb 5595 ed73 a4c1 beba 8ffc dda9  ;.O.U..s........
-0005dd60: 76e5 f8a8 508c f2af f004 f3f3 d8b3 a2f6  v...P...........
-0005dd70: 6608 9be2 9e2f 2244 a331 81bc efbc 29db  f..../"D.1....).
-0005dd80: ebbf 2b11 a46e 3990 761d 7546 2c15 ef5b  ..+..n9.v.uF,..[
-0005dd90: 47c8 db28 0f84 1dcb c4b9 2c9d 78dc e1af  G..(......,.x...
-0005dda0: aa85 bf63 f761 0432 ebcb 7dc9 b59b dd48  ...c.a.2..}....H
-0005ddb0: 1f13 35ce ec7c 10ef b28a 27c5 e486 5e5f  ..5..|....'...^_
-0005ddc0: 12f2 eba5 0efa ff19 75b1 9375 9fab 4229  ........u..u..B)
-0005ddd0: 866c 8fe4 4e72 bdd6 15d7 ec25 f1b2 614b  .l..Nr.....%..aK
-0005dde0: a8d6 ff44 39dc b773 18d0 0fb2 0ebf dd9b  ...D9..s........
-0005ddf0: fe7c edf0 817f c3d1 bff4 7eee 8007 f7f2  .|........~.....
-0005de00: 25f1 35ee 3aa8 c894 618f 3ea8 6dcd a55e  %.5.:...a.>.m..^
-0005de10: a148 7fc4 59f6 1d72 a716 dbb2 ae97 1f73  .H..Y..r.......s
-0005de20: 9494 efec f2a0 7e95 6d86 287d e2c7 1575  ......~.m.(}...u
-0005de30: 9aef a435 66e9 a9e9 d501 138f f55b abe7  ...5f........[..
-0005de40: 9222 58ef 916f e491 2792 68dc c79c e41c  ."X..o..'.h.....
-0005de50: 1965 9e2f d9bf 49f3 53f9 707e 3279 8b7c  .e./..I.S.p~2y.|
-0005de60: 470c 6b01 b9fa 687e 4c59 b941 a920 c80f  G.k...h~LY.A. ..
-0005de70: 4cf5 d7e1 91ea 9f7b becc ebd1 00c5 75e8  L......{......u.
-0005de80: 2a14 813f 37ed 6dfa 5674 53bf 98ab f23b  *..?7.m.VtS....;
-0005de90: 339a 25bd 1bf7 8dae 7bb4 fb39 faf6 8e6d  3.%.....{..9...m
-0005dea0: 748e e742 f402 df8c 67c5 1ffb 93de 511d  t..B....g.....Q.
-0005deb0: ee83 523b f8ab f0f9 ed9a 7a47 402e 9a02  ..R;......zG@...
-0005dec0: 7eb4 3301 b399 a353 4fbc ed8f 8e39 9ede  ~.3....SO....9..
-0005ded0: 43b4 fb4f fe77 b781 73ee 1046 b4a2 357b  C..O.w..s..F..5{
-0005dee0: c124 fff4 a052 1dbe d1be 7d05 c7c7 13fb  .$...R....}.....
-0005def0: 4fcd 96d7 d6e7 3ebe 6fa8 b3e6 0a29 dfb6  O.....>.o....)..
-0005df00: b1cf 9f40 9ce2 bb97 c7c5 f2fa b52b 8e3e  ...@.........+.>
-0005df10: 2fe3 977b 8391 76d5 311b a0ff ab78 ef17  /..{..v.1....x..
-0005df20: af4a 4b0c be26 c33d 152d af19 c310 72c8  .JK..&.=.-....r.
-0005df30: 4291 7a8d 88f4 1aa1 d9fb 40ff 2110 178f  B.z.......@.!...
-0005df40: f2c7 edef 94fb a330 34fd 256f d793 21a6  .......04.%o..!.
-0005df50: f794 a965 e5f7 103f b4d5 fa7f 5f0a 213f  ...e...?...._.!?
-0005df60: ef6c 61d4 216b 3634 40c5 620b ed4d 7c8f  .la.!k64@.b..M|.
-0005df70: 9f91 e159 5fa6 7c1a 9475 f08e a587 b392  ...Y_.|..u......
-0005df80: 741c fa45 9c04 4d31 37f1 4a2e 2f2d 8ff3  t..E..M17.J./-..
-0005df90: 425f 9bde ae78 877c de68 b40f 5edd 04e2  B_...x.|.h..^...
-0005dfa0: 0e96 17f2 cbdc 2ac4 cf96 7b2b a29e 278c  ......*...{+..'.
-0005dfb0: 3251 7f7c 4c7b f05e ce98 1ff2 6db9 0ce2  2Q.|L{.^....m...
-0005dfc0: efa6 fbbc c7ec 1251 dfc3 f1e2 67df 64dd  .......Q....g.d.
-0005dfd0: 2343 45dc 0e1a aea9 fef1 2b65 a165 2b84  #CE.......+e.e+.
-0005dfe0: e7e0 3ebc e029 23f7 0578 533f b6bb 530a  ..>..)#..xS?..S.
-0005dff0: aa5d 0ab6 ec51 b69d 5e08 1f0a 20eb fd94  .]...Q..^... ...
-0005e000: b477 dc7f c747 3fc5 e854 a26d ef95 4dd3  .w...G?..T.m..M.
-0005e010: a5ef 241f 6bbb e3fb 39b9 b928 43ba 1f08  ..$.k...9..(C...
-0005e020: b8f8 467c 749c 7a8c d6b6 f7da b8cc d25d  ..F|t.z........]
-0005e030: 45f9 a7ab 4151 a839 97a1 805e 7340 4114  E...AQ.9...^s@A.
-0005e040: 77e3 8329 96d7 d7d8 b5c4 381d 75ac 858a  w..)......8.u...
-0005e050: 6837 bbad cfa9 69ba 9f06 6e16 c67c d425  h7....i...n..|.%
-0005e060: 3c52 df33 895d 43d7 8840 af84 7ccf 1693  <R.3.]C..@..|...
-0005e070: ef63 29c4 db86 d7ef 318d 7dc0 5dbc abe2  .c).....1.}.]...
-0005e080: 6242 7b7f acf9 1503 26af e43b 8b2f f8e2  bB{.....&..;./..
-0005e090: 2fbe e28b fef9 86e6 f185 c779 31e8 252d  /..........y1.%-
-0005e0a0: ec0f 9fbb 4010 a9a8 01be b8f7 ba21 d162  ....@........!.b
-0005e0b0: f1af 2af5 ef00 27fd d9be e369 c7f9 c899  ..*...'....i....
-0005e0c0: 4c08 ff12 4e54 f60e dbb8 7ed6 90ef 2fbe  L...NT....~.../.
-0005e0d0: e28b bef8 8b2f f8e2 2fbe e28b bef8 8b2f  ...../../....../
-0005e0e0: dae7 8624 3f87 10c7 10b1 351e 7828 f0bd  ...$?.....5.x(..
-0005e0f0: 00de 77f3 12ec c148 a793 7cea 7ed2 f8c2  ..w....H..|.~...
-0005e100: 2fbe e28b bef8 8b2f f8e2 2fbe e28b bef8  /....../../.....
-0005e110: 9f2f 5195 6c1f f4c0 4254 059b 8124 9019  ./Q.l...BT...$..
-0005e120: b8fd bf3f a889 c866 a20a 3270 5217 a642  ...?...f..2pR..B
-0005e130: 6405 c71a 8a8a e014 ffc9 8e15 328c e2fa  d...........2...
-0005e140: 7151 011d 7070 43a9 6077 bbe7 260c 5fad  qQ..ppC.`w..&._.
-0005e150: 1038 f0b7 3afe e101 8de1 d5e1 f904 5600  .8..:.........V.
-0005e160: 5763 9d4f c207 41dd d380 b9b6 6a70 c011  Wc.O..A.....jp..
-0005e170: 1872 a0ac 0dac 8525 8c76 9e09 0f21 30ac  .r.....%.v...!0.
-0005e180: 4d1c bb65 42f2 4dd0 0217 05e4 1925 df11  M..eB.M......%..
-0005e190: 3a67 e094 e180 221c 7422 3e30 40f1 68f0  :g....".t">0@.h.
-0005e1a0: e583 ebd5 919a 533e bec9 0227 a2df 8683  ......S>...'....
-0005e1b0: 190c 0b8a 0c93 2750 1590 32d8 a060 2e7e  ......'P..2..`.~
-0005e1c0: 6b6c 12c0 e02d 03bc 3c78 140e ce90 4ade  kl...-..<x....J.
-0005e1d0: 4010 6a8c 1a2e f8bd 9c26 c025 80c8 7029  @.j......&.%..p)
-0005e1e0: c3e8 3c26 205a 7b52 fcfd 8c2d 08b8 2228  ..<& Z{R...-.."(
-0005e1f0: 07b2 0d4e 42c8 05b3 1ad0 c262 43dd 1702  ...NB......bC...
-0005e200: c271 86b6 1e2c 0a89 8aa2 a123 1311 2110  .q...,.....#..!.
-0005e210: 8ea0 7026 d0a8 f040 2594 0671 210f 4a80  ..p&...@%..q!.J.
-0005e220: 2540 e0a0 3bde 0676 7ebb 42f8 a0e0 e066  %@..;..v~.B....f
-0005e230: 11a2 1b7e 1420 4f12 68c3 2d41 f811 f06e  ...~. O.h.-A...n
-0005e240: 8a1b 0cbf 027f 52d5 011b ce91 2f0b 8666  ......R...../..f
-0005e250: 074c cf02 28c3 9982 aef0 3f21 4f0b 0e04  .L..(.....?!O...
-0005e260: 5363 1801 af70 5921 7e0b 16ec 44e8 02b3  Sc...pY!~...D...
-0005e270: 342c 4e12 5017 8650 7c42 1a41 6900 4e7e  4,N.P..P|B.Ai.N~
-0005e280: 187f 6270 8582 8623 1b58 c5d0 0d55 f137  ..bp...#.X...U.7
-0005e290: 41c1 0657 853f da35 0c08 7c84 07d5 167e  A..W.?.5..|....~
-0005e2a0: 9491 5703 1705 9f70 d90c 0a0d 390a fda7  ..W....p....9...
-0005e2b0: c12f 7143 68aa 7822 9063 4157 0835 5057  ./qCh.x".cAW.5PW
-0005e2c0: 03ba 4811 2264 60c4 2046 3bc2 1808 5a22  ..H."d`. F;...Z"
-0005e2d0: 3c05 0fc6 b146 9c20 2a88 840c c84c c322  <....F. *....L."
-0005e2e0: 9641 4500 9a81 0919 e34f 0b4e fcc4 0ea4  .AE......O.N....
-0005e2f0: a105 77fd 0586 00d6 0147 7e6f a70d 1009  ..w......G~o....
-0005e300: a157 c290 c904 c043 ae70 2a21 2f1b 070d  .W.....C.p*!/...
-0005e310: 9a30 5903 5e21 134e 4fc0 2a2c d198 38f8  .0Y.^!.NO.*,..8.
-0005e320: 0c1d 4e84 4a80 d428 3144 8655 0395 1434  ..N.J..(1D.U...4
-0005e330: bf26 0183 1c6f f02a 834d 7e18 32fc 39d0  .&...o.*.M~.2.9.
-0005e340: c26f 0abc 9d80 0cbb a2c8 be47 835e 85bf  .o.........G.^..
-0005e350: 5e90 d0f9 5650 f1a7 0425 1164 8158 188c  ^...VP...%.d.X..
-0005e360: 8a4a 32d0 26b8 dd95 8583 1c50 f9c7 0d80  .J2.&......P....
-0005e370: 0075 ca67 bc81 386b 433b 2623 f016 f044  .u.g..8kC;&#...D
-0005e380: 60c7 0d6c f0a3 6175 058e 6292 c0b5 90c5  `..l..au..b.....
-0005e390: 3c28 2218 ed25 eff6 040d 84b3 1b7c 0a48  <("..%.......|.H
-0005e3a0: 13a0 6410 86df 1d32 f012 f359 3818 6d8d  ..d....2...Y8.m.
-0005e3b0: 6705 f4e9 a600 8f02 4294 c2c1 0dac e6fa  g.......B.......
-0005e3c0: b110 4c82 3210 d68d 2201 107c c740 0e5a  ..L.2..."..|.@.Z
-0005e3d0: 8523 8375 b889 212c 50f0 f035 ca1b 6f0b  .#.u..!,P..5..o.
-0005e3e0: 500c 2a16 322a 9840 d022 0812 4607 a384  P.*.2*.@."..F...
-0005e3f0: 6e03 35c1 eb23 5507 7989 2544 6efd 9e2a  n.5..#U.y.%Dn..*
-0005e400: 38ec 771a 1405 5241 4260 199a 68b8 8d29  8.w...RAB`..h..)
-0005e410: 048f 0c9f 8dcb 8b16 e4c0 3b14 9e84 c42f  ..........;..../
-0005e420: af2b bc3d 3afb 3938 1510 2914 e180 59ae  .+.=:.98..)...Y.
-0005e430: 341b e70e a6e2 8a3f 39d8 0cec 769a e204  4......?9...v...
-0005e440: a882 b085 2119 4181 d434 5217 e1ba 80b1  ....!.A..4R.....
-0005e450: 80bc 102b 813a e291 43d9 0a5a 7cc5 20a8  ...+.:..C..Z|. .
-0005e460: bcc3 9204 b4c2 5c82 0d62 2038 8d50 911e  ......\..b 8.P..
-0005e470: f7f2 fc9d c036 4702 29d0 c3c1 a261 88e0  .....6G.)....a..
-0005e480: 5c40 aa61 c101 fe67 20d4 1002 c33c 3623  \@.a...g ....<6#
-0005e490: a30b c85d f08a 11fe b481 a163 30ab 7d25  ...].......c0.}%
-0005e4a0: 8982 9718 4eb3 53ff 8703 0c66 f8bb 1b4d  ....N.S....f...M
-0005e4b0: 06b8 f89d a420 81c4 0a03 601f 1ca2 a015  ..... ....`.....
-0005e4c0: 2851 532a 99f8 6e02 0bfc 0482 0766 3711  (QS*..n......f7.
-0005e4d0: d760 7042 dc6e 1805 3a01 5f07 e042 a8e0  .`pB.n..:._..B..
-0005e4e0: 8f0c d0cb 6061 a706 91e5 c195 1a32 470c  ....`a.......2G.
-0005e4f0: 980a b74f 6e01 260c d240 564c 5d43 3220  ...On.&..@VL]C2 
-0005e500: 99eb 6881 8912 690b 0681 5130 2d1c 3ad4  ..h...i...Q0-.:.
-0005e510: af50 2243 1acb 7839 6f88 ace1 e02b e5cb  .P"C..x9o....+..
-0005e520: da10 9c35 6835 b822 d485 751b 61ce 0284  ...5h5."..u.a...
-0005e530: 42c8 8dbc 0590 d83d 242d 4213 de09 9218  B......=$-B.....
-0005e540: c01a e070 38a1 e268 3f28 0d29 0428 2858  ...p8..h?(.).((X
-0005e550: 1a55 0d6e f067 49c0 4785 0891 5c20 500a  .U.n.gI.G...\ P.
-0005e560: 3f36 1a19 05ac addf 3223 7e83 eec2 1317  ?6......2#~.....
-0005e570: b683 37e0 5e07 4f0d 41ce ef8f 0ac8 1aea  ..7.^.O.A.......
-0005e580: 7120 0782 efa0 31be 5061 0453 8d47 a044  q ....1.Pa.S.G.D
-0005e590: 7e4f 3b1b f3b0 11fa 7605 c585 14b0 20b8  ~O;.....v..... .
-0005e5a0: 804a c009 fcec 709e 829b 4199 c154 0754  .J....p...A..T.T
-0005e5b0: 956b b082 9a0d e0e5 0566 a2b2 82d7 0df4  .k.......f......
-0005e5c0: f01b 0c68 5148 c13e d900 5880 37d7 9086  ...hQH.>..X.7...
-0005e5d0: c91d 930b 9102 18b1 a87f 76c4 0827 355c  ..........v..'5\
-0005e5e0: 70a1 3440 fc79 2038 ab0b 5a1a af70 1511  p.4@.y 8..Z..p..
-0005e5f0: 4a12 fc24 7b33 b304 204b e89d 0c00 0b64  J..${3.. K.....d
-0005e600: 160f 167c 62e0 0582 c080 9603 84b9 c031  ...|b..........1
-0005e610: b8d9 a00c 16e8 85fd 35bc 6961 2b2c 3984  ........5.ia+,9.
-0005e620: a8bd ee28 5402 2f38 cca0 2b82 005c 8e48  ...(T./8..+..\.H
-0005e630: 0d01 c271 1950 b87d c3d8 014e 8343 7187  ...q.P.}...N.Cq.
-0005e640: 20a9 aeeb 261d 7811 6115 8aa0 6570 b304   ...&.x.a...ep..
-0005e650: 53e1 e802 1b0f a2b0 a00d 5d5f 0741 5820  S.........]_.AX 
-0005e660: 05dc ee90 7a41 2b2c 1f10 0823 85a4 1004  ....zA+,...#....
-0005e670: c2e0 e202 b618 9251 0e8d 2b22 a949 c179  .......Q..+".I.y
-0005e680: 5c07 14d8 7100 8cdd 2d60 d902 7321 d361  \...q...-`..s!.a
-0005e690: 3682 e0b9 402d 5096 5252 2f71 d9c0 46b0  6...@-P.RR/q..F.
-0005e6a0: 1c1b 300a 4dd8 421b 300c 5c50 686d 0f25  ..0.M.B.0.\Phm.%
-0005e6b0: ce15 0724 4640 153e 3b54 7120 85df 2310  ...$F@.>;Tq ..#.
-0005e6c0: e7a8 419a d802 3817 fa2a 030c 8253 84ea  ..A...8..*...S..
-0005e6d0: 37fc 0950 d8d0 8161 b08c 8b4f 750b 880b  7..P...a...Ou...
-0005e6e0: 142e 87dd a2f1 a807 3664 d88d 6381 75f1  ........6d..c.u.
-0005e6f0: af71 beb8 e0e6 aa81 0e00 bafd e081 89b8  .q..............
-0005e700: 1ae1 e058 cc81 53e0 87a0 1842 23af 8149  ...X..S....B#..I
-0005e710: 087a 260b a888 9c32 1234 5f46 ac0b 1330  .z&....2.4_F...0
-0005e720: 6786 2807 aab0 7d41 c9ef 48f9 920d 1d06  g.(...}A..H.....
-0005e730: 5cd8 a007 2064 9029 4848 623d 181a 5cc8  \... d.)HHb=..\.
-0005e740: 0246 b0df 8c51 33fd 90ab 46c0 888d 4ca0  .F...Q3...F...L.
-0005e750: 4ff6 f8ba 4f38 e101 7f0f 0210 0862 023b  O...O8.......b.;
-0005e760: a9e6 d040 2e84 0c6e c112 c32b 021e 1956  ...@...n...+...V
-0005e770: 08be 4709 60a0 54d3 1532 41a0 0970 026e  ..G.`.T..2A..p.n
-0005e780: 5230 67c1 9a5c a870 4083 58f1 4161 0a49  R0g..\.p@.X.Aa.I
-0005e790: f021 40ac 1cc2 d005 80c8 800c 44f0 215a  .!@.........D.!Z
-0005e7a0: c2c2 bf08 9076 c035 5018 869f 83be 1b12  .....v.5P.......
-0005e7b0: d8f0 b280 3fa1 900d 5207 c32f 4166 7060  ....?...R../Afp`
-0005e7c0: 20ae 19ea 757d 15a6 481d 6e2c 98c3 023c   ...u}..H.n,...<
-0005e7d0: f180 405e 3b7c 85a9 f1b7 8a0e 19d0 2b24  ..@^;|........+$
-0005e7e0: 5c58 5643 5afc 223e 003c d765 9c24 a024  \XVCZ.">.<.e.$.$
-0005e7f0: b8df c109 032f 4525 0952 3dd8 877d 1808  ...../E%.R=..}..
-0005e800: 05bb ea7b 3540 1b10 f0b7 32b8 59d8 8160  ...{5@....2.Y..`
-0005e810: 00da 4160 f859 d5c8 66a0 68fe 620d b704  ..A`.Y..f.h.b...
-0005e820: 51e2 30c1 3ca3 42c3 16ee 41d0 2b28 5e70  Q.0.<.B...A.+(^p
-0005e830: e381 12c3 628d cbc0 90f3 30d8 fb7a 81b0  ....b.....0..z..
-0005e840: c1b1 d88c 4d6e 38f7 be0d c184 48c3 ea23  ....Mn8.....H..#
-0005e850: b80e f86e 4711 0cbf b67d 3ba9 a806 2b8c  ...nG....};...+.
-0005e860: 69e1 b827 a010 01ed 7637 2128 061d a2b2  i..'....v7!(....
-0005e870: 9cac a024 049f 430c 814c 2ce6 942d a027  ...$..C..L,..-.'
-0005e880: b095 0a69 2a30 f296 83b0 c80c a129 d88a  ...i*0.......)..
-0005e890: e00a 1b3a c018 0da8 5afb d8fc 0156 d0d7  ...:....Z....V..
-0005e8a0: 85b8 c0c5 8817 1c3f 811a 3524 76e3 6521  .......?..5$v.e!
-0005e8b0: a1fe 7110 06a6 e627 4853 2265 8210 798b  ..q....'HS"e..y.
-0005e8c0: 00a9 2163 d6b0 d334 82bf 0007 1958 ec73  ..!c...4.....X.s
-0005e8d0: 0c30 14c6 f21f 680d 4402 911f 72a2 689a  .0....h.D...r.h.
-0005e8e0: fc2a 1c36 c3a0 c3b5 8264 86ee 33fc 34c0  .*.6.....d..3.4.
-0005e8f0: 7e12 0e19 4b03 cd6b 4c1a 2406 811d 80a9  ~...K..kL.$.....
-0005e900: 9327 ca16 2014 dd73 9086 85a9 5c7b 0cd8  .'.. ..s....\{..
-0005e910: a480 5c3c 3460 2202 a800 be28 4d98 fdcb  ..\<4`"....(M...
-0005e920: 20e0 94e1 c704 dcec c000 b402 3c10 2806   ...........<.(.
-0005e930: fd13 8405 3271 7e25 a396 967f 918a 45c5  ....2q~%......E.
-0005e940: 0785 abeb 1d1c bec7 e014 bea0 905a 0751  .............Z.Q
-0005e950: 153e 5560 3e8b 410c 3e77 3a7c b270 be9f  .>U`>.A.>w:|.p..
-0005e960: 0016 beba 305b 8757 163e c690 3e21 e016  ....0[.W.>..>!..
-0005e970: 3e71 2e7c 5c80 33b4 0cb9 f988 2c60 84d1  >q.|\.3.....,`..
-0005e980: a3a4 2090 675b e747 b5c7 4a6d a584 b2a6  .. .g[.G..Jm....
-0005e990: 1390 342d 92b8 968a eab1 9948 dce6 2511  ..4-.......H..%.
-0005e9a0: a851 a851 119d e4ec 40ee 9aba 3523 b9bc  .Q.Q....@...5#..
-0005e9b0: be4a a6ce 84c7 46d2 c5f0 a922 192e 245e  .J....F...."..$^
-0005e9c0: af8e 4986 670f e763 57e2 6bd0 a4df aec1  ..I.g..cW.k.....
-0005e9d0: e5b3 4f2b 3259 1fd3 6aa2 9300 c7bc 7d76  ..O+2Y..j.....}v
-0005e9e0: 1e47 020b 1d64 905a db63 853a 08d2 17a1  .G...d.Z.c.:....
-0005e9f0: a199 7c51 aaf4 9228 3cdc 0ad9 3444 9860  ..|Q...(<...4D.`
-0005ea00: e683 280b 0054 469f 9304 62b2 d262 9960  ..(..TF...b..b.`
-0005ea10: 8814 49b3 431a 85aa 2449 7e4a fd88 1011  ..I.C...$I~J....
-0005ea20: 8578 ed5f 50ab 178f fe5f 6ade 4bc5 1815  .x._P...._j.K...
-0005ea30: 3549 233a 9607 c4b8 2b66 ce46 a050 a372  5I#:....+f.F.P.r
-0005ea40: 457c ecc5 44ed 44bc 99d7 6934 0332 546e  E|..D.D...i4.2Tn
-0005ea50: 2231 56d6 db88 5ba8 894b ec7d 11ab 3fc9  "1V...[..K.}..?.
-0005ea60: ec90 e34b 3917 347a 6763 c12e 6684 373f  ...K9.4zgc..f.7?
-0005ea70: 5346 8519 1f5a 855b 1b95 19a4 1f82 e3de  SF...Z.[........
-0005ea80: ccb8 cfa3 a182 124b 89fd d033 af70 e6be  .......K...3.p..
-0005ea90: 961a 26a9 7a48 240d 46ec ecec 239d 6eda  ..&.zH$.F...#.n.
-0005eaa0: e4aa f951 5e6d 9748 888f 473b 657d 6051  ...Q^m.H..G;e}`Q
-0005eab0: 2948 aeb3 d173 3216 7a1d 5644 ecd5 42e7  )H...s2.z.VD..B.
-0005eac0: f73c 8989 1a3f 6a92 adeb 47c9 5c67 75d7  .<...?j...G.\gu.
-0005ead0: cc81 bc8b 657e 6be4 7a12 ac43 4a5f 1a4a  ....e~k.z..CJ_.J
-0005eae0: ff46 376e da1a be52 7ace 898d 7436 c8bd  .F7n...Rz...t6..
-0005eaf0: 2628 47a6 921d 8543 6890 98f8 044e 5cc9  &(G....Ch....N\.
-0005eb00: fdf0 d00c b42c 2981 6e8c 7649 6020 dc88  .....,).n.vI` ..
-0005eb10: 7589 914e b64b aec4 0a15 b753 cb14 d168  u..N.K.....S...h
-0005eb20: 3879 d58c 72c2 7154 98de 4135 d2c3 b164  8y..r.qT..A5...d
-0005eb30: b481 f3ef f502 926b 46c7 91ae 1d13 ba41  .......kF......A
-0005eb40: 5349 6082 4158 b8e8 2c29 2ca8 3a5b 64e9  SI`.AX..,),.:[d.
-0005eb50: a691 62cb 03b3 29ce 6294 8d32 9a4f 4c81  ..b...).b..2.OL.
-0005eb60: 1b45 9961 3043 a468 6282 1513 2cfa ce86  .E.a0C.hb...,...
-0005eb70: 3c4f ac47 63b4 29ba d280 08e4 2e9e 64d2  <O.Gc.).......d.
-0005eb80: f8eb c8da 3b17 11ca 7525 b001 e768 cd0b  ....;...u%...h..
-0005eb90: 561e 34c8 406e 8e25 73ed f495 84a1 134a  V.4.@n.%s......J
-0005eba0: 62ae cad4 04c8 69a0 3f66 2c0b 8d99 a0d5  b.....i.?f,.....
-0005ebb0: 5b89 cb6e dc27 50c3 239a a5ae 5f46 0b9a  [..n.'P.#..._F..
-0005ebc0: cecc 7800 97ef c6e6 3579 649e b613 a40c  ..x.....5yd.....
-0005ebd0: 4ed0 3ec7 3083 8f8f e787 1049 2037 3187  N.>.0......I 71.
-0005ebe0: 36ee 7cc3 44dc 5ac6 cbac f3b4 b0e6 d9b1  6.|.D.Z.........
-0005ebf0: 6f5a 2773 4b93 2451 54f1 940c 34c9 dc6e  oZ'sK.$QT...4..n
-0005ec00: 92a0 8b6c 8c0a 035e f466 3c08 b38e eaa8  ...l...^.f<.....
-0005ec10: 8ac1 2678 33a5 a354 098c 80ca ac97 f411  ..&x3..T........
-0005ec20: c0cd 2723 489f 362c e8cc 2483 8922 aa95  ..'#H.6,..$.."..
-0005ec30: d3f7 cf3e 2489 2b18 3051 4bb3 3028 c4c8  ...>$.+.0QK.0(..
-0005ec40: f692 b9fa 38a6 2a33 ea0f 58a9 c79a b006  ....8.*3..X.....
-0005ec50: 092a 9ca1 4db5 2167 4351 723d 4865 2a9b  .*..M.!gCQr=He*.
-0005ec60: 5307 7b12 3d37 4dcf c3a2 675a 62fb ebd8  S.{.=7M...gZb...
-0005ec70: 3e36 8d1a 833e f1ec 6f36 191a fe29 89ec  >6...>..o6...)..
-0005ec80: c9f2 e0bc d462 30a1 2ce4 8893 1f43 837a  .....b0.,....C.z
-0005ec90: 1bf1 4a1b 5ca9 3141 0f36 74bd 49a9 fb8f  ..J.\.1A.6t.I...
-0005eca0: b870 9ddb 4a8d 6ad0 98f4 ea22 4dc6 2f4a  .p..J.j...."M./J
-0005ecb0: b1b3 6bde fa8e 3a8b 78f2 1599 4d7d aaca  ..k...:.x...M}..
-0005ecc0: 98ce 464d d0a3 96b0 67cd d179 73ac 1441  ..FM....g..ys..A
-0005ecd0: 271c b7f3 5440 7a2e 66c2 77a2 ebe8 ca7b  '...T@z.f.w....{
-0005ece0: e401 7359 9b5a e72f 319d 41f7 679e 4d9e  ..sY.Z./1.A.g.M.
-0005ecf0: c7f6 7b5e 55af b940 08cf 5f8c 4bfd 7b35  ..{^U..@.._.K.{5
-0005ed00: a0a3 bbfc 0e3b 3bc5 63be 48a3 c10b e1c6  .....;;.c.H.....
-0005ed10: 7840 e4e8 6743 4228 d052 a75d b8dd 2de1  x@..gCB(.R.]..-.
-0005ed20: 6173 4c30 b40b d009 833a 7d25 a44f 076f  asL0.....:}%.O.o
-0005ed30: 6899 0698 8f6a 2349 9109 2631 3b79 0e1d  h....j#I..&1;y..
-0005ed40: 05a8 4412 779b aad6 701c 842c 5e22 6ae5  ..D.w...p..,^"j.
-0005ed50: 4654 a821 f851 1c86 e855 d1b3 b4e7 c452  FT.!.Q...U.....R
-0005ed60: dba3 542a ce59 68ce ac81 97aa a25f 03df  ..T*.Yh......_..
-0005ed70: 9c26 a723 cf72 c045 7a86 0e57 edcb 8e0a  .&.#.r.Ez..W....
-0005ed80: 36ec 6daa d606 34f3 707a be5d 92d2 6eef  6.m...4.pz.]..n.
-0005ed90: f4a3 ad61 29e5 b49d 9086 d564 a15b b513  ...a)......d.[..
-0005eda0: 47c2 5769 ed00 e2a4 f559 bdbd 4c2a 0709  G.Wi.....Y..L*..
-0005edb0: ec82 54bd 5aad 6ade 13d4 f944 2e75 35fc  ..T.Z.j....D.u5.
-0005edc0: 54fe 5e22 113f ba4b 6c83 ec46 b6aa 9746  T.^".?.Kl..F...F
-0005edd0: 1a78 294d 6a12 e9dc d44b 8e05 0b77 16ca  .x)Mj....K...w..
-0005ede0: 97a6 1a59 0e3d a90e 58aa d6ae d432 f506  ...Y.=..X....2..
-0005edf0: ed1d 5eb9 1ac2 b154 f51a 1559 207c d349  ..^....T...Y |.I
-0005ee00: eec4 2eb4 f28a f001 9eba 2ce9 2db3 5198  ..........,.-.Q.
-0005ee10: f71d 871a cfca 0e2b 4763 a2e6 3062 7a34  .......+Gc..0bz4
-0005ee20: 4e67 4609 359e 6a46 e10c 4cad ea3d 8ec4  NgF.5.jF..L..=..
-0005ee30: 83b5 fc0c 4bb0 ff15 6165 9bc2 a611 5427  ....K...ae....T'
-0005ee40: d8fb e805 f81c 9648 c69d 4eab 7622 a2cf  .......H..N.v"..
-0005ee50: 6acb 5540 4b0c 0d72 a35e 1b3f 7958 8318  j.U@K..r.^.?yX..
-0005ee60: 4675 8da4 65f4 2520 1e85 52dd 86a4 3456  Fu..e.% ..R...4V
-0005ee70: d623 538b a052 9d72 90c8 b227 0569 0a4f  .#S..R.r...'.i.O
-0005ee80: 9169 673f 5438 6bea a7c1 8949 dfb2 a967  .ig?T8k....I...g
-0005ee90: 46e8 c49b e875 31eb a6ea 2eb0 c153 e317  F....u1......S..
-0005eea0: 3a75 64a4 8811 2809 afcb 3ad5 3e1f 780a  :ud...(...:.>.x.
-0005eeb0: 89a6 c3ba 8f55 1907 7841 6a33 d5aa 6b82  .....U..xAj3..k.
-0005eec0: 131d a453 55bb ff54 cd04 4fad f533 4c59  ...SU..T..O..3LY
-0005eed0: 5a00 c4a2 d9c8 5da3 f7a5 b1f1 d315 4b74  Z.....].......Kt
-0005eee0: 01ca fb9a 6b44 edc5 107d 6f2e cef2 3dac  ....kD...}o...=.
-0005eef0: 6882 b96b 1241 7af7 b0bf b857 acc2 4984  h..k.Az....W..I.
-0005ef00: 9623 ae96 36dc 3f35 3be5 2dab 5861 446a  .#..6.?5;.-.XaDj
-0005ef10: 550a ed55 84f5 fc61 2e64 2f22 2467 a4ac  U..U...a.d/"$g..
-0005ef20: e7ec 7170 d1a5 33ab ca50 0452 62b0 55f0  ..qp..3..P.Rb.U.
-0005ef30: e09a b8d8 bd8e efec c510 abc6 676b 4b87  ............gkK.
-0005ef40: e9b9 a518 ea20 f335 c3a7 ccb1 c276 a8a2  ..... .5.....v..
-0005ef50: d992 4777 265a df0b 09c7 bf6d 21a5 20be  ..Gw&Z.....m!. .
-0005ef60: cc5b 358a d9d2 b1c6 0fc9 a62c d953 f93f  .[5........,.S.?
-0005ef70: abad 1b5a 22c3 2340 1291 97d0 64ab 07a6  ...Z".#@....d...
-0005ef80: 1c79 a410 a6a7 abe9 38e1 523c 38bb d6a5  .y......8.R<8...
-0005ef90: 2fe3 7dfd d4e2 594e 3ae8 907e 6213 572b  /.}...YN:..~b.W+
-0005efa0: 3b16 3403 ba91 88d5 b88d 35da b973 2619  ;.4.......5..s&.
-0005efb0: 0927 674b 5c79 db4e 540d 7058 6446 db75  .'gK\y.NT.pXdF.u
-0005efc0: 3818 a248 f622 2ad8 9cf6 ce07 ce84 2b6b  8..H."*.......+k
-0005efd0: f595 8da0 0274 5112 ebea b1f1 6aa7 289f  .....tQ.....j.(.
-0005efe0: 2c7d 38b0 bf8c 8530 93e2 815d 6a0c daee  ,}8....0...]j...
-0005eff0: 65cc abb3 600b 99d6 4e5c 255a c3c2 1b66  e...`...N\%Z...f
-0005f000: 2325 bf12 acac a5d8 9861 262c a679 62b9  #%.......a&,.yb.
-0005f010: 81a3 c643 aaa4 9b52 902e 8566 1321 3413  ...C...R...f.!4.
-0005f020: 6556 238e 76d8 dd32 bda6 504c e560 310e  eV#.v..2..PL.`1.
-0005f030: da96 9ea5 3b84 96d3 75ba cd5b 909e 4017  ....;...u..[..@.
-0005f040: 63ec 1b38 803e b9d3 4e73 2657 556e 6935  c..8.>..Ns&WUni5
-0005f050: 0999 eb46 1c6f a9a2 6908 d9e4 ccd4 557f  ...F.o..i.....U.
-0005f060: e552 1f59 d16b 44aa 4bb4 a203 113e 4126  .R.Y.kD.K....>A&
-0005f070: b455 1e15 7e26 217a 9b8a 3e2b 6994 e4a4  .U..~&!z..>+i...
-0005f080: c545 7529 07b1 e8cf 791e 44a6 b97d e543  .Eu)....y.D..}.C
-0005f090: 48d8 ba5b 1de2 b955 8da7 a6c6 4289 b3bc  H..[...U....B...
-0005f0a0: a7db 689e 4104 f828 a68e 2edf e91d d1e0  ..h.A..(........
-0005f0b0: 7bf7 be9d 3488 c0e0 389a b6e6 5ce0 a82d  {...4...8...\..-
-0005f0c0: 5a42 29ae 1af7 5098 2292 ab60 2e4a 8154  ZB)...P."..`.J.T
-0005f0d0: 95e7 eb61 d9a9 2e55 1e5d 8bce b39e a5b0  ...a...U.]......
-0005f0e0: ee62 bf56 0b46 7d26 168f 1aec 4663 c4a9  .b.V.F}&....Fc..
-0005f0f0: 4821 6c34 212b bf4d ae4d d07d 544a 9784  H!l4!+.M.M.}TJ..
-0005f100: 2fa8 0fdd 17fd f089 3a8f de05 a9b3 2c09  /.......:.....,.
-0005f110: 4690 937e 7519 fcb4 92e4 4e88 8b7a f4d6  F..~u.....N..z..
-0005f120: f200 4712 1d53 086e 7129 d700 a4da 6597  ..G..S.nq)....e.
-0005f130: 8a91 c1a3 b0b7 bb5c 4647 4494 e368 bb21  .......\FGD..h.!
-0005f140: a4dd a2a1 2626 eb59 7659 42ec 2e69 0981  ....&&.YvYB..i..
-0005f150: 1336 90ae abbf 4814 fa69 43ce a2ae ebec  .6....H..iC.....
-0005f160: 8131 d524 576d 865d 1c35 f296 eca3 f1ee  .1.$Wm.].5......
-0005f170: 1b46 6312 28e5 4b54 ebc5 f262 1ed7 a15e  .Fc.(.KT...b...^
-0005f180: bc38 b8da 409e b5ec a5ea a37a 820d 1245  .8..@......z...E
-0005f190: abbc 6a2f 0490 d2f8 4fd3 7b79 9aad 3870  ..j/....O.{y..8p
-0005f1a0: e5d9 9fcb 2b08 7f58 13d9 be76 f123 f304  ....+..X...v.#..
-0005f1b0: 665e da12 3cde 6187 31fd 9622 cfb5 1203  f^..<.a.1.."....
-0005f1c0: 24ac df6e 6b59 8d92 a197 8788 bc7e c9b5  $..nkY.......~..
-0005f1d0: a606 1293 acbb b5be 36ca 65c7 e544 932b  ........6.e..D.+
-0005f1e0: f67b 2554 22ca af55 c53d 03f9 0fe3 2785  .{%T"..U.=....'.
-0005f1f0: 354d e4bf 518d 1a4f ebf4 b7cb 7ef2 1679  5M..Q..O....~..y
-0005f200: 797a c376 6c1c 8cae 2197 f910 0f0b 8f81  yz.vl...!.......
-0005f210: fb8e ea9e e31c 8127 0dba 942a 5708 db25  .......'...*W..%
-0005f220: 7b60 c1d0 c4a9 c69d 36a9 43f5 134f a004  {`......6.C..O..
-0005f230: 5926 48db b6f9 2870 54f5 e09b b4fc f891  Y&H...(pT.......
-0005f240: 7057 bedd 07a7 0c89 456c 6406 ee1d 1b0f  pW......Eld.....
-0005f250: bbc6 0f54 d42e 57b6 0a64 f1f2 6c28 3c5a  ...T..W..d..l(<Z
-0005f260: 1022 3e7a ba59 03d6 640b 471a 1123 fbba  .">z.Y..d.G..#..
-0005f270: 6e3a 9c95 28b2 d987 7615 4d0e 7aa7 45a2  n:..(...v.M.z.E.
-0005f280: 2ec1 dde4 0e4a 2a86 ceb6 d862 2369 acfa  .....J*....b#i..
-0005f290: 2279 194a 0e7b 19b8 2efa 1b34 6f53 8ecf  "y.J.{.....4oS..
-0005f2a0: ccfe 37dd afad ddb7 8abc 856d 8e5a b12f  ..7........m.Z./
-0005f2b0: 1954 5c1d 2ef0 5f26 cb88 ae1a c228 dd91  .T\..._&.....(..
-0005f2c0: 10cb 33a2 a8ca fc95 33fa 9682 a2ce 347a  ..3.....3.....4z
-0005f2d0: 8259 843b 64ec 61e5 3534 575a 8f65 e619  .Y.;d.a.54WZ.e..
-0005f2e0: 2560 a358 65bf 09aa f00c 2d4d 9702 a78a  %`.Xe.....-M....
-0005f2f0: 2085 caf2 737a 2a0e 35f6 3891 ca44 8597   ...sz*.5.8..D..
-0005f300: 087d aaf4 5c14 ee03 2700 b1b2 ad30 588a  .}..\...'....0X.
-0005f310: 20d7 9863 5b89 84ee 41ed 2406 6c6b 73be   ..c[...A.$.lks.
-0005f320: ca8d a30d 3d0c d81a d6e3 f402 16a2 cf0c  ....=...........
-0005f330: 68bd e80f 37a0 fb30 0679 4809 f897 b3e4  h...7..0.yH.....
-0005f340: 1eb4 263e d72f 59db 6672 493b 9ec7 8b45  ..&>./Y.frI;...E
-0005f350: d609 ec5a fc98 ce8e 41c4 1685 6d47 e6c7  ...Z....A...mG..
-0005f360: 2a01 2566 4e8e 9085 c099 f402 3b81 955e  *.%fN.......;..^
-0005f370: 2163 0b51 41f7 c30e cbfe 2721 46f6 4e65  !c.QA.....'!F.Ne
-0005f380: 1e97 4072 fbf3 e8b3 b785 3b3a 8191 51a9  ..@r......;:..Q.
-0005f390: 90c8 7ab1 4566 6508 f859 2497 f051 6c9a  ..z.Efe..Y$..Ql.
-0005f3a0: 92ee 300f 350f 963c 0c88 c44d c5d3 f2dc  ..0.5..<...M....
-0005f3b0: 8058 4bb1 c1a0 9daa 9093 e085 9d90 6336  .XK...........c6
-0005f3c0: 9357 1955 6045 9842 5c16 f0a1 7379 5518  .W.U`E.B\...syU.
-0005f3d0: acba f8a1 31da 29ac b9cd ec49 0553 898b  ....1.)....I.S..
-0005f3e0: 9056 e5b8 c792 e9c4 1842 068a 9760 3396  .V.......B...`3.
-0005f3f0: a36d 3246 88b9 8737 fa70 fa43 69af aecc  .m2F...7.p.Ci...
-0005f400: e66c 88a4 a016 b35e 8329 35bd 881b 36d0  .l.....^.)5...6.
-0005f410: 6766 e2e3 a504 f6c1 9ca1 cdcc d286 09a1  gf..............
-0005f420: 18d8 e691 c1ad 8743 0caf 2163 a19c 548c  .......C..!c..T.
-0005f430: 38c4 3c3a 75c6 3a6c ab61 c9f6 6d67 0c97  8.<:u.:l.a..mg..
-0005f440: 8882 cf8a 0e3d a079 9e6e 264c 7a69 ea88  .....=.y.n&Lzi..
-0005f450: 34d4 38f9 b546 ce59 3c81 3063 75e3 0eee  4.8..F.Y<.0cu...
-0005f460: 047a 9db1 0989 f6dd 9d0e b0bd 3032 5202  .z..........02R.
-0005f470: 4ce9 6076 3807 8ae8 fb96 b513 33dc 2f91  L.`v8.......3./.
-0005f480: 2a5b 2ece e0dd 274a 3162 e33b 44f4 0a03  *[....'J1b.;D...
-0005f490: 3c13 4f26 da44 0917 9a60 e6d9 b917 8de8  <.O&.D...`......
-0005f4a0: 5123 154e e70a 45e9 9e56 f231 7f35 df49  Q#.N..E..V.1.5.I
-0005f4b0: 451a 1580 f17e 4997 0ba6 e67c 151f 17b5  E....~I....|....
-0005f4c0: 8089 9e1f 69b9 5ea5 319e 5d43 e7e5 ed01  ....i.^.1.]C....
-0005f4d0: 166f ad01 b130 d1cf 3aa3 5059 d4dd 680d  .o...0..:.PY..h.
-0005f4e0: 5149 356d 310c 98f1 aa36 d310 8dae a4d7  QI5m1....6......
-0005f4f0: 51c4 cd6f f369 5221 513c 3f0f ee2d 42d0  Q..o.iR!Q<?..-B.
-0005f500: 1337 adb5 bb1f faee e900 2268 7976 945d  .7........"hyv.]
-0005f510: 6e3c 0b35 d055 bbcd d0ca e9ca 5e42 76ea  n<.5.U......^Bv.
-0005f520: f27e b66d 0a75 444c 1d5b 5153 0a9e d6a4  .~.m.uDL.[QS....
-0005f530: ae22 0d79 64ea 9a33 9900 1572 ac37 4de0  .".yd..3...r.7M.
-0005f540: 9026 4be0 d454 0b94 f117 adc5 5283 379e  .&K..T......R.7.
-0005f550: 239f 30ec 8efd 5aab 6236 3778 9c2b d7c3  #.0...Z.b67x.+..
-0005f560: 74b5 54d0 1246 39c7 6ac8 fefa 1b34 9710  t.T..F9.j....4..
-0005f570: 62ad 6bc2 bf3a e436 4494 47fd ac6d 86e8  b.k..:.6D.G..m..
-0005f580: 2b67 ae0e c17a e1ad dd5c 5d6f 745d abef  +g...z...\]ot]..
-0005f590: 8501 1e8f 1d3d 6afe 157b e033 b32b 4407  .....=j..{.3.+D.
-0005f5a0: f9b7 1c9f 75fd 7daa a356 5955 2ff1 a58d  ....u.}..VYU/...
-0005f5b0: fcfe fd9f 8f6d 26e1 8df7 fcaf dac2 0bfc  .....m&.........
-0005f5c0: f142 97b4 e598 4515 9fd5 c5e2 d3af d5ea  .B....E.........
-0005f5d0: 8f7a 1ee8 f9b7 9b3c e5e3 5362 1bf0 ffaf  .z.....<..Sb....
-0005f5e0: 24e2 b8f1 6bab 96b5 df15 8e1b 96ff c017  $...k...........
-0005f5f0: 4aac c9fd 56de 9f25 b0c9 27be 4a33 a156  J...V..%..'.J3.V
-0005f600: f70a d32a fae6 f776 375e ae3a b1c1 d3fd  ...*...v7^.:....
-0005f610: 7ca7 9fde 51c2 8371 e7c6 b57b f93c 3bbd  |...Q..q...{.<;.
-0005f620: 0fe2 4fc9 5abd 9bcf fff2 9633 abbf feef  ..O.Z......3....
-0005f630: 587b 0070 0810 0200 0000 4363 3033 0000  X{.p......Cc03..
+0005cc80: 5f80 10a5 4108 aa4a e1a0 00f9 121b 6cb0  _...A..J......l.
+0005cc90: 17ca c3b4 fb15 fcfb 8b24 8aae bea2 557e  .........$....U~
+0005cca0: 4153 4620 8a68 00ac ac0c 6c8a b400 a94a  ASF .h....l....J
+0005ccb0: 8245 cdd0 a701 cba8 84c5 1fce cc59 fcab  .E...........Y..
+0005ccc0: 7e01 8718 5e64 f892 280e 23d4 52f2 f9d0  ~...^d..(.#.R...
+0005ccd0: 6045 2533 6310 118e 29e1 aef0 8238 7d35  `E%3c...)....8}5
+0005cce0: 1441 943a 58c9 7a32 2218 087d a743 c3b5  .A.:X.z2"..}.C..
+0005ccf0: 64a7 10a0 0466 b3a4 1261 c804 b813 1110  d....f...a......
+0005cd00: 89df 7012 6d39 980d d7fc d89b 6e6f 03cb  ..p.m9......no..
+0005cd10: 0076 00b0 0003 a001 a332 8729 1be7 1fbe  .v.......2.)....
+0005cd20: 9909 43d2 7fd9 677e 2845 a912 cd2f f3a8  ..C...g~(E.../..
+0005cd30: 479b ba23 1864 f13d fcf7 fd93 65cf 0ca1  G..#.d.=....e...
+0005cd40: bcae b1f8 950a 7745 fcec e7f3 9f23 e528  ......wE.....#.(
+0005cd50: 0714 2fac 6d51 814c 0ffb fba9 bfeb e43a  ../.mQ.L.......:
+0005cd60: 1f26 9d50 17ed ddda b6d1 a317 a6c2 eb3e  .&.P...........>
+0005cd70: 412c e410 5428 c582 7b4d 7ae1 407a c671  A,..T(..{Mz.@z.q
+0005cd80: 1649 3ffb aca4 d9e2 7d64 03c6 f91c d773  .I?.....}d.....s
+0005cd90: 0225 9872 bee2 f3e7 8403 7d6b 633f d4c2  .%.r......}kc?..
+0005cda0: 4377 e7c2 1d0c 6b03 03df bfbf a87c 446f  Cw....k......|Do
+0005cdb0: 0ad0 8b18 cb2f c3db 56e1 6785 101e d1db  ...../..V.g.....
+0005cdc0: ab52 9e6b 2f98 9852 8b5e fc15 bd71 36c6  .R.k/..R.^...q6.
+0005cdd0: cfbf a59a fe45 1242 2b07 3e2c ecf2 1d6f  .....E.B+.>,...o
+0005cde0: 45c8 1b8c ce57 831b 5dfa feaa ae0c 10bd  E....W..].......
+0005cdf0: e42b e68d 298b 8e9f f15b 0dc2 da63 8f84  .+..)....[...c..
+0005ce00: 963f 8f8c e25c 650e 6dfe 156b 7b9e 6dff  .?...\e.m..k{.m.
+0005ce10: 079e 5638 db88 5ed8 9289 f9a9 e43d 1e5a  ..V8..^......=.Z
+0005ce20: 09b9 970c ff5c 7820 91f3 9a8d a6f7 2740  .....\x ......'@
+0005ce30: e5eb e0af 910d f040 f262 6e56 c5d2 7fab  .......@.bnV....
+0005ce40: 6fd4 5a5b 45ad 77e5 7ccf 2aa1 efca cef2  o.Z[E.w.|.*.....
+0005ce50: 7a6f 80e4 ff25 9c85 bfb8 289f 7eaa 9da6  zo...%....(.~...
+0005ce60: ed7d 533f 53f1 a3fa f6e4 f0c9 2c4b 6f19  .}S?S.......,Ko.
+0005ce70: 8830 f28e 06ee b365 544f 698e 2064 5c99  .0.....eTOi. d\.
+0005ce80: d9f6 ea3f 71cb cbc5 f20e 5793 87fa e2b2  ...?q.....W.....
+0005ce90: b7f5 b596 ae68 487e 45ae 0cd7 1687 a4f2  .....hH~E.......
+0005cea0: aa39 b53e 72fc 0765 97d5 63e1 0a86 b7dd  .9.>r..e..c.....
+0005ceb0: f123 6beb 59fe 508f 5c9d f576 f6f6 aeeb  .#k.Y.P.\..v....
+0005cec0: 5ff6 4112 68fd f4de 5e90 e25f 78c4 a17a  _.A.h...^.._x..z
+0005ced0: bfae e8bf 9ec7 bd3f d1b0 47b9 9003 30fa  .......?..G...0.
+0005cee0: ea48 6979 c768 9e9a 09a7 19e2 5071 b139  .Hiy.h......Pq.9
+0005cef0: 7dc3 af7f e8e8 27b7 aea0 867a 97b3 c547  }.....'....z...G
+0005cf00: 6734 0839 8ff4 c9af 483d d59f 8443 4238  g4.9....H=...CB8
+0005cf10: d79a 71a4 b4ff d28b 6afb e56f d4bb 8863  ..q.....j..o...c
+0005cf20: 3597 899a 5fc8 58f4 4c51 5f1d 0b71 d818  5..._.X.LQ_..q..
+0005cf30: f08a a7de e07e 9653 a6c5 a3db 1f3d a950  .....~.S.....=.P
+0005cf40: 7b9d 42e5 3f6e de5d f3d0 f792 9776 0580  {.B.?n.].....v..
+0005cf50: 97b8 1b8a 727f fd45 2a72 1d45 faaa 94b7  ....r..E*r.E....
+0005cf60: f807 c18f fa2f 4fec 0a42 df5b a070 84e3  ...../O..B.[.p..
+0005cf70: 6b6f 4e65 e771 62f0 d7ab 0f16 eaea a793  koNe.qb.........
+0005cf80: e49c 85f2 b87d b99c 391c b5c5 ff74 436c  .....}..9....tCl
+0005cf90: 1893 daae a4f2 d548 46b9 ff7c ebf8 7be1  .......HF..|..{.
+0005cfa0: 06af 7c1f 7e87 fa53 5f4a 7cdf 5508 4bde  ..|.~..S_J|.U.K.
+0005cfb0: 127e c40c 5e6a 6d38 cdd7 5f36 b690 eba5  .~..^jm8.._6....
+0005cfc0: 9fcd bdd3 0e5c 4eef 763e c707 77eb f2b7  .....\N.v>..w...
+0005cfd0: 101f 2ff6 4e6d 46bd 54c8 7ee0 437e b5de  ../.NmF.T.~.C~..
+0005cfe0: d413 f76f 1012 07f4 1bd9 a510 4a82 48ff  ...o........J.H.
+0005cff0: 9208 7fe4 2f26 3f2a 4297 9c28 d75c 8148  ..../&?*B..(.\.H
+0005d000: 7f3f 7b8c 254e 7f7a a049 3111 fb4e 24fe  .?{.%N.z.I1..N$.
+0005d010: f9e5 e889 9af8 fef7 f62c 6b0b 1dbf fec4  .........,k.....
+0005d020: 6b1b 0cff fdab cc8f c98f 732c 3c6a d563  k.........s,<j.c
+0005d030: d87a 15cf 9442 b7b8 370c f568 a1e3 db3f  .z...B..7..h...?
+0005d040: f3a3 543b cd79 1c2b 9482 4247 2072 896f  ..T;.y.+..BG r.o
+0005d050: fe5a 54fb f8d3 bc27 c5e2 12e4 17f9 bd9d  .ZT....'........
+0005d060: 0846 0ed4 d7a3 cd77 abf7 270e 77d3 50e4  .F.....w..'.w.P.
+0005d070: 4549 dfbd 5e93 70ab 72b7 4840 2d4c bfe2  EI..^.p.r.H@-L..
+0005d080: 2135 e763 48fa 903c 09f2 e98f a433 5fee  !5.cH..<.....3_.
+0005d090: cbff bdf6 dec8 9fe9 e64d 7b02 f492 7c9c  .........M{...|.
+0005d0a0: f4cc 399f b90e 5509 6b47 944a 29f5 0599  ..9...U.kG.J)...
+0005d0b0: 8f23 d084 a78f f93a fc14 8f3e a1bd c563  .#.....:...>...c
+0005d0c0: fdbf 94bc a0bf 4361 f1cf 7870 377d fe6e  ......Ca..xp7}.n
+0005d0d0: 716a 8af2 3fdd 3e6a c2ac 32fc e9c6 7adc  qj..?.>j..2...z.
+0005d0e0: b564 d5b6 a347 3bfe e1fa f2ae 2be3 375d  .d...G;.....+.7]
+0005d0f0: be98 bcf3 1e2a cc40 472f 8bc5 e97d 1fce  .....*.@G/...}..
+0005d100: db60 2ba7 fdae 0b75 c519 211d 360b 97f8  .`+....u..!.6...
+0005d110: fa17 c733 6b8c dc3e dfb6 794e de23 af1f  ...3k..>..yN.#..
+0005d120: 526f 8b44 0bc0 afe9 5862 8943 8100 a328  Ro.D....Xb.C...(
+0005d130: 5bfc 8bfc cccb dbee 4f6f 9eb5 664f d17d  [.......Oo..fO.}
+0005d140: 317d 9ea8 79b0 557d 268c 3b3d 627c 75a0  1}..y.U}&.;=b|u.
+0005d150: 9a93 6e5e 51df f667 be3a 152c 9eed 5f94  ..n^Q..g.:.,.._.
+0005d160: 075c a016 a7b7 267a 3e27 c571 3a75 d7f8  .\....&z>'.q:u..
+0005d170: 3b0a 3dd1 579e 017f dcf2 94ff cf70 718e  ;.=.W........pq.
+0005d180: e2ef 073c 2349 fc8f a06c 73fe 9061 384a  ...<#I...ls..a8J
+0005d190: 7d46 2ba6 321f b87f faba fd92 f96f 4df3  }F+.2........oM.
+0005d1a0: ac36 08b1 e60e 2401 bbd6 6aef 0b36 8773  .6....$...j..6.s
+0005d1b0: c2a2 b370 4072 8be7 ebfb 287a 8d5d de41  ...p@r....(z.].A
+0005d1c0: 5ee1 b73e 3854 7eb4 d371 0970 aad4 057c  ^..>8T~..q.p...|
+0005d1d0: b5c6 bbe8 7397 8a5b d239 cbeb 8ac6 ac18  ....s..[.9......
+0005d1e0: 982f 5b57 7ba8 ffe5 a938 afdb 8692 212a  ./[W{....8....!*
+0005d1f0: c0ee e25d 1bf9 b153 8a38 7d96 baf3 05bf  ...]...S.8}.....
+0005d200: 8923 4e63 0f7a a635 cb0f b3ee acdd 6d56  .#Nc.z.5......mV
+0005d210: f7ff fd69 fd9e 47d6 af78 e93b d1f4 57fc  ...i..G..x.;..W.
+0005d220: 22bd f4ed ff3c 57cf ba5b 2452 69b8 10db  "....<W..[$Ri...
+0005d230: 4f77 17ff 3a14 da1e d071 a742 5e02 ac26  Ow..:....q.B^..&
+0005d240: 7cc0 c0fb 4ce7 eae2 91e8 9d83 1df8 675c  |...L.........g\
+0005d250: 7ce6 77e5 430f d8fd a242 c9b9 bbee fdda  |.w.C....B......
+0005d260: e952 e306 6ec7 97a2 5fe4 fa1c 492f 4b90  .R..n..._...I/K.
+0005d270: 8b7f 957a 9a9e 1071 9dfd 1ef2 1e4c 44b1  ...z...q.....LD.
+0005d280: 3439 9473 98bd ff4c 6471 a546 7ace f1aa  49.s...Ldq.Fz...
+0005d290: 649f ff91 a518 e288 bfe8 4d24 ce5a 1e72  d.........M$.Z.r
+0005d2a0: 1bbf b2b7 7d65 40d9 0ced 70bd feee 1f29  ....}e@...p....)
+0005d2b0: 7e56 d7ba b864 f29c 5891 3972 5bf6 cf6b  ~V...d..X.9r[..k
+0005d2c0: 3eac 265b cf70 f2f7 9e7a 9977 2bff 2d0a  >.&[.p...z.w+.-.
+0005d2d0: da43 f370 93ee 5bf8 67f8 bb1f dcef cc7b  .C.p..[.g......{
+0005d2e0: ff04 6576 a9e8 a0ef aab1 bdda eacb a650  ..ev...........P
+0005d2f0: d7c4 0471 4cfa b6e4 98aa af13 3d7d 3ea5  ...qL.......=}>.
+0005d300: 81b2 f36a e1d1 7c1f f205 c801 f143 a23f  ...j..|......C.?
+0005d310: 2edf 0f1e 3841 94f7 313d f655 489e d968  ....8A..1=.UH..h
+0005d320: 88cf a54e 99ca d143 bd76 1fc3 ffa9 8985  ...N...C.v......
+0005d330: 3ba4 70d2 f8af 5f83 02ee 3d84 f720 72da  ;.p..._...=.. r.
+0005d340: 5172 f7c0 6f97 d8f2 8534 8d0b 1327 f84e  Qr..o....4...'.N
+0005d350: fce7 9fea 7c28 3efd 7aaf b527 8b13 2bd2  ....|(>.z..'..+.
+0005d360: a8f5 d4a8 a43f 002a 1df6 78e5 fa1a 55c3  .....?.*..x...U.
+0005d370: deee 8b2a 70c1 1487 0c1d 21d5 2bea 3664  ...*p.....!.+.6d
+0005d380: 706a 236e edfc 3695 79f6 5fed efee 6e4c  pj#n..6.y._...nL
+0005d390: 7138 6adc ef73 d5e5 ea42 a0db f645 2229  q8j..s...B...E")
+0005d3a0: fee3 7d74 e64f f7d9 c2ee 493c 1f8c 7cd0  ..}t.O....I<..|.
+0005d3b0: ffbb 9541 79dd a5e7 5551 8457 edb1 bcff  ...Ay...UQ.W....
+0005d3c0: 28d4 c5f5 997a f5de e397 6f9f e61f 1f1e  (....z....o.....
+0005d3d0: ba57 8422 83bd f4d6 b384 3987 c7ed 57d7  .W."......9...W.
+0005d3e0: 69fe 98e8 bef3 cf29 ffeb f33f d128 6d3e  i......)...?.(m>
+0005d3f0: bc97 bf9f e694 8756 1ce8 537e 6ed2 5cea  .......V..S~n.\.
+0005d400: 56fb c573 f13f 4e51 447f 9a8d a267 8e31  V..s.?NQD....g.1
+0005d410: 3e59 b931 31be c627 cf11 df1b 42fc 3f0e  >Y.11..'....B.?.
+0005d420: 63a0 ebcf 7c20 eb39 cdf7 f597 619e 3f21  c...| .9....a.?!
+0005d430: 3c31 3afa f8bf db68 4420 24e2 fc57 5407  <1:....hD $..WT.
+0005d440: 8875 fee3 dd9b 9ff1 1fe4 0b61 c78a f5df  .u.........a....
+0005d450: 9c02 dc09 04c3 1ca7 1e0b f493 5abd 43c5  ............Z.C.
+0005d460: 2f97 2ae4 2967 ca4f 0950 6e6f 90df 7519  /.*.)g.O.Pno..u.
+0005d470: 9cb3 4b7e bceb c479 507f 1071 a2f0 1085  ..K~...yP..q....
+0005d480: bfb0 f7e4 f0cd 83a2 2ffc 2f78 16f2 ed8d  .......././x....
+0005d490: 257f 32e8 0cfd e8fc bf62 9e27 63ef a5e2  %.2......b.'c...
+0005d4a0: 5957 96e0 f621 4e9f 372b aaa5 506f 9c9f  YW...!N.7+..Po..
+0005d4b0: 58a5 e459 f69b 63fe d4f8 f57a dfe2 fdeb  X..Y..c....z....
+0005d4c0: be14 2b7d 22fc d6df 6dce f4f9 1d85 c613  ..+}"...m.......
+0005d4d0: 1c26 1ec2 5bba ce6b f49c c479 07f2 ab14  .&..[..k...y....
+0005d4e0: beda 5e4d 7ef7 a5b2 c6fb 25f5 39ad 3710  ..^M~.....%.9.7.
+0005d4f0: 1132 bd87 f647 fcef 3d30 15de 6da0 005f  .2...G..=0..m.._
+0005d500: 78ae 90ea 228e 6d7f c7e7 e31f 66d8 20bd  x...".m.....f. .
+0005d510: 211f ce7f eaab 2a7b 2c46 df2a 4382 dde4  !.....*{,F.*C...
+0005d520: a440 d2de e9e0 9dc2 3dc4 f82b cbde 4b3b  .@......=..+..K;
+0005d530: 8ffa dac3 d26c 6b5a 8a09 ea65 b64c cca1  .....lkZ...e.L..
+0005d540: c956 3c82 65a6 cbd8 5db0 a7d2 95df 33f7  .V<.e...].....3.
+0005d550: 4aa5 6932 b9a5 cea4 b58b 7974 e9b5 aee6  J.i2......yt....
+0005d560: b71e e9d2 f7b0 7387 d809 d9b2 43bc 23be  ......s.....C.#.
+0005d570: 2c27 20d5 2d50 f445 75bd af4c 2463 3129  ,' .-P.Eu..L$c1)
+0005d580: cbcf a7a6 4e9d 8a65 9d61 e81c 67e6 e50a  ....N..e.a..g...
+0005d590: b33e cdb6 1851 5929 c436 04a6 f41a cd60  .>...QY).6.....`
+0005d5a0: 346f 5ac3 60ca 58e6 ca25 a4ea acf3 5398  4oZ.`.X..%....S.
+0005d5b0: 159c 3117 d84c 1273 3a46 1b45 f665 29d8  ..1..L.s:F.E.e).
+0005d5c0: a543 88e2 41f1 5ec5 f16b 4c82 e8f9 9fcd  .C..A.^..kL.....
+0005d5d0: 5e3d a4c7 5630 f3e9 f5e2 42ec 4b8b 922e  ^=..V0....B.K...
+0005d5e0: 75b7 561d 5047 fc6e 4b64 f1a7 3ca5 82dd  u.V.PG.nKd..<...
+0005d5f0: eae0 ef9f 4dc7 3cbb 69b6 b926 ea34 9dc6  ....M.<.i..&.4..
+0005d600: 2b73 6048 a8e9 3639 9c19 7162 4356 ac48  +s`H..69..qbCV.H
+0005d610: 8a76 062c fb7a 42bf caad 4511 3af0 767a  .v.,.zB...E.:.vz
+0005d620: ba69 d43e a5ee a48e 64d5 fdcc a935 b63b  .i.>....d....5.;
+0005d630: def1 6adb ba5b 5750 0d38 2fde ccd2 fddd  ..j..[WP.8/.....
+0005d640: 8b96 6187 33ef b28c 89e5 1ede 523b c69e  ..a.3.......R;..
+0005d650: 6a18 8cd5 6627 d1d5 9c4b a391 98a3 ba17  j...f'...K......
+0005d660: e628 3b59 7623 12c2 769b 35ac 042a 6dbe  .(;Yv#..v.5..*m.
+0005d670: 38d2 a6c6 8e47 3357 f415 6427 7645 2d5b  8....G3W..d'vE-[
+0005d680: 9667 6d9b d55c d054 fdd4 dbc9 09a5 7436  .gm..\.T......t6
+0005d690: 51cc c2fc 7fd7 4fa2 64a3 68d3 52ca 5607  Q.....O.d.h.R.V.
+0005d6a0: 5685 dff1 c520 e8c8 4515 069d 5b9d dc2b  V.... ..E...[..+
+0005d6b0: dfbc b990 3a23 e7d0 9037 6ee7 03d5 6616  ....:#...7n...f.
+0005d6c0: f986 56f3 2e7d 9be5 cc77 6669 d2c3 a96f  ..V..}...wfi...o
+0005d6d0: d497 6d87 d16c 54db c39d d30a 92a4 0c68  ..m..lT........h
+0005d6e0: 26e4 96f1 7c65 4412 ab87 7768 cbaa 1313  &...|eD...wh....
+0005d6f0: 1cdc b39b 4bf2 2405 08bf 533d 79b8 70a0  ....K.$...S=y.p.
+0005d700: c91d 0ce9 1de7 266a a56c cee4 da9d 70b7  ......&j.l....p.
+0005d710: 3aec 62ab 3ee1 8b31 69bc 11b1 89fd ee98  :.b.>..1i.......
+0005d720: b354 9b0c e515 b9d7 2e33 ce79 b166 ae89  .T.......3.y.f..
+0005d730: 3126 1e89 a427 9cc9 b3ea 4d97 ed28 1716  1&...'....M..(..
+0005d740: ba3c 44cb c06e 1c53 49b1 e637 2bf7 694e  .<D..n.SI..7+.iN
+0005d750: d392 679f 9e1d ee4e fa91 59c8 18cf f5db  ..g....N..Y.....
+0005d760: 73f8 a73e 9909 f4ae a09f 68e3 1a6d 79f2  s..>......h..my.
+0005d770: fd92 4853 6ce6 a24d 9ec6 e0e4 6cc1 d244  ..HSl..M....l..D
+0005d780: 6459 0cea f205 f3c9 bb65 a205 a127 ed9a  dY.......e...'..
+0005d790: 1025 32a3 617e 121d 6257 be3c cbd7 21a7  .%2.a~..bW.<..!.
+0005d7a0: ea54 5cb8 426f 2241 d453 2419 435d e9e4  .T\.Bo"A.S$.C]..
+0005d7b0: 5825 070f c599 e627 35f7 ba76 19d4 7228  X%.....'5..v..r(
+0005d7c0: c32a 7155 708a 669e 4e8f a842 985e 6738  .*qUp.f.N..B.^g8
+0005d7d0: f193 262a 8b59 fe99 94fa dcd0 b1a4 dd36  ..&*.Y.........6
+0005d7e0: ce34 9a4e 3f73 9926 cc26 bd98 182b 1eed  .4.N?s.&.&...+..
+0005d7f0: ac69 b78a bcaa d8c2 a8b4 ab98 d6d4 3d31  .i............=1
+0005d800: 27a6 5221 229e cc52 9598 5599 543d 314e  '.R!"..R..U.T=1N
+0005d810: d92d c117 a5cf fbd6 5699 34ba a8bd e1ac  .-......V.4.....
+0005d820: 3590 ea4c 268f 5832 13d3 3f08 6da3 27dc  5..L&.X2..?.m.'.
+0005d830: bccd 4d2c 4a1d a69d e47e 6bd7 ae64 ccde  ..M,J....~k..d..
+0005d840: 768e 7d33 be50 f6a6 f6ae 2694 9c17 84bb  v.}3.P....&.....
+0005d850: 238b c7d7 28aa b54a 0b95 47f7 4cb1 71e4  #...(..J..G.L.q.
+0005d860: 3a7a 8975 f10b c0da 3e91 d1e5 f97f 71e6  :z.u....>.....q.
+0005d870: 0c79 335d 7b04 fa7b 541d 7b3a 6642 a971  .y3]{..{T.{:fB.q
+0005d880: 4d4f c4ac b137 a9dc 342b 0f8b 30f9 2992  MO...7..4+..0.).
+0005d890: fa19 2966 4303 b12d 2ea5 d2d8 ffeb b22c  ..)fC..-.......,
+0005d8a0: 3ba5 39ae 6c49 4498 16da e34e 99a7 23a4  ;.9.lID....N..#.
+0005d8b0: 62b7 dc9a 99ef 8e6b 85a7 927b 2c14 6660  b......k...{,.f`
+0005d8c0: 8e57 189d 3fbe 0284 077e e34b 4eff 30e3  .W..?....~.KN.0.
+0005d8d0: 4ebb ae51 9953 c1d5 cb3e 5154 4aa2 a348  N..Q.S...>QTJ..H
+0005d8e0: 5019 62c9 e5d0 760c 548a 7b6a ac52 2854  P.b...v.T.{j.R(T
+0005d8f0: 7a29 19c9 2937 79fe 9a32 724a 2585 a1c8  z)..)7y..2rJ%...
+0005d900: 97d7 38b4 beb4 be9b 68aa 09a4 8d1d b4c8  ..8.....h.......
+0005d910: 8de9 e423 85e5 0dec 421d 6e19 bd91 a211  ...#....B.n.....
+0005d920: 7373 e9c0 7227 ba64 fd2c b50f 93ec f46f  ss..r'.d.,.....o
+0005d930: f51f a1de 5965 1ebb aefe 8775 b3c8 cd39  ....Ye.....u...9
+0005d940: 2896 9395 4af9 a8e9 92c5 fd2f 3d9a 1cd3  (...J....../=...
+0005d950: 7591 494d 4e9b 6312 8553 560b 8ec4 92cf  u.IMN.c..SV.....
+0005d960: 8c50 b642 e43b af64 e444 dcdc e5b0 dbdc  .P.B.;.d.D......
+0005d970: 10ff 8cc7 0eb5 b2ec aa4d bbd9 b6c5 daf9  .........M......
+0005d980: 36a4 ee67 94ab d5e1 6a79 95cb aab5 da9e  6..g....jy......
+0005d990: 775c 7117 373f 2e96 e2d2 66a6 c9ce ccdc  w\q.7?....f.....
+0005d9a0: f6fa 5426 2574 aece d1b7 6c0e f199 4cf6  ..T&%t....l...L.
+0005d9b0: 1102 957e 0aa1 4bbc 8ea1 514e a4d2 e54b  ...~..K...QN...K
+0005d9c0: b6cc 0fa7 6021 ddc6 1e23 9159 d202 ce6b  ....`!...#.Y...k
+0005d9d0: f41c 31c6 4ba3 9837 8c63 df8e e02e 2cef  ..1.K..7.c....,.
+0005d9e0: eab7 600c b62b 3b13 e34c 77dd 4bac d305  ..`..+;..Lw.K...
+0005d9f0: 6647 a5f2 dcdd 65f1 541e 745c c15d e39b  fG....e.T.t\.]..
+0005da00: 9176 8811 37df a9bc 67b2 a41d 95e3 1c19  .v..7...g.......
+0005da10: 76bb 85ea a9cf df2e 4242 30d2 a19f 1837  v.......BB0....7
+0005da20: 34b1 7467 b332 77d4 f42c ba93 d7b3 5df1  4.tg.2w..,....].
+0005da30: e97d d722 9774 6317 261d ee54 69cb c3b0  .}.".tc.&..Ti...
+0005da40: 9a9c e5db 1d3d 05f9 bb51 d0b3 3334 b56a  .....=...Q..34.j
+0005da50: 58cb 4a1e 759a 8431 cb2e 6d66 f031 d958  X.J.u..1..mf.1.X
+0005da60: c6dc ae3b e3aa 3707 30e3 b117 23cd d5b3  ...;..7.0...#...
+0005da70: a3d9 eda2 602a dc5e dfe7 734c 13cf 95de  ....`*.^..sL....
+0005da80: af55 19f3 4afe c572 dfc2 b2bd 7469 921d  .U..J..r....ti..
+0005da90: 82eb 1fc2 6201 5468 0a3b 8e43 2913 1c9b  ....b.Th.;.C)...
+0005daa0: 8cbd d7e1 75dd 65ca d2d6 daad 4626 01ce  ....u.e.....F&..
+0005dab0: f2b4 61f1 3746 bc7d ae44 d943 3037 60ac  ..a.7F.}.D.C07`.
+0005dac0: 5ac8 1df2 3346 6bbd 9f9a 36aa 635b 6aec  Z...3Fk...6.c[j.
+0005dad0: b734 d12e 4edd 67ea 5eab 872d a09f 3bdc  .4..N.g.^..-..;.
+0005dae0: bad4 9625 97ac bd35 8c5e 4bdf 0b5c 99d0  ...%...5.^K..\..
+0005daf0: 1b50 47f6 ad38 e38c 69cb 1238 58b8 951b  .PG..8..i..8X...
+0005db00: 37b0 e439 972c 9ad9 ccd2 3b9b c020 1e4b  7..9.,....;.. .K
+0005db10: c77a 1636 3de3 add6 1473 3bde d402 a393  .z.6=....s;.....
+0005db20: 545c bac1 c07a c984 4835 3de1 e367 56e6  T\...z..H5=..gV.
+0005db30: 1f17 38c5 e3eb 7f94 8841 ca0e c6e6 0bcd  ..8......A......
+0005db40: e2cb c612 3d41 db99 ad50 eb00 8c73 a92b  ....=A...P...s.+
+0005db50: 62d6 a6f7 91ea da42 a919 3217 35f7 d32b  b......B..2.5..+
+0005db60: 8a24 b240 d58b bf5b b6d1 e8b9 fc18 33e9  .$.@...[......3.
+0005db70: a9ee e93a 478f 38ba b109 5832 e4f8 b770  ...:G.8...X2...p
+0005db80: dec7 b31c 31a6 c464 5e5b 6336 96a8 b2e9  ....1..d^[c6....
+0005db90: 778f e198 3743 176d 5726 ef86 d509 6cde  w...7C.mW&....l.
+0005dba0: 63c2 891e 3ab4 5ab5 a376 fa30 27cc 5d55  c...:.Z..v.0'.]U
+0005dbb0: 6aae 980c cdec c3db b56d 39c9 f5f5 bb49  j........m9....I
+0005dbc0: e1b0 d883 fbee 7149 1f90 566a 384c 6c2e  ......qI..Vj8Ll.
+0005dbd0: 8d86 c36d d02e bb21 ce76 66a9 f00b 660f  ...m...!.vf...f.
+0005dbe0: e926 ce3a 3aef 9cc6 875d 5a54 35bd c98e  .&.::....]ZT5...
+0005dbf0: 2af1 7988 d6f1 75e7 428b 9f7c c52a f2eb  *.y...u.B..|.*..
+0005dc00: c3ea afa4 32aa 9de6 568d b273 2d67 0e39  ....2...V..s-g.9
+0005dc10: 789e 765c 039b 7af2 9c67 f56f f7fd 362d  x.v\..z..g.o..6-
+0005dc20: 6b66 c65b 6da4 eb0e 5a11 d2fa e32e 854c  kf.[m...Z......L
+0005dc30: 4f7e 27bf 6e60 780c 731b fa1d 7e6b 6d99  O~'.n`x.s...~km.
+0005dc40: 461a 7d79 bd12 21d0 662e 2c97 e297 e2b7  F.}y..!.f.,.....
+0005dc50: f92a eee8 6d0e 6ea6 db1d 46a4 3824 6fa5  .*..m.n...F.8$o.
+0005dc60: c91d f48e f821 fb9f e496 96ca f01d 6932  .....!........i2
+0005dc70: a77e 21c7 2c26 fcbd 8190 9c0d f4a8 d653  .~!.,&.........S
+0005dc80: afc2 6f62 eca9 45af d548 bdd7 a689 511f  ..ob..E..H....Q.
+0005dc90: d9f0 8fe1 b0ee 2c88 ccee 1d9f c607 bdab  ......,.........
+0005dca0: 176d e8c1 0e73 97d3 889e 707e 0767 7fd6  .m...s....p~.g..
+0005dcb0: cb85 150b bc18 8390 bd06 8900 ce0a e7e7  ................
+0005dcc0: 1796 afaa 8534 df5d d7e8 e6b3 16e2 66bf  .....4.]......f.
+0005dcd0: eb94 6031 79bb 9dd3 e721 0db0 fe25 fb2c  ..`1y....!...%.,
+0005dce0: 5b5b 69d9 456f 8b44 7224 dee7 3963 85fb  [[i.Eo.Dr$..9c..
+0005dcf0: 3ec5 9c98 df55 c762 27d8 07f9 e27b fb0d  >....U.b'....{..
+0005dd00: 20a6 b33a 76e1 9e62 fc8f efa0 7688 29a7   ..:v..b....v.).
+0005dd10: 8442 eb29 9c5f f62f 7b63 0488 f638 b83e  .B.)._./{c...8.>
+0005dd20: febb 4d95 fe7b 670f f737 f610 7935 c0cb  ..M..{g..7..y5..
+0005dd30: e98b c4bc 1e8c b5e7 8a0f f8f1 2efa fd9e  ................
+0005dd40: f799 b545 b3df 0a16 6fb4 f7f9 8a28 7890  ...E....o....(x.
+0005dd50: 97f9 1dbf df79 fc5a abaa 6e5f 250d f7d5  .....y.Z..n_%...
+0005dd60: 7de4 ef4e b52b 8447 c562 907f 8727 9c9e  }..N.+.G.b...'..
+0005dd70: c79e 10b5 7f41 6c8a 79be 8810 0ec7 f671  .....Al.y......q
+0005dd80: bff3 a66c acff 8d44 92ba e43e d975 c429  ...l...D...>.u.)
+0005dd90: b154 bf6f 1c21 6eab bf0f 762c 12e7 bb74  .T.o.!n...v,...t
+0005dda0: e271 86bf a916 fd9e 9c87 13c8 af2f f625  .q.........../.%
+0005ddb0: d56e fa07 3f2a 6a9c e9f9 21ce 6517 4f8a  .n..?*j...!.e.O.
+0005ddc0: e49f 5e3f 12f2 eba6 0efa ff19 75b1 b375  ..^?........u..u
+0005ddd0: 9f8b 4229 4f6c 37f2 27b9 6e6b 8aeb f692  ..B)Ol7.'.nk....
+0005dde0: 7859 b8a5 52e3 7b22 1cee d7b9 0ce8 ff58  xY..R.{".......X
+0005ddf0: 87df ee4d 7fbe 7678 c0bf e1e8 6ffa 3ff7  ...M..vx....o.?.
+0005de00: c003 7a78 92f8 1cf7 9cd4 244a af47 9fd4  ..zx......$J.G..
+0005de10: f666 52cf 4ea4 3fe2 2cfb 10b9 638b 6dd1  .fR.N.?.,...c.m.
+0005de20: d6cb 8fb9 4aca 737a f9cf bf4a 7f45 4a5f  ....J.sz...J.EJ_
+0005de30: f830 479d e67a 698d 6b3a 37fd 3a20 e2b5  .0G..zi.k:7.: ..
+0005de40: 7d66 da79 b4c8 d6bb f23f 3c52 4492 8efb  }f.y.....?<RD...
+0005de50: 9813 9ce3 a38c f327 fbd7 693e 2c3f e7ff  .......'..i>,?..
+0005de60: 9347 c827 c4b0 3670 abdf e697 9485 bfc4  .G.'..6p........
+0005de70: c5c8 7e48 aa47 4e67 543f dc8b 65be 8ff6  ..~H.GNgT?..e...
+0005de80: 285e 3307 a188 fc51 690f d3ff a36b fab6  (^3....Qi....k..
+0005de90: 5c9d dfbd d294 e91c b83f 74dd 9b75 cfd9  \........?t..u..
+0005dea0: b7df 6cd3 5374 0782 1738 afa4 15ff ec9f  ..l.St...8......
+0005deb0: 7a7f 7150 8f46 ed38 b34a e7e3 6bc2 fdb4  z.qP.F.8.J..k...
+0005dec0: b9e8 0a00 cd6e 04f8 66ce 4fcd 710e 3f3e  .....n..f.O.q.?>
+0005ded0: e6b4 7a3b cd7e 3f0f dfed 16fa b9df 18cd  ..z;.~?.........
+0005dee0: 8e42 eccd 92d4 d3f7 4cfd f883 fb76 1544  .B......L....v.D
+0005def0: 1f77 ec1f 354f 5e47 9f5b f85a b3fa cdff  .w..5O^G.[.Z....
+0005df00: 5266 8d15 9fbf c162 c53f 2f39 8b77 f58f  Rf.....b.?/9.w..
+0005df10: 57e4 7d6a c61d b75e 232f aa09 3efc ff63  W.}j...^#/..>..c
+0005df20: f140 4f56 95de 187e 6d96 837c 5a86 332e  .@OV...~m..|Z.3.
+0005df30: 615e 90c7 22e5 1a85 e8b5 62d1 f735 feb3  a^..".....b..5..
+0005df40: 2080 2083 8f2f bfe5 f7db 7118 fa47 de68   . ../....q..G.h
+0005df50: 294b 4aaf 2941 cbee ef53 7eca ac21 ff66  )KJ.)A...S~..!.f
+0005df60: 14f4 7abe dd42 a7df 56c3 6c42 c5fe 0bc0  ..z..B..V.lB....
+0005df70: 4e22 cf6d 915c 579f a6e1 1a5d 7180 8f94  N".m.\W....]q...
+0005df80: 87f0 d2a5 1cd3 4574 04fa 319c f14f 2e37  ......Et..1..O.7
+0005df90: 2c4a f32e 5f8f de44 789b 7cae 6987 0f1e  ,J.._..Dx.|.i...
+0005dfa0: ddb4 e25e 9504 728e dc07 c4cb d62a 2bef  ...^..r......*+.
+0005dfb0: 9e7b 8ba2 11e7 7c32 7b7f 5c4e 98f0 724e  .{....|2{.\N..rN
+0005dfc0: b90f e26d 6f0c def7 f67d 8843 6189 11f0  ...mo....}.Ca...
+0005dfd0: e770 eeb2 25b2 de91 8c22 14c7 78df 32ff  .p..%...."..x.2.
+0005dfe0: b295 e2f0 f015 fe73 141f 7bf0 bc91 9f02  .......s..{.....
+0005dff0: dda9 85db f728 b7ab 510a 9de8 0cbe 0a5e  .....(..Q......^
+0005e000: eb0f 941f 77fd 5fa4 47dc 8587 543f 6de8  ....w._.G...T?m.
+0005e010: 95e2 d2ef f7df 8fd2 6192 fdb5 dcf1 949c  ........a.......
+0005e020: fe5d c291 fe87 1f2e a811 231c ad5e b7b5  .]........#..^..
+0005e030: 73bd 172e be74 6a51 c4f9 4e50 286a d763  s....tjQ..NP(j.c
+0005e040: 109f c11c 7912 e5fe 7a30 cbe2 e80a c396  ....y...z0......
+0005e050: 1587 b58e a752 15ed 75bf f739 204d e2d1  .....R..u..9 M..
+0005e060: cfcd 4498 0abb 8647 eb7b 3ab1 78e8 1011  ..D....G.{:.x...
+0005e070: fd95 92eb cc62 f87d 3085 7dfb f1fa 18a6  .....b.}0.}.....
+0005e080: b71f bc0b 7055 574c 7fef 8035 f562 c7e4  ....pUWL...5.b..
+0005e090: 857c 7cf1 175f f1c5 5f7c dd3f 5010 2f3e  .||.._.._|.?P./>
+0005e0a0: fd38 2506 a0a3 97fd e273 1508 2f1d 3cc0  .8%......s../.<.
+0005e0b0: 04f7 4e37 3558 3efe 3ea5 ff1d f7a4 2ddb  ..N75X>.>.....-.
+0005e0c0: 873c f338 0139 7a09 ea63 c189 d7de 7a1b  .<.8.9z..c....z.
+0005e0d0: ddcf 17f2 f1c5 5f7c c517 7cf1 175f f1c5  ......_|..|.._..
+0005e0e0: 5f7c c517 7cf1 46fb d191 3168 6cf9 78bc  _|..|.F...1hl.x.
+0005e0f0: a9f1 c583 86ef 07f0 dfbf 49b0 46a3 1f4e  ..........I.F..N
+0005e100: f3a9 fb49 e20b bef8 8b2f f8e2 2fbe e28b  ...I...../../...
+0005e110: bef8 8b2f f8e2 7ebe 4253 b47d c903 0a51  .../..~.BS.}...Q
+0005e120: 146c 8411 4164 e0f6 00ff e126 209c 792a  .l..Ad.....& .y*
+0005e130: c8b0 895d 940a b015 1e6a 182a 0354 fc29  ...].....j.*.T.)
+0005e140: 3a56 cc30 923d 888c 0be6 8543 1b48 07bb  :V.0.=.....C.H..
+0005e150: d82d 355f f96c 81c0 88bf d001 0f0f 6e0c  .-5_.l........n.
+0005e160: a80e 0728 b2c2 ba1a e8fc 163c 0bec 9dc6  ...(.......<....
+0005e170: d65e a286 071b 8a20 0ac6 d080 5758 d058  .^..... ....WX.X
+0005e180: f299 1a11 81c3 d6c0 bf5f 2d24 d10c 2e70  ........._-$...p
+0005e190: 5240 b151 b61d a173 084e 910d 22e2 4326  R@.Q...s.N..".C&
+0005e1a0: ef83 0e14 88e6 5d3e db63 174a 79ca c437  ......]>.c.Jy..7
+0005e1b0: 9be0 50f4 c26c 2103 7241 8b81 d204 ba02  ..P..l!.rA......
+0005e1c0: 5086 8f13 ce45 790d 4502 17bc 6e70 7107  P....Ey.E...npq.
+0005e1d0: 92c2 d719 42c9 110c 460d 5943 04bf 64b3  ....B...F.YC..d.
+0005e1e0: 18c0 858f 1d2e 6518 8b07 0a46 7f5f 85bf  ......e....F._..
+0005e1f0: 9691 fc80 56fc e920 b5c1 5600 ba40 4483  ....V.. ..V..@D.
+0005e200: 5b60 60b0 f082 5638 c6c0 c903 5321 c4d0  [``...V8....S!..
+0005e210: 2273 5122 3cf4 4411 95ce 0c1a d21d af04  "sQ"<.D.........
+0005e220: c21f 3864 4809 b584 1b1b 6e87 d7c0 df7f  ..8dH.....n.....
+0005e230: 1c08 0c14 14da 2f62 64c3 8642 f849 106d  ....../bd..B.I.m
+0005e240: a124 0d3f 03de 5769 8fe1 9a60 43a6 3260  .$.?..Wi...`C.2`
+0005e250: b129 e85d c9d0 de40 f859 f064 3c51 c015  .).]...@.Y.d<Q..
+0005e260: 2128 e06b c881 706a 0e22 e015 602b bbcf  !(.k..pj."..`+..
+0005e270: ba05 2d11 8700 040f 6573 13d8 d0a1 129b  ..-.....es......
+0005e280: 8446 1f1a 2093 2006 2018 40e1 97d9 e406  .F.. . . .@.....
+0005e290: 5411 4fc3 70fc 5550 8fa1 8d61 8375 2103  T.O.p.UP...a.u!.
+0005e2a0: 3521 df43 ac85 e064 41d6 e0c5 0328 c335  5!.C...dA....(.5
+0005e2b0: 86c2 6a8a 4b03 50f0 6ada 089e 185e 15e2  ..j.K.P.j....^..
+0005e2c0: 4bf0 1540 2ed0 c0a0 1d52 7108 1138 3089  K..@.....Rq..80.
+0005e2d0: c28e 080a 8296 314f c983 50ac 2126 7f0a  ......1O..P.!&..
+0005e2e0: 1323 0834 f070 8163 8011 8764 4442 d400  .#.4.p.c...dDB..
+0005e2f0: e102 293f 6103 8f68 a15d 76c1 1181 59e0  ..)?a..h.]v...Y.
+0005e300: 83df b261 1648 7408 812f 5132 1c10 802b  ...a.Ht../Q2...+
+0005e310: 064b 43cc c8c1 c026 48d4 8357 f864 4b13  .KC....&H..W.dK.
+0005e320: a20a 8634 0712 a143 a00b 8e12 1935 5504  ...4...C.....5U.
+0005e330: a541 c980 0907 0070 33c0 158e 2770 8d01  .A.....p3...'p..
+0005e340: 7e3d 6019 771c 60e1 2005 dd4c 4486 2431  ~=`.w.`. ..LD.$1
+0005e350: 2f1f df3f b8c2 7c2e 28e8 4c2b 9300 2182  /..?..|.(.L+..!.
+0005e360: acf8 c200 e50b 6645 5419 ca12 c1ee acb2  ......fET.......
+0005e370: 430e c0fc ba06 3380 40e5 35dc 1da4 d161  C.....3.@.5....a
+0005e380: 0694 4270 c7f0 6b50 a30d 75f0 8f81 7205  ..Bp..kP..u...r.
+0005e390: b562 4541 2898 187c 2421 f6ed 0ff1 9304  .bEA(..|$!......
+0005e3a0: 8464 081b 9c0a 3013 df62 3686 1321 5710  .d....0..b6..!W.
+0005e3b0: 18f3 0d38 056f ea47 0804 02a7 947f b142  ...8.o.G.......B
+0005e3c0: b0b2 cf0d e16b 0465 3078 1b63 02ac f844  .....k.e0x.c...D
+0005e3d0: 8220 b48e 071c e90a 1309 5690 e041 6ba0  . ........V..Ak.
+0005e3e0: 37e8 1514 319c 5860 a8a8 c288 cb60 c840  7...1.X`.....`.@
+0005e3f0: 1d30 121c 0d90 049b 6fb4 1dac 2554 10e5  .0......o...%T..
+0005e400: f593 aab8 b03b 69de 13d8 85d0 8247 780a  .....;i......Gx.
+0005e410: 2167 a2e0 4036 fc11 3033 6234 0533 7090  !g..@6..03b4.3p.
+0005e420: 12ec cf98 ae10 eebc ecf3 d8f0 40e2 3054  ............@.0T
+0005e430: 03a7 da7b d9b8 76b0 153d 002a 4157 60cb  ...{..v..=.*AW`.
+0005e440: d364 26a8 1514 2d3c c5c0 0a0e a619 bb90  .d&...-<........
+0005e450: 7b15 1a1b 870b b0c2 a003 1e19 9c2d c035  {............-.5
+0005e460: 57a8 82ca 3b10 47c0 2b2c 2440 a1c6 8213  W...;.G.+,$@....
+0005e470: e804 d9e1 2f1f df78 64c3 2408 0479 1c9c  ..../..xd.$..y..
+0005e480: 9a35 082e 0544 9ac6 1ba1 ff15 42ed 2004  .5...D......B. .
+0005e490: c403 333a b680 e035 ae88 01f0 1b10 3806  ..3:...5......8.
+0005e4a0: b41a 4702 28d8 8992 347c f5ed 3630 6076  ..G.(...4|..60`v
+0005e4b0: bfc7 b184 80bb df68 fa81 503c 5010 f69d  .......h..P<P...
+0005e4c0: 220a 5c01 f204 a482 0940 25a0 c0ef 1fb8  ".\......@%.....
+0005e4d0: e046 0bb1 0d76 2674 ddc6 4fc0 1381 74c0  .F...v&t..O...t.
+0005e4e0: 2ef4 8a0d c440 b9fc 1608 6920 577e 5419  .....@....i W~T.
+0005e4f0: a112 c0e0 aa6c 0385 1670 0261 0d68 c504  .....l...p.a.h..
+0005e500: 3562 03d2 db1b 2c20 4102 6d21 4070 09c2  5b...., A.m!@p..
+0005e510: 85e3 07bb 164a 7408 e359 ef86 0d11 35fc  .....Jt..Y....5.
+0005e520: 8405 fc18 1ba2 b406 b086 57fc bb00 6303  ..........W...c.
+0005e530: 90db 4061 00b2 03af 4164 7647 490b d184  ..@a....AdvGI...
+0005e540: 6702 2386 b486 f81b 4c28 3c1a 0f86 03ca  g.#.....L(<.....
+0005e550: 814a 0e0e c614 839c ec51 1138 91e1 42e4  .J.......Q.8..B.
+0005e560: 160c 9882 6f0d 46c6 01ac eb77 cc58 dd60  ....o.F....w.X.`
+0005e570: bcb0 c805 ebd8 0db8 d7a1 4b83 88f3 3b64  ..........K...;d
+0005e580: 02f2 06ba 1c8c c120 3be4 8cef 5358 a1f4  ....... ;...SX..
+0005e590: 6311 4891 df13 ce86 3cec 84fe 5d21 b161  c.H.....<...]!.a
+0005e5a0: 056e 080e 2012 6042 bf3a 9b26 2027 50a2  .n.. .`B.:.& 'P.
+0005e5b0: 1055 0153 6acf 5a81 b706 c0b5 0564 a292  .U.Sj.Z......d..
+0005e5c0: 02d8 0cf6 f0db 0c66 5150 c1be d900 5690  .......fQP....V.
+0005e5d0: 6e7b 280d 123b 2817 2305 2fa2 51ff fc88  n{(..;(.#./.Q...
+0005e5e0: 1056 6ad8 e040 6980 0004 3e6f 5817 bc34  .Vj..@i...>oX..4
+0005e5f0: 60d9 2a22 9c14 084a 3667 2609 c195 d033  `.*"...J6g&....3
+0005e600: 1800 16c8 2d1e 2e00 c100 0a06 81c1 1707  ....-...........
+0005e610: f0b5 83c7 e05e 8331 3398 19ec 58c3 b216  .....^.13...X...
+0005e620: b7c2 1bc4 82da e07e 4424 fc02 870c b5e2  .......~D$......
+0005e630: 8440 f068 7b10 4a36 3183 1bb7 6918 27d0  .@.h{.J61...i.'.
+0005e640: 7070 35ec 1d2c c71e 044a 055c 7838 9b21  pp5..,...J.\x8.!
+0005e650: c118 f024 a054 83ba ecbe 8327 1760 a17b  ...$.T.....'.`.{
+0005e660: 8883 6e2b b802 2077 18b9 8015 110f 5004  ..n+.. w......P.
+0005e670: 8340 8008 4161 0469 385b 06c9 1187 a015  .@..Aa.i8[......
+0005e680: c4d4 7ed8 d6f6 2014 dd70 688c 022c 21c9  ..~... ..ph..,!.
+0005e690: 8173 82d3 db23 5bb8 2401 a4a0 22a5 c15f  .s...#[.$...".._
+0005e6a0: 60af 3688 133c f0e1 3696 1788 e0e0 dab8  `.6..<..6.......
+0005e6b0: 48e0 2b1e 5094 600e 7888 982a 4076 bfe1  H.+.P.`.x..*@v..
+0005e6c0: 300a d147 b44e 0583 2e90 536c 18f4 a806  0..G.N....Sl....
+0005e6d0: d905 f801 a06e 2113 bff0 1905 a070 1616  .....n!......p..
+0005e6e0: 17ec 5a20 bb29 0310 0f46 e830 1b6c 02b1  ..Z .)...F.0.l..
+0005e6f0: a2c7 23eb 719f ce7d 8341 084c fb1d fb74  ..#.q..}.A.L...t
+0005e700: 70c1 c213 ad34 03c1 b091 41a7 8410 5e11  p....4....A...^.
+0005e710: 9406 e402 1618 114b 6548 7818 8c23 17ba  .......KeHx..#..
+0005e720: 7068 0c26 0eca 8131 0254 dffd f293 1b90  ph.&...1.T......
+0005e730: 0b26 b0fb 0fb4 c420 5340 8c20 768c 3cc4  .&..... S@. v.<.
+0005e740: b031 8dd8 3e03 3ec1 f437 adce 8143 3a12  .1..>.>..7...C:.
+0005e750: 7122 b933 eb3e d9e0 073e 1d74 40fc 9889  q".3.>...>.t@...
+0005e760: ec1f 9a0b 03a6 0032 c8b9 4940 8f04 770c  .......2..I@..w.
+0005e770: 6809 3867 2520 8220 4d83 e830 8254 a005  h.8g% . M..0.T..
+0005e780: b825 8108 054d b477 65b3 194c 8a87 0cbf  .%...M.we..L....
+0005e790: 580a 8f51 6005 f005 2ee0 4487 6208 7207  X..Q`.....D.b.r.
+0005e7a0: d122 968d 4330 b4fb ae81 be20 fc80 f835  ."..C0..... ...5
+0005e7b0: 1018 865f 85c4 019d 6cf8 3a88 7e11 341b  ..._....l.:.~.4.
+0005e7c0: c30a 7085 4007 3dcc e1da d491 b682 39ec  ..p.@.=.......9.
+0005e7d0: b803 0f27 e015 c407 943a 7f5b 0811 01ae  ...'.....:.[....
+0005e7e0: 4292 05b5 35c8 c58f 22a4 c022 3786 73b4  B...5...".."7.s.
+0005e7f0: 9c64 b71b 3001 2026 a864 01aa 073d b09f  .d..0. &.d...=..
+0005e800: 05e1 7017 7db0 0648 03a3 fe6e 8616 0b59  ..p.}..H...n...Y
+0005e810: 183c c03a 108c 3f2a 1a19 0cb8 cd9f ac01  .<.:..?*........
+0005e820: 9280 4afc 263c 6718 7888 025e 07de 05e5  ..J.&<g.x..^....
+0005e830: 0b6d 3bd8 62f8 ac41 1960 717e 081b 3f0f  .m;.b..A.`q~..?.
+0005e840: 1076 3c36 bb31 c90d e7be b341 98d0 6936  .v<6.1.....A..i6
+0005e850: 7d44 7b3f be1b 3104 c3ef 6d1e 3eaa a6c1  }D{?..1...m.>...
+0005e860: 0b27 5a08 eec9 3004 403b dd4b 188a c147  .'Z...0.@;.K...G
+0005e870: a8a8 e6aa 38c9 c126 0083 40d3 8c78 670b  ....8..&..@..xg.
+0005e880: f809 6c24 021a 0a90 bc65 21ac 3403 280a  ..l$.....e!.4.(.
+0005e890: b522 a882 870e 34c6 432a d67e 38bf a015  ."....4.C*.~8...
+0005e8a0: f474 212e 71b1 c205 c60f 90c6 0d47 dd78  .t!.q........G.x
+0005e8b0: 5988 a8ff 2444 c169 f981 d28c 4809 2094  Y...$D.i....H. .
+0005e8c0: 9ce1 88d4 b031 6af8 6d1a c1df 7883 0c2b  .....1j.m...x..+
+0005e8d0: f6b5 0618 0a61 f91f b506 2201 c80f 5991  .....a...."...Y.
+0005e8e0: 334d 7e15 101b 6150 63cf c264 82f0 33fc  3M~...aPc..d..3.
+0005e8f0: 33b8 7e12 0619 4b07 cd6b 4a1a 0306 81fd  3.~...K..kJ.....
+0005e900: 90a9 9326 ce16 4014 dd72 8086 85aa ed81  ...&..@..r......
+0005e910: 18ac 4081 b878 66d0 2304 4fe1 fdd0 9b30  ..@..xf.#.O....0
+0005e920: fb98 41c0 2ab3 4f09 c8d9 8111 4805 7730  ..A.*.O.....H.w0
+0005e930: 580c fa26 080b 64a2 fd8a 462d 2dff 1b1d  X..&..d...F--...
+0005e940: 8b8a 0f0c 54d7 3b36 7c0f 012a 7c43 40b5  ....T.;6|..*|C@.
+0005e950: 0ea3 2b7c a700 7c18 0218 78f0 74f8 67e1  ..+|..|...x.t.g.
+0005e960: 7c3d 412c 7c76 80b6 0eb0 2d7c 8d61 7c40  |=A,|v....-|.a|@
+0005e970: 002e 78e0 5df8 b940 7768 3972 f221 57e0  ..x.]..@wh9r.!W.
+0005e980: 09a4 454b 4020 ceb6 d090 ea0e 14db 4b89  ..EK@ ........K.
+0005e990: 65cd 6660 6d5e 2572 2d17 1464 33b1 98ed  e.f`m^%r-..d3...
+0005e9a0: 4a32 5163 9123 225a 49da c1dc 2c6d 4646  J2Qc.#"ZI...,mFF
+0005e9b0: e572 3b2b 9f3a 1320 1d4b 94c3 a48b 75b8  .r;+.:. .K....u.
+0005e9c0: a258 be3a 2419 9d1d a090 6189 b03f 937e  .X.:$.....a..?.~
+0005e9d0: ba06 94cf 3cae 0be5 fe4c a789 4fc2 3d73  ....<....L..O.=s
+0005e9e0: e5d9 7824 092b 7491 3f69 6c90 27ea 2248  ..x$.+t.?il.'."H
+0005e9f0: 6674 816a f347 a8d2 4b62 13f1 0984 d120  ft.j.G..Kb..... 
+0005ea00: 62a2 990f a02b 8250 1a81 5212 8ac5 4a8c  b....+.P..R...J.
+0005ea10: 6802 2652 2ccd 0671 15ae 7144 3a2a d433  h.&R,..q..qD:*.3
+0005ea20: 2124 15e2 b680 4a9d 652c fb77 aa79 4cd5  !$....J.e,.w.yL.
+0005ea30: 695c d41c 8cf0 5b26 5163 bdb8 3b1b 8240  i\....[&Qc..;..@
+0005ea40: 9dca 0ff5 b319 33b5 1211 25de c411 1da8  ......3...%.....
+0005ea50: d1b9 8c44 d959 aea3 6f81 252e b2fb 47ad  ...D.Y..o.%...G.
+0005ea60: 3ea5 b143 8c4f 265d 9128 9cad 08b7 b911  >..C.O&].(......
+0005ea70: e50c 4411 f565 8d48 366e 4e74 6590 8fe8  ..D..e.H6nNte...
+0005ea80: 8e7b 34e3 408b 950a 4b34 28fe 41cf bec2  .{4.@...K4(.A...
+0005ea90: 98fb 4a6a a194 e419 b334 1bd1 d273 6f94  ..Jj.....4...so.
+0005eaa0: ba69 d1ab e567 71bd 621a 243e 25ed 8df5  .i...gq.b.$>%...
+0005eab0: 793d a618 bace c44f c856 e8f5 7bd1 b357  y=.....O.V..{..W
+0005eac0: 089e def1 2325 6afc ab59 bbb6 1f27 739e  ....#%j..Y...'s.
+0005ead0: d65d 320b d24e a719 ac91 e951 b51e 2175  .]2..N.....Q..!u
+0005eae0: 6920 052c 5cb8 a9ab bb0a e639 243a cee1  i .,\......9$:..
+0005eaf0: 22f9 9aa1 1b9a 6976 1a1e a445 61e2 133a  ".....iv...Ea..:
+0005eb00: 7427 74c4 6033 d2b3 a784 b830 d9a4 7a01  t't.`3.....0..z.
+0005eb10: 7227 d915 4932 db30 d812 2864 5c4f ad12  r'..I2.0..(d\O..
+0005eb20: 46e3 2265 5732 c989 47d1 607a ffd4 4b11  F."eW2..G.`z..K.
+0005eb30: c693 d486 4c40 cd13 4fb6 1a1f 44be 7d4c  ....L@..O...D.}L
+0005eb40: eb0e 4c27 9109 0761 e0a1 f2e4 b2c0 eb6c  ..L'...a.......l
+0005eb50: 9aad 974a 8b2f 0ecc a7b8 0852 b5ca 6a5e  ...J./.....R..j^
+0005eb60: 1105 ed13 65c6 814c 93a3 8909 554a b2e8  ....e..L....UJ..
+0005eb70: 393b e934 b61e 8fd5 a6e8 4c43 a20f bbb8  9;.4......LC....
+0005eb80: 13ca 0330 606b ed9c 422a d496 c286 9b22  ...0`k..B*....."
+0005eb90: 542f 6b99 d110 10d9 5b96 d2bd d25b 1586  T/k.....[....[..
+0005eba0: 4e20 83b9 2d55 1220 a5a1 0cd9 ba34 376a  N ..-U. .....47j
+0005ebb0: 7e56 7525 2eb7 749b 4a0d 8e58 a49a 8ef9  ~Vu%..t.J..X....
+0005ebc0: 2f6c 5853 e311 63be 199c d6e0 887d d84e  /lXS..c......}.N
+0005ebd0: b332 3b61 011d cafc 3e42 9d23 4824 8adc  .2;a....>B.#H$..
+0005ebe0: cf0c dbb8 d30d 1291 ea98 4ef3 cfd3 c39a  ..........N.....
+0005ebf0: 6747 be68 1e4d 2c0d 1345 d0c5 73b2 b144  gG.h.M,..E..s..D
+0005ec00: 72bb 4a82 4b32 f1e9 1d98 d09c 32a1 ca3e  r.J.K2......2..>
+0005ec10: ac9f 0906 9af0 ada4 7e5a 2734 c269 f05e  ........~Z'4.i.^
+0005ec20: 9367 f056 9d8d 207d d9ac a335 8c0c 2686  .g.V.. }...5..&.
+0005ec30: af5a 4ddf 3e7b 9024 a980 c346 ac4d bfe0  .ZM.>{.$...F.M..
+0005ec40: 1225 db4f 26eb f0d8 27cd 2a40 6a95 1e6f  .%.O&...'.*@j..o
+0005ec50: c41a 26a4 768a 37d3 859d 044d c9ed 2aa5  ..&.v.7....M..*.
+0005ec60: a470 4c1d ec51 ffe4 383f 0d8c a06b 8bed  .pL..Q..8?...k..
+0005ec70: a473 f0e0 456a 1302 e4b3 ccb9 6470 0b88  .s..Ej......dp..
+0005ec80: 26b3 a7cb a133 538b c404 b310 a14e 7d4c  &....3S......N}L
+0005ec90: 0fea 6b44 2a6c 72a1 a404 4eb8 d2f5 06c5  ..kD*lr...N.....
+0005eca0: ed1f e3c2 96ae 0b55 ab51 50da 6a8b 45d9  .......U.QP.j.E.
+0005ecb0: ce08 c7ce aef9 ea3b f33c e2c9 5568 2ff5  .......;.<..Uh/.
+0005ecc0: a72c 5f3c 1c35 4390 5f42 9e37 86e7 cdb2  .,_<.5C._B.7....
+0005ecd0: 4e84 a06f 5ccf 48c1 dbb9 5a09 ef99 ada3  N..o\.H...Z.....
+0005ece0: 28ef 5147 0d66 2c4a 9e7f c774 0edd 967d  (.QG.f,J...t...}
+0005ecf0: 397d 1ddb de79 5dbd e90a 223e 7f31 2df5  9}...y]...">.1-.
+0005ed00: 0e16 878e ecf2 43f4 6f14 9e19 188d 262f  ......C.o.....&/
+0005ed10: 7ddb df09 92a3 9d0d 09a2 3f4d a075 e376  }.........?M.u.v
+0005ed20: b684 04ce afc1 d02d 80a7 0ce8 1556 911e  .......-.....V..
+0005ed30: 1eb8 e225 5960 7d2a 9424 8426 9ac4 2ce5  ...%Y`}*.$.&..,.
+0005ed40: 5ab4 14b0 1247 df71 285b e0b1 10b3 7b8a  Z....G.q([....{.
+0005ed50: aa96 9851 a206 6248 7058 a355 c7cf d19d  ...Q..bHpX.U....
+0005ed60: 124d 6e93 51aa 7be7 9a39 b20a 6dca 8f86  .Mn.Q.{..9..m...
+0005ed70: 0c7d 60a2 7d8e 2dcb 041f f919 436c d42f  .}`.}.-.....Cl./
+0005ed80: 4b4a daa8 c4b9 5b23 d28c 016a fb77 4b4a  KJ....[#...j.wKJ
+0005ed90: c2c5 d193 bb86 a694 d276 513a 5593 848e  .........vQ:U...
+0005eda0: d74e 1f0b 5ca6 b643 8994 d769 f476 40c9  .N..\..C...i.v@.
+0005edb0: 1d23 b30b 52f5 46d5 5673 9bc0 cc26 b729  .#..R.F.Vs...&.)
+0005edc0: b0f1 c112 7212 9a18 d86d 221b 6577 3295  ....r....m".ew2.
+0005edd0: db54 d2c8 5889 7693 3ad7 a46e b32c 6ed8  .T..X.v.:..n.,n.
+0005ede0: 3551 da54 d2d8 8008 4d75 e532 a156 2096  5Q.T....Mu.2.V .
+0005edf0: a877 6eef b60a d330 8824 abd5 2ac9 42e1  .wn....0.$..*.B.
+0005ee00: 9a52 7527 73a2 9155 860f efd4 7549 64a1  .Ru's..U....uId.
+0005ee10: 78c2 b8ef 3cd4 7854 7256 431a 1337 8213  x...<.xTrVC..7..
+0005ee20: d3a4 70ba 3448 abef 5233 0d65 5172 56df  ..p.4H..R3.eQrV.
+0005ee30: 5504 208c 2568 59c2 1b30 102b f814 319d  U. .%hY..0.+..1.
+0005ee40: b75a c0de 602f c2e5 b044 35ec 7562 b615  .Z..`/...D5.ub..
+0005ee50: 1881 5059 a802 5c22 eb0f 3a35 da08 a8d3  ..PY..\"..:5....
+0005ee60: 1bc4 756a 4f44 29a3 2c01 b768 a50a 322c  ..ujOD).,..h..2,
+0005ee70: c1d1 741e aa7a 0ba5 ee94 0145 943f aa48  ..t..z.....E.?.H
+0005ee80: 63b8 494c 39bb abbe 5c55 420d 553c f68c  c.IL9...\UB.U<..
+0005ee90: ae9a 6988 4fcc 8e5e 20b7 6bab e742 113e  ..i.O..^ .k..B.>
+0005eea0: 3b76 ab55 c146 8010 ac92 edc2 a15b e0f3  ;v.U.F.......[..
+0005eeb0: 4aa7 db68 756c 0079 9471 9317 ca36 60bd  J..hul.y.q...6`.
+0005eec0: f126 35f1 5b5a 5dbd f047 da4c fbe4 5741  .&5.[Z]..G.L..WA
+0005eed0: c095 8a85 543c 7a8d ba45 7f6f 111d 2f55  ....T<z..E.o../U
+0005eee0: b846 199c b4bf bb46 17df 8250 01e9 2a2d  .F.....F...P..*-
+0005eef0: d783 c6a6 93bb 2ff1 bc97 f502 8c83 c82a  ....../........*
+0005ef00: 93c4 e938 2dab 63a3 7e93 ba53 d6b3 0695  ...8-.c.~..S....
+0005ef10: 41a5 5d25 9e55 88b4 8c3f c485 ecc5 d5e4  A.]%.U...?......
+0005ef20: 7db4 ec9c 140e 45da 6e6e 5a19 9650 662c  }.....E.nnZ..Pf,
+0005ef30: b70e 1b5e 1319 bdd7 e29e 3858 6dd5 e874  ...^......8Xm..t
+0005ef40: 77e9 2b2d ac04 061d f4be 86f8 9e19 52d8  w.+-..........R.
+0005ef50: 1253 305f ebe8 c184 f873 25e1 f4b3 37a4  .S0_.....s%...7.
+0005ef60: 0bc4 927a 3a47 485b 59d6 d531 ea94 178b  ...z:GH[Y..1....
+0005ef70: 35ff 63b5 7945 4662 5204 5a22 7592 548c  5.c.yEFbR.Z"u.T.
+0005ef80: efe0 c223 9514 ddf4 8435 4727 574a 54e7  ...#.....5G'WJT.
+0005ef90: ecda 036e dcaf 895a fd8a 4f07 02d2 4d5c  ...n...Z..O...M\
+0005efa0: f26a 60b7 9666 5a37 13ad 1db7 af48 2377  .j`..fZ7.....H#w
+0005efb0: c523 2b61 ef6b c92b 619b 8fa6 0810 96dc  .#+a.k.+a.......
+0005efc0: 65bf f906 4c24 db5e 6007 00d4 e0f9 dd99  e...L$.^`.......
+0005efd0: 7a6d b0c2 ce11 4280 fd49 865d 343a 4bf5  zm....B..I.]4:K.
+0005efe0: 0fe5 d625 0127 6697 dc50 6a50 20b1 5f8d  ...%.'f..PjP ._.
+0005eff0: 59db be9c 6379 1a6b 2dd7 cb8a b846 edd8  Y...cy.k-....F..
+0005f000: 6403 a2e4 7558 bbb5 b424 2533 cf84 57b4  d...uX...$%3..W.
+0005f010: 94ac 2890 d474 5295 6757 8cd2 a0cc 5222  ..(..tR.gW....R"
+0005f020: 8e56 add0 7bc4 c610 bc3b a9df 0c8b 621c  .V..{....;....b.
+0005f030: 3206 56d9 d1b4 7a07 d772 a750 b47a 82d2  2.V...z..r.P.z..
+0005f040: 1dea 6f8c 6905 9ad0 2e76 c669 c9e6 a6ca  ..o.i....v.i....
+0005f050: 13ad 2941 6d1d 94e7 2155 3a4d 3c9b 8f9a  ..)Am...!U:M<...
+0005f060: aaea ab9c ed23 357a 5668 70a9 4774 2382  .....#5zVhp.Gt#.
+0005f070: aac8 a2f6 c4a3 4fd0 31c4 6355 d365 360d  ......O.1.cU.e6.
+0005f080: 889d a1b4 b730 f91f 03fd b4ce 0fc9 27b8  .....0........'.
+0005f090: bb7c 0d0b 5c77 aa43 34b8 b871 b1d4 9728  .|..\w.C4..q...(
+0005f0a0: 5ba6 fb84 00cd 2584 1327 b3d4 07cc 787a  [.....%..'....xz
+0005f0b0: 7d34 e8e2 46cf 741a 4d60 7b24 715d 162e  }4..F.t.M`{$q]..
+0005f0c0: 01f4 972d db24 5495 8828 50d1 2556 3a57  ...-.$T..(P.%V:W
+0005f0d0: f350 b1aa d515 ea6c 3e57 678f 4e46 d8d9  .P.....l>Wg.NF..
+0005f0e0: 31d2 3b97 a36f 9405 c83e 760b 110d 55c3  1.;..o...>v...U.
+0005f0f0: 1002 1ac4 153a a7b0 e7df 4e17 25e8 026a  .....:....N.%..j
+0005f100: 534c 6e97 bea7 c58b 4700 0a8d 59df 84d4  SLn.....G...Y...
+0005f110: 4c9e 2f23 8d49 5abb 72fe c449 3f27 eb43  L./#.IZ.r..I?'.C
+0005f120: 007a 0978 a133 b78e 1406 90d8 ad6b 6b32  .z.x.3.......kk2
+0005f130: b8ba 51c5 1b61 2dd8 e35d 4ae3 74a2 9170  ..Q..a-..]J.t..p
+0005f140: 2ede 70f2 93d1 2e13 adf3 f6bb 3621 4198  ..p.........6!A.
+0005f150: a304 d70b e048 8215 3528 5f05 d723 f651  .....H..5(_..#.Q
+0005f160: a075 92c0 c68a aeaf 9ac3 4b8f 51f9 7bf6  .u........K.Q.{.
+0005f170: a479 8a0d f231 4a94 e635 b1f7 6b79 318f  .y...1J..5..ky1.
+0005f180: 9d52 ad5e 4f9c b620 f75a bd54 06d2 a1c1  .R.^O.. .Z.T....
+0005f190: 6089 9853 c8b4 8082 6169 bca3 57be 374d  `..S....ai..W.7M
+0005f1a0: 6c9b 05b3 84af ab15 ecff ba89 51df 8278  l...........Q..x
+0005f1b0: af79 2933 4e2d 43fe 1eb1 9298 da4b c1a7  .y)3N-C......K..
+0005f1c0: 548a 3a12 5bcf 936a 988d 88a2 7f83 35bd  T.:.[..j......5.
+0005f1d0: 8649 93a7 bf12 bfad 4a35 c7b6 4665 2be5  .I......J5..Fe+.
+0005f1e0: 9b93 58fe 0926 56e2 5d2f fcc5 e3fb 860f  ..X..&V.]/......
+0005f1f0: 4d27 c037 cd64 ce51 f49a 8beb 0278 797e  M'.7.d.Q.....xy~
+0005f200: 7e16 7675 1ec7 af6b 938c 1023 03f1 8211  ~.vu...k...#....
+0005f210: 8e90 9efb 0cea 29eb ba82 2c8d 0895 2757  ......)...,...'W
+0005f220: 60db d0bb 28c2 1dc5 28c7 7536 4f43 8492  `...(...(.u6OC..
+0005f230: 25a1 5b5a f908 70b6 f348 9c56 3ce1 92b4  %.[Z..p..H.V<...
+0005f240: 6718 fd70 abbe 8a09 740c 064d 5d64 13ee  g..p....t..M]d..
+0005f250: c61d 53bb ae8e 36d5 6457 b30a 2811 1aac  ..S...6.dW..(...
+0005f260: 2a4c 7a00 593e c6ca 0d07 1a66 254b b611  *Lz.Y>.....f%K..
+0005f270: 3cfd 966d b29b 9748 25d9 ee55 a74d a27a  <..m...H%..U.M.z
+0005f280: c545 e626 4cdb 860e b62e e3ce 7918 0234  .E.&L.......y..4
+0005f290: 79ab 4a22 fb98 b80e 7a19 342e 551b d06e  y.J"....z.4.U..n
+0005f2a0: fe0e ddcc ad3f b7b0 fc5d 6d8a 3a85 339e  .....?...]m.:.3.
+0005f2b0: 52b1 1519 e854 2a2e 8963 9acb 27af 11c3  R....T*..c..'...
+0005f2c0: c7d9 9e12 c233 9698 021d 7a23 ce86 7aa3  .....3....z#..z.
+0005f2d0: 5934 2b92 f47c c564 3441 7a55 6567 1990  Y4+..|.d4AzUeg..
+0005f2e0: 64e2 6025 b7a3 ab65 1c09 4df8 0a35 8b9b  d.`%...e..M..5..
+0005f2f0: 85a8 ea28 8aca fe62 f82e 9935 4430 a7aa  ...(...b...5D0..
+0005f300: 7e85 0409 18b2 0b5c 04ee f227 30d1 6acd  ~......\...'0.j.
+0005f310: e718 6110 8999 ee5d ed84 fe40 6b28 c664  ..a....]...@k(.d
+0005f320: 8e77 8dca 0ca4 2245 e1dc 02d6 aae4 0c1a  .w...."E........
+0005f330: bd8f 0f68 a0e8 3277 7afb e905 9858 f408  ...h..2wz....X..
+0005f340: b4bb 3e1e 2f2a dbd7 f259 3b86 d749 459e  ..>./*...Y;..IE.
+0005f350: 098c 5bd6 d96c 960c c4ce 05c2 4b1e c86f  ..[..l......K..o
+0005f360: 4166 6a22 9625 8152 9a91 82c0 a1f4 5e3b  Afj".%.R......^;
+0005f370: 5b95 5323 ff0b 1041 dec3 23cb f629 6546  [.S#...A..#..)eF
+0005f380: 9b56 7120 f33e b4fb 9508 4ab7 894b a981  .Vq .>....J..K..
+0005f390: e891 b1a0 769a 0049 3a65 9708 3134 baf0  ....v..I:e..14..
+0005f3a0: ee6c 1392 2f30 5c15 8c9e 4e0c d444 5c46  .l../0\...N..D\F
+0005f3b0: 78b2 b290 214c a601 94a1 8591 90e4 369d  x...!L........6.
+0005f3c0: 5967 5394 3d19 4258 2698 a93c 79e0 1773  YgS.=.BX&..<y..s
+0005f3d0: 3ad5 a9ac dae8 ac41 8d69 5999 5bfc 8c05  :......A.iY.[...
+0005f3e0: 5889 b891 d265 c547 4469 8918 64f6 9697  X....e.GDi..d...
+0005f3f0: 6d33 86a3 d932 4798 7087 44fa ab7a cd6b  m3...2G.p.D..z.k
+0005f400: 6c2d 94e6 2668 5e9f 49f3 bd43 1b35 d089  l-..&h^.I..C.5..
+0005f410: e6b5 23a8 44e2 c2a6 a576 cd9d 064e 20d3  ..#.D....v...N .
+0005f420: d809 9218 eee6 4501 af88 630e 9d23 8ca2  ......E...c..#..
+0005f430: c454 3a40 ce3c 6479 613a 36ac 77e9 986d  .T:@.<dya:6.w..m
+0005f440: 8a0c 8a78 1d8f 7d0e 6e98 509e 6d26 8c72  ...x..}.n.P.m&.r
+0005f450: d2e8 0135 4630 39a5 85de 6334 0331 ed75  ...5F09...c4.1.u
+0005f460: 5aee 9114 499d dd09 0ef6 bd7d 32b8 2250  Z...I......}2."P
+0005f470: e756 754e 075e f828 4c8a 47f6 c05b 6267  .VuN.^.(L.G..[bg
+0005f480: b59e 1cd6 7b1d 95c0 444f 7660 68c8 06c8  ....{...DOv`h...
+0005f490: 2618 5cb8 8da6 2eb0 e132 d335 37ec d173  &.\......2.57..s
+0005f4a0: 441a 9ba3 552a d2ef ad8a 6344 4bc4 970e  D...U*....cDK...
+0005f4b0: 34be 0287 3d2b 1ee3 4e97 f30c 8cb8 5357  4...=+..N.....SW
+0005f4c0: e6dd 7a40 e576 99ae 777b 8dc5 9878 079b  ..z@.v..w{...x..
+0005f4d0: 3bb5 86d8 c3b5 4147 8d44 a5e9 7783 5550  ;.....AG.D..w.UP
+0005f4e0: 24a2 3446 50f4 46c8 1ae1 43a4 b650 5e37  $.4FP.F...C..P^7
+0005f4f0: 138f 3e43 516f 0a9a d2a1 3a88 7f09 7e76  ..>CQo....:...~v
+0005f500: d811 adad bd48 77df 07d0 434b b313 6ccb  .....Hw...CK..l.
+0005f510: e3a1 a871 be5a 718a 57de 5506 1248 55f9  ...q.Zq.W.U..HU.
+0005f520: f7b4 8d93 a9b3 e252 d962 da6a f89c a655  .......R.b.j...U
+0005f530: 35f1 e873 332f 9c41 848f 10cc bcaa 42e7  5..s3/.A......B.
+0005f540: 366d 0288 964a a0a8 3f59 2d8e daab d1a4  6m...J..?Y-.....
+0005f550: f9bc 611f ec88 7a75 b3e1 e133 5cb9 22e6  ..a...zu...3\.".
+0005f560: acc1 82a7 2092 5996 47de d759 a0f1 94d8  .... .Y.G..Y....
+0005f570: 6bbd 1706 d55b b7f9 e224 ea26 6d7b 446f  k....[...$.&m{Do
+0005f580: 2933 8558 f673 772d e60a 7aeb fbea 7d9f  )3.X.sw-..z...}.
+0005f590: 0c5a 8034 e8e9 f3ef 5854 df29 5d01 ba97  .Z.4....XT.)]...
+0005f5a0: 9f25 f8cc ebe7 54ac f56a ba3a 89bf 6d7c  .%....T..j.:..m|
+0005f5b0: f72f ffe4 6ceb 097f bc37 7f6d 16e6 e0d7  ./..l....7.m....
+0005f5c0: 175a a48d c3b8 ab2a ab2d 16ff 762d 58a3  .Z.....*.-..v-X.
+0005f5d0: d4ac 40ff bff5 e4c9 1fdf 522b 80bf 7fdd  ..@.......R+....
+0005f5e0: 11ff 8d27 59c5 ad5b adaf dcf8 fc77 beb0  ...'Y..[.....w..
+0005f5f0: 6a05 ee5b f24e 2eb5 4dfe f185 9a39 b156  j..[.N..M....9.V
+0005f600: 570a 56b9 379f b7d3 f1ba d5b9 ed95 ee8f  W.V.7...........
+0005f610: 3b9d f4e6 12fe 4b8b 37de dd3b e7a9 e9cd  ;.....K.7..;....
+0005f620: 10df 4a7e eafd 7cd6 97df 9cf9 fdb5 7f5f  ..J~..|........_
+0005f630: daf3 80c3 0810 0200 0000 4363 3033 0000  ..........Cc03..
 0005f640: 0b65 19e5 001f 0277 a4d5 7fb8 f089 3982  .e.....w......9.
 0005f650: 7d1c 9b10 386d 77f9 63e4 745b 7397 eab6  }...8mw.c.t[s...
 0005f660: d6ee 3b47 17c2 efbf 41fe 0080 9101 2b1a  ..;G....A.....+.
 0005f670: 0080 3930 2961 9484 4974 be69 3718 89e2  ..90)a..It.i7...
 0005f680: c4f0 2d0b 0972 917b d8fe 7b17 2b70 60d9  ..-..r.{..{.+p`.
 0005f690: eede 6df7 65bf f701 0f2a 51b1 e5de 7dcd  ..m.e....*Q...}.
 0005f6a0: d096 d8f4 d143 3ec2 6d99 98be 9e96 c899  .....C>.m.......
```

### Comparing `guidata-3.0.1/guidata/guitest.py` & `guidata-3.0.2/guidata/guitest.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/apply.png` & `guidata-3.0.2/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/arredit.png` & `guidata-3.0.2/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/busy.png` & `guidata-3.0.2/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/cell_edit.png` & `guidata-3.0.2/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/copy.png` & `guidata-3.0.2/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/delete.png` & `guidata-3.0.2/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/dictedit.png` & `guidata-3.0.2/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/dtype.png` & `guidata-3.0.2/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/edit.png` & `guidata-3.0.2/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/copywop.png` & `guidata-3.0.2/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/edit.png` & `guidata-3.0.2/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/edit_add.png` & `guidata-3.0.2/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/editclear.png` & `guidata-3.0.2/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/editcopy.png` & `guidata-3.0.2/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/editcut.png` & `guidata-3.0.2/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/editdelete.png` & `guidata-3.0.2/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/editpaste.png` & `guidata-3.0.2/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/fileimport.png` & `guidata-3.0.2/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/filesave.png` & `guidata-3.0.2/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/imshow.png` & `guidata-3.0.2/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/insert.png` & `guidata-3.0.2/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/plot.png` & `guidata-3.0.2/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/rename.png` & `guidata-3.0.2/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/editors/selectall.png` & `guidata-3.0.2/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/exit.png` & `guidata-3.0.2/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/file.png` & `guidata-3.0.2/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/fileclose.png` & `guidata-3.0.2/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/fileimport.png` & `guidata-3.0.2/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/fileopen.png` & `guidata-3.0.2/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filesave.png` & `guidata-3.0.2/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filesaveas.png` & `guidata-3.0.2/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/doc.png` & `guidata-3.0.2/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/gif.png` & `guidata-3.0.2/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/html.png` & `guidata-3.0.2/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/jpg.png` & `guidata-3.0.2/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/pdf.png` & `guidata-3.0.2/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/png.png` & `guidata-3.0.2/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/pps.png` & `guidata-3.0.2/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/ps.png` & `guidata-3.0.2/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/tar.png` & `guidata-3.0.2/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/tgz.png` & `guidata-3.0.2/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/tif.png` & `guidata-3.0.2/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/txt.png` & `guidata-3.0.2/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/xls.png` & `guidata-3.0.2/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/filetypes/zip.png` & `guidata-3.0.2/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/guidata-banner.svg` & `guidata-3.0.2/guidata/images/guidata-banner.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/guidata-vertical.svg` & `guidata-3.0.2/guidata/images/guidata-vertical.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/guidata.svg` & `guidata-3.0.2/guidata/images/guidata.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/not_found.png` & `guidata-3.0.2/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/python.png` & `guidata-3.0.2/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/quickview.png` & `guidata-3.0.2/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/save_all.png` & `guidata-3.0.2/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/selection.png` & `guidata-3.0.2/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/images/settings.png` & `guidata-3.0.2/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.0.2/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/qthelpers.py` & `guidata-3.0.2/guidata/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/_all_tests.py` & `guidata-3.0.2/guidata/tests/_all_tests.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/data/genreqs/pyproject.toml` & `guidata-3.0.2/guidata/tests/data/genreqs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/data/genreqs/setup.cfg` & `guidata-3.0.2/guidata/tests/data/genreqs/setup.cfg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_activable_dataset.py` & `guidata-3.0.2/guidata/tests/test_activable_dataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_activable_items.py` & `guidata-3.0.2/guidata/tests/test_activable_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_all_features.py` & `guidata-3.0.2/guidata/tests/test_all_features.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_all_items.py` & `guidata-3.0.2/guidata/tests/test_all_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_arrayeditor.py` & `guidata-3.0.2/guidata/tests/test_arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_bool_selector.py` & `guidata-3.0.2/guidata/tests/test_bool_selector.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_callbacks.py` & `guidata-3.0.2/guidata/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_codeeditor.py` & `guidata-3.0.2/guidata/tests/test_codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_collectionseditor.py` & `guidata-3.0.2/guidata/tests/test_collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_config.py` & `guidata-3.0.2/guidata/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_console.py` & `guidata-3.0.2/guidata/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_data.py` & `guidata-3.0.2/guidata/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_dataframeeditor.py` & `guidata-3.0.2/guidata/tests/test_dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_datasetgroup.py` & `guidata-3.0.2/guidata/tests/test_datasetgroup.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_disthelpers.py` & `guidata-3.0.2/guidata/tests/test_disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_editgroupbox.py` & `guidata-3.0.2/guidata/tests/test_editgroupbox.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_genreqs.py` & `guidata-3.0.2/guidata/tests/test_genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_importwizard.py` & `guidata-3.0.2/guidata/tests/test_importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_inheritance.py` & `guidata-3.0.2/guidata/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_item_order.py` & `guidata-3.0.2/guidata/tests/test_item_order.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_loadsave_hdf5.py` & `guidata-3.0.2/guidata/tests/test_loadsave_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,13 @@
             writer.close()
 
             e = Parameters()
             reader = HDF5Reader("test.h5")
             e.deserialize(reader)
             reader.close()
             e.edit()
+            os.unlink("test.h5")
         execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_loadsave_hdf5()
```

### Comparing `guidata-3.0.1/guidata/tests/test_loadsave_json.py` & `guidata-3.0.2/guidata/tests/test_loadsave_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,13 @@
             e.serialize(writer)
             writer.save()
 
             e = Parameters()
             reader = JSONReader("test.json")
             e.deserialize(reader)
             e.edit()
+            os.unlink("test.json")
         execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_loadsave_json()
```

### Comparing `guidata-3.0.1/guidata/tests/test_no_qt.py` & `guidata-3.0.2/guidata/tests/test_no_qt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_objecteditor.py` & `guidata-3.0.2/guidata/tests/test_objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_rotatedlabel.py` & `guidata-3.0.2/guidata/tests/test_rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_text.py` & `guidata-3.0.2/guidata/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/tests/test_userconfig_app.py` & `guidata-3.0.2/guidata/tests/test_userconfig_app.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/userconfig.py` & `guidata-3.0.2/guidata/userconfig.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/__init__.py` & `guidata-3.0.2/guidata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/disthelpers.py` & `guidata-3.0.2/guidata/utils/disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/encoding.py` & `guidata-3.0.2/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/genreqs.py` & `guidata-3.0.2/guidata/utils/genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/gettext_helpers.py` & `guidata-3.0.2/guidata/utils/gettext_helpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/utils/misc.py` & `guidata-3.0.2/guidata/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/__init__.py` & `guidata-3.0.2/guidata/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/arrayeditor.py` & `guidata-3.0.2/guidata/widgets/arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/codeeditor.py` & `guidata-3.0.2/guidata/widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/collectionseditor.py` & `guidata-3.0.2/guidata/widgets/collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/__init__.py` & `guidata-3.0.2/guidata/widgets/console/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/base.py` & `guidata-3.0.2/guidata/widgets/console/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/calltip.py` & `guidata-3.0.2/guidata/widgets/console/calltip.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/dochelpers.py` & `guidata-3.0.2/guidata/widgets/console/dochelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/internalshell.py` & `guidata-3.0.2/guidata/widgets/console/internalshell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/interpreter.py` & `guidata-3.0.2/guidata/widgets/console/interpreter.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/mixins.py` & `guidata-3.0.2/guidata/widgets/console/mixins.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/shell.py` & `guidata-3.0.2/guidata/widgets/console/shell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/console/terminal.py` & `guidata-3.0.2/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/dataframeeditor.py` & `guidata-3.0.2/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/dockable.py` & `guidata-3.0.2/guidata/widgets/dockable.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/importwizard.py` & `guidata-3.0.2/guidata/widgets/importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/nsview.py` & `guidata-3.0.2/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/objecteditor.py` & `guidata-3.0.2/guidata/widgets/objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/rotatedlabel.py` & `guidata-3.0.2/guidata/widgets/rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/syntaxhighlighters.py` & `guidata-3.0.2/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata/widgets/texteditor.py` & `guidata-3.0.2/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.1/guidata.egg-info/PKG-INFO` & `guidata-3.0.2/guidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.0.1
+Version: 3.0.2
 Summary: Signal and image processing software
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `guidata-3.0.1/guidata.egg-info/SOURCES.txt` & `guidata-3.0.2/guidata.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
+doc/basic_example.py
+doc/conf.py
+doc/examples.rst
+doc/index.rst
+doc/installation.rst
+doc/overview.rst
+doc/requirements.rst
+doc/_static/favicon.ico
+doc/dev/contribute.rst
+doc/dev/howto.rst
+doc/dev/index.rst
+doc/dev/v2_to_v3.csv
+doc/dev/v2_to_v3.rst
+doc/images/basic_example.png
+doc/images/guidata-banner.png
+doc/images/guidata-vertical.png
+doc/images/layout_example.png
+doc/images/screenshots/__init__.png
+doc/images/screenshots/activable_dataset.png
+doc/images/screenshots/all_features.png
+doc/images/screenshots/all_items.png
+doc/images/screenshots/bool_selector.png
+doc/images/screenshots/datasetgroup.png
+doc/images/screenshots/editgroupbox.png
+doc/reference/guitest.rst
+doc/reference/index.rst
+doc/reference/userconfig.rst
+doc/reference/utils.rst
+doc/reference/widgets.rst
+doc/reference/dataset/dataitems.rst
+doc/reference/dataset/datatypes.rst
+doc/reference/dataset/index.rst
+doc/reference/dataset/io.rst
+doc/reference/dataset/qtwidgets.rst
 guidata/__init__.py
 guidata/config.py
 guidata/configtools.py
 guidata/env.py
 guidata/guidata.chm
 guidata/guitest.py
 guidata/qthelpers.py
```

### Comparing `guidata-3.0.1/pyproject.toml` & `guidata-3.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "guidata"
-authors = [{name = "Codra", email = "p.raybaut@codra.fr"}]
+authors = [{ name = "Codra", email = "p.raybaut@codra.fr" }]
 description = "Signal and image processing software"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = [
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Software Development :: User Interfaces",
@@ -24,53 +24,40 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: OS Independent",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8, <4"
-dependencies = [
-    "h5py>=3.0",
-    "NumPy>=1.21",
-    "QtPy>=1.9",
-    "requests",
-    "tomli"
-]
+dependencies = ["h5py>=3.0", "NumPy>=1.21", "QtPy>=1.9", "requests", "tomli"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/CODRA-Ingenierie-Informatique/guidata/"
 Documentation = "https://guidata.readthedocs.io/en/latest/"
 
 [project.scripts]
 
 [project.optional-dependencies]
-dev = [
-    "black",
-    "isort",
-    "pylint",
-    "Coverage"
-]
+dev = ["black", "isort", "pylint", "Coverage"]
 doc = [
     "PyQt5",
     "pillow",
     "pandas",
     "sphinx",
     "sphinx-copybutton",
     "sphinx_qt_documentation",
-    "python-docs-theme"
-]
-test = [
-    "pytest",
-    "pytest-cov",
-    "pytest-qt",
-    "pytest-xvfb",
+    "python-docs-theme",
 ]
+test = ["pytest", "pytest-cov", "pytest-qt", "pytest-xvfb"]
+
+[tool.setuptools.packages.find]
+include = ["guidata*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.png", "*.svg", "*.mo", "*.chm", "*.cfg", "*.toml"]
 
 [tool.setuptools.dynamic]
-version = {attr = "guidata.__version__"}
+version = { attr = "guidata.__version__" }
```

