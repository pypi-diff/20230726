# Comparing `tmp/hxrsnd-0.3.0.tar.gz` & `tmp/hxrsnd-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hxrsnd-0.3.0.tar", last modified: Tue Jul 25 21:09:45 2023, max compression
+gzip compressed data, was "hxrsnd-0.3.1.tar", last modified: Wed Jul 26 21:25:37 2023, max compression
```

## Comparing `hxrsnd-0.3.0.tar` & `hxrsnd-0.3.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.918804 hxrsnd-0.3.0/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      132 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.coveragerc
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      974 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.flake8
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      125 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.git_archival.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       32 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.gitattributes
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.792904 hxrsnd-0.3.0/.github/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1068 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      751 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.794434 hxrsnd-0.3.0/.github/workflows/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      750 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.github/workflows/standard.yml
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1193 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.gitignore
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      317 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.landscape.yml
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      785 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      174 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/AUTHORS.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2987 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2468 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/LICENSE.md
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       93 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5012 2023-07-25 21:09:45.917712 hxrsnd-0.3.0/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1796 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/README.rst
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.795405 hxrsnd-0.3.0/conda-recipe/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      875 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/conda-recipe/meta.yaml
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       33 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/dev-requirements.txt
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.796360 hxrsnd-0.3.0/docs/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      611 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/Makefile
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.833592 hxrsnd-0.3.0/docs/source/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      453 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/aerotech.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1608 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/alignment.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      343 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/attocube.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5821 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/basic_usage.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      789 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/bragg.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     7025 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/calibrating_delay_scans.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      376 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/calibration.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2941 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/docs/source/conf.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       42 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/diode.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      268 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/exceptions.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1286 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/index.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1172 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/installation.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1368 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/macromotor.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      104 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/misc_plans.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       84 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/pneumatic.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       60 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/rtd.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2001 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/running_daq_scans.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1195 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/running_scans.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      144 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/scans.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      460 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/screens.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      911 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/scripting.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      207 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/sndsystem.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      413 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/tower.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      274 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/utils.rst
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       67 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/docs-requirements.txt
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.858818 hxrsnd-0.3.0/hxrsnd/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      157 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/__init__.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      160 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd/_version.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    25036 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/aerotech.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    17755 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/attocube.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     9792 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/bragg.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8060 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/diode.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1224 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/exceptions.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    49469 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/macromotor.py
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.875357 hxrsnd-0.3.0/hxrsnd/plans/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/__init__.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8872 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/alignment.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    17557 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/calibration.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2064 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/plan_stubs.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1148 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/preprocessors.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     6284 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/scans.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8223 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/pneumatic.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      262 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/rtd.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2392 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/run_snd.py
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.878952 hxrsnd-0.3.0/hxrsnd/screens/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    34405 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/diode.ui
--rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1349 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/motor_expert_screens.sh
--rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1368 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/snd_main
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      719 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/sequencer.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2478 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/snddevice.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    15921 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/sndmotor.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     6401 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/sndsystem.py
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.911610 hxrsnd-0.3.0/hxrsnd/tests/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       69 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8309 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/conftest.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1654 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_aerotech.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1546 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_attocube.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1637 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_alignment.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     9467 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_calibration.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      750 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_plan_stubs.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1232 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_preprocessors.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     3835 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_scans.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1674 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_pneumatic.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      517 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_rtd.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      473 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_scripts.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      535 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sequencer.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      587 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_snd_devices.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      534 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_snddevice.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     7291 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sndmotor.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      397 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sndsystem.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1793 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_tower.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2196 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_utils.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    16093 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tower.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     4860 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/utils.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1898 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/version.py
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.867239 hxrsnd-0.3.0/hxrsnd.egg-info/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5012 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2406 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        1 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       48 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      211 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        7 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/top_level.txt
-drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.913635 hxrsnd-0.3.0/notebooks/
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    76846 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/notebooks/maximize_diode.ipynb
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1156 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/pyproject.toml
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       96 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/requirements.txt
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5548 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/scripts.py
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       38 2023-07-25 21:09:45.919238 hxrsnd-0.3.0/setup.cfg
--rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      570 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/snd_devices.py
--rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1663 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/snd_env.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.447042 hxrsnd-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.415041 hxrsnd-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.415041 hxrsnd-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.landscape.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2987 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-26 21:25:37.447042 hxrsnd-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.415041 hxrsnd-0.3.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.415041 hxrsnd-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.427041 hxrsnd-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/aerotech.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/attocube.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/bragg.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/calibrating_delay_scans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/calibration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/diode.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/macromotor.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/misc_plans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/pneumatic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/rtd.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/running_daq_scans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/running_scans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/scans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/screens.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/scripting.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/sndsystem.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/tower.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.435042 hxrsnd-0.3.1/hxrsnd/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25036 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/aerotech.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17755 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/attocube.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9792 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/bragg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8060 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/diode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49469 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/macromotor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.439041 hxrsnd-0.3.1/hxrsnd/plans/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8872 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17557 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/plans/scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/run_snd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.443042 hxrsnd-0.3.1/hxrsnd/screens/
+-rw-r--r--   0 runner    (1001) docker     (122)    34405 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/screens/diode.ui
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1349 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/screens/motor_expert_screens.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1368 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/screens/snd_main
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/snddevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15921 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/sndmotor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6401 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/sndsystem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.447042 hxrsnd-0.3.1/hxrsnd/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8309 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_aerotech.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_attocube.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_plans_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9467 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_plans_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_plans_plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_plans_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_plans_scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_rtd.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_snd_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_snddevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_sndmotor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_sndsystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_tower.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16093 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/tower.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/hxrsnd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.439041 hxrsnd-0.3.1/hxrsnd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-26 21:25:37.000000 hxrsnd-0.3.1/hxrsnd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:25:37.447042 hxrsnd-0.3.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (122)    76846 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/notebooks/maximize_diode.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5548 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 21:25:37.447042 hxrsnd-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/snd_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1663 2023-07-26 21:25:20.000000 hxrsnd-0.3.1/snd_env.sh
```

### Comparing `hxrsnd-0.3.0/.flake8` & `hxrsnd-0.3.1/.flake8`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/.github/ISSUE_TEMPLATE.md` & `hxrsnd-0.3.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `hxrsnd-0.3.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/.github/workflows/standard.yml` & `hxrsnd-0.3.1/.github/workflows/standard.yml`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   release:
     types:
       - published
 
 jobs:
   standard:
     uses: pcdshub/pcds-ci-helpers/.github/workflows/python-standard.yml@master
+    secrets: inherit
     with:
       # The workflow needs to know the package name.  This can be determined
       # automatically if the repository name is the same as the import name.
       package-name: "hxrsnd"
       # Extras that will be installed for both conda/pip:
       testing-extras: ""
       # Extras to be installed only for conda-based testing:
```

