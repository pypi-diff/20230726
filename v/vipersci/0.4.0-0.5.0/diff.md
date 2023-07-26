# Comparing `tmp/vipersci-0.4.0.tar.gz` & `tmp/vipersci-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vipersci-0.4.0.tar", last modified: Wed Mar  1 17:08:30 2023, max compression
+gzip compressed data, was "vipersci-0.5.0.tar", last modified: Wed Jul 26 18:49:06 2023, max compression
```

## Comparing `vipersci-0.4.0.tar` & `vipersci-0.5.0.tar`

### file list

```diff
@@ -1,103 +1,118 @@
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/
--rw-r--r--   0 rbeyer     (503) staff       (20)      614 2022-09-06 02:06:52.000000 vipersci-0.4.0/AUTHORS.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)     4644 2023-03-01 17:05:14.000000 vipersci-0.4.0/CHANGELOG.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)     7794 2022-10-07 03:30:43.000000 vipersci-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.4.0/LICENSE
--rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.4.0/MANIFEST.in
--rw-r--r--   0 rbeyer     (503) staff       (20)     8751 2023-03-01 17:08:30.000000 vipersci-0.4.0/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     3290 2023-03-01 16:59:24.000000 vipersci-0.4.0/README.rst
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/docs/
--rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.4.0/docs/Makefile
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/docs/_build/
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/docs/_build/html/
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/docs/_build/html/_static/
--rw-r--r--   0 rbeyer     (503) staff       (20)      286 2022-01-20 19:42:47.000000 vipersci-0.4.0/docs/_build/html/_static/file.png
--rw-r--r--   0 rbeyer     (503) staff       (20)       90 2022-01-20 19:42:47.000000 vipersci-0.4.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 rbeyer     (503) staff       (20)       90 2022-01-20 19:42:47.000000 vipersci-0.4.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.4.0/docs/authors.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.4.0/docs/changelog.rst
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.4.0/docs/conf.py
--rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.4.0/docs/contributing.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.4.0/docs/index.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.4.0/docs/installation.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.4.0/docs/make.bat
--rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.4.0/docs/modules.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.4.0/docs/readme.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.4.0/docs/usage.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.4.0/docs/vipersci.pds.data.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.4.0/docs/vipersci.pds.data.template.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.4.0/docs/vipersci.pds.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.4.0/docs/vipersci.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.4.0/docs/vipersci.vis.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      271 2023-03-01 02:15:09.000000 vipersci-0.4.0/pyproject.toml
--rw-r--r--   0 rbeyer     (503) staff       (20)     2439 2023-03-01 17:08:30.000000 vipersci-0.4.0/setup.cfg
--rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.4.0/setup.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/
--rw-r--r--   0 rbeyer     (503) staff       (20)      130 2023-03-01 17:07:58.000000 vipersci-0.4.0/src/vipersci/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/carto/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.4.0/src/vipersci/carto/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3693 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/accrual.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.4.0/src/vipersci/carto/bounds.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/dice_buffer.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/dissolve_dice.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.4.0/src/vipersci/carto/dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    20086 2023-02-24 03:28:58.000000 vipersci-0.4.0/src/vipersci/carto/heatmap.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/msolo_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/nirvss_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3049 2023-03-01 16:59:24.000000 vipersci-0.4.0/src/vipersci/carto/nss_modeler.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     7430 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/carto/nss_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3732 2023-02-24 03:28:58.000000 vipersci-0.4.0/src/vipersci/carto/traverse_interpolator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    10953 2023-03-01 16:59:24.000000 vipersci-0.4.0/src/vipersci/carto/tri2gpkg.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.4.0/src/vipersci/msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.4.0/src/vipersci/nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    10904 2023-03-01 16:59:24.000000 vipersci-0.4.0/src/vipersci/nss.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-01-05 02:33:02.000000 vipersci-0.4.0/src/vipersci/pds/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/pds/datetime.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    12053 2023-02-24 03:28:58.000000 vipersci-0.4.0/src/vipersci/pds/pid.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     1254 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/pds/xml.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2239 2022-11-01 14:54:30.000000 vipersci-0.4.0/src/vipersci/util.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/vis/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.4.0/src/vipersci/vis/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/vis/db/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:57:45.000000 vipersci-0.4.0/src/vipersci/vis/db/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2244 2022-11-30 20:55:10.000000 vipersci-0.4.0/src/vipersci/vis/db/create_vis_dbs.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    24782 2023-02-24 03:28:58.000000 vipersci-0.4.0/src/vipersci/vis/db/raw_products.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1833 2022-11-30 20:55:10.000000 vipersci-0.4.0/src/vipersci/vis/db/raw_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3188 2022-11-01 14:54:30.000000 vipersci-0.4.0/src/vipersci/vis/header.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1895 2022-11-30 20:55:10.000000 vipersci-0.4.0/src/vipersci/vis/image_statistics.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/vis/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.4.0/src/vipersci/vis/pds/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    14823 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/vis/pds/create_raw.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2032 2022-11-01 14:54:30.000000 vipersci-0.4.0/src/vipersci/vis/pds/create_raw_tif.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci/vis/pds/data/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.4.0/src/vipersci/vis/pds/data/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1984 2022-11-10 16:51:53.000000 vipersci-0.4.0/src/vipersci/vis/pds/template_test.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/
--rw-r--r--   0 rbeyer     (503) staff       (20)     8751 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     2290 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/SOURCES.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/dependency_links.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)      726 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/entry_points.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/not-zip-safe
--rw-r--r--   0 rbeyer     (503) staff       (20)      121 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/requires.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        9 2023-03-01 17:08:30.000000 vipersci-0.4.0/src/vipersci.egg-info/top_level.txt
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-03-01 17:08:30.000000 vipersci-0.4.0/tests/
--rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_area_bin.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4800 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_create_raw.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_datetime.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8070 2023-02-24 03:28:58.000000 vipersci-0.4.0/tests/test_density_heatmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.4.0/tests/test_dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.4.0/tests/test_heatmap_helpers.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2496 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_image_statistics.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.4.0/tests/test_msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.4.0/tests/test_msolo_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.4.0/tests/test_nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.4.0/tests/test_nirvss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3737 2022-11-01 14:54:30.000000 vipersci-0.4.0/tests/test_nss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_nss_modeler.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_nss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8413 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_pid.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    17426 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_raw_products.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1289 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_raw_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1342 2022-11-30 20:55:10.000000 vipersci-0.4.0/tests/test_util.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.420861 vipersci-0.5.0/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      614 2022-09-06 02:06:52.000000 vipersci-0.5.0/AUTHORS.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5720 2023-07-26 18:45:59.000000 vipersci-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8020 2023-04-11 20:22:14.000000 vipersci-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.5.0/LICENSE
+-rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.5.0/MANIFEST.in
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9832 2023-07-26 18:49:06.421076 vipersci-0.5.0/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3295 2023-07-26 18:46:41.000000 vipersci-0.5.0/README.rst
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.371893 vipersci-0.5.0/docs/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.5.0/docs/Makefile
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.352129 vipersci-0.5.0/docs/_build/
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.352272 vipersci-0.5.0/docs/_build/html/
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.374103 vipersci-0.5.0/docs/_build/html/_static/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      286 2022-01-20 19:42:47.000000 vipersci-0.5.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 rbeyer     (503) staff       (20)       90 2022-01-20 19:42:47.000000 vipersci-0.5.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 rbeyer     (503) staff       (20)       90 2022-01-20 19:42:47.000000 vipersci-0.5.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.5.0/docs/authors.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.5.0/docs/changelog.rst
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.5.0/docs/conf.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.5.0/docs/contributing.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.5.0/docs/index.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.5.0/docs/installation.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.5.0/docs/make.bat
+-rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.5.0/docs/modules.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.5.0/docs/readme.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.5.0/docs/usage.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.5.0/docs/vipersci.pds.data.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.5.0/docs/vipersci.pds.data.template.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.5.0/docs/vipersci.pds.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.5.0/docs/vipersci.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.5.0/docs/vipersci.vis.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      356 2023-05-05 04:04:23.000000 vipersci-0.5.0/pyproject.toml
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2572 2023-07-26 18:49:06.422639 vipersci-0.5.0/setup.cfg
+-rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.5.0/setup.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.352835 vipersci-0.5.0/src/
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.377886 vipersci-0.5.0/src/vipersci/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      130 2023-07-26 18:48:08.000000 vipersci-0.5.0/src/vipersci/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.390561 vipersci-0.5.0/src/vipersci/carto/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.5.0/src/vipersci/carto/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3731 2023-04-11 20:22:14.000000 vipersci-0.5.0/src/vipersci/carto/accrual.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.5.0/src/vipersci/carto/bounds.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    12441 2023-06-06 20:26:52.000000 vipersci-0.5.0/src/vipersci/carto/colorforge.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/carto/dice_buffer.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/carto/dissolve_dice.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.5.0/src/vipersci/carto/dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    20383 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/carto/heatmap.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/carto/msolo_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/carto/nirvss_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3049 2023-03-01 16:59:24.000000 vipersci-0.5.0/src/vipersci/carto/nss_modeler.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     7430 2023-03-29 01:08:10.000000 vipersci-0.5.0/src/vipersci/carto/nss_simulator.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.391050 vipersci-0.5.0/src/vipersci/carto/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:01:47.000000 vipersci-0.5.0/src/vipersci/carto/pds/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.391632 vipersci-0.5.0/src/vipersci/carto/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:03:38.000000 vipersci-0.5.0/src/vipersci/carto/pds/data/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3732 2023-02-24 03:28:58.000000 vipersci-0.5.0/src/vipersci/carto/traverse_interpolator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    11429 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/carto/tri2gpkg.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.5.0/src/vipersci/msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.5.0/src/vipersci/nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    10898 2023-06-06 20:26:52.000000 vipersci-0.5.0/src/vipersci/nss.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.394627 vipersci-0.5.0/src/vipersci/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-01-05 02:33:02.000000 vipersci-0.5.0/src/vipersci/pds/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/pds/datetime.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    14064 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/pds/pid.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     1254 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/pds/xml.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2239 2022-11-01 14:54:30.000000 vipersci-0.5.0/src/vipersci/util.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.397796 vipersci-0.5.0/src/vipersci/vis/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.5.0/src/vipersci/vis/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.402568 vipersci-0.5.0/src/vipersci/vis/db/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1093 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/db/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2244 2022-11-30 20:55:10.000000 vipersci-0.5.0/src/vipersci/vis/db/create_vis_dbs.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4174 2023-07-24 19:15:12.000000 vipersci-0.5.0/src/vipersci/vis/db/lights.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8699 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/db/pano_products.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    27605 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/db/raw_products.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1873 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/db/raw_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1880 2023-06-06 20:26:52.000000 vipersci-0.5.0/src/vipersci/vis/db/validators.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3188 2022-11-01 14:54:30.000000 vipersci-0.5.0/src/vipersci/vis/header.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1895 2022-11-30 20:55:10.000000 vipersci-0.5.0/src/vipersci/vis/image_statistics.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.404968 vipersci-0.5.0/src/vipersci/vis/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.5.0/src/vipersci/vis/pds/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8848 2023-06-06 20:26:52.000000 vipersci-0.5.0/src/vipersci/vis/pds/create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    14895 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/pds/create_raw.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2032 2022-11-01 14:54:30.000000 vipersci-0.5.0/src/vipersci/vis/pds/create_raw_tif.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.405387 vipersci-0.5.0/src/vipersci/vis/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.5.0/src/vipersci/vis/pds/data/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1984 2022-11-10 16:51:53.000000 vipersci-0.5.0/src/vipersci/vis/pds/template_test.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5252 2023-07-26 18:42:09.000000 vipersci-0.5.0/src/vipersci/vis/viseer.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.380508 vipersci-0.5.0/src/vipersci.egg-info/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9832 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2687 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/SOURCES.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/dependency_links.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)      856 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/entry_points.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/not-zip-safe
+-rw-r--r--   0 rbeyer     (503) staff       (20)      121 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/requires.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        9 2023-07-26 18:49:06.000000 vipersci-0.5.0/src/vipersci.egg-info/top_level.txt
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2023-07-26 18:49:06.420378 vipersci-0.5.0/tests/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_area_bin.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11820 2023-05-05 04:04:23.000000 vipersci-0.5.0/tests/test_colorforge.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1994 2023-06-06 20:26:52.000000 vipersci-0.5.0/tests/test_create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4800 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_create_raw.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_datetime.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8388 2023-07-26 18:42:09.000000 vipersci-0.5.0/tests/test_density_heatmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.5.0/tests/test_dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.5.0/tests/test_heatmap_helpers.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2496 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_image_statistics.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1929 2023-07-24 19:13:36.000000 vipersci-0.5.0/tests/test_lights.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.5.0/tests/test_msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.5.0/tests/test_msolo_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.5.0/tests/test_nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.5.0/tests/test_nirvss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3737 2022-11-01 14:54:30.000000 vipersci-0.5.0/tests/test_nss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_nss_modeler.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_nss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3413 2023-06-06 20:26:52.000000 vipersci-0.5.0/tests/test_pano_products.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11080 2023-07-26 18:42:09.000000 vipersci-0.5.0/tests/test_pid.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    18311 2023-07-26 18:42:09.000000 vipersci-0.5.0/tests/test_raw_products.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1289 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_raw_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1342 2022-11-30 20:55:10.000000 vipersci-0.5.0/tests/test_util.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2148 2023-06-06 20:26:52.000000 vipersci-0.5.0/tests/test_validators.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vipersci-0.4.0/AUTHORS.rst` & `vipersci-0.5.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/CHANGELOG.rst` & `vipersci-0.5.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,48 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+
+0.5.0 (2023-07-26)
+------------------
+
+Added
+^^^^^
+- PanoID class added to pds.pid
+- pano_products and create_pano added, still very preliminary, mostly just mock-ups.
+- colorforge program for managing colormaps.
+- mypy is now in the development dependencies to support type checking.
+- lint/mypy target added to Makefile.
+- tri2gpkg now has a --remove_facets option to remove facets with a particular value.
+
+
+Changed
+^^^^^^^
+- Explicit in documentation about developing in Python 3.8 (although earlier versions
+  should still be supported).
+- Many changes to improve type checking.
+- Added numeric instrument aliases and checking for them.
+- Added information for procesingInfo and outputMask from Yamcs.
+- Upgrade to SQLAlchemy >=2.
+- Moved definition of Base class up to vis.db.
+- heatmaps.py will now accept value data lists or arrays with np.nan or None values
+  which will be appropriate ignored in the density heatmap calculation.
+
+
+Fixed
+^^^^^
+- tri2gpkg - if the provided polygons have zero area, issue an error rather than
+  making a confusing GeoPackage file.
+
+
+
 0.4.0 (2023-03-01)
 ------------------
 
 Added
 ^^^^^
 - carto.bounds module added to unify functionality for both heatmaps and dotmaps.
 - carto.dotmap module for creating simple heatmap-like visualizations from 2d scalar data.
