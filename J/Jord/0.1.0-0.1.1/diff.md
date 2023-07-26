# Comparing `tmp/Jord-0.1.0.tar.gz` & `tmp/Jord-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.1.0.tar", last modified: Mon Jun 26 14:05:07 2023, max compression
+gzip compressed data, was "Jord-0.1.1.tar", last modified: Wed Jul 26 11:10:25 2023, max compression
```

## Comparing `Jord-0.1.0.tar` & `Jord-0.1.1.tar`

### file list

```diff
@@ -1,143 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.823305 Jord-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:05:03.000000 Jord-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 14:05:07.000000 Jord-0.1.0/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 14:05:03.000000 Jord-0.1.0/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-26 14:05:03.000000 Jord-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 14:05:03.000000 Jord-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-26 14:05:07.839305 Jord-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 14:05:03.000000 Jord-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 14:05:03.000000 Jord-0.1.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:05:03.000000 Jord-0.1.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/geopandas_utilities/geometry_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.827305 Jord-0.1.0/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/numpy_utilities/rasters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.831305 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.835305 Jord-0.1.0/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/jord/spatialite_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/spatialite_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-26 14:05:03.000000 Jord-0.1.0/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 14:05:03.000000 Jord-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 14:05:03.000000 Jord-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 14:05:07.839305 Jord-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-26 14:05:03.000000 Jord-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:05:07.839305 Jord-0.1.0/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 14:05:03.000000 Jord-0.1.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 11:10:18.000000 Jord-0.1.1/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 11:10:18.000000 Jord-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-26 11:10:18.000000 Jord-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 11:10:25.532286 Jord-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-26 11:10:18.000000 Jord-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-26 11:10:18.000000 Jord-0.1.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:10:18.000000 Jord-0.1.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/geometry_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/plugin_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qlive_utilities/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/spatialite_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/spatialite_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 11:10:18.000000 Jord-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 11:10:18.000000 Jord-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 11:10:25.532286 Jord-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-26 11:10:18.000000 Jord-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/test_sanity.py
```

### Comparing `Jord-0.1.0/.github/CODE_OF_CONDUCT.md` & `Jord-0.1.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/.github/CONTRIBUTING.md` & `Jord-0.1.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/Jord.egg-info/PKG-INFO` & `Jord-0.1.1/Jord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: extra
-Provides-Extra: samples
-Provides-Extra: pil
-Provides-Extra: gdal
 Provides-Extra: dev
+Provides-Extra: gdal
 Provides-Extra: tests
-Provides-Extra: setup
+Provides-Extra: pil
+Provides-Extra: samples
 Provides-Extra: docs
+Provides-Extra: setup
+Provides-Extra: extra
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.1.0 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.1 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
-Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
-Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: dev Provides-Extra: gdal Provides-Extra: tests Provides-Extra:
+pil Provides-Extra: samples Provides-Extra: docs Provides-Extra: setup
+Provides-Extra: extra Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.1.0/Jord.egg-info/SOURCES.txt` & `Jord-0.1.1/Jord.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,27 @@
 jord/gdal_utilities/spatial_reference.py
 jord/geojson_utilities/README.md
 jord/geojson_utilities/__init__.py
 jord/geojson_utilities/geometry_types.py
 jord/geopandas_utilities/README.md
 jord/geopandas_utilities/__init__.py
 jord/geopandas_utilities/geometry_filtering.py
+jord/geopandas_utilities/importing.py
 jord/pillow_utilities/README.md
 jord/pillow_utilities/__init__.py
 jord/pillow_utilities/exif.py
 jord/pillow_utilities/tiff.py
 jord/qgis_utilities/README.md
 jord/qgis_utilities/__init__.py
 jord/qgis_utilities/categorisation.py
 jord/qgis_utilities/data_provider.py
 jord/qgis_utilities/enums.py
 jord/qgis_utilities/geometry_types.py
 jord/qgis_utilities/importing.py
