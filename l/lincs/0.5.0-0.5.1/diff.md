# Comparing `tmp/lincs-0.5.0.tar.gz` & `tmp/lincs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.5.0.tar", last modified: Thu Jul  6 13:28:58 2023, max compression
+gzip compressed data, was "lincs-0.5.1.tar", last modified: Tue Jul 25 15:45:12 2023, max compression
```

## Comparing `lincs-0.5.0.tar` & `lincs-0.5.1.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-07-04 15:15:34.000000 lincs-0.5.0/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-07-04 15:15:34.000000 lincs-0.5.0/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      122 2023-07-04 15:15:34.000000 lincs-0.5.0/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)     5191 2023-07-06 13:28:58.275458 lincs-0.5.0/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)     4307 2023-07-06 13:28:53.000000 lincs-0.5.0/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1160 2023-07-05 16:05:46.000000 lincs-0.5.0/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    26193 2023-07-06 12:30:08.000000 lincs-0.5.0/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     5634 2023-07-05 07:34:25.000000 lincs-0.5.0/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      369 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    18418 2023-07-05 11:00:30.000000 lincs-0.5.0/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1189 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2735 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1058 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     8254 2023-07-06 06:53:40.000000 lincs-0.5.0/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3158 2023-07-05 07:33:27.000000 lincs-0.5.0/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4923 2023-07-06 06:53:14.000000 lincs-0.5.0/lincs/liblincs/io/problem.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2038 2023-07-06 07:12:12.000000 lincs-0.5.0/lincs/liblincs/io/problem.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1141 2023-07-06 05:20:37.000000 lincs-0.5.0/lincs/liblincs/io/validation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      583 2023-07-06 05:20:22.000000 lincs-0.5.0/lincs/liblincs/io/validation.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      187 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/
--rw-rw-r--   0 user      (1002) user      (1002)       60 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/exception.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      477 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/exception.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
--rw-rw-r--   0 user      (1002) user      (1002)      232 2023-07-04 15:51:24.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1072 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
--rw-rw-r--   0 user      (1002) user      (1002)     1525 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     9322 2023-07-06 07:12:50.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1628 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14371 2023-07-06 07:11:39.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-rw-r--   0 user      (1002) user      (1002)     1885 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4508 2023-07-04 15:49:29.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1226 2023-07-04 15:47:09.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     4107 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      838 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      901 2023-07-05 15:47:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      913 2023-07-06 08:36:25.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      211 2023-07-06 08:30:11.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      779 2023-07-05 15:44:27.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      295 2023-07-05 15:22:15.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      824 2023-07-05 15:44:18.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     7049 2023-07-06 12:20:11.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     4324 2023-07-06 12:17:33.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     9825 2023-07-05 07:35:23.000000 lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      591 2023-07-04 15:15:53.000000 lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    11212 2023-07-05 16:10:39.000000 lincs-0.5.0/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-07-05 16:00:50.000000 lincs-0.5.0/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    23013 2023-07-06 09:43:55.000000 lincs-0.5.0/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/linear-programming/
--rw-rw-r--   0 user      (1002) user      (1002)       57 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/alglib.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2731 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/alglib.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       55 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/glop.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1591 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/test.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      785 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/randomness-utils.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/sat/
--rw-rw-r--   0 user      (1002) user      (1002)       63 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/eval-max-sat.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1665 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/eval-max-sat.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       58 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/minisat.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1341 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/minisat.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2555 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/test.cpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/vendored/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.263458 lincs-0.5.0/lincs/liblincs/vendored/alglib/
--rwxrwxr-x   0 user      (1002) user      (1002)   615853 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    65139 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.h
--rwxrwxr-x   0 user      (1002) user      (1002)   322558 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    88614 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.h
--rwxrwxr-x   0 user      (1002) user      (1002)   493278 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   179632 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.h
--rwxrwxr-x   0 user      (1002) user      (1002)  1927587 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   438786 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.h
--rwxrwxr-x   0 user      (1002) user      (1002)    46242 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    10465 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.h
--rwxrwxr-x   0 user      (1002) user      (1002)   126902 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    27863 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.h
--rwxrwxr-x   0 user      (1002) user      (1002)   149125 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    33746 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.h
--rwxrwxr-x   0 user      (1002) user      (1002)  2674150 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   500164 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.h
--rwxrwxr-x   0 user      (1002) user      (1002)    76185 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)     7372 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.h
--rwxrwxr-x   0 user      (1002) user      (1002)    39356 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)     4704 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.h
--rwxrwxr-x   0 user      (1002) user      (1002)    23798 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)     4058 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.h
--rwxrwxr-x   0 user      (1002) user      (1002)  2288262 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   403192 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.h
--rwxrwxr-x   0 user      (1002) user      (1002)  3545102 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   608685 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.h
--rwxrwxr-x   0 user      (1002) user      (1002)   752491 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)   198547 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.h
--rwxrwxr-x   0 user      (1002) user      (1002)   339371 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    77195 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.h
--rwxrwxr-x   0 user      (1002) user      (1002)   612951 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.cpp
--rwxrwxr-x   0 user      (1002) user      (1002)    56614 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.h
--rwxrwxr-x   0 user      (1002) user      (1002)        4 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/stdafx.h
--rw-rw-r--   0 user      (1002) user      (1002)   321644 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/doctest.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/
--rw-rw-r--   0 user      (1002) user      (1002)    30623 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/
--rw-rw-r--   0 user      (1002) user      (1002)     3857 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
--rw-rw-r--   0 user      (1002) user      (1002)     2559 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
--rw-rw-r--   0 user      (1002) user      (1002)     3617 2023-07-03 05:21:10.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
--rw-rw-r--   0 user      (1002) user      (1002)     6040 2023-07-03 05:18:59.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h
--rw-rw-r--   0 user      (1002) user      (1002)      437 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/math.h
--rw-rw-r--   0 user      (1002) user      (1002)     8586 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     4176 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.h
--rw-rw-r--   0 user      (1002) user      (1002)     7315 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     5242 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/
--rw-rw-r--   0 user      (1002) user      (1002)     5770 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h
--rw-rw-r--   0 user      (1002) user      (1002)     3208 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h
--rw-rw-r--   0 user      (1002) user      (1002)     3293 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h
--rw-rw-r--   0 user      (1002) user      (1002)    68578 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc
--rw-rw-r--   0 user      (1002) user      (1002)    35867 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h
--rw-rw-r--   0 user      (1002) user      (1002)     4067 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h
--rw-rw-r--   0 user      (1002) user      (1002)    20417 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h
--rw-rw-r--   0 user      (1002) user      (1002)    17254 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/
--rw-rw-r--   0 user      (1002) user      (1002)     2814 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h
--rw-rw-r--   0 user      (1002) user      (1002)     4768 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h
--rw-rw-r--   0 user      (1002) user      (1002)      166 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Clone.h
--rw-rw-r--   0 user      (1002) user      (1002)     4772 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h
--rw-rw-r--   0 user      (1002) user      (1002)     1825 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h
--rw-rw-r--   0 user      (1002) user      (1002)     6949 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h
--rw-rw-r--   0 user      (1002) user      (1002)     3162 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h
--rw-rw-r--   0 user      (1002) user      (1002)     3276 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h
--rw-rw-r--   0 user      (1002) user      (1002)     5992 2023-07-03 05:19:40.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h
--rw-rw-r--   0 user      (1002) user      (1002)     7663 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h
--rw-rw-r--   0 user      (1002) user      (1002)     1948 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/
--rw-rw-r--   0 user      (1002) user      (1002)     9383 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc
--rw-rw-r--   0 user      (1002) user      (1002)     5078 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h
--rw-rw-r--   0 user      (1002) user      (1002)    24142 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc
--rw-rw-r--   0 user      (1002) user      (1002)     8631 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h
--rw-rw-r--   0 user      (1002) user      (1002)    20252 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc
--rw-rw-r--   0 user      (1002) user      (1002)     6800 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h
--rw-rw-r--   0 user      (1002) user      (1002)     6558 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc
--rw-rw-r--   0 user      (1002) user      (1002)     6099 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h
--rw-rw-r--   0 user      (1002) user      (1002)     3923 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc
--rw-rw-r--   0 user      (1002) user      (1002)     3805 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h
--rw-rw-r--   0 user      (1002) user      (1002)     7213 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc
--rw-rw-r--   0 user      (1002) user      (1002)     3471 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/
--rw-rw-r--   0 user      (1002) user      (1002)    25949 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc
--rw-rw-r--   0 user      (1002) user      (1002)    11769 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/
--rw-rw-r--   0 user      (1002) user      (1002)     3801 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc
--rw-rw-r--   0 user      (1002) user      (1002)    12150 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h
--rw-rw-r--   0 user      (1002) user      (1002)     5376 2023-07-03 05:03:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h
--rw-rw-r--   0 user      (1002) user      (1002)     3135 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc
--rw-rw-r--   0 user      (1002) user      (1002)     2707 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h
--rw-rw-r--   0 user      (1002) user      (1002)     1645 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1201 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
--rw-rw-r--   0 user      (1002) user      (1002)     8639 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/mcqd.h
--rw-rw-r--   0 user      (1002) user      (1002)     6332 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/monglucose41.h
--rw-rw-r--   0 user      (1002) user      (1002)      545 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1032 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
--rw-rw-r--   0 user      (1002) user      (1002)     3281 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
--rw-rw-r--   0 user      (1002) user      (1002)       58 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     5039 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
--rw-rw-r--   0 user      (1002) user      (1002)    39408 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/lov-e.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    62179 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/magic_enum.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/vendored/minisat/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/
--rw-rw-r--   0 user      (1002) user      (1002)    34998 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.cc
--rw-rw-r--   0 user      (1002) user      (1002)    24022 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.h
--rw-rw-r--   0 user      (1002) user      (1002)    17280 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/SolverTypes.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/
--rw-rw-r--   0 user      (1002) user      (1002)     2839 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alg.h
--rw-rw-r--   0 user      (1002) user      (1002)     4379 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alloc.h
--rw-rw-r--   0 user      (1002) user      (1002)     5344 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Heap.h
--rw-rw-r--   0 user      (1002) user      (1002)     4204 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntMap.h
--rw-rw-r--   0 user      (1002) user      (1002)     1763 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
--rw-rw-r--   0 user      (1002) user      (1002)     6682 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Map.h
--rw-rw-r--   0 user      (1002) user      (1002)     3001 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Queue.h
--rw-rw-r--   0 user      (1002) user      (1002)     2427 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Rnd.h
--rw-rw-r--   0 user      (1002) user      (1002)     3276 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Sort.h
--rw-rw-r--   0 user      (1002) user      (1002)     5588 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Vec.h
--rw-rw-r--   0 user      (1002) user      (1002)     1924 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/
--rw-rw-r--   0 user      (1002) user      (1002)    22244 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
--rw-rw-r--   0 user      (1002) user      (1002)    10816 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/
--rw-rw-r--   0 user      (1002) user      (1002)     3816 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.cc
--rw-rw-r--   0 user      (1002) user      (1002)    12153 2023-07-03 04:58:28.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.h
--rw-rw-r--   0 user      (1002) user      (1002)     4164 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/ParseUtils.h
--rw-rw-r--   0 user      (1002) user      (1002)     5254 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.cc
--rw-rw-r--   0 user      (1002) user      (1002)     3088 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.h
--rw-rw-r--   0 user      (1002) user      (1002)    57901 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/rapidcsv.h
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/valijson/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/
--rw-rw-r--   0 user      (1002) user      (1002)     9433 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    19320 2023-07-06 06:52:35.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      318 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraint_builder.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/
--rw-rw-r--   0 user      (1002) user      (1002)     1929 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    34401 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2030 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4649 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      856 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/exceptions.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/
--rw-rw-r--   0 user      (1002) user      (1002)    16614 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/adapter.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    25566 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2355 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      649 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/debug.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1525 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10088 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1694 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      339 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/optional.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       49 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1206 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/uri.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6144 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/schema.hpp
--rw-rw-r--   0 user      (1002) user      (1002)   102841 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/schema_parser.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     8346 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/subschema.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/
--rw-rw-r--   0 user      (1002) user      (1002)     1028 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1378 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2488 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_results.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    68300 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_visitor.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2250 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validator.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    25311 2023-07-06 12:21:51.000000 lincs-0.5.0/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)     1184 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)     5191 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)    10855 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-07-04 15:15:35.000000 lincs-0.5.0/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-07-06 13:28:58.275458 lincs-0.5.0/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     4185 2023-07-06 13:26:27.000000 lincs-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-25 15:45:05.000000 lincs-0.5.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-25 15:45:05.000000 lincs-0.5.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-25 15:45:05.000000 lincs-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-25 15:45:12.037627 lincs-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-07-25 15:45:05.000000 lincs-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.961627 lincs-0.5.1/lincs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26193 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/command_line_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.965627 lincs-0.5.1/lincs/liblincs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/classification.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/classification.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18418 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/generation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/alternatives.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/alternatives.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8247 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3158 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/model.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/problem.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/validation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io/validation.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/io.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.957627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9322 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.969627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7049 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11262 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/learning.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23065 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/liblincs_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/linear-programming/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/alglib.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/alglib.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/glop.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/glop.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/linear-programming/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/randomness-utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1736 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/randomness-utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.973627 lincs-0.5.1/lincs/liblincs/sat/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/minisat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/minisat.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/sat/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.977627 lincs-0.5.1/lincs/liblincs/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.005627 lincs-0.5.1/lincs/liblincs/vendored/alglib/
+-rwxr-xr-x   0 runner    (1001) docker     (122)   615853 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    65139 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   322558 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    88614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   493278 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   179632 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  1927587 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   438786 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    46242 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10465 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   126902 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    27863 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   149125 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    33746 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  2674150 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   500164 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    76185 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7372 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    39356 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4704 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23798 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4058 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  2288262 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   403192 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3545102 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   608685 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   752491 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)   198547 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   339371 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    77195 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)   612951 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    56614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)        4 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/alglib/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (122)   321644 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/doctest.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.009627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/
+-rw-r--r--   0 runner    (1001) docker     (122)    30725 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.009627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/
+-rw-r--r--   0 runner    (1001) docker     (122)     3857 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6040 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/math.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8586 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4176 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.957627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.013627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h
+-rw-r--r--   0 runner    (1001) docker     (122)    68578 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    35867 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h
+-rw-r--r--   0 runner    (1001) docker     (122)    20417 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.017627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Clone.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6949 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/
+-rw-r--r--   0 runner    (1001) docker     (122)     9383 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)    24142 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8631 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h
+-rw-r--r--   0 runner    (1001) docker     (122)    20252 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6800 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6558 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3471 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/
+-rw-r--r--   0 runner    (1001) docker     (122)    25949 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    11769 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.021627 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3801 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    12150 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5376 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8639 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/mcqd.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/monglucose41.h
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
+-rw-r--r--   0 runner    (1001) docker     (122)    39756 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/lov-e.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    62179 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/magic_enum.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.961627 lincs-0.5.1/lincs/liblincs/vendored/minisat/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.025627 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/
+-rw-r--r--   0 runner    (1001) docker     (122)    34973 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    24022 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17280 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/core/SolverTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.025627 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alg.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4379 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alloc.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Heap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntMap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6682 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Map.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Rnd.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Sort.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.029627 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/
+-rw-r--r--   0 runner    (1001) docker     (122)    22244 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10816 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.029627 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    12153 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4164 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/ParseUtils.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5266 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3088 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57901 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/rapidcsv.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19320 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraint_builder.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.033627 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34401 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/exceptions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)    16614 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    25566 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10088 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/uri.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/schema.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)   102841 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/schema_parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8346 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/subschema.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:12.037627 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    68300 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs/vendored/valijson/validator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    25311 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/liblincs_module_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-07-25 15:45:05.000000 lincs-0.5.1/lincs/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:45:11.965627 lincs-0.5.1/lincs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-25 15:45:11.000000 lincs-0.5.1/lincs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-25 15:45:05.000000 lincs-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 15:45:12.037627 lincs-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4706 2023-07-25 15:45:05.000000 lincs-0.5.1/setup.py
```

### Comparing `lincs-0.5.0/COPYING` & `lincs-0.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/COPYING.LESSER` & `lincs-0.5.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/PKG-INFO` & `lincs-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.5.0/README.rst` & `lincs-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/__init__.py` & `lincs-0.5.1/lincs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 # Classification
 from liblincs import classify_alternatives
 
 # Learning - weights-profiles-breed
 from liblincs import LearnMrsortByWeightsProfilesBreed
 from liblincs import InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion
 from liblincs import OptimizeWeightsUsingGlop, OptimizeWeightsUsingAlglib
