# Comparing `tmp/oceantide-0.4.1.tar.gz` & `tmp/oceantide-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceantide-0.4.1.tar", last modified: Tue Aug 16 22:20:41 2022, max compression
+gzip compressed data, was "oceantide-0.5.0.tar", last modified: Wed Jul 26 10:50:16 2023, max compression
```

## Comparing `oceantide-0.4.1.tar` & `oceantide-0.5.0.tar`

### file list

```diff
@@ -1,167 +1,166 @@
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      292 2022-03-21 03:02:56.000000 oceantide-0.4.1/.editorconfig
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1290 2022-08-03 16:57:50.000000 oceantide-0.4.1/.gitignore
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      298 2022-03-21 03:02:56.000000 oceantide-0.4.1/.travis.yml
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.153435 oceantide-0.4.1/.vscode/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      453 2022-03-21 03:02:56.000000 oceantide-0.4.1/.vscode/launch.json
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      170 2022-03-21 03:02:56.000000 oceantide-0.4.1/AUTHORS.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3530 2022-03-21 03:02:56.000000 oceantide-0.4.1/CONTRIBUTING.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       89 2022-03-21 03:02:56.000000 oceantide-0.4.1/HISTORY.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      301 2022-03-21 03:02:56.000000 oceantide-0.4.1/MANIFEST.in
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2253 2022-03-21 03:02:56.000000 oceantide-0.4.1/Makefile
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      970 2022-08-16 22:20:41.177435 oceantide-0.4.1/PKG-INFO
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       59 2022-08-03 16:57:50.000000 oceantide-0.4.1/README.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.157435 oceantide-0.4.1/docs/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      610 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/Makefile
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.145435 oceantide-0.4.1/docs/_build/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.145435 oceantide-0.4.1/docs/_build/html/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.157435 oceantide-0.4.1/docs/_build/html/_static/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21404 2021-08-15 10:12:55.000000 oceantide-0.4.1/docs/_build/html/_static/broken_example.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      286 2020-10-22 03:39:04.000000 oceantide-0.4.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2020-10-22 03:39:04.000000 oceantide-0.4.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4315 2021-08-15 10:12:55.000000 oceantide-0.4.1/docs/_build/html/_static/no_image.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       90 2020-10-22 03:39:04.000000 oceantide-0.4.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       28 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/authors.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.157435 oceantide-0.4.1/docs/auto_gallery/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      725 2022-08-11 20:45:56.000000 oceantide-0.4.1/docs/auto_gallery/index.rst
--rwxrwxr-x   0 rguedes   (1000) rguedes   (1000)     5537 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/conf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       33 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/contributing.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.157435 oceantide-0.4.1/docs/gallery/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       30 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/gallery/README.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       28 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/history.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      306 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/index.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1126 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/installation.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      771 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/make.bat
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       64 2022-08-11 20:45:54.000000 oceantide-0.4.1/docs/modules.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      483 2022-08-11 20:45:54.000000 oceantide-0.4.1/docs/oceantide.core.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      891 2022-08-11 20:45:54.000000 oceantide-0.4.1/docs/oceantide.input.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      711 2022-08-11 20:45:54.000000 oceantide-0.4.1/docs/oceantide.output.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      840 2022-08-11 20:45:54.000000 oceantide-0.4.1/docs/oceantide.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       27 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/readme.rst
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       73 2022-03-21 03:02:56.000000 oceantide-0.4.1/docs/usage.rst
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.157435 oceantide-0.4.1/oceantide/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1176 2022-08-16 22:19:55.000000 oceantide-0.4.1/oceantide/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      309 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/cli.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1022 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/constituents.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.161435 oceantide-0.4.1/oceantide/core/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/core/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6155 2022-08-03 16:57:50.000000 oceantide-0.4.1/oceantide/core/attributes.yml
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    25147 2022-08-15 14:24:06.000000 oceantide-0.4.1/oceantide/core/otis.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6282 2022-08-03 16:57:50.000000 oceantide-0.4.1/oceantide/core/utils.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21345 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/ellipse.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.161435 oceantide-0.4.1/oceantide/input/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/input/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1205 2022-08-03 16:57:50.000000 oceantide-0.4.1/oceantide/input/oceantide.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5803 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/input/otis_atlas_netcdf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2229 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/input/otis_binary.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1927 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/input/otis_netcdf.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.161435 oceantide-0.4.1/oceantide/output/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-03-21 03:02:56.000000 oceantide-0.4.1/oceantide/output/__init__.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3117 2022-08-03 16:57:50.000000 oceantide-0.4.1/oceantide/output/oceantide.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2569 2022-08-15 18:21:53.000000 oceantide-0.4.1/oceantide/output/otis_binary.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6833 2022-08-15 18:21:43.000000 oceantide-0.4.1/oceantide/output/otis_netcdf.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6676 2022-08-16 14:03:09.000000 oceantide-0.4.1/oceantide/tide.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.161435 oceantide-0.4.1/oceantide.egg-info/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      970 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/PKG-INFO
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     4216 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/SOURCES.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/dependency_links.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       50 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/entry_points.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        1 2022-08-03 17:06:24.000000 oceantide-0.4.1/oceantide.egg-info/not-zip-safe
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       49 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/requires.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       10 2022-08-16 22:20:41.000000 oceantide-0.4.1/oceantide.egg-info/top_level.txt
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      421 2022-08-16 22:20:41.177435 oceantide-0.4.1/setup.cfg
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1438 2022-08-04 18:59:06.000000 oceantide-0.4.1/setup.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      520 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_cli.py
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/test_files/
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/test_files/dataset.zarr/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       42 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/.zgroup
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5419 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/.zmetadata
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/test_files/dataset.zarr/con/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      312 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/con/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/con/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       40 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/con/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/test_files/dataset.zarr/dep/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/dep/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/dep/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1023 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/dep/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.165435 oceantide-0.4.1/tests/test_files/dataset.zarr/h/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/h/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      156 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/h/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10074 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/h/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.169435 oceantide-0.4.1/tests/test_files/dataset.zarr/lat/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lat/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lat/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      168 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lat/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.169435 oceantide-0.4.1/tests/test_files/dataset.zarr/lon/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lon/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lon/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      272 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/lon/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.169435 oceantide-0.4.1/tests/test_files/dataset.zarr/u/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/u/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      158 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/u/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10581 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/u/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.169435 oceantide-0.4.1/tests/test_files/dataset.zarr/v/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/v/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      158 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/v/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10519 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/dataset.zarr/v/0.0.0
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    51858 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.nc
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.169435 oceantide-0.4.1/tests/test_files/oceantide.zarr/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       42 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/.zgroup
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10256 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/.zmetadata
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/con/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      312 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/con/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/con/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       40 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/con/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      538 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      907 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      224 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2305 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      224 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2356 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/lat/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lat/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lat/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      168 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lat/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/lon/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lon/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lon/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      272 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/lon/0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.173435 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      244 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2301 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      244 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2237 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      246 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2307 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/.zarray
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      246 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/.zattrs
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2282 2022-08-03 16:57:50.000000 oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/0.0.0
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/tests/test_files/otis_binary/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       21 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_binary/Model_rag
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1168 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_binary/grid_rag
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     8208 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_binary/h_rag
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    16272 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_binary/u_rag
-drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2022-08-16 22:20:41.177435 oceantide-0.4.1/tests/test_files/otis_netcdf/
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       34 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_netcdf/Model_test
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    71624 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_netcdf/grid.test.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    54945 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_netcdf/hf.test.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69618 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_files/otis_netcdf/uv.test.nc
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2451 2022-08-11 13:59:26.000000 oceantide-0.4.1/tests/test_io.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1881 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_otis.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1071 2022-03-21 03:02:56.000000 oceantide-0.4.1/tests/test_tide.py
--rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      516 2022-08-03 16:57:50.000000 oceantide-0.4.1/tox.ini
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.521696 oceantide-0.5.0/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      292 2022-11-22 02:32:25.000000 oceantide-0.5.0/.editorconfig
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1290 2022-11-22 02:32:25.000000 oceantide-0.5.0/.gitignore
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      298 2022-11-22 02:32:25.000000 oceantide-0.5.0/.travis.yml
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.481695 oceantide-0.5.0/.vscode/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      453 2022-11-22 02:32:25.000000 oceantide-0.5.0/.vscode/launch.json
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      170 2022-11-22 02:32:25.000000 oceantide-0.5.0/AUTHORS.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3530 2022-11-22 02:32:25.000000 oceantide-0.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      336 2023-07-26 10:39:37.000000 oceantide-0.5.0/HISTORY.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1067 2023-07-26 10:15:14.000000 oceantide-0.5.0/LICENSE
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2253 2022-11-22 02:32:25.000000 oceantide-0.5.0/Makefile
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2490 2023-07-26 10:50:16.521696 oceantide-0.5.0/PKG-INFO
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       59 2022-11-22 02:32:25.000000 oceantide-0.5.0/README.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.485695 oceantide-0.5.0/docs/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      610 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/Makefile
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.473694 oceantide-0.5.0/docs/_build/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.473694 oceantide-0.5.0/docs/_build/html/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.485695 oceantide-0.5.0/docs/_build/html/_static/
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)    21404 2021-08-15 10:12:55.000000 oceantide-0.5.0/docs/_build/html/_static/broken_example.png
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      286 2020-10-22 03:39:04.000000 oceantide-0.5.0/docs/_build/html/_static/file.png
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       90 2020-10-22 03:39:04.000000 oceantide-0.5.0/docs/_build/html/_static/minus.png
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)     4315 2021-08-15 10:12:55.000000 oceantide-0.5.0/docs/_build/html/_static/no_image.png
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       90 2020-10-22 03:39:04.000000 oceantide-0.5.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       28 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/authors.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.485695 oceantide-0.5.0/docs/auto_gallery/
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      725 2022-08-11 20:45:56.000000 oceantide-0.5.0/docs/auto_gallery/index.rst
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)     5537 2022-03-21 03:02:56.000000 oceantide-0.5.0/docs/conf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       33 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/contributing.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.485695 oceantide-0.5.0/docs/gallery/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       30 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/gallery/README.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       28 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/history.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      306 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/index.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1126 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/installation.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      771 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/make.bat
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       64 2022-08-11 20:45:54.000000 oceantide-0.5.0/docs/modules.rst
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      483 2022-08-11 20:45:54.000000 oceantide-0.5.0/docs/oceantide.core.rst
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      891 2022-08-11 20:45:54.000000 oceantide-0.5.0/docs/oceantide.input.rst
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      711 2022-08-11 20:45:54.000000 oceantide-0.5.0/docs/oceantide.output.rst
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)      840 2022-08-11 20:45:54.000000 oceantide-0.5.0/docs/oceantide.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       27 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/readme.rst
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       73 2022-11-22 02:32:25.000000 oceantide-0.5.0/docs/usage.rst
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.489695 oceantide-0.5.0/oceantide/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      925 2023-07-26 10:33:24.000000 oceantide-0.5.0/oceantide/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      309 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/cli.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1022 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/constituents.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.489695 oceantide-0.5.0/oceantide/core/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/core/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6155 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/core/attributes.yml
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    25159 2023-07-26 09:44:48.000000 oceantide-0.5.0/oceantide/core/otis.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6282 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/core/utils.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    21345 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/ellipse.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.493695 oceantide-0.5.0/oceantide/input/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/input/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1205 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/input/oceantide.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5803 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/input/otis_atlas_netcdf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2229 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/input/otis_binary.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1927 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/input/otis_netcdf.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.501695 oceantide-0.5.0/oceantide/output/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)        0 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/output/__init__.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     3117 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/output/oceantide.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2574 2022-11-22 02:53:37.000000 oceantide-0.5.0/oceantide/output/otis_binary.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6868 2022-11-22 02:55:15.000000 oceantide-0.5.0/oceantide/output/otis_netcdf.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     6676 2022-11-22 02:32:25.000000 oceantide-0.5.0/oceantide/tide.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.489695 oceantide-0.5.0/oceantide.egg-info/
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)     2490 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/PKG-INFO
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)     4176 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/SOURCES.txt
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)        1 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/dependency_links.txt
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       49 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/entry_points.txt
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       64 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/requires.txt
+-rwxr-xr-x   0 rguedes   (1000) rguedes   (1000)       26 2023-07-26 10:50:16.000000 oceantide-0.5.0/oceantide.egg-info/top_level.txt
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1857 2023-07-26 10:31:18.000000 oceantide-0.5.0/pyproject.toml
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       38 2023-07-26 10:50:16.521696 oceantide-0.5.0/setup.cfg
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.505696 oceantide-0.5.0/tests/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      520 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_cli.py
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.505696 oceantide-0.5.0/tests/test_files/
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.505696 oceantide-0.5.0/tests/test_files/dataset.zarr/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       42 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/.zgroup
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     5419 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/.zmetadata
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.505696 oceantide-0.5.0/tests/test_files/dataset.zarr/con/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      312 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/con/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/con/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       40 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/con/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.505696 oceantide-0.5.0/tests/test_files/dataset.zarr/dep/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      339 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/dep/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/dep/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1023 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/dep/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.509696 oceantide-0.5.0/tests/test_files/dataset.zarr/h/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/h/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      156 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/h/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10074 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/h/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.509696 oceantide-0.5.0/tests/test_files/dataset.zarr/lat/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lat/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lat/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      168 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lat/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.509696 oceantide-0.5.0/tests/test_files/dataset.zarr/lon/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lon/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lon/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      272 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/lon/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.509696 oceantide-0.5.0/tests/test_files/dataset.zarr/u/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/u/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      158 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/u/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10581 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/u/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.509696 oceantide-0.5.0/tests/test_files/dataset.zarr/v/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      360 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/v/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      158 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/v/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10519 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/dataset.zarr/v/0.0.0
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    51858 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.nc
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       42 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       24 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/.zgroup
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    10256 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/.zmetadata
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/con/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      312 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/con/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      109 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/con/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       40 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/con/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      538 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      144 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      907 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      224 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2305 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      224 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2356 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.513696 oceantide-0.5.0/tests/test_files/oceantide.zarr/lat/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lat/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lat/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      168 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lat/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.517696 oceantide-0.5.0/tests/test_files/oceantide.zarr/lon/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      315 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lon/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      113 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lon/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      272 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/lon/0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.517696 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      244 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2301 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.517696 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      244 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2237 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.517696 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      246 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2307 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.517696 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      554 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/.zarray
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      246 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/.zattrs
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2282 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/0.0.0
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.521696 oceantide-0.5.0/tests/test_files/otis_binary/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       21 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_binary/Model_rag
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1168 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_binary/grid_rag
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     8208 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_binary/h_rag
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    16272 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_binary/u_rag
+drwxrwxr-x   0 rguedes   (1000) rguedes   (1000)        0 2023-07-26 10:50:16.521696 oceantide-0.5.0/tests/test_files/otis_netcdf/
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)       34 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_netcdf/Model_test
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    71624 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_netcdf/grid.test.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    54945 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_netcdf/hf.test.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)    69618 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_files/otis_netcdf/uv.test.nc
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     2451 2022-11-22 02:50:18.000000 oceantide-0.5.0/tests/test_io.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1881 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_otis.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)     1071 2022-11-22 02:32:25.000000 oceantide-0.5.0/tests/test_tide.py
+-rw-rw-r--   0 rguedes   (1000) rguedes   (1000)      516 2022-11-22 02:32:25.000000 oceantide-0.5.0/tox.ini
```

### Comparing `oceantide-0.4.1/.gitignore` & `oceantide-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/CONTRIBUTING.rst` & `oceantide-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/Makefile` & `oceantide-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/Makefile` & `oceantide-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/_build/html/_static/broken_example.png` & `oceantide-0.5.0/docs/_build/html/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/_build/html/_static/no_image.png` & `oceantide-0.5.0/docs/_build/html/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/auto_gallery/index.rst` & `oceantide-0.5.0/docs/auto_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/conf.py` & `oceantide-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/installation.rst` & `oceantide-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/make.bat` & `oceantide-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/oceantide.input.rst` & `oceantide-0.5.0/docs/oceantide.input.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/oceantide.output.rst` & `oceantide-0.5.0/docs/oceantide.output.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/docs/oceantide.rst` & `oceantide-0.5.0/docs/oceantide.rst`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/__init__.py` & `oceantide-0.5.0/oceantide/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """Top-level package for oceantide."""
 
-__version__ = "0.4.1"
-__author__ = "Oceanum Developers"
-__contact__ = "developers@oceanum.science"
-__url__ = "http://github.com/wavespectra/oceantide"
-__description__ = "Library for ocean tide prediction"
-__keywords__ = "ocean tide prediction constituents xarray accessor"
+__version__ = "0.5.0"
 
 
 def _import_read_functions(pkgname="input"):
     """Make read functions available at module level.
 
     Functions are imported here if:
         they are defined in a module wavespectra.input.{modname}
```