+jord/qgis_utilities/plugin_version.py
 jord/qgis_utilities/styling.py
 jord/qgis_utilities/configuration/README.md
 jord/qgis_utilities/configuration/__init__.py
 jord/qgis_utilities/configuration/plugin_settings.py
 jord/qgis_utilities/configuration/project_settings.py
 jord/qgis_utilities/conversion/README.md
 jord/qgis_utilities/conversion/__init__.py
@@ -78,14 +80,17 @@
 jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
 jord/qlive_utilities/README.md
 jord/qlive_utilities/__init__.py
 jord/qlive_utilities/client.py
 jord/qlive_utilities/procedures.py
 jord/qlive_utilities/serialisation.py
 jord/qlive_utilities/uri_utilities.py
+jord/qlive_utilities/clients/__init__.py
+jord/qlive_utilities/clients/auto.py
+jord/qlive_utilities/clients/interfaced.py
 jord/qt_utilities/__init__.py
 jord/qt_utilities/enums.py
 jord/rasterio_utilities/README.md
 jord/rasterio_utilities/__init__.py
 jord/shapely_utilities/README.md
 jord/shapely_utilities/__init__.py
 jord/shapely_utilities/clamp.py
```

### Comparing `Jord-0.1.0/Jord.egg-info/requires.txt` & `Jord-0.1.1/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 warg>=1.1.6
 apppath>=1.0.2
 sorcery
 pyzmq
 
 [all]
 sphinxcontrib-programoutput
+Pillow
+pip>=22.1.2
+wheel>=0.33.0
 pre-commit>=2.17.0
-apppath>=1.0.2
 sphinx>=4.0.1
-pytest>=4.3.0
-furo
-coveralls>=1.6.0
 pyzmq
-numpy>=1.20.2
-sorcery
-black[jupyter]>=21.5b0
-mock
 pytest>=4.4.1
-pytest-cov>=2.11.1
+apppath>=1.0.2
+coveralls>=1.6.0
+pytest>=4.3.0
+mock
+black[jupyter]>=21.5b0
+sorcery
 twine>=1.13.0
-wheel>=0.33.0
-Pillow
-pip>=22.1.2
+pytest-cov>=2.11.1
+furo
 warg>=1.1.6
+numpy>=1.20.2
 
 [dev]
-pytest>=4.4.1
-furo
-pytest-cov>=2.11.1
 sphinxcontrib-programoutput
-twine>=1.13.0
-pip>=22.1.2
-pre-commit>=2.17.0
-apppath>=1.0.2
+pytest>=4.3.0
+mock
+wheel>=0.33.0
+black[jupyter]>=21.5b0
+furo
 coveralls>=1.6.0
-pyzmq
+pre-commit>=2.17.0
+sphinx>=4.0.1
 warg>=1.1.6
-wheel>=0.33.0
 numpy>=1.20.2
 sorcery
-black[jupyter]>=21.5b0
-sphinx>=4.0.1
-mock
-pytest>=4.3.0
+twine>=1.13.0
+pytest>=4.4.1
+pytest-cov>=2.11.1
+pyzmq
+apppath>=1.0.2
+pip>=22.1.2
 
 [docs]
-sphinx>=4.0.1
-furo
 sphinxcontrib-programoutput
+furo
+sphinx>=4.0.1
 
 [extra]
 
 [gdal]
 
 [pil]
 Pillow
 
 [samples]
 
 [setup]
 
 [tests]
-pytest>=4.4.1
 mock
+pytest>=4.4.1
```

### Comparing `Jord-0.1.0/LICENSE.md` & `Jord-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/PKG-INFO` & `Jord-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: extra
-Provides-Extra: samples
-Provides-Extra: pil
-Provides-Extra: gdal
 Provides-Extra: dev
+Provides-Extra: gdal
 Provides-Extra: tests
-Provides-Extra: setup
+Provides-Extra: pil
+Provides-Extra: samples
 Provides-Extra: docs
