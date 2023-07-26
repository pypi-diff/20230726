# Comparing `tmp/mattress-0.0.1.tar.gz` & `tmp/mattress-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattress-0.0.1.tar", last modified: Tue Jul 25 19:46:55 2023, max compression
+gzip compressed data, was "mattress-0.0.2.tar", last modified: Wed Jul 26 05:46:36 2023, max compression
```

## Comparing `mattress-0.0.1.tar` & `mattress-0.0.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.723040 mattress-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-25 19:46:38.000000 mattress-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.671040 mattress-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.683040 mattress-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-25 19:46:38.000000 mattress-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 19:46:38.000000 mattress-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 19:46:38.000000 mattress-0.0.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-25 19:46:38.000000 mattress-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 19:46:38.000000 mattress-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 19:46:38.000000 mattress-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-25 19:46:38.000000 mattress-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 19:46:38.000000 mattress-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 19:46:38.000000 mattress-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-25 19:46:55.723040 mattress-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-25 19:46:38.000000 mattress-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.687040 mattress-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.687040 mattress-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-25 19:46:38.000000 mattress-0.0.1/docs/tutorial
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.679040 mattress-0.0.1/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.687040 mattress-0.0.1/extern/tatami/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 19:46:38.000000 mattress-0.0.1/extern/tatami/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.675040 mattress-0.0.1/extern/tatami/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.687040 mattress-0.0.1/extern/tatami/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/.github/workflows/run-gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.691040 mattress-0.0.1/extern/tatami/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.691040 mattress-0.0.1/extern/tatami/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.691040 mattress-0.0.1/extern/tatami/gallery/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/char2double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/colsums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/parallel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/print_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/read_h5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/read_mm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/gallery/src/sparse_extractor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.675040 mattress-0.0.1/extern/tatami/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.691040 mattress-0.0.1/extern/tatami/include/tatami/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/base/
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/base/Extractor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/base/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/base/Options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/base/SparseRange.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/base/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/dense/
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/dense/DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/isometric/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/arith_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/boolean_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/compare_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.695040 mattress-0.0.1/extern/tatami/include/tatami/other/
--rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/other/DelayedBind.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/other/DelayedCast.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/other/DelayedTranspose.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.699040 mattress-0.0.1/extern/tatami/include/tatami/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31532 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/primary_extraction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/sparse/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.699040 mattress-0.0.1/extern/tatami/include/tatami/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/stats/medians.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/stats/ranges.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/stats/sums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/stats/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/stats/variances.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.699040 mattress-0.0.1/extern/tatami/include/tatami/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/subset/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/tatami.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/include/tatami/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/ArrayView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/Oracles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/bind_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/convert_to_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/include/tatami_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/simulate_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/tatami_test.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/temp_file_path.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/test_access_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/test_column_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/test_oracle_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/test_row_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/include/tatami_test/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.679040 mattress-0.0.1/extern/tatami/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/tests/src/dense/
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/dense/DenseMatrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/tests/src/isometric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.703040 mattress-0.0.1/extern/tatami/tests/src/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    42562 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.707040 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    62049 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/isometric/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.707040 mattress-0.0.1/extern/tatami/tests/src/other/
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/other/DelayedBind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/other/DelayedCast.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/other/DelayedTranspose.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.707040 mattress-0.0.1/extern/tatami/tests/src/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.707040 mattress-0.0.1/extern/tatami/tests/src/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/medians.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/parallelize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/ranges.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/sums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/stats/variances.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.707040 mattress-0.0.1/extern/tatami/tests/src/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/subset/DelayedSubset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/ArrayView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/Oracles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/SomeNumericArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/bind_intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/convert_to_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/convert_to_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.679040 mattress-0.0.1/extern/tatami_hdf5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/extern/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.679040 mattress-0.0.1/extern/tatami_hdf5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.711040 mattress-0.0.1/extern/tatami_hdf5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.715040 mattress-0.0.1/extern/tatami_hdf5/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/src/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-25 19:46:39.000000 mattress-0.0.1/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 19:46:38.000000 mattress-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 19:46:55.723040 mattress-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-25 19:46:38.000000 mattress-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.679040 mattress-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.715040 mattress-0.0.1/src/mattress/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.715040 mattress-0.0.1/src/mattress/lib/
--rw-r--r--   0 runner    (1001) docker     (123)  1189094 2023-07-25 19:46:54.000000 mattress-0.0.1/src/mattress/lib/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/lib/bindings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/lib/bindings.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.723040 mattress-0.0.1/src/mattress/lib/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/lib/cpp/Mattress.h
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/lib/cpp/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/lib/cpp/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 19:46:38.000000 mattress-0.0.1/src/mattress/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.715040 mattress-0.0.1/src/mattress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-25 19:46:55.000000 mattress-0.0.1/src/mattress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-25 19:46:55.000000 mattress-0.0.1/src/mattress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:46:55.000000 mattress-0.0.1/src/mattress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:46:54.000000 mattress-0.0.1/src/mattress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-25 19:46:55.000000 mattress-0.0.1/src/mattress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:46:55.000000 mattress-0.0.1/src/mattress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.723040 mattress-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-25 19:46:38.000000 mattress-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-25 19:46:38.000000 mattress-0.0.1/tests/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-25 19:46:38.000000 mattress-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.834629 mattress-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-26 05:46:24.000000 mattress-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.778629 mattress-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.798629 mattress-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-26 05:46:24.000000 mattress-0.0.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 05:46:24.000000 mattress-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 05:46:24.000000 mattress-0.0.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 05:46:24.000000 mattress-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 05:46:24.000000 mattress-0.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 05:46:24.000000 mattress-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-26 05:46:24.000000 mattress-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 05:46:24.000000 mattress-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 05:46:24.000000 mattress-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 05:46:36.834629 mattress-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-26 05:46:24.000000 mattress-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.802629 mattress-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.802629 mattress-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-26 05:46:24.000000 mattress-0.0.2/docs/tutorial
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 05:46:24.000000 mattress-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 05:46:36.834629 mattress-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-26 05:46:24.000000 mattress-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.778629 mattress-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.802629 mattress-0.0.2/src/mattress/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/TatamiNumericPointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.790629 mattress-0.0.2/src/mattress/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.806629 mattress-0.0.2/src/mattress/extern/tatami/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.782629 mattress-0.0.2/src/mattress/extern/tatami/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.806629 mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.806629 mattress-0.0.2/src/mattress/extern/tatami/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.806629 mattress-0.0.2/src/mattress/extern/tatami/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.810629 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/char2double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/colsums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/parallel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/print_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/read_h5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/read_mm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.786629 mattress-0.0.2/src/mattress/extern/tatami/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.810629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.810629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.814629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.814629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.814629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.818629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.818629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31532 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/tatami.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.786629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.822629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.826629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    42562 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.826629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62049 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.826629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.826629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/medians.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/sums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/variances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/convert_to_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.790629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.790629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.830629 mattress-0.0.2/src/mattress/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/include/Mattress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.834629 mattress-0.0.2/src/mattress/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/lib/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/lib/dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-26 05:46:24.000000 mattress-0.0.2/src/mattress/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.806629 mattress-0.0.2/src/mattress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 05:46:36.000000 mattress-0.0.2/src/mattress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:46:36.834629 mattress-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 05:46:24.000000 mattress-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 05:46:24.000000 mattress-0.0.2/tests/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-26 05:46:24.000000 mattress-0.0.2/tox.ini
```

### Comparing `mattress-0.0.1/.coveragerc` & `mattress-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/.github/workflows/pypi-test.yml` & `mattress-0.0.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/.gitignore` & `mattress-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/.readthedocs.yml` & `mattress-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/CONTRIBUTING.md` & `mattress-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/LICENSE.txt` & `mattress-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/PKG-INFO` & `mattress-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.1
+Version: 0.0.2
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.1/README.md` & `mattress-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/docs/Makefile` & `mattress-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/docs/conf.py` & `mattress-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/docs/index.md` & `mattress-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/docs/tutorial` & `mattress-0.0.2/docs/tutorial`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/.github/workflows/doxygenate.yaml` & `mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/.github/workflows/run-gallery.yaml` & `mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/.github/workflows/run-tests.yaml` & `mattress-0.0.2/src/mattress/extern/tatami/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/CMakeLists.txt` & `mattress-0.0.2/src/mattress/extern/tatami/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/LICENSE` & `mattress-0.0.2/src/mattress/extern/tatami/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/README.md` & `mattress-0.0.2/src/mattress/extern/tatami/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/docs/Doxyfile` & `mattress-0.0.2/src/mattress/extern/tatami/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/CMakeLists.txt` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/README.md` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/char2double.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/char2double.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/colsums.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/colsums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/parallel.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/print_vector.h` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/print_vector.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/read_h5.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/read_h5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/read_mm.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/read_mm.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/gallery/src/sparse_extractor.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/base/Extractor.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/base/Matrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/base/Options.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/Options.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/base/SparseRange.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/base/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/base/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/dense/DenseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/arith_utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/binary/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/boolean_utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/compare_utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/other/DelayedBind.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/other/DelayedCast.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/other/DelayedTranspose.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/primary_extraction.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/sparse/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/stats/medians.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/medians.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/stats/ranges.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/stats/sums.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/sums.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/stats/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/stats/variances.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/stats/variances.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubset.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/subset/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/subset/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/tatami.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/tatami.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/ArrayView.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/Oracles.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/SomeNumericArray.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/bind_intersection.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/convert_to_dense.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/convert_to_sparse.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/simulate_vector.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/temp_file_path.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/test_access_base.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/test_column_access.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/test_oracle_access.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/test_row_access.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/include/tatami_test/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami/include/tatami_test/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/CMakeLists.txt` & `mattress-0.0.2/src/mattress/extern/tatami/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/README.md` & `mattress-0.0.2/src/mattress/extern/tatami/tests/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/dense/DenseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/unary/math_helpers.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/isometric/utils.h` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/isometric/utils.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/other/DelayedBind.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/other/DelayedCast.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/other/DelayedTranspose.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/custom_parallel.h` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/medians.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/medians.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/parallelize.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/ranges.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/ranges.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/sums.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/sums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/stats/variances.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/stats/variances.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/subset/DelayedSubset.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/ArrayView.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/Oracles.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/SomeNumericArray.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/bind_intersection.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/convert_to_dense.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/convert_to_dense.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/convert_to_sparse.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/convert_to_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/process_consecutive_indices.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp` & `mattress-0.0.2/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/.github/workflows/doxygenate.yaml` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/.github/workflows/run-tests.yaml` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/CMakeLists.txt` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/LICENSE` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/README.md` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/docs/Doxyfile` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/CMakeLists.txt` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/src/custom_parallel.h` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp` & `mattress-0.0.2/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/setup.cfg` & `mattress-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	Cython
 	numpy>=1.22.4
 	scipy
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `mattress-0.0.1/setup.py` & `mattress-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,47 +2,36 @@
     Setup file for mattress.
     Use setup.cfg to configure your project.
 
     This file was generated with PyScaffold 4.5.
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
+import numpy
 from setuptools import setup
 from setuptools.extension import Extension
 
-from Cython.Build import cythonize
-import numpy
-
 if __name__ == "__main__":
     try:
         setup(
             use_scm_version={"version_scheme": "no-guess-dev"},
-            ext_modules=cythonize(
-                [
-                    Extension(
-                        "mattress.core",
-                        [ 
-                            "src/mattress/lib/bindings.pyx", 
-                            "src/mattress/lib/cpp/dense.cpp", 
-                            "src/mattress/lib/cpp/common.cpp"
-                        ],
-                        include_dirs=[
-                            "extern/tatami/include",
-                            "extern/tatami_hdf5/include",
-                            numpy.get_include(),
-                        ],
-                        language="c++",
-                        extra_compile_args=[
-                            "-std=c++17",
-                        ],
-                        extra_link_args=["-lz"],
-                    )
-                ],
-                compiler_directives={"language_level": "3"},
-            ),
+            ext_modules=[
+                Extension(
+                    "mattress.core",
+                    ["src/mattress/lib/dense.cpp", "src/mattress/lib/common.cpp"],
+                    include_dirs=[
+                        "src/mattress/extern/tatami/include",
+                        "src/mattress/include",
+                    ],
+                    language="c++",
+                    extra_compile_args=[
+                        "-std=c++17",
+                    ],
+                )
+            ],
         )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
```

### Comparing `mattress-0.0.1/src/mattress/__init__.py` & `mattress-0.0.2/src/mattress/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,8 +11,9 @@
     dist_name = __name__
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from .interface import tatamize as tatamize
+from .cpphelpers import includes
+from .interface import tatamize
```

### Comparing `mattress-0.0.1/src/mattress/utils.py` & `mattress-0.0.2/src/mattress/utils.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/src/mattress.egg-info/PKG-INFO` & `mattress-0.0.2/src/mattress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattress
-Version: 0.0.1
+Version: 0.0.2
 Summary: all your matrix representations belong here!
 Home-page: https://github.com/biocpy/mattress
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/mattress
 Platform: any
```

### Comparing `mattress-0.0.1/tests/test_dense.py` & `mattress-0.0.2/tests/test_dense.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.1/tox.ini` & `mattress-0.0.2/tox.ini`

 * *Files identical despite different names*

