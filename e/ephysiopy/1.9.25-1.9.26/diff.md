# Comparing `tmp/ephysiopy-1.9.25.tar.gz` & `tmp/ephysiopy-1.9.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.25.tar", last modified: Mon Jul 17 14:34:41 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.26.tar", last modified: Wed Jul 26 12:56:01 2023, max compression
```

## Comparing `ephysiopy-1.9.25.tar` & `ephysiopy-1.9.26.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/cluster_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 14:34:30.000000 ephysiopy-1.9.25/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:34:41.224531 ephysiopy-1.9.25/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 14:34:41.000000 ephysiopy-1.9.25/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 14:34:41.228531 ephysiopy-1.9.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-17 14:34:31.000000 ephysiopy-1.9.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.641262 ephysiopy-1.9.26/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.641262 ephysiopy-1.9.26/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34751 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/cluster_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41418 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.645262 ephysiopy-1.9.26/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:56:01.641262 ephysiopy-1.9.26/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-26 12:56:01.000000 ephysiopy-1.9.26/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-26 12:56:01.000000 ephysiopy-1.9.26/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:56:01.000000 ephysiopy-1.9.26/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 12:56:01.000000 ephysiopy-1.9.26/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 12:56:01.000000 ephysiopy-1.9.26/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 12:56:01.649262 ephysiopy-1.9.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-26 12:55:51.000000 ephysiopy-1.9.26/setup.py
```

### Comparing `ephysiopy-1.9.25/LICENSE` & `ephysiopy-1.9.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/PKG-INFO` & `ephysiopy-1.9.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.25
+Version: 1.9.26
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.25/README.md` & `ephysiopy-1.9.26/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.26/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.26/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.26/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.26/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/binning.py` & `ephysiopy-1.9.26/ephysiopy/common/binning.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     @nBins.setter
     def nBins(self, value):
         '''
         Sets the number of bins
         '''
         if self.var2Bin == VariableToBin.XY:
             x_lims, y_lims = self._getXYLimits()
+            if type(value) == int: # bad python :(
+                value = [value]
             if len(value) == 1:
                 _x, bs_x = np.linspace(x_lims[0],
                                        x_lims[1],
                                        int(value[0]),
                                        retstep=True)
                 _y, bs_y = np.linspace(y_lims[0],
                                        y_lims[1],
```

### Comparing `ephysiopy-1.9.25/ephysiopy/common/cluster_old.py` & `ephysiopy-1.9.26/ephysiopy/common/cluster_old.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.26/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.26/ephysiopy/common/fieldcalcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -896,16 +896,15 @@
             im_centre = E.params[0:2]
             ellipse_axes = E.params[2:4]
             ellipse_angle = E.params[-1]
             ellipseXY = E.predict_xy(np.linspace(0, 2*np.pi, 50), E.params)
 
             # get the min containing circle given the eliipse minor axis
             from skimage.measure import CircleModel
-            _params = im_centre
-            _params.append(np.min(ellipse_axes))
+            _params = [im_centre, np.min(ellipse_axes)]
             circleXY = CircleModel().predict_xy(
                 np.linspace(0, 2*np.pi, 50), params=_params)
         except (TypeError, ValueError):  # non-iterable x and y
             ellipse_axes = None
             ellipse_angle = (None, None)
             ellipseXY = None
             circleXY = None
@@ -1063,14 +1062,15 @@
     if circleXY is None or ellipseXY is None:
         SAC_stats = grid_field_props(A)
         circleXY = SAC_stats['circleXY']
         ellipseXY = SAC_stats['ellipseXY']
         # The ellipse detection stuff might have failed, if so
         # return the original SAC
         if circleXY is None:
+            warnings.warn("Ellipse detection failed. Returning original SAC")
             return A
 
     tform = skimage.transform.AffineTransform()
     tform.estimate(ellipseXY, circleXY)
 
     """
     the transformation algorithms used here crop values < 0 to 0. Need to
@@ -1081,7 +1081,44 @@
     SACmin = np.nanmin(A.flatten())
     SACmax = np.nanmax(A.flatten())  # should be 1 if autocorr
     AA = A + 1
     deformedSAC = skimage.transform.warp(
         AA / np.nanmax(AA.flatten()), inverse_map=tform.inverse, cval=0)
     return skimage.exposure.rescale_intensity(
         deformedSAC, out_range=(SACmin, SACmax))
+
+def get_circular_regions(A: np.ndarray, **kwargs) -> list:
+    '''
+    Returns a list of images which are expanding circular
+    regions centred on the middle of the image out to the 
+    image edge. Used for calculating the grid score of each
+    image to find the one with the max grid score. Based on
+    some Moser paper I can't recall.
+
+    Parameters
+    ----------
+    A: np.ndarray - the SAC
+    
+    Valid kwargs
+    ------------
+    min_radius: int - the smallest radius circle to start with
+    '''
+    from skimage.measure import CircleModel, grid_points_in_poly
+
+    min_radius = 5
+    if 'min_radius' in kwargs.keys():
+        min_radius = kwargs['min_radius']
+        
+    centre = tuple([d//2 for d in np.shape(A)])
+    max_radius = min(tuple(np.subtract(np.shape(A), centre)))
+    t = np.linspace(0, 2*np.pi, 51)
+    circle = CircleModel()
+
+    result = []
+    for radius in range(min_radius, max_radius):
+        circle.params = [*centre, radius]
+        xy = circle.predict_xy(t)
+        mask = grid_points_in_poly(np.shape(A), xy)
+        im = A.copy()
+        im[~mask] = np.nan
+        result.append(im)
+    return result
```

### Comparing `ephysiopy-1.9.25/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.26/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.26/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.26/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.26/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.26/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/common/utils.py` & `ephysiopy-1.9.26/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.26/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.26/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/io/recording.py` & `ephysiopy-1.9.26/ephysiopy/io/recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         if "egf" in args:
             lfp = EEG(self.pname, egf=1)
         else:
             lfp = EEG(self.pname)
         if lfp is not None:
             self.EEGCalcs = EEGCalcsGeneric(lfp.sig, lfp.sample_rate)
 
-    def load_neural_data(self, pname: Path, *args, **kwargs) -> None:
+    def load_neural_data(self, pname: Path, *args, **kwargs):
         pass
 
     def load_cluster_data(self, *args, **kwargs):
         pass
 
     def load_settings(self, *args, **kwargs):
         return self.settings
```

### Comparing `ephysiopy-1.9.25/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.26/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.26/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.26/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.26/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.26/ephysiopy/visualise/plotting.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.26/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.25
+Version: 1.9.26
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.25/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.26/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.25/setup.py` & `ephysiopy-1.9.26/setup.py`

 * *Files identical despite different names*

