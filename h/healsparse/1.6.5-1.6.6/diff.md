# Comparing `tmp/healsparse-1.6.5.tar.gz` & `tmp/healsparse-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healsparse-1.6.5.tar", last modified: Wed Jun 21 23:52:20 2023, max compression
+gzip compressed data, was "healsparse-1.6.6.tar", last modified: Wed Jul 26 18:02:50 2023, max compression
```

## Comparing `healsparse-1.6.5.tar` & `healsparse-1.6.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 23:52:04.000000 healsparse-1.6.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 23:52:04.000000 healsparse-1.6.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.963693 healsparse-1.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.967694 healsparse-1.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 23:52:04.000000 healsparse-1.6.5/.github/workflows/python-package-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 23:52:04.000000 healsparse-1.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-21 23:52:04.000000 healsparse-1.6.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-21 23:52:04.000000 healsparse-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 23:52:04.000000 healsparse-1.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 23:52:20.979695 healsparse-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-21 23:52:04.000000 healsparse-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-21 23:52:04.000000 healsparse-1.6.5/api_changes_to_1.0.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.971694 healsparse-1.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/basic_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/concatenation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/filespec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/operations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/randoms.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 23:52:04.000000 healsparse-1.6.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.975694 healsparse-1.6.5/healsparse/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/cat_healsparse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    79398 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/healSparseRandoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_coverage_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/io_map_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/parquet_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-21 23:52:04.000000 healsparse-1.6.5/healsparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.975694 healsparse-1.6.5/healsparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 23:52:20.000000 healsparse-1.6.5/healsparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-21 23:52:04.000000 healsparse-1.6.5/long_description.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 23:52:04.000000 healsparse-1.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 23:52:20.979695 healsparse-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 23:52:04.000000 healsparse-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_applymask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_buildmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_cat_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_coverage_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_coverage_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    29282 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_degrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_emptypixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_fits_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_fracdet_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_from_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_generate_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_getset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_healSparseCoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_healpix_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_io_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_moc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47867 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_recarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_single_covpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_single_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_singlevalues.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_update_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_validarea.py
--rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-06-21 23:52:04.000000 healsparse-1.6.5/tests/test_widemasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-21 23:52:04.000000 healsparse-1.6.5/tutorial/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:52:20.979695 healsparse-1.6.5/ups/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 23:52:04.000000 healsparse-1.6.5/ups/healsparse.table
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.943028 healsparse-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 18:02:32.000000 healsparse-1.6.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 18:02:32.000000 healsparse-1.6.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.931027 healsparse-1.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.931027 healsparse-1.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 18:02:32.000000 healsparse-1.6.6/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-26 18:02:32.000000 healsparse-1.6.6/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-26 18:02:32.000000 healsparse-1.6.6/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:02:32.000000 healsparse-1.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-26 18:02:32.000000 healsparse-1.6.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-26 18:02:32.000000 healsparse-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 18:02:32.000000 healsparse-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 18:02:50.943028 healsparse-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-26 18:02:32.000000 healsparse-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-26 18:02:32.000000 healsparse-1.6.6/api_changes_to_1.0.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.935027 healsparse-1.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/basic_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/concatenation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/filespec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/operations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/randoms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:02:32.000000 healsparse-1.6.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.935027 healsparse-1.6.6/healsparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/cat_healsparse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79535 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/healSparseMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/healSparseRandoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_coverage_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_coverage_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_map_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_map_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/io_map_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/parquet_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-26 18:02:32.000000 healsparse-1.6.6/healsparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.939028 healsparse-1.6.6/healsparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 18:02:50.000000 healsparse-1.6.6/healsparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-26 18:02:50.000000 healsparse-1.6.6/healsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:02:50.000000 healsparse-1.6.6/healsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 18:02:50.000000 healsparse-1.6.6/healsparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 18:02:50.000000 healsparse-1.6.6/healsparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 18:02:32.000000 healsparse-1.6.6/long_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 18:02:32.000000 healsparse-1.6.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 18:02:50.943028 healsparse-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-26 18:02:32.000000 healsparse-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.943028 healsparse-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_applymask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_buildmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_cat_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_coverage_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_coverage_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29282 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_degrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_emptypixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_fits_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_fracdet_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_from_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_generate_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_getset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_healSparseCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_healpix_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_io_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_moc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_recarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_single_covpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_single_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_singlevalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_update_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_validarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35373 2023-07-26 18:02:32.000000 healsparse-1.6.6/tests/test_widemasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.943028 healsparse-1.6.6/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-07-26 18:02:32.000000 healsparse-1.6.6/tutorial/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:02:50.943028 healsparse-1.6.6/ups/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 18:02:32.000000 healsparse-1.6.6/ups/healsparse.table
```

### Comparing `healsparse-1.6.5/.github/workflows/python-package-pr.yml` & `healsparse-1.6.6/.github/workflows/python-package-pr.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/.github/workflows/python-package-publish.yml` & `healsparse-1.6.6/.github/workflows/python-package-publish.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/.github/workflows/python-package-push.yml` & `healsparse-1.6.6/.github/workflows/python-package-push.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/.readthedocs.yml` & `healsparse-1.6.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/LICENSE` & `healsparse-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/PKG-INFO` & `healsparse-1.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.6.5
+Version: 1.6.6
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and others
 Author-email: erykoff@stanford.edu
 Description-Content-Type: text/markdown
 Provides-Extra: parquet
 Provides-Extra: healpy