-from liblincs import ImproveProfilesWithAccuracyHeuristicOnCpu, ImproveProfilesWithAccuracyHeuristicOnGpu
+from liblincs import ImproveProfilesWithAccuracyHeuristicOnCpu
+try:
+    from liblincs import ImproveProfilesWithAccuracyHeuristicOnGpu
+except ImportError:
+    pass
 from liblincs import ReinitializeLeastAccurate
 from liblincs import TerminateAtAccuracy, TerminateAfterSeconds, TerminateAfterIterations, TerminateWhenAny
 
 # Learning - SAT by coalitions
 from liblincs import LearnUcncsBySatByCoalitionsUsingMinisat, LearnUcncsBySatByCoalitionsUsingEvalmaxsat
 
 # @todo Accept learning and training set as Pandas DataFrame?
```

### Comparing `lincs-0.5.0/lincs/command_line_interface.py` & `lincs-0.5.1/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/classification.cpp` & `lincs-0.5.1/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/generation.cpp` & `lincs-0.5.1/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/generation.hpp` & `lincs-0.5.1/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/alternatives.cpp` & `lincs-0.5.1/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/alternatives.hpp` & `lincs-0.5.1/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/model.cpp` & `lincs-0.5.1/lincs/liblincs/io/model.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
   }
   out << YAML::EndSeq;
 
   os << '\n';
 }
 
 SufficientCoalitions load_sufficient_coalitions(const Problem& problem, const YAML::Node& node) {
-  switch (magic_enum::enum_cast<SufficientCoalitions::Kind>(node["kind"].as<std::string>()).value()) {
+  switch (*magic_enum::enum_cast<SufficientCoalitions::Kind>(node["kind"].as<std::string>())) {
     case SufficientCoalitions::Kind::weights:
       return SufficientCoalitions(SufficientCoalitions::weights, node["criterion_weights"].as<std::vector<float>>());
     case SufficientCoalitions::Kind::roots:
       return SufficientCoalitions(SufficientCoalitions::roots, problem.criteria.size(), node["upset_roots"].as<std::vector<std::vector<unsigned>>>());
   }
   __builtin_unreachable();
 }
```

### Comparing `lincs-0.5.0/lincs/liblincs/io/model.hpp` & `lincs-0.5.1/lincs/liblincs/io/model.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/problem.cpp` & `lincs-0.5.1/lincs/liblincs/io/problem.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     node["category_correlation"] = std::string(magic_enum::enum_name(criterion.category_correlation));
 
     return node;
   }
 
   static bool decode(const Node& node, lincs::Criterion& criterion) {
     criterion.name = node["name"].as<std::string>();
-    criterion.value_type = magic_enum::enum_cast<lincs::Criterion::ValueType>(node["value_type"].as<std::string>()).value();
-    criterion.category_correlation = magic_enum::enum_cast<lincs::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>()).value();
+    criterion.value_type = *magic_enum::enum_cast<lincs::Criterion::ValueType>(node["value_type"].as<std::string>());
+    criterion.category_correlation = *magic_enum::enum_cast<lincs::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>());
 
     return true;
   }
 };
 
 }  // namespace YAML
