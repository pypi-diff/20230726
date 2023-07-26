# Comparing `tmp/reaxpro-wrappers-1.0.1.tar.gz` & `tmp/reaxpro-wrappers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.0.1.tar", last modified: Mon Jul 24 18:47:12 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.1.0.tar", last modified: Wed Jul 26 10:16:50 2023, max compression
```

## Comparing `reaxpro-wrappers-1.0.1.tar` & `reaxpro-wrappers-1.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/ams/energy_landscape.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.361703 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48929 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27026 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74897 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.365703 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 18:47:12.000000 reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:47:12.369703 reaxpro-wrappers-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-24 18:46:57.000000 reaxpro-wrappers-1.0.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.868833 reaxpro-wrappers-1.1.0/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/energy_landscape.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77014 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.0.1/LICENSE` & `reaxpro-wrappers-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/PKG-INFO` & `reaxpro-wrappers-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.0.1
+Version: 1.1.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.0.1/README.md` & `reaxpro-wrappers-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.1.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.1.0/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.1.0/osp/models/ams/energy_landscape_refinement.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,29 +74,41 @@
     pathways: List[MoleculeReaction] = Field(
         ..., description="""List of molecule pathways included for the refinement."""
     )
 
     def __post_init_post_parse__(self):
         with CoreSession() as session:
             calculation = emmo.LandscapeRefinement()
-            energy_landscape = emmo.EnergyLandscape()
             model = emmo.DFTB()
-            energy_landscape.add(*self._make_landscape(), rel=emmo.hasPart)
-            calculation.add(energy_landscape, model, rel=emmo.hasInput)
-        file = tempfile.NamedTemporaryFile(suffix=".ttl")
+            calculation.add(self._make_landscape(), model, rel=emmo.hasInput)
+        file = tempfile.NamedTemporaryFile(suffix=".ttl",delete=False)
         export_cuds(session, file.name)
+        self._file = file.name
         try:
             self._uuid = get_upload(file)
         except Exception as error:
             self._uuid = None
             message = f"The graph of the model could not be stored at the minio-instance: {error.args}"
             warnings.warn(message)
         self._session = session
 
-    def _make_landscape(self) -> "List[Cuds]":
+    def _make_landscape(self) -> "Cuds":
+        energy_landscape = emmo.EnergyLandscape()
+        pathways = self._make_reaction_paths()
+        for index in range(len(pathways)):
+            if index == 0:
+                energy_landscape.add(pathways[index], rel=emmo.hasSpatialFirst)
+            else:
+                pathways[index-1].add(pathways[index], rel=emmo.hasSpatialNext)
+                energy_landscape.add(pathways[index], rel=emmo.hasSpatialDirectPart)
+            if index == len(pathways) + 1:
+                energy_landscape.add(pathways[index], rel=emmo.hasSpatialLast)
+        return energy_landscape
+
+    def _make_reaction_paths(self) -> "List[Cuds]":
         reactions = self._make_reaction()
         paths = []
         for index in range(len(reactions)):
             if index == 0:
                 molecule1 = reactions[index]["reactant"]
                 path1 = emmo.ReactionPathway()
                 path1.add(molecule1, rel=emmo.hasPart)
@@ -170,13 +182,17 @@
     def cuds(cls):
         return cls._session.load(cls._session.root).first()
 
     @property
     def uuid(cls):
         return cls._uuid
 
+    @property
+    def file(cls):
+        return cls._file
+
     class Config:
         """Pydantic Config for EnergyLandscapeRefinement"""
 
         schema_extra = {
             "example": _get_example_json("energy_landscape.json", STANDARD_XYZ)
         }
```

### Comparing `reaxpro-wrappers-1.0.1/osp/models/settings/general.py` & `reaxpro-wrappers-1.1.0/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/models/utils/general.py` & `reaxpro-wrappers-1.1.0/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.1.0/osp/models/zacros/co_pyzacros.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,14 +563,15 @@
         with CoreSession() as session:
 
             calculation = emmo.MesoscopicCalculation()
             calculation.add(*self._make_model(), rel=emmo.hasInput)
 
         file = tempfile.NamedTemporaryFile(suffix=".ttl")
         export_cuds(session, file.name)
