# Comparing `tmp/jupyterlab_rtc_hub_settings-0.1.1.tar.gz` & `tmp/jupyterlab_rtc_hub_settings-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_rtc_hub_settings-0.1.1.tar", last modified: Wed Sep  8 20:17:55 2021, max compression
+gzip compressed data, was "jupyterlab_rtc_hub_settings-0.1.2.tar", last modified: Wed Jul 26 18:13:40 2023, max compression
```

## Comparing `jupyterlab_rtc_hub_settings-0.1.1.tar` & `jupyterlab_rtc_hub_settings-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.551782 jupyterlab_rtc_hub_settings-0.1.1/
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1520 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/LICENSE
--rwxrwxrwx   0 jovyan    (1000) users      (100)      485 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     5362 2021-09-08 20:17:55.551782 jupyterlab_rtc_hub_settings-0.1.1/PKG-INFO
--rwxrwxrwx   0 jovyan    (1000) users      (100)     4485 2021-09-08 18:12:47.000000 jupyterlab_rtc_hub_settings-0.1.1/README.md
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1911 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/RELEASE.md
--rwxrwxrwx   0 jovyan    (1000) users      (100)      215 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/install.json
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.521782 jupyterlab_rtc_hub_settings-0.1.1/jupyter-config/
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyter-config/nb-config/
--rwxrwxrwx   0 jovyan    (1000) users      (100)      104 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyter-config/nb-config/jupyterlab_rtc_hub_settings.json
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyter-config/server-config/
--rwxrwxrwx   0 jovyan    (1000) users      (100)      102 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyter-config/server-config/jupyterlab_rtc_hub_settings.json
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1159 2021-09-08 15:40:43.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/__init__.py
--rwxrwxrwx   0 jovyan    (1000) users      (100)      440 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/_version.py
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1620 2021-09-08 15:40:15.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/handlers.py
--rwxrwxrwx   0 jovyan    (1000) users      (100)     3090 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/hub_sharing_settings.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/
--rw-r--r--   0 jovyan    (1000) users      (100)    19821 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/build_log.json
--rwxrwxrwx   0 jovyan    (1000) users      (100)     2943 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/package.json
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/
--rw-r--r--   0 jovyan    (1000) users      (100)    13362 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js
--rw-r--r--   0 jovyan    (1000) users      (100)     8135 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js.map
--rw-r--r--   0 jovyan    (1000) users      (100)    28320 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js
--rw-r--r--   0 jovyan    (1000) users      (100)    27350 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js.map
--rw-r--r--   0 jovyan    (1000) users      (100)      170 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)    15502 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js
--rw-r--r--   0 jovyan    (1000) users      (100)    12763 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js.map
--rw-r--r--   0 jovyan    (1000) users      (100)    13179 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js
--rw-r--r--   0 jovyan    (1000) users      (100)    14965 2021-09-08 20:17:03.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js.map
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.531782 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     5362 2021-09-08 20:17:55.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1912 2021-09-08 20:17:55.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2021-09-08 20:17:55.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2021-09-08 20:12:07.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       32 2021-09-08 20:17:55.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       28 2021-09-08 20:17:55.000000 jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/top_level.txt
--rwxrwxrwx   0 jovyan    (1000) users      (100)     2822 2021-09-08 20:11:00.000000 jupyterlab_rtc_hub_settings-0.1.1/package.json
--rwxrwxrwx   0 jovyan    (1000) users      (100)      643 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2021-09-08 20:17:55.551782 jupyterlab_rtc_hub_settings-0.1.1/setup.cfg
--rwxrwxrwx   0 jovyan    (1000) users      (100)     3244 2021-09-08 15:38:21.000000 jupyterlab_rtc_hub_settings-0.1.1/setup.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.551782 jupyterlab_rtc_hub_settings-0.1.1/src/
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1114 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/src/handler.ts
--rwxrwxrwx   0 jovyan    (1000) users      (100)      937 2021-09-08 15:44:49.000000 jupyterlab_rtc_hub_settings-0.1.1/src/index.ts
--rwxrwxrwx   0 jovyan    (1000) users      (100)     2335 2021-09-08 18:53:01.000000 jupyterlab_rtc_hub_settings-0.1.1/src/sidebar.tsx
--rwxrwxrwx   0 jovyan    (1000) users      (100)     1301 2021-09-08 18:54:33.000000 jupyterlab_rtc_hub_settings-0.1.1/src/tableWidget.tsx
--rwxrwxrwx   0 jovyan    (1000) users      (100)      936 2021-09-08 01:35:01.000000 jupyterlab_rtc_hub_settings-0.1.1/src/toolbarWidget.ts
--rwxrwxrwx   0 jovyan    (1000) users      (100)      208 2021-09-08 00:41:37.000000 jupyterlab_rtc_hub_settings-0.1.1/src/types.ts
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-09-08 20:17:55.551782 jupyterlab_rtc_hub_settings-0.1.1/style/
--rwxrwxrwx   0 jovyan    (1000) users      (100)      925 2021-09-08 19:55:29.000000 jupyterlab_rtc_hub_settings-0.1.1/style/base.css
--rwxrwxrwx   0 jovyan    (1000) users      (100)       25 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/style/index.css
--rwxrwxrwx   0 jovyan    (1000) users      (100)       21 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/style/index.js
--rwxrwxrwx   0 jovyan    (1000) users      (100)     8075 2021-09-07 23:05:57.000000 jupyterlab_rtc_hub_settings-0.1.1/style/sharing_settings.svg
--rwxrwxrwx   0 jovyan    (1000) users      (100)      554 2021-09-07 22:56:42.000000 jupyterlab_rtc_hub_settings-0.1.1/tsconfig.json
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.275814 jupyterlab_rtc_hub_settings-0.1.2/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1075 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/LICENSE
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      485 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/MANIFEST.in
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     5360 2023-07-26 18:13:40.275665 jupyterlab_rtc_hub_settings-0.1.2/PKG-INFO
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     4485 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/README.md
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1911 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/RELEASE.md
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      215 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/install.json
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.265499 jupyterlab_rtc_hub_settings-0.1.2/jupyter-config/
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.268093 jupyterlab_rtc_hub_settings-0.1.2/jupyter-config/nb-config/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      104 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyter-config/nb-config/jupyterlab_rtc_hub_settings.json
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.268300 jupyterlab_rtc_hub_settings-0.1.2/jupyter-config/server-config/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      102 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyter-config/server-config/jupyterlab_rtc_hub_settings.json
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.269212 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1159 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/__init__.py
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      440 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/_version.py
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1620 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/handlers.py
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     3090 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/hub_sharing_settings.py
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.271107 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    22087 2023-07-26 18:10:44.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/build_log.json
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     2943 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/package.json
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.273423 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    13391 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     8166 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js.map
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    29258 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    28183 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js.map
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      170 2023-07-26 18:10:44.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/style.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    15502 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    12763 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js.map
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    13179 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)    14965 2023-07-26 18:10:45.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js.map
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.270499 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     5360 2023-07-26 18:13:40.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/PKG-INFO
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1912 2023-07-26 18:13:40.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        1 2023-07-26 18:13:40.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        1 2023-07-26 17:56:14.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/not-zip-safe
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)       32 2023-07-26 18:13:40.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/requires.txt
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)       28 2023-07-26 18:13:40.000000 jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/top_level.txt
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     2801 2023-07-26 17:56:32.000000 jupyterlab_rtc_hub_settings-0.1.2/package.json
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      643 2023-07-26 18:13:25.000000 jupyterlab_rtc_hub_settings-0.1.2/pyproject.toml
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)       38 2023-07-26 18:13:40.275848 jupyterlab_rtc_hub_settings-0.1.2/setup.cfg
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     3244 2023-07-26 03:58:22.000000 jupyterlab_rtc_hub_settings-0.1.2/setup.py
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.274620 jupyterlab_rtc_hub_settings-0.1.2/src/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1114 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/handler.ts
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      948 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/index.ts
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     2115 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/sidebar.tsx
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     1181 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/tableWidget.tsx
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      855 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/toolbarWidget.ts
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      201 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/src/types.ts
+drwxr-xr-x   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)        0 2023-07-26 18:13:40.275306 jupyterlab_rtc_hub_settings-0.1.2/style/
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      925 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/style/base.css
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)       25 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/style/index.css
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)       21 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/style/index.js
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)     8075 2021-11-17 21:47:47.000000 jupyterlab_rtc_hub_settings-0.1.2/style/sharing_settings.svg
+-rw-r--r--   0 taletskiyk2 (400208487) NIH\Domain Users (1360859114)      554 2023-07-26 17:58:29.000000 jupyterlab_rtc_hub_settings-0.1.2/tsconfig.json
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/PKG-INFO` & `jupyterlab_rtc_hub_settings-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_rtc_hub_settings
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension to manage real time collaboration settings on JupyterHub
 Home-page: https://github.com/LabShare/jupyterlab-extensions
 Author: Konstantin Taletskiy
 Author-email: konstantin.taletskiy@labshare.org
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -146,9 +146,7 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_rtc_hub_settings` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
-
-
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/README.md` & `jupyterlab_rtc_hub_settings-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/RELEASE.md` & `jupyterlab_rtc_hub_settings-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/__init__.py` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/handlers.py` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/hub_sharing_settings.py` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/hub_sharing_settings.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/build_log.json` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/build_log.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9634655395723103%*

 * *Differences: {'0': "{'module': {'rules': {15: {'use': ['source-map-loader'], 'enforce': 'pre'}, insert: [(14, "*

 * *      "OrderedDict([('test', OrderedDict()), ('type', 'file-loader')]))]}}, 'resolve': {'alias': "*

 * *      "{'@phosphor/algorithm$': "*

 * *      "'/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/algorithm/dist/index.js', "*

 * *      "'@phosphor/application$': "*

 * *      "'/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/application/d […]*

```diff
@@ -77,550 +77,582 @@
                     "resolve": {
                         "fullySpecified": false
                     },
                     "test": {}
                 },
                 {
                     "test": {},
-                    "use": "file-loader"
+                    "type": "file-loader"
+                },
+                {
+                    "enforce": "pre",
+                    "test": {},
+                    "use": [
+                        "source-map-loader"
+                    ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
-            "path": "/extension/jupyterlab_rtc_hub_settings/labextension/static",
+            "hashFunction": "sha256",
+            "path": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/jupyterlab_rtc_hub_settings/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/extension/lib/index.js",
-                        "./index": "/extension/lib/index.js",
-                        "./style": "/extension/style/index.js"
+                        "./extension": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/lib/index.js",
+                        "./index": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/lib/index.js",
+                        "./style": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "jupyterlab_rtc_hub_settings"
                         ],
                         "type": "var"
                     },
                     "name": "jupyterlab_rtc_hub_settings",
                     "shared": {
+                        "@jupyter/ydoc": {
+                            "import": false,
+                            "requiredVersion": "^0.2.3",
+                            "singleton": true
+                        },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
+                        },
+                        "@jupyterlab/cell-toolbar": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/cell-toolbar-extension": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
+                        },
+                        "@jupyterlab/collaboration": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/collaboration-extension": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.1.0",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.1.0"
+                            "requiredVersion": "^4.6.3"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.1.0",
+                            "requiredVersion": "^6.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.1.0",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.1.0"
+                            "requiredVersion": "^5.6.3"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.1.0",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.0"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.1.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@lumino/algorithm": {
                             "import": false,
