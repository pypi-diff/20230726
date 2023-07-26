# Comparing `tmp/kaldi_native_io-1.8.tar.gz` & `tmp/kaldi_native_io-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kaldi_native_io-1.8.tar", last modified: Sun Apr 24 07:57:02 2022, max compression
+gzip compressed data, was "dist/kaldi_native_io-1.9.tar", last modified: Fri Jun 10 03:43:22 2022, max compression
```

## Comparing `kaldi_native_io-1.8.tar` & `kaldi_native_io-1.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/cmake/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/cmake/Modules/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)    38053 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/cmake/Modules/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/cmake/Modules/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/stl-utils.h
--rw-r--r--   0 runner    (1001) docker     (121)    10420 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)    23638 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6971 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/wave-reader.h
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/parse-options.h
--rw-r--r--   0 runner    (1001) docker     (121)    17660 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table.h
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/posterior.h
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     9760 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io.h
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (121)    28597 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io.cc
--rw-r--r--   0 runner    (1001) docker     (121)    35672 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/basic-filebuf.h
--rw-r--r--   0 runner    (1001) docker     (121)     6959 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/posterior.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-semaphore.cc
--rw-r--r--   0 runner    (1001) docker     (121)    33218 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/compressed-matrix.cc
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/text-utils.h
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-shape.h
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-utils.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7410 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)     7664 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-vector.h
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-common.h
--rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder.h
--rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/parse-options.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-pipebuf.h
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/text-utils.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10557 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/compressed-matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)    10323 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-shape.cc
--rw-r--r--   0 runner    (1001) docker     (121)   100824 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)    10954 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-vector.cc
--rw-r--r--   0 runner    (1001) docker     (121)    25131 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-semaphore.h
--rw-r--r--   0 runner    (1001) docker     (121)    11909 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/wave-reader.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/python/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-table.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-matrix.cc
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/wave-reader.h
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-table.h
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldiio.h
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/compressed-matrix.cc
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/matrix-shape.h
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-vector.h
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldiio.cc
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/compressed-matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/matrix-shape.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-vector.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/csrc/wave-reader.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/python/kaldi_native_io/
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-04-24 07:57:01.000000 kaldi_native_io-1.8/kaldi_native_io/python/kaldi_native_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22457 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/kaldi_native_io/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_wave_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_matrix_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_pair_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_wave_info_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_htk_matrix_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_pair_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_posterior_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_vector_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_matrix_shape_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_token_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_compressed_matrix_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_token_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_gauss_post_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_matrix_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_bool_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_vector_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6867 2022-04-24 07:56:50.000000 kaldi_native_io-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-24 07:57:02.000000 kaldi_native_io-1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/cmake/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/cmake/Modules/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (121)    38053 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/cmake/Modules/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/cmake/Modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/cmake/googletest.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_token_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_vector_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_posterior_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_wave_info_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_matrix_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_compressed_matrix_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_wave_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_token_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_pair_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_gauss_post_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_matrix_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_htk_matrix_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_pair_vector_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_matrix_shape_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/tests/test_bool_writer_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/compressed-matrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldiio.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldiio.h
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/matrix-shape.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-table.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/compressed-matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/matrix-shape.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/wave-reader.h
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-table.h
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-matrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-vector.h
+-rw-r--r--   0 runner    (1001) docker     (121)      770 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/csrc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/python/kaldi_native_io/
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/python/kaldi_native_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22457 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/kaldi_native_io/table_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-semaphore.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10557 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/compressed-matrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/text-utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/stl-utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9760 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io.h
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/text-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-pipebuf.h
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-shape.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10420 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11909 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    33218 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/compressed-matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    23638 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-shape.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6971 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/wave-reader.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6959 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/posterior.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/parse-options.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    17660 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7410 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10323 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/parse-options.h
+-rw-r--r--   0 runner    (1001) docker     (121)   100824 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10954 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/posterior.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7664 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-vector.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-semaphore.h
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    35672 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/basic-filebuf.h
+-rw-r--r--   0 runner    (1001) docker     (121)    25131 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    28597 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io.cc
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/kaldi_native_io/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6867 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-10 03:43:14.000000 kaldi_native_io-1.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-10 03:43:22.000000 kaldi_native_io-1.9/kaldi_native_io.egg-info/requires.txt
```

### Comparing `kaldi_native_io-1.8/CMakeLists.txt` & `kaldi_native_io-1.9/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 endif()
 
 cmake_minimum_required(VERSION 3.3 FATAL_ERROR)
 
 
 project(kaldi_native_io CXX)
 
-set(KALDI_NATIVE_IO_VERSION "1.8")
+set(KALDI_NATIVE_IO_VERSION "1.9")
 
 set(ALLOWABLE_BUILD_TYPES Debug Release RelWithDebInfo MinSizeRel)
 set(DEFAULT_BUILD_TYPE "Release")
 set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS "${ALLOWABLE_BUILD_TYPES}")
 if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
   # CMAKE_CONFIGURATION_TYPES: with config type values from other generators (IDE).
   message(STATUS "No CMAKE_BUILD_TYPE given, default to ${DEFAULT_BUILD_TYPE}")