+Provides-Extra: setup
+Provides-Extra: extra
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.1.0 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.1 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
-Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
-Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: dev Provides-Extra: gdal Provides-Extra: tests Provides-Extra:
+pil Provides-Extra: samples Provides-Extra: docs Provides-Extra: setup
+Provides-Extra: extra Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.1.0/README.md` & `Jord-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/SECURITY.md` & `Jord-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/__init__.py` & `Jord-0.1.1/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pkg_resources
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
```

### Comparing `Jord-0.1.0/jord/gdal_utilities/__init__.py` & `Jord-0.1.1/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/gdal_utilities/cloning.py` & `Jord-0.1.1/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/gdal_utilities/context.py` & `Jord-0.1.1/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/gdal_utilities/conversion.py` & `Jord-0.1.1/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/gdal_utilities/importing.py` & `Jord-0.1.1/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/gdal_utilities/persistence.py` & `Jord-0.1.1/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/geojson_utilities/geometry_types.py` & `Jord-0.1.1/jord/geojson_utilities/geometry_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,7 +28,11 @@
     multi_point = MultiPoint  #
 
     multi_line_string = MultiLineString  #
 
     multi_polygon = MultiPolygon  #
 
     geometry_collection = GeometryCollection  #
+
+
+if __name__ == "__main__":
+    print(GeoJsonGeometryTypesEnum.geometry_collection.value.__name__)
```

### Comparing `Jord-0.1.0/jord/qgis_utilities/__init__.py` & `Jord-0.1.1/jord/qgis_utilities/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,11 +20,12 @@
     from .data_provider import *
     from .geometry_types import *
     from .shapely_utilities import *
     from .qlive_utilities import *
     from .conversion import *
     from .categorisation import *
     from .styling import *
+    from .plugin_version import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     print(f"Make sure qgis module is available for {this_package_name}")
     raise ix
```

### Comparing `Jord-0.1.0/jord/qgis_utilities/categorisation.py` & `Jord-0.1.1/jord/qgis_utilities/categorisation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 import random
 from itertools import cycle
-from typing import Any, Iterable, Sized
+from typing import Iterable, Sized, Callable, Generator
 
 from PyQt5.Qt import QColor
 from qgis.core import (
     QgsVectorLayer,
     QgsSymbol,
     QgsRendererCategory,
     QgsCategorizedSymbolRenderer,
 )
-from warg import TripleNumber
+from warg import TripleNumber, QuadNumber, n_uint_mix_generator_builder
 
 __all__ = ["categorise_layer"]
 
 
 def random_rgb(mix: TripleNumber = (255, 255, 255)) -> TripleNumber:
     red = random.randrange(0, mix[0])
     green = random.randrange(0, mix[1])
     blue = random.randrange(0, mix[2])
     return (red, green, blue)
 
 
-def random_rgba(mix: TripleNumber = (1, 1, 1, 1)) -> TripleNumber:
+def random_rgba(mix: QuadNumber = (1, 1, 1, 1)) -> QuadNumber:
     red = random.randrange(0, mix[0])
     green = random.randrange(0, mix[1])
     blue = random.randrange(0, mix[2])
     alpha = random.randrange(0, mix[3])
     return (red, green, blue, alpha)
 
 
-def random_color_generator() -> Any:
+def random_color_generator() -> TripleNumber:
     while 1:
         yield random_rgb()
 
 
+def random_color_alpha_generator() -> QuadNumber:
+    while 1:
+        yield random_rgba()
+
+
 def categorise_layer(
     layer: QgsVectorLayer,
     field_name: str = "layer",
-    iterable: Iterable = random_color_generator,
+    iterable: Iterable = n_uint_mix_generator_builder(255, 255, 255, 255),
 ) -> None:
     if isinstance(iterable, Sized):
         iterable = cycle(iterable)
-    color_iter = iter(iterable())
+    if isinstance(iterable, Callable) and not isinstance(iterable, Generator):
+        iterable = iterable()  # Compat
+    color_iter = iter(iterable)
 
     render_categories = []
     for cat in layer.uniqueValues(layer.fields().indexFromName(field_name)):
         sym = QgsSymbol.defaultSymbol(layer.geometryType())
