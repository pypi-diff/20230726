# Comparing `tmp/aiida_vibroscopy-1.0.1.tar.gz` & `tmp/aiida_vibroscopy-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_vibroscopy-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_vibroscopy-1.0.1a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_vibroscopy-1.0.1.tar` & `aiida_vibroscopy-1.0.1a1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      300 2023-07-26 15:48:15.466434 aiida_vibroscopy-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0     5367 2023-07-26 15:48:15.466434 aiida_vibroscopy-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1354 2023-07-26 15:48:15.466434 aiida_vibroscopy-1.0.1/README.md
--rw-r--r--   0        0        0      391 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/environment.yml
--rw-r--r--   0        0        0     3599 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      691 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/__init__.py
--rw-r--r--   0        0        0     2784 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/create_directional_kpoints.py
--rw-r--r--   0        0        0    21146 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/numerical_derivatives_utils.py
--rw-r--r--   0        0        0     5617 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/phonon_utils.py
--rw-r--r--   0        0        0    26215 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/spectra_utils.py
--rw-r--r--   0        0        0    17747 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/symmetry.py
--rw-r--r--   0        0        0      137 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/common/__init__.py
--rw-r--r--   0        0        0     2632 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/common/constants.py
--rw-r--r--   0        0        0      939 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/common/properties.py
--rw-r--r--   0        0        0      798 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/__init__.py
--rw-r--r--   0        0        0      964 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_fp.py
--rw-r--r--   0        0        0      927 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_lr.py
--rw-r--r--   0        0        0    25777 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_mixin.py
--rw-r--r--   0        0        0        0 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/__init__.py
--rw-r--r--   0        0        0     7704 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/broadenings.py
--rw-r--r--   0        0        0     2661 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/elfield_cards_functions.py
--rw-r--r--   0        0        0      638 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/__init__.py
--rw-r--r--   0        0        0    11887 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/lebedev.py
--rw-r--r--   0        0        0      652 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/__init__.py
--rw-r--r--   0        0        0      144 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_003.json
--rw-r--r--   0        0        0      165 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_005.json
--rw-r--r--   0        0        0      288 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_007.json
--rw-r--r--   0        0        0      301 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_009.json
--rw-r--r--   0        0        0      351 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_011.json
--rw-r--r--   0        0        0      400 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_013.json
--rw-r--r--   0        0        0      423 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_015.json
--rw-r--r--   0        0        0      479 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_017.json
--rw-r--r--   0        0        0      552 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_019.json
--rw-r--r--   0        0        0      623 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_021.json
--rw-r--r--   0        0        0      715 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_023.json
--rw-r--r--   0        0        0      775 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_025.json
--rw-r--r--   0        0        0      829 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_027.json
--rw-r--r--   0        0        0      884 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_029.json
--rw-r--r--   0        0        0      960 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_031.json
--rw-r--r--   0        0        0     1184 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_035.json
--rw-r--r--   0        0        0     1421 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_041.json
--rw-r--r--   0        0        0     1736 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_047.json
--rw-r--r--   0        0        0     1895 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_053.json
--rw-r--r--   0        0        0     2279 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_059.json
--rw-r--r--   0        0        0     2625 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_065.json
--rw-r--r--   0        0        0     3063 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_071.json
--rw-r--r--   0        0        0     3469 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_077.json
--rw-r--r--   0        0        0     3974 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_083.json
--rw-r--r--   0        0        0     4493 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_089.json
--rw-r--r--   0        0        0     5069 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_095.json
--rw-r--r--   0        0        0     5640 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_101.json
--rw-r--r--   0        0        0     6285 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_107.json
--rw-r--r--   0        0        0     6900 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_113.json
--rw-r--r--   0        0        0     7588 2023-07-26 15:48:15.626434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_119.json
--rw-r--r--   0        0        0     8330 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_125.json
--rw-r--r--   0        0        0     9072 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_131.json
--rw-r--r--   0        0        0     2818 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/plotting.py
--rw-r--r--   0        0        0     2029 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/spectra.py
--rw-r--r--   0        0        0     2567 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/validation.py
--rw-r--r--   0        0        0      598 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/__init__.py
--rw-r--r--   0        0        0      598 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/__init__.py
--rw-r--r--   0        0        0    36809 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/base.py
--rw-r--r--   0        0        0     9379 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/numerical_derivatives.py
--rw-r--r--   0        0        0      598 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/__init__.py
--rw-r--r--   0        0        0    22323 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/base.py
--rw-r--r--   0        0        0    17290 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/harmonic.py
--rw-r--r--   0        0        0      584 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/base.yaml
--rw-r--r--   0        0        0     1130 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/dielectric/base.yaml
--rw-r--r--   0        0        0     1341 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/phonons/harmonic.yaml
--rw-r--r--   0        0        0     1177 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/phonons/phonon.yaml
--rw-r--r--   0        0        0     1364 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/spectra/iraman.yaml
--rw-r--r--   0        0        0      598 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/__init__.py
--rw-r--r--   0        0        0     5478 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/intensities_average.py
--rw-r--r--   0        0        0     9069 2023-07-26 15:48:15.630434 aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/iraman.py
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 aiida_vibroscopy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      300 2023-07-26 15:24:14.274910 aiida_vibroscopy-1.0.1a1/.readthedocs.yml
+-rw-r--r--   0        0        0     5367 2023-07-26 15:24:14.274910 aiida_vibroscopy-1.0.1a1/LICENSE.txt
+-rw-r--r--   0        0        0     1354 2023-07-26 15:24:14.274910 aiida_vibroscopy-1.0.1a1/README.md
+-rw-r--r--   0        0        0      391 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/environment.yml
+-rw-r--r--   0        0        0     3599 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0      693 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/__init__.py
+-rw-r--r--   0        0        0     2784 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/create_directional_kpoints.py
+-rw-r--r--   0        0        0    21146 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/numerical_derivatives_utils.py
+-rw-r--r--   0        0        0     5617 2023-07-26 15:24:14.450913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/phonon_utils.py
+-rw-r--r--   0        0        0    26215 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/spectra_utils.py
+-rw-r--r--   0        0        0    17747 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/symmetry.py
+-rw-r--r--   0        0        0      137 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/common/__init__.py
+-rw-r--r--   0        0        0     2632 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/common/constants.py
+-rw-r--r--   0        0        0      939 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/common/properties.py
+-rw-r--r--   0        0        0      798 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/__init__.py
+-rw-r--r--   0        0        0      964 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_fp.py
+-rw-r--r--   0        0        0      927 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_lr.py
+-rw-r--r--   0        0        0    25777 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_mixin.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/__init__.py
+-rw-r--r--   0        0        0     7704 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/broadenings.py
+-rw-r--r--   0        0        0     2661 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/elfield_cards_functions.py
+-rw-r--r--   0        0        0      638 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/__init__.py
+-rw-r--r--   0        0        0    11887 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/lebedev.py
+-rw-r--r--   0        0        0      652 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_003.json
+-rw-r--r--   0        0        0      165 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_005.json
+-rw-r--r--   0        0        0      288 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_007.json
+-rw-r--r--   0        0        0      301 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_009.json
+-rw-r--r--   0        0        0      351 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_011.json
+-rw-r--r--   0        0        0      400 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_013.json
+-rw-r--r--   0        0        0      423 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_015.json
+-rw-r--r--   0        0        0      479 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_017.json
+-rw-r--r--   0        0        0      552 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_019.json
+-rw-r--r--   0        0        0      623 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_021.json
+-rw-r--r--   0        0        0      715 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_023.json
+-rw-r--r--   0        0        0      775 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_025.json
+-rw-r--r--   0        0        0      829 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_027.json
+-rw-r--r--   0        0        0      884 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_029.json
+-rw-r--r--   0        0        0      960 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_031.json
+-rw-r--r--   0        0        0     1184 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_035.json
+-rw-r--r--   0        0        0     1421 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_041.json
+-rw-r--r--   0        0        0     1736 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_047.json
+-rw-r--r--   0        0        0     1895 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_053.json
+-rw-r--r--   0        0        0     2279 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_059.json
+-rw-r--r--   0        0        0     2625 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_065.json
+-rw-r--r--   0        0        0     3063 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_071.json
+-rw-r--r--   0        0        0     3469 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_077.json
+-rw-r--r--   0        0        0     3974 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_083.json
+-rw-r--r--   0        0        0     4493 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_089.json
+-rw-r--r--   0        0        0     5069 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_095.json
+-rw-r--r--   0        0        0     5640 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_101.json
+-rw-r--r--   0        0        0     6285 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_107.json
+-rw-r--r--   0        0        0     6900 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_113.json
+-rw-r--r--   0        0        0     7588 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_119.json
+-rw-r--r--   0        0        0     8330 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_125.json
+-rw-r--r--   0        0        0     9072 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_131.json
+-rw-r--r--   0        0        0     2818 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/plotting.py
+-rw-r--r--   0        0        0     2029 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/spectra.py
+-rw-r--r--   0        0        0     2567 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/validation.py
+-rw-r--r--   0        0        0      598 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/__init__.py
+-rw-r--r--   0        0        0      598 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/__init__.py
+-rw-r--r--   0        0        0    36809 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/base.py
+-rw-r--r--   0        0        0     9379 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/numerical_derivatives.py
+-rw-r--r--   0        0        0      598 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/__init__.py
+-rw-r--r--   0        0        0    22323 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/base.py
+-rw-r--r--   0        0        0    17290 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/harmonic.py
+-rw-r--r--   0        0        0      584 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/base.yaml
+-rw-r--r--   0        0        0     1130 2023-07-26 15:24:14.454913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/dielectric/base.yaml
+-rw-r--r--   0        0        0     1341 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/phonons/harmonic.yaml
+-rw-r--r--   0        0        0     1177 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/phonons/phonon.yaml
+-rw-r--r--   0        0        0     1364 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/spectra/iraman.yaml
+-rw-r--r--   0        0        0      598 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/__init__.py
+-rw-r--r--   0        0        0     5478 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/intensities_average.py
+-rw-r--r--   0        0        0     9069 2023-07-26 15:24:14.458913 aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/iraman.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 aiida_vibroscopy-1.0.1a1/PKG-INFO
```

### Comparing `aiida_vibroscopy-1.0.1/LICENSE.txt` & `aiida_vibroscopy-1.0.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/README.md` & `aiida_vibroscopy-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/pyproject.toml` & `aiida_vibroscopy-1.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 # Copyright (c), All rights reserved.                                           #
 # This file is part of the AiiDA-Vibroscopy code.                               #
 #                                                                               #
 # The code is hosted on GitHub at https://github.com/bastonero/aiida-vibroscopy #
 # For further information on the license, see the LICENSE.txt file              #
 #################################################################################
 """AiiDA plugin for vibrational spectoscopy using Quantum ESPRESSO."""