```

### Comparing `vipersci-0.4.0/CONTRIBUTING.rst` & `vipersci-0.5.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
   are welcome :)
 
 Get Started!
 ------------
 
 Ready to contribute? Here's how to set up `vipersci` for local development.
 
+At this time, the target version of Python for this library is 3.8 in order to
+align with current anticipated mission systems.  The intent is to allow this library
+to work successfully against Python as early as version 3.6.
+
 1. Fork the `vipersci` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/vipersci.git
 
 3. Install your local copy into a virtual environment of your choice
    (there are many to choose from like conda, etc.). We will assume
```

### Comparing `vipersci-0.4.0/LICENSE` & `vipersci-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/PKG-INFO` & `vipersci-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.4.0
+Version: 0.5.0
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -89,15 +89,15 @@
 
 
 License
 -------
 
 See LICENSE file for the full text of the license that applies to vipersci.
 
-Copyright (c) 2022, United States Government as represented by
+Copyright (c) 2022-2023, United States Government as represented by
 the Administrator of the National Aeronautics and Space
 Administration. All rights reserved.
 
 The "vipersci" software is licensed under the Apache License, Version 2.0
 (the "License"); you may not use this file except in compliance with the
 License.  You may obtain a copy of the License at
 http://www.apache.org/licenses/LICENSE-2.0
@@ -137,14 +137,48 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+
+0.5.0 (2023-07-26)
+------------------
+
+Added
+^^^^^
+- PanoID class added to pds.pid
+- pano_products and create_pano added, still very preliminary, mostly just mock-ups.
+- colorforge program for managing colormaps.
+- mypy is now in the development dependencies to support type checking.
+- lint/mypy target added to Makefile.
+- tri2gpkg now has a --remove_facets option to remove facets with a particular value.
+
+
+Changed
+^^^^^^^
+- Explicit in documentation about developing in Python 3.8 (although earlier versions
+  should still be supported).
+- Many changes to improve type checking.
+- Added numeric instrument aliases and checking for them.
+- Added information for procesingInfo and outputMask from Yamcs.
+- Upgrade to SQLAlchemy >=2.
+- Moved definition of Base class up to vis.db.
+- heatmaps.py will now accept value data lists or arrays with np.nan or None values
+  which will be appropriate ignored in the density heatmap calculation.
+
+
+Fixed
+^^^^^
+- tri2gpkg - if the provided polygons have zero area, issue an error rather than
+  making a confusing GeoPackage file.
+
+
+
 0.4.0 (2023-03-01)
 ------------------
 
 Added
 ^^^^^
 - carto.bounds module added to unify functionality for both heatmaps and dotmaps.
 - carto.dotmap module for creating simple heatmap-like visualizations from 2d scalar data.
```

### Comparing `vipersci-0.4.0/README.rst` & `vipersci-0.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 
 License
 -------
 
 See LICENSE file for the full text of the license that applies to vipersci.
 
-Copyright (c) 2022, United States Government as represented by
+Copyright (c) 2022-2023, United States Government as represented by
 the Administrator of the National Aeronautics and Space
 Administration. All rights reserved.
 
 The "vipersci" software is licensed under the Apache License, Version 2.0
 (the "License"); you may not use this file except in compliance with the
 License.  You may obtain a copy of the License at
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vipersci-0.4.0/docs/Makefile` & `vipersci-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/docs/conf.py` & `vipersci-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/docs/installation.rst` & `vipersci-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/docs/make.bat` & `vipersci-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/docs/vipersci.pds.rst` & `vipersci-0.5.0/docs/vipersci.pds.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/setup.cfg` & `vipersci-0.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0
+current_version = 0.5.0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
 
@@ -63,26 +63,29 @@
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	create_vis_dbs = vipersci.vis.db.create_vis_dbs:main
 	accrual = vipersci.carto.accrual:main
+	colorforge = vipersci.carto.colorforge:main
 	dice_buffer = vipersci.carto.dice_buffer:main
 	dissolve_dice = vipersci.carto.dissolve_dice:main
 	image_stats = vipersci.vis.image_statistics:main
 	msolo_simulator = vipersci.carto.msolo_simulator:main
 	nirvss_simulator = vipersci.carto.nirvss_simulator:main
 	nss_modeler = vipersci.carto.nss_modeler:main
 	nss_simulator = vipersci.carto.nss_simulator:main
 	traverse_interpolator = vipersci.carto.traverse_interpolator:main
 	tri2gpkg = vipersci.carto.tri2gpkg:main
 	template_test = vipersci.vis.pds.template_test:main
+	vis_create_pano = vipersci.vis.pds.create_pano:main
 	vis_create_raw = vipersci.vis.pds.create_raw:main
 	vis_create_raw_tif = vipersci.vis.pds.create_raw_tif:main
+	viseer = vipersci.vis.viseer:main
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = docs
 max_line_length = 88
```

### Comparing `vipersci-0.4.0/src/vipersci/carto/accrual.py` & `vipersci-0.5.0/src/vipersci/carto/accrual.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 #
 # Reuse is permitted under the terms of the license.
 # The AUTHORS file and the LICENSE file are at the
 # top level of this library.
 
 import argparse
 from collections import Counter
+from typing import Optional
 
 import geopandas as gp
 from shapely.geometry import LineString, box
 
 
 def arg_parser():
     parser = argparse.ArgumentParser(description=__doc__)
@@ -88,15 +89,15 @@
         print("This is different from the input total length!")
 
     print(f'Total length: {path["geometry"].length}')
     print(accrual)
 
 
 def accumulate(
-    path: LineString, areas: gp.GeoDataFrame, counter: dict = None
+    path: LineString, areas: gp.GeoDataFrame, counter: Optional[dict] = None
 ) -> Counter:
     """Returns a collections.Counter of floating point accumulations
     of the length of *Path* against each of the geometries in *areas*.
 
     The *path* LineString is expected to be in the projection/CRS of *areas*.
 
     If a *counter* dict-like (which can be a collections.Counter object)
```

### Comparing `vipersci-0.4.0/src/vipersci/carto/bounds.py` & `vipersci-0.5.0/src/vipersci/carto/bounds.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/dice_buffer.py` & `vipersci-0.5.0/src/vipersci/carto/dice_buffer.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/dissolve_dice.py` & `vipersci-0.5.0/src/vipersci/carto/dissolve_dice.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/dotmap.py` & `vipersci-0.5.0/src/vipersci/carto/dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/heatmap.py` & `vipersci-0.5.0/src/vipersci/carto/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-This heatmaps module takes scalar values with 2D coordinates and creates a heatmap
-representation with individual points effectively averaged together.
+This heatmaps module takes scalar values with 2D coordinates and creates a density
+heatmap representation with individual points effectively averaged together.
 """
 