-        sym.setColor(QColor(*(next(color_iter)), 255))
+        col = next(color_iter)
+        if len(col) == 3:
+            col = (*col, 255)
+        sym.setColor(QColor(*col))
+        label = str(cat)
         render_categories.append(
-            QgsRendererCategory(cat, symbol=sym, label=cat, render=True)
+            QgsRendererCategory(cat, symbol=sym, label=label, render=True)
         )
 
     layer.setRenderer(QgsCategorizedSymbolRenderer(field_name, render_categories))
     layer.triggerRepaint()
```

### Comparing `Jord-0.1.0/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.1.1/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.1.1/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/enums.py` & `Jord-0.1.1/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/geometry_types.py` & `Jord-0.1.1/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/actions.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/environment.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/models.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/signals.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.1.1/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py` & `Jord-0.1.1/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qgis_utilities/styling.py` & `Jord-0.1.1/jord/qgis_utilities/styling.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,18 @@
     style_mapping = style_mapping_field_dict[field_name]
 
     render_categories = []
     for cat in layer.uniqueValues(layer.fields().indexFromName(field_name)):
         cat_color = default_color
         cat_opacity = default_opacity
         cat_width = default_width
+        label = str(cat)
 
         if cat in style_mapping.keys():
-            style = style_mapping[cat]
+            style = style_mapping[label]
             if "color" in style:
                 cat_color = (
                     int(n) for n in style["color"]
                 )  #  TODO: also support with AlphaChannel | Qt.GlobalColor | QGradient
             if "opacity" in style:
                 cat_opacity = max(0.0, min(float(style["opacity"]), 1.0))
             if "width" in style:
@@ -52,12 +53,12 @@
 
         if isinstance(symbol, QgsLineSymbol):
             symbol.setWidth(cat_width)
         else:
             print(f"width ignored, symbol is of type: {type(symbol)}")
 
         render_categories.append(
-            QgsRendererCategory(cat, symbol=symbol, label=cat, render=True)
+            QgsRendererCategory(cat, symbol=symbol, label=label, render=True)
         )
 
     layer.setRenderer(QgsCategorizedSymbolRenderer(field_name, render_categories))
     layer.triggerRepaint()
```

### Comparing `Jord-0.1.0/jord/qlive_utilities/procedures.py` & `Jord-0.1.1/jord/qlive_utilities/procedures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import time
 from enum import Enum
 
-__all__ = ["QliveRPCMethodEnum", "QliveRPCMethodMap"]
-
 from typing import Mapping, Any, Tuple, Optional
 
-import geopandas.geodataframe
+
 import numpy
 import shapely.geometry.base
 from warg import passes_kws_to, Number
+from jord.geojson_utilities import GeoJsonGeometryTypesEnum
 from pandas import DataFrame
 from shapely.geometry.base import BaseGeometry
-from jord.geopandas_utilities import split_on_geom_type
+from shapely.geometry import GeometryCollection
+
 
 APPEND_TIMESTAMP = True
 SKIP_MEMORY_LAYER_CHECK_AT_CLOSE = True
 PIXEL_SIZE = 1
 DEFAULT_NUMBER = 0
 CONTRAST_ENHANCE = True
 DEFAULT_LAYER_NAME = "TemporaryLayer"
@@ -27,29 +27,31 @@
     "add_raster",
     "add_wkb",
     "add_wkts",
     "add_wkbs",
     "add_rasters",
     "add_wkt",
     "add_dataframe",
-    "add_geom_layer",
+    "add_geojson",
     "clear_all",
     "remove_layers",
+    "QliveRPCMethodEnum",
+    "QliveRPCMethodMap",
 ]
 
 
 def add_raster(
     qgis_instance_handle: Any,
     raster: numpy.ndarray,
     name: str = DEFAULT_LAYER_NAME,
     centroid: Tuple[Number, Number] = None,
     extent_tuple: Tuple[Number, Number, Number, Number] = None,
     pixel_size: Tuple[Number, Number] = PIXEL_SIZE,
     crs_str: str = DEFAULT_LAYER_CRS,
-    default_value=DEFAULT_NUMBER,
+    default_value: Number = DEFAULT_NUMBER,
     field: str = None,
 ) -> None:
     """
 
     :param qgis_instance_handle:
     :param raster:
     :param name:
@@ -221,56 +223,61 @@
     :param kwargs:
     :return:
     """
     for layer_name, raster in rasters.items():
         add_raster(qgis_instance_handle, raster, name=layer_name, **kwargs)
 
 
