# Comparing `tmp/mopac_step-2023.7.24.tar.gz` & `tmp/mopac_step-2023.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopac_step-2023.7.24.tar", last modified: Tue Jul 25 20:14:13 2023, max compression
+gzip compressed data, was "mopac_step-2023.7.26.tar", last modified: Wed Jul 26 20:42:00 2023, max compression
```

## Comparing `mopac_step-2023.7.24.tar` & `mopac_step-2023.7.26.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/seamm-mopac.yml
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.565137 mopac_step-2023.7.24/mopac_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:13:57.000000 mopac_step-2023.7.24/mopac_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/tests/test_mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.717808 mopac_step-2023.7.26/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.721808 mopac_step-2023.7.26/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.729808 mopac_step-2023.7.26/mopac_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 20:42:00.729808 mopac_step-2023.7.26/mopac_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/mopac_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/data/seamm-mopac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41932 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/forceconstants_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/ir_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/lewis_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/thermodynamics_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/mopac_step/tk_thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/mopac_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 20:42:00.000000 mopac_step-2023.7.26/mopac_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:41:40.000000 mopac_step-2023.7.26/mopac_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:42:00.725808 mopac_step-2023.7.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/tests/test_mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-26 20:41:36.000000 mopac_step-2023.7.26/versioneer.py
```

### Comparing `mopac_step-2023.7.24/CONTRIBUTING.rst` & `mopac_step-2023.7.26/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/HISTORY.rst` & `mopac_step-2023.7.26/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2023.7.26 -- Added output of bond orders
+  * Also added capability to use the bond orders to put bond multiplicities on the
+    structure.
+    
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
     
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
```

### Comparing `mopac_step-2023.7.24/LICENSE` & `mopac_step-2023.7.26/LICENSE`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/PKG-INFO` & `mopac_step-2023.7.26/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac_step
-Version: 2023.7.24
+Version: 2023.7.26
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.26 -- Added output of bond orders
+  * Also added capability to use the bond orders to put bond multiplicities on the
+    structure.
+    
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
     
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
```

### Comparing `mopac_step-2023.7.24/README.rst` & `mopac_step-2023.7.26/README.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/Makefile` & `mopac_step-2023.7.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/SEAMM inverted.png` & `mopac_step-2023.7.26/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/SEAMM logo.png` & `mopac_step-2023.7.26/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/molssi_main_logo.png` & `mopac_step-2023.7.26/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/molssi_main_logo_inverted_white.png` & `mopac_step-2023.7.26/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/molssi_square.png` & `mopac_step-2023.7.26/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/_static/nsf.png` & `mopac_step-2023.7.26/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/conf.py` & `mopac_step-2023.7.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/developer_guide/installation.rst` & `mopac_step-2023.7.26/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/getting_started/index.rst` & `mopac_step-2023.7.26/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/index.rst` & `mopac_step-2023.7.26/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/docs/make.bat` & `mopac_step-2023.7.26/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/__init__.py` & `mopac_step-2023.7.26/mopac_step/__init__.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/data/configuration.txt` & `mopac_step-2023.7.26/mopac_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/data/properties.csv` & `mopac_step-2023.7.26/mopac_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/data/references.bib` & `mopac_step-2023.7.26/mopac_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/energy.py` & `mopac_step-2023.7.26/mopac_step/energy.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,23 @@
 
         if self.parameters["COSMO"].is_expr or self.parameters["COSMO"].get():
             text += (
                 "dielectric constant = {eps}, solvent radius = {rsolve}, "
                 "{nspa} grid points per atom, and a cutoff of {disex}."
             )
 
+        # And bond orders
+        if P["bond orders"] == "yes":
+            text += "\n\nThe bond orders will be calculated."
+        elif P["bond orders"] == "yes, and apply to structure":
+            text += (
+                "\n\nThe bond orders will be calculated and used to set the bonding "
+                "for the structure."
+            )
+
         return self.header + "\n" + __(text, **P, indent=4 * " ").__str__()
 
     def get_input(self):
         """Get the input for an energy calculation for MOPAC"""
         system, configuration = self.get_system_configuration(None)
         references = self.parent.references
 