### Comparing `hxrsnd-0.3.0/.gitignore` & `hxrsnd-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/.pre-commit-config.yaml` & `hxrsnd-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/CONTRIBUTING.rst` & `hxrsnd-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/LICENSE.md` & `hxrsnd-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/PKG-INFO` & `hxrsnd-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hxrsnd
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python controls suite for HXRSnD
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hxrsnd-0.3.0/README.rst` & `hxrsnd-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/conda-recipe/meta.yaml` & `hxrsnd-0.3.1/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/Makefile` & `hxrsnd-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/alignment.rst` & `hxrsnd-0.3.1/docs/source/alignment.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/basic_usage.rst` & `hxrsnd-0.3.1/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/bragg.rst` & `hxrsnd-0.3.1/docs/source/bragg.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/calibrating_delay_scans.rst` & `hxrsnd-0.3.1/docs/source/calibrating_delay_scans.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/conf.py` & `hxrsnd-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/index.rst` & `hxrsnd-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/installation.rst` & `hxrsnd-0.3.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/macromotor.rst` & `hxrsnd-0.3.1/docs/source/macromotor.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/running_daq_scans.rst` & `hxrsnd-0.3.1/docs/source/running_daq_scans.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/running_scans.rst` & `hxrsnd-0.3.1/docs/source/running_scans.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/docs/source/scripting.rst` & `hxrsnd-0.3.1/docs/source/scripting.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/aerotech.py` & `hxrsnd-0.3.1/hxrsnd/aerotech.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/attocube.py` & `hxrsnd-0.3.1/hxrsnd/attocube.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/bragg.py` & `hxrsnd-0.3.1/hxrsnd/bragg.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/diode.py` & `hxrsnd-0.3.1/hxrsnd/diode.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/exceptions.py` & `hxrsnd-0.3.1/hxrsnd/exceptions.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/macromotor.py` & `hxrsnd-0.3.1/hxrsnd/macromotor.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/plans/alignment.py` & `hxrsnd-0.3.1/hxrsnd/plans/alignment.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/plans/calibration.py` & `hxrsnd-0.3.1/hxrsnd/plans/calibration.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/plans/plan_stubs.py` & `hxrsnd-0.3.1/hxrsnd/plans/plan_stubs.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/plans/preprocessors.py` & `hxrsnd-0.3.1/hxrsnd/plans/preprocessors.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/plans/scans.py` & `hxrsnd-0.3.1/hxrsnd/plans/scans.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/pneumatic.py` & `hxrsnd-0.3.1/hxrsnd/pneumatic.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/run_snd.py` & `hxrsnd-0.3.1/hxrsnd/run_snd.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/screens/diode.ui` & `hxrsnd-0.3.1/hxrsnd/screens/diode.ui`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/screens/motor_expert_screens.sh` & `hxrsnd-0.3.1/hxrsnd/screens/motor_expert_screens.sh`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/screens/snd_main` & `hxrsnd-0.3.1/hxrsnd/screens/snd_main`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/sequencer.py` & `hxrsnd-0.3.1/hxrsnd/sequencer.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/snddevice.py` & `hxrsnd-0.3.1/hxrsnd/snddevice.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/sndmotor.py` & `hxrsnd-0.3.1/hxrsnd/sndmotor.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/sndsystem.py` & `hxrsnd-0.3.1/hxrsnd/sndsystem.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/conftest.py` & `hxrsnd-0.3.1/hxrsnd/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_aerotech.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_aerotech.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_attocube.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_attocube.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_plans_alignment.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_plans_alignment.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_plans_calibration.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_plans_calibration.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_plans_plan_stubs.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_plans_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_plans_preprocessors.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_plans_preprocessors.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_plans_scans.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_plans_scans.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_pneumatic.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_rtd.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_rtd.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_sequencer.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_sequencer.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_snd_devices.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_snd_devices.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_snddevice.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_snddevice.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_sndmotor.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_sndmotor.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_tower.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_tower.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tests/test_utils.py` & `hxrsnd-0.3.1/hxrsnd/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/tower.py` & `hxrsnd-0.3.1/hxrsnd/tower.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/utils.py` & `hxrsnd-0.3.1/hxrsnd/utils.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd/version.py` & `hxrsnd-0.3.1/hxrsnd/version.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/hxrsnd.egg-info/PKG-INFO` & `hxrsnd-0.3.1/hxrsnd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hxrsnd
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python controls suite for HXRSnD
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hxrsnd-0.3.0/hxrsnd.egg-info/SOURCES.txt` & `hxrsnd-0.3.1/hxrsnd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/notebooks/maximize_diode.ipynb` & `hxrsnd-0.3.1/notebooks/maximize_diode.ipynb`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/pyproject.toml` & `hxrsnd-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/scripts.py` & `hxrsnd-0.3.1/scripts.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/snd_devices.py` & `hxrsnd-0.3.1/snd_devices.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.3.0/snd_env.sh` & `hxrsnd-0.3.1/snd_env.sh`

 * *Files identical despite different names*