```

### Comparing `healsparse-1.6.5/README.md` & `healsparse-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/api_changes_to_1.0.md` & `healsparse-1.6.6/api_changes_to_1.0.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/Makefile` & `healsparse-1.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/basic_interface.rst` & `healsparse-1.6.6/docs/basic_interface.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/concatenation.rst` & `healsparse-1.6.6/docs/concatenation.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/conf.py` & `healsparse-1.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/filespec.rst` & `healsparse-1.6.6/docs/filespec.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/geometry.rst` & `healsparse-1.6.6/docs/geometry.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/index.rst` & `healsparse-1.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/install.rst` & `healsparse-1.6.6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/make.bat` & `healsparse-1.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/modules.rst` & `healsparse-1.6.6/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/operations.rst` & `healsparse-1.6.6/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/docs/randoms.rst` & `healsparse-1.6.6/docs/randoms.rst`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/__init__.py` & `healsparse-1.6.6/healsparse/__init__.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/cat_healsparse_files.py` & `healsparse-1.6.6/healsparse/cat_healsparse_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/fits_shim.py` & `healsparse-1.6.6/healsparse/fits_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/geom.py` & `healsparse-1.6.6/healsparse/geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/healSparseCoverage.py` & `healsparse-1.6.6/healsparse/healSparseCoverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/healSparseMap.py` & `healsparse-1.6.6/healsparse/healSparseMap.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,17 +529,18 @@
             is_single_value = True
 
         # First, check if these are the same type
         if not is_single_value and not isinstance(_values, np.ndarray):
             raise ValueError("Values are not a numpy ndarray")
 
         if hasattr(pixels, "__len__") and len(pixels) == 0:
-            if not is_single_value:
-                raise ValueError("Shape mismatch: cannot set an array of values "
-                                 "to a zero-length list of pixels.")
+            if len(_values) != 0:
+                warnings.warn("Shape mismatch: using a non-zero-length array of values "
+                              "to set a zero-length list of pixels.",
+                              UserWarning)
             # Nothing to do
             return
 
         if not nest:
             _pix = hpg.ring_to_nest(self._nside_sparse, pixels)
         else:
             _pix = pixels
@@ -736,15 +737,18 @@
 
         Returns
         -------
         values : `np.ndarray`
             Array of values/validity from the map.
         """
         if hasattr(pixels, "__len__") and len(pixels) == 0:
-            return np.array([], dtype=self.dtype)
+            if self._is_wide_mask:
+                return np.zeros((0, self._wide_mask_width), dtype=self.dtype)
+            else:
+                return np.array([], dtype=self.dtype)
 
         if not nest:
             _pix = hpg.ring_to_nest(self._nside_sparse, pixels)
         else:
             _pix = pixels
 
         if nside is not None:
@@ -1554,18 +1558,17 @@
             test_value = np.zeros(1, key.dtype)[0]
             if not is_integer_value(test_value):
                 raise IndexError("Numpy array indices must be integers for __getitem__")
             return self.get_values_pix(key)
         elif isinstance(key, list):
             # Make sure that it's integers
             arr = np.atleast_1d(key)
-            if len(arr) == 0:
-                return np.array([], dtype=self.dtype)
-            if not is_integer_value(arr[0]):
-                raise IndexError("List array indices must be integers for __getitem__")
+            if len(arr) > 0:
+                if not is_integer_value(arr[0]):
+                    raise IndexError("List array indices must be integers for __getitem__")
             return self.get_values_pix(arr)
         else:
             raise IndexError("Illegal index type (%s) for __getitem__ in HealSparseMap." %
                              (key.__class__))
 
     def __setitem__(self, key, value):
         """
```

