# Comparing `tmp/hera_sim-4.1.0.tar.gz` & `tmp/hera_sim-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_sim-4.1.0.tar", last modified: Tue Jun 27 19:28:49 2023, max compression
+gzip compressed data, was "hera_sim-4.1.1.tar", last modified: Wed Jul 26 16:53:50 2023, max compression
```

## Comparing `hera_sim-4.1.0.tar` & `hera_sim-4.1.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.612172 hera_sim-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.556171 hera_sim-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 19:28:40.000000 hera_sim-4.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-06-27 19:28:40.000000 hera_sim-4.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-27 19:28:40.000000 hera_sim-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 19:28:40.000000 hera_sim-4.1.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 19:28:40.000000 hera_sim-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-27 19:28:49.612172 hera_sim-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-27 19:28:40.000000 hera_sim-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/config_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 19:28:40.000000 hera_sim-4.1.0/config_examples/simulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-27 19:28:40.000000 hera_sim-4.1.0/config_examples/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/notes_for_developers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.580171 hera_sim-4.1.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/end_to_end_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_defaults.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_tour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_vis_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/mutual_coupling_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/polybeam_simulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/visibility_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.584171 hera_sim-4.1.0/hera_sim/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/__yaml_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    41449 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    48320 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.588172 hera_sim-4.1.0/hera_sim/config/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/H1C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/H2C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.592172 hera_sim-4.1.0/hera_sim/data/
--rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/H37_FR_Filters_small.npz
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_REFLECTIONS.npz
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_BANDPASS.npz
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
--rw-r--r--   0 runner    (1001) docker     (123)    49740 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_REFLECTIONS.npz
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_LAT_LON_ALT.npy
--rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_Tsky_Reformatted.npz
--rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_Tsky_vs_LST.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.560171 hera_sim-4.1.0/hera_sim/data/tutorials_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.596171 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.596171 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/eor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    63166 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.604172 hera_sim-4.1.0/hera_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_eor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    34979 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_sim_red_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_simulate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_vis_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_yaml_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.604172 hera_sim-4.1.0/hera_sim/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/healvis_catalog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2635200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
--rw-r--r--   0 runner    (1001) docker     (123)    59077 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/viscpu.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/visgpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27060 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/hera_sim/visibilities/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/pyuvsim_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/vis_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.584171 hera_sim-4.1.0/hera_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 19:28:40.000000 hera_sim-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-27 19:28:40.000000 hera_sim-4.1.0/scripts/hera-sim-simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-27 19:28:40.000000 hera_sim-4.1.0/scripts/hera-sim-vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-27 19:28:49.612172 hera_sim-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:28:40.000000 hera_sim-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.182934 hera_sim-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.154934 hera_sim-4.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.158934 hera_sim-4.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 16:53:39.000000 hera_sim-4.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 16:53:39.000000 hera_sim-4.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-07-26 16:53:39.000000 hera_sim-4.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-26 16:53:39.000000 hera_sim-4.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 16:53:39.000000 hera_sim-4.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 16:53:39.000000 hera_sim-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-26 16:53:50.182934 hera_sim-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-26 16:53:39.000000 hera_sim-4.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.158934 hera_sim-4.1.1/config_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 16:53:39.000000 hera_sim-4.1.1/config_examples/simulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-26 16:53:39.000000 hera_sim-4.1.1/config_examples/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.158934 hera_sim-4.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.158934 hera_sim-4.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/notes_for_developers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.158934 hera_sim-4.1.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.166934 hera_sim-4.1.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/end_to_end_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/hera_sim_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/hera_sim_defaults.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/hera_sim_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/hera_sim_tour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/hera_sim_vis_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/mutual_coupling_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/polybeam_simulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials/visibility_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-26 16:53:39.000000 hera_sim-4.1.1/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.170934 hera_sim-4.1.1/hera_sim/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/__yaml_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41449 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48320 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.170934 hera_sim-4.1.1/hera_sim/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/config/H1C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/config/H2C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/config/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.174934 hera_sim-4.1.1/hera_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/H37_FR_Filters_small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H1C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H1C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H1C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H2C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H2C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H4C_BANDPASS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    49740 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_H4C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_LAT_LON_ALT.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_Tsky_Reformatted.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/HERA_Tsky_vs_LST.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.154934 hera_sim-4.1.1/hera_sim/data/tutorials_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.174934 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.174934 hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63166 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.178934 hera_sim-4.1.1/hera_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34979 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_sim_red_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_simulate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_vis_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/test_yaml_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.178934 hera_sim-4.1.1/hera_sim/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/healvis_catalog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.178934 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2635200 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    59077 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/viscpu.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/visgpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27060 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.182934 hera_sim-4.1.1/hera_sim/visibilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/visibilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/visibilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/visibilities/pyuvsim_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/visibilities/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-07-26 16:53:39.000000 hera_sim-4.1.1/hera_sim/visibilities/vis_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.170934 hera_sim-4.1.1/hera_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-26 16:53:50.000000 hera_sim-4.1.1/hera_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-26 16:53:50.000000 hera_sim-4.1.1/hera_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:53:50.000000 hera_sim-4.1.1/hera_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:53:49.000000 hera_sim-4.1.1/hera_sim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-26 16:53:50.000000 hera_sim-4.1.1/hera_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 16:53:50.000000 hera_sim-4.1.1/hera_sim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-26 16:53:39.000000 hera_sim-4.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:53:50.182934 hera_sim-4.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-26 16:53:39.000000 hera_sim-4.1.1/scripts/hera-sim-simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 16:53:39.000000 hera_sim-4.1.1/scripts/hera-sim-vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-26 16:53:50.182934 hera_sim-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 16:53:39.000000 hera_sim-4.1.1/setup.py
```

### Comparing `hera_sim-4.1.0/.coveragerc` & `hera_sim-4.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/.flake8` & `hera_sim-4.1.1/.flake8`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/.github/workflows/publish.yaml` & `hera_sim-4.1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/.github/workflows/test_suite.yaml` & `hera_sim-4.1.1/.github/workflows/test_suite.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/.pre-commit-config.yaml` & `hera_sim-4.1.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -29,30 +29,30 @@
           - flake8-rst-docstrings
           - flake8-rst
 #          - flake8-markdown    # not available for flake8>5 (check later...)
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-print
 -   repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
     - id: black
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: rst-backticks
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.7.0
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
     args: [--py39-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v2.3.0
+  rev: v2.4.0
   hooks:
   - id: setup-cfg-fmt
```