### Comparing `oceantide-0.4.1/oceantide/constituents.py` & `oceantide-0.5.0/oceantide/constituents.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/core/attributes.yml` & `oceantide-0.5.0/oceantide/core/attributes.yml`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/core/otis.py` & `oceantide-0.5.0/oceantide/core/otis.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     dsl = mz.isel(ny=[0]).stack({"n": ["nx", "ny"]})
     dst = mz.isel(nx=[-1]).stack({"n": ["nx", "ny"]})
     dsr = mz.isel(ny=[-1]).sortby("nx", ascending=False).stack({"n": ["nx", "ny"]})
     dsb = mz.isel(nx=[0]).sortby("ny", ascending=False).stack({"n": ["nx", "ny"]})
 
     # Concatenate boundaries and keep water points
     iob = xr.concat([dsl, dst, dsr, dsb], dim="n")
-    iob = iob.where(iob == 1, drop=True)
+    iob = iob.where((iob == 1).compute(), drop=True)
 
     return np.array([iob.nx.values, iob.ny.values], dtype=INT)
 
 
 def u_from_z(dz, mz=None, mu=None):
     """Interpolate data from Z-nodes onto U-Nodes.
```

### Comparing `oceantide-0.4.1/oceantide/core/utils.py` & `oceantide-0.5.0/oceantide/core/utils.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/ellipse.py` & `oceantide-0.5.0/oceantide/ellipse.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/input/oceantide.py` & `oceantide-0.5.0/oceantide/input/oceantide.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/input/otis_atlas_netcdf.py` & `oceantide-0.5.0/oceantide/input/otis_atlas_netcdf.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/input/otis_binary.py` & `oceantide-0.5.0/oceantide/input/otis_binary.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/input/otis_netcdf.py` & `oceantide-0.5.0/oceantide/input/otis_netcdf.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/output/oceantide.py` & `oceantide-0.5.0/oceantide/output/oceantide.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide/output/otis_binary.py` & `oceantide-0.5.0/oceantide/output/otis_binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         - gfile (bool): Save grid file.
         - suffix (str): Suffix to define file names, by default defined by cons names.
 
     Return:
         - filename (dict): Name of files written.
 
     """