@@ -37,16 +37,21 @@
 set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
 
 set(CMAKE_SKIP_BUILD_RPATH FALSE)
 set(BUILD_RPATH_USE_ORIGIN TRUE)
 set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
-set(CMAKE_INSTALL_RPATH "$ORIGIN")
-set(CMAKE_BUILD_RPATH "$ORIGIN")
+if(NOT APPLE)
+  set(CMAKE_INSTALL_RPATH "$ORIGIN")
+  set(CMAKE_BUILD_RPATH "$ORIGIN")
+else()
+  set(CMAKE_INSTALL_RPATH "@loader_path")
+  set(CMAKE_BUILD_RPATH "@loader_path")
+endif()
 
 set(CMAKE_CXX_STANDARD 14 CACHE STRING "The C++ version to be used.")
 
 set(BUILD_SHARED_LIBS ON)
 if(WIN32)
   message(STATUS "Set BUILD_SHARED_LIBS to OFF for Windows")
   set(BUILD_SHARED_LIBS OFF CACHE BOOL "" FORCE)
```

### Comparing `kaldi_native_io-1.8/cmake/googletest.cmake` & `kaldi_native_io-1.9/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/cmake/pybind11.cmake` & `kaldi_native_io-1.9/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `kaldi_native_io-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/cmake/Modules/FetchContent.cmake` & `kaldi_native_io-1.9/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io.egg-info/PKG-INFO` & `kaldi_native_io-1.9/kaldi_native_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldi-native-io
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/csukuangfj/kaldi_native_io
 Author: Fangjun Kuang
 Author-email: csukuangfj@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Description:
```

### Comparing `kaldi_native_io-1.8/kaldi_native_io.egg-info/SOURCES.txt` & `kaldi_native_io-1.9/kaldi_native_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/LICENSE` & `kaldi_native_io-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/setup.py` & `kaldi_native_io-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/stl-utils.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/stl-utils.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs-inl.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs-inl.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/wave-reader.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/wave-reader.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/parse-options.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/parse-options.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/posterior.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/posterior.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-utils.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-utils.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/log.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/log.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/basic-filebuf.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/basic-filebuf.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/posterior.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/posterior.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-semaphore.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-semaphore.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/compressed-matrix.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/compressed-matrix.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix-inl.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix-inl.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/text-utils.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/text-utils.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-shape.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-shape.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-utils.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-utils.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-io-inl.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-io-inl.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-vector.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-vector.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-common.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-common.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/parse-options.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/parse-options.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-pipebuf.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-pipebuf.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/text-utils.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/text-utils.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/compressed-matrix.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/compressed-matrix.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-matrix.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-matrix.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/matrix-shape.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/matrix-shape.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-table-inl.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-table-inl.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-vector.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-vector.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-holder-inl.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-holder-inl.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/kaldi-semaphore.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/kaldi-semaphore.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/wave-reader.cc` & `kaldi_native_io-1.9/kaldi_native_io/csrc/wave-reader.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/csrc/io-funcs.h` & `kaldi_native_io-1.9/kaldi_native_io/csrc/io-funcs.h`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-table.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-table.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-matrix.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-matrix.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/compressed-matrix.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/compressed-matrix.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldiio.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldiio.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/matrix-shape.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/matrix-shape.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/kaldi-vector.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/kaldi-vector.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/csrc/wave-reader.cc` & `kaldi_native_io-1.9/kaldi_native_io/python/csrc/wave-reader.cc`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/kaldi_native_io/__init__.py` & `kaldi_native_io-1.9/kaldi_native_io/python/kaldi_native_io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,8 +66,8 @@
     SequentialTokenReader,
     SequentialTokenVectorReader,
     SequentialWaveInfoReader,
     SequentialWaveReader,
     TokenVectorWriter,
     TokenWriter,
 )
-__version__ = '1.8'
+__version__ = '1.9'
```

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/kaldi_native_io/table_types.py` & `kaldi_native_io-1.9/kaldi_native_io/python/kaldi_native_io/table_types.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_wave_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_wave_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/CMakeLists.txt` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_matrix_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_matrix_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_pair_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_pair_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_wave_info_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_wave_info_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_htk_matrix_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_htk_matrix_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_pair_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_pair_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_posterior_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_posterior_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_int32_vector_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_int32_vector_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_matrix_shape_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_matrix_shape_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_float_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_float_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_token_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_token_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_compressed_matrix_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_compressed_matrix_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_token_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_token_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_gauss_post_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_gauss_post_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_matrix_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_matrix_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_bool_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_bool_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/kaldi_native_io/python/tests/test_double_vector_writer_reader.py` & `kaldi_native_io-1.9/kaldi_native_io/python/tests/test_double_vector_writer_reader.py`

 * *Files identical despite different names*

### Comparing `kaldi_native_io-1.8/PKG-INFO` & `kaldi_native_io-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldi_native_io
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/csukuangfj/kaldi_native_io
 Author: Fangjun Kuang
 Author-email: csukuangfj@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Description:
```

### Comparing `kaldi_native_io-1.8/README.md` & `kaldi_native_io-1.9/README.md`

 * *Files identical despite different names*

