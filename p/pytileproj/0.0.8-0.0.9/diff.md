# Comparing `tmp/pytileproj-0.0.8.tar.gz` & `tmp/pytileproj-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytileproj-0.0.8.tar", last modified: Wed Oct 17 14:22:20 2018, max compression
+gzip compressed data, was "dist\pytileproj-0.0.9.tar", last modified: Tue Nov 27 15:16:32 2018, max compression
```

## Comparing `pytileproj-0.0.8.tar` & `pytileproj-0.0.9.tar`

### file list

```diff
@@ -1,793 +1,793 @@
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/
--rw-rw-rw-   0        0        0      568 2017-08-24 14:09:00.000000 pytileproj-0.0.8/.coveragerc
--rw-rw-rw-   0        0        0     1374 2018-10-17 13:53:01.000000 pytileproj-0.0.8/.travis.yml
--rw-rw-rw-   0        0        0      172 2018-01-31 16:11:53.000000 pytileproj-0.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0      434 2018-08-06 11:04:53.000000 pytileproj-0.0.8/CHANGES.rst
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/docs/
--rw-rw-rw-   0        0        0       43 2017-08-24 14:09:00.000000 pytileproj-0.0.8/docs/authors.rst
--rw-rw-rw-   0        0        0       43 2017-08-24 14:09:00.000000 pytileproj-0.0.8/docs/changes.rst
--rw-rw-rw-   0        0        0     8999 2018-08-06 11:04:53.000000 pytileproj-0.0.8/docs/conf.py
--rw-rw-rw-   0        0        0      288 2018-08-06 11:04:53.000000 pytileproj-0.0.8/docs/index.rst
--rw-rw-rw-   0        0        0       81 2017-08-24 14:09:00.000000 pytileproj-0.0.8/docs/license.rst
--rw-rw-rw-   0        0        0     6952 2017-08-24 14:09:00.000000 pytileproj-0.0.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/docs/_static/
--rw-rw-rw-   0        0        0       19 2017-08-24 14:09:00.000000 pytileproj-0.0.8/docs/_static/.gitignore
--rw-rw-rw-   0        0        0     1128 2018-01-31 16:11:53.000000 pytileproj-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     5019 2018-10-17 14:22:20.000000 pytileproj-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/
--rw-rw-rw-   0        0        0    38504 2018-10-17 13:20:18.000000 pytileproj-0.0.8/pytileproj/base.py
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/
--rw-rw-rw-   0        0        0    14701 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0  1621156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0     1092 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    23044 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    23044 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    22564 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    22564 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    14020 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    11860 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13948 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    11428 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13948 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    11428 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13540 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shx
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/
--rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.dbf
--rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.prj
--rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shp
--rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shx
--rw-rw-rw-   0        0        0     4914 2018-07-13 12:19:57.000000 pytileproj-0.0.8/pytileproj/data/utm/make_utmdata.py
--rw-rw-rw-   0        0        0     9439 2018-07-13 08:26:34.000000 pytileproj-0.0.8/pytileproj/data/utm/make_utm_shapefiles.py
--rw-rw-rw-   0        0        0  1425706 2018-07-16 17:29:33.000000 pytileproj-0.0.8/pytileproj/data/utm/utmgrid.dat
--rw-rw-rw-   0        0        0        0 2018-07-12 12:15:36.000000 pytileproj-0.0.8/pytileproj/data/__init__.py
--rw-rw-rw-   0        0        0    15938 2018-07-12 14:00:47.000000 pytileproj-0.0.8/pytileproj/geometry.py
--rw-rw-rw-   0        0        0    27389 2018-10-17 13:08:37.000000 pytileproj-0.0.8/pytileproj/utmgrid.py
--rw-rw-rw-   0        0        0      161 2018-08-06 11:04:53.000000 pytileproj-0.0.8/pytileproj/__init__.py
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:19.000000 pytileproj-0.0.8/pytileproj.egg-info/
--rw-rw-rw-   0        0        0        1 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2017-09-06 11:04:41.000000 pytileproj-0.0.8/pytileproj.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5019 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       61 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj.egg-info/requires.txt
--rw-rw-rw-   0        0        0    34315 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2018-10-17 14:22:18.000000 pytileproj-0.0.8/pytileproj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3763 2018-08-06 11:04:53.000000 pytileproj-0.0.8/README.rst
--rw-rw-rw-   0        0        0       68 2018-01-31 16:11:53.000000 pytileproj-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0      776 2018-10-17 14:22:20.000000 pytileproj-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      626 2018-08-06 11:04:53.000000 pytileproj-0.0.8/setup.py
--rw-rw-rw-   0        0        0      252 2018-07-13 12:34:39.000000 pytileproj-0.0.8/test-requirements.txt
-drwxrwxrwx   0        0        0        0 2018-10-17 14:22:20.000000 pytileproj-0.0.8/tests/
--rw-rw-rw-   0        0        0      328 2018-08-06 11:04:53.000000 pytileproj-0.0.8/tests/conftest.py
--rw-rw-rw-   0        0        0    13043 2018-10-17 13:42:16.000000 pytileproj-0.0.8/tests/test_utmgrid.py
--rw-rw-rw-   0        0        0      136 2017-08-24 14:09:00.000000 pytileproj-0.0.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/
+-rw-rw-rw-   0        0        0      568 2017-08-24 14:09:00.000000 pytileproj-0.0.9/.coveragerc
+-rw-rw-rw-   0        0        0     1374 2018-10-17 13:53:01.000000 pytileproj-0.0.9/.travis.yml
+-rw-rw-rw-   0        0        0      172 2018-01-31 16:11:53.000000 pytileproj-0.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0      434 2018-08-06 11:04:53.000000 pytileproj-0.0.9/CHANGES.rst
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/docs/
+-rw-rw-rw-   0        0        0       43 2017-08-24 14:09:00.000000 pytileproj-0.0.9/docs/authors.rst
+-rw-rw-rw-   0        0        0       43 2017-08-24 14:09:00.000000 pytileproj-0.0.9/docs/changes.rst
+-rw-rw-rw-   0        0        0     8999 2018-08-06 11:04:53.000000 pytileproj-0.0.9/docs/conf.py
+-rw-rw-rw-   0        0        0      288 2018-08-06 11:04:53.000000 pytileproj-0.0.9/docs/index.rst
+-rw-rw-rw-   0        0        0       81 2017-08-24 14:09:00.000000 pytileproj-0.0.9/docs/license.rst
+-rw-rw-rw-   0        0        0     6952 2017-08-24 14:09:00.000000 pytileproj-0.0.9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/docs/_static/
+-rw-rw-rw-   0        0        0       19 2017-08-24 14:09:00.000000 pytileproj-0.0.9/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0     1128 2018-01-31 16:11:53.000000 pytileproj-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5019 2018-11-27 15:16:32.000000 pytileproj-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/
+-rw-rw-rw-   0        0        0    38482 2018-11-23 13:34:56.000000 pytileproj-0.0.9/pytileproj/base.py
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/
+-rw-rw-rw-   0        0        0    14701 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0  1621156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0     1092 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    23044 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    23044 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    22564 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    22564 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:35.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:27.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:28.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:36.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    14020 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:29.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    11860 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13948 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    11428 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13948 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    11428 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13540 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:30.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:37.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:31.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    13156 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shx
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/
+-rw-rw-rw-   0        0        0       75 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.dbf
+-rw-rw-rw-   0        0        0      147 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.prj
+-rw-rw-rw-   0        0        0    12580 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shp
+-rw-rw-rw-   0        0        0      108 2018-07-13 08:26:38.000000 pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shx
+-rw-rw-rw-   0        0        0     4914 2018-07-13 12:19:57.000000 pytileproj-0.0.9/pytileproj/data/utm/make_utmdata.py
+-rw-rw-rw-   0        0        0     9439 2018-07-13 08:26:34.000000 pytileproj-0.0.9/pytileproj/data/utm/make_utm_shapefiles.py
+-rw-rw-rw-   0        0        0  1425706 2018-07-16 17:29:33.000000 pytileproj-0.0.9/pytileproj/data/utm/utmgrid.dat
+-rw-rw-rw-   0        0        0        0 2018-07-12 12:15:36.000000 pytileproj-0.0.9/pytileproj/data/__init__.py
+-rw-rw-rw-   0        0        0    15938 2018-07-12 14:00:47.000000 pytileproj-0.0.9/pytileproj/geometry.py
+-rw-rw-rw-   0        0        0    27389 2018-10-17 13:08:37.000000 pytileproj-0.0.9/pytileproj/utmgrid.py
+-rw-rw-rw-   0        0        0      161 2018-08-06 11:04:53.000000 pytileproj-0.0.9/pytileproj/__init__.py
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-11-27 15:16:25.000000 pytileproj-0.0.9/pytileproj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2017-09-06 11:04:41.000000 pytileproj-0.0.9/pytileproj.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5019 2018-11-27 15:16:25.000000 pytileproj-0.0.9/pytileproj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2018-11-27 15:16:25.000000 pytileproj-0.0.9/pytileproj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0    34315 2018-11-27 15:16:26.000000 pytileproj-0.0.9/pytileproj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2018-11-27 15:16:25.000000 pytileproj-0.0.9/pytileproj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3763 2018-08-06 11:04:53.000000 pytileproj-0.0.9/README.rst
+-rw-rw-rw-   0        0        0       68 2018-01-31 16:11:53.000000 pytileproj-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      776 2018-11-27 15:16:32.000000 pytileproj-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      626 2018-08-06 11:04:53.000000 pytileproj-0.0.9/setup.py
+-rw-rw-rw-   0        0        0      252 2018-07-13 12:34:39.000000 pytileproj-0.0.9/test-requirements.txt
+drwxrwxrwx   0        0        0        0 2018-11-27 15:16:32.000000 pytileproj-0.0.9/tests/
+-rw-rw-rw-   0        0        0      328 2018-08-06 11:04:53.000000 pytileproj-0.0.9/tests/conftest.py
+-rw-rw-rw-   0        0        0    14264 2018-11-23 13:36:43.000000 pytileproj-0.0.9/tests/test_utmgrid.py
+-rw-rw-rw-   0        0        0      136 2017-08-24 14:09:00.000000 pytileproj-0.0.9/tests/__init__.py
```

### Comparing `pytileproj-0.0.8/.coveragerc` & `pytileproj-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/.travis.yml` & `pytileproj-0.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/docs/conf.py` & `pytileproj-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/docs/Makefile` & `pytileproj-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/LICENSE.txt` & `pytileproj-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/PKG-INFO` & `pytileproj-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytileproj
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: http://...
 Author: Bernhard Bauer-Marschallinger
 Author-email: bernhard.bauer-marschallinger@geo.tuwien.ac.at
 License: none
 Description: ==========
         pytileproj