### Comparing `healsparse-1.6.5/healsparse/healSparseRandoms.py` & `healsparse-1.6.6/healsparse/healSparseRandoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_coverage.py` & `healsparse-1.6.6/healsparse/io_coverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_coverage_fits.py` & `healsparse-1.6.6/healsparse/io_coverage_fits.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_coverage_parquet.py` & `healsparse-1.6.6/healsparse/io_coverage_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_map.py` & `healsparse-1.6.6/healsparse/io_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_map_fits.py` & `healsparse-1.6.6/healsparse/io_map_fits.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_map_healpix.py` & `healsparse-1.6.6/healsparse/io_map_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/io_map_parquet.py` & `healsparse-1.6.6/healsparse/io_map_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/operations.py` & `healsparse-1.6.6/healsparse/operations.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/parquet_shim.py` & `healsparse-1.6.6/healsparse/parquet_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse/utils.py` & `healsparse-1.6.6/healsparse/utils.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/healsparse.egg-info/PKG-INFO` & `healsparse-1.6.6/healsparse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healsparse
-Version: 1.6.5
+Version: 1.6.6
 Summary: Sparse healpix maps and geometry library
 Home-page: https://github.com/lsstdesc/healsparse
 Author: Eli Rykoff, Javier Sanchez, and others
 Author-email: erykoff@stanford.edu
 Description-Content-Type: text/markdown
 Provides-Extra: parquet
 Provides-Extra: healpy