-    ds = self._obj.transpose("con", "lon", "lat")
+    ds = self._obj.transpose("con", "lon", "lat", ...)
     ds = ds.rename({"con": "nc", "lon": "nx", "lat": "ny"})
     ds = ds.fillna(0.0)
 
     if suffix is None:
         suffix = "".join(list(ds.nc.values)).lower()
 
     filenames = {}
```

### Comparing `oceantide-0.4.1/oceantide/output/otis_netcdf.py` & `oceantide-0.5.0/oceantide/output/otis_netcdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         - gfile (bool): Save grid file.
         - suffix (str): Suffix to define file names, by default defined by cons names.
 
     Return:
         - filename (dict): Name of files written.
 
     """
-    ds = self._obj.transpose("con", "lon", "lat")
+    ds = self._obj.transpose("con", "lon", "lat", ...)
     ds = ds.rename({"con": "nc", "lon": "nx", "lat": "ny"})
     ds = ds.fillna(0.0)
 
     if suffix is None:
         suffix = "".join(list(ds.nc.values)).lower()
 
     lat_z, lon_z = np.meshgrid(ds.ny, ds.nx)
@@ -47,17 +47,17 @@
     filenames = {}
 
     # Write elevations
     if hfile:
         fname = f"h_{suffix.lstrip('_')}.nc" if suffix else "h.nc"
         filenames["hfile"] = Path(dirname) / fname
 
-        ha = self.amplitude("h").transpose("con", "lon", "lat")
+        ha = self.amplitude("h").transpose("con", "lon", "lat", ...)
         ha = ha.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
-        hp = self.phase("h").transpose("con", "lon", "lat")
+        hp = self.phase("h").transpose("con", "lon", "lat", ...)
         hp = hp.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
         dsout = xr.Dataset()
         dsout["con"] = xr.DataArray(cons, dims=("nc"))
         dsout["lon_z"] = xr.DataArray(lon_z, dims=("nx", "ny"))
         dsout["lat_z"] = xr.DataArray(lat_z, dims=("nx", "ny"))
         dsout["ha"] = xr.DataArray(ha, dims=("nc", "nx", "ny"))
         dsout["hp"] = xr.DataArray(hp, dims=("nc", "nx", "ny"))
@@ -70,21 +70,21 @@
         dsout.to_netcdf(filenames["hfile"])
 
     # Write transports
     if ufile:
         fname = f"u_{suffix.lstrip('_')}.nc" if suffix else "u.nc"
         filenames["ufile"] = Path(dirname) / fname
 
-        ua = self.amplitude("u").transpose("con", "lon", "lat")
+        ua = self.amplitude("u").transpose("con", "lon", "lat", ...)
         ua = ua.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
-        up = self.phase("u").transpose("con", "lon", "lat")
+        up = self.phase("u").transpose("con", "lon", "lat", ...)
         up = up.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
-        va = self.amplitude("v").transpose("con", "lon", "lat")
+        va = self.amplitude("v").transpose("con", "lon", "lat", ...)
         va = va.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
-        vp = self.phase("v").transpose("con", "lon", "lat")
+        vp = self.phase("v").transpose("con", "lon", "lat", ...)
         vp = vp.rename({"con": "nc", "lon": "nx", "lat": "ny"}).drop(["nc", "nx", "ny"])
         dsout = xr.Dataset()
         dsout["con"] = dsout["con"] = xr.DataArray(cons, dims=("nc"))
         dsout["lon_u"] = xr.DataArray(lon_u, dims=("nx", "ny"))
         dsout["lat_u"] = xr.DataArray(lat_u, dims=("nx", "ny"))
         dsout["lon_v"] = xr.DataArray(lon_v, dims=("nx", "ny"))
         dsout["lat_v"] = xr.DataArray(lat_v, dims=("nx", "ny"))
```

### Comparing `oceantide-0.4.1/oceantide/tide.py` & `oceantide-0.5.0/oceantide/tide.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/oceantide.egg-info/SOURCES.txt` & `oceantide-0.5.0/oceantide.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 .editorconfig
 .gitignore
 .travis.yml
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
-MANIFEST.in
+LICENSE
 Makefile
 README.rst
-setup.cfg
-setup.py
+pyproject.toml
 tox.ini
 .vscode/launch.json
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
@@ -38,15 +37,14 @@
 oceantide/constituents.py
 oceantide/ellipse.py
 oceantide/tide.py
 oceantide.egg-info/PKG-INFO
 oceantide.egg-info/SOURCES.txt
 oceantide.egg-info/dependency_links.txt
 oceantide.egg-info/entry_points.txt
-oceantide.egg-info/not-zip-safe
 oceantide.egg-info/requires.txt
 oceantide.egg-info/top_level.txt
 oceantide/core/__init__.py
 oceantide/core/attributes.yml
 oceantide/core/otis.py
 oceantide/core/utils.py
 oceantide/input/__init__.py
```

### Comparing `oceantide-0.4.1/tests/test_cli.py` & `oceantide-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/dataset.zarr/.zmetadata` & `oceantide-0.5.0/tests/test_files/dataset.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/dataset.zarr/dep/0.0` & `oceantide-0.5.0/tests/test_files/dataset.zarr/dep/0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/dataset.zarr/h/0.0.0` & `oceantide-0.5.0/tests/test_files/dataset.zarr/h/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/dataset.zarr/u/0.0.0` & `oceantide-0.5.0/tests/test_files/dataset.zarr/u/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/dataset.zarr/v/0.0.0` & `oceantide-0.5.0/tests/test_files/dataset.zarr/v/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.nc` & `oceantide-0.5.0/tests/test_files/oceantide.nc`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/.zmetadata` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/dep/0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/dep/0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/h_imag/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/h_imag/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/h_real/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/h_real/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/u_imag/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/u_imag/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/u_real/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/u_real/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/v_imag/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/v_imag/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/.zarray` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/.zarray`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/oceantide.zarr/v_real/0.0.0` & `oceantide-0.5.0/tests/test_files/oceantide.zarr/v_real/0.0.0`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_binary/grid_rag` & `oceantide-0.5.0/tests/test_files/otis_binary/grid_rag`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_binary/h_rag` & `oceantide-0.5.0/tests/test_files/otis_binary/h_rag`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_binary/u_rag` & `oceantide-0.5.0/tests/test_files/otis_binary/u_rag`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_netcdf/grid.test.nc` & `oceantide-0.5.0/tests/test_files/otis_netcdf/grid.test.nc`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_netcdf/hf.test.nc` & `oceantide-0.5.0/tests/test_files/otis_netcdf/hf.test.nc`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_files/otis_netcdf/uv.test.nc` & `oceantide-0.5.0/tests/test_files/otis_netcdf/uv.test.nc`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_io.py` & `oceantide-0.5.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_otis.py` & `oceantide-0.5.0/tests/test_otis.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tests/test_tide.py` & `oceantide-0.5.0/tests/test_tide.py`

 * *Files identical despite different names*

### Comparing `oceantide-0.4.1/tox.ini` & `oceantide-0.5.0/tox.ini`

 * *Files identical despite different names*