```

### Comparing `pytileproj-0.0.8/pytileproj/base.py` & `pytileproj-0.0.9/pytileproj/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,36 +246,38 @@
 
         Parameters
         ----------
         lon : list of numbers
             longitude coordinates
         lat : list of numbers
             latitude coordinates
-        subgrid : str
-            optional: acronym / subgrid ID to search within (speeding up)
+        subgrid : str, optional
+             acronym / subgrid ID to search within (speeding up)
+             forces to find coordinates in given subgrid
+             --> can return outlying or negative coordinates!
 
         Returns
         -------
         subgrid : str
-            subgrid ID
+            subgrid ID in which the returned x, y coordinates are defined
         x, y : list of float
             TPS grid coordinates
         """
 
         if subgrid is None:
             vfunc = np.vectorize(self._lonlat2xy)
             return vfunc(lon, lat)
         else:
             return self._lonlat2xy_subgrid(lon, lat, subgrid)
 
 
     def _lonlat2xy(self, lon, lat):
         """
-        finds overlapping subgrids of a given point in lon-lat-space
-        and computes the projected coordinates.
+        finds overlapping subgrid of a given point in lon-lat-space
+        and computes the projected coordinates referring to that subgrid.
 
         Parameters
         ----------
         lon : number
             longitude coordinate
         lat : number
             latitude coordinate
@@ -305,36 +307,31 @@
 
     def _lonlat2xy_subgrid(self, lon, lat, subgrid):
         """
         computes the projected coordinates in given subgrid.
 
         Parameters
         ----------
-        lon : number
-            longitude coordinate
-        lat : number
-            latitude coordinate
-        subgrid : str
-            acronym / subgrid ID to search within (speeding up)
+        lon : list of numbers
+            longitude coordinates
+        lat : list of numbers
+            latitude coordinates
+        subgrid : str, optional
+             acronym / subgrid ID to search within (speeding up)
+             forces to find coordinates in given subgrid
+             --> can return outlying or negative coordinates!
 
         Returns
         -------
         subgrid : str
             acronym / subgrid ID
         x, y : int
             TPS grid coordinates
         """
 