-                            "requiredVersion": "^1.3.3",
+                            "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.16.0",
+                            "requiredVersion": "^1.31.4",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
-                            "requiredVersion": "^1.12.0",
+                            "requiredVersion": "^1.19.0",
                             "singleton": true
                         },
                         "@lumino/coreutils": {
                             "import": false,
-                            "requiredVersion": "^1.5.3",
+                            "requiredVersion": "^1.11.0",
                             "singleton": true
                         },
                         "@lumino/disposable": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/domutils": {
                             "import": false,
-                            "requiredVersion": "^1.2.3",
+                            "requiredVersion": "^1.8.0",
                             "singleton": true
                         },
                         "@lumino/dragdrop": {
                             "import": false,
-                            "requiredVersion": "^1.7.1",
+                            "requiredVersion": "^1.13.0",
                             "singleton": true
                         },
                         "@lumino/messaging": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/properties": {
                             "import": false,
-                            "requiredVersion": "^1.2.3",
+                            "requiredVersion": "^1.8.0",
                             "singleton": true
                         },
                         "@lumino/signaling": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/virtualdom": {
                             "import": false,
-                            "requiredVersion": "^1.8.0",
+                            "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.19.0",
+                            "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "jupyterlab_rtc_hub_settings": {
-                            "import": "/extension/lib/index.js",
+                            "import": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.1"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "yjs": {
                             "import": false,
-                            "requiredVersion": "^13.5.6",
+                            "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
                 }
             },
             {}
         ],
         "resolve": {
             "alias": {
-                "@phosphor/algorithm$": "/extension/node_modules/@lumino/algorithm/dist/index.js",
-                "@phosphor/application$": "/extension/node_modules/@lumino/application/dist/index.js",
-                "@phosphor/commands$": "/extension/node_modules/@lumino/commands/dist/index.js",
-                "@phosphor/coreutils$": "/extension/node_modules/@lumino/coreutils/dist/index.js",
-                "@phosphor/disposable$": "/extension/node_modules/@lumino/disposable/dist/index.js",
-                "@phosphor/domutils$": "/extension/node_modules/@lumino/domutils/dist/index.js",
-                "@phosphor/dragdrop$": "/extension/node_modules/@lumino/dragdrop/dist/index.js",
-                "@phosphor/dragdrop/style": "/extension/node_modules/@lumino/widgets/style",
-                "@phosphor/messaging$": "/extension/node_modules/@lumino/messaging/dist/index.js",
-                "@phosphor/properties$": "/extension/node_modules/@lumino/properties/dist/index.js",
-                "@phosphor/signaling": "/extension/node_modules/@lumino/signaling/dist/index.js",
-                "@phosphor/virtualdom$": "/extension/node_modules/@lumino/virtualdom/dist/index.js",
-                "@phosphor/widgets$": "/extension/node_modules/@lumino/widgets/dist/index.js",
-                "@phosphor/widgets/style": "/extension/node_modules/@lumino/widgets/style"
+                "@phosphor/algorithm$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/algorithm/dist/index.js",
+                "@phosphor/application$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/application/dist/index.js",
+                "@phosphor/commands$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/commands/dist/index.js",
+                "@phosphor/coreutils$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/coreutils/dist/index.node.js",
+                "@phosphor/disposable$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/disposable/dist/index.js",
+                "@phosphor/domutils$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/domutils/dist/index.js",
+                "@phosphor/dragdrop$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/dragdrop/dist/index.js",
+                "@phosphor/dragdrop/style": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/widgets/style",
+                "@phosphor/messaging$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/messaging/dist/index.js",
+                "@phosphor/properties$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/properties/dist/index.js",
+                "@phosphor/signaling": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/signaling/dist/index.js",
+                "@phosphor/virtualdom$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/virtualdom/dist/index.js",
+                "@phosphor/widgets$": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/widgets/dist/index.js",
+                "@phosphor/widgets/style": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/@lumino/widgets/style"
             },
             "fallback": {
                 "buffer": false,
-                "path": "/extension/node_modules/path-browserify/index.js",
-                "process": "/extension/node_modules/process/browser.js",
+                "crypto": false,
+                "path": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/path-browserify/index.js",
+                "process": "/Users/taletskiyk2/git/jupyterlab-extensions/jupyterlab_rtc_hub_settings/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/package.json` & `jupyterlab_rtc_hub_settings-0.1.2/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9551136363636363%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.4', '@jupyterlab/coreutils': '^5.6.5', "*

 * *                   "'@jupyterlab/services': '^6.6.5'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -3,21 +3,21 @@
         "email": "konstantin.taletskiy@labshare.org",
         "name": "Konstantin Taletskiy"
     },
     "bugs": {
         "url": "https://github.com/LabShare/jupyterlab-extensions/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/services": "^6.1.0"
+        "@jupyterlab/application": "^3.6.4",
+        "@jupyterlab/coreutils": "^5.6.5",
+        "@jupyterlab/services": "^6.6.5"
     },
     "description": "A JupyterLab extension to manage real time collaboration settings on JupyterHub",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
+        "@jupyterlab/builder": "^3.6.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
@@ -35,19 +35,14 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.4ea8b094493f59bbfe18.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_rtc_hub_settings"
                 },
                 "managers": [
                     "pip"
@@ -89,9 +84,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "requestAPI": () => ( /* binding */ requestAPI)
+                    requestAPI: () => ( /* binding */ requestAPI)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/coreutils */ "webpack/sharing/consume/default/@jupyterlab/coreutils");
                 /* harmony import */
                 var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -94,15 +94,16 @@
                     autoStart: true,
                     requires: [_jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabShell],
                     activate: (app, labShell) => {
                         console.log('JupyterLab extension jupyterlab_rtc_hub_settings is activated!');
                         // Create the sharing settings sidebar panel
                         const sidebar = new _sidebar__WEBPACK_IMPORTED_MODULE_1__.SharingSettingsSidebar();
                         sidebar.id = 'rtc-hub-settings-labextension:plugin';
-                        sidebar.title.iconClass = 'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';
+                        sidebar.title.iconClass =
+                            'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';
                         sidebar.title.caption = 'Sharing settings';
                         // Register sidebar panel with JupyterLab
                         labShell.add(sidebar, 'left', {
                             rank: 600
                         });
                     }
                 };
@@ -121,15 +122,15 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "SharingSettingsSidebar": () => ( /* binding */ SharingSettingsSidebar)
+                    SharingSettingsSidebar: () => ( /* binding */ SharingSettingsSidebar)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @lumino/widgets */ "webpack/sharing/consume/default/@lumino/widgets");
                 /* harmony import */
                 var _lumino_widgets__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_lumino_widgets__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -163,49 +164,47 @@
                 class SharingSettingsSidebar extends _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.Widget {
                     constructor() {
                         super();
                         this._users = [];
                         this._valueChanged = new _lumino_signaling__WEBPACK_IMPORTED_MODULE_2__.Signal(this);
                         this.addClass('rtc-hub-settings-SharingSettingsSidebar');
                         // Define widget layout
-                        let layout = (this.layout = new _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.PanelLayout());
+                        const layout = (this.layout = new _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.PanelLayout());
                         // Add Toolbar widget
-                        let toolbar = new _toolbarWidget__WEBPACK_IMPORTED_MODULE_4__.ToolbarWidget(() => {
+                        const toolbar = new _toolbarWidget__WEBPACK_IMPORTED_MODULE_4__.ToolbarWidget(() => {
                             this._getUsers();
                         });
                         layout.addWidget(toolbar);
                         // Add Users table widget
-                        let table = _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget.create(react__WEBPACK_IMPORTED_MODULE_3___default().createElement(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.UseSignal, {
+                        const table = _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget.create(react__WEBPACK_IMPORTED_MODULE_3___default().createElement(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.UseSignal, {
                             signal: this._valueChanged,
                             initialArgs: this._users
-                        }, (_, oa) => react__WEBPACK_IMPORTED_MODULE_3___default().createElement(_tableWidget__WEBPACK_IMPORTED_MODULE_5__.UsersTableWidget, {
-                            ar: oa,
-                            updateUsers: (arg0) => this._updateUsers(arg0),
+                        }, (_, oa) => (react__WEBPACK_IMPORTED_MODULE_3___default().createElement(_tableWidget__WEBPACK_IMPORTED_MODULE_5__.UsersTableWidget, {
+                            ar: oa === undefined ? [] : oa,
+                            updateUsers: arg0 => this._updateUsers(arg0),
                             refreshUsers: () => this._getUsers()
-                        })));
+                        }))));
                         table.addClass('rtc-hub-settings-SharingSettingsSidebar-table-div');
                         layout.addWidget(table);
                     }
                     async _getUsers() {
                         // Return results of API request
-                        (0, _handler__WEBPACK_IMPORTED_MODULE_6__.requestAPI)('users')
-                        .then(response => {
+                        (0, _handler__WEBPACK_IMPORTED_MODULE_6__.requestAPI)('users').then(response => {
                             // Update internal variable
                             this._users = response;
                             // Send signal for table widget to update data
                             this._valueChanged.emit(this._users);
                         });
                     }
                     async _updateUsers(users) {
                         // Send updated list of users statuses
                         (0, _handler__WEBPACK_IMPORTED_MODULE_6__.requestAPI)('users', {
                             method: 'POST',
                             body: JSON.stringify(users)
-                        })
-                        .then(response => {
+                        }).then(response => {
                             // Update internal variable
                             this._users = response;
                             // Send signal for table widget to update data
                             this._valueChanged.emit(this._users);
                         });
                     }
                 }
@@ -222,29 +221,29 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "UsersTableWidget": () => ( /* binding */ UsersTableWidget)
+                    UsersTableWidget: () => ( /* binding */ UsersTableWidget)
                     /* harmony export */
                 });
                 /* harmony import */
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! react */ "webpack/sharing/consume/default/react");
                 /* harmony import */
                 var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);
 
                 // Class for table of users
                 class UsersTableWidget extends react__WEBPACK_IMPORTED_MODULE_0__.Component {
                     constructor(props) {
                         super(props);
                         this.updateUser = (name) => {
-                            let props = this.props;
-                            let index = props.ar.findIndex((user) => (user.name == name));
+                            const props = this.props;
+                            const index = props.ar.findIndex((user) => user.name === name);
                             props.ar[index].shared = !props.ar[index].shared;
                             props.updateUsers(props.ar);
                         };
                         props.refreshUsers();
                     }
                     render() {
                         const tableRows = this.props.ar.map((user) => {
@@ -256,19 +255,19 @@
                                         checked: user.shared,
                                         onChange: () => this.updateUser(user.name)
                                     }))));
                         });
                         // Assemble headers and rows in the full table
                         return (react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", null,
                             react__WEBPACK_IMPORTED_MODULE_0___default().createElement("table", {
-                                    className: 'rtc-hub-settings-SharingSettingsSidebar-table'
+                                    className: "rtc-hub-settings-SharingSettingsSidebar-table"
                                 },
                                 react__WEBPACK_IMPORTED_MODULE_0___default().createElement("tbody", null, tableRows))));
                     }