### Comparing `hera_sim-4.1.0/CHANGELOG.rst` & `hera_sim-4.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/CONTRIBUTING.rst` & `hera_sim-4.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/LICENSE.rst` & `hera_sim-4.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/PKG-INFO` & `hera_sim-4.1.1/hera_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hera_sim
-Version: 4.1.0
+Name: hera-sim
+Version: 4.1.1
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.1.0/README.rst` & `hera_sim-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/config_examples/template_config.yaml` & `hera_sim-4.1.1/config_examples/template_config.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/Makefile` & `hera_sim-4.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/_templates/class.rst` & `hera_sim-4.1.1/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/_templates/module.rst` & `hera_sim-4.1.1/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/conf.py` & `hera_sim-4.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/reference/index.rst` & `hera_sim-4.1.1/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/end_to_end_example.ipynb` & `hera_sim-4.1.1/docs/tutorials/end_to_end_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/hera_sim_cli.rst` & `hera_sim-4.1.1/docs/tutorials/hera_sim_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/hera_sim_defaults.ipynb` & `hera_sim-4.1.1/docs/tutorials/hera_sim_defaults.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/hera_sim_simulator.ipynb` & `hera_sim-4.1.1/docs/tutorials/hera_sim_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/hera_sim_tour.ipynb` & `hera_sim-4.1.1/docs/tutorials/hera_sim_tour.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/hera_sim_vis_cli.rst` & `hera_sim-4.1.1/docs/tutorials/hera_sim_vis_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/mutual_coupling_example.ipynb` & `hera_sim-4.1.1/docs/tutorials/mutual_coupling_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/polybeam_simulation.ipynb` & `hera_sim-4.1.1/docs/tutorials/polybeam_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials/visibility_simulator.ipynb` & `hera_sim-4.1.1/docs/tutorials/visibility_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/docs/tutorials.rst` & `hera_sim-4.1.1/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/__init__.py` & `hera_sim-4.1.1/hera_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/__yaml_constructors.py` & `hera_sim-4.1.1/hera_sim/__yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/adjustment.py` & `hera_sim-4.1.1/hera_sim/adjustment.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/antpos.py` & `hera_sim-4.1.1/hera_sim/antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/beams.py` & `hera_sim-4.1.1/hera_sim/beams.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/cli_utils.py` & `hera_sim-4.1.1/hera_sim/cli_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/components.py` & `hera_sim-4.1.1/hera_sim/components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/config/H1C.yaml` & `hera_sim-4.1.1/hera_sim/config/H1C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/config/H2C.yaml` & `hera_sim-4.1.1/hera_sim/config/H2C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/config/debug.yaml` & `hera_sim-4.1.1/hera_sim/config/debug.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/H37_FR_Filters_small.npz` & `hera_sim-4.1.1/hera_sim/data/H37_FR_Filters_small.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H1C_REFLECTIONS.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H1C_REFLECTIONS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy` & `hera_sim-4.1.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy` & `hera_sim-4.1.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H4C_BANDPASS.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H4C_BANDPASS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_H4C_REFLECTIONS.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_H4C_REFLECTIONS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_Tsky_Reformatted.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_Tsky_Reformatted.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/HERA_Tsky_vs_LST.npz` & `hera_sim-4.1.1/hera_sim/data/HERA_Tsky_vs_LST.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py` & `hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt` & `hera_sim-4.1.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv` & `hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5` & `hera_sim-4.1.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/defaults.py` & `hera_sim-4.1.1/hera_sim/defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/eor.py` & `hera_sim-4.1.1/hera_sim/eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/foregrounds.py` & `hera_sim-4.1.1/hera_sim/foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/interpolators.py` & `hera_sim-4.1.1/hera_sim/interpolators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/io.py` & `hera_sim-4.1.1/hera_sim/io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/noise.py` & `hera_sim-4.1.1/hera_sim/noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/rfi.py` & `hera_sim-4.1.1/hera_sim/rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/sigchain.py` & `hera_sim-4.1.1/hera_sim/sigchain.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/simulate.py` & `hera_sim-4.1.1/hera_sim/simulate.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/conftest.py` & `hera_sim-4.1.1/hera_sim/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_adjustment.py` & `hera_sim-4.1.1/hera_sim/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_antpos.py` & `hera_sim-4.1.1/hera_sim/tests/test_antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_beams.py` & `hera_sim-4.1.1/hera_sim/tests/test_beams.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_cli_utils.py` & `hera_sim-4.1.1/hera_sim/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_compare_pyuvsim.py` & `hera_sim-4.1.1/hera_sim/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_components.py` & `hera_sim-4.1.1/hera_sim/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_defaults.py` & `hera_sim-4.1.1/hera_sim/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_eor.py` & `hera_sim-4.1.1/hera_sim/tests/test_eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_foregrounds.py` & `hera_sim-4.1.1/hera_sim/tests/test_foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_interpolators.py` & `hera_sim-4.1.1/hera_sim/tests/test_interpolators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_io.py` & `hera_sim-4.1.1/hera_sim/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_noise.py` & `hera_sim-4.1.1/hera_sim/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_rfi.py` & `hera_sim-4.1.1/hera_sim/tests/test_rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_sigchain.py` & `hera_sim-4.1.1/hera_sim/tests/test_sigchain.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_sim_red_data.py` & `hera_sim-4.1.1/hera_sim/tests/test_sim_red_data.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_simulate_cli.py` & `hera_sim-4.1.1/hera_sim/tests/test_simulate_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_simulator.py` & `hera_sim-4.1.1/hera_sim/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_utils.py` & `hera_sim-4.1.1/hera_sim/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_vis.py` & `hera_sim-4.1.1/hera_sim/tests/test_vis.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_vis_cli.py` & `hera_sim-4.1.1/hera_sim/tests/test_vis_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/test_yaml_constructors.py` & `hera_sim-4.1.1/hera_sim/tests/test_yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv` & `hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits` & `hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot` & `hera_sim-4.1.1/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/utils.py` & `hera_sim-4.1.1/hera_sim/utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/vis.py` & `hera_sim-4.1.1/hera_sim/vis.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/visibilities/__init__.py` & `hera_sim-4.1.1/hera_sim/visibilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/visibilities/cli.py` & `hera_sim-4.1.1/hera_sim/visibilities/cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/visibilities/pyuvsim_wrapper.py` & `hera_sim-4.1.1/hera_sim/visibilities/pyuvsim_wrapper.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/visibilities/simulators.py` & `hera_sim-4.1.1/hera_sim/visibilities/simulators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim/visibilities/vis_cpu.py` & `hera_sim-4.1.1/hera_sim/visibilities/vis_cpu.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim.egg-info/PKG-INFO` & `hera_sim-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hera-sim
-Version: 4.1.0
+Name: hera_sim
+Version: 4.1.1
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.1.0/hera_sim.egg-info/SOURCES.txt` & `hera_sim-4.1.1/hera_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/hera_sim.egg-info/requires.txt` & `hera_sim-4.1.1/hera_sim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/scripts/hera-sim-simulate.py` & `hera_sim-4.1.1/scripts/hera-sim-simulate.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.1.0/setup.cfg` & `hera_sim-4.1.1/setup.cfg`

 * *Files identical despite different names*

