# Comparing `tmp/agh_vqis-3.2.0.tar.gz` & `tmp/agh_vqis-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-3.2.0.tar", last modified: Mon Jul 24 12:41:01 2023, max compression
+gzip compressed data, was "agh_vqis-3.2.1.tar", last modified: Wed Jul 26 07:38:45 2023, max compression
```

## Comparing `agh_vqis-3.2.0.tar` & `agh_vqis-3.2.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/
--rw-rw-rw-   0        0        0     2826 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/LICENSE
--rw-rw-rw-   0        0        0    13218 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    12210 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0    13218 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8201 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1329 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/src/agh_vqis/
--rw-rw-rw-   0        0        0      381 2023-07-24 12:37:50.000000 agh_vqis-3.2.0/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    22941 2023-07-24 12:24:21.000000 agh_vqis-3.2.0/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0     1349 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.348658 agh_vqis-3.2.0/src/agh_vqis/binaries/
--rw-rw-rw-   0        0        0    60648 2023-07-24 11:09:44.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt
--rw-rw-rw-   0        0        0    66424 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt
--rw-rw-rw-   0        0        0    97508 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt
--rw-rw-rw-   0        0        0    88328 2023-07-21 14:04:46.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt
--rwxrwxrwx   0        0        0   122077 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_win64_mt.exe
--rw-rw-rw-   0        0        0  2952245 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/cygwin1.dll
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/src/agh_vqis/models/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.536963 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/
--rw-rw-rw-   0        0        0    21075 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    21723 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    14595 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    15027 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    32379 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    35763 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    34035 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    29643 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
--rw-rw-rw-   0        0        0    33747 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
--rw-rw-rw-   0        0        0    28059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
--rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
--rw-rw-rw-   0        0        0    33531 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
--rw-rw-rw-   0        0        0    29355 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
--rw-rw-rw-   0        0        0    26691 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
--rw-rw-rw-   0        0        0    31803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
--rw-rw-rw-   0        0        0    30291 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
--rw-rw-rw-   0        0        0    30795 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    26907 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    38355 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
--rw-rw-rw-   0        0        0    39075 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
--rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
--rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
--rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
--rw-rw-rw-   0        0        0    39219 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
--rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
--rw-rw-rw-   0        0        0    37995 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
--rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    38643 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
--rw-rw-rw-   0        0        0    39363 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
--rw-rw-rw-   0        0        0    38067 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
--rw-rw-rw-   0        0        0    38211 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
--rw-rw-rw-   0        0        0    36915 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
--rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
--rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
--rw-rw-rw-   0        0        0    28779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
--rw-rw-rw-   0        0        0    29715 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
--rw-rw-rw-   0        0        0    30219 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
--rw-rw-rw-   0        0        0    38283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
--rw-rw-rw-   0        0        0    37563 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
--rw-rw-rw-   0        0        0    27843 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
--rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
--rw-rw-rw-   0        0        0    27699 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
--rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
--rw-rw-rw-   0        0        0    37275 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
--rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
--rw-rw-rw-   0        0        0    29283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
--rw-rw-rw-   0        0        0    27483 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
--rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
--rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
--rw-rw-rw-   0        0        0    38139 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
--rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
--rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    17835 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    27411 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
--rw-rw-rw-   0        0        0    25179 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
--rw-rw-rw-   0        0        0    22659 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
--rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    17187 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    25395 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
--rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    16827 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    23667 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
--rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
--rw-rw-rw-   0        0        0    22299 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
--rw-rw-rw-   0        0        0    22155 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
--rw-rw-rw-   0        0        0    19059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
--rw-rw-rw-   0        0        0    18987 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
--rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
--rw-rw-rw-   0        0        0    23163 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
--rw-rw-rw-   0        0        0    22011 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
--rw-rw-rw-   0        0        0    20283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
--rw-rw-rw-   0        0        0    18123 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
--rw-rw-rw-   0        0        0    22947 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
--rw-rw-rw-   0        0        0    22587 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
--rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
--rw-rw-rw-   0        0        0    21435 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
--rw-rw-rw-   0        0        0    18699 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
--rw-rw-rw-   0        0        0     4587 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
--rw-rw-rw-   0        0        0     5739 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
--rw-rw-rw-   0        0        0     6459 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
--rw-rw-rw-   0        0        0     5307 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
--rw-rw-rw-   0        0        0     5811 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
--rw-rw-rw-   0        0        0     4947 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
--rw-rw-rw-   0        0        0     5379 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
--rw-rw-rw-   0        0        0     5163 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
--rw-rw-rw-   0        0        0    40443 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    43467 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    39435 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    42171 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    42747 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
--rw-rw-rw-   0        0        0    39939 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
--rw-rw-rw-   0        0        0    41235 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
--rw-rw-rw-   0        0        0    38931 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
--rw-rw-rw-   0        0        0    40875 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
--rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.536963 agh_vqis-3.2.0/src/agh_vqis/models/ugc/
--rw-rw-rw-   0        0        0   594166 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/ugc/12k_all_set.json
-drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     6317 2023-07-24 12:34:08.000000 agh_vqis-3.2.0/src/agh_vqis/utils/helpers.py
--rw-rw-rw-   0        0        0      754 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/utils/resolution_cast.py
--rw-rw-rw-   0        0        0     5735 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:45.941806 agh_vqis-3.2.1/
+-rw-rw-rw-   0        0        0     2826 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/LICENSE
+-rw-rw-rw-   0        0        0    13226 2023-07-26 07:38:45.941806 agh_vqis-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12218 2023-07-26 07:19:32.000000 agh_vqis-3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.886016 agh_vqis-3.2.1/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0    13226 2023-07-26 07:38:44.000000 agh_vqis-3.2.1/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8201 2023-07-26 07:38:44.000000 agh_vqis-3.2.1/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:38:44.000000 agh_vqis-3.2.1/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-07-26 07:38:44.000000 agh_vqis-3.2.1/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 07:38:44.000000 agh_vqis-3.2.1/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.870329 agh_vqis-3.2.1/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.886016 agh_vqis-3.2.1/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-07-16 23:41:56.000000 agh_vqis-3.2.1/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-07-16 23:41:56.000000 agh_vqis-3.2.1/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-07-16 23:41:56.000000 agh_vqis-3.2.1/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-07-26 07:38:45.941806 agh_vqis-3.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.870329 agh_vqis-3.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.886016 agh_vqis-3.2.1/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-07-26 07:22:12.000000 agh_vqis-3.2.1/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    22904 2023-07-26 07:34:59.000000 agh_vqis-3.2.1/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.901663 agh_vqis-3.2.1/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    60648 2023-07-24 11:09:44.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt
+-rw-rw-rw-   0        0        0    66424 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt
+-rw-rw-rw-   0        0        0    97508 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt
+-rw-rw-rw-   0        0        0    88328 2023-07-21 14:04:46.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt
+-rwxrwxrwx   0        0        0   122077 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_win64_mt.exe
+-rw-rw-rw-   0        0        0  2952245 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/binaries/cygwin1.dll
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:44.870329 agh_vqis-3.2.1/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:45.926182 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:45.926182 agh_vqis-3.2.1/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-07-26 07:38:45.926182 agh_vqis-3.2.1/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     6317 2023-07-24 12:34:08.000000 agh_vqis-3.2.1/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-07-16 23:33:06.000000 agh_vqis-3.2.1/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-3.2.0/LICENSE` & `agh_vqis-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/PKG-INFO` & `agh_vqis-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh_vqis
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Filip Korus, Jakub Nawała
 Author-email: fkorus@student.agh.edu.pl, jakub.nawala@agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -88,15 +88,15 @@
    ```shell
    python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
    ```
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
-6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `webm`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
 7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
    ```python
```