```

### Comparing `lincs-0.5.0/lincs/liblincs/io/problem.hpp` & `lincs-0.5.1/lincs/liblincs/io/problem.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/validation.cpp` & `lincs-0.5.1/lincs/liblincs/io/validation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/io/validation.hpp` & `lincs-0.5.1/lincs/liblincs/io/validation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -39,20 +39,24 @@
 
 template<>
 __inline__
 void Host::memset<lincs::Desirability>(const std::size_t n, const char v, lincs::Desirability* const p) {
   Host::force_memset<lincs::Desirability>(n, v, p);
 }
 
+#ifdef LINCS_HAS_NVCC
+
 template<>
 __inline__
 lincs::Desirability* Device::alloc<lincs::Desirability>(const std::size_t n) {
   return Device::force_alloc<lincs::Desirability>(n);
 }
 
 template<>
 __inline__
 void Device::memset<lincs::Desirability>(const std::size_t n, const char v, lincs::Desirability* const p) {
   Device::force_memset<lincs::Desirability>(n, v, p);
 }
 
+#endif  // LINCS_HAS_NVCC
+
 #endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
```

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 #include "../../mrsort-by-weights-profiles-breed.hpp"
 #include "accuracy-heuristic/desirability.hpp"
 
 
 namespace lincs {
 
+#ifdef LINCS_HAS_NVCC
+
 class ImproveProfilesWithAccuracyHeuristicOnGpu : public LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy {
  private:
   struct GpuLearningData {
     unsigned categories_count;
     unsigned criteria_count;
     unsigned learning_alternatives_count;
     Array2D<Device, float> learning_alternatives;
@@ -51,10 +53,12 @@
  private:
   LearningData& host_learning_data;
   GpuLearningData gpu_learning_data;
 
   static const unsigned destinations_count = 64;
 };
 
+#endif  // LINCS_HAS_NVCC
+
 }  // namespace lincs
 
 #endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
```

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp` & `lincs-0.5.1/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp` & `lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp` & `lincs-0.5.1/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/learning.cpp` & `lincs-0.5.1/lincs/liblincs/learning.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,16 @@
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
   check_exact_learning<Wrapper>(true);
 }
 