-                };
+                }
 
 
                 /***/
             }),
 
         /***/
         "./lib/toolbarWidget.js":
@@ -278,15 +277,15 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "ToolbarWidget": () => ( /* binding */ ToolbarWidget)
+                    ToolbarWidget: () => ( /* binding */ ToolbarWidget)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -326,8 +325,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.de2dc6ad8eda78818ec6.js.map
+//# sourceMappingURL=lib_index_js.aa27acd2f9d9b6c528e8.js.map
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js.map` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8035714285714286%*

 * *Differences: {"'file'": "'lib_index_js.aa27acd2f9d9b6c528e8.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,kEAAgB;AACrC,uBAAuB,yDAAM;AAC7B;AACA;AACA;AACA,yBAAyB,kEAAgB;AACzC;AACA;AACA,kBAAkB,kEAAgB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,kEAAgB;AAClC;AACA;AACA;;;;;;;;;;;;;;;;;;AClCoD;AACD;AACnD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,8DAAS;AACxB;AACA;AACA;AACA,4BAA4B,4DAAsB;AAClD;AACA;AACA;AACA;AACA;AACA,wCAAwC,WAAW;AACnD;AACA;A […]*

```diff
@@ -1,21 +1,21 @@
 {
-    "file": "lib_index_js.de2dc6ad8eda78818ec6.js",
-    "mappings": ";;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;AClCoD;AACD;AACnD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,8DAAS;AACxB;AACA;AACA;AACA,4BAA4B,4DAAsB;AAClD;AACA;AACA;AACA;AACA,wCAAwC,WAAW;AACnD;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;ACpBgC;AACf;AACU;AACD;AACc;AACnB;AACjB;AAC1B;AACA;AACA;AACO,qCAAqC,mDAAM;AAClD;AACA;AACA;AACA,iCAAiC,qDAAM;AACvC;AACA;AACA,wCAAwC,wDAAW;AACnD;AACA,0BAA0B,yDAAa,SAAS,mBAAmB;AACnE;AACA;AACA,oBAAoB,oEAAkB,CAAC,0DAAmB,CAAC,2DAAS,IAAI,sDAAsD,aAAa,0DAAmB,CAAC,0DAAgB,IAAI,8FAA8F;AACjR;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;ACjDyC;AACzC;AACO,+BAA+B,4CAAS;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,0DAAmB;AACvC,gBAAgB,0DAAmB;AACnC,gBAAgB,0DAAmB;AACnC,oBAAoB,0DAAmB,YAAY,oFAAoF;AACvI,SAAS;AACT;AACA,gBAAgB,0DAAmB;AACnC,YAAY,0DAAmB,YAAY,4DAA4D;AACvG,gBAAgB,0DAAmB;AACnC;AACA;AACA;;;;;;;;;;;;;;;;;;;;;AC1BwD;AACF;AACD;AAC9C,4BAA4B,mDAAM;AACzC;AACA;AACA;AACA,0CAA0C,wDAAW;AACrD,2BAA2B,mDAAM,GAAG,qCAAqC;AACzE;AACA;AACA,2BAA2B,mDAAM,GAAG,sCAAsC;AAC1E;AACA;AACA;AACA,kCAAkC,+DAAa;AAC/C,kBAAkB,kEAAW;AAC7B;AACA,SAAS;AACT;AACA;AACA",
+    "file": "lib_index_js.aa27acd2f9d9b6c528e8.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,kEAAgB;AACrC,uBAAuB,yDAAM;AAC7B;AACA;AACA;AACA,yBAAyB,kEAAgB;AACzC;AACA;AACA,kBAAkB,kEAAgB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,kEAAgB;AAClC;AACA;AACA;;;;;;;;;;;;;;;;;;AClCoD;AACD;AACnD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,8DAAS;AACxB;AACA;AACA;AACA,4BAA4B,4DAAsB;AAClD;AACA;AACA;AACA;AACA;AACA,wCAAwC,WAAW;AACnD;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;ACrBgC;AACf;AACU;AACD;AACc;AACnB;AACjB;AAC1B;AACA;AACA;AACO,qCAAqC,mDAAM;AAClD;AACA;AACA;AACA,iCAAiC,qDAAM;AACvC;AACA;AACA,0CAA0C,wDAAW;AACrD;AACA,4BAA4B,yDAAa;AACzC;AACA,SAAS;AACT;AACA;AACA,sBAAsB,6DAAW,QAAQ,0DAAmB,CAAC,2DAAS,IAAI,sDAAsD,cAAc,0DAAmB,CAAC,0DAAgB,IAAI,oHAAoH;AAC1S;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;ACjDyC;AACzC;AACO,+BAA+B,4CAAS;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,0DAAmB;AACvC,gBAAgB,0DAAmB;AACnC,gBAAgB,0DAAmB;AACnC,oBAAoB,0DAAmB,YAAY,oFAAoF;AACvI,SAAS;AACT;AACA,gBAAgB,0DAAmB;AACnC,YAAY,0DAAmB,YAAY,4DAA4D;AACvG,gBAAgB,0DAAmB;AACnC;AACA;;;;;;;;;;;;;;;;;;;;;ACzBwD;AACF;AACD;AAC9C,4BAA4B,mDAAM;AACzC;AACA;AACA;AACA,0CAA0C,wDAAW;AACrD,2BAA2B,mDAAM,GAAG,qCAAqC;AACzE;AACA;AACA,2BAA2B,mDAAM,GAAG,sCAAsC;AAC1E;AACA;AACA;AACA,kCAAkC,+DAAa;AAC/C,kBAAkB,kEAAW;AAC7B;AACA,SAAS;AACT;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_rtc_hub_settings/./lib/handler.js",
         "webpack://jupyterlab_rtc_hub_settings/./lib/index.js",
         "webpack://jupyterlab_rtc_hub_settings/./lib/sidebar.js",
         "webpack://jupyterlab_rtc_hub_settings/./lib/tableWidget.js",
         "webpack://jupyterlab_rtc_hub_settings/./lib/toolbarWidget.js"
     ],
     "sourcesContent": [
         "import { URLExt } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI(endPoint = '', init = {}) {\n    // Make request to Jupyter API\n    const settings = ServerConnection.makeSettings();\n    const requestUrl = URLExt.join(settings.baseUrl, 'jupyterlab-rtc-hub-settings', // API Namespace\n    endPoint);\n    let response;\n    try {\n        response = await ServerConnection.makeRequest(requestUrl, init, settings);\n    }\n    catch (error) {\n        throw new ServerConnection.NetworkError(error);\n    }\n    let data = await response.text();\n    if (data.length > 0) {\n        try {\n            data = JSON.parse(data);\n        }\n        catch (error) {\n            console.log('Not a JSON response body.', response);\n        }\n    }\n    if (!response.ok) {\n        throw new ServerConnection.ResponseError(response, data.message || data);\n    }\n    return data;\n}\n",
-        "import { ILabShell } from '@jupyterlab/application';\nimport { SharingSettingsSidebar } from './sidebar';\n/**\n * Initialization data for the jupyterlab_rtc_hub_settings extension.\n */\nconst plugin = {\n    id: 'jupyterlab_rtc_hub_settings:plugin',\n    autoStart: true,\n    requires: [ILabShell],\n    activate: (app, labShell) => {\n        console.log('JupyterLab extension jupyterlab_rtc_hub_settings is activated!');\n        // Create the sharing settings sidebar panel\n        const sidebar = new SharingSettingsSidebar();\n        sidebar.id = 'rtc-hub-settings-labextension:plugin';\n        sidebar.title.iconClass = 'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';\n        sidebar.title.caption = 'Sharing settings';\n        // Register sidebar panel with JupyterLab\n        labShell.add(sidebar, 'left', { rank: 600 });\n    }\n};\nexport default plugin;\n",
-        "import { Widget, PanelLayout } from '@lumino/widgets';\nimport { requestAPI } from './handler';\nimport { UsersTableWidget } from './tableWidget';\nimport { ToolbarWidget } from './toolbarWidget';\nimport { ReactWidget, UseSignal } from '@jupyterlab/apputils';\nimport { Signal } from '@lumino/signaling';\nimport React from 'react';\n/**\n * Sidebar widget for displaying RTC sharing settings.\n */\nexport class SharingSettingsSidebar extends Widget {\n    constructor() {\n        super();\n        this._users = [];\n        this._valueChanged = new Signal(this);\n        this.addClass('rtc-hub-settings-SharingSettingsSidebar');\n        // Define widget layout\n        let layout = (this.layout = new PanelLayout());\n        // Add Toolbar widget\n        let toolbar = new ToolbarWidget(() => { this._getUsers(); });\n        layout.addWidget(toolbar);\n        // Add Users table widget\n        let table = ReactWidget.create(React.createElement(UseSignal, { signal: this._valueChanged, initialArgs: this._users }, (_, oa) => React.createElement(UsersTableWidget, { ar: oa, updateUsers: (arg0) => this._updateUsers(arg0), refreshUsers: () => this._getUsers() })));\n        table.addClass('rtc-hub-settings-SharingSettingsSidebar-table-div');\n        layout.addWidget(table);\n    }\n    async _getUsers() {\n        // Return results of API request\n        requestAPI('users')\n            .then(response => {\n            // Update internal variable\n            this._users = response;\n            // Send signal for table widget to update data\n            this._valueChanged.emit(this._users);\n        });\n    }\n    async _updateUsers(users) {\n        // Send updated list of users statuses\n        requestAPI('users', {\n            method: 'POST',\n            body: JSON.stringify(users)\n        })\n            .then(response => {\n            // Update internal variable\n            this._users = response;\n            // Send signal for table widget to update data\n            this._valueChanged.emit(this._users);\n        });\n    }\n}\n",
-        "import React, { Component } from 'react';\n// Class for table of users\nexport class UsersTableWidget extends Component {\n    constructor(props) {\n        super(props);\n        this.updateUser = (name) => {\n            let props = this.props;\n            let index = props.ar.findIndex((user) => (user.name == name));\n            props.ar[index].shared = !props.ar[index].shared;\n            props.updateUsers(props.ar);\n        };\n        props.refreshUsers();\n    }\n    render() {\n        const tableRows = this.props.ar.map((user) => {\n            return (React.createElement(\"tr\", null,\n                React.createElement(\"td\", null, user.name),\n                React.createElement(\"td\", null,\n                    React.createElement(\"input\", { type: \"checkbox\", checked: user.shared, onChange: () => this.updateUser(user.name) }))));\n        });\n        // Assemble headers and rows in the full table\n        return (React.createElement(\"div\", null,\n            React.createElement(\"table\", { className: 'rtc-hub-settings-SharingSettingsSidebar-table' },\n                React.createElement(\"tbody\", null, tableRows))));\n    }\n}\n;\n",
+        "import { ILabShell } from '@jupyterlab/application';\nimport { SharingSettingsSidebar } from './sidebar';\n/**\n * Initialization data for the jupyterlab_rtc_hub_settings extension.\n */\nconst plugin = {\n    id: 'jupyterlab_rtc_hub_settings:plugin',\n    autoStart: true,\n    requires: [ILabShell],\n    activate: (app, labShell) => {\n        console.log('JupyterLab extension jupyterlab_rtc_hub_settings is activated!');\n        // Create the sharing settings sidebar panel\n        const sidebar = new SharingSettingsSidebar();\n        sidebar.id = 'rtc-hub-settings-labextension:plugin';\n        sidebar.title.iconClass =\n            'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';\n        sidebar.title.caption = 'Sharing settings';\n        // Register sidebar panel with JupyterLab\n        labShell.add(sidebar, 'left', { rank: 600 });\n    }\n};\nexport default plugin;\n",
+        "import { Widget, PanelLayout } from '@lumino/widgets';\nimport { requestAPI } from './handler';\nimport { UsersTableWidget } from './tableWidget';\nimport { ToolbarWidget } from './toolbarWidget';\nimport { ReactWidget, UseSignal } from '@jupyterlab/apputils';\nimport { Signal } from '@lumino/signaling';\nimport React from 'react';\n/**\n * Sidebar widget for displaying RTC sharing settings.\n */\nexport class SharingSettingsSidebar extends Widget {\n    constructor() {\n        super();\n        this._users = [];\n        this._valueChanged = new Signal(this);\n        this.addClass('rtc-hub-settings-SharingSettingsSidebar');\n        // Define widget layout\n        const layout = (this.layout = new PanelLayout());\n        // Add Toolbar widget\n        const toolbar = new ToolbarWidget(() => {\n            this._getUsers();\n        });\n        layout.addWidget(toolbar);\n        // Add Users table widget\n        const table = ReactWidget.create(React.createElement(UseSignal, { signal: this._valueChanged, initialArgs: this._users }, (_, oa) => (React.createElement(UsersTableWidget, { ar: oa === undefined ? [] : oa, updateUsers: arg0 => this._updateUsers(arg0), refreshUsers: () => this._getUsers() }))));\n        table.addClass('rtc-hub-settings-SharingSettingsSidebar-table-div');\n        layout.addWidget(table);\n    }\n    async _getUsers() {\n        // Return results of API request\n        requestAPI('users').then(response => {\n            // Update internal variable\n            this._users = response;\n            // Send signal for table widget to update data\n            this._valueChanged.emit(this._users);\n        });\n    }\n    async _updateUsers(users) {\n        // Send updated list of users statuses\n        requestAPI('users', {\n            method: 'POST',\n            body: JSON.stringify(users)\n        }).then(response => {\n            // Update internal variable\n            this._users = response;\n            // Send signal for table widget to update data\n            this._valueChanged.emit(this._users);\n        });\n    }\n}\n",
+        "import React, { Component } from 'react';\n// Class for table of users\nexport class UsersTableWidget extends Component {\n    constructor(props) {\n        super(props);\n        this.updateUser = (name) => {\n            const props = this.props;\n            const index = props.ar.findIndex((user) => user.name === name);\n            props.ar[index].shared = !props.ar[index].shared;\n            props.updateUsers(props.ar);\n        };\n        props.refreshUsers();\n    }\n    render() {\n        const tableRows = this.props.ar.map((user) => {\n            return (React.createElement(\"tr\", null,\n                React.createElement(\"td\", null, user.name),\n                React.createElement(\"td\", null,\n                    React.createElement(\"input\", { type: \"checkbox\", checked: user.shared, onChange: () => this.updateUser(user.name) }))));\n        });\n        // Assemble headers and rows in the full table\n        return (React.createElement(\"div\", null,\n            React.createElement(\"table\", { className: \"rtc-hub-settings-SharingSettingsSidebar-table\" },\n                React.createElement(\"tbody\", null, tableRows))));\n    }\n}\n",
         "import { refreshIcon } from '@jupyterlab/ui-components';\nimport { PanelLayout, Widget } from '@lumino/widgets';\nimport { ToolbarButton } from '@jupyterlab/apputils';\nexport class ToolbarWidget extends Widget {\n    constructor(refresh) {\n        super();\n        this.addClass('rtc-hub-settings-Toolbar-layout');\n        const layout = (this.layout = new PanelLayout());\n        const header = new Widget({ node: document.createElement('div') });\n        header.node.textContent = 'Collaboration Sharing';\n        layout.addWidget(header);\n        const spacer = new Widget({ node: document.createElement('span') });\n        spacer.addClass('rtc-hub-settings-Toolbar-spacer');\n        layout.addWidget(spacer);\n        // Search button\n        const refreshButton = new ToolbarButton({\n            icon: refreshIcon,\n            onClick: refresh\n        });\n        layout.addWidget(refreshButton);\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
                     "./index": () => {
                         return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
                         return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
+                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -35,16 +35,16 @@
                         })
                     );
                     __webpack_require__.R = undefined;
                     return getScope;
                 };
                 var init = (shareScope, initScope) => {
                     if (!__webpack_require__.S) return;
-                    var oldScope = __webpack_require__.S["default"];
                     var name = "default"
+                    var oldScope = __webpack_require__.S[name];
                     if (oldScope && oldScope !== shareScope) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                     __webpack_require__.S[name] = shareScope;
                     return __webpack_require__.I(name, initScope);
                 };
 
                 // This exports getters to disallow modifications
                 __webpack_require__.d(exports, {
@@ -182,17 +182,17 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "de2dc6ad8eda78818ec6",
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda": "e45f95686c6bc860f917",
-                "style_index_js": "ed36e06a9ec9cea697a5"
+                "lib_index_js": "aa27acd2f9d9b6c528e8",
+                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f": "7b993b2d1f84a3f18312",
+                "style_index_js": "7e039c6467f810b4fa05"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -278,14 +278,15 @@
                     /******/
                     script.setAttribute("nonce", __webpack_require__.nc);
                     /******/
                 }
                 /******/
                 script.setAttribute("data-webpack", dataWebpackPrefix + key);
                 /******/
+                /******/
                 script.src = url;
                 /******/
             }
             /******/
             inProgress[url] = [done];
             /******/
             var onScriptComplete = (prev, event) => {
@@ -303,16 +304,14 @@
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
             }
             /******/