-__version__ = '1.0.1'
+__version__ = '1.0.1a1'
```

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/create_directional_kpoints.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/create_directional_kpoints.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/numerical_derivatives_utils.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/numerical_derivatives_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/phonon_utils.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/phonon_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/spectra_utils.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/spectra_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/calculations/symmetry.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/calculations/symmetry.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/common/constants.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/common/constants.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/common/properties.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/common/properties.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_fp.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_fp.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_lr.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_lr.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/data/vibro_mixin.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/data/vibro_mixin.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/broadenings.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/broadenings.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/elfield_cards_functions.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/elfield_cards_functions.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/lebedev.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/lebedev.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_019.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_019.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_021.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_021.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_023.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_023.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_025.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_025.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_027.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_027.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_029.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_029.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_031.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_031.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_035.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_035.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_041.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_041.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_047.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_047.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_053.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_053.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_059.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_059.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_065.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_065.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_071.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_071.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_077.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_077.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_083.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_083.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_089.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_089.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_095.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_095.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_101.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_101.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_107.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_107.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_113.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_113.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_119.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_119.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_125.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_125.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_131.json` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/integration/schemas/lebedev_131.json`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/plotting.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/spectra.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/spectra.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/utils/validation.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/utils/validation.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/base.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/base.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/dielectric/numerical_derivatives.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/dielectric/numerical_derivatives.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/base.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/base.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/phonons/harmonic.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/phonons/harmonic.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/base.yaml` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/dielectric/base.yaml` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/dielectric/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/phonons/harmonic.yaml` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/phonons/harmonic.yaml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/phonons/phonon.yaml` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/phonons/phonon.yaml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/protocols/spectra/iraman.yaml` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/protocols/spectra/iraman.yaml`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/__init__.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/intensities_average.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/intensities_average.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/src/aiida_vibroscopy/workflows/spectra/iraman.py` & `aiida_vibroscopy-1.0.1a1/src/aiida_vibroscopy/workflows/spectra/iraman.py`

 * *Files identical despite different names*

### Comparing `aiida_vibroscopy-1.0.1/PKG-INFO` & `aiida_vibroscopy-1.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-vibroscopy
-Version: 1.0.1
+Version: 1.0.1a1
 Summary: AiiDA plugin for vibrational spectoscopy using Quantum ESPRESSO.
 Keywords: aiida,workflows
 Author-email: Lorenzo Bastonero <bastonero.lorenzo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AiiDA
```