```

### Comparing `healsparse-1.6.5/healsparse.egg-info/SOURCES.txt` & `healsparse-1.6.6/healsparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/long_description.md` & `healsparse-1.6.6/long_description.md`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/setup.py` & `healsparse-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_applymask.py` & `healsparse-1.6.6/tests/test_applymask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_astype.py` & `healsparse-1.6.6/tests/test_astype.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_buildmaps.py` & `healsparse-1.6.6/tests/test_buildmaps.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_cat_files.py` & `healsparse-1.6.6/tests/test_cat_files.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_coverage_map.py` & `healsparse-1.6.6/tests/test_coverage_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_coverage_mask.py` & `healsparse-1.6.6/tests/test_coverage_mask.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_degrade.py` & `healsparse-1.6.6/tests/test_degrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_emptypixels.py` & `healsparse-1.6.6/tests/test_emptypixels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 import numpy.testing as testing
 import numpy as np
 
 import healsparse
+from healsparse import WIDE_MASK
 
 
 class EmptyPixelsTestCase(unittest.TestCase):
     def test_emptypixels_get_values(self):
         """
         Test getting an empty list via get_values_pix()
         """
@@ -14,67 +15,100 @@
         m[1000] = 1.0
 
         empty_arr = np.array([], dtype=m.dtype)
 
         testing.assert_array_equal(m.get_values_pix([]), empty_arr)
         testing.assert_array_equal(m.get_values_pix(np.array([], dtype=np.int64)), empty_arr)
 
+    def test_emptypixels_get_values_widemask(self):
+        """
+        Test getting an empty list via get_values_pix() (wide mask).
+        """
+        m = healsparse.HealSparseMap.make_empty(32, 512, WIDE_MASK, wide_mask_maxbits=16)
+        testing.assert_array_equal(m.get_values_pix([]), np.zeros((0, 2), dtype=np.uint8))
+
     def test_emptypixels_get_by_index(self):
         """
         Test getting an empty list by index
         """
         m = healsparse.HealSparseMap.make_empty(32, 512, np.float64)
         m[1000] = 1.0
 
         empty_arr = np.array([], dtype=m.dtype)
 
         testing.assert_array_equal(m[[]], empty_arr)
         testing.assert_array_equal(m[np.array([], dtype=np.int64)], empty_arr)
 
+    def test_emptypixels_get_by_index_widemask(self):
+        """
+        Test getting an empty list by index (wide mask).
+        """
+        m = healsparse.HealSparseMap.make_empty(32, 512, WIDE_MASK, wide_mask_maxbits=16)
+        testing.assert_array_equal(m[[]], np.zeros((0, 2), dtype=np.uint8))
+
     def test_emptypixels_get_by_slice(self):
         """
         Test getting an empty pixel list by slice
         """
         m = healsparse.HealSparseMap.make_empty(32, 512, np.float64)
         m[1000] = 1.0
 
         empty_arr = np.array([], dtype=m.dtype)
 
         testing.assert_array_equal(m[0: 0], empty_arr)
 
+    def test_emptypixels_get_by_slice_widemask(self):
+        """
+        Test getting an empty pixel list by slice (wide mask).
+        """
+        m = healsparse.HealSparseMap.make_empty(32, 512, WIDE_MASK, wide_mask_maxbits=16)
+        testing.assert_array_equal(m[0: 0], np.zeros((0, 2), dtype=np.uint8))
+
     def test_emptypixels_update_values(self):
         """
         Test setting an empty list with update_values_pix
         """
         m = healsparse.HealSparseMap.make_empty(32, 512, np.int64)
         m[1000] = 1
 
-        m.update_values_pix([], 100)
+        m.update_values_pix([], np.array([], dtype=np.int64))
         self.assertEqual(m[1000], 1)
         self.assertEqual(len(m.valid_pixels), 1)
 
-        m.update_values_pix(np.array([], dtype=np.int32), 100)
+        m.update_values_pix(np.array([], dtype=np.int32), np.array([], dtype=np.int64))
         self.assertEqual(m[1000], 1)
         self.assertEqual(len(m.valid_pixels), 1)
 
-        self.assertRaises(ValueError, m.update_values_pix, [], np.zeros(5, dtype=m.dtype))
+        m.update_values_pix([], np.array([], dtype=np.int64))
+
+        self.assertWarns(UserWarning, m.update_values_pix, [], np.zeros(5, dtype=m.dtype))
+        self.assertWarns(UserWarning, m.update_values_pix, [], 5)
+
+        m.update_values_pos(
+            np.array([], dtype=np.float64),
+            np.array([], dtype=np.float64),
+            np.array([], dtype=np.int64),
+        )
 
     def test_emptypixels_set_by_index(self):
         """
         Test setting an empty list by index
         """
         m = healsparse.HealSparseMap.make_empty(32, 512, np.int32)
         m[1000] = 1
 
-        m[[]] = 100
+        m[[]] = np.array([], dtype=np.int32)
         self.assertEqual(m[1000], 1)
         self.assertEqual(len(m.valid_pixels), 1)
 
-        m[np.array([], dtype=np.int32)] = 100
+        m[np.array([], dtype=np.int32)] = np.array([], dtype=np.int32)
         self.assertEqual(m[1000], 1)
         self.assertEqual(len(m.valid_pixels), 1)
 
-        self.assertRaises(ValueError, m.__setitem__, [], np.zeros(5, dtype=np.int32))
+        m[[]] = np.array([], dtype=np.int32)
+
+        self.assertWarns(UserWarning, m.__setitem__, [], np.zeros(5, dtype=np.int32))
+        self.assertWarns(UserWarning, m.__setitem__, [], 100)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `healsparse-1.6.5/tests/test_fits_shim.py` & `healsparse-1.6.6/tests/test_fits_shim.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_fracdet_map.py` & `healsparse-1.6.6/tests/test_fracdet_map.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_from_healpix.py` & `healsparse-1.6.6/tests/test_from_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_generate_healpix.py` & `healsparse-1.6.6/tests/test_generate_healpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_geom.py` & `healsparse-1.6.6/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_getset.py` & `healsparse-1.6.6/tests/test_getset.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_healSparseCoverage.py` & `healsparse-1.6.6/tests/test_healSparseCoverage.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_healpix_io.py` & `healsparse-1.6.6/tests/test_healpix_io.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_io.py` & `healsparse-1.6.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_io_parquet.py` & `healsparse-1.6.6/tests/test_io_parquet.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_lookup.py` & `healsparse-1.6.6/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_metadata.py` & `healsparse-1.6.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_moc.py` & `healsparse-1.6.6/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_operations.py` & `healsparse-1.6.6/tests/test_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         Test map addition.
         """
         random.seed(seed=12345)
 
         nside_coverage = 32
         nside_map = 64
 
+        sparse_map_empty = healsparse.HealSparseMap.make_empty(nside_coverage, nside_map, np.float64)
+
         # Test adding two or three maps
 
         sparse_map1 = healsparse.HealSparseMap.make_empty(nside_coverage, nside_map, np.float64)
         pixel1 = np.arange(4000, 20000)
         pixel1 = np.delete(pixel1, 15000)
         values1 = np.random.random(size=pixel1.size)
         sparse_map1.update_values_pix(pixel1, values1)
@@ -57,15 +59,22 @@
         hpmap_sum_intersection[gd] = hpmap1[gd] + hpmap2[gd] + hpmap3[gd]
 
         testing.assert_almost_equal(hpmap_sum_intersection, added_map_intersection.generate_healpix_map())
 
         # Union addition
 
         # sum 2
-        added_map_union = healsparse.sum_union([sparse_map1, sparse_map2])
+        added_map_union = healsparse.sum_union(
+            [
+                sparse_map_empty,
+                sparse_map1,
+                sparse_map2,
+                sparse_map_empty
+            ]
+        )
 
         gd, = np.where((hpmap1 > hpg.UNSEEN) | (hpmap2 > hpg.UNSEEN))
         hpmap_sum_union = np.zeros_like(hpmap1) + hpg.UNSEEN
         # This hack works because we don't have summands going below zero...
         hpmap_sum_union[gd] = np.clip(hpmap1[gd], 0.0, None) + np.clip(hpmap2[gd], 0.0, None)
 
         testing.assert_almost_equal(hpmap_sum_union, added_map_union.generate_healpix_map())
```

### Comparing `healsparse-1.6.5/tests/test_randoms.py` & `healsparse-1.6.6/tests/test_randoms.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_recarray.py` & `healsparse-1.6.6/tests/test_recarray.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_single_covpix.py` & `healsparse-1.6.6/tests/test_single_covpix.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_single_datatypes.py` & `healsparse-1.6.6/tests/test_single_datatypes.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_singlevalues.py` & `healsparse-1.6.6/tests/test_singlevalues.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_update_values.py` & `healsparse-1.6.6/tests/test_update_values.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_upgrade.py` & `healsparse-1.6.6/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_validarea.py` & `healsparse-1.6.6/tests/test_validarea.py`

 * *Files identical despite different names*

### Comparing `healsparse-1.6.5/tests/test_widemasks.py` & `healsparse-1.6.6/tests/test_widemasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,14 +359,17 @@
         Test wide mask oring
         """
         random.seed(seed=12345)
 
         nside_coverage = 32
         nside_map = 64
 