-            ;
-            /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
             /******/
@@ -377,15 +376,19 @@
             /******/ // creates a new share scope if needed
             /******/
             if (!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};
             /******/ // runs all init snippets from all modules reachable
             /******/
             var scope = __webpack_require__.S[name];
             /******/
-            var warn = (msg) => (typeof console !== "undefined" && console.warn && console.warn(msg));
+            var warn = (msg) => {
+                /******/
+                if (typeof console !== "undefined" && console.warn) console.warn(msg);
+                /******/
+            };
             /******/
             var uniqueName = "jupyterlab_rtc_hub_settings";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
@@ -411,29 +414,29 @@
                     /******/
                     var initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))
                     /******/
                     if (module.then) return promises.push(module.then(initFn, handleError));
                     /******/
                     var initResult = initFn(module);
                     /******/
-                    if (initResult && initResult.then) return promises.push(initResult.catch(handleError));
+                    if (initResult && initResult.then) return promises.push(initResult['catch'](handleError));
                     /******/
                 } catch (err) {
                     handleError(err);
                 }
                 /******/
             }
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab_rtc_hub_settings", "0.1.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_rtc_hub_settings", "0.1.2", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -456,21 +459,27 @@
         /******/
         var document = __webpack_require__.g.document;
         /******/
         if (!scriptUrl && document) {
             /******/
             if (document.currentScript)
                 /******/
-                scriptUrl = document.currentScript.src
+                scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
-                if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
+                if (scripts.length) {
+                    /******/
+                    var i = scripts.length - 1;
+                    /******/
+                    while (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;
+                    /******/
+                }
                 /******/
             }
             /******/
         }
         /******/ // When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration
         /******/ // or pass an empty string ("") and set the __webpack_public_path__ variable from your code to use your own logic.
         /******/
@@ -617,35 +626,43 @@
                 /******/
                 return !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;
                 /******/
             }, 0);
             /******/
         };
         /******/
