# Comparing `tmp/reaxpro-wrappers-1.1.0.tar.gz` & `tmp/reaxpro-wrappers-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.1.0.tar", last modified: Wed Jul 26 10:16:50 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.1.1.tar", last modified: Wed Jul 26 12:29:01 2023, max compression
```

## Comparing `reaxpro-wrappers-1.1.0.tar` & `reaxpro-wrappers-1.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.868833 reaxpro-wrappers-1.1.0/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/ams/energy_landscape.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    77014 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.872833 reaxpro-wrappers-1.1.0/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 10:16:50.000000 reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:16:50.876833 reaxpro-wrappers-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-26 10:16:34.000000 reaxpro-wrappers-1.1.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.890489 reaxpro-wrappers-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 12:29:01.890489 reaxpro-wrappers-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.878489 reaxpro-wrappers-1.1.1/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.878489 reaxpro-wrappers-1.1.1/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.878489 reaxpro-wrappers-1.1.1/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/ams/energy_landscape.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.878489 reaxpro-wrappers-1.1.1/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.878489 reaxpro-wrappers-1.1.1/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.882489 reaxpro-wrappers-1.1.1/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.886489 reaxpro-wrappers-1.1.1/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77148 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.886489 reaxpro-wrappers-1.1.1/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.886489 reaxpro-wrappers-1.1.1/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.886489 reaxpro-wrappers-1.1.1/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.890489 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 12:29:01.000000 reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-26 12:29:01.890489 reaxpro-wrappers-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:01.890489 reaxpro-wrappers-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-26 12:28:42.000000 reaxpro-wrappers-1.1.1/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.1.0/LICENSE` & `reaxpro-wrappers-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/PKG-INFO` & `reaxpro-wrappers-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.1.0
+Version: 1.1.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.1.0/README.md` & `reaxpro-wrappers-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.1.1/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.1.1/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.1.1/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.1.1/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.1.1/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/models/settings/general.py` & `reaxpro-wrappers-1.1.1/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/models/utils/general.py` & `reaxpro-wrappers-1.1.1/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.1.1/osp/models/zacros/co_pyzacros.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.1.1/osp/tools/graph_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/tools/io_functions.py` & `reaxpro-wrappers-1.1.1/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.1.1/osp/tools/mapping_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1556,21 +1556,22 @@
 
         real_number = te.get(oclass=emmo.Real)
         electronic_energy_values.append(real_number[0].hasNumericalData)
 
     return electronic_energy_values
 
 