+        self._file = file.name
         try:
             self._uuid = get_upload(file)
         except Exception as error:
             self._uuid = None
             message = message = f"The graph of the model could not be stored at the minio-instance: {error.args}"
             warnings.warn(message)
         self._session = session
@@ -1202,13 +1203,17 @@
 
         return cuds_object
 
     @property
     def cuds(cls):
         return cls._session.load(cls._session.root).first()
 
+    @property
+    def file(cls):
+        return cls._file
+
     class Config:
         """Pydantic Config for COpyZacrosModel"""
 
         schema_extra = {
             "example": _get_example_json("Ziff-Gulari-Barshad-model-variants.json", STANDARD_DATA)
         }
```

### Comparing `reaxpro-wrappers-1.0.1/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.1.0/osp/tools/graph_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Functions to graph dependencies between CUDS objects."""
 
 import os
 from osp.core.cuds import Cuds
 from osp.core.ontology.relationship import OntologyRelationship
 from osp.core.utils import simple_search as search
 from osp.tools.io_functions import raise_error
-from osp.core.namespaces import emmo
+from osp.core.namespaces import emmo, cuba
 from osp.core.utils.general import get_relationships_between
 from typing import List
 # from osp.core.utils import pretty_print
 
 
 def graph_wrapper_dependencies(root_cuds_object: Cuds) -> dict:
     """
@@ -22,15 +22,15 @@
     """
 
     # Find Simulation objects in cuba.Wrapper:
     search_simulation = \
         search.find_cuds_object(criterion=lambda x:
                                 x.is_a(oclass=emmo.Simulation),
                                 root=root_cuds_object,
-                                rel=emmo.hasPart,
+                                rel=cuba.relationship,
                                 find_all=True,
                                 max_depth=1)
 
     # Zero Simulations found:
     if len(search_simulation) == 0:
 
         wrapper_dependencies = {"Calculation": [Cuds],
@@ -125,15 +125,15 @@
                         message="emmo.hasTemporalFirst calculation without"
                                 " an emmo.hasTemporalNext.")
     else:
         search_calculation = \
             search.find_cuds_object(criterion=lambda x:
                                     x.oclass in calculations_types,
                                     root=root_cuds_object,
-                                    rel=emmo.hasPart,
+                                    rel=cuba.relationship,
                                     find_all=True,
                                     max_depth=1)
         relationship_list.append(
             get_relationships_between(root_cuds_object, search_calculation[0]))
 
         if len(search_calculation) == 0:
             raise_error(file=os.path.basename(__file__),
```

### Comparing `reaxpro-wrappers-1.0.1/osp/tools/io_functions.py` & `reaxpro-wrappers-1.1.0/osp/tools/io_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         coordinates.append([float(x), float(y), float(z)])
         regions.append(region.split("=")[1])
     xyz.close()
     print("molecule_from_xyz: External", filename, "file has been read.")
 
     # Creating atom containers and adding them to the root_cuds_object
     # (i.e. MolecularGeometry)
+    atoms = []
     for iatom in range(n_atoms):
         atom = emmo.AtomEntity()
         atom_symbol = emmo.ChemicalElement(hasSymbolData=labels[iatom])
 
         position_vec = emmo.PositionVector()
         coordinate_x = emmo.Real(hasNumericalData=coordinates[iatom][0])
         coordinate_y = emmo.Real(hasNumericalData=coordinates[iatom][1])
@@ -208,18 +209,26 @@
         position_vec.add(coordinate_z, rel=emmo.hasSpatialLast)
 
         if regions[iatom] == "NIL":
             atom.add(position_vec, atom_symbol, rel=emmo.hasPart)
         else:
             region = emmo.Region(hasSymbolData=regions[iatom].lower())
             atom.add(position_vec, atom_symbol, region, rel=emmo.hasPart)
+        if iatom == 0:
+            rel = emmo.hasSpatialFirst
+        elif iatom == n_atoms:
+            rel = emmo.hasSpatialLast
+        else:
+            rel = emmo.hasSpatialDirectPart
+            atoms[iatom-1].add(atom, rel=emmo.hasSpatialNext)
+        atoms.append(atom)
         if TS:
-            transition_state.add(atom, rel=emmo.hasSpatialPart)
+            transition_state.add(atom, rel=rel)
         else:
-            molecule.add(atom, rel=emmo.hasSpatialPart)
+            molecule.add(atom, rel=rel)
     if TS:
         assign_chemical_name(transition_state, labels)
         return transition_state
     else:
         assign_chemical_name(molecule, labels)
         return molecule
 
@@ -724,26 +733,26 @@
 
     :param type: Error type.
 
     :param message: String describing the error.
     """
 
     nl = "\n"