-# Copyright 2022, United States Government as represented by the
+# Copyright 2022-2023, United States Government as represented by the
 # Administrator of the National Aeronautics and Space Administration.
 # All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -131,15 +131,16 @@
     """
     Perform tophat kernel density estimation to build a continuous heatmap
     representation of scalar values with 2d coordinates.
 
     Parameters:
         x_coords: x coordinates of the data points
         y_coords: y coordinates of the data points
-        values: values of the data points
+        values: values of the data points.  Any None or np.nan values will be ignored
+            in the kernel density estimation.
         gsd: Coordinate interval at which to sample the output distribution,
             or the ground sample distance of the output arrays.
             Defaults to 1.
         radius:  This is the kernel bandwidth used in the density estimation,
             and should be the sensing "radius" of the instrument.
             Defaults to 1.
         padding: Square padding in pixels to add to the bounds of data when
@@ -172,17 +173,21 @@
 
     if processes < 1:
         raise ValueError("Processes must be a positive integer.")
 
     if not (len(x_coords) == len(y_coords) == len(values)):
         raise ValueError("Input arrays must be of the same length.")
 
-    x_coords_np = as_ndarray(x_coords)
-    y_coords_np = as_ndarray(y_coords)
-    values_np = as_ndarray(values)
+    values_all = as_ndarray(values)
+
+    missing_idx = np.isnan(values_all.astype(float))
+
+    x_coords_np = np.delete(as_ndarray(x_coords), np.argwhere(missing_idx))
+    y_coords_np = np.delete(as_ndarray(y_coords), np.argwhere(missing_idx))
+    values_np = np.delete(values_all, np.argwhere(missing_idx))
 
     points = shapely.geometry.LineString(np.stack((x_coords_np, y_coords_np), axis=1))
     if sample_bounds is not None:
         points = points.intersection(sample_bounds)
 
     if padding is None:
         buffer = radius
```

### Comparing `vipersci-0.4.0/src/vipersci/carto/msolo_simulator.py` & `vipersci-0.5.0/src/vipersci/carto/msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/nirvss_simulator.py` & `vipersci-0.5.0/src/vipersci/carto/nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/nss_modeler.py` & `vipersci-0.5.0/src/vipersci/carto/nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/nss_simulator.py` & `vipersci-0.5.0/src/vipersci/carto/nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/traverse_interpolator.py` & `vipersci-0.5.0/src/vipersci/carto/traverse_interpolator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/carto/tri2gpkg.py` & `vipersci-0.5.0/src/vipersci/carto/tri2gpkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,20 @@
     parser.add_argument(
         "--value_file",
         help="If provided another whitespace-separated file will be read in, "
         "and the value(s) from the column(s) indicated by --value_columns "
         "will be used as the value(s).",
     )
     parser.add_argument(
+        "--remove_facets",
+        type=float,
+        help="If provided, any facets with this value will not be included in the "
+        "output GeoPackage.  Ignored if there is more than one value_column.",
+    )
+    parser.add_argument(
         "--replace_with_zero",
         help="If there is a value that should be replaced with zero, it can "
         "be provided here.  If the --value_name is 'Depth (m)' this will "
         "automatically be set to '-1'.  If you want to override that, "
         "you can set '--replace_with_zero 0'.",
     )
     parser.add_argument(
@@ -203,14 +209,18 @@
     values = {k: [] for k in value_keys}
 
     polys = list()
     with open(args.file, "r") as f:
         logger.info(f"Reading vertices from {args.file}")
         for line in f:
             tokens = line.split()
+
+            if len(col_idxs) == 1 and float(tokens[col_idxs[0]]) == args.remove_facets:
+                continue
+
             poly = vertexes_to_poly(transformer, tokens[:9], args.keep_z)
             polys.append(poly)
 
             for i, col in enumerate(col_idxs):
                 values[value_keys[i]].append(
                     replace_with(0, replace_with_zero, tokens[col])
                 )
@@ -229,14 +239,15 @@
             parser.error(
                 "The provided value_file has a different number of entries "
                 "than the provided .tri file with facet vertices."
             )
 
     values["geometry"] = polys
     gdf = geopandas.GeoDataFrame(values, crs=t_crs)
+    logger.info(gdf.describe())
 
     if not args.keep_all_facets:
         logger.info("Dissolving polygons.")
         gdf = gdf.dissolve(by=value_keys[0])
 
     if args.csv:
         gdf.to_file(outfile.with_suffix(".csv"), driver="CSV")
@@ -284,14 +295,17 @@
     v3 = transformer.transform(in_m[6], in_m[7], in_m[8])
 
     if z:
         poly = Polygon([v1, v2, v3])
     else:
         poly = Polygon([v1[:-1], v2[:-1], v3[:-1]])
 
+    if poly.area == 0:
+        raise ValueError(f"This polygon has zero area: {poly}")
+
     return poly
 
 
 def replace_with(replacement_val, replacement_check, value):
     if float(value) == replacement_check:
         return replacement_val
     else:
```

### Comparing `vipersci-0.4.0/src/vipersci/msolo.py` & `vipersci-0.5.0/src/vipersci/msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/nirvss.py` & `vipersci-0.5.0/src/vipersci/nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/nss.py` & `vipersci-0.5.0/src/vipersci/nss.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 # Reuse is permitted under the terms of the license.
 # The AUTHORS file and the LICENSE file are at the
 # top level of this library.
 
 import logging
-import os
-from typing import Any, Generator, List, Sequence, Union
+from typing import Any, Iterable, Sequence, Union
+from os import PathLike
 
 import numpy as np
+import numpy.typing as npt
 from scipy.interpolate import RegularGridInterpolator
 
 logger = logging.getLogger(__name__)
 
 # type alias for the exhaustive variety of arguments that np.genfromtxt() takes.
-Readable = Union[os.PathLike, str, List[str], Generator[Union[str, bytes], Any, Any]]
+Readable = Union[str, PathLike, Iterable[str], Iterable[bytes]]
 
 
 class DataSimulator:
     """
     The DataSimulator object is initiated with inverse model model files,
     and then can be called to return simulated detector
     data given burial depth and water equivalent hydrogen values.
@@ -136,16 +137,16 @@
         self.det1_model = model(bd_mod, bounds_error=False, fill_value=fill_value)
         self.det2_model = model(weh_mod, bounds_error=False, fill_value=fill_value)
         self.fill_value = fill_value
         return
 
     def __call__(
         self,
-        det1: Union[float, Sequence[float], np.typing.ArrayLike],
-        det2: Union[float, Sequence[float], np.typing.ArrayLike],
+        det1: Union[float, Sequence[float], npt.ArrayLike],
+        det2: Union[float, Sequence[float], npt.ArrayLike],
     ):
         """
         Returns model-provided burial depth, water equivalent hydrogen, and
         uniform water equivalent hydrogen values.
 
         :param det1:  A single value or sequence of detector 1 values.
         :param det2: A single value or sequence of detector 2 values.
@@ -231,15 +232,15 @@
         arr = np.flipud(arr)
 
     # arr is in [row, col] order.
     return arr, row_coords, col_coords
 
 
 def uniform_weh(
-    measured: Union[float, Sequence[float], np.typing.ArrayLike],
+    measured: Union[float, Sequence[float], npt.ArrayLike],
     c0: float = 30.75,
     a: float = 0.0256,
     b: float = 1.0990,
     bounds_error: bool = True,
     fill_value: Any = np.nan,
 ):
     """Returns fraction of water equivalent hydrogen.
```

### Comparing `vipersci-0.4.0/src/vipersci/pds/datetime.py` & `vipersci-0.5.0/src/vipersci/pds/datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/pds/pid.py` & `vipersci-0.5.0/src/vipersci/pds/pid.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,56 +32,79 @@
     ncr="NavCam Right",
     hfp="HazCam Forward Port",
     hfs="HazCam Forward Starboard",
     hap="HazCam Aft Port",
     has="HazCam Aft Starboard",
     acl="AftCam Left",
     acr="AftCam Right",
+    pan="Panorama",  # Not an instrument, but a valid combined product type.
 )
 vis_instrument_aliases = {
     "navcam left": "ncl",
     "navcam right": "ncr",
     "aftcam left": "acl",
     "aftcam right": "acr",
     "hazcam forward port": "hfp",
     "hazcam forward starboard": "hfs",
     "hazcam aft port": "hap",
     "hazcam aft starboard": "has",
     "hazcam front left": "hfp",
     "hazcam front right": "hfs",
     "hazcam back left": "hap",
     "hazcam back right": "has",
+    "hazcam_1": "hfp",
+    "hazcam_2": "hap",
+    "hazcam_3": "hfs",
+    "hazcam_4": "has",
+}
+vis_instrument_numbers = {
+    0: "ncl",
+    1: "ncr",
+    2: "acl",
+    3: "acr",
+    4: "hfp",
+    5: "hfs",
+    6: "hap",
+    7: "has",
 }
 instruments.update(vis_instruments)
 vis_compression = dict(
-    a=None,  # Lossless compression
+    a=1,  # 1:1 Lossless compression
     b=5,  # 5:1 compression
     c=16,  # 16:1 compression
     d=64,  # 64:1 compression
     s="SLoG",  # SLoG compression
+    z=None,  # Uncompressed
 )
 
 nirvss_instruments = dict(
     aim="Ames Imaging Module",
 )
 instruments.update(nirvss_instruments)
 
 # Create some compiled regex Patterns to use in this module.
 date_re = re.compile(r"(2\d)(1[0-2]|0[1-9])(3[01]|[12][0-9]|0[1-9])")  # YYMMDD
 time_re = re.compile(r"(2[0-3]|[01]\d)([0-5]\d)([0-5]\d)(\d{3})?")  # hhmmssfff
 inst_re = re.compile("|".join(instruments.keys()))
+vis_inst_re = re.compile("|".join(vis_instruments.keys()))
 
 pid_re = re.compile(
     rf"(?P<date>{date_re.pattern})-"
     rf"(?P<time>{time_re.pattern})-"
     rf"(?P<instrument>{inst_re.pattern})"
 )
 
 vis_comp_re = re.compile("|".join(vis_compression.keys()))
 vis_pid_re = re.compile(pid_re.pattern + rf"-(?P<compression>{vis_comp_re.pattern})")
+vis_pan_re = re.compile(
+    f"(?P<date>{date_re.pattern})-"
+    rf"(?P<time>{time_re.pattern})-"
+    rf"((?P<instrument>{vis_inst_re.pattern})-)?"
+    rf"pan"
+)
 
 
 def get_key(value, dictionary):
     for k, v in dictionary.items():
         if v == value:
             return k
     else:
@@ -165,14 +188,17 @@
             return (
                 self.date == other.date
                 and self.time == other.time
                 and self.instrument == other.instrument
             )
         return False
 
+    def __hash__(self):
+        return hash((self.date, self.time, self.instrument))
+
     def __lt__(self, other):
         if isinstance(other, self.__class__):
             return (
                 self.date,
                 self.time,
                 self.instrument,
             ) < (
@@ -285,20 +311,15 @@
                         f"{args} did not match regex: {vis_pid_re.pattern}"
                     )
         elif len(args) == 4:
             (date, time, instrument, compression) = args
         else:
             raise IndexError("accepts 1 or 4 arguments")
 