@@ -649,14 +658,17 @@
             keywords.append(f"RSOLVE={rsolve}")
             keywords.append(f"NSPA={P['nspa']}")
             keywords.append(f"DISEX={P['disex']}")
 
         if P["calculate gradients"]:
             keywords.append("GRADIENTS")
 
+        if "yes" in P["bond orders"]:
+            keywords.append("BONDS")
+
         # Add any extra keywords so that they appear at the end
         metadata = self.metadata["keywords"]
         for keyword in P["extra keywords"]:
             if "=" in keyword:
                 keyword, value = keyword.split("=")
                 if keyword not in metadata or "format" not in metadata[keyword]:
                     keywords.append(keyword + "=" + value)
@@ -961,14 +973,19 @@
                     )
                 )
 
         text = str(__(text, **data, indent=self.indent + 4 * " "))
         text += "\n\n"
         text += textwrap.indent("\n".join(text_lines), self.indent + 7 * " ")
 
+        if "BOND_ORDERS" in data:
+            text += self._bond_orders(
+                P["bond orders"], data["BOND_ORDERS"], starting_configuration
+            )
+
         printer.normal(text)
 
         if used_mozyme and "CPU_TIME" in data_sections[0]:
             t0 = data_sections[0]["CPU_TIME"]
             if "CPU_TIME" in data:
                 t1 = data["CPU_TIME"]
                 text = (
@@ -984,7 +1001,101 @@
 
         # Put any requested results into variables or tables
         self.store_results(
             configuration=configuration,
             data=data,
             create_tables=self.parameters["create tables"].get(),
         )
+
+    def _bond_orders(self, control, bond_order_matrix, configuration):
+        """Analyze and print the bond orders, and optionally use for the bonding
+        in the structure.
+
+        Parameters
+        ----------
+        control : str
+            The control option for the bond order analysis
+        bond_order_matrix : [float]
+            Lower triangular part of the bond order matrix.
+        configuration : molsystem.Configuration
+            The configuration to put the bonds on, if requested.
+        """
+        text = ""
+        n_atoms = configuration.n_atoms
+        bond_i = []
+        bond_j = []
+        bond_order = []
+        bond_order_str = []
+        orders = []
+        ij = 0
+        for j in range(n_atoms):
+            for i in range(j + 1):
+                if i != j:
+                    order = bond_order_matrix[ij]
+                    if order > 0.5:
+                        bond_i.append(i)
+                        bond_j.append(j)
+                        if order > 1.3 and order < 1.7:
+                            bond_order.append(5)
+                            bond_order_str.append("aromatic")
+                        else:
+                            bond_order.append(round(order))
+                            bond_order_str.append(str(round(order)))
+                        orders.append(order)
+                ij += 1
+
+        symbols = configuration.atoms.symbols
+        options = self.parent.options
+        text_lines = []
+        if len(symbols) <= int(options["max_atoms_to_print"]):
+            if "name" in configuration.atoms:
+                name = configuration.atoms.get_column_data("name")
+            else:
+                name = []
+                count = {}
+                for symbol in symbols:
+                    if symbol not in count:
+                        count[symbol] = 1
+                    else:
+                        count[symbol] += 1
+                    name.append(f"{symbol}{count[symbol]}")
+            table = {
+                "i": [name[i] for i in bond_i],
+                "j": [name[j] for j in bond_j],
+                "bond order": orders,
+                "bond multiplicity": bond_order_str,
+            }
+            tmp = tabulate(
+                table,
+                headers="keys",
+                tablefmt="pretty",
+                disable_numparse=True,
+                colalign=("center", "center", "right", "center"),
+            )
+            length = len(tmp.splitlines()[0])
+            text_lines.append("\n")
+            text_lines.append("Bond Orders".center(length))
+            text_lines.append(
+                tabulate(
+                    table,
+                    headers="keys",
+                    tablefmt="psql",
+                    colalign=("center", "center", "decimal", "center"),
+                )
+            )
+            text += "\n\n"
+            text += textwrap.indent("\n".join(text_lines), self.indent + 7 * " ")
+
+        if control == "yes, and apply to structure":
+            ids = configuration.atoms.ids
+            iatoms = [ids[i] for i in bond_i]
+            jatoms = [ids[j] for j in bond_j]
+            configuration.bonds.delete()
+            configuration.bonds.append(i=iatoms, j=jatoms, bondorder=bond_order)
+            text2 = (
+                "\nReplaced the bonds in the configuration with those from the "
+                "calculated bond orders.\n"
+            )
+
+        text += str(__(text2, indent=self.indent + 4 * " "))
+
+        return text
```

### Comparing `mopac_step-2023.7.24/mopac_step/energy_parameters.py` & `mopac_step-2023.7.26/mopac_step/energy_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,23 @@
             "format_string": "",
             "description": "criterion",
             "help_text": (
                 "The SCF convergence criterion, based on the "
                 "change in energy between iterations."
             ),
         },