-    if type == "NotImplementedError":
-        raise NameError(message)
 
+    msg = (
+        f"{nl}### ERROR ### {function} function/method"
+        f" in {file}:"
+        f'{nl}              "{message}"'
+    )
     if type == "NameError":
-        msg = (
-            f"{nl}### ERROR ### {function} function/method"
-            f" in {file}:"
-            f'{nl}              "{message}"'
-        )
         raise NameError(msg)
-    return
-
+    elif type == "ValueError":
+        raise ValueError(msg)
+    elif type == "NotImplementedError":
+        raise NameError(message)
 
 def raise_warning(file: str, function: str, message: str, message2=None):
     """
     Raise warning according to arguments:
 
     :param file: Python file where the error occurs.
```

### Comparing `reaxpro-wrappers-1.0.1/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.1.0/osp/tools/mapping_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from arcp import arcp_random
 from osp.tools.io_functions import raise_error, raise_warning
 from osp.tools.io_functions import read_mechanism, read_cluster_expansion, read_molecule
 from osp.tools.set_functions import AMS_default_setting
 from osp.core.utils import simple_search as search
 from osp.core.ontology.oclass import OntologyClass
 from osp.core.cuds import Cuds
-from osp.core.namespaces import emmo, crystallography
+from osp.core.namespaces import emmo, crystallography, cuba
 from osp.core.utils import pretty_print
+from typing import List
 
 
 def map_function(self, root_cuds_object: Cuds, engine=None) -> tuple:
     """
     Map a Calculations CUDS object to a engine-understandable input.
 
     :param root_cuds_object: Calculation CUDS object.
@@ -38,15 +39,27 @@
         search_landscape = \
             search.find_cuds_objects_by_oclass(emmo.EnergyLandscape, root_cuds_object, emmo.hasPart)
 
         if search_landscape:
             plams_molecule = map_PLAMSLandscape(search_landscape[0])
 
         else:
-            plams_molecule = map_PLAMSMolecule(root_cuds_object)
+            search_molecule = \
+                search.find_cuds_objects_by_oclass(emmo.MolecularGeometry, root_cuds_object, emmo.hasPart)
+
+            if len(search_molecule) > 1:
+                raise_error(file=os.path.basename(__file__),
+                            function=map_function.__name__,
+                            type='ValueError',
+                            message='More than one emmo.MolecularGeometry defined in the Wrapper object.')
+            elif not search_molecule:
+                raise_error(file=os.path.basename(__file__), function=map_molecule.__name__,
+                            type='ValueError', message='Molecule CUDS object missed in the wrapper.')
+            else:
+                plams_molecule = map_PLAMSMolecule(search_molecule[0])
 
         plams_settings = map_PLAMSSettings(root_cuds_object)
 
         return (plams_molecule, plams_settings)
 
     elif engine == "Zacros":
 
@@ -132,32 +145,29 @@
 
     :param root_cuds_object: EnergyLandscape CUDS object.
 
     :return {PlamsMolecule}:
     """
 
     landscape_dict = {}
-    search_reaction_path = \
-        search.find_cuds_objects_by_oclass(emmo.ReactionPathway,
-                                           root_cuds_object, emmo.hasPart)
+    search_reaction_path = find_reaction_path(root_cuds_object)
 
     if search_reaction_path:
 
         # Generate list of labels for single-molecule states:
         path_label_list = []
 
         for index, reaction_path in enumerate(search_reaction_path):
 
             path_label = "state" + str(1 + index)
 
             search_molecule = search.find_cuds_object(
                 criterion=lambda x:
                 x.is_a(oclass=emmo.MolecularGeometry), root=reaction_path, rel=emmo.hasPart,
                 find_all=True, max_depth=1)
-
             if search_molecule:
 
                 if len(search_molecule) > 1:
                     raise_error(
                         file=os.path.basename(__file__), function=map_PLAMSLandscape.__name__,
                         type='NameError', message='More than one Molecule '
                         'defined in ReactionPathway CUDS object.')
@@ -259,97 +269,98 @@
      "atom_coordinates":
                     [[coordinate_x_1, coordinate_y_1, coordinate_z_1, (region)],
                     [coordinate_x_2, coordinate_y_2, coordinate_z_2, (region)],
                      ...
                     [coordinate_x_2, coordinate_y_n, coordinate_z_n, (region)]]
     }
 
-    :param root_cuds_object: CUDS wrapper to be checked.
+    :param root_cuds_object: CUDS MolecularGeometry to be checked.
 
     :return str: If a Molecule object is present, return dictionary with
                  atom labels and positions. Otherwise, raise an error.
     """