+        sparse_map_empty = healsparse.HealSparseMap.make_empty(nside_coverage, nside_map, WIDE_MASK,
+                                                               wide_mask_maxbits=100)
+
         sparse_map1 = healsparse.HealSparseMap.make_empty(nside_coverage, nside_map, WIDE_MASK,
                                                           wide_mask_maxbits=100)
         pixel1 = np.arange(4000, 20000)
         pixel1 = np.delete(pixel1, 15000)
         values1 = np.random.poisson(size=(pixel1.size, sparse_map1._wide_mask_width), lam=2).astype(WIDE_MASK)
         sparse_map1.update_values_pix(pixel1, values1)
 
@@ -384,15 +387,25 @@
         gd, = np.where((arr1.sum(axis=1) > 0) & (arr2.sum(axis=1) > 0))
         for i in range(2):
             test_or_intersection = np.zeros_like(arr1[:, 0])
             test_or_intersection[gd] = arr1[gd, i] | arr2[gd, i]
             testing.assert_equal(or_map_intersection.get_values_pix(all_pixels)[:, i],
                                  test_or_intersection)
 
-        or_map_union = healsparse.or_union([sparse_map1, sparse_map2])
+        or_map_intersection_with_empty = healsparse.or_intersection(
+            [
+                sparse_map_empty,
+                sparse_map1,
+                sparse_map2
+            ]
+        )
+
+        self.assertEqual(or_map_intersection_with_empty.valid_pixels.size, 0)
+
+        or_map_union = healsparse.or_union([sparse_map_empty, sparse_map1, sparse_map2])
 
         gd, = np.where((arr1.sum(axis=1) > 0) | (arr2.sum(axis=1) > 0))
         for i in range(2):
             test_or_union = np.zeros_like(arr1[:, 0])
             test_or_union[gd] = arr1[gd, i] | arr2[gd, i]
             testing.assert_equal(or_map_union.get_values_pix(all_pixels)[:, i],
                                  test_or_union)
```

### Comparing `healsparse-1.6.5/tutorial/quickstart.ipynb` & `healsparse-1.6.6/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