+        "bond orders": {
+            "default": "yes",
+            "kind": "enum",
+            "default_units": "",
+            "enumeration": ("yes", "yes, and apply to structure", "no"),
+            "format_string": "",
+            "description": "Calculate bond orders:",
+            "help_text": "Whether to calculate bond orders and also apply to structure",
+        },
         "extra keywords": {
             "default": [],
             "kind": "list",
             "default_units": "",
             "enumeration": tuple(),
             "format_string": "",
             "description": "Extra keywords",
```

### Comparing `mopac_step-2023.7.24/mopac_step/energy_step.py` & `mopac_step-2023.7.26/mopac_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/forceconstants.py` & `mopac_step-2023.7.26/mopac_step/forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/forceconstants_parameters.py` & `mopac_step-2023.7.26/mopac_step/forceconstants_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/forceconstants_step.py` & `mopac_step-2023.7.26/mopac_step/forceconstants_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/installer.py` & `mopac_step-2023.7.26/mopac_step/installer.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/ir.py` & `mopac_step-2023.7.26/mopac_step/ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/ir_parameters.py` & `mopac_step-2023.7.26/mopac_step/ir_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/ir_step.py` & `mopac_step-2023.7.26/mopac_step/ir_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/lewis_structure.py` & `mopac_step-2023.7.26/mopac_step/lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/lewis_structure_parameters.py` & `mopac_step-2023.7.26/mopac_step/lewis_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/lewis_structure_step.py` & `mopac_step-2023.7.26/mopac_step/lewis_structure_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/metadata.py` & `mopac_step-2023.7.26/mopac_step/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1329,14 +1329,20 @@
     "ATOM_X_UPDATED": {
         "calculation": ["optimization"],
         "description": "trajectory coordinates",
         "dimensionality": ["nsteps", [3, "n_atoms"]],
         "type": "float",
         "units": "Å",
     },
+    "BOND_ORDERS": {
+        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "description": "bond order matrix",
+        "dimensionality": ["triangular", "n_atoms", "n_atoms"],
+        "type": "float",
+    },
     "COMMENTS": {
         "calculation": [],
         "description": "User comment line",
         "dimensionality": "scalar",
         "type": "string",
     },
     "CPU_TIME": {
```

### Comparing `mopac_step-2023.7.24/mopac_step/mopac.py` & `mopac_step-2023.7.26/mopac_step/mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/mopac_base.py` & `mopac_step-2023.7.26/mopac_step/mopac_base.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/mopac_step.py` & `mopac_step-2023.7.26/mopac_step/mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/optimization.py` & `mopac_step-2023.7.26/mopac_step/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,20 +390,27 @@
         # Update the structure
         if "ATOM_X_OPT" in data or "ATOM_X_UPDATED" in data:
             periodicity = starting_configuration.periodicity
             if (
                 "structure handling" in P
                 and P["structure handling"] == "be put in a new configuration"
             ):
-                configuration = system.create_configuration(
-                    periodicity=periodicity,
-                    atomset=starting_configuration.atomset,
-                    bondset=starting_configuration.bondset,
-                    cell_id=starting_configuration.cell_id,
-                )
+                if P["bond orders"] == "yes, and apply to structure":
+                    configuration = system.create_configuration(
+                        periodicity=periodicity,
+                        atomset=starting_configuration.atomset,
+                        cell_id=starting_configuration.cell_id,
+                    )
+                else:
+                    configuration = system.create_configuration(
+                        periodicity=periodicity,
+                        atomset=starting_configuration.atomset,
+                        bondset=starting_configuration.bondset,
+                        cell_id=starting_configuration.cell_id,
+                    )
                 configuration.charge = starting_configuration.charge
                 configuration.spin_multiplicity = (
                     starting_configuration.spin_multiplicity
                 )
             else:
                 configuration = starting_configuration
```

### Comparing `mopac_step-2023.7.24/mopac_step/optimization_parameters.py` & `mopac_step-2023.7.26/mopac_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/optimization_step.py` & `mopac_step-2023.7.26/mopac_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/thermodynamics.py` & `mopac_step-2023.7.26/mopac_step/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/thermodynamics_parameters.py` & `mopac_step-2023.7.26/mopac_step/thermodynamics_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/thermodynamics_step.py` & `mopac_step-2023.7.26/mopac_step/thermodynamics_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_energy.py` & `mopac_step-2023.7.26/mopac_step/tk_energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,11 +151,16 @@
 
             for key in ("eps", "rsolve", "nspa", "disex"):
                 self[key].grid(row=row, column=1, sticky=tk.W)
                 widgets1.append(self[key])
                 row += 1
             sw.align_labels(widgets1, sticky=tk.E)
 
+        for key in ("bond orders",):
+            self[key].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+            widgets.append(self[key])
+            row += 1
+
         sw.align_labels(widgets, sticky=tk.E)
         frame.columnconfigure(0, minsize=100)
 
         return row
```

### Comparing `mopac_step-2023.7.24/mopac_step/tk_forceconstants.py` & `mopac_step-2023.7.26/mopac_step/tk_forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_ir.py` & `mopac_step-2023.7.26/mopac_step/tk_ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_lewis_structure.py` & `mopac_step-2023.7.26/mopac_step/tk_lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_mopac.py` & `mopac_step-2023.7.26/mopac_step/tk_mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_optimization.py` & `mopac_step-2023.7.26/mopac_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step/tk_thermodynamics.py` & `mopac_step-2023.7.26/mopac_step/tk_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step.egg-info/PKG-INFO` & `mopac_step-2023.7.26/mopac_step.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac-step
-Version: 2023.7.24
+Version: 2023.7.26
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.26 -- Added output of bond orders
+  * Also added capability to use the bond orders to put bond multiplicities on the
+    structure.
+    
 2023.7.24 -- Bugfix in Lewis structure with bond orders
   * Major issue in getting the bonds from the Lewis structure where the atoms and bond
     orders were mixed up.
     
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
```

### Comparing `mopac_step-2023.7.24/mopac_step.egg-info/SOURCES.txt` & `mopac_step-2023.7.26/mopac_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/mopac_step.egg-info/entry_points.txt` & `mopac_step-2023.7.26/mopac_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/setup.py` & `mopac_step-2023.7.26/setup.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/tests/test_mopac_step.py` & `mopac_step-2023.7.26/tests/test_mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.7.24/versioneer.py` & `mopac_step-2023.7.26/versioneer.py`

 * *Files identical despite different names*