### Comparing `agh_vqis-3.2.0/README.md` & `agh_vqis-3.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
    ```shell
    python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
    ```
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
-6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `webm`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
 7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
    ```python
```

### Comparing `agh_vqis-3.2.0/agh_vqis.egg-info/PKG-INFO` & `agh_vqis-3.2.1/agh_vqis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh-vqis
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Filip Korus, Jakub Nawała
 Author-email: fkorus@student.agh.edu.pl, jakub.nawala@agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -88,15 +88,15 @@
    ```shell
    python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
    ```
    Whereas this command will display help:
    ```shell
    $ python3 -m agh_vqis -h
    ```
-6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+6. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `webm`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
 
 
 7. First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given IQI when applied to the respective frame.
 
 
 8. Cast chosen indicators for different resolutions (**experimental**). For example: to cast Blur to 1440p and Blockiness to 2160p you should pass two additional lines in `options` dictionary like below.
    ```python
```

### Comparing `agh_vqis-3.2.0/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-3.2.1/agh_vqis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/python-cpbd/cpbd/compute.py` & `agh_vqis-3.2.1/python-cpbd/cpbd/compute.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/python-cpbd/cpbd/octave.py` & `agh_vqis-3.2.1/python-cpbd/cpbd/octave.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/setup.cfg` & `agh_vqis-3.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2033 2e32 2e30 0d0a 6175  sion = 3.2.0..au
+00000020: 7369 6f6e 203d 2033 2e32 2e31 0d0a 6175  sion = 3.2.1..au
 00000030: 7468 6f72 203d 2046 696c 6970 204b 6f72  thor = Filip Kor
 00000040: 7573 2c20 4a61 6b75 6220 4e61 7761 c582  us, Jakub Nawa..
 00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
 00000060: 3d20 666b 6f72 7573 4073 7475 6465 6e74  = fkorus@student
 00000070: 2e61 6768 2e65 6475 2e70 6c2c 206a 616b  .agh.edu.pl, jak
 00000080: 7562 2e6e 6177 616c 6140 6167 682e 6564  ub.nawala@agh.ed
 00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