+    molecule_data = {}
 
-    search_molecule = \
-        search.find_cuds_objects_by_oclass(emmo.MolecularGeometry, root_cuds_object, emmo.hasPart)
-
-    if (len(search_molecule) > 1):
-        # Raise error if two molecules, for some reason, are found:
-        raise_error(file=os.path.basename(__file__), function=map_molecule.__name__,
-                    type='NameError', message='More than one emmo.MolecularGeometry defined'
-                                              ' in the Wrapper object.')
-
-    if search_molecule:
-        molecule_data = {}
-
-        # Looking for atoms:
-        atom_list = \
-            search.find_cuds_objects_by_oclass(emmo.AtomEntity, search_molecule[0], emmo.hasPart)
-
-        # Looking for charges:
-        search_charge =  \
-            search.find_cuds_objects_by_oclass(emmo.ElectricCharge, search_molecule[0],
-                                               emmo.hasProperty)
-
-        # Is there any charge?
-        if search_charge:
-            molecular_charge = search_charge[0].get(oclass=emmo.Integer,
-                                                    rel=emmo.hasQuantityValue)[0].hasNumericalData
-
-        # For each of the atoms, we add labels and positions:
-        for count, iatom in enumerate(atom_list):
-
-            search_label = \
-                search.find_cuds_objects_by_oclass(emmo.ChemicalElement, iatom, emmo.hasPart)
-
-            search_position_vec = \
-                search.find_cuds_objects_by_oclass(emmo.PositionVector, iatom, emmo.hasPart)
-
-            search_region = \
-                search.find_cuds_objects_by_oclass(emmo.Region, iatom, emmo.hasPart)
-
-            # Is there any region defined? For EON PES exploration.
+    # Looking for atoms:
+    first = root_cuds_object.get(rel=emmo.hasSpatialFirst)
+    if len(first) > 1:
+        raise_error(file=os.path.basename(__file__),
+                    function=map_molecule.__name__,
+                    type='ValueError',
+                    message='More than one first spatial atom found in molecule.')
+    elif len(first) == 0:
+        raise_error(file=os.path.basename(__file__),
+                    function=map_molecule.__name__,
+                    type='ValueError',
+                    message='First spatial atom in molecule not found.')
+    else:
+        atom_list = []
+        current = first
+        while current:
+            current = current.pop()
+            atom_list.append(current)
+            current = current.get(rel=emmo.hasSpatialNext)
+    # Looking for charges:
+    search_charge =  \
+        search.find_cuds_objects_by_oclass(emmo.ElectricCharge, root_cuds_object,
+                                            emmo.hasProperty)
+
+    # Is there any charge?
+    if search_charge:
+        molecular_charge = search_charge[0].get(oclass=emmo.Integer,
+                                                rel=emmo.hasQuantityValue)[0].hasNumericalData
+
+    # For each of the atoms, we add labels and positions:
+    for count, iatom in enumerate(atom_list):
+
+        search_label = \
+            search.find_cuds_objects_by_oclass(emmo.ChemicalElement, iatom, emmo.hasPart)
+
+        search_position_vec = \
+            search.find_cuds_objects_by_oclass(emmo.PositionVector, iatom, emmo.hasPart)
+
+        search_region = \
+            search.find_cuds_objects_by_oclass(emmo.Region, iatom, emmo.hasPart)
+
+        # Is there any region defined? For EON PES exploration.
+        if search_region:
+            region = search_region[0].hasSymbolData
+
+        # Atom coordinates:
+        coordinate_x = \
+            search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialFirst)
+        coordinate_y = \
+            search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialNext)
+        coordinate_z = \
+            search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialLast)
+
+        if count == 0:
+            molecule_data = {
+                'atom_symbol': [search_label[0].hasSymbolData],
+                'atom_coordinates': [[
+                    coordinate_x[0].hasNumericalData,
+                    coordinate_y[0].hasNumericalData,
+                    coordinate_z[0].hasNumericalData
+                ]]
+            }
             if search_region:
