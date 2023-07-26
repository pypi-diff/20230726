# Comparing `tmp/scikit-beam-0.0.8.post0.tar.gz` & `tmp/scikit-beam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-beam-0.0.8.post0.tar", last modified: Fri Mar  4 10:59:19 2016, max compression
+gzip compressed data, was "dist/scikit-beam-0.0.9.tar", last modified: Fri Aug 23 17:21:24 2019, max compression
```

## Comparing `scikit-beam-0.0.8.post0.tar` & `scikit-beam-0.0.9.tar`

### file list

```diff
@@ -1,111 +1,115 @@
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/
--rw-rw-r--   0 edill     (1000) edill     (1000)      416 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/setup.cfg
--rw-rw-r--   0 edill     (1000) edill     (1000)    62474 2016-01-04 18:36:54.000000 scikit-beam-0.0.8.post0/versioneer.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     1790 2016-03-04 10:49:30.000000 scikit-beam-0.0.8.post0/setup.py
--rw-rw-r--   0 edill     (1000) edill     (1000)      747 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/PKG-INFO
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/src/
--rw-rw-r--   0 edill     (1000) edill     (1000)    22362 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/src/ctrans.c
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/
--rw-rw-r--   0 edill     (1000) edill     (1000)       10 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/requires.txt
--rw-rw-r--   0 edill     (1000) edill     (1000)      747 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/PKG-INFO
--rw-rw-r--   0 edill     (1000) edill     (1000)        1 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/dependency_links.txt
--rw-rw-r--   0 edill     (1000) edill     (1000)     2715 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/SOURCES.txt
--rw-rw-r--   0 edill     (1000) edill     (1000)       46 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/pbr.json
--rw-rw-r--   0 edill     (1000) edill     (1000)        7 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/scikit_beam.egg-info/top_level.txt
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/
--rw-rw-r--   0 edill     (1000) edill     (1000)      471 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/_version.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/
--rw-rw-r--   0 edill     (1000) edill     (1000)    39336 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/utils.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     9619 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/feature.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3985 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/stats.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     9030 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/calibration.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    12322 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/speckle.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/
--rw-rw-r--   0 edill     (1000) edill     (1000)      792 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/timings.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)     3204 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/tests/test_histogram.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)  1569065 2016-03-04 10:54:02.000000 scikit-beam-0.0.8.post0/skbeam/core/accumulators/histogram.c
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)     5901 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_spectroscopy.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    15338 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_roi.py
--rw-rw-r--   0 edill     (1000) edill     (1000)      269 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/utils.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5090 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_cdi.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    20970 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_utils.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     8704 2016-03-04 10:52:07.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_dpc.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5413 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_feature.py
--rw-rw-r--   0 edill     (1000) edill     (1000)      547 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_stats.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3959 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_arithmetic.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     1049 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_image.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3572 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_mask.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     7027 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_recip.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     9085 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_correlation.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4424 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_calibration.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5228 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/tests/test_speckle.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    18003 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/dpc.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    30506 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/correlation.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    12846 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/recip.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    13042 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/spectroscopy.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4623 2016-03-04 10:52:07.000000 scikit-beam-0.0.8.post0/skbeam/core/mask.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/
--rw-rw-r--   0 edill     (1000) edill     (1000)    54228 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/xrf_model.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/base/
--rw-rw-r--   0 edill     (1000) edill     (1000)    13963 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/base/parameter_data.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     2829 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/base/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     1084 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/funcs.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)     3816 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_background.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     8846 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_xrf_fit.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    13271 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_lineshapes.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3590 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5983 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/models.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    15123 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/lineshapes.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     8569 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/fitting/background.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    22524 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/roi.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     7053 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/arithmetic.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/data/
--rw-rw-r--   0 edill     (1000) edill     (1000)    45203 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/data/AtomicConstants.dat
--rw-rw-r--   0 edill     (1000) edill     (1000)     7128 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/basic.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    10541 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/xrs.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    17882 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/xrf.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)     7066 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_xrf.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5111 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_basic.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3697 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_xrs.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3050 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_api.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     2898 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/constants/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4561 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/image.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    13036 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/core/cdi.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/io/
--rw-rw-r--   0 edill     (1000) edill     (1000)    10661 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/save_powder_output.py
--rw-rw-r--   0 edill     (1000) edill     (1000)    10337 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/avizo_io.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3187 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/net_cdf_io.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/io/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)       21 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/io/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     5386 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/tests/test_powder_output.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3160 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/io/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     8616 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/gsas_file_reader.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4212 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/io/binary.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4307 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/diffraction.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/tests/
--rw-rw-r--   0 edill     (1000) edill     (1000)     4309 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/tests/test_openness.py
--rw-rw-r--   0 edill     (1000) edill     (1000)       71 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/tests/test_diffraction.py
--rw-rw-r--   0 edill     (1000) edill     (1000)       73 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/tests/test_fluorescence.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     2778 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/tests/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     3130 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/fluorescence.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     2758 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/__init__.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/testing/
--rw-rw-r--   0 edill     (1000) edill     (1000)     4462 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/testing/decorators.py
--rw-rw-r--   0 edill     (1000) edill     (1000)     4580 2016-03-04 10:53:46.000000 scikit-beam-0.0.8.post0/skbeam/testing/noseclasses.py
--rw-rw-r--   0 edill     (1000) edill     (1000)        1 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/testing/__init__.py
-drwxrwxr-x   0 edill     (1000) edill     (1000)        0 2016-03-04 10:59:19.000000 scikit-beam-0.0.8.post0/skbeam/ext/
--rw-rw-r--   0 edill     (1000) edill     (1000)        0 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/skbeam/ext/__init__.py
--rw-rw-r--   0 edill     (1000) edill     (1000)       48 2016-01-04 18:36:54.000000 scikit-beam-0.0.8.post0/optional-requirements.txt
--rw-rw-r--   0 edill     (1000) edill     (1000)       21 2016-01-04 18:36:54.000000 scikit-beam-0.0.8.post0/requirements.txt
--rw-rw-r--   0 edill     (1000) edill     (1000)      108 2016-03-04 10:39:19.000000 scikit-beam-0.0.8.post0/MANIFEST.in
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1584 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/LICENSE
+-rw-r--r--   0 mrakitin   (501) staff       (20)      108 2019-08-23 17:20:43.000000 scikit-beam-0.0.9/MANIFEST.in
+-rw-r--r--   0 mrakitin   (501) staff       (20)      741 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2484 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/README.md
+-rw-r--r--   0 mrakitin   (501) staff       (20)       48 2019-08-23 17:20:43.000000 scikit-beam-0.0.9/optional-requirements.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)       21 2019-08-23 17:20:43.000000 scikit-beam-0.0.9/requirements.txt
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      741 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2827 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)        1 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)       10 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/requires.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)        7 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/scikit_beam.egg-info/top_level.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)      418 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/setup.cfg
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2254 2019-08-23 17:21:00.000000 scikit-beam-0.0.9/setup.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2758 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)      471 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/_version.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/__init__.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/accumulators/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/accumulators/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    25108 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/core/accumulators/binned_statistic.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)  6265227 2019-08-23 17:15:49.000000 scikit-beam-0.0.9/skbeam/core/accumulators/histogram.c
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/accumulators/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/accumulators/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     6360 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/core/accumulators/tests/test_binned_statistic.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4902 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/accumulators/tests/test_histogram.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     7053 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/core/arithmetic.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     9233 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/calibration.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    13311 2019-08-23 17:21:00.000000 scikit-beam-0.0.9/skbeam/core/cdi.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/constants/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2916 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     7129 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/basic.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/constants/data/
+-rw-r--r--   0 mrakitin   (501) staff       (20)    45203 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/data/AtomicConstants.dat
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3050 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/test_api.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5111 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/test_basic.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     7573 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/test_xrf.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3697 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/tests/test_xrs.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    18664 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/constants/xrf.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    10498 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/constants/xrs.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    30277 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/correlation.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    18036 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/dpc.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     9619 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/feature.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/fitting/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3590 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8569 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/background.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/fitting/base/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2829 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/base/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    13963 2019-08-23 17:20:43.000000 scikit-beam-0.0.9/skbeam/core/fitting/base/parameter_data.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1084 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/funcs.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    15123 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/lineshapes.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5991 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/models.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/fitting/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3816 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/tests/test_background.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    13271 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/fitting/tests/test_lineshapes.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8846 2019-08-23 17:21:00.000000 scikit-beam-0.0.9/skbeam/core/fitting/tests/test_xrf_fit.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    54231 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/fitting/xrf_model.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     7503 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/core/image.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     6729 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/core/mask.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    12753 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/recip.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    24207 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/roi.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    12322 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/speckle.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    13050 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/spectroscopy.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3985 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/stats.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/core/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3959 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_arithmetic.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4424 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_calibration.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5090 2019-08-23 17:21:00.000000 scikit-beam-0.0.9/skbeam/core/tests/test_cdi.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     9085 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/tests/test_correlation.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8704 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_dpc.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5413 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_feature.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3231 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/tests/test_image.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5314 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_mask.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     7027 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_recip.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    16377 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/tests/test_roi.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5228 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_speckle.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5901 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_spectroscopy.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)      547 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_stats.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    21436 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/test_utils.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)      269 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/core/tests/utils.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    40349 2019-08-23 17:21:10.000000 scikit-beam-0.0.9/skbeam/core/utils.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4307 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/diffraction.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/ext/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/ext/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3130 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/fluorescence.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/io/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3150 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    10337 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/avizo_io.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4212 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/binary.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     6793 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/io/fit2d_save.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8616 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/gsas_file_reader.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3191 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/io/net_cdf_io.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    10665 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/save_powder_output.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/io/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)       21 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3069 2019-08-23 17:21:21.000000 scikit-beam-0.0.9/skbeam/io/tests/test_fit2d_save.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5386 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/io/tests/test_powder_output.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/testing/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        1 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/testing/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4462 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/testing/decorators.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4580 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/testing/noseclasses.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/skbeam/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2778 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)       71 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/tests/test_diffraction.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)       73 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/tests/test_fluorescence.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4309 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/skbeam/tests/test_openness.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2019-08-23 17:21:24.000000 scikit-beam-0.0.9/src/
+-rw-r--r--   0 mrakitin   (501) staff       (20)    15628 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/src/ctrans.c
+-rw-r--r--   0 mrakitin   (501) staff       (20)    62474 2019-08-15 21:51:41.000000 scikit-beam-0.0.9/versioneer.py
```

### Comparing `scikit-beam-0.0.8.post0/versioneer.py` & `scikit-beam-0.0.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/setup.py` & `scikit-beam-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 #!/usr/bin/env python
 
 import setuptools
 from distutils.core import setup, Extension
 import versioneer
 import numpy as np
 import os
