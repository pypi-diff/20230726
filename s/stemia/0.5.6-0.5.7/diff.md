# Comparing `tmp/stemia-0.5.6.tar.gz` & `tmp/stemia-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemia-0.5.6.tar", last modified: Thu Feb  9 14:26:46 2023, max compression
+gzip compressed data, was "stemia-0.5.7.tar", last modified: Thu Feb  9 16:09:43 2023, max compression
```

## Comparing `stemia-0.5.6.tar` & `stemia-0.5.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.503649 stemia-0.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.495649 stemia-0.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-09 14:26:26.000000 stemia-0.5.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-09 14:26:26.000000 stemia-0.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-09 14:26:26.000000 stemia-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-02-09 14:26:46.503649 stemia-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-02-09 14:26:26.000000 stemia-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-02-09 14:26:26.000000 stemia-0.5.6/docs/generate_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-09 14:26:26.000000 stemia-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-09 14:26:46.503649 stemia-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/aln2xf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/aretomo/batch_warp/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/aretomo/batch_warp/topaz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/cryosparc/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/cryosparc/csplot/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/csplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/csplot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/csplot/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/csplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/fix_filament_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/cryosparc/generate_tilt_angles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia/image/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.503649 stemia-0.5.6/stemia/image/center_filament/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/center_filament/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/center_filament/center_filament.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/center_filament/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/extract_z_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/flip_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/image/rescale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.503649 stemia-0.5.6/stemia/relion/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/relion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.503649 stemia-0.5.6/stemia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/utils/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/utils/io_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.503649 stemia-0.5.6/stemia/warp/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/offset_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/parse_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/prepare_isonet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/preprocess_serialem.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-09 14:26:26.000000 stemia-0.5.6/stemia/warp/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:26:46.499649 stemia-0.5.6/stemia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 14:26:46.000000 stemia-0.5.6/stemia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-09 16:09:21.000000 stemia-0.5.7/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-09 16:09:21.000000 stemia-0.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-09 16:09:21.000000 stemia-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-02-09 16:09:43.306962 stemia-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-02-09 16:09:21.000000 stemia-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-02-09 16:09:21.000000 stemia-0.5.7/docs/generate_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-09 16:09:21.000000 stemia-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-09 16:09:43.310962 stemia-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/stemia/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/stemia/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/aln2xf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/aretomo/batch_warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/aretomo/batch_warp/topaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/cryosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/cryosparc/csplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/csplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/csplot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/csplot/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/csplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/fix_filament_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/cryosparc/generate_tilt_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/image/center_filament/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/center_filament/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/center_filament/center_filament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/center_filament/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/extract_z_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/flip_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/image/rescale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/relion/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/relion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/utils/io_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.306962 stemia-0.5.7/stemia/warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/offset_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/parse_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/prepare_isonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/preprocess_serialem.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-09 16:09:21.000000 stemia-0.5.7/stemia/warp/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 16:09:43.302962 stemia-0.5.7/stemia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 16:09:43.000000 stemia-0.5.7/stemia.egg-info/top_level.txt
```

### Comparing `stemia-0.5.6/.github/workflows/deploy.yml` & `stemia-0.5.7/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/LICENSE` & `stemia-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/PKG-INFO` & `stemia-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.5.6
+Version: 0.5.7
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.5.6/README.md` & `stemia-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/docs/generate_readme.py` & `stemia-0.5.7/docs/generate_readme.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/setup.cfg` & `stemia-0.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/aln2xf.py` & `stemia-0.5.7/stemia/aretomo/aln2xf.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/aretomo.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/aretomo.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/fix.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/fix.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/main.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/parse.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,29 +32,34 @@
             tilt_series_unprocessed.append(ts_name)
             continue
 
         # extract even/odd paths
         tilts = [warp_dir / PureWindowsPath(tilt).name for tilt in df.SubFramePath]
         odd = []
         even = []
+        valid_xml = None
         for tilt in tilts:
             xml = ElementTree.parse(tilt.with_suffix('.xml')).getroot()
             if xml.attrib['UnselectManual'] == 'True':
                 continue
 
+            valid_xml = xml
             odd.append(odd_dir / (tilt.stem + '.mrc'))
             even.append(even_dir / (tilt.stem + '.mrc'))
 
+        if valid_xml is None:
+            continue
+
         if train:
             for img in odd + even:
                 if not img.exists():
                     raise FileNotFoundError(img)
 
         # extract metadata from warp xmls (we assume the last xml has the same data as the others)
-        for param in xml.find('OptionsCTF'):
+        for param in valid_xml.find('OptionsCTF'):
             if param.get('Name') == 'BinTimes':
                 bin = float(param.get('Value'))
             elif param.get('Name') == 'Voltage':
                 kv = int(param.get('Value'))
             elif param.get('Name') == 'Cs':
                 cs = float(param.get('Value'))
         for param in xml.find('CTF'):
```

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/stack.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/stack.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/threaded.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/threaded.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/aretomo/batch_warp/topaz.py` & `stemia-0.5.7/stemia/aretomo/batch_warp/topaz.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/cryosparc/csplot/main.py` & `stemia-0.5.7/stemia/cryosparc/csplot/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/cryosparc/csplot/parse.py` & `stemia-0.5.7/stemia/cryosparc/csplot/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/cryosparc/csplot/plot.py` & `stemia-0.5.7/stemia/cryosparc/csplot/plot.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/cryosparc/fix_filament_ids.py` & `stemia-0.5.7/stemia/cryosparc/fix_filament_ids.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/cryosparc/generate_tilt_angles.py` & `stemia-0.5.7/stemia/cryosparc/generate_tilt_angles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/image/center_filament/center_filament.py` & `stemia-0.5.7/stemia/image/center_filament/center_filament.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/image/center_filament/funcs.py` & `stemia-0.5.7/stemia/image/center_filament/funcs.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/image/extract_z_snapshots.py` & `stemia-0.5.7/stemia/image/extract_z_snapshots.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/image/flip_z.py` & `stemia-0.5.7/stemia/image/flip_z.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/image/rescale.py` & `stemia-0.5.7/stemia/image/rescale.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/utils/click.py` & `stemia-0.5.7/stemia/utils/click.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/utils/image_processing.py` & `stemia-0.5.7/stemia/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/utils/io_.py` & `stemia-0.5.7/stemia/utils/io_.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/warp/fix_mdoc.py` & `stemia-0.5.7/stemia/warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/warp/offset_angle.py` & `stemia-0.5.7/stemia/warp/offset_angle.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/warp/prepare_isonet.py` & `stemia-0.5.7/stemia/warp/prepare_isonet.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/warp/preprocess_serialem.sh` & `stemia-0.5.7/stemia/warp/preprocess_serialem.sh`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia/warp/summarize.py` & `stemia-0.5.7/stemia/warp/summarize.py`

 * *Files identical despite different names*

### Comparing `stemia-0.5.6/stemia.egg-info/PKG-INFO` & `stemia-0.5.7/stemia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.5.6
+Version: 0.5.7
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.5.6/stemia.egg-info/SOURCES.txt` & `stemia-0.5.7/stemia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