+#ifdef LINCS_HAS_NVCC
+
 TEST_CASE("GPU MR-Sort learning" * doctest::skip(forbid_gpu)) {
   class Wrapper {
    public:
     Wrapper(const Problem& problem, const Alternatives& learning_set) :
       learning_data(LearnMrsortByWeightsProfilesBreed::LearningData::make(
         problem, learning_set, LearnMrsortByWeightsProfilesBreed::default_models_count, 44
       )),
@@ -216,14 +218,16 @@
     TerminateAtAccuracy termination_strategy;
     LearnMrsortByWeightsProfilesBreed learning;
   };
 
   check_exact_learning<Wrapper>(true);
 }
 
+#endif  // LINCS_HAS_NVCC
+
 TEST_CASE("SAT by coalitions using Minisat learning") {
   check_exact_learning<LearnUcncsBySatByCoalitionsUsingMinisat>();
 }
 
 TEST_CASE("SAT by coalitions using EvalMaxSAT learning") {
   check_exact_learning<LearnUcncsBySatByCoalitionsUsingEvalmaxsat>();
 }
```

### Comparing `lincs-0.5.0/lincs/liblincs/learning.hpp` & `lincs-0.5.1/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/liblincs_module.cpp` & `lincs-0.5.1/lincs/liblincs/liblincs_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -453,24 +453,26 @@
   >(
     "ImproveProfilesWithAccuracyHeuristicOnCpu",
     bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
     .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles)
   ;
 