-                region = search_region[0].hasSymbolData
-
-            # Atom coordinates:
-            coordinate_x = \
-                search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialFirst)
-            coordinate_y = \
-                search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialNext)
-            coordinate_z = \
-                search_position_vec[0].get(oclass=emmo.Real, rel=emmo.hasSpatialLast)
-
-            if count == 0:
-                molecule_data = {
-                    'atom_symbol': [search_label[0].hasSymbolData],
-                    'atom_coordinates': [[
-                        coordinate_x[0].hasNumericalData,
+                molecule_data['region'] = [region]
+            if search_charge:
+                molecule_data['molecular_charge'] = [molecular_charge]
+        else:
+            molecule_data['atom_symbol'].\
+                append(search_label[0].hasSymbolData)
+            molecule_data['atom_coordinates'].\
+                append([coordinate_x[0].hasNumericalData,
                         coordinate_y[0].hasNumericalData,
                         coordinate_z[0].hasNumericalData
-                    ]]
-                }
-                if search_region:
-                    molecule_data['region'] = [region]
-                if search_charge:
-                    molecule_data['molecular_charge'] = [molecular_charge]
-            else:
-                molecule_data['atom_symbol'].\
-                    append(search_label[0].hasSymbolData)
-                molecule_data['atom_coordinates'].\
-                    append([coordinate_x[0].hasNumericalData,
-                            coordinate_y[0].hasNumericalData,
-                            coordinate_z[0].hasNumericalData
-                            ])
-                if search_region:
-                    molecule_data['region'].append(region)
+                        ])
+            if search_region:
+                molecule_data['region'].append(region)
 
-    else:
-        raise_error(file=os.path.basename(__file__), function=map_molecule.__name__,
-                    type='NameError', message='Molecule CUDS object missed in the wrapper.')
     return molecule_data
 
 
 def map_lattice(root_cuds_object: Cuds) -> dict:
     """Map Lattice from a Calculation CUDS object.
 
     It returns a dictionary containing 3x3 lattice vector array
@@ -1124,14 +1135,53 @@
                                                           emmo.hasInput)
 
     if search_wall_time:
         syntactic_settings.Wall_Time = map_generic_setting(emmo.WallTime, root_cuds_object)
 
     return syntactic_settings
 
+def find_reaction_path(root_cuds_object: Cuds) -> List[Cuds]:
+    """
+    Find reaction pathways in root cuds object with specific order
+
+    :param root_cuds_object: Calculation CUDS object.
+
+    :return List[Cuds]:
+    """
+    landscape = search.find_cuds_objects_by_oclass(emmo.EnergyLandscape, root_cuds_object, emmo.hasPart)
+    if len(landscape) > 1:
+        raise_error(file=os.path.basename(__file__),
+                    function=find_reaction_path.__name__,
+                    type='ValueError',
+                    message='More than one energy landscape found.')
+    elif not landscape:
+        raise_error(file=os.path.basename(__file__),
+                    function=find_reaction_path.__name__,
+                    type='ValueError',
+                    message='No energy landscape found.')
+    else:
+        first = landscape.pop().get(oclass=emmo.ReactionPathway, rel=emmo.hasSpatialFirst)
+        if len(first) > 1:
+            raise_error(file=os.path.basename(__file__),
+                        function=find_reaction_path.__name__,
+                        type='ValueError',
+                        message='More than one first spatial reaction pathways found.')
+        elif not first:
+            raise_error(file=os.path.basename(__file__),
+                        function=find_reaction_path.__name__,
+                        type='ValueError',
+                        message='First spatial pathway in energy landscape not found.')
+        else:
+            paths = []
+            current = first
+            while current:
+                current = current.pop()
+                paths.append(current)
+                current = current.get(rel=emmo.hasSpatialNext)
+            return paths
 
 def map_PyZacrosMechanism(root_cuds_object: Cuds) -> pz.Mechanism:
     """
     Map ontology-defined Mechanism to pz.Mechanism() object.
 
     :param root_cuds_object: Calculation CUDS object.
 
