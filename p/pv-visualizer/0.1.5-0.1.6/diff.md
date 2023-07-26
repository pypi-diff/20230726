# Comparing `tmp/pv-visualizer-0.1.5.tar.gz` & `tmp/pv-visualizer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pv-visualizer-0.1.5.tar", last modified: Fri Jul 21 21:39:14 2023, max compression
+gzip compressed data, was "pv-visualizer-0.1.6.tar", last modified: Wed Jul 26 15:36:34 2023, max compression
```

## Comparing `pv-visualizer-0.1.5.tar` & `pv-visualizer-0.1.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      137 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3466 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2770 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer/
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer/app/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/assets/
--rw-r--r--   0 root         (0) root         (0)      201 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/database-remove-outline.svg
--rw-r--r--   0 root         (0) root         (0)      628 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/pv_logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/
--rw-r--r--   0 root         (0) root         (0)      778 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/const.py
--rw-r--r--   0 root         (0) root         (0)    14492 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/core.py
--rw-r--r--   0 root         (0) root         (0)     8236 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/data_informations.py
--rw-r--r--   0 root         (0) root         (0)    12162 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/decorators.py
--rw-r--r--   0 root         (0) root         (0)    12539 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/definitions.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domain_helpers.py
--rw-r--r--   0 root         (0) root         (0)     5290 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domains.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/paraview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/camera.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/representation.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/scalar_range.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/ui/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/algorithms.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/files.py
--rw-r--r--   0 root         (0) root         (0)     5083 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/main.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/settings.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/state_change.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/view_toolbox.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/html/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4366 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/data_information.py
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/file_browser.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/pv_visualizer/html/module/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   249207 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js
--rw-r--r--   0 root         (0) root         (0)   322614 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map
--rw-r--r--   0 root         (0) root         (0)   249609 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js
--rw-r--r--   0 root         (0) root         (0)   323178 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map
--rw-r--r--   0 root         (0) root         (0)    97976 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js
--rw-r--r--   0 root         (0) root         (0)   368476 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)     4356 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3975 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/proxy_editor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3466 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2122 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.807469 pv-visualizer-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-26 15:36:06.000000 pv-visualizer-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      137 2023-07-26 15:36:06.000000 pv-visualizer-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-07-26 15:36:34.807469 pv-visualizer-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2770 2023-07-26 15:36:06.000000 pv-visualizer-0.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.799469 pv-visualizer-0.1.6/pv_visualizer/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/assets/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/assets/database-remove-outline.svg
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/assets/pv_logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/engine/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/const.py
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/core.py
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/data_informations.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    12539 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/domain_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5290 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/domains.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/paraview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/camera.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/representation.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/scalar_range.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/app/ui/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/files.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/main.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/state_change.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/app/ui/view_toolbox.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/html/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/data_information.py
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/file_browser.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer/html/module/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.807469 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-26 15:36:29.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   249207 2023-07-26 15:36:30.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js
+-rw-r--r--   0 root         (0) root         (0)   322614 2023-07-26 15:36:30.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map
+-rw-r--r--   0 root         (0) root         (0)   249609 2023-07-26 15:36:29.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js
+-rw-r--r--   0 root         (0) root         (0)   323178 2023-07-26 15:36:29.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)    97976 2023-07-26 15:36:30.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)   368476 2023-07-26 15:36:30.000000 pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3975 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/pv_visualizer/html/proxy_editor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 15:36:34.803469 pv-visualizer-0.1.6/pv_visualizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-26 15:36:34.000000 pv-visualizer-0.1.6/pv_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 15:36:34.807469 pv-visualizer-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 15:36:07.000000 pv-visualizer-0.1.6/setup.py
```

### Comparing `pv-visualizer-0.1.5/LICENSE` & `pv-visualizer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/PKG-INFO` & `pv-visualizer-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-visualizer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web frontend to ParaView
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pv-visualizer-0.1.5/README.rst` & `pv-visualizer-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/assets/database-remove-outline.svg` & `pv-visualizer-0.1.6/pv_visualizer/app/assets/database-remove-outline.svg`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/assets/pv_logo.svg` & `pv-visualizer-0.1.6/pv_visualizer/app/assets/pv_logo.svg`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/__init__.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/const.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/const.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/core.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,21 +149,19 @@
             else:
                 property.SetUncheckedElement(0, value)
 
     @staticmethod
     def before_delete(simput_proxy):
         pv_proxy = simput_proxy.object
         logger.info(
-            "Deleting PV proxy",
+            "Deleting PV proxy: %s -> %s",
             simput_proxy.id,
             pv_proxy.GetGlobalIDAsString(),
-            pv_proxy.GetReferenceCount(),
         )
         simple.Delete(pv_proxy)
-        logger.info("simple.Delete() => done", pv_proxy.GetReferenceCount())
 
 
 # -----------------------------------------------------------------------------
 
 
 class PVObjectFactory:
     def __init__(self):
```

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/data_informations.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/data_informations.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/decorators.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/decorators.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/definitions.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/definitions.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domain_helpers.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/domain_helpers.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domains.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/proxymanager/domains.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/camera.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/camera.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/representation.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/representation.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/scalar_range.py` & `pv-visualizer-0.1.6/pv_visualizer/app/engine/reactions/scalar_range.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/jupyter.py` & `pv-visualizer-0.1.6/pv_visualizer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/main.py` & `pv-visualizer-0.1.6/pv_visualizer/app/main.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/algorithms.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/algorithms.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/files.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/files.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/main.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/main.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/pipeline.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/pipeline.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/settings.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/settings.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/state_change.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/state_change.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/app/ui/view_toolbox.py` & `pv-visualizer-0.1.6/pv_visualizer/app/ui/view_toolbox.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/data_information.py` & `pv-visualizer-0.1.6/pv_visualizer/html/data_information.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/file_browser.py` & `pv-visualizer-0.1.6/pv_visualizer/html/file_browser.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/filters.py` & `pv-visualizer-0.1.6/pv_visualizer/html/filters.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/__init__.py` & `pv-visualizer-0.1.6/pv_visualizer/html/module/__init__.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map` & `pv-visualizer-0.1.6/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/pipeline.py` & `pv-visualizer-0.1.6/pv_visualizer/html/pipeline.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer/html/proxy_editor.py` & `pv-visualizer-0.1.6/pv_visualizer/html/proxy_editor.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/pv_visualizer.egg-info/PKG-INFO` & `pv-visualizer-0.1.6/pv_visualizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-visualizer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web frontend to ParaView
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pv-visualizer-0.1.5/pv_visualizer.egg-info/SOURCES.txt` & `pv-visualizer-0.1.6/pv_visualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.5/setup.cfg` & `pv-visualizer-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pv-visualizer
-version = 0.1.5
+version = 0.1.6
 description = Web frontend to ParaView
 long_description = file: README.rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 1 - Planning
 	Environment :: Web Environment
```