-        #check for correct subgrid for the given lonlat coords
-        bb = self.subgrids[subgrid].polygon_geog.GetEnvelope()
-        if (lon <= bb[0]).any() or (lon >= bb[1]).any() or \
-                (lat <= bb[2]).any() or (lat >= bb[3]).any():
-            raise ValueError("Check: lon or lat or "
-                             "outside of the given subgrid!")
-
         # set up spatial references
         p_grid = pyproj.Proj(self.subgrids[subgrid].core.projection.proj4)
         p_geo = pyproj.Proj(init="EPSG:4326")
 
         x, y, = pyproj.transform(p_geo, p_grid, lon, lat)
 
         return subgrid, x, y
```

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.dbf` & `pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.dbf`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shx` & `pytileproj-0.0.9/pytileproj/data/utm/grids/000_grids_combined/UTM_UPS_V10_ALL_ZONES_GEOG_ZONE.shx`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z00A/GEOG/UTM_UPS_V10_Z00A_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z00B/GEOG/UTM_UPS_V10_Z00B_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Y/GEOG/UTM_UPS_V10_Z00Y_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z00Z/GEOG/UTM_UPS_V10_Z00Z_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z01N/GEOG/UTM_UPS_V10_Z01N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z01S/GEOG/UTM_UPS_V10_Z01S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z02N/GEOG/UTM_UPS_V10_Z02N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z02S/GEOG/UTM_UPS_V10_Z02S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z03N/GEOG/UTM_UPS_V10_Z03N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z03S/GEOG/UTM_UPS_V10_Z03S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z04N/GEOG/UTM_UPS_V10_Z04N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z04S/GEOG/UTM_UPS_V10_Z04S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z05N/GEOG/UTM_UPS_V10_Z05N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z05S/GEOG/UTM_UPS_V10_Z05S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z06N/GEOG/UTM_UPS_V10_Z06N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z06S/GEOG/UTM_UPS_V10_Z06S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z07N/GEOG/UTM_UPS_V10_Z07N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z07S/GEOG/UTM_UPS_V10_Z07S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z08N/GEOG/UTM_UPS_V10_Z08N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z08S/GEOG/UTM_UPS_V10_Z08S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z09N/GEOG/UTM_UPS_V10_Z09N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z09S/GEOG/UTM_UPS_V10_Z09S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z10N/GEOG/UTM_UPS_V10_Z10N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z10S/GEOG/UTM_UPS_V10_Z10S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z11N/GEOG/UTM_UPS_V10_Z11N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z11S/GEOG/UTM_UPS_V10_Z11S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z12N/GEOG/UTM_UPS_V10_Z12N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z12S/GEOG/UTM_UPS_V10_Z12S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z13N/GEOG/UTM_UPS_V10_Z13N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z13S/GEOG/UTM_UPS_V10_Z13S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z14N/GEOG/UTM_UPS_V10_Z14N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z14S/GEOG/UTM_UPS_V10_Z14S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z15N/GEOG/UTM_UPS_V10_Z15N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z15S/GEOG/UTM_UPS_V10_Z15S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z16N/GEOG/UTM_UPS_V10_Z16N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z16S/GEOG/UTM_UPS_V10_Z16S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z17N/GEOG/UTM_UPS_V10_Z17N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z17S/GEOG/UTM_UPS_V10_Z17S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z18N/GEOG/UTM_UPS_V10_Z18N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z18S/GEOG/UTM_UPS_V10_Z18S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z19N/GEOG/UTM_UPS_V10_Z19N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z19S/GEOG/UTM_UPS_V10_Z19S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z20N/GEOG/UTM_UPS_V10_Z20N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z20S/GEOG/UTM_UPS_V10_Z20S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z21N/GEOG/UTM_UPS_V10_Z21N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z21S/GEOG/UTM_UPS_V10_Z21S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z22N/GEOG/UTM_UPS_V10_Z22N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z22S/GEOG/UTM_UPS_V10_Z22S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z23N/GEOG/UTM_UPS_V10_Z23N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z23S/GEOG/UTM_UPS_V10_Z23S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z24N/GEOG/UTM_UPS_V10_Z24N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z24S/GEOG/UTM_UPS_V10_Z24S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z25N/GEOG/UTM_UPS_V10_Z25N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z25S/GEOG/UTM_UPS_V10_Z25S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z26N/GEOG/UTM_UPS_V10_Z26N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z26S/GEOG/UTM_UPS_V10_Z26S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z27N/GEOG/UTM_UPS_V10_Z27N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z27S/GEOG/UTM_UPS_V10_Z27S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z28N/GEOG/UTM_UPS_V10_Z28N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z28S/GEOG/UTM_UPS_V10_Z28S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z29N/GEOG/UTM_UPS_V10_Z29N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z29S/GEOG/UTM_UPS_V10_Z29S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z30N/GEOG/UTM_UPS_V10_Z30N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z30S/GEOG/UTM_UPS_V10_Z30S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z31N/GEOG/UTM_UPS_V10_Z31N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z31S/GEOG/UTM_UPS_V10_Z31S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z32N/GEOG/UTM_UPS_V10_Z32N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z32S/GEOG/UTM_UPS_V10_Z32S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z33N/GEOG/UTM_UPS_V10_Z33N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z33S/GEOG/UTM_UPS_V10_Z33S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z34N/GEOG/UTM_UPS_V10_Z34N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z34S/GEOG/UTM_UPS_V10_Z34S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z35N/GEOG/UTM_UPS_V10_Z35N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z35S/GEOG/UTM_UPS_V10_Z35S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z36N/GEOG/UTM_UPS_V10_Z36N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z36S/GEOG/UTM_UPS_V10_Z36S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z37N/GEOG/UTM_UPS_V10_Z37N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z37S/GEOG/UTM_UPS_V10_Z37S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z38N/GEOG/UTM_UPS_V10_Z38N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z38S/GEOG/UTM_UPS_V10_Z38S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z39N/GEOG/UTM_UPS_V10_Z39N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z39S/GEOG/UTM_UPS_V10_Z39S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z40N/GEOG/UTM_UPS_V10_Z40N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z40S/GEOG/UTM_UPS_V10_Z40S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z41N/GEOG/UTM_UPS_V10_Z41N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z41S/GEOG/UTM_UPS_V10_Z41S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z42N/GEOG/UTM_UPS_V10_Z42N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z42S/GEOG/UTM_UPS_V10_Z42S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z43N/GEOG/UTM_UPS_V10_Z43N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z43S/GEOG/UTM_UPS_V10_Z43S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z44N/GEOG/UTM_UPS_V10_Z44N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z44S/GEOG/UTM_UPS_V10_Z44S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z45N/GEOG/UTM_UPS_V10_Z45N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z45S/GEOG/UTM_UPS_V10_Z45S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z46N/GEOG/UTM_UPS_V10_Z46N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z46S/GEOG/UTM_UPS_V10_Z46S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z47N/GEOG/UTM_UPS_V10_Z47N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z47S/GEOG/UTM_UPS_V10_Z47S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z48N/GEOG/UTM_UPS_V10_Z48N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z48S/GEOG/UTM_UPS_V10_Z48S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z49N/GEOG/UTM_UPS_V10_Z49N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z49S/GEOG/UTM_UPS_V10_Z49S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z50N/GEOG/UTM_UPS_V10_Z50N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z50S/GEOG/UTM_UPS_V10_Z50S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z51N/GEOG/UTM_UPS_V10_Z51N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z51S/GEOG/UTM_UPS_V10_Z51S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z52N/GEOG/UTM_UPS_V10_Z52N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z52S/GEOG/UTM_UPS_V10_Z52S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z53N/GEOG/UTM_UPS_V10_Z53N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z53S/GEOG/UTM_UPS_V10_Z53S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z54N/GEOG/UTM_UPS_V10_Z54N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z54S/GEOG/UTM_UPS_V10_Z54S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z55N/GEOG/UTM_UPS_V10_Z55N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z55S/GEOG/UTM_UPS_V10_Z55S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z56N/GEOG/UTM_UPS_V10_Z56N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z56S/GEOG/UTM_UPS_V10_Z56S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z57N/GEOG/UTM_UPS_V10_Z57N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z57S/GEOG/UTM_UPS_V10_Z57S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z58N/GEOG/UTM_UPS_V10_Z58N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z58S/GEOG/UTM_UPS_V10_Z58S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z59N/GEOG/UTM_UPS_V10_Z59N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z59S/GEOG/UTM_UPS_V10_Z59S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z60N/GEOG/UTM_UPS_V10_Z60N_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shp` & `pytileproj-0.0.9/pytileproj/data/utm/grids/Z60S/GEOG/UTM_UPS_V10_Z60S_GEOG_ZONE.shp`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/make_utmdata.py` & `pytileproj-0.0.9/pytileproj/data/utm/make_utmdata.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/make_utm_shapefiles.py` & `pytileproj-0.0.9/pytileproj/data/utm/make_utm_shapefiles.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/data/utm/utmgrid.dat` & `pytileproj-0.0.9/pytileproj/data/utm/utmgrid.dat`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/geometry.py` & `pytileproj-0.0.9/pytileproj/geometry.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj/utmgrid.py` & `pytileproj-0.0.9/pytileproj/utmgrid.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/pytileproj.egg-info/PKG-INFO` & `pytileproj-0.0.9/pytileproj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytileproj
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: http://...
 Author: Bernhard Bauer-Marschallinger
 Author-email: bernhard.bauer-marschallinger@geo.tuwien.ac.at
 License: none
 Description: ==========
         pytileproj
```