-        if instrument in vis_instruments:
-            pass
-        elif instrument.casefold() in vis_instrument_aliases:
-            instrument = vis_instrument_aliases[instrument.casefold()]
-        else:
-            raise ValueError(f"{instrument} is not a VIS instrument.")
+        instrument = self.instrument_name(instrument)
 
         if compression in vis_compression:
             pass
         elif compression in vis_compression.values():
             compression = get_key(compression, vis_compression)
         else:
             raise ValueError(f"{args[3]} is not one of {vis_compression.keys()}")
@@ -310,32 +331,71 @@
         return "-".join((super().__str__(), self.compression))
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return super().__eq__(other) and self.compression == other.compression
         return False
 
+    def __hash__(self):
+        return hash((super().__hash__(), self.compression))
+
     def __lt__(self, other):
         if isinstance(other, self.__class__):
             if super().__eq__(other):
                 return self.compression < other.compression
             else:
                 return super().__lt__(other)
         else:
             return NotImplemented
 
     @staticmethod
     def instrument_name(name):
         """Returns fullname of VIS instrument based on *name*."""
+        if isinstance(name, int):
+            return vis_instruments[vis_instrument_numbers[name]]
         if name.casefold() in vis_instruments:
             return vis_instruments[name.casefold()]
         elif name.casefold() in vis_instrument_aliases:
             return vis_instruments[vis_instrument_aliases[name.casefold()]]
         else:
-            raise ValueError(f"No instrument name based on {name} could be found.")
+            raise ValueError(f"No VIS instrument name based on {name} could be found.")
 
     def compression_class(self):
         """Returns text value for the PDS onboard_compression_class."""
         if self.compression == "a" or self.compression == "s":
             return "Lossless"
         else:
             return "Lossy"
+
+
+class PanoID(VIPERID):
+    """A Class for VIPER VIS Panorama Product IDs.  The date/time combination
+       should be equal to the earliest source product date/time combination.
+
+    :ivar date: a six digit string denoting YYMMDD (or strftime %y%m%d) where
+        the two digit year can be prefixed with "20" to get the four-digit year.
+    :ivar time: a six or nine digit string denoting hhmmss (or strftime
+        %H%M%S%f) or hhmmssuuu, similar to the first, but where the trailing
+        three digits are miliseconds.
+    :ivar instrument: A three character sequence denoting the instrument (if all
+        source data came from the same instrument), can be None (indicating multiple
+        instruments contributed).
+    """
+
+    def __init__(self, *args):
+        if len(args) == 1:
+            match = vis_pan_re.search(str(args).lower())
+            if not match:
+                raise ValueError(f"{args} did not match regex: {vis_pan_re.pattern}")
+        elif 2 <= len(args) <= 3:
+            instrument = args[-1]
+            VISID.instrument_name(instrument)
+
+        super().__init__(*args)
+        if self.instrument == "pan":
+            self.instrument = None
+
+    def __str__(self):
+        if self.instrument in ("pan", None):
+            return "-".join((self.date, self.time, "pan"))
+        else:
+            return "-".join((self.date, self.time, self.instrument, "pan"))
```

### Comparing `vipersci-0.4.0/src/vipersci/pds/xml.py` & `vipersci-0.5.0/src/vipersci/pds/xml.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/util.py` & `vipersci-0.5.0/src/vipersci/util.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/vis/db/create_vis_dbs.py` & `vipersci-0.5.0/src/vipersci/vis/db/create_vis_dbs.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/vis/db/raw_products.py` & `vipersci-0.5.0/src/vipersci/vis/db/raw_products.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,264 +22,281 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 # Reuse is permitted under the terms of the license.
 # The AUTHORS file and the LICENSE file are at the
 # top level of this library.
 
 from datetime import datetime, timedelta, timezone
+from enum import Flag
 from warnings import warn
 import xml.etree.ElementTree as ET
 
 from sqlalchemy import (
     Boolean,
-    Column,
     DateTime,
     Float,
     Identity,
     Integer,
     String,
 )
 from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.orm import declarative_base, synonym, validates
+from sqlalchemy.orm import mapped_column, synonym, validates
 
 from vipersci.pds.pid import VISID, vis_instruments, vis_compression
 from vipersci.pds.xml import ns
 from vipersci.pds.datetime import fromisozformat, isozformat
 from vipersci.vis.header import pga_gain as header_pga_gain
+from vipersci.vis.db import Base
+import vipersci.vis.db.validators as vld
 
 
-Base = declarative_base()
-
 luminaire_names = {
     "NavLight Left": "navlight_left_on",
     "NavLight Right": "navlight_right_on",
     "HazLight Aft Port": "hazlight_aft_port_on",
     "HazLight Aft Starboard": "hazlight_aft_starboard_on",
     "HazLight Center Port": "hazlight_center_port_on",
     "HazLight Center Starboard": "hazlight_center_starboard_on",
     "HazLight Fore Port": "hazlight_fore_port_on",
     "HazLight Fore Starboard": "hazlight_fore_starboard_on",
 }
 
 
+class ImageType(Flag):
+    """This Flag class can be used to interpret the outputImageMask but not the
+    immediateDownloadInfo Yamcs parameters, because only a single flag value can
+    be set."""
+
+    LOSSLESS_ICER_IMAGE = 1
+    # RESERVED_2 = 2
+    # RESERVED_4 = 4
+    LOSSY_ICER_IMAGE = 8
+    SLOG_ICER_IMAGE = 16
+
+    @classmethod
+    def _missing_(cls, value):
+        return None
+
+
+class ProcessingStage(Flag):
+    # PROCESS_RESERVED = 1
+    PROCESS_FLATFIELD = 2
+    # PROCESS_RESERVED_2 = 4
+    PROCESS_LINEARIZATION = 8
+    PROCESS_SLOG = 16
+
+
 class RawProduct(Base):
     """An object to represent rows in the raw_products table for VIS."""
 
-    # This class is derived from SQLAlchemy's orm.declarative_base()
+    # This class is derived from SQLAlchemy's orm.DeclarativeBase
     # which means that it has a variety of class properties that are
     # then swept up into properties on the instantiated object via
     # super().__init__().
 
     # The table represents many of these objects, so the __tablename__ is
     # plural while the class name is singular.
     __tablename__ = "raw_products"
 
-    # The Column() names below should use "snake_case" for the names that are
+    # The mapped_column() names below should use "snake_case" for the names that are
     # committed to the database as column names.  Furthermore, those names
     # should be similar, if not identical, to the PDS4 Class and Attribute
     # names that they represent.  Other names (like Yamcs parameter camelCase
     # names) are implemented as synonyms. Aside from the leading "id" column,
     # the remainder are in alphabetical order, since there are so many.
 