+import sys
 from Cython.Build import cythonize
 
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 def c_ext():
+    if os.name == 'nt':
+        # we are on windows. Do not compile the extension. Tons of errors are
+        # spit out when we compile on AppVeyor.
+        # https://gist.github.com/ericdill/bdc86eb81e338ca4624b
+        return []
+
+    # compile for MacOS without openmp
+    if sys.platform == 'darwin':
+        return [Extension('skbeam.ext.ctrans', ['src/ctrans.c'])]
+    # compile the extension on Linux.
     return [Extension('skbeam.ext.ctrans', ['src/ctrans.c'],
-                      define_macros=[('USE_THREADS', None)])]
+                      extra_compile_args=['-fopenmp'],
+                      extra_link_args=['-lgomp'])]
 
 
 def cython_ext():
     return cythonize("**/*.pyx")
 
 
 setup(
```

### Comparing `scikit-beam-0.0.8.post0/PKG-INFO` & `scikit-beam-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-beam
-Version: 0.0.8.post0
+Version: 0.0.9
 Summary: Data analysis tools for X-ray science
 Home-page: http://github.com/scikit-beam/scikit-beam
 Author: Brookhaven National Lab
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Keywords: Xray Analysis
```

### Comparing `scikit-beam-0.0.8.post0/scikit_beam.egg-info/PKG-INFO` & `scikit-beam-0.0.9/scikit_beam.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-beam
-Version: 0.0.8.post0
+Version: 0.0.9
 Summary: Data analysis tools for X-ray science
 Home-page: http://github.com/scikit-beam/scikit-beam
 Author: Brookhaven National Lab
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Keywords: Xray Analysis
```

### Comparing `scikit-beam-0.0.8.post0/scikit_beam.egg-info/SOURCES.txt` & `scikit-beam-0.0.9/scikit_beam.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+LICENSE
 MANIFEST.in
+README.md
 optional-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 scikit_beam.egg-info/PKG-INFO
 scikit_beam.egg-info/SOURCES.txt
 scikit_beam.egg-info/dependency_links.txt
-scikit_beam.egg-info/pbr.json
 scikit_beam.egg-info/requires.txt
 scikit_beam.egg-info/top_level.txt
 skbeam/__init__.py
 skbeam/_version.py
 skbeam/diffraction.py
 skbeam/fluorescence.py
 skbeam/core/__init__.py
@@ -26,17 +27,18 @@
 skbeam/core/recip.py
 skbeam/core/roi.py
 skbeam/core/speckle.py
 skbeam/core/spectroscopy.py
 skbeam/core/stats.py
 skbeam/core/utils.py
 skbeam/core/accumulators/__init__.py
+skbeam/core/accumulators/binned_statistic.py
 skbeam/core/accumulators/histogram.c
-skbeam/core/accumulators/timings.py
 skbeam/core/accumulators/tests/__init__.py
+skbeam/core/accumulators/tests/test_binned_statistic.py
 skbeam/core/accumulators/tests/test_histogram.py
 skbeam/core/constants/__init__.py
 skbeam/core/constants/basic.py
 skbeam/core/constants/xrf.py
 skbeam/core/constants/xrs.py
 skbeam/core/constants/data/AtomicConstants.dat
 skbeam/core/constants/tests/__init__.py
@@ -72,18 +74,20 @@
 skbeam/core/tests/test_stats.py
 skbeam/core/tests/test_utils.py
 skbeam/core/tests/utils.py
 skbeam/ext/__init__.py
 skbeam/io/__init__.py
 skbeam/io/avizo_io.py
 skbeam/io/binary.py
+skbeam/io/fit2d_save.py
 skbeam/io/gsas_file_reader.py
 skbeam/io/net_cdf_io.py
 skbeam/io/save_powder_output.py
 skbeam/io/tests/__init__.py
+skbeam/io/tests/test_fit2d_save.py
 skbeam/io/tests/test_powder_output.py
 skbeam/testing/__init__.py
 skbeam/testing/decorators.py
 skbeam/testing/noseclasses.py
 skbeam/tests/__init__.py
 skbeam/tests/test_diffraction.py
 skbeam/tests/test_fluorescence.py
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/utils.py` & `scikit-beam-0.0.9/skbeam/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,21 @@
 import time
 import sys
 
 from collections import namedtuple, MutableMapping, defaultdict, deque
 import numpy as np
 from itertools import tee
 
-from ..ext import ctrans
-
 import logging
-logger = logging.getLogger(__name__)
+import scipy.stats as sts
 
+logger = logging.getLogger(__name__)
 
 md_value = namedtuple("md_value", ['value', 'units'])
 
-
 _defaults = {
     "bins": 100,
     'nx': 100,
     'ny': 100,
     'nz': 100
 }
 
@@ -92,14 +90,15 @@
     >>> tt['nested.a'].units is None
     True
     >>> tt['name'].value
     'test'
     >>> tt['nested.b'].units
     'm'
     """
+
     def __init__(self, md_dict=None):
         # TODO properly walk the input on upgrade dicts -> MD_dict
         if md_dict is None:
             md_dict = dict()
 
         self._dict = md_dict
         self._split = '.'
@@ -192,29 +191,30 @@
 
 
 class verbosedict(dict):
     """
     A sub-class of dict which raises more verbose errors if
     a key is not found.
     """
+
     def __getitem__(self, key):
         try:
             v = dict.__getitem__(self, key)
         except KeyError:
             if len(self) < 25:
                 new_msg = ("You tried to access the key '{key}' "
                            "which does not exist.  The "
                            "extant keys are: {valid_keys}").format(
-                               key=key, valid_keys=list(self))
+                    key=key, valid_keys=list(self))
             else:
                 new_msg = ("You tried to access the key '{key}' "
                            "which does not exist.  There "
                            "are {num} extant keys, which is too many to "
                            "show you").format(
-                               key=key, num=len(self))
+                    key=key, num=len(self))
             six.reraise(KeyError, KeyError(new_msg), sys.exc_info()[2])
         return v
 
 
 class RCParamDict(MutableMapping):
     """A class to make dealing with storing default values easier.
 
@@ -581,15 +581,15 @@
         min_x = np.min(x)
     if max_x is None:
         max_x = np.max(x)
     if nx is None:
         nx = int(max_x - min_x)
 
     # use a weighted histogram to get the bin sum
-    bins = np.linspace(start=min_x, stop=max_x, num=nx+1, endpoint=True)
+    bins = np.linspace(start=min_x, stop=max_x, num=nx + 1, endpoint=True)
     val, _ = np.histogram(a=x, bins=bins, weights=y)
     # use an un-weighted histogram to get the counts
     count, _ = np.histogram(a=x, bins=bins)
     # return the three arrays
     return bins, val, count
 
 
@@ -618,15 +618,15 @@
     """
 
     if pixel_size is None:
         pixel_size = (1, 1)
 
     X, Y = np.meshgrid(pixel_size[1] * (np.arange(shape[1]) - center[1]),
                        pixel_size[0] * (np.arange(shape[0]) - center[0]))
-    return np.sqrt(X*X + Y*Y)
+    return np.sqrt(X * X + Y * Y)
 
 
 def angle_grid(center, shape, pixel_size=None):
     """
     Make a grid of angular positions.
 
     Read note for our conventions here -- there be dragons!
@@ -793,15 +793,15 @@
         return np.linspace(range_min, range_max, nbins + 1, endpoint=True)
 
     # in this case, the user gave use min, max, and step
     if nbins is None:
         if step > (range_max - range_min):
             raise ValueError("The step can not be greater than the difference "
                              "between min and max")
-        nbins = int((range_max - range_min)//step)
+        nbins = int((range_max - range_min) // step)
         ret = range_min + np.arange(nbins + 1) * step
         # if the last value is greater than the max (should never happen)
         if ret[-1] > range_max:
             return ret[:-1]
         if range_max - ret[-1] > 1e-10 * step:
             logger.debug("Inconsistent "
                          "(range_min, range_max, step) "
@@ -822,15 +822,15 @@
         return range_max - np.arange(nbins + 1)[::-1] * step
 
 
 def grid3d(q, img_stack,
            nx=None, ny=None, nz=None,
            xmin=None, xmax=None, ymin=None,
            ymax=None, zmin=None, zmax=None,
-           binary_mask=None, n_threads=None):
+           binary_mask=None):
     """Grid irregularly spaced data points onto a regular grid via histogramming
 
     This function will process the set of reciprocal space values (q), the
     image stack (img_stack) and grid the image data based on the bounds
     provided, using defaults if none are provided.
 
     Parameters
@@ -860,48 +860,37 @@
         Maximum value along z. Defaults to largest z value in q
     binary_mask : ndarray, optional
         The binary mask provides a mechanism to remove unwanted pixels
         from the images.
         Binary mask can be two different shapes.
         - 1: 2-D with binary_mask.shape == np.asarray(img_stack[0]).shape
         - 2: 3-D with binary_mask.shape == np.asarray(img_stack).shape
-    n_threads : int, optional
-        Specify the number of threads for the c-module to use in its
-        calculations. A value of None indicates to use the number of
-        configured cores on the system.
 
     Returns
     -------
     mean : ndarray
         intensity grid.  The values in this grid are the
         mean of the values that fill with in the grid.
     occupancy : ndarray
         The number of data points that fell in the grid.
     std_err : ndarray
         This is the standard error of the value in the
         grid box.
-    oob : int
-        Out Of Bounds. Number of data points that are outside of
-        the gridded region.
     bounds : list
         tuple of (min, max, step) for x, y, z in order: [x_bounds,
         y_bounds, z_bounds]
 
-    Notes
-    -----
-    The standard error is calculated "on the fly" on a per thread basis.
-    Therefore, the standard error is not correctly calculated if there is only
-    one value per voxel per thread. The standard error calculation is
-    therefore only valid when the number of values per voxel per thread is
-    greater than one. The n_threads can be used to set the number of cores used
-    to correct this if the standard error is needed to be accurate.
     """
-
-    if n_threads is None:
-        n_threads = 0
+    try:
+        from ..ext import ctrans
+    except ImportError:
+        raise NotImplementedError(
+            "ctrans is not available on your platform. See "
+            "https://github.com/scikit-beam/scikit-beam/issues/418 "
+            "to follow updates to this problem.")
 
     # validate input
     img_stack = np.asarray(img_stack)
     # todo determine if we're going to support masked arrays
     # todo masked arrays seemed to have been punted to `process_to_q`
 
     # check to see if the binary mask and the image stack are identical shapes
@@ -953,37 +942,36 @@
 
     # creating (Qx, Qy, Qz, I) Nx4 array - HKL values and Intensity
     # getting the intensity value for each pixel
     q = np.insert(q, 3, np.ravel(img_stack), axis=1)
     if binary_mask is not None:
         q = q[np.ravel(binary_mask)]
 
-    #            3D grid of the data set
+    # 3D grid of the data set
     # starting time for gridding
     t1 = time.time()
 
     # call the c library
 
-    total, mean, occupancy, std_err, oob = ctrans.grid3d(q, qmin, qmax, dqn,
-                                                         n_threads)
+    total, total2, occupancy, std_err = ctrans.grid3d(q, qmin, qmax, dqn)
+    mean = total / occupancy
+
     # ending time for the gridding
     t2 = time.time()
-    logger.info("Done processed in {0} seconds".format(t2-t1))
+    logger.info("Done processed in {0} seconds".format(t2 - t1))
 
     # No. of values zero in the grid
     empt_nb = (occupancy == 0).sum()
 
     # log some information about the grid at the debug level
-    if oob:
-        logger.debug("There are %.2e points outside the grid", oob)
     logger.debug("There are %2e bins in the grid", mean.size)
     if empt_nb:
         logger.debug("There are %.2e values zero in the grid", empt_nb)
 
-    return mean, occupancy, std_err, oob, bounds
+    return mean, occupancy, std_err, bounds
 
 
 def bin_edges_to_centers(input_edges):
     """
     Helper function for turning a array of bin edges into
     an array of bin centers
 
@@ -1059,70 +1047,70 @@
 
 
     """
     return (2 * np.pi) / np.asarray(d)
 
 
 def q_to_twotheta(q, wavelength):
-    """
+    r"""
     Helper function to convert q to two-theta.
 
     By definition the relationship is:
 
     ..math ::
 
-        \\sin\\left(\\frac{2\\theta}{2}\right) = \\frac{\\lambda q}{4 \\pi}
+        \sin\left(\frac{2\theta}{2}\right) = \frac{\lambda q}{4 \pi}
 
     thus
 
     ..math ::
 
-        2\\theta_n = 2 \\arcsin\\left(\\frac{\\lambda q}{4 \\pi}\\right
+        2\theta_n = 2 \arcsin\left(\frac{\lambda q}{4 \pi}\right
 
     Parameters
     ----------
     q : array
         An array of :math:`q` values
 
     wavelength : float
         Wavelength of the incoming x-rays
 
     Returns
     -------
     two_theta : array
-        An array of :math:`2\\theta` values
-
-
+        An array of :math:`2\theta` values
     """
     q = np.asarray(q)
     wavelength = float(wavelength)
     pre_factor = wavelength / (4 * np.pi)
     return 2 * np.arcsin(q * pre_factor)
 
 
 def twotheta_to_q(two_theta, wavelength):
-    """
+    r"""
     Helper function to convert two-theta to q
 
-    By definition the relationship is:
+    By definition the relationship is
 
     ..math ::
 
-        \\sin\\left(\\frac{2\\theta}{2}\right) = \\frac{\\lambda q}{4 \\pi}
+        \sin\left(\frac{2\theta}{2}\right) = \frac{\lambda q}{4 \pi}
 
     thus
 
     ..math ::
 
-        q = \\frac{4 \\pi \\sin\\left(\\frac{2\\theta}{2}\right)}{\\lambda}
+        q = \frac{4 \pi \sin\left(\frac{2\theta}{2}\right)}{\lambda}
+
+
 
     Parameters
     ----------
     two_theta : array
-        An array of :math:`2\\theta` values
+        An array of :math:`2\theta` values
 
     wavelength : float
         Wavelength of the incoming x-rays
 
     Returns
     -------
     q : array
@@ -1170,24 +1158,24 @@
 
     if (multitau_channels % 2 != 0):
         raise ValueError("Number of  multiple tau channels(buffers)"
                          " must be even. You provided {0} "
                          .format(multitau_channels))
 
     # total number of channels ( or total number of delay times)
-    tot_channels = (multitau_levels + 1)*multitau_channels//2
+    tot_channels = (multitau_levels + 1) * multitau_channels // 2
 
     lag = []
     dict_lags = {}
     lag_steps = np.arange(0, multitau_channels)
     dict_lags[1] = lag_steps
     for i in range(2, multitau_levels + 1):
         y = []
-        for j in range(0, multitau_channels//2):
-            value = (multitau_channels//2 + j)*(2**(i - 1))
+        for j in range(0, multitau_channels // 2):
+            value = (multitau_channels // 2 + j) * (2 ** (i - 1))
             lag.append(value)
             y.append(value)
         dict_lags[i] = y
 
     lag_steps = np.append(lag_steps, np.array(lag))
     return tot_channels, lag_steps, dict_lags
 
@@ -1225,10 +1213,61 @@
     a - first term in the series
 
     r - is the common ratio
     """
 
     geometric_series = [first_term]
 
-    while geometric_series[-1]*common_ratio < number_of_images:
-        geometric_series.append(geometric_series[-1]*common_ratio)
+    while geometric_series[-1] * common_ratio < number_of_images:
+        geometric_series.append(geometric_series[-1] * common_ratio)
     return geometric_series
+
+
+def bin_grid(image, r_array, pixel_sizes, statistic='mean', mask=None,
+             bins=None):
+    """
+    Bin and integrate an image, given the radial array of pixels
+
+    Parameters
+    ----------
+    image: np.array
+        The image in quesion
+    r_array: np.array
+        The array which maps pixel positions to tilt/rotation corrected radii
+    pixel_sizes: tuple
+        The size of the pixels in the same units as the r_array
+    statistic: str or func, optional
+        The statistic to compute over the integration, defaults to mean
+    mask: bool array, optional
+        The array of pixels to be removed from the image before integration
+    bins: array, optional
+        The bins to use in the integration, if none given the function will
+        give its best assessment based on the pixel_size and r_array
+
+    Returns
+    -------
+    bin_centers : array
+        The center of each bin in R
+    int_stat : array
+        Radial integrated statistic of the image.
+
+    See Also
+    --------
+    circular_average : circularly average an image, assuming linear radial
+        spacing (less general)
+
+    """
+    if mask is None:
+        mask = np.ones(image.shape, dtype=int).astype(bool)
+    if bins is None:
+        res = np.hypot(*pixel_sizes)
+        bins = np.arange(np.min(r_array) - res * .5,
+                         np.max(r_array) + res * .5, res)
+
+    int_stat, bin_edge, bin_num = sts.binned_statistic(r_array[mask],
+                                                       image[mask],
+                                                       statistic=statistic,
+                                                       bins=bins)
+
+    bin_centers = bin_edges_to_centers(bin_edge)
+
+    return bin_centers, int_stat
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/feature.py` & `scikit-beam-0.0.9/skbeam/core/feature.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/stats.py` & `scikit-beam-0.0.9/skbeam/core/stats.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/calibration.py` & `scikit-beam-0.0.9/skbeam/core/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR   #
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
-"""
-This is the module for calibration functions and data
+"""Automatically calibrate a diffraction beam line given a powder sample of a
+known sample.
 """
 
 from __future__ import absolute_import, division, print_function
 
 from collections import deque
+from string import Template
 
 import numpy as np
 import scipy.signal
 
 from .constants import calibration_standards
 from .feature import (filter_peak_height, peak_refinement,
                       refine_log_quadratic)
@@ -56,28 +57,30 @@
     Estimate the sample-detector distance
 
     Given a radially integrated calibration image return an estimate for
     the sample-detector distance.  This function does not require a
     rough estimate of what d should be.
 
     For the peaks found the detector-sample distance is estimated via
+
     .. math ::
 
         D = \\frac{r}{\\tan 2\\theta}
 
     where :math:`r` is the distance in mm from the calibrated center
     to the ring on the detector and :math:`D` is the distance from
     the sample to the detector.
 
     Parameters
     ----------
     name : str
         The name of the calibration standard.  Used to look up the
         expected peak location
-        For valid options, see the name attribute on this function
+
+        Valid options: $name_ops
 
     wavelength : float
         The wavelength of scattered x-ray in nm
 
     bin_centers : array
         The distance from the calibrated center to the center of
         the ring's annulus in mm
@@ -127,14 +130,17 @@
     # estimate the sample-detector distance for each of the peaks
     d_array = (peaks_x[slc] / tan2theta[slc])
     return np.mean(d_array), np.std(d_array)
 
 # Set an attribute for the calibration names that are valid options.  This
 # attribute also aids in autowrapping into VisTrails
 estimate_d_blind.name = list(calibration_standards)
+if estimate_d_blind.__doc__ is not None:
+    estimate_d_blind.__doc__ = Template(estimate_d_blind.__doc__).substitute(
+        name_ops=repr(sorted(estimate_d_blind.name)))
 
 
 def refine_center(image, calibrated_center, pixel_size, phi_steps, max_peaks,
                   thresh, window_size,
                   nx=None, min_x=None, max_x=None):
     """
     Refines the location of the center of the beam.
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/speckle.py` & `scikit-beam-0.0.9/skbeam/core/speckle.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_spectroscopy.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_roi.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_roi.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,29 @@
     assert_array_almost_equal(ring_avg, [8., 2.5, 5.55555556, 0.,
                                          0., 0.], decimal=6)
 
     bin_cen1, ring_avg1 = roi.circular_average(image, calib_center, min_x=0,
                                                max_x=10, nx=None)
     assert_array_almost_equal(bin_cen1, [0.5, 1.5, 2.5, 3.5, 4.5, 5.5, 6.5,
                                          7.5, 8.5])
+    mask = np.ones_like(image)
+    mask[4:6, 2:3] = 0
+
+    bin_cen_masked, ring_avg_masked = roi.circular_average(image,
+                                                           calib_center,
+                                                           min_x=0,
+                                                           max_x=10,
+                                                           nx=6,
+                                                           mask=mask)
+
+    assert_array_almost_equal(bin_cen_masked, [0.83333333,  2.5, 4.16666667,
+                              5.83333333,  7.5, 9.16666667])
+
+    assert_array_almost_equal(ring_avg_masked, [8.88888889,  3.84615385,  2.5,
+                              0.,  0.,  0.])
 
 
 def test_kymograph():
     calib_center = (25, 25)
     inner_radius = 5
 
     edges = roi.ring_edges(inner_radius, width=2, num_rings=1)
@@ -368,7 +383,17 @@
     n_edges = edges = [[3, 4], [5, 7], [8]]
     h_values, v_values = np.mgrid[0:10, 0:10]
     h_val, v_val = np.mgrid[0:20, 0:20]
 
     assert_raises(ValueError, roi.box, shape, n_edges)
     assert_raises(ValueError, roi.box, shape, edges, h_values=h_val,
                   v_values=v_values)
+
+
+def test_lines():
+    points = ([30, 45, 50, 256], [56, 60, 80, 150])
+    shape = (256, 150)
+    label_array = roi.lines(points, shape)
+    assert_array_equal(np.array([1, 2]), np.unique(label_array)[1:])
+
+    assert_raises(ValueError, roi.lines,
+                  ([10, 12, 30], [30, 45, 50, 256]), shape)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_cdi.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_cdi.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_utils.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,26 @@
 import sys
 
 import numpy.testing as npt
 from numpy.testing import (assert_array_equal, assert_array_almost_equal,
                            assert_almost_equal)
 from nose.tools import assert_equal, assert_true, raises
 
+from skbeam.testing.decorators import known_fail_if
+
 import skbeam.core.utils as core
 
 import logging
+
+try:
+    from pyFAI.geometry import Geometry
+    pf = True
+except ImportError:
+    pf = False
+    pass
 logger = logging.getLogger(__name__)
 
 
 def test_bin_1D():
     # set up simple data
     x = np.linspace(0, 1, 100)
     y = np.arange(100)
@@ -174,16 +183,16 @@
                   'zmin': q_min[2],
                   'xmax': q_max[0],
                   'ymax': q_max[1],
                   'zmax': q_max[2]}
     # slice tricks
     # this make a list of slices, the imaginary value in the
     # step is interpreted as meaning 'this many values'
-    slc = [slice(_min + (_max - _min)/(s * 2),
-                 _max - (_max - _min)/(s * 2),
+    slc = [slice(_min + (_max - _min) / (s * 2),
+                 _max - (_max - _min) / (s * 2),
                  1j * s)
            for _min, _max, s in zip(q_min, q_max, dqn)]
     # use the numpy slice magic to make X, Y, Z these are dense meshes with
     # points in the center of each bin
     X, Y, Z = np.mgrid[slc]
 
     # make and ravel the image data (which is all ones)
@@ -191,19 +200,18 @@
 
     # make input data (Nx3
     data = np.array([np.ravel(X),
                      np.ravel(Y),
                      np.ravel(Z)]).T
 
     (mean, occupancy,
-     std_err, oob, bounds) = core.grid3d(data, I, **param_dict)
+     std_err, bounds) = core.grid3d(data, I, **param_dict)
 
     # check the values are as expected
     npt.assert_array_equal(mean.ravel(), I)
-    npt.assert_equal(oob, 0)
     npt.assert_array_equal(occupancy, np.ones_like(occupancy))
     npt.assert_array_equal(std_err, 0)
 
 
 def test_process_grid_std_err():
     size = 10
     q_max = np.array([1.0, 1.0, 1.0])
@@ -213,47 +221,44 @@
                   'ny': dqn[1],
                   'nz': dqn[2],
                   'xmin': q_min[0],
                   'ymin': q_min[1],
                   'zmin': q_min[2],
                   'xmax': q_max[0],
                   'ymax': q_max[1],
-                  'zmax': q_max[2],
-                  'n_threads': 1}
+                  'zmax': q_max[2]}
     # slice tricks
     # this make a list of slices, the imaginary value in the
     # step is interpreted as meaning 'this many values'
-    slc = [slice(_min + (_max - _min)/(s * 2),
-                 _max - (_max - _min)/(s * 2),
+    slc = [slice(_min + (_max - _min) / (s * 2),
+                 _max - (_max - _min) / (s * 2),
                  1j * s)
            for _min, _max, s in zip(q_min, q_max, dqn)]
     # use the numpy slice magic to make X, Y, Z these are dense meshes with
     # points in the center of each bin
     X, Y, Z = np.mgrid[slc]
 
     # make and ravel the image data (which is all ones)
-    I = np.hstack([j * np.ones_like(X).ravel() for j in range(1, 6)])
+    I = np.hstack([j * np.ones_like(X).ravel() for j in range(1, 101)])
 
     # make input data (N*5x3)
-    data = np.vstack([np.tile(_, 5)
+    data = np.vstack([np.tile(_, 100)
                       for _ in (np.ravel(X), np.ravel(Y), np.ravel(Z))]).T
     (mean, occupancy,
-     std_err, oob, bounds) = core.grid3d(data, I, **param_dict)
+     std_err, bounds) = core.grid3d(data, I, **param_dict)
 
     # check the values are as expected
     npt.assert_array_equal(mean,
-                           np.ones_like(X) * np.mean(np.arange(1, 6)))
-    npt.assert_equal(oob, 0)
-    npt.assert_array_equal(occupancy, np.ones_like(occupancy)*5)
+                           np.ones_like(X) * np.mean(np.arange(1, 101)))
+    npt.assert_array_equal(occupancy, np.ones_like(occupancy) * 100)
     # need to convert std -> ste (standard error)
-    # according to wikipedia ste = std/sqrt(n), but experimentally, this is
-    # implemented as ste = std / srt(n - 1)
-    npt.assert_array_equal(std_err,
-                           (np.ones_like(occupancy) *
-                            np.std(np.arange(1, 6))/np.sqrt(5 - 1)))
+    # according to wikipedia ste = std/sqrt(n)
+    npt.assert_array_almost_equal(std_err,
+                                  (np.ones_like(occupancy) *
+                                   np.std(np.arange(1, 101)) / np.sqrt(100)))
 
 
 def test_bin_edge2center():
     test_edges = np.arange(11)
     centers = core.bin_edges_to_centers(test_edges)
     assert_array_almost_equal(.5, centers % 1)
     assert_equal(10, len(centers))
@@ -268,15 +273,15 @@
     assert_equal(dd['a'], 1)
     try:
         dd['b']
     except KeyError as e:
         assert_equal(eval(six.text_type(e)), expected_string)
     else:
         # did not raise a KeyError
-        assert(False)
+        assert (False)
 
 
 def test_large_verbosedict():
     expected_sting = ("You tried to access the key 'a' "
                       "which does not exist.  There are 100 "
                       "extant keys, which is too many to show you")
 
@@ -289,15 +294,15 @@
     # test failure
     try:
         dd['a']
     except KeyError as e:
         assert_equal(eval(six.text_type(e)), expected_sting)
     else:
         # did not raise a KeyError
-        assert(False)
+        assert (False)
 
 
 def test_d_q_conversion():
     assert_equal(2 * np.pi, core.d_to_q(1))
     assert_equal(2 * np.pi, core.q_to_d(1))
     test_data = np.linspace(.1, 5, 100)
     assert_array_almost_equal(test_data, core.d_to_q(core.q_to_d(test_data)),
@@ -325,23 +330,23 @@
 
 def test_radius_to_twotheta():
     dist_sample = 100
     radius = np.linspace(50, 100)
 
     two_theta = np.array(
         [0.46364761, 0.47177751, 0.47984053, 0.48783644, 0.49576508,
-         0.5036263,   0.51142,    0.51914611, 0.52680461, 0.53439548,
-         0.54191875,  0.54937448, 0.55676277, 0.56408372, 0.57133748,
-         0.57852421,  0.58564412, 0.5926974,  0.59968432, 0.60660511,
-         0.61346007,  0.62024949, 0.62697369, 0.63363301, 0.6402278,
-         0.64675843,  0.65322528, 0.65962874, 0.66596924, 0.67224718,
-         0.67846301,  0.68461716, 0.6907101,  0.69674228, 0.70271418,
-         0.70862627,  0.71447905, 0.720273,   0.72600863, 0.73168643,
-         0.73730693,  0.74287063, 0.74837805, 0.75382971, 0.75922613,
-         0.76456784,  0.76985537, 0.77508925, 0.78027,    0.78539816])
+         0.5036263, 0.51142, 0.51914611, 0.52680461, 0.53439548,
+         0.54191875, 0.54937448, 0.55676277, 0.56408372, 0.57133748,
+         0.57852421, 0.58564412, 0.5926974, 0.59968432, 0.60660511,
+         0.61346007, 0.62024949, 0.62697369, 0.63363301, 0.6402278,
+         0.64675843, 0.65322528, 0.65962874, 0.66596924, 0.67224718,
+         0.67846301, 0.68461716, 0.6907101, 0.69674228, 0.70271418,
+         0.70862627, 0.71447905, 0.720273, 0.72600863, 0.73168643,
+         0.73730693, 0.74287063, 0.74837805, 0.75382971, 0.75922613,
+         0.76456784, 0.76985537, 0.77508925, 0.78027, 0.78539816])
 
     assert_array_almost_equal(two_theta,
                               core.radius_to_twotheta(dist_sample,
                                                       radius), decimal=8)
 
 
 def test_multi_tau_lags():
@@ -524,15 +529,15 @@
             print('{0} calls successful'.format(num_calls))
 
 
 def test_angle_grid():
     a = core.angle_grid((3, 3), (7, 7))
     assert_equal(a[3, -1], 0)
     assert_almost_equal(a[3, 0], np.pi)
-    assert_almost_equal(a[4, 4], np.pi/4)  # (1, 1) should be 45 degrees
+    assert_almost_equal(a[4, 4], np.pi / 4)  # (1, 1) should be 45 degrees
     # The documented domain is [-pi, pi].
     correct_domain = np.all((a < np.pi + 0.1) & (a > -np.pi - 0.1))
     assert_true(correct_domain)
 
 
 def test_radial_grid():
     a = core.radial_grid((3, 3), (7, 7))
@@ -542,10 +547,28 @@
 
 def test_geometric_series():
     time_series = core.geometric_series(common_ratio=5, number_of_images=150)
 
     assert_array_equal(time_series, [1, 5, 25, 125])
 
 
+@known_fail_if(not pf)
+def test_bin_grid():
+    geo = Geometry(
+        detector='Perkin', pixel1=.0002, pixel2=.0002,
+        dist=.23,
+        poni1=.209, poni2=.207,
+        # poni1=0, poni2=0,
+        # rot1=.0128, rot2=-.015, rot3=-5.2e-8,
+        wavelength=1.43e-11
+    )
+    r_array = geo.rArray((2048, 2048))
+    img = r_array.copy()
+    x, y = core.bin_grid(img, r_array, (geo.pixel1, geo.pixel2))
+
+    assert_array_almost_equal(y, x, decimal=2)
+
+
 if __name__ == '__main__':
     import nose
+
     nose.runmodule(argv=['-s', '--with-doctest'], exit=False)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_dpc.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_dpc.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_feature.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_stats.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_arithmetic.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_mask.py` & `scikit-beam-0.0.9/skbeam/core/constants/tests/test_xrs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # ######################################################################
 # Copyright (c) 2014, Brookhaven Science Associates, Brookhaven        #
 # National Laboratory. All rights reserved.                            #
 #                                                                      #
+# @author: Li Li (lili@bnl.gov)                                        #
+# created on 08/19/2014                                                #
+#                                                                      #
 # Redistribution and use in source and binary forms, with or without   #
 # modification, are permitted provided that the following conditions   #
 # are met:                                                             #
 #                                                                      #
 # * Redistributions of source code must retain the above copyright     #
 #   notice, this list of conditions and the following disclaimer.      #
 #                                                                      #
@@ -29,58 +32,43 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
 from __future__ import absolute_import, division, print_function
-import logging
 
 import numpy as np
-from numpy.testing import assert_array_equal
-
-import skbeam.core.mask as mask
-
-logger = logging.getLogger(__name__)
-
-
-def test_threshold_mask():
-    xdim = 10
-    ydim = 10
-    stack_size = 10
-    img_stack = np.random.randint(1, 3, (stack_size, xdim, ydim))
-
-    img_stack[0][0, 1] = 100
-    img_stack[0][9, 1] = 98
-    img_stack[6][8, 8] = 75
-    img_stack[7][6, 6] = 80
+from numpy.testing import assert_array_equal, assert_array_almost_equal
+from nose.tools import assert_equal
 
-    th = mask.threshold_mask(img_stack, 75)
+from skbeam.core.constants.xrs import HKL, calibration_standards
+from skbeam.core.utils import q_to_d, d_to_q
 
-    for final in th:
-        pass
 
-    y = np.ones_like(img_stack[0])
-    y[0, 1] = 0
-    y[9, 1] = 0
-    y[8, 8] = 0
-    y[6, 6] = 0
+def smoke_test_powder_standard():
+    name = 'Si'
+    cal = calibration_standards[name]
+    assert(name == cal.name)
 
-    assert_array_equal(final, y)
+    for d, hkl, q in cal:
+        assert_array_almost_equal(d_to_q(d), q)
+        assert_array_almost_equal(q_to_d(q), d)
+        assert_array_equal(np.linalg.norm(hkl), hkl.length)
 
+    assert_equal(str(cal), "Calibration standard: Si")
+    assert_equal(len(cal), 11)
 
-def test_bad_to_nan_gen():
-    xdim = 2
-    ydim = 2
-    stack_size = 5
-    img_stack = np.random.randint(1, 3, (stack_size, xdim, ydim))
 
-    bad_list = [1, 3]
+def test_hkl():
+    a = HKL(1, 1, 1)
+    b = HKL('1', '1', '1')
+    c = HKL(h='1', k='1', l='1')
+    d = HKL(1.5, 1.5, 1.75)
+    assert_equal(a, b)
+    assert_equal(a, c)
+    assert_equal(a, d)
 
-    img = mask.bad_to_nan_gen(img_stack, bad_list)
-    y = []
-    for im in img:
-        y.append(im)
 
-    assert np.isnan(np.asarray(y)[1]).all()
-    assert np.isnan(np.asarray(y)[3]).all()
-    assert not np.isnan(np.asarray(y)[4]).all()
+if __name__ == '__main__':
+    import nose
+    nose.runmodule(argv=['-s', '--with-doctest'], exit=False)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_recip.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_recip.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_correlation.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_calibration.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/tests/test_speckle.py` & `scikit-beam-0.0.9/skbeam/core/tests/test_speckle.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/dpc.py` & `scikit-beam-0.0.9/skbeam/core/dpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,15 @@
 
 # attributes
 dpc_fit.solver = ['Nelder-Mead', 'Powell', 'CG', 'BFGS', 'Anneal', 'L-BFGS-B',
                   'TNC', 'COBYLA', 'SLSQP']
 
 
 def recon(gx, gy, scan_xstep, scan_ystep, padding=0, weighting=0.5):
-    """
-    Reconstruct the final phase image.
+    """Reconstruct the final phase image.
 
     Parameters
     ----------
     gx : ndarray
         Phase gradient along x direction.
 
     gy : ndarray
@@ -217,17 +216,21 @@
     scan_xstep : float
         Scanning step size in x direction (in micro-meter).
 
     scan_ystep : float
         Scanning step size in y direction (in micro-meter).
 
     padding : int, optional
-        Pad a N-by-M array to be a (N*(2*padding+1))-by-(M*(2*padding+1)) array
-        with the image in the middle with a (N*padding, M*padding) thick edge
+
+        Pad a N-by-M array to be a
+        ``(N*(2*padding+1))``-by-``(M*(2*padding+1))`` array with the
+        image in the middle with a (N*padding, M*padding) thick edge
         of zeros. Default is 0.
+
+
         padding = 0 --> v (the original image, size = (N, M))
                         0 0 0
         padding = 1 --> 0 v 0 (the padded image, size = (3 * N, 3 * M))
                         0 0 0
 
     weighting : float, optional
         Weighting parameter for the phase gradient along x and y direction when
@@ -447,17 +450,20 @@
     negate : bool, optional
         If True (default), negate the phase gradient along x direction before
         reconstructing the final phase image. Default is True.
     scale : bool, optional
         If True, scale gx and gy according to the experiment set up.
         If False, ignore pixel_size, focus_to_det, energy. Default is True.
     padding : int, optional
-        Pad a N-by-M array to be a (N*(2*padding+1))-by-(M*(2*padding+1)) array
-        with the image in the middle with a (N*padding, M*padding) thick edge
-        of zeros. Default is 0.
+
+        Pad a N-by-M array to be a
+        ``(N*(2*padding+1))``-by-``(M*(2*padding+1))`` array with the image in
+        the middle with a (N*padding, M*padding) thick edge of
+        zeros. Default is 0.
+
         padding = 0 --> v (the original image, size = (N, M))
                         0 0 0
         padding = 1 --> 0 v 0 (the padded image, size = (3 * N, 3 * M))
                         0 0 0
     weighting : float, optional
         Weighting parameter for the phase gradient along x and y direction when
         constructing the final phase image.
@@ -466,14 +472,15 @@
 
     Returns
     -------
     phase : ndarray
         The final reconstructed phase image.
     amplitude : ndarray
         Amplitude of the sample transmission function.
+
     """
     if weighting < 0 or weighting > 1:
         raise ValueError('weighting should be within the range of [0, 1]!')
     gx = None
     gy = dpc_state.gy
     if pixel_size and focus_to_det:
         # Convert to wavelength
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/correlation.py` & `scikit-beam-0.0.9/skbeam/core/correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,58 +235,57 @@
     num_bufs : int, must be even
         maximum lag step to compute in each generation of downsampling
     labels : array
         Labeled array of the same shape as the image stack.
         Each ROI is represented by sequential integers starting at one.  For
         example, if you have four ROIs, they must be labeled 1, 2, 3,
         4. Background is labeled as 0
-    labels : array
-        Labeled array of the same shape as the image stack.
-        Each ROI is represented by sequential integers starting at one.  For
-        example, if you have four ROIs, they must be labeled 1, 2, 3,
-        4. Background is labeled as 0
     internal_state : namedtuple, optional
         internal_state is a bucket for all of the internal state of the
         generator. It is part of the `results` object that is yielded from
         this generator
 
     Yields
     ------
     namedtuple
         A `results` object is yielded after every image has been processed.
         This `reults` object contains, in this order:
+
         - `g2`: the normalized correlation
           shape is (len(lag_steps), num_rois)
         - `lag_steps`: the times at which the correlation was computed
         - `_internal_state`: all of the internal state. Can be passed back in
           to `lazy_one_time` as the `internal_state` parameter
 
     Notes
     -----
     The normalized intensity-intensity time-autocorrelation function
     is defined as
 
     .. math::
+
         g_2(q, t') = \\frac{<I(q, t)I(q, t + t')> }{<I(q, t)>^2}
 
         t' > 0
 
     Here, ``I(q, t)`` refers to the scattering strength at the momentum
     transfer vector ``q`` in reciprocal space at time ``t``, and the brackets
     ``<...>`` refer to averages over time ``t``. The quantity ``t'`` denotes
     the delay time
 
     This implementation is based on published work. [1]_
 
     References
     ----------
+
     .. [1] D. Lumma, L. B. Lurio, S. G. J. Mochrie and M. Sutton,
-        "Area detector based photon correlation in the regime of
-        short data batches: Data reduction for dynamic x-ray
-        scattering," Rev. Sci. Instrum., vol 70, p 3274-3289, 2000.
+       "Area detector based photon correlation in the regime of
+       short data batches: Data reduction for dynamic x-ray
+       scattering," Rev. Sci. Instrum., vol 71, p 3274-3289, 2000.
+
     """
 
     if internal_state is None:
         internal_state = _init_state_one_time(num_levels, num_bufs, labels)
     # create a shorthand reference to the results and state named tuple
     s = internal_state
 
@@ -442,25 +441,28 @@
     for result in gen:
         pass
     return two_time_state_to_results(result)
 
 
 def lazy_two_time(labels, images, num_frames, num_bufs, num_levels=1,
                   two_time_internal_state=None):
-    """ Generator implementation of two-time correlation
+    """Generator implementation of two-time correlation
 
     If you do not want multi-tau correlation, set num_levels to 1 and
     num_bufs to the number of images you wish to correlate
 
     Multi-tau correlation uses a scheme to achieve long-time correlations
     inexpensively by downsampling the data, iteratively combining successive
     frames.
 
-    The longest lag time computed is num_levels * num_bufs.
-    ** see comments on multi_tau_auto_corr
+    The longest lag time computed is ``num_levels * num_bufs``.
+
+    See Also
+    --------
+    comments on `multi_tau_auto_corr`
 
     Parameters
     ----------
     labels : array
         labeled array of the same shape as the image stack;
         each ROI is represented by a distinct label (i.e., integer)
     images : iterable of 2D arrays
@@ -477,14 +479,15 @@
         default is one
 
     Yields
     ------
     namedtuple
         A ``results`` object is yielded after every image has been processed.
         This `reults` object contains, in this order:
+
         - ``g2``: the normalized correlation
           shape is (num_rois, len(lag_steps), len(lag_steps))
         - ``lag_steps``: the times at which the correlation was computed
         - ``_internal_state``: all of the internal state. Can be passed back in
           to ``lazy_one_time`` as the ``internal_state`` parameter
 
     Notes
@@ -499,21 +502,24 @@
     ``(t1+t2)/2``, measured by the distance along the ``t1 = t2`` diagonal.
     The time difference ``t = |t1 - t2|``, with is distance from the
     ``t1 = t2`` diagonal in the perpendicular direction.
     In the equilibrium system, the two-time correlation functions depend only
     on the time difference ``t``, and hence the two-time correlation contour
     lines are parallel.
 
+    [1]_
+
     References
     ----------
 
-    .. [1]
-        A. Fluerasu, A. Moussaid, A. Mandsen and A. Schofield, "Slow dynamics
-        and aging in collodial gels studied by x-ray photon correlation
-        spectroscopy," Phys. Rev. E., vol 76, p 010401(1-4), 2007.
+    .. [1] A. Fluerasu, A. Moussaid, A. Mandsen and A. Schofield,
+       "Slow dynamics and aging in collodial gels studied by x-ray
+       photon correlation spectroscopy," Phys. Rev. E., vol 76, p
+       010401(1-4), 2007.
+
     """
     if two_time_internal_state is None:
         two_time_internal_state = _init_state_two_time(num_levels, num_bufs,
                                                        labels, num_frames)
     # create a shorthand reference to the results and state named tuple
     s = two_time_internal_state
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/recip.py` & `scikit-beam-0.0.9/skbeam/core/recip.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,23 +46,22 @@
 import time
 
 try:
     from pyFAI import geometry as geo
 except ImportError:
     geo = None
 
-from ..ext import ctrans
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 def process_to_q(setting_angles, detector_size, pixel_size,
                  calibrated_center, dist_sample, wavelength, ub,
-                 frame_mode=None, n_threads=None):
+                 frame_mode=None):
     """
     This will compute the hkl values for all pixels in a shape specified by
     detector_size.
 
     Parameters
     ----------
     setting_angles : ndarray
@@ -99,19 +98,14 @@
         'theta'    : Theta axis frame.
         'phi'      : Phi axis frame.
         'cart'     : Crystal cartesian frame.
         'hkl'      : Reciprocal lattice units frame.
         See the `process_to_q.frame_mode` attribute for an exact list of
         valid options.
 
-    n_threads : int, optional
-        Specify the number of threads for the c-module to use in its
-        calculations. A value of None indicates to use the number of
-        configured cores on the system.
-
     Returns
     -------
     hkl : ndarray
         (Qx, Qy, Qz) - HKL values
         shape is [num_images * num_rows * num_columns][3]
 
     Notes
@@ -126,18 +120,23 @@
        1993.
 
     .. [2] E. Vlieg, "A (2+3)-Type surface diffractometer: Mergence of the
        z-axis and (2+2)-Type geometries," J. Appl. Cryst., vol 31, pp 198-203,
        1998.
 
     """
+    try:
+        from ..ext import ctrans
+    except ImportError:
+        raise NotImplementedError(
+            "ctrans is not available on your platform. See"
+            "https://github.com/scikit-beam/scikit-beam/issues/418"
+            "to follow updates to this problem.")
 
     # Set default threads
-    if n_threads is None:
-        n_threads = 0
 
     # set default frame_mode
     if frame_mode is None:
         frame_mode = 4
     else:
         str_to_int = verbosedict((k, j + 1) for j, k
                                  in enumerate(process_to_q.frame_mode))
@@ -164,16 +163,15 @@
     hkl = ctrans.ccdToQ(angles=setting_angles * np.pi / 180.0,
                         mode=frame_mode,
                         ccd_size=(detector_size),
                         ccd_pixsize=(pixel_size),
                         ccd_cen=(calibrated_center),
                         dist=dist_sample,
                         wavelength=wavelength,
-                        UBinv=np.matrix(ub).I,
-                        n_threads=n_threads)
+                        UBinv=np.matrix(ub).I)
 
     # ending time for the process
     t2 = time.time()
     logger.info("Processing time for {0} {1} x {2} images took {3} seconds."
                 "".format(setting_angles.shape[0], detector_size[0],
                           detector_size[1], (t2 - t1)))
     return hkl
@@ -265,46 +263,47 @@
         out of plane angle, default 0.0
 
     Returns
     -------
     namedtuple
         `gisaxs_output` object is returned
         This `gisaxs_output` object contains, in this order:
+
         - alpha_i : float
-            incident angle
+          incident angle
         - theta_f : array
-            out of plane angle
-            shape (detector_size[0], detector_size[1])
+          out of plane angle
+          shape (detector_size[0], detector_size[1])
         - alpha_f : array
-            exit angle
-            shape (detector_size[0], detector_size[1])
+          exit angle
+          shape (detector_size[0], detector_size[1])
         - tilt_angle : float
-            tilt angle
+          tilt angle
         - qx : array
-            x component of the scattering wave vector
-            shape (detector_size[0], detector_size[1])
+          x component of the scattering wave vector
+          shape (detector_size[0], detector_size[1])
         - qy : array
-            y component of the scattering wave vector
-            shape (detector_size[0], detector_size[1])
+          y component of the scattering wave vector
+          shape (detector_size[0], detector_size[1])
         - qz : array
-            z component of the scattering wave vector
-            shape (detector_size[0], detector_size[1])
+          z component of the scattering wave vector
+          shape (detector_size[0], detector_size[1])
         - qr : array
-            q parallel component
-            shape (detector_size[0], detector_size[1])
+          q parallel component
+          shape (detector_size[0], detector_size[1])
 
     Notes
     -----
     This implementation is based on published work. [1]_
 
     References
     ----------
     .. [1] R. Lazzari, "IsGISAXS: a program for grazing-incidence small-
-        angle X-ray scattering analysis of supported islands," J. Appl.
-        Cryst., vol 35, p 406-421, 2002.
+       angle X-ray scattering analysis of supported islands," J. Appl.
+       Cryst., vol 35, p 406-421, 2002.
     """
     inc_x, inc_y = incident_beam
     refl_x, refl_y = reflected_beam
 
     # convert pixel_size to meters
     pixel_size = np.asarray(pixel_size) * 10 ** (-6)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/spectroscopy.py` & `scikit-beam-0.0.9/skbeam/core/spectroscopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     Finds and estimates the location, width, and height of
     the largest peak. Assumes the top of the peak can be
     approximated as a Gaussian.  Finds the peak properties
     using least-squares fitting of a parabola to the log of
     the counts.
 
     The region around the peak can be approximated by
-    Y = Y0 * exp(- (X - X0)**2 / (2 * sigma **2))
+    :math:`Y = Y0 * exp(- (X - X0)**2 / (2 * sigma **2))`
 
     Parameters
     ----------
     x : ndarray
        The independent variable
 
     y : ndarary
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/mask.py` & `scikit-beam-0.0.9/skbeam/io/binary.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # ######################################################################
 # Copyright (c) 2014, Brookhaven Science Associates, Brookhaven        #
 # National Laboratory. All rights reserved.                            #
 #                                                                      #
-# Developed at the NSLS-II, Brookhaven National Laboratory             #
-# Developed by Sameera K. Abeykoon, January 2016                       #
-#                                                                      #
 # Redistribution and use in source and binary forms, with or without   #
 # modification, are permitted provided that the following conditions   #
 # are met:                                                             #
 #                                                                      #
 # * Redistributions of source code must retain the above copyright     #
 #   notice, this list of conditions and the following disclaimer.      #
 #                                                                      #
@@ -31,80 +28,66 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR   #
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
-
-"""
-This module is for functions specific to mask or threshold an image
-basically to clean images
-"""
-
 from __future__ import absolute_import, division, print_function
 import numpy as np
 
 import logging
 logger = logging.getLogger(__name__)
 
 
-def bad_to_nan_gen(images, bad):
+def read_binary(filename, nx, ny, nz, dtype_str, headersize):
     """
-    Convert the images marked as "bad" in `bad` by their index in
-    images into a np.nan array
+    docstring, woo!
 
     Parameters
     ----------
-    images : iterable
-        Iterable of 2-D arrays
-    bad : list
-        List of integer indices into the `images` parameter that mark those
-        images as "bad".
-
-    Yields
-    ------
-    img : array
-        if image is bad it will convert to np.nan array otherwise no
-        change to the array
-    """
-    ret_val = None
-    for n, im in enumerate(images):
-        if n in bad:
-            if ret_val is None:
-                ret_val = np.empty(im.shape)
-                ret_val[:] = np.nan
-            yield ret_val
-        else:
-            yield im
-
+    filename : String
+        The name of the file to open
+    nx : integer
+        The number of data elements in the x-direction
+    ny : integer
+        The number of data elements in the y-direction
+    nz : integer
+        The number of data elements in the z-direction
+    dtype_str : str
+        A valid argument for np.dtype(some_str). See read_binary.dsize
+        attribute
+    headersize : integer
+        The size of the file header in bytes
 
-def threshold_mask(images, threshold, mask=None):
+    Returns
+    -------
+    data : ndarray
+            data.shape = (x, y, z) if z > 1
+            data.shape = (x, y) if z == 1
+            data.shape = (x,) if y == 1 && z == 1
+    header : String
+            header = file.read(headersize)
     """
-    This generator sets all pixels whose value is greater than `threshold`
-    to 0 and yields the thresholded images out
 
-    Parameters
-    ----------
-    images : iterable
-        Iterable of 2-D arrays
-    threshold : float
-        threshold value to remove the hot spots in the image
-    mask : array
-        array with values above the threshold marked as 0 and values
-        below marked as 1.
-        shape is (num_columns, num_rows) of the image, optional None
+    # open the file
+    with open(filename, "rb") as opened_file:
+        # read the file header
+        header = opened_file.read(headersize)
+
+        # read the entire file in as 1D list
+        data = np.fromfile(file=opened_file, dtype=np.dtype(dtype_str),
+                           count=-1)
+
+    # reshape the array to 3D
+    if nz is not 1:
+        data.resize(nx, ny, nz)
+    # unless the 3rd dimension is 1, in which case reshape the array to 2D
+    elif ny is not 1:
+        data.resize(nx, ny)
+    # unless the 2nd dimension is also 1, in which case leave the array as 1D
 
-    Yields
-    -------
-    mask : array
-        array with values above the threshold marked as 0 and values
-        below marked as 1.
-        shape is (num_columns, num_rows) of the image
-    """
-    if mask is None:
-        mask = np.ones_like(images[0])
-    for im in images:
-        bad_pixels = np.where(im >= threshold)
-        if len(bad_pixels[0]) != 0:
-            mask[bad_pixels] = 0
-        yield mask
+    # return the array and the header
+    return data, header
+
+# set an attribute for the dsize params that are valid options
+read_binary.dtype_str = sorted(np.typeDict, key=str)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/xrf_model.py` & `scikit-beam-0.0.9/skbeam/core/fitting/xrf_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -969,14 +969,15 @@
         result = self.mod.fit(spectrum, pars, x=channel_number, weights=weights,
                               method=method, fit_kws=kwargs)
         return result
 
 
 def get_line_energy(elemental_line):
     """Return the energy of the first line in K, L or M series.
+
     Parameters
     ----------
     elemental_line : str
         For instance, Eu_L is the format for L lines and Pt_M for M lines.
         And for K lines, user needs to define lines like ka1, kb1,
         because for K lines, we consider contributions from either ka1
         or kb1, while for L or M lines, we only consider the primary peak.
@@ -1352,18 +1353,20 @@
         The row number that is being computed
     args
         The arguments to `fit_per_line_nnls`
     """
     logger.info('Row number at {}'.format(row_num))
     return fit_per_line_nnls(*args)
 
+
 def fit_pixel_multiprocess_nnls(exp_data, matv, param,
                                 use_snip=False):
     """
     Multiprocess fit of experiment data.
+
     Parameters
     ----------
     exp_data : array
         3D data of experiment spectrum,
         with x,y positions as the first 2-dim, and energy as the third one.
     matv : array
         matrix for regression analysis
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/base/parameter_data.py` & `scikit-beam-0.0.9/skbeam/core/fitting/base/parameter_data.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/base/__init__.py` & `scikit-beam-0.0.9/skbeam/core/fitting/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/funcs.py` & `scikit-beam-0.0.9/skbeam/core/fitting/funcs.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_background.py` & `scikit-beam-0.0.9/skbeam/core/fitting/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_xrf_fit.py` & `scikit-beam-0.0.9/skbeam/core/fitting/tests/test_xrf_fit.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/tests/test_lineshapes.py` & `scikit-beam-0.0.9/skbeam/core/fitting/tests/test_lineshapes.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/__init__.py` & `scikit-beam-0.0.9/skbeam/core/fitting/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/models.py` & `scikit-beam-0.0.9/skbeam/core/fitting/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         function of peak profile
 
     Returns
     -------
     str :
         documentation of the function
     """
-    return ("Wrap the {} function for fitting within lmfit "
-            "framework\n".format(func.__name__) + func.__doc__)
+    return ("    Wrap the {} function for fitting within lmfit "
+            "framework\n    ".format(func.__name__) + func.__doc__)
 
 
 # DEFINE NEW MODELS
 class ElasticModel(Model):
 
     __doc__ = _gen_class_docs(elastic)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/lineshapes.py` & `scikit-beam-0.0.9/skbeam/core/fitting/lineshapes.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/fitting/background.py` & `scikit-beam-0.0.9/skbeam/core/fitting/background.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/roi.py` & `scikit-beam-0.0.9/skbeam/core/roi.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 This module contain convenience methods to generate ROI labeled arrays for
 simple shapes such as rectangles and concentric circles.
 """
 from __future__ import absolute_import, division, print_function
 
 import collections
 import scipy.ndimage.measurements as ndim
+from skimage.draw import line
 import numpy as np
 from . import utils
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -367,16 +368,17 @@
         ROIs
 
     Returns
     -------
     mean_intensity : array
         The mean intensity of each ROI for all `images`
         Dimensions:
-            len(mean_intensity) == len(index)
-            len(mean_intensity[0]) == len(images)
+
+          -  len(mean_intensity) == len(index)
+          -  len(mean_intensity[0]) == len(images)
     index : list
         The labels for each element of the `mean_intensity` list
     """
     if labeled_array.shape != images[0].shape[0:]:
         raise ValueError(
             "`images` shape (%s) needs to be equal to the labeled_array shape"
             "(%s)" % (images[0].shape, labeled_array.shape))
@@ -394,47 +396,62 @@
     for n, img in enumerate(images):
         # use a mean that is mask-aware
         mean_intensity[n] = ndim.mean(img, labeled_array, index=index)
     return mean_intensity, index
 
 
 def circular_average(image, calibrated_center, threshold=0, nx=100,
-                     pixel_size=(1, 1),  min_x=None, max_x=None):
+                     pixel_size=(1, 1), min_x=None, max_x=None, mask=None):
     """Circular average of the the image data
     The circular average is also known as the radial integration
+
     Parameters
     ----------
     image : array
         Image to compute the average as a function of radius
     calibrated_center : tuple
         The center of the image in pixel units
         argument order should be (row, col)
     threshold : int, optional
-        Ignore counts above `threshold`
+        Ignore counts below `threshold`
         default is zero
     nx : int, optional
         number of bins in x
         defaults is 100 bins
     pixel_size : tuple, optional
         The size of a pixel (in a real unit, like mm).
         argument order should be (pixel_height, pixel_width)
         default is (1, 1)
     min_x : float, optional number of pixels
         Left edge of first bin defaults to minimum value of x
     max_x : float, optional number of pixels
         Right edge of last bin defaults to maximum value of x
+    mask : mask for 2D data. Assumes 1 is non masked and 0 masked.
+        None defaults to no mask.
+
     Returns
     -------
     bin_centers : array
         The center of each bin in R. shape is (nx, )
     ring_averages : array
         Radial average of the image. shape is (nx, ).
+
+    See Also
+    --------
+    bad_to_nan_gen : Create a mask with np.nan entries
+    bin_grid : Bin and integrate an image, given the radial array of pixels
+        Useful for nonlinear spacing (Ewald curvature)
     """
     radial_val = utils.radial_grid(calibrated_center, image.shape, pixel_size)
 
+    if mask is not None:
+        w = np.where(mask == 1)
+        radial_val = radial_val[w]
+        image = image[w]
+
     bin_edges, sums, counts = utils.bin_1D(np.ravel(radial_val),
                                            np.ravel(image), nx,
                                            min_x=min_x,
                                            max_x=max_x)
     th_mask = counts > threshold
     ring_averages = sums[th_mask] / counts[th_mask]
 
@@ -576,15 +593,15 @@
     if not np.all(np.diff(edges) >= 0):
         raise ValueError("edges are expected to be monotonically increasing, "
                          "giving inner and outer radii of each bar from "
                          "r=0 outward")
     if values is None:
         values = np.repeat(range(shape[0]), shape[1])
     if not horizontal:
-        values = values.reshape(shape).T.ravel()
+        values = np.tile(range(shape[1]), shape[0])
 
     return _make_roi(values, edges, shape)
 
 
 def box(shape, v_edges, h_edges=None, h_values=None, v_values=None):
     """Draw box shaped rois when the horizontal and vertical edges
      are provided.
@@ -636,7 +653,41 @@
                              "giving inner, outer edges for each roi")
     coords = []
     for h in h_edges:
         for v in v_edges:
             coords.append((h[0], v[0], h[1]-h[0], v[1] - v[0]))
 
     return rectangles(coords, v_values.shape)
+
+
+def lines(end_points, shape):
+    """
+    Parameters
+    ----------
+    end_points : iterable
+        coordinates of the starting point and the ending point of each
+        line: e.g., [(start_x, start_y, end_x, end_y), (x1, y1, x2, y2)]
+    shape : tuple
+        Image shape which is used to determine the maximum extent of output
+        pixel coordinates. Order is (rr, cc).
+
+    Returns
+    -------
+    label_array : array
+        Elements not inside any ROI are zero; elements inside each
+        ROI are 1, 2, 3, corresponding to the order they are specified
+        in coords. Order is (rr, cc).
+
+    """
+    label_array = np.zeros(shape, dtype=np.int64)
+    label = 0
+    for points in end_points:
+        if len(points) != 4:
+            raise ValueError("end points should have four number of"
+                             " elements, giving starting co-ordinates,"
+                             " ending co-ordinates for each line")
+        rr, cc = line(np.max([points[0], 0]), np.max([points[1], 0]),
+                      np.min([points[2], shape[0]-1]),
+                      np.min([points[3], shape[1]-1]))
+        label += 1
+        label_array[rr, cc] = label
+    return label_array
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/arithmetic.py` & `scikit-beam-0.0.9/skbeam/core/arithmetic.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/data/AtomicConstants.dat` & `scikit-beam-0.0.9/skbeam/core/constants/data/AtomicConstants.dat`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/basic.py` & `scikit-beam-0.0.9/skbeam/core/constants/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     >>> e.density
     7.14
     """
 
 
 @functools.total_ordering
 class BasicElement(object):
+
     # define the docs
     __doc__ = """{}
     Parameters
     ----------{}
     Attributes
     ----------{}
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/xrs.py` & `scikit-beam-0.0.9/skbeam/core/constants/xrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,14 @@
 
     Parameters
     ----------
     h : int
     k : int
     l : int
 
-    Attributes
-    ----------
-    length
-    h
-    k
-    l
     '''
     __slots__ = ()
 
     def __new__(cls, *args, **kwargs):
         args = [int(_) for _ in args]
         for k in list(kwargs):
             kwargs[k] = int(kwargs[k])
@@ -101,19 +95,14 @@
 
     hkl : `hkl`
         miller indicies
 
     q : float
         q-value of the reflection
 
-    Attributes
-    ----------
-    d
-    HKL
-    q
     """
     __slots__ = ()
 
 
 class PowderStandard(object):
     """
     Class for providing safe access to powder calibration standards
@@ -153,15 +142,15 @@
         return self._reflections
 
     def __iter__(self):
         return iter(self._reflections)
 
     def convert_2theta(self, wavelength):
         """
-        Convert the measured 2theta values to a different wavelength
+        Convert the measured $2theta$ values to a different wavelength
 
         Parameters
         ----------
         wavelength : float
             The new lambda in Angstroms
 
         Returns
@@ -248,14 +237,15 @@
 # https://www-s.nist.gov/srmors/certificates/640D.pdf?CFID=3219362&CFTOKEN=c031f50442c44e42-57C377F6-BC7A-395A-F39B8F6F2E4D0246&jsessionid=f030c7ded9b463332819566354567a698744
 
 # CeO2 (Standard Reference Material 674b) data taken from
 # http://11bm.xray.aps.anl.gov/documents/NISTSRM/NIST_SRM_676b_%5BZnO,TiO2,Cr2O3,CeO2%5D.pdf
 
 # Alumina (Al2O3), (Standard Reference Material 676a) taken from
 # https://www-s.nist.gov/srmors/certificates/676a.pdf?CFID=3259108&CFTOKEN=fa5bb0075f99948c-FA6ABBDA-9691-7A6B-FBE24BE35748DC08&jsessionid=f030e1751fc5365cac74417053f2c344f675
+#: Mapping of known calibration standards and their reflections
 calibration_standards = {
     'Si': PowderStandard.from_lambda_2theta_hkl(
         name='Si',
         wavelength=1.5405929,
         two_theta=np.deg2rad([28.441, 47.3, 56.119, 69.126, 76.371, 88.024,
                               94.946, 106.7, 114.082, 127.532, 136.877]),
         hkl=((1, 1, 1), (2, 2, 0), (3, 1, 1), (4, 0, 0), (3, 3, 1), (4, 2, 2),
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/xrf.py` & `scikit-beam-0.0.9/skbeam/core/constants/xrf.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,20 +104,22 @@
 
     line_dict = verbosedict((k.lower(), v) for k, v in zip(line_name,
                                                            line_list))
 
     shell_dict = verbosedict((k.lower(), v) for k, v in zip(bindingE,
                                                             shell_list))
 
-    XRAYLIB_MAP = verbosedict({'lines': (line_dict, xraylib.LineEnergy),
-                               'cs': (line_dict, xraylib.CS_FluorLine_Kissel),
-                               'binding_e': (shell_dict, xraylib.EdgeEnergy),
-                               'jump': (shell_dict, xraylib.JumpFactor),
-                               'yield': (shell_dict, xraylib.FluorYield),
-                               })
+    XRAYLIB_MAP = verbosedict({
+        'lines': (line_dict, xraylib.LineEnergy),
+        'cs': (line_dict, xraylib.CS_FluorLine_Kissel),
+        'csb': (line_dict, xraylib.CSb_FluorLine_Kissel),
+        'binding_e': (shell_dict, xraylib.EdgeEnergy),
+        'jump': (shell_dict, xraylib.JumpFactor),
+        'yield': (shell_dict, xraylib.FluorYield),
+        })
 
 
 class XrayLibWrap(Mapping):
     """High-level interface to xraylib.
 
     This class exposes various functions in xraylib
 
@@ -134,19 +136,14 @@
     info_type : {'lines',  'binding_e', 'jump', 'yield'}
         option to choose which physics quantity to calculate as follows:
         :lines: emission lines
         :binding_e: binding energy
         :jump: absorption jump factor
         :yield: fluorescence yield
 
-    Attributes
-    ----------
-    info_type : str
-
-
     Examples
     --------
     Access the lines for zinc
 
     >>> x = XrayLibWrap(30, 'lines') # 30 is atomic number for element Zn
 
     Access the energy of the Kα1 line.
@@ -228,42 +225,42 @@
 class XrayLibWrap_Energy(XrayLibWrap):
     """
     This is an interface to wrap xraylib
     to perform calculation on fluorescence
     cross section, or other incident energy
     related quantity.
 
-    Attributes
-    ----------
-    incident_energy : float
-    info_type : str
-
     Parameters
     ----------
     element : int
         atomic number
-    info_type : {'cs'}, optional
+    info_type : {'cs', 'csb'}, optional
         option to calculate physics quantities which depend on
         incident energy.
         See Class attribute `opts_info_type` for valid options
 
         :cs: cross section, unit in cm2/g
+        :csb: cross section, unit in barns/atom
 
     incident_energy : float
         incident energy for fluorescence in KeV
 
     Examples
     --------
     >>> # Cross section of zinc with an incident X-ray at 12 KeV
     >>> x = XrayLibWrap_Energy(30, 'cs', 12)
     >>> # Compute the cross section of the Kα1 line.
     >>> x['Ka1'] # cross section for Ka1, unit in cm2/g
-    34.44424057006836
+    34.68250086875594
+    >>> xb = XrayLibWrap_Energy(30, 'csb', 12)
+    >>> # Compute the cross section of the Kα1 line.
+    >>> xb['Ka1'] # cross section for Ka1, unit in barns/atom
+    3765.3415913117224
     """
-    opts_info_type = ['cs']
+    opts_info_type = ['cs', 'csb']
 
     def __init__(self, element, info_type, incident_energy):
         if xraylib is None:
             raise XraylibNotInstalledError(self.__class__)
 
         super(XrayLibWrap_Energy, self).__init__(element, info_type)
         self._incident_energy = incident_energy
@@ -303,25 +300,33 @@
     Object to return all the elemental information related to fluorescence
     """
 # dont change the doc_params
 doc_params = doc_params
 #
 doc_attrs += """    emission_line : `XrayLibWrap`
     cs : function
+    csb : function
     bind_energy : `XrayLibWrap`
     jump_factor : `XrayLibWrap`
     fluor_yield : `XrayLibWrap`
     """
-doc_ex += """>>> # Get the emission energy for the Kα1 line.
-    >>> e.emission_line['Ka1'] #
+doc_ex += """
+    >>> from skbeam.core.constants.xrf import XrfElement as Element
+    >>> e = Element('Zn')
+    >>> # Get the emission energy for the Kα1 line.
+    >>> e.emission_line['Ka1']
     8.638900756835938
 
-    >>> Cross section for emission line Kα1 with 10 keV incident energy
+    >>> # Cross section [barns/atom] for Kα1 line at 10 keV incident energy
+    >>> e.csb(10)['Ka1']
+    5987.081587605121
+
+    >>> # Cross section [cm2/g] for Kα1 line at 10 keV incident energy
     >>> e.cs(10)['Ka1']
-    54.756561279296875
+    55.146912259583296
 
     >>> # fluorescence yield for K shell
     >>> e.fluor_yield['K']
     0.46936899423599243
 
     >>> # Find all emission lines within with in the range [9.5, 10.5]
     >>> # keV with an incident energy of 12 KeV.
@@ -348,52 +353,50 @@
      ('ll', 0.8837999701499939),
      ('ln', 0.9069000482559204),
      ('ma1', 0.0),
      ('ma2', 0.0),
      ('mb', 0.0),
      ('mg', 0.0)]
 
-    >>> # List all of the known cross sections
-    >>> e.cs(10).all
-    [('ka1', 54.756561279296875),
-     ('ka2', 28.13692855834961),
-     ('kb1', 7.509212970733643),
+    >>> # List all of the known cross sections [barns/atom]
+    >>> e.csb(10).all
+    [('ka1', 5987.081587605121),
+     ('ka2', 3076.4914784265347),
+     ('kb1', 821.0572112842519),
      ('kb2', 0.0),
-     ('la1', 0.13898827135562897),
-     ('la2', 0.01567710004746914),
-     ('lb1', 0.0791187509894371),
+     ('la1', 188.06856034970164),
+     ('la2', 21.213083101234524),
+     ('lb1', 94.10717616654374),
      ('lb2', 0.0),
-     ('lb3', 0.004138986114412546),
-     ('lb4', 0.002259803470224142),
+     ('lb3', 6.2207984090565),
+     ('lb4', 3.3964315566384187),
      ('lb5', 0.0),
      ('lg1', 0.0),
      ('lg2', 0.0),
      ('lg3', 0.0),
      ('lg4', 0.0),
-     ('ll', 0.008727769367396832),
-     ('ln', 0.00407258840277791),
+     ('ll', 11.809765990232954),
+     ('ln', 4.8441078404731766),
      ('ma1', 0.0),
      ('ma2', 0.0),
      ('mb', 0.0),
      ('mg', 0.0)]
     """""
 
 
 class XrfElement(BasicElement):
     # define the docs
     __doc__ = """{}
     Parameters
     ----------{}
-    Attributes
-    ----------{}
+
     Examples
     --------{}
     """.format(doc_title,
                doc_params,
-               doc_attrs,
                doc_ex)
 
     def __init__(self, element):
         if xraylib is None:
             raise XraylibNotInstalledError(self.__class__)
 
         super(XrfElement, self).__init__(element)
@@ -422,22 +425,41 @@
         elemental cross section in cm2/g
 
         The signature of the function is ::
 
            x_section = func(enery)
 
         where `energy` in in keV and `x_section` is in
-        cm²/g
+        cm2/g
         """
         def myfunc(incident_energy):
             return XrayLibWrap_Energy(self.Z, 'cs',
                                       incident_energy)
         return myfunc
 
     @property
+    def csb(self):
+        """Fluorescence cross section function, `function`
+
+        Returns a function of energy which returns the
+        elemental cross section in barns/atom
+
+        The signature of the function is ::
+
+           x_section = func(enery)
+
+        where `energy` in in keV and `x_section` is in
+        barns/atom
+        """
+        def myfunc(incident_energy):
+            return XrayLibWrap_Energy(self.Z, 'csb',
+                                      incident_energy)
+        return myfunc
+
+    @property
     def bind_energy(self):
         """Binding energy, `XrayLibWrap`
 
         Binding energy is a measure of the energy required
         to free electrons from their atomic orbits.
         shell is string type and defined as "K", "L1".
         unit in KeV
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_xrf.py` & `scikit-beam-0.0.9/skbeam/core/constants/tests/test_xrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
 from __future__ import absolute_import, division, print_function
 import six
-from numpy.testing import (assert_array_equal, assert_raises)
+import numpy as np
+from numpy.testing import (assert_array_equal, assert_array_almost_equal,
+                           assert_raises)
 from nose.tools import assert_equal, assert_not_equal
 
 from skbeam.core.constants.xrf import (XrfElement, emission_line_search,
                                        XrayLibWrap, XrayLibWrap_Energy)
 from skbeam.core.utils import NotInstalledError
 from skbeam.core.constants.basic import basic
 
@@ -114,14 +116,26 @@
                                       incident_energy=incident_energy)
             incident_energy *= 2
             xlwe.incident_energy = incident_energy
             assert_equal(xlwe.incident_energy, incident_energy)
             assert_equal(xlwe.info_type, infotype)
 
 
+def test_cs_different_units():
+    e = XrfElement('Fe')
+    # test at different energies
+    for eng in range(10, 20):
+        cs1 = np.array([v for k, v in e.cs(eng).all])   # unit in cm2/g
+        cs2 = np.array([v for k, v in e.csb(eng).all])  # unit in barns/atom
+        cs1 /= cs1[0]
+        cs2 /= cs2[0]
+        # ratio should be the same no matter which unit is used
+        assert_array_almost_equal(cs1, cs2, decimal=10)
+
+
 def smoke_test_element_creation():
     prev_element = None
     elements = [elm for abbrev, elm in six.iteritems(basic)
                 if isinstance(abbrev, int)]
     elements.sort()
     for element in elements:
         Z = element.Z
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_basic.py` & `scikit-beam-0.0.9/skbeam/core/constants/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_xrs.py` & `scikit-beam-0.0.9/skbeam/core/constants/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,44 +31,18 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR   #
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
-from __future__ import absolute_import, division, print_function
 
-import numpy as np
-from numpy.testing import assert_array_equal, assert_array_almost_equal
-from nose.tools import assert_equal
-
-from skbeam.core.constants.xrs import HKL, calibration_standards
-from skbeam.core.utils import q_to_d, d_to_q
-
-
-def smoke_test_powder_standard():
-    name = 'Si'
-    cal = calibration_standards[name]
-    assert(name == cal.name)
-
-    for d, hkl, q in cal:
-        assert_array_almost_equal(d_to_q(d), q)
-        assert_array_almost_equal(q_to_d(q), d)
-        assert_array_equal(np.linalg.norm(hkl), hkl.length)
-
-    assert_equal(str(cal), "Calibration standard: Si")
-    assert_equal(len(cal), 11)
-
-
-def test_hkl():
-    a = HKL(1, 1, 1)
-    b = HKL('1', '1', '1')
-    c = HKL(h='1', k='1', l='1')
-    d = HKL(1.5, 1.5, 1.75)
-    assert_equal(a, b)
-    assert_equal(a, c)
-    assert_equal(a, d)
 
+# smoketest the api
+from skbeam.core.constants.basic import BasicElement
+from skbeam.core.constants.xrs import calibration_standards
+from skbeam.core.constants.xrf import XrfElement
+from skbeam.core.constants.xrf import emission_line_search
 
 if __name__ == '__main__':
     import nose
     nose.runmodule(argv=['-s', '--with-doctest'], exit=False)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/tests/test_api.py` & `scikit-beam-0.0.9/skbeam/io/tests/test_fit2d_save.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # ######################################################################
 # Copyright (c) 2014, Brookhaven Science Associates, Brookhaven        #
 # National Laboratory. All rights reserved.                            #
 #                                                                      #
-# @author: Li Li (lili@bnl.gov)                                        #
-# created on 08/19/2014                                                #
-#                                                                      #
 # Redistribution and use in source and binary forms, with or without   #
 # modification, are permitted provided that the following conditions   #
 # are met:                                                             #
 #                                                                      #
 # * Redistributions of source code must retain the above copyright     #
 #   notice, this list of conditions and the following disclaimer.      #
 #                                                                      #
@@ -32,17 +29,26 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
 
+"""
+    This module is for test output.py saving integrated powder
+    x-ray diffraction intensities into  different file formats.
+    (Output into different file formats, .chi, .dat, .xye, gsas)
+    Added a test to check the GSAS file reader and file writer
+"""
+from __future__ import absolute_import, division, print_function
+import os
+import numpy as np
+from skbeam.io.fit2d_save import fit2d_save
+
+
+def test_save_output_for_smoke():
+    filename = "function_values"
+    msk = np.ones((2048, 2048))
 
-# smoketest the api
-from skbeam.core.constants.basic import BasicElement
-from skbeam.core.constants.xrs import calibration_standards
-from skbeam.core.constants.xrf import XrfElement
-from skbeam.core.constants.xrf import emission_line_search
+    fit2d_save(msk, filename, dir_path=None)
 
-if __name__ == '__main__':
-    import nose
-    nose.runmodule(argv=['-s', '--with-doctest'], exit=False)
+    os.remove("function_values.msk")
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/constants/__init__.py` & `scikit-beam-0.0.9/skbeam/core/constants/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,15 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR   #
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
+'''Constants
+'''
 from .basic import BasicElement
 from .xrs import calibration_standards
 from .xrf import XrfElement, emission_line_search
 
 import logging
-logger = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/image.py` & `scikit-beam-0.0.9/skbeam/testing/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ######################################################################
+########################################################################
 # Copyright (c) 2014, Brookhaven Science Associates, Brookhaven        #
 # National Laboratory. All rights reserved.                            #
 #                                                                      #
 # Redistribution and use in source and binary forms, with or without   #
 # modification, are permitted provided that the following conditions   #
 # are met:                                                             #
 #                                                                      #
@@ -29,70 +29,69 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)   #
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
 """
-This is the module for putting advanced/x-ray specific image
-processing tools.  These should be interesting compositions of existing
-tools, not just straight wrapping of np/scipy/scikit images.
+This module is for decorators related to testing.
+
+Much of this code is inspired by the code in matplotlib.  Exact copies
+are noted.
 """
-from __future__ import absolute_import, division, print_function
-import numpy as np
-import logging
-logger = logging.getLogger(__name__)
+from skbeam.testing.noseclasses import (KnownFailureTest,
+                                        KnownFailureDidNotFailTest)
+
+import nose
+from nose.tools import make_decorator
 
 
-def find_ring_center_acorr_1D(input_image):
+def known_fail_if(cond):
     """
-    Find the pixel-resolution center of a set of concentric rings.
+    Make sure a known failure fails.
 
-    This function uses correlation between the image and it's mirror
-    to find the approximate center of  a single set of concentric rings.
-    It is assumed that there is only one set of rings in the image.  For
-    this method to work well the image must have significant mirror-symmetry
-    in both dimensions.
-
-    Parameters
-    ----------
-    input_image : ndarray
-        A single image.
-
-    Returns
-    -------
-    calibrated_center : tuple
-        Returns the index (row, col) of the pixel that rings
-        are centered on.  Accurate to pixel resolution.
+    This function is a decorator factory.
     """
-    return tuple(bins[np.argmax(vals)] for vals, bins in
-                 (_corr_ax1(_im) for _im in (input_image.T, input_image)))
+    # make the decorator function
+    def dec(in_func):
+        # make the wrapper function
+        # if the condition is True
+        if cond:
+            def inner_wrap():
+                # try the test anywoy
+                try:
+                    in_func()
+                # when in fails, raises KnownFailureTest
+                # which is registered with nose and it will be marked
+                # as K in the results
+                except Exception:
+                    raise KnownFailureTest()
+                # if it does not fail, raise KnownFailureDidNotFailTest which
+                # is a normal exception.  This may seem counter-intuitive
+                # but knowing when tests that _should_ fail don't can be useful
+                else:
+                    raise KnownFailureDidNotFailTest()
+            # use `make_decorator` from nose to make sure that the meta-data on
+            # the function is forwarded properly (name, teardown, setup, etc)
+            return make_decorator(in_func)(inner_wrap)
+
+        # if the condition is false, don't make a wrapper function
+        # this is effectively a no-op
+        else:
+            return in_func
 
+    # return the decorator function
+    return dec
 
-def _corr_ax1(input_image):
-    """
-    Internal helper function that finds the best estimate for the
-    location of the vertical mirror plane.  For each row the maximum
-    of the correlating with it's mirror is found.  The most common value
-    is reported back as the location of the mirror plane.
-
-    Parameters
-    ----------
-    input_image : ndarray
-        The input image
-
-    Returns
-    -------
-    vals : ndarray
-        histogram of what pixel has the highest correlation
 
-    bins : ndarray
-        Bin edges for the vals histogram
+def skip_if(cond, msg=''):
+    """
+    A decorator to skip a test if condition is met
     """
-    dim = input_image.shape[1]
-    m_ones = np.ones(dim)
-    norm_mask = np.correlate(m_ones, m_ones, mode='full')
-    # not sure that the /2 is the correct correction
-    est_by_row = [
-        np.argmax(np.correlate(v, v[::-1], mode='full')/norm_mask) / 2
-        for v in input_image]
-    return np.histogram(est_by_row, bins=np.arange(0, dim + 1))
+    def dec(in_func):
+        if cond:
+            def wrapper():
+                raise nose.SkipTest(msg)
+            return make_decorator(in_func)(wrapper)
+        else:
+            return in_func
+    return dec
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/core/cdi.py` & `scikit-beam-0.0.9/skbeam/core/cdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,29 +237,29 @@
               sw_flag=True, sw_sigma=0.5, sw_threshold=0.1, sw_start=0.2,
               sw_end=0.8, sw_step=10, n_iterations=1000,
               cb_function=None, cb_step=10):
     """
     Run reconstruction with difference map algorithm.
 
     Parameters
-    ---------
+    ----------
     diffracted_pattern : array
         diffraction pattern from experiments
     sample_obj : array
         initial sample with phase, complex number
     sup : array
         initial support
     beta : float, optional
         feedback parameter for difference map algorithm.
         default is 1.15.
     start_avg : float, optional
         define the point to start doing average.
         default is 0.8.
-    pi_modulus_flag : str, optional
-        'Complex' or 'Real', defining the way to perform pi_modulus
+    pi_modulus_flag : {'complex', 'real'}, optional
+        'complex' or 'real', defining the way to perform pi_modulus
         calculation.
         default is 'Complex'.
     sw_flag : Bool, optional
         flag to use shrinkwrap algorithm or not.
         default is True.
     sw_sigma : float, optional
         gaussian width used in sw algorithm.
@@ -306,17 +306,23 @@
     .. [1] V. Elser, "Phase retrieval by iterated projections",
         J. Opt. Soc. Am. A, vol. 20, No. 1, 2003
     """
 
     diffracted_pattern = np.array(diffracted_pattern)     # diffraction data
     diffracted_pattern = np.fft.fftshift(diffracted_pattern)
 
+    pi_modulus_flag = pi_modulus_flag.lower()
     real_operation = False
-    if pi_modulus_flag.lower() == 'real':
+    if pi_modulus_flag == 'real':
         real_operation = True
+    elif pi_modulus_flag == 'complex':
+        real_operation = False
+    else:
+        raise ValueError('py_modulus_flag must be one of {"complex",'
+                         'real"} not' '{!r}'.format(pi_modulus_flag))
 
     gamma_1 = -1/beta
     gamma_2 = 1/beta
 
     # get support index
     outside_sup_index = sup != 1
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/save_powder_output.py` & `scikit-beam-0.0.9/skbeam/io/save_powder_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,20 @@
 """
     This module is for saving integrated powder x-ray diffraction
     intensities into  different file formats.
     (Output into different file formats, .chi, .dat and .xye)
 
 """
 from __future__ import absolute_import, division, print_function
-import numpy as np
-import os
+
 import logging
+import os
+
+import numpy as np
+
 logger = logging.getLogger(__name__)
 
 
 def save_output(tth, intensity, output_name, q_or_2theta, ext='.chi',
                 err=None, dir_path=None):
     """
     Save output diffraction intensities into .chi, .dat or .xye file formats.
@@ -132,14 +135,15 @@
     f.write(_HEADER.encode('utf-8'))
 
 
 def gsas_writer(tth, intensity, output_name, mode=None,
                 err=None, dir_path=None):
     """
     Save diffraction intensities into .gsas file format
+
     Parameters
     ----------
     tth : ndarray
         twotheta values (degrees) shape (N, ) array
     intensity : ndarray
         intensity values shape (N, ) array
     output_name : str
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/avizo_io.py` & `scikit-beam-0.0.9/skbeam/io/avizo_io.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/net_cdf_io.py` & `scikit-beam-0.0.9/skbeam/io/net_cdf_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 The functions included in this module focus on reading and writing
 netCDF files. This is the file format used by Mark Rivers for
 x-ray computed microtomography data collected at Argonne National Laboratory,
 Sector 13BMD, GSECars.
 """
 from __future__ import division, absolute_import, print_function
 import os
-from netCDF4 import Dataset
 
 
 def load_netCDF(file_name):
     """
     This function loads the specified netCDF file format data set (e.g.*.volume
     APS-Sector 13 GSECARS extension) file into a numpy array for further
     analysis.
@@ -58,14 +57,15 @@
     data : ndarray
         ndarray containing the image data contained in the netCDF file.
         The image data is scaled using the scale factor defined in the
         netCDF metadata, if a scale factor was recorded during data
         acquisition or reconstruction. If a scale factor is not present,
         then a default value of 1.0 is used.
     """
+    from netCDF4 import Dataset
 
     with Dataset(os.path.normpath(file_name), 'r') as src_file:
         data = src_file.variables['VOLUME']
         md_dict = src_file.__dict__
         # Check for voxel intensity scale factor and apply if value is present
         data /= data.scale_factor if data.scale_factor != 1.0 else 1.0
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/tests/test_powder_output.py` & `scikit-beam-0.0.9/skbeam/io/tests/test_powder_output.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/__init__.py` & `scikit-beam-0.0.9/skbeam/io/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,  #
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OTHERWISE) ARISING   #
 # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE   #
 # POSSIBILITY OF SUCH DAMAGE.                                          #
 ########################################################################
 from __future__ import absolute_import, division, print_function
 
-import six
 import logging
+
 logger = logging.getLogger(__name__)
 
 try:
     from .net_cdf_io import load_netCDF
 except ImportError:
     def load_netCDF(*args, **kwargs):
         # Die at call time so as not to ruin entire io package.
```

### Comparing `scikit-beam-0.0.8.post0/skbeam/io/gsas_file_reader.py` & `scikit-beam-0.0.9/skbeam/io/gsas_file_reader.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/diffraction.py` & `scikit-beam-0.0.9/skbeam/diffraction.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/tests/test_openness.py` & `scikit-beam-0.0.9/skbeam/tests/test_openness.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/tests/__init__.py` & `scikit-beam-0.0.9/skbeam/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/fluorescence.py` & `scikit-beam-0.0.9/skbeam/fluorescence.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/__init__.py` & `scikit-beam-0.0.9/skbeam/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-beam-0.0.8.post0/skbeam/testing/decorators.py` & `scikit-beam-0.0.9/skbeam/testing/noseclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 ########################################################################
+# This file contains code from numpy and matplotlib (noted in the code)#
+# which is (c) the respective projects.                                #
+#                                                                      #
+# Modifications and original code are (c) BNL/BSA, license below       #
+#                                                                      #
 # Copyright (c) 2014, Brookhaven Science Associates, Brookhaven        #
 # National Laboratory. All rights reserved.                            #
 #                                                                      #
 # Redistribution and use in source and binary forms, with or without   #
 # modification, are permitted provided that the following conditions   #
 # are met:                                                             #
 #                                                                      #
@@ -34,64 +39,53 @@
 ########################################################################
 """
 This module is for decorators related to testing.
 
 Much of this code is inspired by the code in matplotlib.  Exact copies
 are noted.
 """
-from skbeam.testing.noseclasses import (KnownFailureTest,
-                                        KnownFailureDidNotFailTest)
+from __future__ import absolute_import, division, print_function
 
-import nose
-from nose.tools import make_decorator
+import os
+from nose.plugins.errorclass import ErrorClass, ErrorClassPlugin
 
 
-def known_fail_if(cond):
-    """
-    Make sure a known failure fails.
-
-    This function is a decorator factory.
-    """
-    # make the decorator function
-    def dec(in_func):
-        # make the wrapper function
-        # if the condition is True
-        if cond:
-            def inner_wrap():
-                # try the test anywoy
-                try:
-                    in_func()
-                # when in fails, raises KnownFailureTest
-                # which is registered with nose and it will be marked
-                # as K in the results
-                except Exception:
-                    raise KnownFailureTest()
-                # if it does not fail, raise KnownFailureDidNotFailTest which
-                # is a normal exception.  This may seem counter-intuitive
-                # but knowing when tests that _should_ fail don't can be useful
-                else:
-                    raise KnownFailureDidNotFailTest()
-            # use `make_decorator` from nose to make sure that the meta-data on
-            # the function is forwarded properly (name, teardown, setup, etc)
-            return make_decorator(in_func)(inner_wrap)
-
-        # if the condition is false, don't make a wrapper function
-        # this is effectively a no-op
-        else:
-            return in_func
-
-    # return the decorator function
-    return dec
-
-
-def skip_if(cond, msg=''):
-    """
-    A decorator to skip a test if condition is met
-    """
-    def dec(in_func):
-        if cond:
-            def wrapper():
-                raise nose.SkipTest(msg)
-            return make_decorator(in_func)(wrapper)
-        else:
-            return in_func
-    return dec
+# copied from matplotlib
+class KnownFailureDidNotFailTest(Exception):
+    '''Raise this exception to mark a test should have failed but did not.'''
+    pass
+
+
+# This code is copied from numpy
+class KnownFailureTest(Exception):
+    '''Raise this exception to mark a test as a known failing test.'''
+    pass
+
+
+# This code is copied from numpy
+class KnownFailure(ErrorClassPlugin):
+    '''Plugin that installs a KNOWNFAIL error class for the
+    KnownFailureClass exception.  When KnownFailureTest is raised,
+    the exception will be logged in the knownfail attribute of the
+    result, 'K' or 'KNOWNFAIL' (verbose) will be output, and the
+    exception will not be counted as an error or failure.
+
+    '''
+    enabled = True
+    knownfail = ErrorClass(KnownFailureTest,
+                           label='KNOWNFAIL',
+                           isfailure=False)
+
+    def options(self, parser, env=os.environ):
+        env_opt = 'NOSE_WITHOUT_KNOWNFAIL'
+        parser.add_option('--no-knownfail', action='store_true',
+                          dest='noKnownFail', default=env.get(env_opt, False),
+                          help='Disable special handling of KnownFailureTest '
+                               'exceptions')
+
+    def configure(self, options, conf):
+        if not self.can_configure:
+            return
+        self.conf = conf
+        disable = getattr(options, 'noKnownFail', False)
+        if disable:
+            self.enabled = False
```