### Comparing `pytileproj-0.0.8/pytileproj.egg-info/SOURCES.txt` & `pytileproj-0.0.9/pytileproj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/README.rst` & `pytileproj-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/setup.cfg` & `pytileproj-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/setup.py` & `pytileproj-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytileproj-0.0.8/tests/test_utmgrid.py` & `pytileproj-0.0.9/tests/test_utmgrid.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,346 +14,352 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 
 """
 Tests for the UTMGrid().
 """
-
+import unittest
 import numpy as np
 import numpy.testing as nptest
 
 from pytileproj.utmgrid import UTMGrid
 from pytileproj.geometry import setup_test_geom_spitzbergen
 from pytileproj.geometry import setup_geom_kamchatka
 
 
-def test_lonlat2xy_doubles():
-    """
-    Tests lonlat to xy projection using double numbers.
-    """
-    utm = UTMGrid(500)
-    x_should = 433124.249310
-    y_should = 5338921.352324
-    lon, lat = 14.1, 48.2
-    sgrid_id, x, y = utm.lonlat2xy(lon, lat)
-    assert sgrid_id == 'Z33N'
-    nptest.assert_allclose(x_should, x)
-    nptest.assert_allclose(y_should, y)
-
-
-def test_lonlat2xy_numpy_array():
-    """
-    Tests lonlat to xy projection using numpy arrays.
-    """
-    utm = UTMGrid(500)
-    x_should = np.array([507840.292027,
-                         210029.47])
-    y_should = np.array([4983717.660043,
-                         6820022.61])
-    lon = np.array([15.1, 3.564943])
-    lat = np.array([-45.3, 61.405307])
-    sgrid_id, x, y = utm.lonlat2xy(lon, lat)
-    nptest.assert_array_equal(sgrid_id, np.array(['Z33S', 'Z32N']))
-    nptest.assert_allclose(x_should, x)
-    nptest.assert_allclose(y_should, y)
-
-
-def ctest_lonlat2xy_MGRS_numpy_array():
-    """
-    Tests lonlat to xy projection using numpy arrays.
-    """
-    utm = UTMGrid(500)
-    x_should = np.array([507840.292027,
-                         210029.47,
-                         2394255.583836])
-    y_should = np.array([4983717.660043,
-                         6820022.61,
-                         2000000.0])
-    lon = np.array([15.1, 3.564943, 90.0])
-    lat = np.array([-45.3, 61.405307, -86.45])
-    sgrid_id, x, y = utm.lonlat2xy_MGRS(lon, lat)
-    nptest.assert_array_equal(sgrid_id, np.array(['Z33G', 'Z32V', 'Z00B']))
-    nptest.assert_allclose(x_should, x)
-    nptest.assert_allclose(y_should, y)
-
-
-def test_lonlat2xy_numpy_array_subgrid():
-    """
-    Tests lonlat to xy projection using numpy arrays.
-    """
-    utm = UTMGrid(500)
-    x_should = np.array([492159.707973])
-    y_should = np.array([5016282.339957])
-    lon = np.array([-15.1])
-    lat = np.array([45.3])
-    sgrid_id, x, y = utm.lonlat2xy(lon, lat, subgrid='Z28N')
-    nptest.assert_array_equal(sgrid_id, np.array(['Z28N']))
-    nptest.assert_allclose(x_should, x)
-    nptest.assert_allclose(y_should, y)
-
-
-def test_lonlat2xy_numpy_array_wrong_subgrid():
-    """
-    Tests lonlat to xy projection giving a wrong subgrid.
-    """
-    utm = UTMGrid(500)
-    x_should = np.array([492159.707973])
-    y_should = np.array([5016282.339957])
-    lon = np.array([-15.1])
-    lat = np.array([45.3])
-    with nptest.assert_raises(ValueError) as excinfo:
-        utm.lonlat2xy(lon, lat, subgrid='Z44S')
-    assert str(excinfo.exception) == ('Check: lon or lat or outside '
-                                      'of the given subgrid!')
-
-
-def test_xy2lonlat_doubles():
-    """
-    Tests xy to lonlat projection using double numbers.
-    """
-    utm = UTMGrid(500)
-    x = 458119.890658
-    y = 6312037.887621
-    lon_should, lat_should = -105.45, -33.33
-    lon, lat = utm.Z13S.xy2lonlat(x, y)
-    nptest.assert_allclose(lon_should, lon)
-    nptest.assert_allclose(lat_should, lat)
-
-
-def test_xy2lonlat_numpy_array():
-    """
-    Tests xy to lonlat projection using numpy arrays.
-    """
-    utm = UTMGrid(500)
-    x = np.array([458119.890658])
-    y = np.array([6312037.887621])
-    lon_should, lat_should = -105.68849338, 56.95006105
-    lon, lat = utm.Z13N.xy2lonlat(x, y)
-    nptest.assert_allclose(lon_should, lon)
-    nptest.assert_allclose(lat_should, lat)
-
-
-def test_ij2xy():
-    """
-    Tests tile indices to xy coordination in the subgrid projection.
-    """
-    utm = UTMGrid(500)
-    x_should = 481500
-    y_should = 9270500
-    tile = utm.Z18N.tilesys.create_tile(x=481746, y=9270569)
-    x, y = tile.ij2xy(963, 659)
-    nptest.assert_allclose(x_should, x)
-    nptest.assert_allclose(y_should, y)
-
-
-def test_xy2ij():
-    """
-    Tests xy to tile array indices.
-    """
-    utm = UTMGrid(500)
-    column_should = 963
-    row_should = 659
-    tile = utm.Z18N.tilesys.create_tile(x=481746, y=9270569)
-    column, row = tile.xy2ij(481500, 9270500)
-    nptest.assert_allclose(column_should, column)
-    nptest.assert_allclose(row_should, row)
-
-
-def test_decode_tilename():
-    """
-    Tests the decoding of tilenames.
-    """
-    utm_500 = UTMGrid(500)
-    utm_10 = UTMGrid(10)
-
-    assert utm_500.Z24N.tilesys.decode_tilename('Z24N500M_E000N006T6') == \
-           ('Z24N', 500, 600000, 0, 600000, 'T6')
-    assert utm_10.Z01N.tilesys.decode_tilename('Z01N010M_E085N091T1') == \
-           ('Z01N', 10, 100000, 8500000, 9100000, 'T1')
-
-    assert utm_500.Z24N.tilesys.decode_tilename('Z24N500M_E000N006T6') == \
-           ('Z24N', 500, 600000, 0, 600000, 'T6')
-    assert utm_10.Z01N.tilesys.decode_tilename('Z01N010M_E085N091T1') == \
-           ('Z01N', 10, 100000, 8500000, 9100000, 'T1')
-
-    with nptest.assert_raises(ValueError) as excinfo:
-        utm_10.Z01N.tilesys.decode_tilename('E000N006T6')
-    assert str(excinfo.exception).startswith(
-        '"tilename" is not properly defined!')
-
-
-def test_find_overlapping_tilenames():
-    """
-    Tests search for tiles which share the same extent_m but
-    with different resolution and tilecode.
-    """
-    utm_500 = UTMGrid(500)
-    utm_10 = UTMGrid(10)
-
-    tiles1_should = ['Z33N025M_E000N006T3', 'Z33N025M_E000N009T3',
-                     'Z33N025M_E003N006T3', 'Z33N025M_E003N009T3']
-    tiles1 = utm_500.Z33N.tilesys.find_overlapping_tilenames(
-        'Z33N500M_E000N006T6',
-        target_sampling=25)
-    assert sorted(tiles1) == sorted(tiles1_should)
-
-    tiles2_should = ['E000N006T3', 'E000N009T3', 'E003N006T3',
-                     'E003N009T3']
-    tiles2 = utm_500.Z33N.tilesys.find_overlapping_tilenames('E000N006T6',
-                                                          target_tiletype='T3')
-    assert sorted(tiles2) == sorted(tiles2_should)
-
-    tiles3_should = ['Z33N500M_E000N012T6']
-    tiles3 = utm_10.Z33N.tilesys.find_overlapping_tilenames('E004N015T1',
-                                                         target_sampling=500)
-    assert sorted(tiles3) == sorted(tiles3_should)
-
-    tiles4_should = ['E003N009T3']
-    tiles4 = utm_10.Z33N.tilesys.find_overlapping_tilenames('E004N011T1',
-                                                         target_tiletype='T3')
-    assert sorted(tiles4) == sorted(tiles4_should)
-
-
-def test_search_tiles_lon_lat_extent():
-    """
-    Tests searching for tiles with input of lon lat extent
-    """
-    # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
-    # adapted for coverland!
-
-    utm = UTMGrid(500)
-
-    tiles = utm.search_tiles_in_roi(extent=[-10, 80, 5, 85],
-                                   coverland=True)
-    desired_tiles = ['Z31N500M_E000N084T6', 'Z31N500M_E000N090T6',
-                     'Z00Z500M_E018N012T6', 'Z00Y500M_E018N012T6',
-                     'Z29N500M_E000N084T6', 'Z29N500M_E000N090T6',
-                     'Z30N500M_E000N084T6', 'Z30N500M_E000N090T6']
-    assert sorted(tiles) == sorted(desired_tiles)
+class TestBaseViaUTMGrid(unittest.TestCase):
+
+    def test_lonlat2xy_doubles(self):
+        """
+        Tests lonlat to xy projection using double numbers.
+        """
+        utm = UTMGrid(500)
+        x_should = 433124.249310
+        y_should = 5338921.352324
+        lon, lat = 14.1, 48.2
+        sgrid_id, x, y = utm.lonlat2xy(lon, lat)
+        assert sgrid_id == 'Z33N'
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def test_lonlat2xy_numpy_array(self):
+        """
+        Tests lonlat to xy projection using numpy arrays.
+        """
+        utm = UTMGrid(500)
+        x_should = np.array([507840.292027,
+                             210029.47])
+        y_should = np.array([4983717.660043,
+                             6820022.61])
+        lon = np.array([15.1, 3.564943])
+        lat = np.array([-45.3, 61.405307])
+        sgrid_id, x, y = utm.lonlat2xy(lon, lat)
+        nptest.assert_array_equal(sgrid_id, np.array(['Z33S', 'Z32N']))
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def ctest_lonlat2xy_MGRS_numpy_array(self):
+        """
+        Tests lonlat to xy projection using numpy arrays.
+        """
+        utm = UTMGrid(500)
+        x_should = np.array([507840.292027,
+                             210029.47,
+                             2394255.583836])
+        y_should = np.array([4983717.660043,
+                             6820022.61,
+                             2000000.0])
+        lon = np.array([15.1, 3.564943, 90.0])
+        lat = np.array([-45.3, 61.405307, -86.45])
+        sgrid_id, x, y = utm.lonlat2xy_MGRS(lon, lat)
+        nptest.assert_array_equal(sgrid_id, np.array(['Z33G', 'Z32V', 'Z00B']))
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def test_lonlat2xy_numpy_array_subgrid(self):
+        """
+        Tests lonlat to xy projection using numpy arrays.
+        """
+        utm = UTMGrid(500)
+        x_should = np.array([492159.707973])
+        y_should = np.array([5016282.339957])
+        lon = np.array([-15.1])
+        lat = np.array([45.3])
+        sgrid_id, x, y = utm.lonlat2xy(lon, lat, subgrid='Z28N')
+        nptest.assert_array_equal(sgrid_id, np.array(['Z28N']))
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def test_lonlat2xy_numpy_array_wrong_subgrid(self):
+        """
+        Tests lonlat to xy projection giving a wrong subgrid.
+        """
+        utm = UTMGrid(500)
+        x_should = np.array([-5028208.49022517])
+        y_should = np.array([20666035.74265257])
+        lon = np.array([-15.1])
+        lat = np.array([45.3])
+        sgrid_id, x, y = utm.lonlat2xy(lon, lat, subgrid='Z44S')
+        nptest.assert_array_equal(sgrid_id, np.array(['Z44S']))
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def test_xy2lonlat_doubles(self):
+        """
+        Tests xy to lonlat projection using double numbers.
+        """
+        utm = UTMGrid(500)
+        x = 458119.890658
+        y = 6312037.887621
+        lon_should, lat_should = -105.45, -33.33
+        lon, lat = utm.Z13S.xy2lonlat(x, y)
+        nptest.assert_allclose(lon_should, lon)
+        nptest.assert_allclose(lat_should, lat)
+
+
+    def test_xy2lonlat_numpy_array(self):
+        """
+        Tests xy to lonlat projection using numpy arrays.
+        """
+        utm = UTMGrid(500)
+        x = np.array([458119.890658])
+        y = np.array([6312037.887621])
+        lon_should, lat_should = -105.68849338, 56.95006105
+        lon, lat = utm.Z13N.xy2lonlat(x, y)
+        nptest.assert_allclose(lon_should, lon)
+        nptest.assert_allclose(lat_should, lat)
+
+
+    def test_ij2xy(self):
+        """
+        Tests tile indices to xy coordination in the subgrid projection.
+        """
+        utm = UTMGrid(500)
+        x_should = 481500
+        y_should = 9270500
+        tile = utm.Z18N.tilesys.create_tile(x=481746, y=9270569)
+        x, y = tile.ij2xy(963, 659)
+        nptest.assert_allclose(x_should, x)
+        nptest.assert_allclose(y_should, y)
+
+
+    def test_xy2ij(self):
+        """
+        Tests xy to tile array indices.
+        """
+        utm = UTMGrid(500)
+        column_should = 963
+        row_should = 659
+        tile = utm.Z18N.tilesys.create_tile(x=481746, y=9270569)
+        column, row = tile.xy2ij(481500, 9270500)
+        nptest.assert_allclose(column_should, column)
+        nptest.assert_allclose(row_should, row)
+
+
+    def test_decode_tilename(self):
+        """
+        Tests the decoding of tilenames.
+        """
+        utm_500 = UTMGrid(500)
+        utm_10 = UTMGrid(10)
+
+        assert utm_500.Z24N.tilesys.decode_tilename('Z24N500M_E000N006T6') == \
+               ('Z24N', 500, 600000, 0, 600000, 'T6')
+        assert utm_10.Z01N.tilesys.decode_tilename('Z01N010M_E085N091T1') == \
+               ('Z01N', 10, 100000, 8500000, 9100000, 'T1')
+
+        assert utm_500.Z24N.tilesys.decode_tilename('Z24N500M_E000N006T6') == \
+               ('Z24N', 500, 600000, 0, 600000, 'T6')
+        assert utm_10.Z01N.tilesys.decode_tilename('Z01N010M_E085N091T1') == \
+               ('Z01N', 10, 100000, 8500000, 9100000, 'T1')
+
+        with nptest.assert_raises(ValueError) as excinfo:
+            utm_10.Z01N.tilesys.decode_tilename('E000N006T6')
+        assert str(excinfo.exception).startswith(
+            '"tilename" is not properly defined!')
+
+
+    def test_find_overlapping_tilenames(self):
+        """
+        Tests search for tiles which share the same extent_m but
+        with different resolution and tilecode.
+        """
+        utm_500 = UTMGrid(500)
+        utm_10 = UTMGrid(10)
+
+        tiles1_should = ['Z33N025M_E000N006T3', 'Z33N025M_E000N009T3',
+                         'Z33N025M_E003N006T3', 'Z33N025M_E003N009T3']
+        tiles1 = utm_500.Z33N.tilesys.find_overlapping_tilenames(
+            'Z33N500M_E000N006T6',
+            target_sampling=25)
+        assert sorted(tiles1) == sorted(tiles1_should)
+
+        tiles2_should = ['E000N006T3', 'E000N009T3', 'E003N006T3',
+                         'E003N009T3']
+        tiles2 = utm_500.Z33N.tilesys.find_overlapping_tilenames('E000N006T6',
+                                                              target_tiletype='T3')
+        assert sorted(tiles2) == sorted(tiles2_should)
+
+        tiles3_should = ['Z33N500M_E000N012T6']
+        tiles3 = utm_10.Z33N.tilesys.find_overlapping_tilenames('E004N015T1',
+                                                             target_sampling=500)
+        assert sorted(tiles3) == sorted(tiles3_should)
+
+        tiles4_should = ['E003N009T3']
+        tiles4 = utm_10.Z33N.tilesys.find_overlapping_tilenames('E004N011T1',
+                                                             target_tiletype='T3')
+        assert sorted(tiles4) == sorted(tiles4_should)
+
+
+    def test_search_tiles_lon_lat_extent(self):
+        """
+        Tests searching for tiles with input of lon lat extent
+        """
+        # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
+        # adapted for coverland!
+
+        utm = UTMGrid(500)
 