+  #ifdef LINCS_HAS_NVCC
   bp::class_<
     lincs::ImproveProfilesWithAccuracyHeuristicOnGpu,
     bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy>,
     boost::noncopyable
   >(
     "ImproveProfilesWithAccuracyHeuristicOnGpu",
     bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
     .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles)
   ;
+  #endif  // LINCS_HAS_NVCC
 
   struct BreedingStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy> {
     void breed() override { this->get_override("breed")(); }
   };
 
   learn_wbp_class.attr("BreedingStrategy") = bp::class_<BreedingStrategyWrap, boost::noncopyable>("BreedingStrategy")
     .def("breed", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy::breed))
```

### Comparing `lincs-0.5.0/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-0.5.1/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/linear-programming/glop.hpp` & `lincs-0.5.1/lincs/liblincs/linear-programming/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/linear-programming/test.cpp` & `lincs-0.5.1/lincs/liblincs/linear-programming/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/randomness-utils.cpp` & `lincs-0.5.1/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/randomness-utils.hpp` & `lincs-0.5.1/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/sat/eval-max-sat.hpp` & `lincs-0.5.1/lincs/liblincs/sat/eval-max-sat.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/sat/minisat.hpp` & `lincs-0.5.1/lincs/liblincs/sat/minisat.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/sat/test.cpp` & `lincs-0.5.1/lincs/liblincs/sat/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibinternal.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/alglibmisc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/ap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/dataanalysis.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/diffequations.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/fasttransforms.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/integration.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/interpolation.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_avx2.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_fma.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/kernels_sse2.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/linalg.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/optimization.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/solvers.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/specialfunctions.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.h` & `lincs-0.5.1/lincs/liblincs/vendored/alglib/statistics.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/doctest.h` & `lincs-0.5.1/lincs/liblincs/vendored/doctest.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h`

 * *Files 1% similar despite different names*

```diff
@@ -515,14 +515,16 @@
         }
     }
 
 
 public:
 
     bool solve() {
+        std::mt19937 rng((std::random_device()()));
+
         // CONFIG
         unsigned int nbSecondSolveMin = 20;
         unsigned int timeOutForSecondSolve = 60;
         // END CONFIG
         
         // Reinit CL
         CL_ConflictToMinimize.clear();
@@ -639,15 +641,15 @@
                             break;
                         nbSecondSolve++;
                         if(chronoForBreak.tacSec() > timeOutForSecondSolve)
                             break;
                         if(nbSecondSolve > 10000)
                             break;
 
-                        std::random_shuffle(forSolve.begin(), forSolve.end());
+                        std::shuffle(forSolve.begin(), forSolve.end(), rng);
 
                         bool res = solver->solve(forSolve);
                         assert(!res);
 
                         if( bestUnminimizedConflict.size() > solver->sizeConflict() ) {
                             bestUnminimizedConflict = solver->getConflict();
                         }
@@ -807,14 +809,16 @@
                 result++;
         return result;
     }
 
 private:
 
     bool fullMinimize(VirtualSAT* solverForMinimize, std::set<int> &conflict, std::vector<int> &uselessLit, long timeRef) {
+        std::mt19937 rng((std::random_device()()));
+
         MaLib::Chrono chrono;
         bool minimum = true;
 
         int B = 1000;
         //int B = 10000;
 
         if(timeRef > 60000000) {
@@ -906,15 +910,15 @@
 
             if((i>=2) // Au moins 3 loops
                     && (timeRef*(1+numberMinimizeThreadRunning) <= chrono.tac())) {
                 MonPrint("\t\t\t\t\tfullMinimize: TimeOut after ", (i+1), " loops");
                 break;
             }
 
-            std::random_shuffle(removable.begin(), removable.end());
+            std::shuffle(removable.begin(), removable.end(), rng);
         }
 
         for(auto lit: uselessLit) {
             conflict.erase(lit);
         }
 
         return minimum;
```

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/card_oe.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/cardincremental.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/mcqd.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/mcqd.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/monglucose41.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/monglucose41.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualcard.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h` & `lincs-0.5.1/lincs/liblincs/vendored/eval-max-sat/virtualsat.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/lov-e.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/lov-e.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 // Copyright 2022 Laurent Cabaret
 
 // Documentation and license information for this file are available at https://github.com/jacquev6/lov-e-cuda
 
 #ifndef LOV_E_HPP_
 #define LOV_E_HPP_
 
+#ifdef LINCS_HAS_NVCC
 #include <cuda_runtime.h>
+#endif  // LINCS_HAS_NVCC
 
 #include <cassert>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
 #include <exception>
 #include <type_traits>
@@ -23,14 +25,16 @@
 #endif
 
 
 /*                          *
  * Error checking utilities *
  *                          */
 
+#ifdef LINCS_HAS_NVCC
+
 struct CudaError : public std::exception {
   CudaError(const char* const file_, const unsigned line_, const cudaError_t error_) :
       file(file_), line(line_), error(error_) {
     std::snprintf(
       _what, sizeof(_what),
       "CUDA ERROR, detected at %s:%i: code %i=%s: %s",
       file, line, static_cast<unsigned>(error), cudaGetErrorName(error), cudaGetErrorString(error));
@@ -82,14 +86,16 @@
 
 #define check_cuda_error(e) check_cuda_error_(e, __FILE__, __LINE__)
 
 #define check_last_cuda_error_no_sync() check_last_cuda_error_no_sync_(__FILE__, __LINE__)
 #define check_last_cuda_error_sync_stream(stream) check_last_cuda_error_sync_stream_(stream, __FILE__, __LINE__)
 #define check_last_cuda_error_sync_device() check_last_cuda_error_sync_device_(__FILE__, __LINE__)
 
+#endif  // LINCS_HAS_NVCC
+
 /*                   *
  * Memory management *
  *                   */
 
 
 class Anywhere {};
 
@@ -159,14 +165,16 @@
       } else {
         std::free(p);
       }
     #endif
   }
 };
 
+#ifdef LINCS_HAS_NVCC
+
 class Device {
  public:
   static const bool can_be_allocated_on_device = true;
 
  private:
   template<typename T>
   static void force_memset(const std::size_t n, const char v, T* const p) {
@@ -222,14 +230,16 @@
       return;
     } else {
       check_cuda_error(cudaFree(p));
     }
   }
 };
 
+#endif  // LINCS_HAS_NVCC
+
 template<typename WhereFrom>
 struct From {
   template<typename WhereTo>
   struct To {
     template<typename T>
     static void copy(const std::size_t n, const T* const src, typename std::remove_const<T>::type* const dst);
 
@@ -250,14 +260,16 @@
   if (n == 0) {
     return;
   } else {
     std::memcpy(dst, src, n * sizeof(T));
   }
 }
 
+#ifdef LINCS_HAS_NVCC
+
 template<> template<> template<typename T>
 void From<Host>::To<Device>::copy(
     const std::size_t n,
     const T* const src,
     typename std::remove_const<T>::type* const dst) {
   if (n == 0) {
     return;
@@ -286,14 +298,16 @@
   if (n == 0) {
     return;
   } else {
     check_cuda_error(cudaMemcpy(dst, src, n * sizeof(T), cudaMemcpyDeviceToHost));
   }
 }
 
+#endif  // LINCS_HAS_NVCC
+
 /*                       *
  * Arrays and ArrayViews *
  *                       */
 
 // The 'ArrayView?D' classes have "non-owning pointer" semantics, so they follow the
 // [Rule of Zero](http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#Rc-zero).
 
@@ -427,14 +441,16 @@
  private:
   std::size_t _s0;
   T* _data;
 
   friend class Array1D<Host, typename std::remove_const<T>::type>;
 };
 
+#ifdef LINCS_HAS_NVCC
+
 template<typename T>
 class ArrayView1D<Device, T> {
  public:
   // Constructor
   HOST_DEVICE_DECORATORS
   ArrayView1D(std::size_t s0, T* data) :
     _s0(s0), _data(data) {}
@@ -493,14 +509,16 @@
  private:
   std::size_t _s0;
   T* _data;
 
   friend class Array1D<Device, typename std::remove_const<T>::type>;
 };
 
+#endif  // LINCS_HAS_NVCC
+
 template<typename WhereFrom, typename WhereTo, typename T>
 void copy(ArrayView1D<WhereFrom, T> src, ArrayView1D<WhereTo, typename std::remove_const<T>::type> dst) {
   assert(dst.s0() == src.s0());
 
   From<WhereFrom>::template To<WhereTo>::template copy(
     src.s0(), src.data(), dst.data());
 }
@@ -590,22 +608,26 @@
 template<typename WhereTo>
 Array1D<WhereTo, typename std::remove_const<T>::type> ArrayView1D<Host, T>::clone_to() const {
   Array1D<WhereTo, typename std::remove_const<T>::type> dst(this->s0(), uninitialized);
   copy(*this, ref(dst));  // NOLINT(build/include_what_you_use)
   return dst;
 }
 
+#ifdef LINCS_HAS_NVCC
+
 template<typename T>
 template<typename WhereTo>
 Array1D<WhereTo, typename std::remove_const<T>::type> ArrayView1D<Device, T>::clone_to() const {
   Array1D<WhereTo, typename std::remove_const<T>::type> dst(this->s0(), uninitialized);
   copy(*this, ref(dst));  // NOLINT(build/include_what_you_use)
   return dst;
 }
 
+#endif  // LINCS_HAS_NVCC
+
 template<typename Where, typename T> class Array2D;
 
 template<typename Where, typename T>
 class ArrayView2D {
  public:
   // Constructor
   HOST_DEVICE_DECORATORS
@@ -1331,14 +1353,16 @@
 // END GENERATED SECTION: arrays-and-array-views
 
 
 /*                          *
  * Grid and block utilities *
  *                          */
 
+#ifdef LINCS_HAS_NVCC
+
 struct Grid {
   const dim3 gridDim;
   const dim3 blockDim;
 };
 
 #define LOVE_CONFIG(grid) grid.gridDim, grid.blockDim
 
@@ -1449,10 +1473,12 @@
     return blockIdx.z * BLOCKDIM_Z + threadIdx.z;
   }
 #endif  // __NVCC__
 
   static constexpr dim3 blockDim = {BLOCKDIM_X, BLOCKDIM_Y, BLOCKDIM_Z};
 };
 
+#endif  // LINCS_HAS_NVCC
+
 #undef HOST_DEVICE_DECORATORS
 
 #endif  // LOV_E_HPP_
```

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/magic_enum.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/magic_enum.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.cc` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.cc`

 * *Files 0% similar despite different names*

```diff
@@ -988,19 +988,19 @@
 }
 
 
 void Solver::printStats() const
 {
     double cpu_time = cpuTime();
     double mem_used = memUsedPeak();
-    printf("restarts              : %"PRIu64"\n", starts);
-    printf("conflicts             : %-12"PRIu64"   (%.0f /sec)\n", conflicts   , conflicts   /cpu_time);
-    printf("decisions             : %-12"PRIu64"   (%4.2f %% random) (%.0f /sec)\n", decisions, (float)rnd_decisions*100 / (float)decisions, decisions   /cpu_time);
-    printf("propagations          : %-12"PRIu64"   (%.0f /sec)\n", propagations, propagations/cpu_time);
-    printf("conflict literals     : %-12"PRIu64"   (%4.2f %% deleted)\n", tot_literals, (max_literals - tot_literals)*100 / (double)max_literals);
+    printf("restarts              : %" "\n", starts);
+    printf("conflicts             : %-12" "   (%.0f /sec)\n", conflicts   , conflicts   /cpu_time);
+    printf("decisions             : %-12" "   (%4.2f %% random) (%.0f /sec)\n", decisions, (float)rnd_decisions*100 / (float)decisions, decisions   /cpu_time);
+    printf("propagations          : %-12" "   (%.0f /sec)\n", propagations, propagations/cpu_time);
+    printf("conflict literals     : %-12" "   (%4.2f %% deleted)\n", tot_literals, (max_literals - tot_literals)*100 / (double)max_literals);
     if (mem_used != 0) printf("Memory used           : %.2f MB\n", mem_used);
     printf("CPU time              : %g s\n", cpu_time);
 }
 
 
 //=================================================================================================
 // Garbage Collection methods:
```

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/core/Solver.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/core/SolverTypes.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/core/SolverTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alg.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alg.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alloc.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Alloc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Heap.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Heap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntMap.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntMap.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/IntTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Map.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Map.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Queue.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Queue.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Rnd.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Rnd.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Sort.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Sort.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Vec.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/Vec.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/mtl/XAlloc.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/simp/SimpSolver.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.cc` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.cc`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/Options.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/ParseUtils.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/ParseUtils.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.cc` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.cc`

 * *Files 2% similar despite different names*

```diff
@@ -73,29 +73,29 @@
 
 #elif defined(__FreeBSD__) || defined(__FreeBSD_kernel__) || defined(__gnu_hurd__)
 
 double Minisat::memUsed() {
     struct rusage ru;
     getrusage(RUSAGE_SELF, &ru);
     return (double)ru.ru_maxrss / 1024; }
-double Minisat::memUsedPeak() { return memUsed(); }
+double Minisat::memUsedPeak(bool) { return memUsed(); }
 
 
 #elif defined(__APPLE__)
 #include <malloc/malloc.h>
 
 double Minisat::memUsed() {
     malloc_statistics_t t;
     malloc_zone_statistics(NULL, &t);
     return (double)t.max_size_in_use / (1024*1024); }
-double Minisat::memUsedPeak() { return memUsed(); }
+double Minisat::memUsedPeak(bool) { return memUsed(); }
 
 #else
 double Minisat::memUsed()     { return 0; }
-double Minisat::memUsedPeak() { return 0; }
+double Minisat::memUsedPeak(bool) { return 0; }
 #endif
 
 
 void Minisat::setX86FPUPrecision()
 {
 #if defined(__linux__) && defined(_FPU_EXTENDED) && defined(_FPU_DOUBLE) && defined(_FPU_GETCW)
     // Only correct FPU precision on Linux architectures that needs and supports it:
```

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.h` & `lincs-0.5.1/lincs/liblincs/vendored/minisat/utils/System.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/rapidcsv.h` & `lincs-0.5.1/lincs/liblincs/vendored/rapidcsv.h`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/exceptions.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/adapter.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/debug.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/debug.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/json_reference.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/uri.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/internal/uri.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/schema.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/schema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/schema_parser.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/schema_parser.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/subschema.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/subschema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/file_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_results.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_results.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_visitor.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/validation_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs/vendored/valijson/validator.hpp` & `lincs-0.5.1/lincs/liblincs/vendored/valijson/validator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/liblincs_module_tests.py` & `lincs-0.5.1/lincs/liblincs_module_tests.py`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs/visualization.py` & `lincs-0.5.1/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/lincs.egg-info/PKG-INFO` & `lincs-0.5.1/lincs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.1/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.5.0/lincs.egg-info/SOURCES.txt` & `lincs-0.5.1/lincs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lincs-0.5.0/setup.py` & `lincs-0.5.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # Copyright 2023 Vincent Jacques
 
 import glob
 import itertools
 import os
+import shutil
 import sys
 import setuptools
 import setuptools.command.build_ext
 
 
-version = "0.5.0"
+version = "0.5.1"
 
 with open("README.rst") as f:
     long_description = f.read()
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
 for lang in ["yaml", "shell", "text", "diff"]:
     long_description = long_description.replace(f".. highlight:: {lang}", "")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
+has_nvcc = os.environ.get("LINCS_DEV_FORBID_NVCC", "false") != "true" and shutil.which("nvcc") is not None
+
 # Method for building an extension with CUDA code extracted from https://stackoverflow.com/a/13300714/905845
 # @todo Consider using scikit-build:
 # it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
 # Note that pybind11 comes with an example of building using scikit-build.
 # (see also https://www.benjack.io/hybrid-python/c-packages-revisited/)
 def customize_compiler_for_nvcc(self):
     self.src_extensions.append(".cu")
@@ -48,40 +51,52 @@
 
 
 class custom_build_ext(setuptools.command.build_ext.build_ext):
     def build_extensions(self):
         customize_compiler_for_nvcc(self.compiler)
         setuptools.command.build_ext.build_ext.build_extensions(self)
 
+optional_libraries = []
+
+if has_nvcc:
+    optional_libraries.append("cudart")
+
+if sys.platform == "linux":
+    omp_compile_args = ["-fopenmp"]
+    omp_link_args = ["-fopenmp"]
+    # Weirdly required because of BoostPython:
+    optional_libraries.append(f"python{sys.version_info.major}.{sys.version_info.minor}{'m' if sys.hexversion < 0x03080000 else ''}")
+elif sys.platform == "darwin":
+    omp_compile_args = ["-Xclang", "-fopenmp"]
+    omp_link_args = ["-lomp"]
+else:
+    assert False, f"Unsupported platform: {sys.platform}"
 
 liblincs = setuptools.Extension(
     "liblincs",
     sources=list(itertools.chain.from_iterable(
         glob.glob(f"lincs/liblincs/**/*.{ext}", recursive=True)
-        for ext in ["c", "cc", "cpp", "cu"]
+        for ext in ["c", "cc", "cpp"] + (["cu"] if has_nvcc else [])
     )),
     libraries=[
         f"boost_python{sys.version_info.major}{sys.version_info.minor}",
         "ortools",
-        f"python{sys.version_info.major}.{sys.version_info.minor}{'m' if sys.hexversion < 0x03080000 else ''}",  # Weirdly required because of BoostPython
         "yaml-cpp",
-        "cudart",
-    ],
-    define_macros=[("DOCTEST_CONFIG_DISABLE", None)],
-    # @todo Support building without CUDA (required on macOS)
+    ] + optional_libraries,
+    define_macros=[("DOCTEST_CONFIG_DISABLE", None)] + ([("LINCS_HAS_NVCC", None)] if has_nvcc else []),
     # @todo Support several versions of CUDA?
     include_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/include"],
     library_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/lib"],
     # Non-standard: the dict is accessed in `customize_compiler_for_nvcc`
     # to get the standard form for `extra_compile_args`
     extra_compile_args={
-        "gcc": ["-std=c++17", "-fopenmp", "-Werror=switch"],
+        "gcc": ["-std=c++17", "-Werror=switch"] + omp_compile_args,
         "nvcc": ["-std=c++17", "-Xcompiler", "-fopenmp,-fPIC,-Werror=switch"],
     },
-    extra_link_args=["-fopenmp"],
+    extra_link_args=omp_link_args,
 )
 
 setuptools.setup(
     name="lincs",
     version=version,
     description="Learn and Infer Non Compensatory Sortings",
     license="LGPLv3",
```