```

### Comparing `agh_vqis-3.2.0/src/agh_vqis/__main__.py` & `agh_vqis-3.2.1/src/agh_vqis/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ._logger import setup_console_and_file_logger
 from .utils import ugc
 from .utils.helpers import *
 from .utils.resolution_cast import *
 
 logger = setup_console_and_file_logger(__name__, log_file_name=f"{__name__}.log", level=logging.INFO)
 
-allowed_mm_file_extensions = ['.jpg', '.jpeg', '.png', '.ts', '.mp4', '.y4m', '.mov', '.avi', '.mkv', '.gif', '.bmp']
+allowed_mm_file_extensions = ['.mp4', '.y4m', '.mov', '.mkv', '.avi', '.ts', '.webm', '.jpg', '.jpeg', '.png', '.gif', '.bmp']
 
 
 def _run_agh_vqis(mm_file_path: Path, vqis_binary=None, selected_vqis=32767):
     """
     Runs 15 VQ AGH's Video Quality Indicators (VQIs) on an input video or image (identified by *video_path*) and returns
     Pandas DataFrame with results.
 
@@ -470,19 +470,18 @@
         # Ignore subdirectories
         if child.is_dir():
             logger.info(f"Skipping a subdirectory ({str(child)})")
             continue
         # Ignore non-video and non-image files
         # TODO Add here any video or image extensions we want to support
         if child.suffix not in allowed_mm_file_extensions:
-            logger.info(f"Not a multimedia file ({str(child)}), skipping")
+            logger.info(f"Not a multimedia file ({str(child)}). Skipping.")
             continue
         # Process a single video file
-        # TODO Consider adding functionality of keeping all results in a single CSV file (as done in the legacy BATCH
-        #  file)
+        # TODO Consider adding functionality of keeping all results in a single CSV file
         mm_file_path = child  # mm = multimedia
         status = process_single_mm_file(mm_file_path, cli, options, args)
     return 0
 
 
 def main():
     # TODO Implement user input processing interface that allows to choose individual VQIs from the 15 AGH VQIs in a
```

### Comparing `agh_vqis-3.2.0/src/agh_vqis/_logger.py` & `agh_vqis-3.2.1/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt` & `agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt` & `agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt` & `agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt` & `agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_win64_mt.exe` & `agh_vqis-3.2.1/src/agh_vqis/binaries/agh_vqis_win64_mt.exe`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/binaries/cygwin1.dll` & `agh_vqis-3.2.1/src/agh_vqis/binaries/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb` & `agh_vqis-3.2.1/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/models/ugc/12k_all_set.json` & `agh_vqis-3.2.1/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/utils/helpers.py` & `agh_vqis-3.2.1/src/agh_vqis/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/utils/resolution_cast.py` & `agh_vqis-3.2.1/src/agh_vqis/utils/resolution_cast.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.2.0/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.2.1/src/agh_vqis/utils/ugc.py`

 * *Files identical despite different names*

