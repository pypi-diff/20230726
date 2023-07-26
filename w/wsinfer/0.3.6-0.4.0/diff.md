# Comparing `tmp/wsinfer-0.3.6.tar.gz` & `tmp/wsinfer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsinfer-0.3.6.tar", last modified: Fri Feb 24 18:04:49 2023, max compression
+gzip compressed data, was "wsinfer-0.4.0.tar", last modified: Wed Jul 26 00:36:27 2023, max compression
```

## Comparing `wsinfer-0.3.6.tar` & `wsinfer-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,85 @@
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.973441 wsinfer-0.3.6/
--rw-r--r--   0 jakub     (1000) jakub     (1000)    35149 2022-08-19 18:55:37.000000 wsinfer-0.3.6/LICENSE
--rw-r--r--   0 jakub     (1000) jakub     (1000)     3767 2023-02-24 18:04:49.973441 wsinfer-0.3.6/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)     2485 2023-02-24 16:24:34.000000 wsinfer-0.3.6/README.md
--rw-r--r--   0 jakub     (1000) jakub     (1000)     2346 2023-02-24 18:04:49.977440 wsinfer-0.3.6/setup.cfg
--rw-r--r--   0 jakub     (1000) jakub     (1000)      137 2022-08-26 00:53:07.000000 wsinfer-0.3.6/setup.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.965440 wsinfer-0.3.6/tests/
--rw-r--r--   0 jakub     (1000) jakub     (1000)    33724 2023-02-24 16:15:41.000000 wsinfer-0.3.6/tests/test_all.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    81295 2022-09-14 19:30:50.000000 wsinfer-0.3.6/versioneer.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.977440 wsinfer-0.3.6/wsinfer/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      541 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)       63 2023-01-23 02:27:11.000000 wsinfer-0.3.6/wsinfer/__main__.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer/_modellib/
--rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    11690 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/inceptionv4_no_batchnorm.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    11498 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/models.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     2679 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/resnet_preact.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    12963 2023-02-22 18:59:09.000000 wsinfer-0.3.6/wsinfer/_modellib/run_inference.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     2047 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/transforms.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)      615 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_modellib/vgg16mod.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer/_patchlib/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      970 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     2193 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/create_dense_patch_grid.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    15074 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_patchlib/create_patches_fp.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer/_patchlib/presets/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      213 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/presets/tcga.csv
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer/_patchlib/utils/
--rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/utils/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1248 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/utils/file_utils.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     6513 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_patchlib/utils/utils.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/
--rw-r--r--   0 jakub     (1000) jakub     (1000)    28986 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/WholeSlideImage.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     4049 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/batch_process_utils.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     5046 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/util_classes.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    14429 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/_patchlib/wsi_core/wsi_utils.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)      497 2023-02-24 18:04:49.977440 wsinfer-0.3.6/wsinfer/_version.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.973441 wsinfer-0.3.6/wsinfer/cli/
--rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2022-12-26 23:47:24.000000 wsinfer-0.3.6/wsinfer/cli/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)      578 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/cli/cli.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     4228 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/cli/convert_csv_to_geojson.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    15635 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/cli/convert_csv_to_sbubmi.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)    13534 2023-02-22 18:59:09.000000 wsinfer-0.3.6/wsinfer/cli/infer.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1007 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/cli/list_models_and_weights.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1834 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/cli/patch.py
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.973441 wsinfer-0.3.6/wsinfer/modeldefs/
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1066 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/modeldefs/inceptionv4_tcga-brca-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1320 2023-02-22 18:59:01.000000 wsinfer-0.3.6/wsinfer/modeldefs/inceptionv4nobn_tcga-tils-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1152 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/modeldefs/preactresnet34_tcga-paad-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1077 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/modeldefs/resnet34_tcga-brca-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1066 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/modeldefs/resnet34_tcga-luad-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1029 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/modeldefs/resnet34_tcga-prad-v1.yaml
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1324 2023-01-09 21:15:16.000000 wsinfer-0.3.6/wsinfer/modeldefs/vgg16mod_tcga-BRCA-v1.yaml
-drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-02-24 18:04:49.969440 wsinfer-0.3.6/wsinfer.egg-info/
--rw-r--r--   0 jakub     (1000) jakub     (1000)     3767 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1556 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/SOURCES.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)        1 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/dependency_links.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)       48 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/entry_points.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)      311 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/requires.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)        8 2023-02-24 18:04:49.000000 wsinfer-0.3.6/wsinfer.egg-info/top_level.txt
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3137 2023-06-29 12:27:33.000000 wsinfer-0.4.0/.dockerignore
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       33 2023-07-19 15:15:33.000000 wsinfer-0.4.0/.gitattributes
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.812525 wsinfer-0.4.0/.github/
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.816526 wsinfer-0.4.0/.github/workflows/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     6586 2023-07-24 13:42:44.000000 wsinfer-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3188 2023-07-23 16:18:11.000000 wsinfer-0.4.0/.gitignore
+-rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2023-07-19 15:15:33.000000 wsinfer-0.4.0/.gitmodules
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      647 2023-07-17 14:48:33.000000 wsinfer-0.4.0/.readthedocs.yaml
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.816526 wsinfer-0.4.0/.vscode/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      237 2023-06-29 12:27:33.000000 wsinfer-0.4.0/.vscode/settings.json
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      876 2023-07-24 13:42:44.000000 wsinfer-0.4.0/Dockerfile
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    11346 2023-07-19 15:15:33.000000 wsinfer-0.4.0/LICENSE
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3845 2023-07-26 00:36:27.828526 wsinfer-0.4.0/PKG-INFO
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     2294 2023-07-24 15:24:34.000000 wsinfer-0.4.0/README.md
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.820526 wsinfer-0.4.0/docs/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      634 2023-06-29 12:27:33.000000 wsinfer-0.4.0/docs/Makefile
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/docs/_static/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)   598112 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/_static/brca-heatmap.png
+-rw-r--r--   0 jakub     (1000) jakub     (1000)  1245650 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/_static/brca-tissue.png
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      263 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/_static/switcher.json
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      109 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/cli.rst
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4108 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/conf.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4717 2023-07-24 15:24:15.000000 wsinfer-0.4.0/docs/index.rst
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     2080 2023-07-24 13:42:44.000000 wsinfer-0.4.0/docs/installing.rst
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      800 2023-06-29 12:27:33.000000 wsinfer-0.4.0/docs/make.bat
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      159 2023-07-24 13:42:44.000000 wsinfer-0.4.0/docs/qupath_ext.rst
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     5535 2023-07-24 13:42:44.000000 wsinfer-0.4.0/docs/user_guide.rst
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3759 2023-07-26 00:34:33.000000 wsinfer-0.4.0/pyproject.toml
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/scripts/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3784 2023-06-29 12:27:33.000000 wsinfer-0.4.0/scripts/README.md
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    16619 2023-06-29 12:27:33.000000 wsinfer-0.4.0/scripts/convert_tf_to_pytorch_til_inceptionv4.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4463 2023-06-29 12:27:33.000000 wsinfer-0.4.0/scripts/convert_tf_to_pytorch_til_vgg16.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     2451 2023-06-29 12:27:33.000000 wsinfer-0.4.0/scripts/convert_to_torchscript.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       38 2023-07-26 00:36:27.828526 wsinfer-0.4.0/setup.cfg
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.816526 wsinfer-0.4.0/tests/reference/
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/breast-tumor-inception_v4.tcga-brca/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     7980 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/breast-tumor-inception_v4.tcga-brca/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/breast-tumor-resnet34.tcga-brca/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     7980 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/breast-tumor-resnet34.tcga-brca/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/breast-tumor-vgg16mod.tcga-brca/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     7980 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/breast-tumor-vgg16mod.tcga-brca/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/lung-tumor-resnet34.tcga-luad/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4779 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/lung-tumor-resnet34.tcga-luad/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/pancancer-lymphocytes-inceptionv4.tcga/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    17365 2023-07-19 15:15:33.000000 wsinfer-0.4.0/tests/reference/pancancer-lymphocytes-inceptionv4.tcga/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/pancreas-tumor-preactresnet34.tcga-paad/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      150 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/pancreas-tumor-preactresnet34.tcga-paad/purple.csv
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/tests/reference/prostate-tumor-resnet34.tcga-prad/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    11172 2023-07-17 14:48:33.000000 wsinfer-0.4.0/tests/reference/prostate-tumor-resnet34.tcga-prad/purple.csv
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    15289 2023-07-26 00:29:10.000000 wsinfer-0.4.0/tests/test_all.py
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.824526 wsinfer-0.4.0/wsinfer/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      700 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/__init__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       99 2023-07-23 17:44:12.000000 wsinfer-0.4.0/wsinfer/__main__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      160 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer/_version.py
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/wsinfer/cli/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       35 2023-07-17 14:48:33.000000 wsinfer-0.4.0/wsinfer/cli/__init__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1268 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/cli/cli.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4240 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/cli/convert_csv_to_geojson.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    15629 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/cli/convert_csv_to_sbubmi.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    13307 2023-07-24 21:06:37.000000 wsinfer-0.4.0/wsinfer/cli/infer.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3129 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/cli/patch.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      950 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/errors.py
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/wsinfer/modellib/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       35 2023-07-17 14:48:33.000000 wsinfer-0.4.0/wsinfer/modellib/__init__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4017 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/modellib/data.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     2734 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/modellib/models.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     7329 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/modellib/run_inference.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      829 2023-07-23 16:18:11.000000 wsinfer-0.4.0/wsinfer/modellib/transforms.py
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/wsinfer/patchlib/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)    13928 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/patchlib/__init__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     5535 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/patchlib/patch.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3003 2023-07-24 13:42:44.000000 wsinfer-0.4.0/wsinfer/patchlib/segment.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)        0 2023-07-19 15:15:33.000000 wsinfer-0.4.0/wsinfer/py.typed
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/wsinfer/schemas/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1725 2023-07-17 14:48:33.000000 wsinfer-0.4.0/wsinfer/schemas/model-config.schema.json
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     8623 2023-07-26 00:29:10.000000 wsinfer-0.4.0/wsinfer/wsi.py
+drwxr-sr-x   0 jakub     (1000) jakub     (1000)        0 2023-07-26 00:36:27.828526 wsinfer-0.4.0/wsinfer.egg-info/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     3845 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/PKG-INFO
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1697 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)        1 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       48 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/entry_points.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      506 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/requires.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)        8 2023-07-26 00:36:27.000000 wsinfer-0.4.0/wsinfer.egg-info/top_level.txt
```

### Comparing `wsinfer-0.3.6/PKG-INFO` & `wsinfer-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 Metadata-Version: 2.1
 Name: wsinfer