-def add_geom_layer(
+def add_geometries(qgis_instance_handle: Any):
+    ...
+
+
+def add_geometry(
     qgis_instance_handle: Any,
-    geom: BaseGeometry,
+    geom,  #: QgsGeometry,
     name: Optional[str] = None,
     crs: Optional[str] = None,
     fields: Mapping = None,
     index: bool = False,
     categorise_by_attribute: Optional[str] = None,
 ) -> None:
     """
 
     An example url is “Point?crs=epsg:4326&field=id:integer&field=name:string(20)&index=yes”
 
-      :param fields: Field=name:type(length,precision) Defines an attribute of the layer. Multiple field parameters can be added to the data provider definition. Type is one of “integer”, “double”, “string”.
-      :param index:     index=yes Specifies that the layer will be constructed with a spatial index
-      :param qgis_instance_handle:
-      :param geom:
-      :param name:
-      :param crs: Crs=definition Defines the coordinate reference system to use for the layer. Definition is any string accepted by QgsCoordinateReferenceSystem.createFromString()
-      :return: None
-      :rtype: None
+    :param fields: Field=name:type(length,precision) Defines an attribute of the layer. Multiple field parameters can be added to the data provider definition. Type is one of “integer”, “double”, “string”.
+    :param index:     index=yes Specifies that the layer will be constructed with a spatial index
+    :param qgis_instance_handle:
+    :param geom:
+    :param name:
+    :param crs: Crs=definition Defines the coordinate reference system to use for the layer. Definition is any string accepted by QgsCoordinateReferenceSystem.createFromString()
+    :return: None
+    :rtype: None
     """
 
     from qgis.core import QgsVectorLayer, QgsFeature
 
     # uri = geom.type()
     # uri = geom.wkbType()
     # uri = geom.wktTypeStr()
 
-    uri = json.loads(geom.asJson())["type"]
+    geom_type = json.loads(geom.asJson())["type"]
+    uri = geom_type
 
     if name is None:
         name = DEFAULT_LAYER_NAME
 
     if crs is None:
         crs = DEFAULT_LAYER_CRS
 
     layer_name = f"{name}"
     if APPEND_TIMESTAMP:
         layer_name += f"_{time.time()}"
 
-    if uri == "GeometryCollection":
+    if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
         gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
 
         for g in geom.asGeometryCollection():  # TODO: Look into recursion?
             uri = json.loads(g.asJson())["type"]
             sub_type = uri
 
             if crs:
@@ -289,14 +296,57 @@
             sub_layer.dataProvider().addFeatures([feat])
 
             if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
                 sub_layer.setCustomProperty("skipMemoryLayersCheck", 1)
 
             qgis_instance_handle.qgis_project.addMapLayer(sub_layer, False)
             gm_group.insertLayer(0, sub_layer)
+    elif geom_type == GeoJsonGeometryTypesEnum.multi_point.value.__name__:
+        ...
+    elif geom_type == GeoJsonGeometryTypesEnum.multi_line_string.value.__name__:
+        ...
+    elif geom_type == "CurvePolygon":
+        ...
+    elif geom_type == "MultiSurface":
+        ...
+    elif geom_type == "CompoundCurve":
+        ...
+    elif geom_type == "MultiCurve":
+        ...
+    elif geom_type == GeoJsonGeometryTypesEnum.multi_polygon.value.__name__:
+        gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
+
+        g = geom
+        uri = json.loads(g.asJson())["type"]
+        sub_type = uri
+
+        if crs:
+            uri += f"?crs={crs}"
+
+        if fields:
+            for k, v in fields.items():
+                uri += f"&field={k}:{v}"
+
+        uri += f'&index={"yes" if index else "no"}'
+
+        sub_layer = QgsVectorLayer(uri, f"{layer_name}_{sub_type}", "memory")
+
+        features = []
+        for g_ in [g]:
+            feat = QgsFeature()
+            feat.setGeometry(g)
+            features.append(feat)
+
+        sub_layer.dataProvider().addFeatures(features)
+
+        if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
+            sub_layer.setCustomProperty("skipMemoryLayersCheck", 1)
+
+        qgis_instance_handle.qgis_project.addMapLayer(sub_layer, False)
+        gm_group.insertLayer(0, sub_layer)
     else:
         if crs:
             uri += f"?crs={crs}"
 
         if fields:
             for k, v in fields.items():
                 uri += f"&field={k}:{v}"
@@ -312,40 +362,40 @@
         if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
             layer.setCustomProperty("skipMemoryLayersCheck", 1)
 
         qgis_instance_handle.qgis_project.addMapLayer(layer, False)
         qgis_instance_handle.temporary_group.insertLayer(0, layer)
 
 
-@passes_kws_to(add_geom_layer)
+@passes_kws_to(add_geometry)
 def add_wkb(qgis_instance_handle: Any, wkb: str, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkb:
     :param kwargs:
     :return:
     """
     from qgis.core import QgsGeometry
 
-    add_geom_layer(qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs)
+    add_geometry(qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs)
 
 
-@passes_kws_to(add_geom_layer)
+@passes_kws_to(add_geometry)
 def add_wkt(qgis_instance_handle: Any, wkt: str, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkt:
     :param kwargs:
     :return:
     """
     from qgis.core import QgsGeometry
 
-    add_geom_layer(qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs)
+    add_geometry(qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs)
 
 
 @passes_kws_to(add_wkb)
 def add_wkbs(qgis_instance_handle: Any, wkbs: Mapping, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
@@ -366,73 +416,115 @@
     :param kwargs:
     :return:
     """
     for layer_name, wkt in wkts.items():
         add_wkt(qgis_instance_handle, wkt, name=layer_name, **kwargs)
 
 
-@passes_kws_to(add_geom_layer)
+@passes_kws_to(add_geometry)
 def add_dataframe(qgis_instance_handle: Any, dataframe: DataFrame, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param dataframe:
     :param kwargs:
     :return:
     """
-    if isinstance(dataframe, geopandas.geodataframe.GeoDataFrame):
+    from geopandas import GeoDataFrame
+    from jord.geopandas_utilities import split_on_geom_type
+
+    if isinstance(dataframe, GeoDataFrame):
         columns_to_include = ("layer",)
         geom_dict = split_on_geom_type(dataframe)
         for df in geom_dict.values():
-            add_wkt(qgis_instance_handle, df.to_wkt())
-    elif isinstance(dataframe, DataFrame):
+            if False:
+                for w in df.geometry.to_wkt():
+                    add_wkt(qgis_instance_handle, w)
+            else:
+                for w in df.geometry.to_wkb():
+                    add_wkb(qgis_instance_handle, w)
+
+    elif isinstance(dataframe, DataFrame) and False:
         geometry_column = "geometry"
         if isinstance(
             dataframe[geometry_column][0], shapely.geometry.base.BaseGeometry
         ):
             a = dataframe[geometry_column][0]
-            wkts = a.geom_type == "MultiPolygon"
-            # TODO: Implement
+            # if a.geom_type == "MultiPolygon":
+
+            wkts = [d.wkt for d in dataframe[geometry_column]]
         elif isinstance(dataframe[geometry_column][0], str):
             wkts = dataframe[geometry_column]
         else:
             raise NotImplemented
 
         for row in wkts:
-            add_geom_layer(qgis_instance_handle, row)
+            add_wkt(qgis_instance_handle, row)
+    else:
+        if VERBOSE:
+            print("SKIP!")
+
+
+@passes_kws_to(add_geometry)
+def add_geojson(qgis_instance_handle: Any, geojson: str, **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param dataframe:
+    :param kwargs:
+    :return:
+    """
+    geom = shapely.from_geojson(geojson)
+    add_shapely(geom)
 
 
 def remove_layers(qgis_instance_handle: Any, *args) -> None:
     """
+    clear all the added layers
 
     :param qgis_instance_handle:
     :param args:
     :return:
     """
     qgis_instance_handle.on_clear_temporary()
 
 
-def clear_all(qgis_instance_handle: Any) -> None:
+def clear_all(qgis_instance_handle: Any, *args) -> None:  # TODO: REMOVE THIS!
     """
+    clear all the added layers
 
     :param qgis_instance_handle:
     :return:
     """
     remove_layers(qgis_instance_handle)
-    print("CLEAR ALL!")
+    if VERBOSE:
+        print("CLEAR ALL!")
+
+
+def add_shapely(qgis_instance_handle: Any, geom: BaseGeometry, **kwargs) -> None:
+    """
+    Add a shapely geometry
+
+    :param qgis_instance_handle:
+    :param args:
+    :return:
+    """
+
+    add_wkt(qgis_instance_handle, geom.wkt)
 
 
 class QliveRPCMethodEnum(Enum):
     # add_layers = add_layers.__name__
+    remove_layers = remove_layers.__name__
+    clear_all = clear_all.__name__
     add_wkt = add_wkt.__name__
     add_wkb = add_wkb.__name__
     add_wkts = add_wkts.__name__
     add_wkbs = add_wkbs.__name__
     add_dataframe = add_dataframe.__name__
+    add_shapely = add_shapely.__name__
     add_raster = add_raster.__name__
     add_rasters = add_rasters.__name__
-    remove_layers = remove_layers.__name__
-    clear_all = clear_all.__name__
 
 
 funcs = locals()  # In local scope for name
 QliveRPCMethodMap = {e: funcs[e.value] for e in QliveRPCMethodEnum}
```

### Comparing `Jord-0.1.0/jord/qlive_utilities/serialisation.py` & `Jord-0.1.1/jord/qlive_utilities/serialisation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import base64
 import json
 import pickle
 from enum import Enum
-from typing import Tuple, Sequence
+from typing import Tuple, Sequence, Any
 
 __all__ = ["build_package", "read_package"]
 
 from sorcery import assigned_names
 
 from jord.qlive_utilities.procedures import QliveRPCMethodEnum, QliveRPCMethodMap
 
 
 class SerialisationMethodEnum(Enum):
     json, pickle = assigned_names()
 
 
 SERIALISATION_METHOD = SerialisationMethodEnum.pickle
+VERBOSE = False
 
 
-def build_package(method: QliveRPCMethodEnum, *args) -> bytes:
+def build_package(method: QliveRPCMethodEnum, *args: Any) -> bytes:
     """
 
     :param method:
     :param args:
     :return:
     """
+    if VERBOSE:
+        print(type(method), method, args)
+
+    if not isinstance(method, QliveRPCMethodEnum):
+        assert method
+        assert isinstance(method, str), method
+        method = QliveRPCMethodEnum(method)
+
+    if VERBOSE:
+        print(type(method.value), method.value, args)
+
     if SERIALISATION_METHOD == SerialisationMethodEnum.pickle:
         return pickle.dumps({"method": method.value, "args": args})
     elif SERIALISATION_METHOD == SERIALISATION_METHOD.json:
         return json.dump({"method": method.value, "args": args})  # TODO: ?
         # return base64.b64encode(str({"method": method.value, "args": args}).encode("ascii"))
     else:
         raise NotImplemented
@@ -55,8 +67,8 @@
         res_dict = pickle.loads(package)
     else:
         raise NotImplemented
     return QliveRPCMethodMap[QliveRPCMethodEnum(res_dict["method"])], res_dict["args"]
 
 
 if __name__ == "__main__":
-    print(read_package(build_package(method=QliveRPCMethodEnum.clear_all)))
+    print(read_package(build_package(method=QliveRPCMethodEnum.add_wkt)))
```

### Comparing `Jord-0.1.0/jord/qlive_utilities/uri_utilities.py` & `Jord-0.1.1/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/qt_utilities/enums.py` & `Jord-0.1.1/jord/qt_utilities/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-__all__ = ["DockWidgetAreaFlag"]
+__all__ = ["DockWidgetAreaFlag", "AlignmentFlag"]
 
 from enum import Flag, Enum
+
 from qgis.PyQt.QtCore import Qt
 
 
 class DockWidgetAreaFlag(Flag):
-    left = Qt.LeftDockWidgetArea  # 	0x1	The left dock area of a QMainWindow.
-    right = Qt.RightDockWidgetArea  # 	0x2	The right dock area of a QMainWindow.
-    top = Qt.TopDockWidgetArea  # 	0x4	The top dock area of a QMainWindow.
-    bottom = Qt.BottomDockWidgetArea  # 	0x8	The bottom dock area of a QMainWindow.
-    all = Qt.AllDockWidgetAreas  # 	DockWidgetArea_Mask	All dock widget areas (default).
-    none = Qt.NoDockWidgetArea  # 	0	No dock widget areas.
+    left = Qt.LeftDockWidgetArea  # 0x1	The left dock area of a QMainWindow.
+    right = Qt.RightDockWidgetArea  # 0x2	The right dock area of a QMainWindow.
+    top = Qt.TopDockWidgetArea  # 0x4	The top dock area of a QMainWindow.
+    bottom = Qt.BottomDockWidgetArea  # 0x8	The bottom dock area of a QMainWindow.
+    all = Qt.AllDockWidgetAreas  # DockWidgetArea_Mask	All dock widget areas (default).
+    none = Qt.NoDockWidgetArea  # 0	No dock widget areas.
 
 
 class DropActionFlag(Flag):
     """
       Qt::CopyAction	0x1	Copy the data to the target.
     Qt::MoveAction	0x2	Move the data from the source to the target.
     Qt::LinkAction	0x4	Create a link from the source to the target.
@@ -560,7 +561,17 @@
     Qt::Key_Printer	0x01020002
     Qt::Key_Play	0x01020005
     Qt::Key_Sleep	0x01020004
     Qt::Key_Zoom	0x01020006
     Qt::Key_Exit	0x0102000a
     Qt::Key_Cancel	0x01020001
     """
+
+
+class AlignmentFlag(Flag):
+    left = Qt.AlignLeft
+    right = Qt.AlignRight
+    bottom = Qt.AlignBottom
+    top = Qt.AlignTop
+    center = Qt.AlignCenter
+    horizontal_center = Qt.AlignHCenter
+    vertical_center = Qt.AlignVCenter
```

### Comparing `Jord-0.1.0/jord/shapely_utilities/__init__.py` & `Jord-0.1.1/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/clamp.py` & `Jord-0.1.1/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/geometry_types.py` & `Jord-0.1.1/jord/shapely_utilities/geometry_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,7 +34,11 @@
     multi_line_string = MultiLineString  # MultiLineString([lines]) # A collection of one or more LineStrings.
 
     multi_polygon = (
         MultiPolygon  # MultiPolygon([polygons]) # A collection of one or more Polygons.
     )
 
     geometry_collection = GeometryCollection  # GeometryCollection([geoms]) # A collection of one or more geometries that  may contain more than  one type of geometry.
+
+
+if __name__ == "__main__":
+    print([p.value.__name__ for p in ShapelyGeometryTypesEnum])
```

### Comparing `Jord-0.1.0/jord/shapely_utilities/iteration.py` & `Jord-0.1.1/jord/shapely_utilities/iteration.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/lines.py` & `Jord-0.1.1/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/mirroring.py` & `Jord-0.1.1/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/morphology.py` & `Jord-0.1.1/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/points.py` & `Jord-0.1.1/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/projection.py` & `Jord-0.1.1/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.1.1/jord/shapely_utilities/sanitise_poly.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/jord/shapely_utilities/transformation.py` & `Jord-0.1.1/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/setup.py` & `Jord-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.0/tests/test_import.py` & `Jord-0.1.1/tests/test_import.py`

 * *Files identical despite different names*