-    id = Column(Integer, Identity(start=1), primary_key=True)
-    adc_gain = Column(
+    id = mapped_column(Integer, Identity(start=1), primary_key=True)
+    adc_gain = mapped_column(
         Integer, nullable=False, doc="ADC_GAIN from the MCSE Image Header."
     )
     adcGain = synonym("adc_gain")
-    auto_exposure = Column(
+    auto_exposure = mapped_column(
         Boolean,
         nullable=False,
         doc="AUTO_EXPOSURE from the MCSE Image Header.",
     )
     autoExposure = synonym("auto_exposure")
-    bad_pixel_table_id = Column(
+    bad_pixel_table_id = mapped_column(
         Integer,
         nullable=False,
         # There is a Defective Pixel Map (really a list of 128 coordinates) for
         # each MCAM.  The "state" of this is managed by the ground and not
         # reflected in any Image Header information attached to an individual
         # image.  It is not clear how to obtain this information from Yamcs,
         # or even what might be recorded, so this column's value is TBD.
     )
-    cameraId = synonym(
-        "mcam_id"
-    )  # This value maybe isn't the mcam_id since it is 0-7 from Yamcs?
-    capture_id = Column(
+    capture_id = mapped_column(
         Integer,
         nullable=False,
         doc="The captureId from the command sequence."
         # TODO: learn more about captureIds to provide better doc here.
     )
     captureId = synonym("capture_id")
-    _exposure_duration = Column(
+    _exposure_duration = mapped_column(
         "exposure_duration",
         Integer,
         nullable=False,
         doc="The exposure time in microseconds, the result of decoding the "
         "EXP_STEP and EXP paramaters from the MCSE Image Header.",
     )
     exposureTime = synonym("exposure_duration")  # Yamcs parameter name.
-    file_creation_datetime = Column(
+    file_creation_datetime = mapped_column(
         DateTime(timezone=True),
         nullable=False,
         doc="The time at which file_name was created.",
     )
-    file_md5_checksum = Column(
+    file_md5_checksum = mapped_column(
         String,
         nullable=False,
         doc="The md5 checksum of the file described by file_path.",
     )
-    file_path = Column(
+    file_path = mapped_column(
         String,
         nullable=False,
         doc="The absolute path (POSIX style) that contains the Array_2D_Image "
         "that this metadata refers to.",
     )
     # Not sure where we're getting info for these light booleans yet.
-    hazlight_aft_port_on = Column(Boolean, nullable=False)
-    hazlight_aft_starboard_on = Column(Boolean, nullable=False)
-    hazlight_center_port_on = Column(Boolean, nullable=False)
-    hazlight_center_starboard_on = Column(Boolean, nullable=False)
-    hazlight_fore_port_on = Column(Boolean, nullable=False)
-    hazlight_fore_starboard_on = Column(Boolean, nullable=False)
-    image_id = Column(
+    hazlight_aft_port_on = mapped_column(Boolean, nullable=False)
+    hazlight_aft_starboard_on = mapped_column(Boolean, nullable=False)
+    hazlight_center_port_on = mapped_column(Boolean, nullable=False)
+    hazlight_center_starboard_on = mapped_column(Boolean, nullable=False)
+    hazlight_fore_port_on = mapped_column(Boolean, nullable=False)
+    hazlight_fore_starboard_on = mapped_column(Boolean, nullable=False)
+    image_id = mapped_column(
         Integer,
         nullable=False,
         doc="The IMG_ID from the MCSE Image Header used for CCU storage and "
         "retrieval.",
     )
     imageHeight = synonym("lines")
     imageId = synonym("image_id")
     imageWidth = synonym("samples")
-    instrument_name = Column(
+    instrument_name = mapped_column(
         String, nullable=False, doc="The full name of the instrument."
     )
-    instrument_temperature = Column(
+    instrument_temperature = mapped_column(
         Float,
         nullable=False,
         doc="The TEMPERATURE from the MCSE Image Header.  TBD how to convert "
         "this 16-bit integer into degrees C.",
     )
     # There is a sensor in the camera body (PT1000) which is apparently not
     # connected (sigh).  And there is also a sensor external to each camera
     # body (AD590), need to track down its Yamcs feed.
-    lines = Column(
+    lines = mapped_column(
         Integer,
         nullable=False,
         doc="The imageHeight parameter from the Yamcs imageHeader.",
     )
-    _lobt = Column(
+    _lobt = mapped_column(
         "lobt",
         Integer,
         nullable=False,
         doc="The TIME_TAG from the MCSE Image Header.",
     )
-    mcam_id = Column(
-        Integer, nullable=False, doc="The MCAM_ID from the MCSE Image Header."
-    )
-    mission_phase = Column(
+    # mcam_id, The MCAM_ID from the MCSE Image Header is not returned to the ground.
+    mission_phase = mapped_column(
         String,
         nullable=False,
         # Not sure what form this will take, nor where it can be looked up.
     )
-    navlight_left_on = Column(Boolean, nullable=False)
-    navlight_right_on = Column(Boolean, nullable=False)
-    offset = Column(
+    navlight_left_on = mapped_column(Boolean, nullable=False)
+    navlight_right_on = mapped_column(Boolean, nullable=False)
+    offset = mapped_column(
         Integer,
         nullable=False,
         doc="The OFFSET parameter from the MCSE Image Header describing the dark "
         "level offset.",
     )
-    onboard_compression_ratio = Column(
+    onboard_compression_ratio = mapped_column(
         Float,
         doc="The PDS img:Onboard_Compression parameter.  Will be NULL for "
         "lossless compression or uncompressed images."
         # This is a PDS img:Onboard_Compression parameter which is the ratio
         # of the size, in bytes, of the original uncompressed data object
         # to its compressed size.  This operation is done by RFSW, but not
         # sure where to get this parameter from ...?
     )
-    output_image_mask = Column(
+    output_image_mask = mapped_column(
         Integer,
         nullable=False,
-        doc="The outputImageMask from the Yamcs imageHeader."
-        # TODO: learn more about outputImageMask to provide better doc here.
-    )
-    output_image_type = Column(
-        String,
-        nullable=False,
-        doc="The outputImageType from the Yamcs imageHeader."
-        # TODO: learn more about outputImageType to provide better doc here.
+        doc="The outputImageMask from the Yamcs imageHeader.  For each downlinked "
+        "image this can be exactly one value of the ImageType class.  This value "
+        "indicates whether the image is SLoG or not, and what level of compression "
+        "has been set.",
     )
+    # outputImageType is redundant with the outputImageMask, as it is just the
+    # longform name of the value specified in the outputImageMask.
     outputImageMask = synonym("output_image_mask")
-    outputImageType = synonym("output_image_type")
-    _pid = Column(
+    _pid = mapped_column(
         "product_id", String, nullable=False, unique=True, doc="The PDS Product ID."
     )
-    padding = Column(
+    padding = mapped_column(
         Integer,
         nullable=False,
         doc="The padding parameter from the Yamcs imageHeader.",
         # Not sure what this value means or where it comes from.
     )
-    pga_gain = Column(
+    pga_gain = mapped_column(
         Float,
         nullable=False,
         doc="The translated floating point multiplier derived from PGA_GAIN "
         "from the MCSE Image Header.",
     )
     ppaGain = synonym("pga_gain")  # Surely, this is a Yamcs typo, should be pgaGain
-    processing_info = Column(
+    processing_info = mapped_column(
         Integer,
         nullable=False,
-        doc="The processingInfo parameter from the Yamcs imageHeader."
-        # TODO: learn more about processingInfo to provide better doc here.
+        doc="The processingInfo parameter from the Yamcs imageHeader. This integer "
+        "value must correspond to a valid value of ProcessingStage, and indicates "
+        "what onboard processing occurred.",
     )
     processingInfo = synonym("processing_info")
-    purpose = Column(
+    purpose = mapped_column(
         String,
         nullable=False,
         doc="This is the value for the PDS "
         "Observation_Area/Primary_Result_Summary/purpose parameter, it "
         "has a restricted set of allowable values.",
     )
-    samples = Column(
+    samples = mapped_column(
         Integer,
         nullable=False,
         doc="The imageWidth parameter from the Yamcs imageHeader.",
     )
-    slog = Column(
+    slog = mapped_column(
         Boolean,
         nullable=False,
         doc="Indicates whether onboard SLoG processing occurred.",
     )
-    software_name = Column(String, nullable=False)
-    software_version = Column(String, nullable=False)
-    software_program_name = Column(String, nullable=False)
-    start_time = Column(DateTime(timezone=True), nullable=False)
-    stereo = Column(
+    software_name = mapped_column(String, nullable=False)
+    software_version = mapped_column(String, nullable=False)
+    software_program_name = mapped_column(String, nullable=False)
+    start_time = mapped_column(DateTime(timezone=True), nullable=False)
+    stereo = mapped_column(
         Boolean,
         nullable=False,
         doc="The stereo parameter from the Yamcs imageHeader."
         # TODO: learn more about stereo to provide better doc here.
     )
-    stop_time = Column(DateTime(timezone=True), nullable=False)
+    stop_time = mapped_column(DateTime(timezone=True), nullable=False)
     temperature = synonym("instrument_temperature")
-    voltage_ramp = Column(
+    voltage_ramp = mapped_column(
         Integer,
         nullable=False,
         doc="The VOLTAGE_RAMP parameter from the MCSE Image Header.",
     )
     voltageRamp = synonym("voltage_ramp")
-    yamcs_generation_time = Column(
+    yamcs_generation_time = mapped_column(
         DateTime(timezone=True),
         nullable=False,
         doc="The generation time of the source record from Yamcs.",
     )
-    yamcs_name = Column(
+    yamcs_name = mapped_column(
         String,
         nullable=False,
         doc="The full parameter name from Yamcs that this product data came from, "
         "formatted like a / separated string.",
     )
 
     def __init__(self, **kwargs):
@@ -338,17 +355,59 @@
         elif "yamcs_name" in kwargs:
             maybe_name = self.yamcs_name.split("/")[-1].replace("_", " ")
             if maybe_name.endswith((" icer", " jpeg", " slog")):
                 maybe_name = maybe_name[:-5]
 
             self.instrument_name = VISID.instrument_name(maybe_name)
 
+        if "cameraId" in otherargs:
+            if VISID.instrument_name(otherargs["cameraId"]) != self.instrument_name:
+                warn(
+                    f"cameraId ({otherargs['cameraId']}) does not match the "
+                    f"instrument_name ({self.instrument_name})."
+                )
+
         # Derive slog, if possible.
-        if "slog" not in kwargs and "yamcs_name" in kwargs:
-            self.slog = self.yamcs_name.endswith("slog")
+        if self.processing_info is not None:
+            try:
+                if "slog" in kwargs:
+                    # check against processing_info
+                    if kwargs[
+                        "slog"
+                    ] and ProcessingStage.PROCESS_SLOG not in ProcessingStage(
+                        self.processing_info
+                    ):
+                        warn(
+                            "slog is True, but ProcessingStage.PROCESS_SLOG not "
+                            f"in {ProcessingStage(self.processing_info)}"
+                        )
+
+                    if not kwargs[
+                        "slog"
+                    ] and ProcessingStage.PROCESS_SLOG in ProcessingStage(
+                        self.processing_info
+                    ):
+                        warn(
+                            "slog is False, but ProcessingStage.PROCESS_SLOG "
+                            f"in {ProcessingStage(self.processing_info)}"
+                        )
+                else:
+                    if ProcessingStage.PROCESS_SLOG in ProcessingStage(
+                        self.processing_info
+                    ):
+                        self.slog = True
+                    else:
+                        self.slog = False
+            except ValueError as err:
+                warn(str(err))
+                if "slog" not in kwargs and "yamcs_name" in kwargs:
+                    self.slog = self.yamcs_name.endswith("slog")
+        else:
+            if "slog" not in kwargs and "yamcs_name" in kwargs:
+                self.slog = self.yamcs_name.endswith("slog")
 
         # Ensure product_id consistency
         if pid:
             if "lobt" in kwargs:
                 if pid.datetime() != lobt_dt:
                     raise ValueError(
                         f"The product_id datetime ({pid.datetime()}) and the "
@@ -424,37 +483,37 @@
 
         return
 
     @hybrid_property
     def exposure_duration(self):
         return self._exposure_duration
 
-    @exposure_duration.setter
-    def exposure_duration(self, value: int):
+    @exposure_duration.inplace.setter
+    def _exposure_duration_setter(self, value: int):
         """Takes an exposure time in microseconds."""
         self._exposure_duration = value
         self.stop_time = self.start_time + timedelta(microseconds=value)
 
     @hybrid_property
     def lobt(self):
         return self._lobt
 
-    @lobt.setter
-    def lobt(self, lobt):
+    @lobt.inplace.setter
+    def _lobt_setter(self, lobt):
         self._lobt = lobt
         self.start_time = datetime.fromtimestamp(lobt, tz=timezone.utc)
 
     @hybrid_property
     def product_id(self):
         # Really am going back and forth about whether this should be returned as
         # a full VISID object or just as the string as it is now.
         return self._pid
 
-    @product_id.setter
-    def product_id(self, pid):
+    @product_id.inplace.setter
+    def _product_id_setter(self, pid):
         # In this class, the source of product_id information really is what
         # comes from Yamcs, and so this should not be monkeyed with.  Theoretically
         # changing this would imply changes to start time, lobt, stop time,
         # intrument name and onboard_compression_ratio directly, but those changes then
         # also divorce this object from the Yamcs parameters that it came from and
         # has all manner of other implications.  So at this time, this can only be
         # set when this object is instantiated.
@@ -462,59 +521,44 @@
             "product_id cannot be set directly after instantiation."
         )
 
     @validates("pga_gain")
     def validate_pga_gain(self, key, value):
         return header_pga_gain(value)
 
-    @validates("mcam_id")
-    def validate_mcam_id(self, key, value: int):
-        s = {0, 1, 2, 3, 4}
-        if value not in s:
-            # raise ValueError(f"mcam_id must be one of {s}, but is {value}")
-            warn(f"mcam_id must be one of {s}, but is {value}")
-        return value
-
     @validates(
         "file_creation_datetime",
         "start_time",
         "stop_time",
         "yamcs_generation_time",
     )
     def validate_datetime_asutc(self, key, value):
-        if isinstance(value, datetime):
-            if value.utcoffset() is None:
-                raise ValueError(f"{key} must be tz aware.")
-            dt = value
-        elif isinstance(value, str):
-            if value.endswith("Z"):
-                dt = fromisozformat(value)
-            else:
-                dt = datetime.fromisoformat(value)
-        else:
-            raise ValueError(
-                f"{key} must be a datetime or an ISO 8601 formatted string."
-            )
+        return vld.validate_datetime_asutc(key, value)
 
-        return dt.astimezone(timezone.utc)
+    @validates("output_image_mask")
+    def validate_output_image_mask(self, key, value):
+        try:
+            ImageType(value)
+        except ValueError:
+            warn(f"{key} ({value}) is not one of {list(ImageType)}")
+
+        return value
+
+    @validates("processing_info")
+    def validate_processing_info(self, key, value):
+        try:
+            ProcessingStage(value)
+        except ValueError:
+            warn(f"{key} ({value}) is not one of {list(ProcessingStage)}")
+
+        return value
 
     @validates("purpose")
     def validate_purpose(self, key, value: str):
-        s = {
-            "Calibration",
-            "Checkout",
-            "Engineering",
-            "Navigation",
-            "Observation Geometry",
-            "Science",
-            "Supporting Observation",
-        }
-        if value not in s:
-            raise ValueError(f"purpose must be one of {s}")
-        return value
+        return vld.validate_purpose(value)
 
     def asdict(self):
         d = {}
 
         for c in self.__table__.columns:
             if isinstance(getattr(self, c.name), datetime):
                 d[c.name] = isozformat(getattr(self, c.name))
@@ -529,93 +573,107 @@
     def from_xml(cls, text: str):
         """
         Returns an instantiated RawProduct object from parsing the provided *text*
         as XML.
         """
         d = {}
 
+        def _find_text(root, xpath, unit_check=None):
+            element = root.find(xpath, ns)
+            if element is not None:
+                if unit_check is not None:
+                    if element.get("unit") != unit_check:
+                        raise ValueError(
+                            f"The {xpath} element does not have units of "
+                            f"{unit_check}, has {element.get('unit')}"
+                        )
+                el_text = element.text
+                if el_text:
+                    return el_text
+                else:
+                    raise ValueError(
+                        f"The XML {xpath} element contains no information."
+                    )
+            else:
+                raise ValueError(f"XML text does not have a {xpath} element.")
+
         root = ET.fromstring(text)
-        lid = root.find(
-            "./pds:Identification_Area/pds:logical_identifier", ns
-        ).text.split(":")
+        lid = _find_text(
+            root, "./pds:Identification_Area/pds:logical_identifier"
+        ).split(":")
+
         if lid[3] != "viper_vis":
             raise ValueError(
                 f"XML text has a logical_identifier which is not viper_vis: {lid[3]}"
             )
 
         if lid[4] != "raw":
             raise ValueError(
                 f"XML text has a logical_identifier which is not raw: {lid[4]}"
             )
         d["product_id"] = lid[5]
 
         d["auto_exposure"] = (
-            True if root.find(".//img:exposure_type", ns).text == "Auto" else False
+            True if _find_text(root, ".//img:exposure_type") == "Auto" else False
         )
         d["bad_pixel_table_id"] = int(
-            root.find(".//img:bad_pixel_replacement_table_id", ns).text
+            _find_text(root, ".//img:bad_pixel_replacement_table_id")
         )
-        exp_dur = root.find(".//img:exposure_duration", ns)
-        if exp_dur.get("unit") != "microseconds":
-            raise ValueError(
-                "The img:exposure_duration element does not have units of "
-                f"microseconds, has {exp_dur.get('unit')}"
-            )
-        d["exposure_duration"] = int(exp_dur.text)
+        d["exposure_duration"] = int(
+            _find_text(root, ".//img:exposure_duration", unit_check="microseconds")
+        )
+
         d["file_creation_datetime"] = fromisozformat(
-            root.find(".//pds:creation_date_time", ns).text
+            _find_text(root, ".//pds:creation_date_time")
         )
-        d["file_path"] = root.find(".//pds:file_name", ns).text
+        d["file_path"] = _find_text(root, ".//pds:file_name")
 
         for k, v in luminaire_names.items():
             light = root.find(f".//img:LED_Illumination_Source[img:name='{k}']", ns)
             d[v] = (
-                True if light.find("img:illumination_state", ns).text == "On" else False
+                True if _find_text(light, "img:illumination_state") == "On" else False
             )
 
         osc = root.find(".//pds:Observing_System_Component[pds:type='Instrument']", ns)
-        d["instrument_name"] = osc.find("pds:name", ns).text
+        d["instrument_name"] = _find_text(osc, "pds:name")
 
-        temp = root.find(".//img:temperature_value", ns)
-        if temp.get("unit") != "K":
-            raise ValueError(
-                "The img:temperature_value element does not have units of K, has "
-                f"{temp.get('unit')}"
-            )
-        d["instrument_temperature"] = float(temp.text)
+        d["instrument_temperature"] = float(
+            _find_text(root, ".//img:temperature_value", unit_check="K")
+        )
 
         aa = root.find(".//pds:Axis_Array[pds:axis_name='Line']", ns)
-        d["lines"] = int(aa.find("./pds:elements", ns).text)
-        d["file_md5_checksum"] = root.find(".//pds:md5_checksum", ns).text
-        d["mission_phase"] = root.find(".//msn:mission_phase_name", ns).text
-        d["offset"] = root.find(".//img:analog_offset", ns).text
-
-        ocr = root.find(".//img:onboard_compression_ratio", ns)
-        if ocr is not None:
-            d["onboard_compression_ratio"] = float(ocr.text)
+        d["lines"] = int(_find_text(aa, "./pds:elements"))
+        d["file_md5_checksum"] = _find_text(root, ".//pds:md5_checksum")
+        d["mission_phase"] = _find_text(root, ".//msn:mission_phase_name")
+        d["offset"] = _find_text(root, ".//img:analog_offset")
+
+        try:
+            d["onboard_compression_ratio"] = float(
+                _find_text(root, ".//img:onboard_compression_ratio")
+            )
+        except ValueError:
+            pass
 
-        d["purpose"] = root.find(".//pds:purpose", ns).text
+        d["purpose"] = _find_text(root, ".//pds:purpose")
 
         aa = root.find(".//pds:Axis_Array[pds:axis_name='Sample']", ns)
-        d["samples"] = int(aa.find("./pds:elements", ns).text)
+        d["samples"] = int(_find_text(aa, "./pds:elements"))
 
         sw = root.find(".//proc:Software", ns)
-        d["software_name"] = sw.find("./proc:name", ns).text
-        d["software_version"] = sw.find("./proc:software_version_id", ns).text
-        d["software_program_name"] = sw.find(
-            "./proc:Software_Program/proc:name", ns
-        ).text
+        d["software_name"] = _find_text(sw, "./proc:name")
+        d["software_version"] = _find_text(sw, "./proc:software_version_id")
+        d["software_program_name"] = _find_text(sw, "./proc:Software_Program/proc:name")
 
         # Start times must be on the whole second, which is why we don't use
         # fromisozformat() here.
         d["start_time"] = datetime.strptime(
-            root.find(".//pds:start_date_time", ns).text, "%Y-%m-%dT%H:%M:%SZ"
+            _find_text(root, ".//pds:start_date_time"), "%Y-%m-%dT%H:%M:%SZ"
         ).replace(tzinfo=timezone.utc)
 
-        d["stop_time"] = fromisozformat(root.find(".//pds:stop_date_time", ns).text)
+        d["stop_time"] = fromisozformat(_find_text(root, ".//pds:stop_date_time"))
 
         return cls(**d)
 
     def label_dict(self):
         """Returns a dictionary suitable for label generation."""
         _inst = self.instrument_name.lower().replace(" ", "_")
         _sclid = "urn:nasa:pds:context:instrument_host:spacecraft.viper"
@@ -624,29 +682,35 @@
         d = dict(
             lid=f"urn:nasa:pds:viper_vis:raw:{self.product_id}",
             mission_lid="urn:nasa:pds:viper",
             sc_lid=_sclid,
             inst_lid=f"{_sclid}.{_inst}",
             gain_number=(self.adc_gain * self.pga_gain),
             exposure_type="Auto" if self.auto_exposure else "Manual",
-            image_filter=None,
+            image_filters=list(),
             led_wavelength=453,  # nm
             luminaires={},
             compression_class=pid.compression_class(),
             onboard_compression_type="ICER",
             sample_bits=12,
             sample_bit_mask="2#0000111111111111",
         )
         for k, v in luminaire_names.items():
             d["luminaires"][k] = onoff[getattr(self, v)]
 
+        proc_info = ProcessingStage(self.processing_info)
+        if ProcessingStage.PROCESS_FLATFIELD in proc_info:
+            d["image_filters"].append(("Onboard", "Flat field normalization."))
+
+        if ProcessingStage.PROCESS_LINEARIZATION in proc_info:
+            d["image_filters"].append(("Onboard", "Linearization."))
+
         if self.slog:
-            d["image_filter"] = dict(
-                processing_venue="Onboard",
-                processing_algorithm="Sign of the Laplacian of the Gaussian, SLoG",
+            d["image_filters"].append(
+                ("Onboard", "Sign of the Laplacian of the Gaussian, SLoG")
             )
             d["sample_bits"] = 8
             d["sample_bit_mask"] = "2#11111111"
 
         d.update(self.asdict())
 
         return d
```

### Comparing `vipersci-0.4.0/src/vipersci/vis/db/raw_stats.py` & `vipersci-0.5.0/src/vipersci/vis/db/raw_stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 # Reuse is permitted under the terms of the license.
 # The AUTHORS file and the LICENSE file are at the
 # top level of this library.
 
 from sqlalchemy import (
-    Column,
     Float,
     ForeignKey,
     Identity,
     Integer,
     String,
 )
-from sqlalchemy.orm import backref, declarative_base, relationship
+from sqlalchemy.orm import backref, mapped_column, relationship
 
+from vipersci.vis.db import Base
 from vipersci.vis.db.raw_products import RawProduct
 
-Base = declarative_base()
-
 
 class RawStats(Base):
     """An object to represent rows in the raw_stats table for VIS."""
 
     __tablename__ = "raw_stats"
 
-    id = Column(Integer, Identity(start=1), primary_key=True)
-    product_id = Column(String, ForeignKey(RawProduct.product_id), nullable=False)
+    id = mapped_column(Integer, Identity(start=1), primary_key=True)
+    product_id = mapped_column(
+        String, ForeignKey(RawProduct.product_id), nullable=False
+    )
     raw_product = relationship(RawProduct, backref=backref("stats", uselist=False))
 
-    blur = Column(
+    blur = mapped_column(
         Float, nullable=False, doc="Blur metric from skimage.measure.blur_effect()."
     )
-    mean = Column(Float, nullable=False, doc="Image mean.")
-    std = Column(Float, nullable=False, doc="Image standard deviation.")
+    mean = mapped_column(Float, nullable=False, doc="Image mean.")
+    std = mapped_column(Float, nullable=False, doc="Image standard deviation.")
```

### Comparing `vipersci-0.4.0/src/vipersci/vis/header.py` & `vipersci-0.5.0/src/vipersci/vis/header.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/vis/image_statistics.py` & `vipersci-0.5.0/src/vipersci/vis/image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/vis/pds/create_raw.py` & `vipersci-0.5.0/src/vipersci/vis/pds/create_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import argparse
 from datetime import datetime, date, timezone
 import hashlib
 from importlib import resources
 import io
 import json
 import logging
-from typing import Union
+from typing import Union, Optional
 from pathlib import Path
 
 from genshi.template import MarkupTemplate
 import numpy as np
 import numpy.typing as npt
 from skimage.io import imread, imsave  # maybe just imageio here?
 from sqlalchemy import create_engine
@@ -174,30 +174,30 @@
     given, the current working directory will be used (beware!).  If *session* is not
     given, no writes to a database will occur.
     """
 
     def __init__(
         self,
         outdir: Path = Path.cwd(),
-        session: Session = None,
+        session: Optional[Session] = None,
     ):
         self.outdir = outdir
         self.session = session
 
-    def __call__(self, metadata: dict, image: ImageType = None):
+    def __call__(self, metadata: dict, image: Union[ImageType, Path, None] = None):
         rp = make_raw_product(metadata, image, self.outdir)
         logger.info(f"{rp.product_id} created.")
 
         write_json(rp.asdict(), self.outdir)
 
         if self.session is not None:
             with self.session.begin() as s:
                 s.add(rp)
 
-        return
+        return rp
 
     def from_yamcs_parameters(self, data):
         for parameter in data.parameters:
             logger.info(f"{parameter.generation_time} - {parameter.name}")
             # These are hard-coded until we figure out where they come from.
             d = {
                 "bad_pixel_table_id": 0,
@@ -220,20 +220,20 @@
                 im = imread(f)
 
             self.__call__(d, im)
 
 
 def create(
     metadata: dict,
-    image: Union[ImageType, Path] = None,
+    image: Union[ImageType, Path, None] = None,
     outdir: Path = Path.cwd(),
-    session: Union[Session, sessionmaker] = None,
+    session: Optional[Session] = None,
     json: bool = True,
     xml: bool = False,
-    template_path: Path = None,
+    template_path: Optional[Path] = None,
 ):
     """
     Creates a PDS4 XML label file in *outdir* based on the provided
     meta-data.  Returns None.
 
     If *image* is a numpy array, that array will be considered the
     Array_2D_Image and will be written to a TIFF file with the same
@@ -268,15 +268,15 @@
     if xml:
         write_xml(rp.label_dict(), outdir, template_path)
 
     if session is not None:
         with session.begin() as s:
             s.add(rp)
 
-    return
+    return rp
 
 
 def check_bit_depth(pid: pds.VISID, bit_depth: Union[int, str, np.dtype]):
     """If the provided *bit_depth* is incompatible with *pid* a ValueError will be
     raised.
 
     The *bit_depth* will attempt to be converted to a valid integer value the bit
@@ -311,15 +311,15 @@
                 f"This product ({pid}) should be 16-bit, but it is {bit_depth}"
             )
     return
 
 
 def make_raw_product(
     metadata: dict,
-    image: Union[ImageType, Path] = None,
+    image: Union[ImageType, Path, None] = None,
     outdir: Path = Path.cwd(),
 ) -> RawProduct:
     """
     Returns a Raw_Product created from the provided meta-data, and
     if *image* is a numpy array, it will also use write_tiff() to
     create a TIFF data product in *outdir* (defaults to current
     working directory).
@@ -427,15 +427,17 @@
     logger.debug(desc)
     outpath = (outdir / str(pid)).with_suffix(".tif")
 
     imsave(str(outpath), image, check_contrast=False, description=desc, metadata=None)
     return outpath
 
 
-def write_xml(product: dict, outdir: Path = Path.cwd(), template_path: Path = None):
+def write_xml(
+    product: dict, outdir: Path = Path.cwd(), template_path: Optional[Path] = None
+):
     """
     Writes a PDS4 XML label in *outdir* based on the contents of
     the *product* object, which must be of type Raw_Product.
 
     The *template_path* can be a path to an appropriate template
     XML file, but defaults to the raw-template.xml file provided
     with this library.
```

### Comparing `vipersci-0.4.0/src/vipersci/vis/pds/create_raw_tif.py` & `vipersci-0.5.0/src/vipersci/vis/pds/create_raw_tif.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci/vis/pds/template_test.py` & `vipersci-0.5.0/src/vipersci/vis/pds/template_test.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/src/vipersci.egg-info/PKG-INFO` & `vipersci-0.5.0/src/vipersci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.4.0
+Version: 0.5.0
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -89,15 +89,15 @@
 
 
 License
 -------
 
 See LICENSE file for the full text of the license that applies to vipersci.
 
-Copyright (c) 2022, United States Government as represented by
+Copyright (c) 2022-2023, United States Government as represented by
 the Administrator of the National Aeronautics and Space
 Administration. All rights reserved.
 
 The "vipersci" software is licensed under the Apache License, Version 2.0
 (the "License"); you may not use this file except in compliance with the
 License.  You may obtain a copy of the License at
 http://www.apache.org/licenses/LICENSE-2.0
@@ -137,14 +137,48 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+
+0.5.0 (2023-07-26)
+------------------
+
+Added
+^^^^^
+- PanoID class added to pds.pid
+- pano_products and create_pano added, still very preliminary, mostly just mock-ups.
+- colorforge program for managing colormaps.
+- mypy is now in the development dependencies to support type checking.
+- lint/mypy target added to Makefile.
+- tri2gpkg now has a --remove_facets option to remove facets with a particular value.
+
+
+Changed
+^^^^^^^
+- Explicit in documentation about developing in Python 3.8 (although earlier versions
+  should still be supported).
+- Many changes to improve type checking.
+- Added numeric instrument aliases and checking for them.
+- Added information for procesingInfo and outputMask from Yamcs.
+- Upgrade to SQLAlchemy >=2.
+- Moved definition of Base class up to vis.db.
+- heatmaps.py will now accept value data lists or arrays with np.nan or None values
+  which will be appropriate ignored in the density heatmap calculation.
+
+
+Fixed
+^^^^^
+- tri2gpkg - if the provided polygons have zero area, issue an error rather than
+  making a confusing GeoPackage file.
+
+
+
 0.4.0 (2023-03-01)
 ------------------
 
 Added
 ^^^^^
 - carto.bounds module added to unify functionality for both heatmaps and dotmaps.
 - carto.dotmap module for creating simple heatmap-like visualizations from 2d scalar data.
```

### Comparing `vipersci-0.4.0/src/vipersci.egg-info/SOURCES.txt` & `vipersci-0.5.0/src/vipersci.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -37,51 +37,64 @@
 src/vipersci.egg-info/entry_points.txt
 src/vipersci.egg-info/not-zip-safe
 src/vipersci.egg-info/requires.txt
 src/vipersci.egg-info/top_level.txt
 src/vipersci/carto/__init__.py
 src/vipersci/carto/accrual.py
 src/vipersci/carto/bounds.py
+src/vipersci/carto/colorforge.py
 src/vipersci/carto/dice_buffer.py
 src/vipersci/carto/dissolve_dice.py
 src/vipersci/carto/dotmap.py
 src/vipersci/carto/heatmap.py
 src/vipersci/carto/msolo_simulator.py
 src/vipersci/carto/nirvss_simulator.py
 src/vipersci/carto/nss_modeler.py
 src/vipersci/carto/nss_simulator.py
 src/vipersci/carto/traverse_interpolator.py
 src/vipersci/carto/tri2gpkg.py
+src/vipersci/carto/pds/__init__.py
+src/vipersci/carto/pds/data/__init__.py
 src/vipersci/pds/__init__.py
 src/vipersci/pds/datetime.py
 src/vipersci/pds/pid.py
 src/vipersci/pds/xml.py
 src/vipersci/vis/__init__.py
 src/vipersci/vis/header.py
 src/vipersci/vis/image_statistics.py
+src/vipersci/vis/viseer.py
 src/vipersci/vis/db/__init__.py
 src/vipersci/vis/db/create_vis_dbs.py
+src/vipersci/vis/db/lights.py
+src/vipersci/vis/db/pano_products.py
 src/vipersci/vis/db/raw_products.py
 src/vipersci/vis/db/raw_stats.py
+src/vipersci/vis/db/validators.py
 src/vipersci/vis/pds/__init__.py
+src/vipersci/vis/pds/create_pano.py
 src/vipersci/vis/pds/create_raw.py
 src/vipersci/vis/pds/create_raw_tif.py
 src/vipersci/vis/pds/template_test.py
 src/vipersci/vis/pds/data/__init__.py
 tests/test_area_bin.py
+tests/test_colorforge.py
+tests/test_create_pano.py
 tests/test_create_raw.py
 tests/test_datetime.py
 tests/test_density_heatmap.py
 tests/test_dotmap.py
 tests/test_heatmap_helpers.py
 tests/test_image_statistics.py
+tests/test_lights.py
 tests/test_msolo.py
 tests/test_msolo_simulator.py
 tests/test_nirvss.py
 tests/test_nirvss_simulator.py
 tests/test_nss.py
 tests/test_nss_modeler.py
 tests/test_nss_simulator.py
+tests/test_pano_products.py
 tests/test_pid.py
 tests/test_raw_products.py
 tests/test_raw_stats.py
-tests/test_util.py
+tests/test_util.py
+tests/test_validators.py
```

### Comparing `vipersci-0.4.0/src/vipersci.egg-info/entry_points.txt` & `vipersci-0.5.0/src/vipersci.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [console_scripts]
 accrual = vipersci.carto.accrual:main
+colorforge = vipersci.carto.colorforge:main
 create_vis_dbs = vipersci.vis.db.create_vis_dbs:main
 dice_buffer = vipersci.carto.dice_buffer:main
 dissolve_dice = vipersci.carto.dissolve_dice:main
 image_stats = vipersci.vis.image_statistics:main
 msolo_simulator = vipersci.carto.msolo_simulator:main
 nirvss_simulator = vipersci.carto.nirvss_simulator:main
 nss_modeler = vipersci.carto.nss_modeler:main
 nss_simulator = vipersci.carto.nss_simulator:main
 template_test = vipersci.vis.pds.template_test:main
 traverse_interpolator = vipersci.carto.traverse_interpolator:main
 tri2gpkg = vipersci.carto.tri2gpkg:main
+vis_create_pano = vipersci.vis.pds.create_pano:main
 vis_create_raw = vipersci.vis.pds.create_raw:main
 vis_create_raw_tif = vipersci.vis.pds.create_raw_tif:main
+viseer = vipersci.vis.viseer:main
```

### Comparing `vipersci-0.4.0/tests/test_area_bin.py` & `vipersci-0.5.0/tests/test_area_bin.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_create_raw.py` & `vipersci-0.5.0/tests/test_create_raw.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_datetime.py` & `vipersci-0.5.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_density_heatmap.py` & `vipersci-0.5.0/tests/test_density_heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # top level of this library.
 
 import math
 from typing import Tuple
 import unittest
 
 import numpy as np
+import numpy.testing as npt
 from rasterio import transform, windows
 import shapely
 
 from vipersci.carto import heatmap as hm
 
 
 class TestDensityHeatmap(unittest.TestCase):
@@ -248,7 +249,15 @@
             expected_bounds,
             windows.bounds(windows.get_data_window(out_avg), affine_transform),
         )
 
         expected_frequencies = np.full((2, 2), shape[0] * shape[1])
 
         self.assertTrue(np.array_equal(expected_frequencies, frequencies))
+
+    def test_missing_value(self):
+        t, counts, avg, freqs = hm.generate_density_heatmap(
+            (1, 2, 3), (1, 2, 3), (1, np.nan, 1), 1, 1
+        )
+        npt.assert_array_equal(
+            counts, np.array([[0, 0, 1, 1], [0, 0, 1, 1], [1, 1, 0, 0], [1, 1, 0, 0]])
+        )
```

### Comparing `vipersci-0.4.0/tests/test_dotmap.py` & `vipersci-0.5.0/tests/test_dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_heatmap_helpers.py` & `vipersci-0.5.0/tests/test_heatmap_helpers.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_image_statistics.py` & `vipersci-0.5.0/tests/test_image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_msolo.py` & `vipersci-0.5.0/tests/test_msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_msolo_simulator.py` & `vipersci-0.5.0/tests/test_msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_nirvss.py` & `vipersci-0.5.0/tests/test_nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_nirvss_simulator.py` & `vipersci-0.5.0/tests/test_nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_nss.py` & `vipersci-0.5.0/tests/test_nss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_nss_modeler.py` & `vipersci-0.5.0/tests/test_nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_nss_simulator.py` & `vipersci-0.5.0/tests/test_nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_pid.py` & `vipersci-0.5.0/tests/test_pid.py`

 * *Files 14% similar despite different names*

```diff
@@ -113,14 +113,19 @@
         self.assertRaises(IndexError, pid.VIPERID)
 
     def test_repr(self):
         s = "This is a VIPER ID: 220117-010101-ncl"
         p = pid.VIPERID(s)
         self.assertEqual("VIPERID('220117-010101-ncl')", repr(p))
 
+    def test_str_(self):
+        test = "This is a VIPER Id: 220117-010101-aim"
+        truth = "220117-010101-aim"
+        self.assertEqual(truth, pid.VIPERID(test).__str__())
+
     def test_lt(self):
         p1 = pid.VIPERID("231120-010101-acl")
         p2 = pid.VIPERID("231121-010101-acl")
         p3 = pid.VIPERID("231121-010102-acl")
         p4 = pid.VIPERID("231121-010102-ncl")
         self.assertTrue(p1 < p2)
         self.assertTrue(p2 < p3)
@@ -138,14 +143,18 @@
     def test_init_tuple(self):
         tuples = (
             (
                 ("220117", "010101", "ncl", "a"),
                 (datetime.date(2022, 1, 17), datetime.time(1, 1, 1), "ncl", "a"),
             ),
             (
+                ("220117", "010101", "ncl", "a"),
+                (datetime.date(2022, 1, 17), datetime.time(1, 1, 1), 0, "a"),
+            ),
+            (
                 ("220117", "010101", "ncl", "b"),
                 (datetime.date(2022, 1, 17), datetime.time(1, 1, 1), "ncl", 5),
             ),
             (
                 ("240330", "121212", "hap", "d"),
                 (datetime.date(2024, 3, 30), datetime.time(12, 12, 12), "hap", "d"),
             ),
@@ -178,24 +187,24 @@
         d = dict(
             lobt=1643241600, instrument_name="NavCam Left", onboard_compression_ratio=5
         )
         vid = pid.VISID(d)
         self.assertEqual("220127-000000-ncl-b", str(vid))
 
     def test_init_bad_tuples(self):
-        tuples = ((datetime.date(2024, 1, 1), datetime.time(1, 1, 1), "ncl", "z"),)
+        tuples = ((datetime.date(2024, 1, 1), datetime.time(1, 1, 1), "ncl", "w"),)
         for t in tuples:
             with self.subTest(test=t):
                 self.assertRaises(ValueError, pid.VISID, *t)
 
     def test_init_bad_strings(self):
         strings = (
             "220117-010101-ncl",
             "220117-010101-aaa-a",
-            "220117-010101-ncl-z",
+            "220117-010101-ncl-q",
             "foobar",
         )
         for s in strings:
             with self.subTest(test=s):
                 self.assertRaises(ValueError, pid.VISID, s)
 
     def test_init_bad_dict(self):
@@ -245,12 +254,76 @@
         self.assertTrue(vid2 < vid3)
         self.assertTrue(vid3 < vid4)
 
         vids = [vid3, vid4, vid1, vid2]
         self.assertEqual(sorted(vids), [vid1, vid2, vid3, vid4])
 
 
-class TestStrings(unittest.TestCase):
+class TestPanoID(unittest.TestCase):
+    def test_init_tuple(self):
+        tuples = (
+            (
+                ("220117", "010101", "ncl"),
+                (datetime.date(2022, 1, 17), datetime.time(1, 1, 1), "ncl"),
+            ),
+            (
+                ("220117", "010101", "ncl"),
+                (datetime.date(2022, 1, 17), datetime.time(1, 1, 1), "NavCam Left"),
+            ),
+            (
+                ("231225", "182000", "acr"),
+                (datetime.date(2023, 12, 25), datetime.time(18, 20, 0), "acr"),
+            ),
+            (
+                ("240330", "121212", "hap"),
+                (datetime.datetime(2024, 3, 30, 12, 12, 12), "hap"),
+            ),
+        )
+        for truth, t in tuples:
+            with self.subTest():
+                p = pid.PanoID(*t)
+                self.assertTupleEqual(truth, (p.date, p.time, p.instrument))
+
+    def test_init_string(self):
+        string_tuples = (
+            ("220117-010101-ncl-pan", "220117-010101-ncl-pano"),
+            ("220117-010101-ncl-pan", "220117-010101-NCL-PAN"),
+            ("220117-010101-ncl-pan", "20220117-010101-ncl-pano"),
+            ("231225-182000-acr-pan", "231225-182000-acr-pan ignored"),
+            ("231225-182000-pan", "231225-182000-pan multiple instruments"),
+        )
+        for s in string_tuples:
+            with self.subTest():
+                p = pid.PanoID(s[1])
+                self.assertEqual(s[0], str(p))
+
+    def test_init_bad_tuples(self):
+        tuples = (
+            ("not a datetime", "ncl"),
+            ("not a date", datetime.time(1, 1, 1), "ncl"),
+            ("220117", "010101001", "aim"),
+            (datetime.date(2024, 1, 1), "not a time", "ncl"),
+            (datetime.datetime(2022, 1, 17, 1, 1, 1), "not an instrument"),
+        )
+        for t in tuples:
+            with self.subTest(t):
+                self.assertRaises(ValueError, pid.PanoID, *t)
+
+    def test_init_bad_strings(self):
+        strings = (
+            "220117-010101-ncl",
+            "220117-10101-ncl",
+            "foobar",
+        )
+        for s in strings:
+            with self.subTest(s):
+                self.assertRaises(ValueError, pid.PanoID, s)
+
+    def test_repr(self):
+        s = "This is a Pano ID: 220117-010101-ncl-pan"
+        p = pid.PanoID(s)
+        self.assertEqual("PanoID('220117-010101-ncl-pan')", repr(p))
+
     def test_str_(self):
-        test = "This is a VIPER Id: 220117-010101-aim"
-        truth = "220117-010101-aim"
-        self.assertEqual(truth, pid.VIPERID(test).__str__())
+        test = "This is a Pano Id: 220117-010101-ncr-pan"
+        truth = "220117-010101-ncr-pan"
+        self.assertEqual(truth, pid.PanoID(test).__str__())
```

### Comparing `vipersci-0.4.0/tests/test_raw_products.py` & `vipersci-0.5.0/tests/test_raw_products.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,40 @@
 
 from datetime import datetime, timedelta, timezone
 import unittest
 
 from vipersci.vis.db import raw_products as trp
 
 
+class TestImageType(unittest.TestCase):
+    def test_init(self):
+        self.assertEqual(trp.ImageType.LOSSLESS_ICER_IMAGE, trp.ImageType(1))
+
+    def test_single_flags(self):
+        self.assertRaises(ValueError, trp.ImageType, 9)
+
+    def test_not_member(self):
+        self.assertRaises(ValueError, trp.ImageType, 1000)
+
+
+class TestProcessingStage(unittest.TestCase):
+    def test_init(self):
+        self.assertEqual(trp.ProcessingStage.PROCESS_FLATFIELD, trp.ProcessingStage(2))
+
+    def test_combintation(self):
+        self.assertEqual(
+            trp.ProcessingStage.PROCESS_FLATFIELD
+            | trp.ProcessingStage.PROCESS_LINEARIZATION,
+            trp.ProcessingStage(10),
+        )
+
+    def test_not_member(self):
+        self.assertRaises(ValueError, trp.ProcessingStage, 15)
+
+
 class TestRawProduct(unittest.TestCase):
     def setUp(self):
         self.startUTC = datetime(2022, 1, 27, 0, 0, 0, tzinfo=timezone.utc)
         self.d = dict(
             adc_gain=63,
             auto_exposure=False,
             bad_pixel_table_id=0,
@@ -47,23 +73,22 @@
             hazlight_fore_port_on=False,
             hazlight_fore_starboard_on=False,
             image_id=0,
             instrument_name="NavCam Left",
             instrument_temperature=128,
             lines=2048,
             lobt=self.startUTC.timestamp(),
-            mcam_id=1,
             md5_checksum="dummychecksum",
             mission_phase="Test",
             navlight_left_on=False,
             navlight_right_on=False,
             offset=16324,
             onboard_compression_ratio=5,
             onboard_compression_type="ICER",
-            output_image_mask=0,
+            output_image_mask=8,
             output_image_type="?",
             padding=0,
             pga_gain=0,
             processing_info=0,
             purpose="Engineering",
             samples=2048,
             slog=False,
@@ -105,14 +130,18 @@
         self.assertRaises(ValueError, trp.RawProduct, **d)
 
         d = self.d.copy()
         d["product_id"] = "220127-000000-ncl-b"
         d["onboard_compression_ratio"] = 999
         self.assertRaises(ValueError, trp.RawProduct, **d)
 
+        d = self.d.copy()
+        d["cameraId"] = 1
+        self.assertWarns(UserWarning, trp.RawProduct, **d)
+
     # Commented out while this exception has been converted to a warning until we
     # sort out the Yamcs parameter.
     # def test_mcam_id(self):
     #     rp = trp.RawProduct(**self.d)
     #     self.assertRaises(ValueError, setattr, rp, "mcam_id", 5)
 
     def test_product_id(self):
```

### Comparing `vipersci-0.4.0/tests/test_raw_stats.py` & `vipersci-0.5.0/tests/test_raw_stats.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.4.0/tests/test_util.py` & `vipersci-0.5.0/tests/test_util.py`

 * *Files identical despite different names*