-        var getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {
+        var getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {
+            /******/
+            return "Unsatisfied version " + version + " from " + (version && scope[key][version].from) + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
+            /******/
+        };
+        /******/
+        var getSingleton = (scope, scopeName, key, requiredVersion) => {
+            /******/
+            var version = findSingletonVersionKey(scope, key);
             /******/
-            return "Unsatisfied version " + version + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
+            return get(scope[key][version]);
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var findValidVersion = (scope, key, requiredVersion) => {
             /******/
@@ -683,17 +700,23 @@
             /******/
             if (entry) return get(entry);
             /******/
             throw new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
+        var warn = (msg) => {
+            /******/
+            if (typeof console !== "undefined" && console.warn) console.warn(msg);
+            /******/
+        };
+        /******/
         var warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
-            typeof console !== "undefined" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
+            warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
         var get = (entry) => {
             /******/
             entry.loaded = 1;
             /******/
@@ -730,14 +753,22 @@
             /******/
             ensureExistence(scopeName, key);
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
+        var loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {
+            /******/
+            ensureExistence(scopeName, key);
+            /******/
+            return getSingleton(scope, scopeName, key);
+            /******/
+        });
+        /******/
         var loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {
             /******/
             ensureExistence(scopeName, key);
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -762,14 +793,22 @@
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
+        var loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {
+            /******/
+            if (!scope || !__webpack_require__.o(scope, key)) return fallback();
+            /******/
+            return getSingleton(scope, scopeName, key);
+            /******/
+        });
+        /******/
         var loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -790,29 +829,29 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 1, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 19, 0])),
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 37, 2])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 1, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 4, 3])),
+            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 10, 0])),
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 1, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 1, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 1, 0]))
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 6, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -875,15 +914,15 @@
                     /******/
                     try {
                         /******/
                         var promise = moduleToHandlerMapping[id]();
                         /******/
                         if (promise.then) {
                             /******/
-                            promises.push(installedModules[id] = promise.then(onFactory).catch(onError));
+                            promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
                             /******/
                         } else onFactory(promise);
                         /******/
                     } catch (e) {
                         onError(e);
                     }
                     /******/
@@ -969,15 +1008,15 @@
                                 /******/
                             }
                             /******/
                         };
                         /******/
                         __webpack_require__.l(url, loadingEnded, "chunk-" + chunkId, chunkId);
                         /******/
-                    } else installedChunks[chunkId] = 0;
+                    }
                     /******/
                 }
                 /******/
             }
             /******/
         };
         /******/
@@ -1025,15 +1064,15 @@
                 /******/
                 if (__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {
                     /******/
                     installedChunks[chunkId][0]();
                     /******/
                 }
                 /******/
-                installedChunks[chunkIds[i]] = 0;
+                installedChunks[chunkId] = 0;
                 /******/
             }
             /******/
             /******/
         }
         /******/
         /******/
@@ -1041,20 +1080,29 @@
         /******/
         chunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));
         /******/
         chunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));
         /******/
     })();
     /******/