-Version: 0.3.6
+Version: 0.4.0
 Summary: Run patch-based classification on pathology whole slide images.
-Home-page: https://github.com/SBU-BMI/wsinfer
-Author: Jakub Kaczmarzyk
-Author-email: jakub.kaczmarzyk@stonybrookmedicine.edu
-License: GNU General Public License v3 (GPLv3)
+Author-email: Jakub Kaczmarzyk <jakub.kaczmarzyk@stonybrookmedicine.edu>
+Maintainer-email: Jakub Kaczmarzyk <jakub.kaczmarzyk@stonybrookmedicine.edu>
+License: Apache License, Version 2.0
+Project-URL: Homepage, https://wsinfer.readthedocs.io
+Project-URL: Documentation, https://wsinfer.readthedocs.io
+Project-URL: Repository, https://github.com/SBU-BMI/wsinfer
+Project-URL: Bug Tracker, https://github.com/SBU-BMI/wsinfer/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: openslide
 License-File: LICENSE
 
 # WSInfer: deep learning inference on whole slide images
 
 Original H&E                        |  Heatmap of Tumor Probability
 :----------------------------------:|:-----------------------------------:
-![](docs/images/brca-tissue.png)  | ![](docs/images/brca-heatmap.png)
+![](docs/_static/brca-tissue.png)  | ![](docs/_static/brca-heatmap.png)
 
 🔥 🚀 Blazingly fast pipeline to run patch-based classification models on whole slide images.
 
 [![Continuous Integration](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml/badge.svg)](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/wsinfer/badge/?version=latest)](https://wsinfer.readthedocs.io/en/latest/?badge=latest)
 [![Version on PyPI](https://img.shields.io/pypi/v/wsinfer.svg)](https://pypi.org/project/wsinfer/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/wsinfer)](https://pypi.org/project/wsinfer/)
 
 See https://wsinfer.readthedocs.io for documentation.
 
 # Installation
 
 ## Pip
 
-Pip install this package from GitHub. First install `torch` and `torchvision`
-(please see [the PyTorch documentation](https://pytorch.org/get-started/locally/)).
-We do not install these dependencies automatically because their installation can vary based
-on a user's system. Then use the command below to install this package.
+WSInfer will install PyTorch automatically if it is not installed, but this may not
+install GPU-enabled PyTorch even if a GPU is available. For this reason, install PyTorch
+before installing WSInfer. Please see [PyTorch's installation instructions](https://pytorch.org/get-started/locally/)
+for help install PyTorch.
 
 ```
-python -m pip install --find-links https://girder.github.io/large_image_wheels wsinfer
+python -m pip install wsinfer
 ```
 
 To use the _bleeding edge_, use
 
 ```
-python -m pip install \
-    --find-links https://girder.github.io/large_image_wheels \
-    git+https://github.com/SBU-BMI/wsinfer.git
+python -m pip install git+https://github.com/SBU-BMI/wsinfer.git
 ```
 
 ## Developers
 
 Clone this GitHub repository and install the package (in editable mode with the `dev` extras).
 
 ```
 git clone https://github.com/SBU-BMI/wsinfer.git
 cd wsinfer
-python -m pip install --editable .[dev] --find-links https://girder.github.io/large_image_wheels
+python -m pip install --editable .[dev]
 ```
 
 # Cutting a release
 
 When ready to cut a new release, follow these steps:
 
 1. Update the base image versions Dockerfiles in `dockerfiles/`. Update the version to
```

### Comparing `wsinfer-0.3.6/README.md` & `wsinfer-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 # WSInfer: deep learning inference on whole slide images
 
 Original H&E                        |  Heatmap of Tumor Probability
 :----------------------------------:|:-----------------------------------:
-![](docs/images/brca-tissue.png)  | ![](docs/images/brca-heatmap.png)
+![](docs/_static/brca-tissue.png)  | ![](docs/_static/brca-heatmap.png)
 
 🔥 🚀 Blazingly fast pipeline to run patch-based classification models on whole slide images.
 
 [![Continuous Integration](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml/badge.svg)](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/wsinfer/badge/?version=latest)](https://wsinfer.readthedocs.io/en/latest/?badge=latest)
 [![Version on PyPI](https://img.shields.io/pypi/v/wsinfer.svg)](https://pypi.org/project/wsinfer/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/wsinfer)](https://pypi.org/project/wsinfer/)
 
 See https://wsinfer.readthedocs.io for documentation.
 
 # Installation
 
 ## Pip
 
-Pip install this package from GitHub. First install `torch` and `torchvision`
-(please see [the PyTorch documentation](https://pytorch.org/get-started/locally/)).
-We do not install these dependencies automatically because their installation can vary based
-on a user's system. Then use the command below to install this package.
+WSInfer will install PyTorch automatically if it is not installed, but this may not
+install GPU-enabled PyTorch even if a GPU is available. For this reason, install PyTorch
+before installing WSInfer. Please see [PyTorch's installation instructions](https://pytorch.org/get-started/locally/)
+for help install PyTorch.
 
 ```
-python -m pip install --find-links https://girder.github.io/large_image_wheels wsinfer
+python -m pip install wsinfer
 ```
 
 To use the _bleeding edge_, use
 
 ```
-python -m pip install \
-    --find-links https://girder.github.io/large_image_wheels \
-    git+https://github.com/SBU-BMI/wsinfer.git
+python -m pip install git+https://github.com/SBU-BMI/wsinfer.git
 ```
 
 ## Developers
 
 Clone this GitHub repository and install the package (in editable mode with the `dev` extras).
 
 ```
 git clone https://github.com/SBU-BMI/wsinfer.git
 cd wsinfer
-python -m pip install --editable .[dev] --find-links https://girder.github.io/large_image_wheels
+python -m pip install --editable .[dev]
 ```
 
 # Cutting a release
 
 When ready to cut a new release, follow these steps:
 
 1. Update the base image versions Dockerfiles in `dockerfiles/`. Update the version to
```

### Comparing `wsinfer-0.3.6/wsinfer/cli/convert_csv_to_geojson.py` & `wsinfer-0.4.0/wsinfer/cli/convert_csv_to_geojson.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Convert CSVs of model outputs to GeoJSON files.
 
 GeoJSON files can be loaded into whole slide image viewers like QuPath.
 """
 
+from __future__ import annotations
+
 import json
 from pathlib import Path
-import typing
 
 import click
 import pandas as pd
 import tqdm
 
 
 def _box_to_polygon(
     *, minx: int, miny: int, width: int, height: int
-) -> typing.List[typing.Tuple[int, int]]:
+) -> list[tuple[int, int]]:
     """Get coordinates of a box polygon."""
     maxx = minx + width
     maxy = miny + height
     return [(maxx, miny), (maxx, maxy), (minx, maxy), (minx, miny), (maxx, miny)]
 
 
-def _row_to_geojson(row: pd.Series, prob_cols: typing.List[str]) -> typing.Dict:
+def _row_to_geojson(row: pd.Series, prob_cols: list[str]) -> dict:
     """Convert information about one tile to a single GeoJSON feature."""
     minx, miny, width, height = row["minx"], row["miny"], row["width"], row["height"]
     coords = _box_to_polygon(minx=minx, miny=miny, width=width, height=height)
     prob_dict = row[prob_cols].to_dict()
     measurements = [{"name": k, "value": v} for k, v in prob_dict.items()]
     return {
         "type": "Feature",
@@ -44,24 +45,24 @@
             # We do not include classification because we do not enforce a single class
             # per tile.
             # "classification": {"name": class_name},
         },
     }
 
 
-def _dataframe_to_geojson(df: pd.DataFrame, prob_cols: typing.List[str]) -> typing.Dict:
+def _dataframe_to_geojson(df: pd.DataFrame, prob_cols: list[str]) -> dict:
     """Convert a dataframe of tiles to GeoJSON format."""
     features = df.apply(_row_to_geojson, axis=1, prob_cols=prob_cols)
     return {
         "type": "FeatureCollection",
         "features": features.tolist(),
     }
 
 
-def convert(input, output) -> None:
+def convert(input: str | Path, output: str | Path) -> None:
     df = pd.read_csv(input)
     prob_cols = [col for col in df.columns.tolist() if col.startswith("prob_")]
     if not prob_cols:
         raise click.ClickException("Did not find any columns with prob_ prefix.")
     geojson = _dataframe_to_geojson(df, prob_cols)
     with open(output, "w") as f:
         json.dump(geojson, f)
@@ -74,15 +75,15 @@
         exists=True, file_okay=False, dir_okay=True, path_type=Path, resolve_path=True
     ),
 )
 @click.argument(
     "output",
     type=click.Path(exists=False, path_type=Path, resolve_path=True),
 )
-def togeojson(*, results_dir: Path, output: Path):
+def togeojson(*, results_dir: Path, output: Path) -> None:
     """Convert model outputs to GeoJSON format.
 
     GeoJSON files can be used with pathology viewers like QuPath.
 
     RESULTS_DIR     Path to results directory (containing model-outputs dir).
 
     OUTPUT          Path to output directory in which to save GeoJSON files.
```

### Comparing `wsinfer-0.3.6/wsinfer/cli/convert_csv_to_sbubmi.py` & `wsinfer-0.4.0/wsinfer/cli/convert_csv_to_sbubmi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 """Convert CSV of model outputs to Stony Brook BMI formats.
 
 Output directory tree for single class outputs:
 ├── heatmap_jsons
-│   ├── heatmap-SLIDEID.json
-│   └── meta-SLIDEID.json
+│   ├── heatmap-SLIDEID.json
+│   └── meta-SLIDEID.json
 └── heatmap_txt
     ├── color-SLIDEID
     └── prediction-SLIDEID
 
 Output directory tree for multi-class outputs:
 ├── heatmap_jsons
-│   └── CLASS_LABEL
-│       ├── heatmap-SLIDEID.json
-│       └── meta-SLIDEID.json
+│   └── CLASS_LABEL
+│       ├── heatmap-SLIDEID.json
+│       └── meta-SLIDEID.json
 └── heatmap_txt
     └── CLASS_LABEL
         ├── color-SLIDEID
         └── prediction-SLIDEID
 """
 
+from __future__ import annotations
+
 import json
 import multiprocessing
-from pathlib import Path
 import pprint
 import random
 import shutil
 import time
-import typing
+from pathlib import Path
+from typing import Any
 
 import click
-import large_image
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import tqdm
 
-
-PathType = typing.Union[str, Path]
+from ..wsi import WSI
+from ..wsi import CanReadRegion
 
 
 def _box_to_polygon(
     *, minx: float, miny: float, width: float, height: float
-) -> typing.List[typing.Tuple[float, float]]:
+) -> list[tuple[float, float]]:
     """Get coordinates of a box polygon."""
     maxx = minx + width
     maxy = miny + height
     return [(maxx, miny), (maxx, maxy), (minx, maxy), (minx, miny), (maxx, miny)]
 
 
 def write_heatmap_and_meta_json_lines(
-    input: PathType,
-    output_heatmap: PathType,
-    output_meta: PathType,
-    slide_width: PathType,
-    slide_height: PathType,
+    input: str | Path,
+    output_heatmap: str | Path,
+    output_meta: str | Path,
+    slide_width: int,
+    slide_height: int,
     execution_id: str,
     study_id: str,
     case_id: str,
     subject_id: str,
     class_name: str,
-    run_metadata: typing.Dict,
+    run_metadata: dict,
 ) -> None:
     """Write JSON-lines files for one slide."""
 
     # Run this before defining the function so the entire JSON file has the same
     # execution time value.
     date = int(time.time())
 
-    version_dict: typing.Dict = run_metadata["runtime"]["git"] or {}
+    version_dict: dict = run_metadata["runtime"]["git"] or {}
     version_dict["model_path"] = run_metadata["model_weights"]["weights_file"]
     version_dict["model_hash"] = run_metadata["model_weights"]["weights_sha256"]
     version_dict["model_url"] = run_metadata["model_weights"]["weights_url"]
     version_dict["model_ver"] = None
 
-    def row_to_json(row: pd.Series):
+    def row_to_json(row: pd.Series) -> dict[str, Any]:
         minx, miny, width, height = (
             row["minx"],
             row["miny"],
             row["width"],
             row["height"],
         )
         patch_area_base_pixels = width * height
@@ -165,59 +167,58 @@
         "submit_date": {"$date": date},
         "randval": random.uniform(0, 1),
     }
     with open(output_meta, "w") as f:
         json.dump(meta_dict, f)
 
 
-def write_heatmap_txt(input: PathType, output: PathType, class_names: typing.List[str]):
+def write_heatmap_txt(
+    input: str | Path, output: str | Path, class_names: list[str]
+) -> None:
     df = pd.read_csv(input)
     # TODO: should we round and cast to int here?
     df.loc[:, "x_loc"] = (df.minx + (df.width / 2)).round().astype(int)
     df.loc[:, "y_loc"] = (df.miny + (df.height / 2)).round().astype(int)
     prob_cols = [f"prob_{c}" for c in class_names]
     cols = ["x_loc", "y_loc", *prob_cols]
     df = df.loc[:, cols]
     # Rename 'prob_NAME' columns to 'NAME'.
     df = df.rename(columns={c: c[5:] for c in prob_cols})
     df.to_csv(output, index=False, sep=" ")
 
 
 def write_color_txt(
-    input: PathType,
-    output: PathType,
-    ts: large_image.tilesource.TileSource,
+    input: str | Path,
+    output: str | Path,
+    slide: CanReadRegion,
     num_processes: int = 6,
-):
-    def whiteness(arr):
+) -> None:
+    def whiteness(arr: npt.ArrayLike) -> float:
         arr = np.asarray(arr)
-        return np.std(arr, axis=(0, 1)).mean()
+        return np.std(arr, axis=(0, 1)).mean()  # type: ignore
 
-    def blackness(arr):
+    def blackness(arr: npt.ArrayLike) -> float:
         arr = np.asarray(arr)
-        return arr.mean()
+        return arr.mean()  # type: ignore
 
-    def redness(arr):
+    def redness(arr: npt.ArrayLike) -> float:
         arr = np.asarray(arr)
         r, g, b = arr[:, :, 0], arr[:, :, 1], arr[:, :, 2]
         # boolean multiplication is logical and
-        return np.mean((r >= 190) * (g <= 100) * (b <= 100))
+        return np.mean((r >= 190) * (g <= 100) * (b <= 100))  # type: ignore
 
     global get_color  # Hack to please multiprocessing.
 
-    def get_color(row: pd.Series):
-        arr, _ = ts.getRegion(
-            format=large_image.constants.TILE_FORMAT_NUMPY,
-            region=dict(
-                left=row["minx"],
-                top=row["miny"],
-                width=row["width"],
-                height=row["height"],
-            ),
+    def get_color(row: pd.Series) -> tuple[float, float, float]:
+        patch_im = slide.read_region(
+            location=(row["minx"], row["miny"]),
+            level=0,
+            size=(row["width"], row["height"]),
         )
+        arr = np.asarray(patch_im)
         white = whiteness(arr)
         black = blackness(arr)
         red = redness(arr)
         return white, black, red
 
     df = pd.read_csv(input)
     df_rows_as_dicts = df.to_dict("records")
@@ -283,15 +284,15 @@
     results_dir: Path,
     output: Path,
     wsi_dir: Path,
     execution_id: str,
     study_id: str,
     make_color_text: bool = False,
     num_processes: int = 4,
-):
+) -> None:
     """Convert model outputs to Stony Brook format.
 
     Convert CSVs of patch predictions to .txt and .json formats for use with Stony
     Brook Biomedical Informatics viewers.
 
     RESULTS_DIR     Path to results directory (containing model-outputs dir).
 
@@ -324,25 +325,25 @@
     csvs = list((results_dir / "model-outputs").glob("*.csv"))
     if not csvs:
         raise click.ClickException("No CSVs found. Did you generate model outputs?")
 
     output.mkdir(exist_ok=False)
 
     with open(results_dir / "run_metadata.json") as f:
-        run_metadata: typing.Dict = json.load(f)
+        run_metadata: dict = json.load(f)
 
     print("-" * 40)
     print("Run metadata")
     pprint.pprint(run_metadata, indent=2)
     print("-" * 40, "\n")
 
     # Get the output classes of the model. We will create separate directories for each
     # label name. But by default, we do not include labels that start with "no", like
     # "notils" and "notumor".
-    class_names: typing.List[str] = run_metadata["model_weights"]["class_names"]
+    class_names: list[str] = run_metadata["model_weights"]["class_names"]
     ignore_names = {"notils", "notumor"}
     class_names = [n for n in class_names if n not in ignore_names]
 
     print("-" * 40)
     print("Output class names:")
     for c in class_names:
         print(f"  - {c}")
@@ -353,19 +354,17 @@
         print(f"Converting outputs for slide {ii+1} of {len(csvs)}")
         slide_id = input_csv.stem
         wsi_file = wsi_dir / f"{slide_id}.svs"
         if not wsi_file.exists():
             click.secho(f"WSI file not found: {wsi_file}", bg="red")
             click.secho("Skipping...", bg="red")
             continue
-        ts = large_image.getTileSource(wsi_file)
-        if ts.sizeX is None or ts.sizeY is None:
-            click.secho(f"Unknown size for WSI: {wsi_file}", bg="red")
-            click.secho("Skipping...", bg="red")
-            continue
+        slide = WSI(wsi_file)
+
+        slide_width, slide_height = slide.level_dimensions[0]
 
         for class_name in class_names:
             if len(class_names) == 1:
                 # Do not use class-specific dirs if there is only one class.
                 output_heatmap = output / "heatmap_json" / f"heatmap_{slide_id}.json"
                 output_meta = output_heatmap.parent / f"meta_{slide_id}.json"
             else:
@@ -379,16 +378,16 @@
             click.echo(f"  {output_heatmap}")
             click.echo("Writing JSON meta:")
             click.echo(f"  {output_meta}")
             write_heatmap_and_meta_json_lines(
                 input=input_csv,
                 output_heatmap=output_heatmap,
                 output_meta=output_meta,
-                slide_width=ts.sizeX,
-                slide_height=ts.sizeY,
+                slide_width=slide_width,
+                slide_height=slide_height,
                 execution_id=execution_id,
                 study_id=study_id,
                 case_id=slide_id,  # TODO: should case_id be different?
                 subject_id=slide_id,
                 class_name=class_name,
                 run_metadata=run_metadata,
             )
@@ -415,26 +414,26 @@
             print("Writing color TXT file with color information for each patch")
             if len(class_names) == 1:
                 output_color = output / "heatmap_txt" / f"color-{slide_id}"
                 print(f"  {output_color}")
                 write_color_txt(
                     input=input_csv,
                     output=output_color,
-                    ts=ts,
+                    slide=slide,
                     num_processes=num_processes,
                 )
             else:
                 output_color = (
                     output / "heatmap_txt" / class_names[0] / f"color-{slide_id}"
                 )
                 print(f"  {output_color}")
                 write_color_txt(
                     input=input_csv,
                     output=output_color,
-                    ts=ts,
+                    slide=slide,
                     num_processes=num_processes,
                 )
                 # Copy this color file to all class-specific dirs.
                 print("Copying color TXT file to class-specific TXT directories")
                 for class_name in class_names[1:]:
                     cp_dst = output_color.parent.parent / class_name / output_color.name
                     print(f"  {cp_dst}")
```

### Comparing `wsinfer-0.3.6/wsinfer/cli/infer.py` & `wsinfer-0.4.0/wsinfer/cli/infer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Detect cancerous regions in a whole slide image."""
 
-from datetime import datetime
+from __future__ import annotations
+
+import dataclasses
 import getpass
 import json
 import os
-from pathlib import Path
 import platform
 import shutil
 import subprocess
 import sys
-import typing
+from datetime import datetime
+from pathlib import Path
+from typing import Any
 
 import click
-
-from .._modellib.run_inference import run_inference
-from .._modellib import models
-from .._patchlib.create_dense_patch_grid import create_grid_and_save_multi_slides
-from .._patchlib.create_patches_fp import create_patches
-
-PathType = typing.Union[str, Path]
+import wsinfer_zoo
+import wsinfer_zoo.client
+from wsinfer_zoo.client import HFModel
+from wsinfer_zoo.client import ModelConfiguration
+
+from ..modellib import models
+from ..modellib.run_inference import run_inference
+from ..patchlib import segment_and_patch_directory_of_slides
 
 
 def _num_cpus() -> int:
     """Get number of CPUs on the system."""
     try:
         return len(os.sched_getaffinity(0))
     # os.sched_getaffinity seems to be linux only.
@@ -50,14 +54,15 @@
     return dt.strftime("%c %Z")
 
 
 def _print_system_info() -> None:
     """Print information about the system."""
     import torch
     import torchvision
+
     from .. import __version__
 
     click.secho(f"\nRunning wsinfer version {__version__}", fg="green")
     print("\nIf you run into issues, please submit a new issue at")
     print("https://github.com/kaczmarj/patch-classification-pipeline/issues/new")
     print("\nSystem information")
     print("------------------")
@@ -98,26 +103,29 @@
         click.secho("\n*******************************************", fg="yellow")
         click.secho("GPU WILL NOT BE USED", fg="yellow")
         if torch.version.cuda is None:
             click.secho("  CUDA DEVICES NOT AVAILABLE", fg="yellow")
         click.secho("*******************************************", fg="yellow")
 
 
-def _get_info_for_save(weights: models.Weights):
+def _get_info_for_save(
+    model_obj: models.LocalModelTorchScript | HFModel,
+) -> dict[str, Any]:
     """Get dictionary with information about the run. To save as JSON in output dir."""
 
     import torch
+
     from .. import __version__
 
     here = Path(__file__).parent.resolve()
 
-    def get_git_info():
+    def get_git_info() -> dict[str, str | bool]:
         here = Path(__file__).parent.resolve()
 
-        def get_stdout(args) -> str:
+        def get_stdout(args: list[str]) -> str:
             proc = subprocess.run(args, capture_output=True, cwd=here)
             return "" if proc.returncode != 0 else proc.stdout.decode().strip()
 
         git_remote = get_stdout("git config --get remote.origin.url".split())
         git_branch = get_stdout("git rev-parse --abbrev-ref HEAD".split())
         git_commit = get_stdout("git rev-parse HEAD".split())
 
@@ -143,152 +151,148 @@
             stderr=subprocess.DEVNULL,
         )
         is_git_repo = cmd.returncode == 0
     git_info = None
     if git_installed and is_git_repo:
         git_info = get_git_info()
 
-    weights_file = weights.file
-    if weights_file is None:
-        if weights.url_file_name is None:
-            raise TypeError("url_file_name must not be None if file is None.")
-        weights_file = str(
-            Path(torch.hub.get_dir()) / "checkpoints" / weights.url_file_name
-        )
+    hf_info = None
+    if hasattr(model_obj, "hf_info"):
+        hf_info = dataclasses.asdict(model_obj.hf_info)
 
     return {
-        "model_weights": {
-            "name": weights.name,
-            "architecture": weights.architecture,
-            "weights_url": weights.url,
-            "weights_url_file_name": weights.url_file_name,
-            "weights_file": weights_file,
-            "weights_sha256": weights.get_sha256_of_weights(),
-            "class_names": weights.class_names,
-            "num_classes": weights.num_classes,
-            "patch_size_pixels": weights.patch_size_pixels,
-            "spacing_um_px": weights.spacing_um_px,
-            "transform": {
-                "resize_size": weights.transform.resize_size,
-                "mean": weights.transform.mean,
-                "std": weights.transform.std,
-            },
-            "metadata": weights.metadata or None,
+        "model": {
+            "config": dataclasses.asdict(model_obj.config),
+            "huggingface_location": hf_info,
+            "path": str(model_obj.model_path),
         },
         "runtime": {
             "version": __version__,
             "working_dir": os.getcwd(),
             "args": " ".join(sys.argv),
             "python_executable": sys.executable,
             "python_version": platform.python_version(),
             "in_container": _inside_container(),
             "pytorch_version": torch.__version__,
             "cuda_version": torch.version.cuda,
             "git": git_info,
+            "wsinfer_zoo_version": wsinfer_zoo.__version__,
         },
         "timestamp": _get_timestamp(),
     }
 
 
-@click.command(context_settings=dict(auto_envvar_prefix="WSINFER"))
+@click.command()
 @click.pass_context
 @click.option(
+    "-i",
     "--wsi-dir",
     type=click.Path(exists=True, file_okay=False, path_type=Path, resolve_path=True),
     required=True,
     help="Directory containing whole slide images. This directory can *only* contain"
     " whole slide images.",
 )
 @click.option(
+    "-o",
     "--results-dir",
     type=click.Path(file_okay=False, path_type=Path, resolve_path=True),
     required=True,
     help="Directory to store results. If directory exists, will skip"
     " whole slides for which outputs exist.",
 )
 @click.option(
+    "-m",
     "--model",
-    type=click.Choice(sorted({a for a, _ in models.list_all_models_and_weights()})),
-    help="Model architecture to use. Not required if 'config' is used.",
-)
-@click.option(
-    "--weights",
-    type=click.Choice(sorted({w for _, w in models.list_all_models_and_weights()})),
-    help="Name of weights to use for the model. Not required if 'config' is used.",
+    "model_name",
+    type=click.Choice(sorted(wsinfer_zoo.client.load_registry().models.keys())),
+    help="Name of the model to use from WSInfer Model Zoo. Mutually exclusive with"
+    " --config.",
 )
 @click.option(
+    "-c",
     "--config",
     type=click.Path(exists=True, dir_okay=False, path_type=Path, resolve_path=True),
     help=(
-        "Path to configuration for architecture and weights. Use this option if the"
+        "Path to configuration for the trained model. Use this option if the"
         " model weights are not registered in wsinfer. Mutually exclusive with"
-        " 'model' and 'weights'."
+        "--model"
+    ),
+)
+@click.option(
+    "-p",
+    "--model-path",
+    type=click.Path(exists=True, dir_okay=False, path_type=Path, resolve_path=True),
+    help=(
+        "Path to the pretrained model. Use only when --config is passed. Mutually "
+        "exclusive with --model."
     ),
 )
 @click.option(
+    "-b",
     "--batch-size",
     type=click.IntRange(min=1),
     default=32,
     show_default=True,
     help="Batch size during model inference. If using multiple GPUs, increase the"
     " batch size.",
 )
 @click.option(
+    "-n",
     "--num-workers",
     default=min(_num_cpus(), 8),  # Use at most 8 workers by default.
     show_default=True,
     type=click.IntRange(min=0),
     help="Number of workers to use for data loading during model inference (n=0 for"
     " single thread). Set this to the number of cores on your machine or lower.",
 )
 @click.option(
     "--speedup/--no-speedup",
     default=False,
     show_default=True,
-    help="JIT-compile the model for potential speedups.",
-)
-@click.option(
-    "--dense-grid/--no-dense-grid",
-    default=False,
-    show_default=True,
-    help="Use a dense grid of patch coordinates. Patches will be present even if no"
-    " tissue is present",
+    help="JIT-compile the model and apply inference optimizations. This imposes a"
+    " startup cost but may improve performance overall.",
 )
 def run(
     ctx: click.Context,
     *,
     wsi_dir: Path,
     results_dir: Path,
-    model: typing.Optional[str],
-    weights: typing.Optional[str],
-    config: typing.Optional[Path],
+    model_name: str | None,
+    config: Path | None,
+    model_path: Path | None,
     batch_size: int,
     num_workers: int = 0,
     speedup: bool = False,
-    dense_grid: bool = False,
-):
+) -> None:
     """Run model inference on a directory of whole slide images.
 
     This command will create a tissue mask of each WSI. Then patch coordinates will be
     computed. The chosen model will be applied to each patch, and the results will be
     saved to a CSV in `RESULTS_DIR/model-output`.
 
     Example:
 
-    CUDA_VISIBLE_DEVICES=0 wsinfer run --wsi_dir slides/ --results_dir results
-    --model resnet34 --weights TCGA-BRCA-v1 --batch_size 32 --num_workers 4
+    CUDA_VISIBLE_DEVICES=0 wsinfer run --wsi-dir slides/ --results-dir results
+    --model breast-tumor-resnet34.tcga-brca --batch-size 32 --num-workers 4
 
-    To list all available models and weights, use `wsinfer list`.
+    To list all available models and weights, use `wsinfer-zoo ls`.
     """
-    if model is None and weights is None and config is None:
-        raise click.UsageError("one of (model and weights) or config is required.")
-    elif (model is not None or weights is not None) and config is not None:
-        raise click.UsageError("model and weights are mutually exclusive with config.")
-    elif (model is not None) ^ (weights is not None):  # XOR
-        raise click.UsageError("model and weights must both be set if one is set.")
+
+    if model_name is None and config is None and model_path is None:
+        raise click.UsageError(
+            "one of --model or (--config and --model-path) is required."
+        )
+    elif (config is not None or model_path is not None) and model_name is not None:
+        raise click.UsageError(
+            "--config and --model-path are mutually exclusive with --model."
+        )
+    elif (config is not None) ^ (model_path is not None):  # XOR
+        raise click.UsageError(
+            "--config and --model-path must both be set if one is set."
+        )
 
     wsi_dir = wsi_dir.resolve()
     results_dir = results_dir.resolve()
 
     if not wsi_dir.exists():
         raise FileNotFoundError(f"Whole slide image directory not found: {wsi_dir}")
 
@@ -307,44 +311,51 @@
     print("----------------------")
     for key, value in ctx.params.items():
         print(f"{key} = {value}")
     print("----------------------\n")
 
     # Get weights object before running the patching script because we need to get the
     # necessary spacing and patch size.
-    if model is not None and weights is not None:
-        weights_obj = models.get_model_weights(model, name=weights)
+    model_obj: HFModel | models.LocalModelTorchScript
+    if model_name is not None:
+        model_obj = models.get_registered_model(name=model_name)
     elif config is not None:
-        weights_obj = models.Weights.from_yaml(config)
-
-    click.secho("\nFinding patch coordinates...\n", fg="green")
-    if dense_grid:
-        click.echo("Not using a tissue mask.")
-        create_grid_and_save_multi_slides(
-            wsi_dir=wsi_dir,
-            results_dir=results_dir,
-            orig_patch_size=weights_obj.patch_size_pixels,
-            patch_spacing_um_px=weights_obj.spacing_um_px,
+        with open(config) as f:
+            _config_dict = json.load(f)
+        model_config = ModelConfiguration.from_dict(_config_dict)
+        model_obj = models.LocalModelTorchScript(
+            config=model_config, model_path=str(model_path)
         )
+        del _config_dict, model_config
     else:
-        create_patches(
-            source=str(wsi_dir),
-            save_dir=str(results_dir),
-            patch_size=weights_obj.patch_size_pixels,
-            patch_spacing=weights_obj.spacing_um_px,
-            seg=True,
-            patch=True,
-            preset="tcga.csv",
-        )
+        raise click.ClickException("Neither of --config and --model was passed")
+
+    click.secho("\nFinding patch coordinates...\n", fg="green")
+
+    # FIXME: add presets for different tissue types?
+
+    segment_and_patch_directory_of_slides(
+        wsi_dir=wsi_dir,
+        save_dir=results_dir,
+        patch_size_px=model_obj.config.patch_size_pixels,
+        patch_spacing_um_px=model_obj.config.spacing_um_px,
+        thumbsize=(2048, 2048),
+        # TODO: these can be made arguments to the CLI.
+        median_filter_size=7,
+        binary_threshold=7,
+        closing_kernel_size=6,
+        min_object_size_um2=200**2,
+        min_hole_size_um2=190**2,
+    )
 
     click.secho("\nRunning model inference.\n", fg="green")
     failed_patching, failed_inference = run_inference(
         wsi_dir=wsi_dir,
         results_dir=results_dir,
-        weights=weights_obj,
+        model_info=model_obj,
         batch_size=batch_size,
         num_workers=num_workers,
         speedup=speedup,
     )
 
     if failed_patching:
         click.secho(f"\nPatching failed for {len(failed_patching)} slides", fg="yellow")
@@ -354,12 +365,12 @@
             f"\nInference failed for {len(failed_inference)} slides", fg="yellow"
         )
         click.secho("\n".join(failed_inference), fg="yellow")
 
     timestamp = datetime.now().astimezone().strftime("%Y%m%dT%H%M%S")
     run_metadata_outpath = results_dir / f"run_metadata_{timestamp}.json"
     click.echo(f"Saving metadata about run to {run_metadata_outpath}")
-    run_metadata = _get_info_for_save(weights_obj)
+    run_metadata = _get_info_for_save(model_obj)
     with open(run_metadata_outpath, "w") as f:
         json.dump(run_metadata, f, indent=2)
 
     click.secho("Finished.", fg="green")
```

### Comparing `wsinfer-0.3.6/wsinfer.egg-info/PKG-INFO` & `wsinfer-0.4.0/wsinfer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 Metadata-Version: 2.1
 Name: wsinfer
-Version: 0.3.6
+Version: 0.4.0
 Summary: Run patch-based classification on pathology whole slide images.
-Home-page: https://github.com/SBU-BMI/wsinfer
-Author: Jakub Kaczmarzyk
-Author-email: jakub.kaczmarzyk@stonybrookmedicine.edu
-License: GNU General Public License v3 (GPLv3)
+Author-email: Jakub Kaczmarzyk <jakub.kaczmarzyk@stonybrookmedicine.edu>
+Maintainer-email: Jakub Kaczmarzyk <jakub.kaczmarzyk@stonybrookmedicine.edu>
+License: Apache License, Version 2.0
+Project-URL: Homepage, https://wsinfer.readthedocs.io
+Project-URL: Documentation, https://wsinfer.readthedocs.io
+Project-URL: Repository, https://github.com/SBU-BMI/wsinfer
+Project-URL: Bug Tracker, https://github.com/SBU-BMI/wsinfer/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: openslide
 License-File: LICENSE
 
 # WSInfer: deep learning inference on whole slide images
 
 Original H&E                        |  Heatmap of Tumor Probability
 :----------------------------------:|:-----------------------------------:
-![](docs/images/brca-tissue.png)  | ![](docs/images/brca-heatmap.png)
+![](docs/_static/brca-tissue.png)  | ![](docs/_static/brca-heatmap.png)
 
 🔥 🚀 Blazingly fast pipeline to run patch-based classification models on whole slide images.
 
 [![Continuous Integration](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml/badge.svg)](https://github.com/SBU-BMI/wsinfer/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/wsinfer/badge/?version=latest)](https://wsinfer.readthedocs.io/en/latest/?badge=latest)
 [![Version on PyPI](https://img.shields.io/pypi/v/wsinfer.svg)](https://pypi.org/project/wsinfer/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/wsinfer)](https://pypi.org/project/wsinfer/)
 
 See https://wsinfer.readthedocs.io for documentation.
 
 # Installation
 
 ## Pip
 
-Pip install this package from GitHub. First install `torch` and `torchvision`
-(please see [the PyTorch documentation](https://pytorch.org/get-started/locally/)).
-We do not install these dependencies automatically because their installation can vary based
-on a user's system. Then use the command below to install this package.
+WSInfer will install PyTorch automatically if it is not installed, but this may not
+install GPU-enabled PyTorch even if a GPU is available. For this reason, install PyTorch
+before installing WSInfer. Please see [PyTorch's installation instructions](https://pytorch.org/get-started/locally/)
+for help install PyTorch.
 
 ```
-python -m pip install --find-links https://girder.github.io/large_image_wheels wsinfer
+python -m pip install wsinfer
 ```
 
 To use the _bleeding edge_, use
 
 ```
-python -m pip install \
-    --find-links https://girder.github.io/large_image_wheels \
-    git+https://github.com/SBU-BMI/wsinfer.git
+python -m pip install git+https://github.com/SBU-BMI/wsinfer.git
 ```
 
 ## Developers
 
 Clone this GitHub repository and install the package (in editable mode with the `dev` extras).
 
 ```
 git clone https://github.com/SBU-BMI/wsinfer.git
 cd wsinfer
-python -m pip install --editable .[dev] --find-links https://girder.github.io/large_image_wheels
+python -m pip install --editable .[dev]
 ```
 
 # Cutting a release
 
 When ready to cut a new release, follow these steps:
 
 1. Update the base image versions Dockerfiles in `dockerfiles/`. Update the version to
```

