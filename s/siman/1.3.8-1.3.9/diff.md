# Comparing `tmp/siman-1.3.8.tar.gz` & `tmp/siman-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.8.tar", last modified: Tue Jul 18 16:00:07 2023, max compression
+gzip compressed data, was "dist/siman-1.3.9.tar", last modified: Wed Jul 26 16:54:36 2023, max compression
```

## Comparing `siman-1.3.8.tar` & `siman-1.3.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.8/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.8/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-18 16:00:07.185332 siman-1.3.8/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.8/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-18 16:00:07.185332 siman-1.3.8/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-18 16:00:05.000000 siman-1.3.8/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.8/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.8/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.8/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.8/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.8/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.8/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.8/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.8/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.8/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.8/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.184332 siman-1.3.8/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.8/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.184332 siman-1.3.8/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.8/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.8/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.3.8/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.8/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.8/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.8/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.8/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.8/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.8/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16435 2023-07-18 15:59:51.000000 siman-1.3.8/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.8/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.8/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    87557 2023-07-16 18:04:57.000000 siman-1.3.8/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.8/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.8/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.8/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.8/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.8/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.8/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.8/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-18 15:59:51.000000 siman-1.3.8/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.8/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.8/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.8/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.8/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.8/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.8/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.8/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.8/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.8/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.8/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.633509 siman-1.3.9/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.9/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.9/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-26 16:54:36.633509 siman-1.3.9/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.9/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-26 16:54:36.633509 siman-1.3.9/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-26 16:54:24.000000 siman-1.3.9/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.630509 siman-1.3.9/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.9/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.9/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.9/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.9/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.9/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.9/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.9/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.9/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.9/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.9/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.9/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.632509 siman-1.3.9/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.9/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.632509 siman-1.3.9/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.9/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.9/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.3.9/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.3.9/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.9/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.9/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.9/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.9/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.9/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.9/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16531 2023-07-26 16:52:32.000000 siman-1.3.9/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.9/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.9/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    88140 2023-07-26 16:53:10.000000 siman-1.3.9/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.9/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.633509 siman-1.3.9/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.9/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.9/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.9/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.9/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.9/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.9/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-18 15:59:51.000000 siman-1.3.9/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.9/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.9/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.9/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.9/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.9/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.9/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.9/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.9/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.9/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.9/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.8/LICENSE` & `siman-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/PKG-INFO` & `siman-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.8
+Version: 1.3.9
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.8/setup.py` & `siman-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.8",
+    version="1.3.9",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.8/siman/3d_plot.py` & `siman-1.3.9/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/SSHTools.py` & `siman-1.3.9/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/analysis.py` & `siman-1.3.9/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/analysis_functions.py` & `siman-1.3.9/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/analyze/segregation.py` & `siman-1.3.9/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/approximation.py` & `siman-1.3.9/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/bands.py` & `siman-1.3.9/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calc_manage.py` & `siman-1.3.9/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calcul.py` & `siman-1.3.9/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calculators/aims.py` & `siman-1.3.9/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calculators/gaussian.py` & `siman-1.3.9/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calculators/qe.py` & `siman-1.3.9/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calculators/vasp.py` & `siman-1.3.9/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/calculators/vasp_old.py` & `siman-1.3.9/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/chg/chg_func.py` & `siman-1.3.9/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.9/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/classes.py` & `siman-1.3.9/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/core/calculation.py` & `siman-1.3.9/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/core/calculation_old.py` & `siman-1.3.9/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/core/cluster_batch_script.py` & `siman-1.3.9/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/core/cluster_run_script.py` & `siman-1.3.9/siman/core/cluster_run_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     Generate run file
 
     INPUT:
         - cl_dir (str) - calculation directory cl.dir
         - schedule_system (str) - ['SGE', 'PBS', 'SLURM', 'none']
     """
 
+    printlog('make_run():', schedule_system, run_name, imp = 'n')
+    # sys.exit()
+
+
     with open('run','a', newline = '') as f:
 
         if schedule_system == 'SGE':
             #'qsub -pe 'mpi*' NCORES -l CLUSTER_TAG script.parallel.sh' for mpi-jobs which should run on CLUSTER_TAG (cmmd or cmdft)
             #IMPORTANT: NCORES must be a multiple of 8(24) on cmdft(cmmd). 
             # f.write("qsub -pe 'mpi*' "+str(header.corenum)+" "+header.queue+" "+run_name+"\n") #str(self.set.np) #-l cmmd; on MPIE
```

### Comparing `siman-1.3.8/siman/core/molecule.py` & `siman-1.3.9/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/core/structure.py` & `siman-1.3.9/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/database.py` & `siman-1.3.9/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/default_project_conf.py` & `siman-1.3.9/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/dev_functions.py` & `siman-1.3.9/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/dos_functions.py` & `siman-1.3.9/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/fit_hex.py` & `siman-1.3.9/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/functions.py` & `siman-1.3.9/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/geo.py` & `siman-1.3.9/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/header.py` & `siman-1.3.9/siman/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,41 +104,44 @@
     global siman_run, project_folder
 
     if pfolder:
         project_folder = pfolder
     elif 'project_conf.py' in filename:
         project_folder = os.path.dirname(filename)
     else:
+        project_folder = None
         pass
 
+    configfile_name = os.path.basename(filename)
+
     if project_folder:
         siman_run = 1 # means that siman is used as an application to run tasks, not just a library
 
 
 
     import importlib.util, sys
     spec = importlib.util.spec_from_file_location('project_conf', filename)
     project_conf = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(project_conf)
     # print(dir(project_conf))
-    config_vars = ['CIF2CELL', 'DEFAULT_CLUSTER', 'EXCLUDE_NODES', 
+    config_vars = ['MEM_CPU','CIF2CELL', 'DEFAULT_CLUSTER', 'EXCLUDE_NODES', 
     'NEW_BATCH', 'PATH2ARCHIVE', 'PATH2DATABASE', 'PATH2JMOL', 'PATH2NEBMAKE', 
     'PATH2PHONOPY', 'PATH2POTENTIALS', 'PATH2PROJECT', 'PBS_PROCS', 
     'RAMDISK', 'SIMAN_WEB', 'WALLTIME_LIMIT', 
     'geo_folder', 'path_to_images', 'path_to_paper', 
     'path_to_wrapper', 'pmgkey', 'reorganize', 'CLUSTERS', 'PATH2SHELVE_DBSUP', 'PATH2SHELVE_DB', 'PATH2HISTORYFILE']
 
     for var in config_vars:
         try: 
             value = getattr(project_conf, var)
             # print(type(value))
             setattr(header, var, value)
             # exec(var + " = " + str(value))
         except AttributeError:
-            print('Warning! Your project_conf.py doesnot contain', var)
+            print('Warning! Your '+ configfile_name +' doesnot contain', var)
             pass
         # print(var, value)
     # CLUSTERS = getattr(project_conf, 'CLUSTERS')
 
     # print(CLUSTERS)
 
     return
```

### Comparing `siman-1.3.8/siman/impurity.py` & `siman-1.3.9/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/inout.py` & `siman-1.3.9/siman/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1409,14 +1409,15 @@
         self.extpress = 0
 
         self.intstress = None
         spin_polarized = None
         ifmaglist = None
         for line in outcarlines:
 
+
             #Check bands
 
             # if 'band No.' in line:
             #     kpoint = float(outcarlines[i_line-1].split()[1])
             #     lastocc = float(outcarlines[i_line+self.nbands].split()[2])
             #     lastbandno = outcarlines[i_line+self.nbands].split()[0]
             #     if lastocc > 0:
@@ -1859,14 +1860,15 @@
                     i = 0
                     while 'ELASTIC MODULI CONTR FROM IONIC RELAXATION' not in line:
                         i+=1
                         line = outcarlines[i_line+i]
                         if 'f  =' in line:
                             freq.append(float(line.split()[3]) ) #THz
                             # print(line)
+                    self.freq = freq
 
 
             if 'TOTAL ELASTIC MODULI' in line:
                 eltensor = []
                 for i in range(9):
                     line = outcarlines[i_line+i]
                     # print(line.strip())
@@ -1878,14 +1880,15 @@
                 printlog('Elastic tensor, GPa:', imp = 'y')
 
                 np.set_printoptions(formatter={'float_kind':"{:6.1f}".format})
                 print(eltensor)
                 w, v = np.linalg.eig(eltensor)
                 printlog('Eigenvalues are:', w, imp = 'y')
                         # eltensor
+                self.eltensor = eltensor
 
             if 'average eigenvalue GAMMA=' in line:
                 # print(line)
                 gamma = float(line.split()[-1])
                 if gamma > 1 and 'conv' in show:
                     printlog('average eigenvalue GAMMA >1', gamma, imp = 'y')
                 # sys.exit()
@@ -2373,16 +2376,19 @@
         finefreq = np.linspace(fmin, fmax, 1000)
         dos = [0]*1000
 
         # for i in range(1000):
         # print(fw)
         for f in freq:
             # print(f)
-            i = int( np.round( (f-fmin)/ fw * 999 ,0) )
-            dos[i] += 1
+            try:
+                i = int( np.round( (f-fmin)/ fw * 999 ,0) )
+                dos[i] += 1
+            except ZeroDivisionError:
+                pass
             # print(i, finefreq[i], f)
         
 
         def butter_lowpass(cutoff, fs, order=5):
             nyq = 0.5 * fs
             normal_cutoff = cutoff / nyq
             b, a = butter(order, normal_cutoff, btype='low', analog=False)
@@ -2401,19 +2407,30 @@
 
         # plt.plot(finefreq, smoother(smoother(dos,10), 10), '-') 
         plt.plot(finefreq, y, '-') 
         # plt.plot(finefreq, dos, '-')
         plt.xlabel('Frequency, THz')
         plt.ylabel('DOS' )
         # plt.plot(finefreq, y, '-') 
-        filename = 'figs/'+str(self.id)+'.pdf'
-        plt.savefig(filename)
-        printlog('Freq file saved to ', filename, imp = 'y')
-        plt.show()
-        plt.clf()
+        # filename = 'figs/'+str(self.id)+'.pdf'
+        from siman import header
+        if header.SIMAN_WEB:
+            path_l = cl.path['output'].replace('400.OUTCAR','')
+            plt.tight_layout()
+            filename = path_l+str(self.name)+'.png'
+            plt.savefig(filename)
+            printlog('Freq file saved to ', filename, imp = 'y')
+
+        else:
+            path_l = 'figs/'
+            filename = path_l+str(self.id)+'.pdf'
+            plt.savefig(filename)
+            printlog('Freq file saved to ', filename, imp = 'y')
+            plt.show()
+            plt.clf()
 
     # sys.exit()
 
 
     printlog("Reading of results completed\n\n", imp = 'n')
     self.end.outfile = path_to_outcar
```

### Comparing `siman-1.3.8/siman/kpoints_functions.py` & `siman-1.3.9/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/mat_prop/mat_prop.py` & `siman-1.3.9/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/matproj_functions.py` & `siman-1.3.9/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/monte.py` & `siman-1.3.9/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/monte_functions.py` & `siman-1.3.9/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/neb.py` & `siman-1.3.9/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/pairs.py` & `siman-1.3.9/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/picture_functions.py` & `siman-1.3.9/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/plot_functions.py` & `siman-1.3.9/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/polaron.py` & `siman-1.3.9/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/polaron_hop.py` & `siman-1.3.9/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/polaron_mod.py` & `siman-1.3.9/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/project_funcs.py` & `siman-1.3.9/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/properties_2d.py` & `siman-1.3.9/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/properties_energy.py` & `siman-1.3.9/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/properties_lattice.py` & `siman-1.3.9/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/set_functions.py` & `siman-1.3.9/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/simanrc.py` & `siman-1.3.9/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/small_functions.py` & `siman-1.3.9/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/structure_functions.py` & `siman-1.3.9/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/table_functions.py` & `siman-1.3.9/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/thermo.py` & `siman-1.3.9/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman/workflow_utilities.py` & `siman-1.3.9/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.8/siman.egg-info/PKG-INFO` & `siman-1.3.9/siman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.8
+Version: 1.3.9
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.8/siman.egg-info/SOURCES.txt` & `siman-1.3.9/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