+    /******/
+    /* webpack/runtime/nonce */
+    /******/
+    (() => {
+        /******/
+        __webpack_require__.nc = undefined;
+        /******/
+    })();
+    /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_rtc_hub_settings");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_rtc_hub_settings = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.4ea8b094493f59bbfe18.js.map
+//# sourceMappingURL=remoteEntry.5df98682aa24d1bcf559.js.map
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js.map` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8103174603174603%*

 * *Differences: {"'file'": "'remoteEntry.5df98682aa24d1bcf559.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.4ea8b094493f59bbfe18.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCzKA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
+    "file": "remoteEntry.5df98682aa24d1bcf559.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCxLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_rtc_hub_settings/webpack/container-entry",
         "webpack://jupyterlab_rtc_hub_settings/webpack/bootstrap",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/compat get default export",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/define property getters",
@@ -14,32 +14,34 @@
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/hasOwnProperty shorthand",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/load script",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/make namespace object",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/sharing",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/publicPath",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/consumes",
         "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/jsonp chunk loading",
+        "webpack://jupyterlab_rtc_hub_settings/webpack/runtime/nonce",
         "webpack://jupyterlab_rtc_hub_settings/webpack/before-startup",
         "webpack://jupyterlab_rtc_hub_settings/webpack/startup",
         "webpack://jupyterlab_rtc_hub_settings/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar oldScope = __webpack_require__.S[\"default\"];\n\tvar name = \"default\"\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"de2dc6ad8eda78818ec6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda\":\"e45f95686c6bc860f917\",\"style_index_js\":\"ed36e06a9ec9cea697a5\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"aa27acd2f9d9b6c528e8\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f\":\"7b993b2d1f84a3f18312\",\"style_index_js\":\"7e039c6467f810b4fa05\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_rtc_hub_settings:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_rtc_hub_settings:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab_rtc_hub_settings\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult.catch(handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_rtc_hub_settings\", \"0.1.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,1,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,19,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,1,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,4,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,1,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,1,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,1,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory).catch(onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_rtc_hub_settings\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkIds[i]] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_rtc_hub_settings\"] = self[\"webpackChunkjupyterlab_rtc_hub_settings\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_rtc_hub_settings\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_rtc_hub_settings\", \"0.1.2\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,37,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,6,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_rtc_hub_settings\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_rtc_hub_settings\"] = self[\"webpackChunkjupyterlab_rtc_hub_settings\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_rtc_hub_settings\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -54,14 +54,32 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (___CSS_LOADER_EXPORT___);
 
 
                 /***/
             }),
 
         /***/
+        "./style/index.js":
+            /*!************************!*\
+              !*** ./style/index.js ***!
+              \************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                "use strict";
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony import */
+                var _base_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ./base.css */ "./style/base.css");
+
+
+
+                /***/
+            }),
+
+        /***/
         "./style/base.css":
             /*!************************!*\
               !*** ./style/base.css ***!
               \************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -104,30 +122,12 @@
               \************************************/
             /***/
             ((module) => {
 
                 module.exports = "data:image/svg+xml,%3Csvg viewBox='0 0 24 16' width='16' version='1.1' id='svg243' sodipodi:docname='sharing_settings.svg' height='16' inkscape:version='1.1 (c68e22c387, 2021-05-23)' xmlns:inkscape='http://www.inkscape.org/namespaces/inkscape' xmlns:sodipodi='http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd' xmlns='http://www.w3.org/2000/svg' xmlns:svg='http://www.w3.org/2000/svg'%3E %3Cdefs id='defs247' /%3E %3Csodipodi:namedview id='namedview245' pagecolor='%23ffffff' bordercolor='%23666666' borderopacity='1.0' inkscape:pageshadow='2' inkscape:pageopacity='0.0' inkscape:pagecheckerboard='0' showgrid='false' height='16px' inkscape:zoom='51.442018' inkscape:cx='10.9638' inkscape:cy='10.458377' inkscape:window-width='3840' inkscape:window-height='2054' inkscape:window-x='-11' inkscape:window-y='-11' inkscape:window-maximized='1' inkscape:current-layer='svg243' /%3E %3Cg id='g42423' transform='matrix(0.15141914,0,0,0.15141914,31.40988,1.4890104)'%3E %3Cg id='g18813' transform='matrix(0.30905661,0,0,0.30905661,-154.34385,-14.050415)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571' /%3E %3C/g%3E %3Cg id='g18813-52' transform='matrix(0.30905661,0,0,0.30905661,-29.821718,-11.794773)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-29' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-9' /%3E %3C/g%3E %3Cg id='g18813-5' transform='translate(-11.475638,11.106735)' style='fill:%23616161;fill-opacity:1'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-2' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-5' /%3E %3C/g%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -191.05005,16.994511 20.76124,33.357944' id='path19015' /%3E %3Cpath style='fill:none;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -83.044958,49.885911 15.1627,-31.725039' id='path19017' /%3E %3C/g%3E %3C/svg%3E"
 
                 /***/
-            }),
-
-        /***/
-        "./style/index.js":
-            /*!************************!*\
-              !*** ./style/index.js ***!
-              \************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                "use strict";
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony import */
-                var _base_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ./base.css */ "./style/base.css");
-
-
-
-                /***/
             })
 
     }
 ]);
-//# sourceMappingURL=style_index_js.ed36e06a9ec9cea697a5.js.map
+//# sourceMappingURL=style_index_js.7e039c6467f810b4fa05.js.map
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js.map` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.780952380952381%*

 * *Differences: {"'file'": "'style_index_js.7e039c6467f810b4fa05.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;AAAA;AACsH;AAC7B;AACO;AAC7B;AACnE,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,yCAAyC,sFAA+B,CAAC,8DAA6B;AACtG;AACA,iFAAiF,wEAAwE,GAAG,8CAA8C,0CAA0C,sCAAsC,yCAAyC,qBAAqB,GAAG,oDAAoD,yBAAyB,kBAAkB,GAAG,wDAAwD,uBAAuB,8BAA8B,kBAAkB,iBAAiB,4BAA4B,GAAG,sCAAsC,0EAA0E,oBAAoB,0BAA0B,qBAAqB,yCAAyC,uBAAuB,0BAA0B,kBAAkB,wBAAwB,gCAAgC,GAAG,sCAAsC,qBAAqB,GAAG,OAAO,iFAAiF,YAAY,OAAO,KAAK,YAAY,aAAa,aAAa,WAAW,OAAO,KAAK,YAAY,WAAW,MAAM,KAAK,YAAY,a […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "style_index_js.ed36e06a9ec9cea697a5.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAA;AACsH;AAC7B;AACO;AAC7B;AACnE,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,yCAAyC,sFAA+B,CAAC,8DAA6B;AACtG;AACA,iFAAiF,wEAAwE,GAAG,8CAA8C,0CAA0C,sCAAsC,yCAAyC,qBAAqB,GAAG,oDAAoD,yBAAyB,kBAAkB,GAAG,wDAAwD,uBAAuB,8BAA8B,kBAAkB,iBAAiB,4BAA4B,GAAG,sCAAsC,0EAA0E,oBAAoB,0BAA0B,qBAAqB,yCAAyC,uBAAuB,0BAA0B,kBAAkB,wBAAwB,gCAAgC,GAAG,sCAAsC,qBAAqB,GAAG,OAAO,iFAAiF,YAAY,OAAO,KAAK,YAAY,aAAa,aAAa,WAAW,OAAO,KAAK,YAAY,WAAW,MAAM,KAAK,YAAY,aAAa,WAAW,UAAU,YAAY,OAAO,KAAK,YAAY,WAAW,YAAY,WAAW,YAAY,aAAa,aAAa,WAAW,YAAY,aAAa,OAAO,KAAK,UAAU,iEAAiE,kDAAkD,GAAG,8CAA8C,0CAA0C,sCAAsC,yCAAyC,qBAAqB,GAAG,oDAAoD,yBAAyB,kBAAkB,GAAG,wDAAwD,uBAAuB,8BAA8B,kBAAkB,iBAAiB,4BAA4B,GAAG,sCAAsC,0EAA0E,oBAAoB,0BAA0B,qBAAqB,yCAAyC,uBAAuB,0BAA0B,kBAAkB,wBAAwB,gCAAgC,GAAG,sCAAsC,qBAAqB,GAAG,mBAAmB;AACx5E;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;ACVkD;AACzF,YAAsF;;AAEtF;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,4FAAc,MAAM;;;;;;;;;;ACZnC,4kCAA4kC,eAAe,y1DAAy1D,eAAe,6KAA6K,eAAe,41DAA41D,eAAe,2IAA2I,iDAAiD,eAAe,21DAA21D,eAAe,oFAAoF,eAAe,iBAAiB,mBAAmB,oBAAoB,sBAAsB,6GAA6G,iBAAiB,mBAAmB,oBAAoB,sBAAsB;;;;;;;;;;;;;ACAv3O",
+    "file": "style_index_js.7e039c6467f810b4fa05.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAA;AACsH;AAC7B;AACO;AAC7B;AACnE,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,yCAAyC,sFAA+B,CAAC,8DAA6B;AACtG;AACA,iFAAiF,wEAAwE,GAAG,8CAA8C,0CAA0C,sCAAsC,yCAAyC,qBAAqB,GAAG,oDAAoD,yBAAyB,kBAAkB,GAAG,wDAAwD,uBAAuB,8BAA8B,kBAAkB,iBAAiB,4BAA4B,GAAG,sCAAsC,0EAA0E,oBAAoB,0BAA0B,qBAAqB,yCAAyC,uBAAuB,0BAA0B,kBAAkB,wBAAwB,gCAAgC,GAAG,sCAAsC,qBAAqB,GAAG,OAAO,iFAAiF,YAAY,OAAO,KAAK,YAAY,aAAa,aAAa,WAAW,OAAO,KAAK,YAAY,WAAW,MAAM,KAAK,YAAY,aAAa,WAAW,UAAU,YAAY,OAAO,KAAK,YAAY,WAAW,YAAY,WAAW,YAAY,aAAa,aAAa,WAAW,YAAY,aAAa,OAAO,KAAK,UAAU,iEAAiE,kDAAkD,GAAG,8CAA8C,0CAA0C,sCAAsC,yCAAyC,qBAAqB,GAAG,oDAAoD,yBAAyB,kBAAkB,GAAG,wDAAwD,uBAAuB,8BAA8B,kBAAkB,iBAAiB,4BAA4B,GAAG,sCAAsC,0EAA0E,oBAAoB,0BAA0B,qBAAqB,yCAAyC,uBAAuB,0BAA0B,kBAAkB,wBAAwB,gCAAgC,GAAG,sCAAsC,qBAAqB,GAAG,mBAAmB;AACx5E;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;ACVnB;;;;;;;;;;;;;;;;;;;ACAqE;AACzF,YAAsF;;AAEtF;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,qFAAO,aAAa;;;;;;;;;;ACZnC,4kCAA4kC,eAAe,y1DAAy1D,eAAe,6KAA6K,eAAe,41DAA41D,eAAe,2IAA2I,iDAAiD,eAAe,21DAA21D,eAAe,oFAAoF,eAAe,iBAAiB,mBAAmB,oBAAoB,sBAAsB,6GAA6G,iBAAiB,mBAAmB,oBAAoB,sBAAsB",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_rtc_hub_settings/./style/base.css",
-        "webpack://jupyterlab_rtc_hub_settings/./style/base.css?c30b",
-        "webpack://jupyterlab_rtc_hub_settings/./style/sharing_settings.svg",
-        "webpack://jupyterlab_rtc_hub_settings/./style/index.js"
+        "webpack://jupyterlab_rtc_hub_settings/./style/index.js",
+        "webpack://jupyterlab_rtc_hub_settings/./style/base.css?1944",
+        "webpack://jupyterlab_rtc_hub_settings/./style/sharing_settings.svg"
     ],
     "sourcesContent": [
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nimport ___CSS_LOADER_GET_URL_IMPORT___ from \"../node_modules/css-loader/dist/runtime/getUrl.js\";\nimport ___CSS_LOADER_URL_IMPORT_0___ from \"./sharing_settings.svg\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\nvar ___CSS_LOADER_URL_REPLACEMENT_0___ = ___CSS_LOADER_GET_URL_IMPORT___(___CSS_LOADER_URL_IMPORT_0___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \".rtc-hub-settings-SharingSettingsLogo {\\n    background-image: url(\" + ___CSS_LOADER_URL_REPLACEMENT_0___ + \");\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar {\\n    background: var(--jp-layout-color1);\\n    color: var(--jp-ui-font-color1);\\n    font-size: var(--jp-ui-font-size1);\\n    overflow: auto;\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar-table {\\n    table-layout: auto;\\n    width: 100%;\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar-table-div {\\n    display: inherit;\\n    justify-content: center;\\n    margin: 8px;\\n    padding: 0;\\n    list-style-type: none;\\n}\\n\\n.rtc-hub-settings-Toolbar-layout {\\n    border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\\n    display: flex;\\n    align-items: center;\\n    flex: 0 0 auto;\\n    font-size: var(--jp-ui-font-size0);\\n    font-weight: 600;\\n    letter-spacing: 1px;\\n    margin: 0px;\\n    padding: 8px 12px;\\n    text-transform: uppercase;\\n}\\n\\n.rtc-hub-settings-Toolbar-spacer {\\n    flex: 1 1 auto;\\n}\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;IACI,yDAA2C;AAC/C;;AAEA;IACI,mCAAmC;IACnC,+BAA+B;IAC/B,kCAAkC;IAClC,cAAc;AAClB;;AAEA;IACI,kBAAkB;IAClB,WAAW;AACf;;AAEA;IACI,gBAAgB;IAChB,uBAAuB;IACvB,WAAW;IACX,UAAU;IACV,qBAAqB;AACzB;;AAEA;IACI,mEAAmE;IACnE,aAAa;IACb,mBAAmB;IACnB,cAAc;IACd,kCAAkC;IAClC,gBAAgB;IAChB,mBAAmB;IACnB,WAAW;IACX,iBAAiB;IACjB,yBAAyB;AAC7B;;AAEA;IACI,cAAc;AAClB\",\"sourcesContent\":[\".rtc-hub-settings-SharingSettingsLogo {\\n    background-image: url(sharing_settings.svg);\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar {\\n    background: var(--jp-layout-color1);\\n    color: var(--jp-ui-font-color1);\\n    font-size: var(--jp-ui-font-size1);\\n    overflow: auto;\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar-table {\\n    table-layout: auto;\\n    width: 100%;\\n}\\n\\n.rtc-hub-settings-SharingSettingsSidebar-table-div {\\n    display: inherit;\\n    justify-content: center;\\n    margin: 8px;\\n    padding: 0;\\n    list-style-type: none;\\n}\\n\\n.rtc-hub-settings-Toolbar-layout {\\n    border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\\n    display: flex;\\n    align-items: center;\\n    flex: 0 0 auto;\\n    font-size: var(--jp-ui-font-size0);\\n    font-weight: 600;\\n    letter-spacing: 1px;\\n    margin: 0px;\\n    padding: 8px 12px;\\n    text-transform: uppercase;\\n}\\n\\n.rtc-hub-settings-Toolbar-spacer {\\n    flex: 1 1 auto;\\n}\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
+        "import './base.css';\n",
         "import api from \"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n            import content from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nexport default content.locals || {};",
-        "module.exports = \"data:image/svg+xml,%3Csvg viewBox='0 0 24 16' width='16' version='1.1' id='svg243' sodipodi:docname='sharing_settings.svg' height='16' inkscape:version='1.1 (c68e22c387, 2021-05-23)' xmlns:inkscape='http://www.inkscape.org/namespaces/inkscape' xmlns:sodipodi='http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd' xmlns='http://www.w3.org/2000/svg' xmlns:svg='http://www.w3.org/2000/svg'%3E %3Cdefs id='defs247' /%3E %3Csodipodi:namedview id='namedview245' pagecolor='%23ffffff' bordercolor='%23666666' borderopacity='1.0' inkscape:pageshadow='2' inkscape:pageopacity='0.0' inkscape:pagecheckerboard='0' showgrid='false' height='16px' inkscape:zoom='51.442018' inkscape:cx='10.9638' inkscape:cy='10.458377' inkscape:window-width='3840' inkscape:window-height='2054' inkscape:window-x='-11' inkscape:window-y='-11' inkscape:window-maximized='1' inkscape:current-layer='svg243' /%3E %3Cg id='g42423' transform='matrix(0.15141914,0,0,0.15141914,31.40988,1.4890104)'%3E %3Cg id='g18813' transform='matrix(0.30905661,0,0,0.30905661,-154.34385,-14.050415)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571' /%3E %3C/g%3E %3Cg id='g18813-52' transform='matrix(0.30905661,0,0,0.30905661,-29.821718,-11.794773)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-29' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-9' /%3E %3C/g%3E %3Cg id='g18813-5' transform='translate(-11.475638,11.106735)' style='fill:%23616161;fill-opacity:1'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-2' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-5' /%3E %3C/g%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -191.05005,16.994511 20.76124,33.357944' id='path19015' /%3E %3Cpath style='fill:none;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -83.044958,49.885911 15.1627,-31.725039' id='path19017' /%3E %3C/g%3E %3C/svg%3E\"",
-        "import './base.css';\n"
+        "module.exports = \"data:image/svg+xml,%3Csvg viewBox='0 0 24 16' width='16' version='1.1' id='svg243' sodipodi:docname='sharing_settings.svg' height='16' inkscape:version='1.1 (c68e22c387, 2021-05-23)' xmlns:inkscape='http://www.inkscape.org/namespaces/inkscape' xmlns:sodipodi='http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd' xmlns='http://www.w3.org/2000/svg' xmlns:svg='http://www.w3.org/2000/svg'%3E %3Cdefs id='defs247' /%3E %3Csodipodi:namedview id='namedview245' pagecolor='%23ffffff' bordercolor='%23666666' borderopacity='1.0' inkscape:pageshadow='2' inkscape:pageopacity='0.0' inkscape:pagecheckerboard='0' showgrid='false' height='16px' inkscape:zoom='51.442018' inkscape:cx='10.9638' inkscape:cy='10.458377' inkscape:window-width='3840' inkscape:window-height='2054' inkscape:window-x='-11' inkscape:window-y='-11' inkscape:window-maximized='1' inkscape:current-layer='svg243' /%3E %3Cg id='g42423' transform='matrix(0.15141914,0,0,0.15141914,31.40988,1.4890104)'%3E %3Cg id='g18813' transform='matrix(0.30905661,0,0,0.30905661,-154.34385,-14.050415)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571' /%3E %3C/g%3E %3Cg id='g18813-52' transform='matrix(0.30905661,0,0,0.30905661,-29.821718,-11.794773)'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-29' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-9' /%3E %3C/g%3E %3Cg id='g18813-5' transform='translate(-11.475638,11.106735)' style='fill:%23616161;fill-opacity:1'%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke-width:0.136607' d='m -152.74343,85.507535 c -3.9646,-0.5108 -7.3883,-1.94708 -10.21009,-4.28326 -1.68085,-1.39158 -2.6095,-2.86369 -3.50131,-5.55032 -1.01914,-3.07022 -1.55441,-6.35612 -1.55771,-9.56248 -0.002,-1.63966 0.0605,-2.20483 0.43583,-3.9616 1.54896,-7.24965 3.74526,-12.5369 6.97978,-16.80265 3.9386,-5.19433 9.18113,-7.91784 16.05223,-8.33919 l 1.50268,-0.0922 0.89638,0.47845 c 0.49301,0.26314 2.52162,1.51949 4.50803,2.79188 1.9864,1.27239 4.13416,2.59493 4.7728,2.93897 3.51388,1.89298 8.87329,3.58979 12.84105,4.06552 2.88028,0.34535 7.49885,0.12355 10.31382,-0.49529 2.64839,-0.58222 6.1313,-1.7882 8.67453,-3.00361 1.755129,-0.83877 2.318289,-1.17499 6.673349,-3.98409 1.6793,-1.08318 3.45559,-2.15768 3.94732,-2.38779 l 0.89406,-0.41838 1.88684,0.15351 c 6.1788,0.50272 10.98673,2.89504 14.69314,7.31098 3.74824,4.46577 6.36133,10.59169 7.89224,18.50192 0.38201,1.9738 0.44015,3.56407 0.21097,5.77074 -0.40183,3.86917 -1.25041,7.05164 -2.56797,9.63079 -1.8999,3.71907 -7.1675,6.63901 -13.16768,7.29913 -2.08493,0.22938 -70.364389,0.17159 -72.170289,-0.0611 z' id='path4534-2' sodipodi:nodetypes='csssssccsssssssscsssssscc' /%3E %3Cpath d='m -120.22697,35.758707 c -6.47585,-0.71586 -11.8904,-3.26265 -16.61861,-7.816731 -5.10218,-4.914279 -7.94324,-10.482973 -8.79634,-17.241507 -0.23731,-1.8800413 -0.19877,-5.8753663 0.0752,-7.7896883 0.92949,-6.495862 3.68984,-11.8283838 8.55477,-16.5263387 4.56157,-4.404999 9.38338,-6.837846 15.48727,-7.814106 2.33162,-0.372921 7.20834,-0.331692 9.54935,0.08073 6.25478,1.101923 11.17745,3.772188 15.791226,8.56583 4.83966,5.0283254 7.420269,10.8171197 7.92729,17.7824117 0.37886,5.2045923 -0.53847,10.0921053 -2.74183,14.6083893 -1.562891,3.203509 -3.2345,5.470869 -6.02274,8.169219 -4.473806,4.329561 -9.487516,6.87498 -15.350636,7.793361 -1.64061,0.25698 -6.23723,0.367249 -7.85489,0.18843 z' style='fill:%23616161;fill-opacity:1;stroke-width:0.204911' id='path18571-5' /%3E %3C/g%3E %3Cpath style='fill:%23616161;fill-opacity:1;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -191.05005,16.994511 20.76124,33.357944' id='path19015' /%3E %3Cpath style='fill:none;stroke:%23616161;stroke-width:1.5px;stroke-linecap:butt;stroke-linejoin:miter;stroke-opacity:1' d='m -83.044958,49.885911 15.1627,-31.725039' id='path19017' /%3E %3C/g%3E %3C/svg%3E\""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 "use strict";
 (self["webpackChunkjupyterlab_rtc_hub_settings"] = self["webpackChunkjupyterlab_rtc_hub_settings"] || []).push([
-    ["vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda"], {
+    ["vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f"], {
 
         /***/
         "./node_modules/css-loader/dist/runtime/api.js":
             /*!*****************************************************!*\
               !*** ./node_modules/css-loader/dist/runtime/api.js ***!
               \*****************************************************/
             /***/
@@ -497,8 +497,8 @@
                 };
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js.map
+//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js.map
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js.map` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js",
+    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js",
     "mappings": ";;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;;AAEjB;AACA;AACA;;AAEA;AACA,4CAA4C,qBAAqB;AACjE;;AAEA;AACA,KAAK;AACL,KAAK;AACL;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA,sBAAsB,iBAAiB;AACvC;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA,qBAAqB,qBAAqB;AAC1C;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;;;;;;;;;ACjEa;;AAEb,kCAAkC;;AAElC,8BAA8B;;AAE9B,kDAAkD,gBAAgB,gEAAgE,wDAAwD,6DAA6D,sDAAsD;;AAE7S,uCAAuC,uDAAuD,uCAAuC,SAAS,OAAO,oBAAoB;;AAEzK,yCAAyC,8FAA8F,wBAAwB,eAAe,eAAe,gBAAgB,YAAY,MAAM,wBAAwB,+BAA+B,aAAa,qBAAqB,uCAAuC,cAAc,WAAW,YAAY,UAAU,MAAM,mDAAmD,UAAU,sBAAsB;;AAEve,gCAAgC;;AAEhC;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA,KAAK;AACL;AACA;;AAEA;AACA;;;;;;;;;;ACnCa;;AAEb;AACA;AACA;AACA;AACA,IAAI;;;AAGJ;;AAEA;AACA;AACA,IAAI;;;AAGJ;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,IAAI;AACJ;;;AAGA;AACA;AACA;;AAEA;AACA;;;;;;;;;;ACjCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;AACA;AACA;AACA;AACA,wDAAwD;;AAExD;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;;AAEA;AACA;;AAEA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA,OAAO;AACP;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA,gBAAgB,KAAwC,GAAG,sBAAiB,GAAG,CAAI;;AAEnF;AACA;AACA;AACA;;AAEA;AACA;AACA,GAAG;;AAEH;AACA;AACA,IAAI;AACJ;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;;AAED;AACA,qEAAqE,qBAAqB,cAAc;;AAExG;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA,yDAAyD;AACzD,IAAI;;AAEJ;;;AAGA;AACA;AACA,IAAI;AACJ;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA,2BAA2B;AAC3B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;;AAEA;;AAEA,qBAAqB,6BAA6B;AAClD;;AAEA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_rtc_hub_settings/./node_modules/css-loader/dist/runtime/api.js",
         "webpack://jupyterlab_rtc_hub_settings/./node_modules/css-loader/dist/runtime/cssWithMappingToString.js",
         "webpack://jupyterlab_rtc_hub_settings/./node_modules/css-loader/dist/runtime/getUrl.js",
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/PKG-INFO` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-rtc-hub-settings
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension to manage real time collaboration settings on JupyterHub
 Home-page: https://github.com/LabShare/jupyterlab-extensions
 Author: Konstantin Taletskiy
 Author-email: konstantin.taletskiy@labshare.org
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -146,9 +146,7 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_rtc_hub_settings` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
-
-
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/jupyterlab_rtc_hub_settings.egg-info/SOURCES.txt` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 jupyterlab_rtc_hub_settings.egg-info/SOURCES.txt
 jupyterlab_rtc_hub_settings.egg-info/dependency_links.txt
 jupyterlab_rtc_hub_settings.egg-info/not-zip-safe
 jupyterlab_rtc_hub_settings.egg-info/requires.txt
 jupyterlab_rtc_hub_settings.egg-info/top_level.txt
 jupyterlab_rtc_hub_settings/labextension/build_log.json
 jupyterlab_rtc_hub_settings/labextension/package.json
-jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js
-jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.de2dc6ad8eda78818ec6.js.map
-jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js
-jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.4ea8b094493f59bbfe18.js.map
+jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js
+jupyterlab_rtc_hub_settings/labextension/static/lib_index_js.aa27acd2f9d9b6c528e8.js.map
+jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js
+jupyterlab_rtc_hub_settings/labextension/static/remoteEntry.5df98682aa24d1bcf559.js.map
 jupyterlab_rtc_hub_settings/labextension/static/style.js
-jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js
-jupyterlab_rtc_hub_settings/labextension/static/style_index_js.ed36e06a9ec9cea697a5.js.map
-jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js
-jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-313cda.e45f95686c6bc860f917.js.map
+jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js
+jupyterlab_rtc_hub_settings/labextension/static/style_index_js.7e039c6467f810b4fa05.js.map
+jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js
+jupyterlab_rtc_hub_settings/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-7d5e6f.7b993b2d1f84a3f18312.js.map
 src/handler.ts
 src/index.ts
 src/sidebar.tsx
 src/tableWidget.tsx
 src/toolbarWidget.ts
 src/types.ts
 style/base.css
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/package.json` & `jupyterlab_rtc_hub_settings-0.1.2/jupyterlab_rtc_hub_settings/labextension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9551136363636363%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.4', '@jupyterlab/coreutils': '^5.6.5', "*

 * *                   "'@jupyterlab/services': '^6.6.5'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.5'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.5df98682aa24d1bcf559.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -3,21 +3,21 @@
         "email": "konstantin.taletskiy@labshare.org",
         "name": "Konstantin Taletskiy"
     },
     "bugs": {
         "url": "https://github.com/LabShare/jupyterlab-extensions/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/services": "^6.1.0"
+        "@jupyterlab/application": "^3.6.4",
+        "@jupyterlab/coreutils": "^5.6.5",
+        "@jupyterlab/services": "^6.6.5"
     },
     "description": "A JupyterLab extension to manage real time collaboration settings on JupyterHub",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
+        "@jupyterlab/builder": "^3.6.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
@@ -35,14 +35,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.5df98682aa24d1bcf559.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_rtc_hub_settings"
                 },
                 "managers": [
                     "pip"
@@ -84,9 +89,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/pyproject.toml` & `jupyterlab_rtc_hub_settings-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["jupyter_packaging~=0.10,<2", "jupyterlab~=3.1"]
+requires = ["jupyter_packaging~=0.10,<2", "jupyterlab~=3.6"]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["jupyterlab_rtc_hub_settings/labextension/static/style.js"]
 ensured-targets = ["jupyterlab_rtc_hub_settings/labextension/static/style.js", "jupyterlab_rtc_hub_settings/labextension/package.json"]
 
 [tool.jupyter-packaging.builder]
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/setup.py` & `jupyterlab_rtc_hub_settings-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     author_email=pkg_json["author"]["email"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        "jupyter_server>=1.6,<2",
+        "jupyter_server>=1.6,<3",
         "escapism"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/src/handler.ts` & `jupyterlab_rtc_hub_settings-0.1.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/src/index.ts` & `jupyterlab_rtc_hub_settings-0.1.2/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-import { JupyterFrontEnd, JupyterFrontEndPlugin, ILabShell } from '@jupyterlab/application';
+import {
+  JupyterFrontEnd,
+  JupyterFrontEndPlugin,
+  ILabShell
+} from '@jupyterlab/application';
 import { SharingSettingsSidebar } from './sidebar';
 
 /**
  * Initialization data for the jupyterlab_rtc_hub_settings extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab_rtc_hub_settings:plugin',
   autoStart: true,
   requires: [ILabShell],
-  activate: (
-    app: JupyterFrontEnd,
-    labShell: ILabShell
-  ) => {
-    console.log('JupyterLab extension jupyterlab_rtc_hub_settings is activated!');
+  activate: (app: JupyterFrontEnd, labShell: ILabShell) => {
+    console.log(
+      'JupyterLab extension jupyterlab_rtc_hub_settings is activated!'
+    );
 
     // Create the sharing settings sidebar panel
     const sidebar = new SharingSettingsSidebar();
     sidebar.id = 'rtc-hub-settings-labextension:plugin';
-    sidebar.title.iconClass = 'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';
+    sidebar.title.iconClass =
+      'rtc-hub-settings-SharingSettingsLogo jp-SideBar-tabIcon';
     sidebar.title.caption = 'Sharing settings';
 
     // Register sidebar panel with JupyterLab
     labShell.add(sidebar, 'left', { rank: 600 });
-
   }
 };
 
 export default plugin;
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/src/sidebar.tsx` & `jupyterlab_rtc_hub_settings-0.1.2/src/sidebar.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import { Widget, PanelLayout } from '@lumino/widgets';
 import { requestAPI } from './handler';
 import { IUserStatus } from './types';
-import { UsersTableWidget } from './tableWidget'
-import { ToolbarWidget } from './toolbarWidget'
+import { UsersTableWidget } from './tableWidget';
+import { ToolbarWidget } from './toolbarWidget';
 import { ReactWidget, UseSignal } from '@jupyterlab/apputils';
 import { Signal } from '@lumino/signaling';
 
-
 import React from 'react';
 
 /**
  * Sidebar widget for displaying RTC sharing settings.
  */
 export class SharingSettingsSidebar extends Widget {
-    constructor() {
-        super();
+  constructor() {
+    super();
 
-        this.addClass('rtc-hub-settings-SharingSettingsSidebar');
+    this.addClass('rtc-hub-settings-SharingSettingsSidebar');
 
-        // Define widget layout
-        let layout = (this.layout = new PanelLayout());
+    // Define widget layout
+    const layout = (this.layout = new PanelLayout());
 
-        // Add Toolbar widget
-        let toolbar = new ToolbarWidget(() => { this._getUsers() });
-        layout.addWidget(toolbar);
-
-        // Add Users table widget
-        let table = ReactWidget.create(
-            <UseSignal signal={this._valueChanged} initialArgs={this._users}>
-                {(_, oa) => <UsersTableWidget
-                    ar={oa!}
-                    updateUsers={(arg0) => this._updateUsers(arg0)}
-                    refreshUsers={() => this._getUsers()}
-                ></UsersTableWidget>
-                }
-            </UseSignal>
-        )
-        table.addClass('rtc-hub-settings-SharingSettingsSidebar-table-div');
-        layout.addWidget(table);
-    }
-
-    private async _getUsers() {
-        // Return results of API request
-        requestAPI<IUserStatus[]>('users')
-            .then(response => {
-                // Update internal variable
-                this._users = response;
-
-                // Send signal for table widget to update data
-                this._valueChanged.emit(this._users);
-            })
-    }
-
-    private async _updateUsers(users: IUserStatus[]) {
-        // Send updated list of users statuses
-        requestAPI<IUserStatus[]>('users', {
-            method: 'POST',
-            body: JSON.stringify(users)
-        })
-            .then(response => {
-                // Update internal variable
-                this._users = response;
-
-                // Send signal for table widget to update data
-                this._valueChanged.emit(this._users);
-            })
-    }
-
-    private _users: IUserStatus[] = [];
-    private _valueChanged = new Signal<this, IUserStatus[]>(this);
-}
+    // Add Toolbar widget
+    const toolbar = new ToolbarWidget(() => {
+      this._getUsers();
+    });
+    layout.addWidget(toolbar);
+
+    // Add Users table widget
+    const table = ReactWidget.create(
+      <UseSignal signal={this._valueChanged} initialArgs={this._users}>
+        {(_, oa) => (
+          <UsersTableWidget
+            ar={oa === undefined ? [] : oa}
+            updateUsers={arg0 => this._updateUsers(arg0)}
+            refreshUsers={() => this._getUsers()}
+          ></UsersTableWidget>
+        )}
+      </UseSignal>
+    );
+    table.addClass('rtc-hub-settings-SharingSettingsSidebar-table-div');
+    layout.addWidget(table);
+  }
+
+  private async _getUsers() {
+    // Return results of API request
+    requestAPI<IUserStatus[]>('users').then(response => {
+      // Update internal variable
+      this._users = response;
+
+      // Send signal for table widget to update data
+      this._valueChanged.emit(this._users);
+    });
+  }
+
+  private async _updateUsers(users: IUserStatus[]) {
+    // Send updated list of users statuses
+    requestAPI<IUserStatus[]>('users', {
+      method: 'POST',
+      body: JSON.stringify(users)
+    }).then(response => {
+      // Update internal variable
+      this._users = response;
+
+      // Send signal for table widget to update data
+      this._valueChanged.emit(this._users);
+    });
+  }
+
+  private _users: IUserStatus[] = [];
+  private _valueChanged = new Signal<this, IUserStatus[]>(this);
+}
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/src/tableWidget.tsx` & `jupyterlab_rtc_hub_settings-0.1.2/src/tableWidget.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import React, { Component } from 'react';
-import {IUsersTableProps, IUserStatus} from './types'
+import { IUsersTableProps, IUserStatus } from './types';
 
 // Class for table of users
-export class UsersTableWidget extends Component<IUsersTableProps, IUsersTableProps> {
-    constructor(
-        props: IUsersTableProps,
-    ) {
-        super(props);
-        props.refreshUsers();
-    }
+export class UsersTableWidget extends Component<
+  IUsersTableProps,
+  IUsersTableProps
+> {
+  constructor(props: IUsersTableProps) {
+    super(props);
+    props.refreshUsers();
+  }
 
-    updateUser = (name: string) => {
-        let props: IUsersTableProps = this.props;
-        let index = props.ar.findIndex((user: IUserStatus) => (user.name==name));
-        props.ar[index].shared = !props.ar[index].shared;
-        props.updateUsers(props.ar);
-    }
-        
+  updateUser = (name: string): void => {
+    const props: IUsersTableProps = this.props;
+    const index = props.ar.findIndex((user: IUserStatus) => user.name === name);
+    props.ar[index].shared = !props.ar[index].shared;
+    props.updateUsers(props.ar);
+  };
 
-    render() {
-        const tableRows = this.props.ar.map((user: IUserStatus) => {
-            return (
-                <tr>
-                    <td>{user.name}</td>
-                    <td><input type="checkbox" checked={user.shared} onChange={() => this.updateUser(user.name)}></input>
-                    </td>
-                </tr>
-            )
-        });
+  render(): JSX.Element {
+    const tableRows = this.props.ar.map((user: IUserStatus) => {
+      return (
+        <tr>
+          <td>{user.name}</td>
+          <td>
+            <input
+              type="checkbox"
+              checked={user.shared}
+              onChange={() => this.updateUser(user.name)}
+            ></input>
+          </td>
+        </tr>
+      );
+    });
 
-
-        // Assemble headers and rows in the full table
-        return (
-            <div>
-                <table className='rtc-hub-settings-SharingSettingsSidebar-table'>
-                    <tbody>
-                        {tableRows}
-                    </tbody>
-                </table>
-            </div>
-        );
-    }
-};
+    // Assemble headers and rows in the full table
+    return (
+      <div>
+        <table className="rtc-hub-settings-SharingSettingsSidebar-table">
+          <tbody>{tableRows}</tbody>
+        </table>
+      </div>
+    );
+  }
+}
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/src/toolbarWidget.ts` & `jupyterlab_rtc_hub_settings-0.1.2/src/toolbarWidget.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import { refreshIcon } from '@jupyterlab/ui-components';
 import { PanelLayout, Widget } from '@lumino/widgets';
 import { ToolbarButton } from '@jupyterlab/apputils';
 
 export class ToolbarWidget extends Widget {
-    constructor(
-        refresh: () => void
-    ) {
-        super();
-        this.addClass('rtc-hub-settings-Toolbar-layout');
+  constructor(refresh: () => void) {
+    super();
+    this.addClass('rtc-hub-settings-Toolbar-layout');
 
-        const layout = (this.layout = new PanelLayout());
+    const layout = (this.layout = new PanelLayout());
 
-        const header = new Widget({ node: document.createElement('div') });
-        header.node.textContent = 'Collaboration Sharing';
-        layout.addWidget(header);
+    const header = new Widget({ node: document.createElement('div') });
+    header.node.textContent = 'Collaboration Sharing';
+    layout.addWidget(header);
 
-        const spacer = new Widget({ node: document.createElement('span') });
-        spacer.addClass('rtc-hub-settings-Toolbar-spacer');
-        layout.addWidget(spacer);
+    const spacer = new Widget({ node: document.createElement('span') });
+    spacer.addClass('rtc-hub-settings-Toolbar-spacer');
+    layout.addWidget(spacer);
 
-        // Search button
-        const refreshButton = new ToolbarButton({
-            icon: refreshIcon,
-            onClick: refresh
-        });
-        layout.addWidget(refreshButton);
-    }
-}
+    // Search button
+    const refreshButton = new ToolbarButton({
+      icon: refreshIcon,
+      onClick: refresh
+    });
+    layout.addWidget(refreshButton);
+  }
+}
```

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/style/base.css` & `jupyterlab_rtc_hub_settings-0.1.2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/style/sharing_settings.svg` & `jupyterlab_rtc_hub_settings-0.1.2/style/sharing_settings.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_rtc_hub_settings-0.1.1/tsconfig.json` & `jupyterlab_rtc_hub_settings-0.1.2/tsconfig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "es2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