-def map_results(engine, root_cuds_object: Cuds):
+def map_results(engine, root_cuds_object: Cuds) -> str:
     """
     Add main results to the Cuds (Wrapper) object.
 
     :engine: main engine object, e.g. Multijob for AMS calculations.
     :param root_cuds_object: CUDS wrapper to add results to.
     :param wrapper_settings: SimamsSettings object.
+    :return str: file system path to tarball-
    """
 
     if isinstance(engine, MultiJob):
 
         # in case of several children, outputs will be added in the order of dependencies.
         search_simulation = \
             search.find_cuds_object(criterion=lambda x: x.is_a(oclass=emmo.Simulation),
@@ -1580,15 +1581,15 @@
         if not len(search_simulation):
 
             # Attach results to Calculation CUDS object using hasOutput rel.
             search_calculation = \
                     search.find_cuds_objects_by_oclass(
                                        emmo.Calculation,
                                        root_cuds_object, rel=cuba.relationship)
-            map_tarball(engine, search_calculation[0])
+            tarball = map_tarball(engine, search_calculation[0])
 
             if map_calculation_type(root_cuds_object) == "WavefunctionOptimization":
                 add_AMSenergy_to_object(engine.children[0], search_calculation[0])
 
             elif map_calculation_type(root_cuds_object) == "GeometryOptimization":
 
                 optimized_geometry = read_molecule(
@@ -1632,16 +1633,14 @@
                 lattice_output = crystallography.UnitCell(iri=iri)
                 search_calculation[0].add(lattice_output, rel=emmo.hasOutput)
 
             elif map_calculation_type(root_cuds_object) == "LandscapeRefinement":
                 add_AMSLandscape_to_object(engine.children[0], search_calculation[0])
 
             # TODO elif map_calculation_type(root_cuds_object) == "XXXX":
-            else:
-                return
 
         else:
             if (map_calculation_type(root_cuds_object) == "WavefunctionOptimization") \
                or (map_calculation_type(root_cuds_object) == "GeometryOptimization"):
 
                 # First
                 first_calculation = search.find_relationships(
@@ -1659,26 +1658,27 @@
                 # Last
                 last_calculation = \
                     search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalLast,
                                               root=search_simulation[0],
                                               consider_rel=emmo.hasTemporalLast)
                 add_AMSenergy_to_object(engine.children[2], last_calculation[0])
 
-            map_tarball(engine, last_calculation[0])
+            tarball = map_tarball(engine, last_calculation[0])
 
     elif isinstance(engine, pz.ZacrosResults):
         search_calculation = search.find_cuds_objects_by_oclass(
                                    emmo.MesoscopicCalculation, root_cuds_object,
                                    rel=cuba.relationship)
-        map_tarball(engine, search_calculation[0])
+        tarball = map_tarball(engine, search_calculation[0])
 
     else:
         raise_error(file=os.path.basename(__file__), function=map_results.__name__,
                     type='NameError',
                     message='Mapping of the results is not implemented for this engine.')
+    return tarball
 
 
 
 def add_AMSenergy_to_object(job: AMSJob, root_cuds_object: Cuds):
     """
     Add Total Energy result to the Cuds (Calculation) object.
 
@@ -1795,27 +1795,30 @@
 
     root_cuds_object.add(semantic_energy_landscape, rel=emmo.hasOutput)
 #    pretty_print(semantic_energy_landscape)
 
     return
 
 
-def map_tarball(engine, root_cuds_object, path=None):
+def map_tarball(engine, root_cuds_object, path=None) -> str:
     """
     Creates and links tarball of the results to root_cuds_object Calculation:
 
     :engine: Job PLAMS /Multijob PLAMS object for AMS calculations, str: for Zacros calculation
 
     :param root_cuds_object: CUDS Calculation to add results to.
+
+    :return str: file system path to tarball
    """
 
     path = "plams_workdir/"
 
     tar = tempfile.NamedTemporaryFile().name
     shutil.make_archive(tar, "tar", path)
     tar_file = f"{tar}.tar"
 
     print(f"Job output dumped to {tar_file}")
 
     iri = arcp_random(tar_file)
     string = emmo.String(iri=iri)
     root_cuds_object.add(string, rel=emmo.hasOutput)
+    return tar_file
```

### Comparing `reaxpro-wrappers-1.1.0/osp/tools/set_functions.py` & `reaxpro-wrappers-1.1.1/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.1.1/osp/wrappers/simams/simams_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         """
         Execute engine session.
 
         :param root_cuds_object: Main Cuds object.
 
         """
         self.engine.run()
-        map_results(self.engine, root_cuds_object)
+        self._tarball = map_results(self.engine, root_cuds_object)
 
     # OVERRIDE   # Map results
     def _load_from_backend(self, uids, expired=None):
         """Load the cuds object from the simulation engine."""
         # TODO load cuds objects from the backend
         for uid in uids:
             if uid in self._registry:
@@ -73,7 +73,11 @@
 
     # OVERRIDE
     def _apply_deleted(self, root_obj, buffer):
         """Deletes the deleted cuds from the engine."""
         # TODO: What should happen in the engine
         # when the user removes a certain cuds?
         # The given buffer contains all the deleted CUDS object in a dictionary
+
+    @property
+    def tarball(cls) -> str:
+        return cls._tarball
```

### Comparing `reaxpro-wrappers-1.1.0/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.1.1/osp/wrappers/simzacros/simzacros_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """
 
         (pz_settings, pz_lattice, pz_mechanism, pz_cluster_expansion) = \
             map_function(self, root_cuds_object, self.engine)
         pz_job = pz.ZacrosJob(settings=pz_settings, lattice=pz_lattice,
                               mechanism=pz_mechanism, cluster_expansion=pz_cluster_expansion)
         results = pz_job.run()
-        map_results(results, root_cuds_object)
+        self._tarball = map_results(results, root_cuds_object)
 
         # Attributes to easily access (syntactic) info from results.
         self.get_reaction_network = results.get_reaction_network()
         self.provided_quantities_names = results.provided_quantities_names()
         self.provided_quantities = results.provided_quantities()
         self.number_of_lattice_sites = results.number_of_lattice_sites()
         self.gas_species_names = results.gas_species_names()
@@ -136,7 +136,11 @@
 
     # OVERRIDE
     def _apply_deleted(self, root_obj, buffer):
         """Deletes the deleted cuds from the engine."""
         # TODO: What should happen in the engine
         # when the user removes a certain cuds?
         # The given buffer contains all the deleted CUDS object in a dictionary
+
+    @property
+    def tarball(cls) -> str:
+        return cls._tarball
```

### Comparing `reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.1.0
+Version: 1.1.1
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.1.0/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.1.1/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/setup.cfg` & `reaxpro-wrappers-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.1.0
+version = v1.1.1
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.1.0/setup.py` & `reaxpro-wrappers-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.1.1/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/tests/test_examples.py` & `reaxpro-wrappers-1.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.1.1/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.0/tests/test_tools.py` & `reaxpro-wrappers-1.1.1/tests/test_tools.py`

 * *Files identical despite different names*