@@ -1520,24 +1570,24 @@
    """
 
     if isinstance(engine, MultiJob):
 
         # in case of several children, outputs will be added in the order of dependencies.
         search_simulation = \
             search.find_cuds_object(criterion=lambda x: x.is_a(oclass=emmo.Simulation),
-                                    root=root_cuds_object, rel=emmo.hasPart, find_all=True,
+                                    root=root_cuds_object, rel=cuba.relationship, find_all=True,
                                     max_depth=1)
 
         if not len(search_simulation):
 
             # Attach results to Calculation CUDS object using hasOutput rel.
             search_calculation = \
                     search.find_cuds_objects_by_oclass(
                                        emmo.Calculation,
-                                       root_cuds_object, rel=emmo.hasPart)
+                                       root_cuds_object, rel=cuba.relationship)
             map_tarball(engine, search_calculation[0])
 
             if map_calculation_type(root_cuds_object) == "WavefunctionOptimization":
                 add_AMSenergy_to_object(engine.children[0], search_calculation[0])
 
             elif map_calculation_type(root_cuds_object) == "GeometryOptimization":
 
@@ -1614,22 +1664,22 @@
                 add_AMSenergy_to_object(engine.children[2], last_calculation[0])
 
             map_tarball(engine, last_calculation[0])
 
     elif isinstance(engine, pz.ZacrosResults):
         search_calculation = search.find_cuds_objects_by_oclass(
                                    emmo.MesoscopicCalculation, root_cuds_object,
-                                   rel=emmo.hasPart)
+                                   rel=cuba.relationship)
         map_tarball(engine, search_calculation[0])
 
     else:
         raise_error(file=os.path.basename(__file__), function=map_results.__name__,
                     type='NameError',
                     message='Mapping of the results is not implemented for this engine.')
-    return
+
 
 
 def add_AMSenergy_to_object(job: AMSJob, root_cuds_object: Cuds):
     """
     Add Total Energy result to the Cuds (Calculation) object.
 
     :job: Multijob object.
```

### Comparing `reaxpro-wrappers-1.0.1/osp/tools/set_functions.py` & `reaxpro-wrappers-1.1.0/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.1.0/osp/wrappers/simams/simams_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/simzacros_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Describe Zacros Session class."""
-from osp.core.namespaces import emmo, crystallography
+from osp.core.namespaces import emmo, crystallography, cuba
 from osp.core.session import SimWrapperSession
 from osp.core.cuds import Cuds
 from osp.tools.io_functions import raise_error
 from osp.tools.mapping_functions import map_function, map_results
 from osp.core.utils import simple_search as search
 import scm.pyzacros as pz
 import os
@@ -67,16 +67,15 @@
 
         self.input_path = '../tests/test_files'
 
         # Calculation
         search_calculation = \
             search.find_cuds_objects_by_oclass(
                            emmo.MesoscopicCalculation,
-                           root_obj, emmo.hasPart)
-
+                           root_obj, cuba.relationship)
         #  Raise error if two calculations, for some reason, are found:
         if len(search_calculation) > 1:
             raise_error(file=os.path.basename(__file__),
                         function="_apply_added method",
                         type='NameError',
                         message='More than one emmo.MesoscopicCalculation defined'
                         ' in the Wrapper object.')
```

### Comparing `reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.0.1
+Version: 1.1.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.0.1/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/setup.cfg` & `reaxpro-wrappers-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.0.1
+version = v1.1.0
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.0.1/setup.py` & `reaxpro-wrappers-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.1.0/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/tests/test_examples.py` & `reaxpro-wrappers-1.1.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.1.0/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.0.1/tests/test_tools.py` & `reaxpro-wrappers-1.1.0/tests/test_tools.py`

 * *Files identical despite different names*