-    tiles_all = utm.search_tiles_in_roi(extent=[-179.9, -89.9, 179.9, 89.9],
+        tiles = utm.search_tiles_in_roi(extent=[-10, 80, 5, 85],
                                        coverland=True)
-    assert len(tiles_all) == 3638
+        desired_tiles = ['Z31N500M_E000N084T6', 'Z31N500M_E000N090T6',
+                         'Z00Z500M_E018N012T6', 'Z00Y500M_E018N012T6',
+                         'Z29N500M_E000N084T6', 'Z29N500M_E000N090T6',
+                         'Z30N500M_E000N084T6', 'Z30N500M_E000N090T6']
+        assert sorted(tiles) == sorted(desired_tiles)
+
+        tiles_all = utm.search_tiles_in_roi(extent=[-179.9, -89.9, 179.9, 89.9],
+                                           coverland=True)
+        assert len(tiles_all) == 3638
+
+
 
+    def test_search_tiles_lon_lat_extent_by_points(self):
+        """
+        Tests searching for tiles with input of lon lat points
+        """
+        # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
+        # adapted for coverland!
 
+        utm = UTMGrid(500)
 
-def test_search_tiles_lon_lat_extent_by_points():
-    """
-    Tests searching for tiles with input of lon lat points
-    """
-    # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
-    # adapted for coverland!
+        tiles = utm.search_tiles_in_roi(
+            extent=[(10, 40), (5, 50), (-90.9, -1.2), (-175.2, 66)],
+            coverland=True)
+        desired_tiles = ['Z31N500M_E006N054T6', 'Z01N500M_E000N072T6',
+                         'Z32N500M_E000N042T6', 'Z15S500M_E006N096T6']
+        assert sorted(tiles) == sorted(desired_tiles)
 
-    utm = UTMGrid(500)
 
-    tiles = utm.search_tiles_in_roi(
-        extent=[(10, 40), (5, 50), (-90.9, -1.2), (-175.2, 66)],
-        coverland=True)
-    desired_tiles = ['Z31N500M_E006N054T6', 'Z01N500M_E000N072T6',
-                     'Z32N500M_E000N042T6', 'Z15S500M_E006N096T6']
-    assert sorted(tiles) == sorted(desired_tiles)
+    def test_search_tiles_spitzbergen(self):
+        """
+        Tests the tile searching over Spitzbergen in the polar zone; ROI #defined
+        by a 4-corner polygon over high latitudes (is much curved on the globe).
+        """
+        # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
+        # adapted for coverland!
 
+        grid = UTMGrid(500)
 
-def test_search_tiles_spitzbergen():
-    """
-    Tests the tile searching over Spitzbergen in the polar zone; ROI #defined
-    by a 4-corner polygon over high latitudes (is much curved on the globe).
-    """
-    # TODO: STILL NEEDS TO BE CAREFULLY CHECKED! Also need to be
-    # adapted for coverland!
+        spitzbergen_geom = setup_test_geom_spitzbergen()
+        spitzbergen_geom_tiles = sorted(
+            ['Z31N500M_E006N084T6', 'Z33N500M_E000N084T6', 'Z33N500M_E000N090T6',
+             'Z33N500M_E006N084T6', 'Z33N500M_E006N090T6', 'Z35N500M_E000N078T6',
+             'Z35N500M_E000N084T6', 'Z35N500M_E000N090T6', 'Z35N500M_E006N084T6',
+             'Z37N500M_E000N084T6'])
+        tiles = sorted(grid.search_tiles_in_roi(spitzbergen_geom,
+                                                coverland=False))
+        assert sorted(tiles) == sorted(spitzbergen_geom_tiles)
 
-    grid = UTMGrid(500)
+        spitzbergen_geom_tiles = sorted(
+            ['Z31N500M_E006N084T6', 'Z33N500M_E000N084T6', 'Z33N500M_E000N090T6',
+             'Z33N500M_E006N084T6', 'Z33N500M_E006N090T6', 'Z35N500M_E000N078T6',
+             'Z35N500M_E000N084T6', 'Z35N500M_E000N090T6', 'Z35N500M_E006N084T6',
+             'Z37N500M_E000N084T6'])
+        tiles = sorted(grid.search_tiles_in_roi(spitzbergen_geom,
+                                                coverland=True))
+        assert sorted(tiles) == sorted(spitzbergen_geom_tiles)
 
-    spitzbergen_geom = setup_test_geom_spitzbergen()
-    spitzbergen_geom_tiles = sorted(
-        ['Z31N500M_E006N084T6', 'Z33N500M_E000N084T6', 'Z33N500M_E000N090T6',
-         'Z33N500M_E006N084T6', 'Z33N500M_E006N090T6', 'Z35N500M_E000N078T6',
-         'Z35N500M_E000N084T6', 'Z35N500M_E000N090T6', 'Z35N500M_E006N084T6',
-         'Z37N500M_E000N084T6'])
-    tiles = sorted(grid.search_tiles_in_roi(spitzbergen_geom,
-                                            coverland=False))
-    assert sorted(tiles) == sorted(spitzbergen_geom_tiles)
 
-    spitzbergen_geom_tiles = sorted(
-        ['Z31N500M_E006N084T6', 'Z33N500M_E000N084T6', 'Z33N500M_E000N090T6',
-         'Z33N500M_E006N084T6', 'Z33N500M_E006N090T6', 'Z35N500M_E000N078T6',
-         'Z35N500M_E000N084T6', 'Z35N500M_E000N090T6', 'Z35N500M_E006N084T6',
-         'Z37N500M_E000N084T6'])
-    tiles = sorted(grid.search_tiles_in_roi(spitzbergen_geom,
-                                            coverland=True))
-    assert sorted(tiles) == sorted(spitzbergen_geom_tiles)
+    def test_search_tiles_kamchatka(self):
+        """
+        Tests the tile searching over Kamchatka in far east Sibiria;
 
+        This test is especially nice, as it contains also a tile that covers both,
+        the ROI and the continental zone, but the intersection of the tile and
+        the ROI is outside of the zone.
 
-def test_search_tiles_kamchatka():
-    """
-    Tests the tile searching over Kamchatka in far east Sibiria;
+        Furthermore, it also covers zones that consist of a multipolygon, as it
+        is located at the 180deg/dateline.
+        """
 
-    This test is especially nice, as it contains also a tile that covers both,
-    the ROI and the continental zone, but the intersection of the tile and
-    the ROI is outside of the zone.
+        grid = UTMGrid(500)
 
-    Furthermore, it also covers zones that consist of a multipolygon, as it
-    is located at the 180deg/dateline.
-    """
+        kamchatka_geom = setup_geom_kamchatka()
+        kamchatka_geom_tiles = sorted(
+            ['Z58N500M_E000N060T6', 'Z58N500M_E006N060T6',
+             'Z59N500M_E000N060T6', 'Z59N500M_E006N060T6',
+             'Z60N500M_E000N060T6', 'Z60N500M_E006N060T6'])
+        tiles = sorted(
+            grid.search_tiles_in_roi(kamchatka_geom, coverland=False))
 
-    grid = UTMGrid(500)
+        assert sorted(tiles) == sorted(kamchatka_geom_tiles)
 
-    kamchatka_geom = setup_geom_kamchatka()
-    kamchatka_geom_tiles = sorted(
-        ['Z58N500M_E000N060T6', 'Z58N500M_E006N060T6',
-         'Z59N500M_E000N060T6', 'Z59N500M_E006N060T6',
-         'Z60N500M_E000N060T6', 'Z60N500M_E006N060T6'])
-    tiles = sorted(
-        grid.search_tiles_in_roi(kamchatka_geom, coverland=False))
 
-    assert sorted(tiles) == sorted(kamchatka_geom_tiles)
+    def test_identify_tiles_overlapping_xybbox(self):
+        """
+        Tests identification of tiles covering a bounding box
+        given in UTM coordinats
+        """
+        # TODO: implemented check for out of bounds/zone tiles
+        utm_500 = UTMGrid(500)
+        utm_10 = UTMGrid(10)
 
+        tiles1_should = ['Z33N500M_E000N054T6', 'Z33N500M_E006N054T6']
 
-def test_identify_tiles_overlapping_xybbox():
-    """
-    Tests identification of tiles covering a bounding box
-    given in UTM coordinats
-    """
-    # TODO: implemented check for out of bounds/zone tiles
-    utm_500 = UTMGrid(500)
-    utm_10 = UTMGrid(10)
+        tiles2_should = ['Z33N010M_E005N058T1', 'Z33N010M_E005N059T1',
+                         'Z33N010M_E005N060T1', 'Z33N010M_E005N061T1']
 
-    tiles1_should = ['Z33N500M_E000N054T6', 'Z33N500M_E006N054T6']
+        tiles1 = utm_500.Z33N.tilesys.identify_tiles_overlapping_xybbox(
+            [559745, 5852882, 611111, 5952882])
 
-    tiles2_should = ['Z33N010M_E005N058T1', 'Z33N010M_E005N059T1',
-                     'Z33N010M_E005N060T1', 'Z33N010M_E005N061T1']
+        tiles2 = utm_10.Z33N.tilesys.identify_tiles_overlapping_xybbox(
+            [559745, 5852882, 571111, 6102882])
 
-    tiles1 = utm_500.Z33N.tilesys.identify_tiles_overlapping_xybbox(
-        [559745, 5852882, 611111, 5952882])
+        assert sorted(tiles1) == sorted(tiles1_should)
+        assert sorted(tiles2) == sorted(tiles2_should)
 
-    tiles2 = utm_10.Z33N.tilesys.identify_tiles_overlapping_xybbox(
-        [559745, 5852882, 571111, 6102882])
 
-    assert sorted(tiles1) == sorted(tiles1_should)
-    assert sorted(tiles2) == sorted(tiles2_should)
+    def test_get_covering_tiles(self):
+        """
+        Tests the search for co-locating tiles of other type.
+        """
 
+        utm_500 = UTMGrid(500)
+        utm_10 = UTMGrid(10)
 
-def test_get_covering_tiles():
-    """
-    Tests the search for co-locating tiles of other type.
-    """
+        fine_tiles = ['Z33N010M_E005N058T1', 'Z33N010M_E005N059T1',
+                      'Z33N010M_E005N060T1', 'Z33N010M_E005N061T1']
 
-    utm_500 = UTMGrid(500)
-    utm_10 = UTMGrid(10)
+        target_tiletype = utm_500.get_tiletype()
+        target_sampling = utm_500.core.sampling
 
-    fine_tiles = ['Z33N010M_E005N058T1', 'Z33N010M_E005N059T1',
-                  'Z33N010M_E005N060T1', 'Z33N010M_E005N061T1']
+        # invoke the results as tile name in short form
+        coarse_tiles_shortform = utm_10.Z33N.tilesys.get_covering_tiles(fine_tiles,
+                                                 target_tiletype=target_tiletype)
 
-    target_tiletype = utm_500.get_tiletype()
-    target_sampling = utm_500.core.sampling
+        # invoke the results as tile name in long form
+        coarse_tiles_longform = utm_10.Z33N.tilesys.get_covering_tiles(fine_tiles,
+                                               target_sampling=target_sampling)
 
-    # invoke the results as tile name in short form
-    coarse_tiles_shortform = utm_10.Z33N.tilesys.get_covering_tiles(fine_tiles,
-                                             target_tiletype=target_tiletype)
+        assert sorted(coarse_tiles_shortform) == ['E000N054T6', 'E000N060T6']
+        assert sorted(coarse_tiles_longform) == ['Z33N500M_E000N054T6', 'Z33N500M_E000N060T6']
 
-    # invoke the results as tile name in long form
-    coarse_tiles_longform = utm_10.Z33N.tilesys.get_covering_tiles(fine_tiles,
-                                           target_sampling=target_sampling)
 
-    assert sorted(coarse_tiles_shortform) == ['E000N054T6', 'E000N060T6']
-    assert sorted(coarse_tiles_longform) == ['Z33N500M_E000N054T6', 'Z33N500M_E000N060T6']
+if __name__ == '__main__':
+    unittest.main()
```

