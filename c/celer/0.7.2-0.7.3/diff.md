# Comparing `tmp/celer-0.7.2.tar.gz` & `tmp/celer-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celer-0.7.2.tar", last modified: Wed Jul 20 11:08:14 2022, max compression
+gzip compressed data, was "celer-0.7.3.tar", last modified: Wed Jul 26 15:28:49 2023, max compression
```

## Comparing `celer-0.7.2.tar` & `celer-0.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.356938 celer-0.7.2/
--rw-rw-rw-   0        0        0     1539 2022-07-20 11:06:20.000000 celer-0.7.2/LICENSE
--rw-rw-rw-   0        0        0      562 2022-07-20 11:06:20.000000 celer-0.7.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6142 2022-07-20 11:08:14.356938 celer-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     4711 2022-07-20 11:06:20.000000 celer-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.345937 celer-0.7.2/celer/
--rw-rw-rw-   0        0        0    21600 2022-07-20 11:06:20.000000 celer-0.7.2/celer/PN_logreg.pyx
--rw-rw-rw-   0        0        0      367 2022-07-20 11:06:20.000000 celer-0.7.2/celer/__init__.py
--rw-rw-rw-   0        0        0     2018 2022-07-20 11:06:20.000000 celer-0.7.2/celer/cython_utils.pxd
--rw-rw-rw-   0        0        0    15508 2022-07-20 11:06:20.000000 celer-0.7.2/celer/cython_utils.pyx
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.351937 celer-0.7.2/celer/datasets/
--rw-rw-rw-   0        0        0      233 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/__init__.py
--rw-rw-rw-   0        0        0     2936 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/climate.py
--rw-rw-rw-   0        0        0     1125 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/libsvm.py
--rw-rw-rw-   0        0        0     1460 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/ml_uci.py
--rw-rw-rw-   0        0        0     3208 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/simulated.py
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.351937 celer-0.7.2/celer/datasets/tests/
--rw-rw-rw-   0        0        0      584 2022-07-20 11:06:20.000000 celer-0.7.2/celer/datasets/tests/test_datasets.py
--rw-rw-rw-   0        0        0    45470 2022-07-20 11:06:20.000000 celer-0.7.2/celer/dropin_sklearn.py
--rw-rw-rw-   0        0        0    17123 2022-07-20 11:06:20.000000 celer-0.7.2/celer/group_fast.pyx
--rw-rw-rw-   0        0        0    19096 2022-07-20 11:06:20.000000 celer-0.7.2/celer/homotopy.py
--rw-rw-rw-   0        0        0    16152 2022-07-20 11:06:20.000000 celer-0.7.2/celer/lasso_fast.pyx
--rw-rw-rw-   0        0        0    13826 2022-07-20 11:06:20.000000 celer-0.7.2/celer/multitask_fast.pyx
--rw-rw-rw-   0        0        0      987 2022-07-20 11:06:20.000000 celer-0.7.2/celer/plot_utils.py
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.355937 celer-0.7.2/celer/tests/
--rw-rw-rw-   0        0        0     7903 2022-07-20 11:06:20.000000 celer-0.7.2/celer/tests/test_docstring_parameters.py
--rw-rw-rw-   0        0        0     5977 2022-07-20 11:06:20.000000 celer-0.7.2/celer/tests/test_enet.py
--rw-rw-rw-   0        0        0     9028 2022-07-20 11:06:20.000000 celer-0.7.2/celer/tests/test_lasso.py
--rw-rw-rw-   0        0        0     2853 2022-07-20 11:06:20.000000 celer-0.7.2/celer/tests/test_logreg.py
--rw-rw-rw-   0        0        0     9610 2022-07-20 11:06:20.000000 celer-0.7.2/celer/tests/test_mtl.py
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.356938 celer-0.7.2/celer/utils/
--rw-rw-rw-   0        0        0        0 2022-07-20 11:06:20.000000 celer-0.7.2/celer/utils/__init__.py
--rw-rw-rw-   0        0        0      656 2022-07-20 11:06:20.000000 celer-0.7.2/celer/utils/testing.py
-drwxrwxrwx   0        0        0        0 2022-07-20 11:08:14.348937 celer-0.7.2/celer.egg-info/
--rw-rw-rw-   0        0        0     6142 2022-07-20 11:08:14.000000 celer-0.7.2/celer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-07-20 11:08:14.000000 celer-0.7.2/celer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-20 11:08:14.000000 celer-0.7.2/celer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2022-07-20 11:08:14.000000 celer-0.7.2/celer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-20 11:08:14.000000 celer-0.7.2/celer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      129 2022-07-20 11:06:20.000000 celer-0.7.2/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-07-20 11:08:14.357937 celer-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     2833 2022-07-20 11:06:20.000000 celer-0.7.2/setup.py
--rw-rw-rw-   0        0        0      933 2022-07-20 11:06:20.000000 celer-0.7.2/whats_new.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/
+-rw-rw-rw-   0        0        0     1539 2023-07-26 15:25:08.000000 celer-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0      536 2023-07-26 15:25:08.000000 celer-0.7.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5289 2023-07-26 15:28:49.878876 celer-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4862 2023-07-26 15:25:08.000000 celer-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer/
+-rw-rw-rw-   0        0        0    21691 2023-07-26 15:25:08.000000 celer-0.7.3/celer/PN_logreg.pyx
+-rw-rw-rw-   0        0        0      367 2023-07-26 15:25:08.000000 celer-0.7.3/celer/__init__.py
+-rw-rw-rw-   0        0        0     2018 2023-07-26 15:25:08.000000 celer-0.7.3/celer/cython_utils.pxd
+-rw-rw-rw-   0        0        0    15541 2023-07-26 15:25:08.000000 celer-0.7.3/celer/cython_utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer/datasets/
+-rw-rw-rw-   0        0        0      233 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2936 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/climate.py
+-rw-rw-rw-   0        0        0     1125 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/libsvm.py
+-rw-rw-rw-   0        0        0     1460 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/ml_uci.py
+-rw-rw-rw-   0        0        0     3208 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/simulated.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer/datasets/tests/
+-rw-rw-rw-   0        0        0      584 2023-07-26 15:25:08.000000 celer-0.7.3/celer/datasets/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    45470 2023-07-26 15:25:08.000000 celer-0.7.3/celer/dropin_sklearn.py
+-rw-rw-rw-   0        0        0    17389 2023-07-26 15:25:08.000000 celer-0.7.3/celer/group_fast.pyx
+-rw-rw-rw-   0        0        0    19122 2023-07-26 15:25:08.000000 celer-0.7.3/celer/homotopy.py
+-rw-rw-rw-   0        0        0    16508 2023-07-26 15:25:08.000000 celer-0.7.3/celer/lasso_fast.pyx
+-rw-rw-rw-   0        0        0    14061 2023-07-26 15:25:08.000000 celer-0.7.3/celer/multitask_fast.pyx
+-rw-rw-rw-   0        0        0      987 2023-07-26 15:25:08.000000 celer-0.7.3/celer/plot_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer/tests/
+-rw-rw-rw-   0        0        0     7903 2023-07-26 15:25:08.000000 celer-0.7.3/celer/tests/test_docstring_parameters.py
+-rw-rw-rw-   0        0        0     5977 2023-07-26 15:25:08.000000 celer-0.7.3/celer/tests/test_enet.py
+-rw-rw-rw-   0        0        0     9472 2023-07-26 15:25:08.000000 celer-0.7.3/celer/tests/test_lasso.py
+-rw-rw-rw-   0        0        0     2853 2023-07-26 15:25:08.000000 celer-0.7.3/celer/tests/test_logreg.py
+-rw-rw-rw-   0        0        0     9610 2023-07-26 15:25:08.000000 celer-0.7.3/celer/tests/test_mtl.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:25:08.000000 celer-0.7.3/celer/utils/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-07-26 15:25:08.000000 celer-0.7.3/celer/utils/testing.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:28:49.878876 celer-0.7.3/celer.egg-info/
+-rw-rw-rw-   0        0        0     5289 2023-07-26 15:28:49.000000 celer-0.7.3/celer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-07-26 15:28:49.000000 celer-0.7.3/celer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:28:49.000000 celer-0.7.3/celer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-26 15:28:49.000000 celer-0.7.3/celer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 15:28:49.000000 celer-0.7.3/celer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      923 2023-07-26 15:25:08.000000 celer-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-26 15:28:49.878876 celer-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2023-07-26 15:25:08.000000 celer-0.7.3/setup.py
+-rw-rw-rw-   0        0        0      933 2023-07-26 15:25:08.000000 celer-0.7.3/whats_new.rst
```

### Comparing `celer-0.7.2/LICENSE` & `celer-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/MANIFEST.in` & `celer-0.7.3/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 include *.rst
 include *.md
 include *.in
 include LICENSE
 include celer/__init__.py
-include requirements.txt
 
 recursive-include examples *.py
 recursive-include examples *.txt
 recursive-include celer *.py
 recursive-include celer *.pyx
 recursive-include celer *.pxd
```

### Comparing `celer-0.7.2/README.md` & `celer-0.7.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: celer
+Version: 0.7.3
+Summary: A fast algorithm with dual extrapolation for sparse problems
+Author-email: Mathurin Massias <mathurin.massias@gmail.com>
+License: BSD (3-clause)
+Project-URL: documentation, https://mathurinm.github.io/celer/
+Project-URL: repository, https://github.com/mathurinm/celer.git
+Description-Content-Type: text/markdown
+Provides-Extra: doc
+License-File: LICENSE
+
 # celer
 
 ![build](https://github.com/mathurinm/celer/workflows/build/badge.svg)
 ![coverage](https://codecov.io/gh/mathurinm/celer/branch/main/graphs/badge.svg?branch=main)
 ![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)
-![Downloads](https://pepy.tech/badge/celer/month)
-![PyPI version](https://badge.fury.io/py/celer.svg)
+[![Downloads](https://static.pepy.tech/badge/celer)](https://pepy.tech/project/celer)
+[![Downloads](https://pepy.tech/badge/celer/month)](https://pepy.tech/project/celer)
+[![PyPI version](https://badge.fury.io/py/celer.svg)](https://pypi.org/project/celer)
 
 
 ``celer`` is a Python package that solves Lasso-like problems and provides estimators that follow the ``scikit-learn`` API. Thanks to a tailored implementation, ``celer`` provides a fast solver that tackles large-scale datasets with millions of features **up to 100 times faster than ``scikit-learn``**.
 
 Currently, the package handles the following problems:
 
 
@@ -21,15 +34,15 @@
 | Sparse Logistic regression    | ✕               | ✕
 
 
 
 ## Why ``celer``?
 
 ``celer`` is specially designed to handle Lasso-like problems which makes it a fast solver of such problems.
-``celer`` comes particularly with
+In particular it comes with tools such as:
 
 - automated parallel cross-validation
 - support of sparse and dense data
 - optional feature centering and normalization
 - unpenalized intercept fitting
 
 ``celer`` also provides easy-to-use estimators as it is designed under the ``scikit-learn`` API.
@@ -86,15 +99,15 @@
 pip install -e .
 ```
 
 3. To run the gallery examples and build the documentation, run the followings
 
 ```shell
 cd doc
-pip install -r doc-requirements.txt
+pip install -e .[doc]
 make html
 ```
 
 
 ## Cite
 
 ``celer`` is licensed under the [BSD 3-Clause](https://github.com/mathurinm/celer/blob/main/LICENSE). Hence, you are free to use it.
@@ -123,8 +136,8 @@
 }
 ```
 
 ## Further links
 
 - https://mathurinm.github.io/celer/
 - https://arxiv.org/abs/1802.07481
-- https://arxiv.org/abs/1907.05830
+- https://arxiv.org/abs/1907.05830
```

### Comparing `celer-0.7.2/celer/PN_logreg.pyx` & `celer-0.7.3/celer/PN_logreg.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     cdef int n_samples = y.shape[0]
     cdef int n_features = w.shape[0]
     # scale tol for when problem has large or small p_obj
     tol *= n_samples * np.log(2)
 
     cdef int t = 0
     cdef int i, j, k
-    cdef floating p_obj, d_obj, norm_Xtheta, norm_Xtheta_acc, tmp
+    cdef floating p_obj, d_obj, dnorm_XTtheta, theta_scaling
     cdef floating gap = -1  # initialized for the warning if max_iter=0
     cdef int info_dposv
     cdef int ws_size
     cdef floating eps_inner = 0.1
     cdef floating growth = 2.
 
 
@@ -106,21 +106,21 @@
     cdef bint positive = 0
 
     for t in range(max_iter):
         p_obj = primal(LOGREG, alpha, l1_ratio, Xw, y, w, weights_pen)
 
         # theta = y * sigmoid(-y * Xw)
         create_dual_pt(LOGREG, n_samples, &theta[0], &Xw[0], &y[0])
-        norm_Xtheta = dnorm_enet(
+        dnorm_XTtheta = dnorm_enet(
             is_sparse, theta, w, X, X_data, X_indices, X_indptr,
             screened, X_mean, weights_pen, center, positive, alpha, l1_ratio)
 
-        if norm_Xtheta > alpha:
-            tmp = alpha / norm_Xtheta
-            fscal(&n_samples, &tmp, &theta[0], &inc)
+        if dnorm_XTtheta > alpha:
+            theta_scaling = alpha / dnorm_XTtheta
+            fscal(&n_samples, &theta_scaling, &theta[0], &inc)
 
         d_obj = dual(LOGREG, n_samples, alpha, l1_ratio, 0., norm_w2, &theta[0], &y[0])
         gap = p_obj - d_obj
 
         if t != 0 and use_accel:
             # do some epochs of CD to create an extrapolated dual point
             for k in range(K):
@@ -165,21 +165,21 @@
             for i in range(n_samples):
                 theta_acc[i] = y[i] * sigmoid(- y[i] * theta_acc[i])
 
             # do not forget to update exp_Xw
             for i in range(n_samples):
                 exp_Xw[i] = exp(Xw[i])
 
-            norm_Xtheta_acc = dnorm_enet(
+            dnorm_XTtheta = dnorm_enet(
                 is_sparse, theta_acc, w, X, X_data, X_indices, X_indptr,
                 screened, X_mean, weights_pen, center, positive, alpha, l1_ratio)
 
-            if norm_Xtheta_acc > alpha:
-                tmp = alpha / norm_Xtheta_acc
-                fscal(&n_samples, &tmp, &theta_acc[0], &inc)
+            if dnorm_XTtheta > alpha:
+                theta_scaling = alpha / dnorm_XTtheta
+                fscal(&n_samples, &theta_scaling, &theta_acc[0], &inc)
 
             d_obj_acc = dual(LOGREG, n_samples, alpha, l1_ratio, 0., norm_w2, &theta_acc[0], &y[0])
             if d_obj_acc > d_obj:
                 fcopy(&n_samples, &theta_acc[0], &inc, &theta[0], &inc)
                 gap = p_obj - d_obj_acc
 
         gaps[t] = gap
@@ -285,16 +285,16 @@
     cdef floating approx_grad, actual_grad, sum_sq_hess_diff, pn_epsilon
     cdef floating[:] pn_grad_cache = np.zeros(ws_size, dtype=dtype)
 
     cdef int i, j, ind, max_cd_itr, cd_itr, pn_iter
     cdef floating prob
 
     cdef int start_ptr, end_ptr
-    cdef floating  gap, p_obj, d_obj, norm_Xtheta, norm_Xaux
-    cdef floating tmp, new_value, old_value, diff
+    cdef floating  gap, p_obj, d_obj, dnorm_XTtheta
+    cdef floating tmp, theta_scaling, new_value, old_value, diff
 
     cdef int[:] notin_WS = np.ones(n_features, dtype=np.int32)
     for ind in range(ws_size):
         notin_WS[WS[ind]] = 0
 
     for pn_iter in range(max_pn_iter):
         # run prox newton iterations:
@@ -365,28 +365,28 @@
                     X_delta_w, weights, j, is_sparse, X, X_data, X_indices,
                     X_indptr, False)
                 pn_grad_cache[ind] = actual_grad
                 diff = approx_grad - actual_grad
 
                 pn_grad_diff += diff ** 2
 
-            norm_Xaux = 0.
+            dnorm_XTtheta = 0.
             for ind in range(ws_size):
-                tmp = fabs(pn_grad_cache[ind])
-                if tmp > norm_Xaux:
-                    norm_Xaux = tmp
+                theta_scaling = fabs(pn_grad_cache[ind])
+                if theta_scaling > dnorm_XTtheta:
+                    dnorm_XTtheta = theta_scaling
 
         else:
             # rescale aux to create dual point
-            norm_Xaux = dnorm_enet(
+            dnorm_XTtheta = dnorm_enet(
                 is_sparse, aux, w, X, X_data, X_indices, X_indptr,
                 notin_WS, X_mean, weights_pen, center, 0, alpha, l1_ratio)
 
         for i in range(n_samples):
-            aux[i] /= max(1, norm_Xaux / alpha)
+            aux[i] /= max(1, dnorm_XTtheta / alpha)
 
         d_obj = dual(LOGREG, n_samples, alpha, l1_ratio, 0., norm_w2, &aux[0], &y[0])
         p_obj = primal(LOGREG, alpha, l1_ratio, Xw, y, w, weights_pen)
 
         gap = p_obj - d_obj
         if verbose_in:
             print("iter %d, p_obj %.10f, d_obj % .10f" % (pn_iter, p_obj, d_obj))
```

### Comparing `celer-0.7.2/celer/cython_utils.pxd` & `celer-0.7.3/celer/cython_utils.pxd`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/cython_utils.pyx` & `celer-0.7.3/celer/cython_utils.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return xlogx(x) + xlogx(1. - x)
     else:
         return INFINITY  # not - INFINITY
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
-cdef floating fweighted_norm_w2(floating[:] w, floating[:] weights) nogil: 
+cdef floating fweighted_norm_w2(floating[:] w, floating[:] weights) nogil:
     cdef floating weighted_norm = 0.
     cdef int n_features = w.shape[0]
     cdef int j
 
     for j in range(n_features):
         if weights[j] == INFINITY:
             continue
@@ -387,15 +387,15 @@
         floating[:] X_data, int[:] X_indices, int[:] X_indptr, int[:] skip,
         floating[:] X_mean, floating[:] weights, bint center,
         bint positive, floating alpha, floating l1_ratio) nogil:
     """compute norm(X[:, ~skip].T.dot(theta), ord=inf)"""
     cdef int n_samples = theta.shape[0]
     cdef int n_features = skip.shape[0]
     cdef floating Xj_theta
-    cdef floating scal = 0.
+    cdef floating dnorm_XTtheta = 0.
     cdef floating theta_sum = 0.
     cdef int i, j, Cj, startptr, endptr
 
     if is_sparse:
         # TODO by design theta_sum should always be 0 when center
         if center:
             for i in range(n_samples):
@@ -418,16 +418,16 @@
 
         # minus sign to consider the choice theta = y - Xw and not theta = Xw -y
         if l1_ratio != 1:
             Xj_theta -= alpha * (1 - l1_ratio) * weights[j] * w[j]
 
         if not positive:
             Xj_theta = fabs(Xj_theta)
-        scal = max(scal, Xj_theta / weights[j])
-    return scal
+        dnorm_XTtheta = max(dnorm_XTtheta, Xj_theta / weights[j])
+    return dnorm_XTtheta
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.cdivision(True)
 cdef void set_prios(
     bint is_sparse, floating[:] theta, floating[:] w, floating alpha, floating l1_ratio,
@@ -453,17 +453,17 @@
             for i in range(startptr, endptr):
                 Xj_theta += theta[X_indices[i]] * X_data[i]
         else:
             Xj_theta = fdot(&n_samples, &theta[0], &inc, &X[0, j], &inc)
 
         norms_X_col_j = norms_X_col[j]
         if l1_ratio != 1:
-            Xj_theta -= alpha * (1 - l1_ratio) * weights[j] * w[j] 
+            Xj_theta -= alpha * (1 - l1_ratio) * weights[j] * w[j]
 
-            norms_X_col_j = norms_X_col_j ** 2 
+            norms_X_col_j = norms_X_col_j ** 2
             norms_X_col_j += sqrt(norms_X_col_j + alpha * (1 - l1_ratio) * weights[j])
 
         if positive:
             prios[j] = fabs(Xj_theta - alpha * l1_ratio * weights[j]) / norms_X_col_j
         else:
             prios[j] = (alpha * l1_ratio * weights[j] - fabs(Xj_theta)) / norms_X_col_j
```

### Comparing `celer-0.7.2/celer/datasets/climate.py` & `celer-0.7.3/celer/datasets/climate.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/datasets/libsvm.py` & `celer-0.7.3/celer/datasets/libsvm.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/datasets/ml_uci.py` & `celer-0.7.3/celer/datasets/ml_uci.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/datasets/simulated.py` & `celer-0.7.3/celer/datasets/simulated.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/datasets/tests/test_datasets.py` & `celer-0.7.3/celer/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/dropin_sklearn.py` & `celer-0.7.3/celer/dropin_sklearn.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/group_fast.pyx` & `celer-0.7.3/celer/group_fast.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 cpdef floating dnorm_grp(
         bint is_sparse, floating[::1] theta, int[::1] grp_ptr,
         int[::1] grp_indices, floating[::1, :] X, floating[::1] X_data,
         int[::1] X_indices, int[::1] X_indptr, floating[::1] X_mean,
         floating[:] weights, int ws_size, int[:] C, bint center):
     """Dual norm in the group case, i.e. L2/infty ofter groups."""
     cdef floating Xj_theta, tmp
-    cdef floating scal = 0.
+    cdef floating dnorm_XTtheta = 0.
     cdef floating theta_sum = 0.
     cdef int i, j, g, g_idx, k, startptr, endptr
     cdef int n_groups = grp_ptr.shape[0] - 1
     cdef int n_samples = theta.shape[0]
 
     if is_sparse:
         if center:
@@ -81,15 +81,15 @@
                     if center:
                         Xj_theta -= theta_sum * X_mean[j]
                 else:
                     Xj_theta = fdot(&n_samples, &theta[0], &inc, &X[0, j],
                                     &inc)
                 tmp += Xj_theta ** 2
 
-            scal = max(scal, sqrt(tmp) / weights[g])
+            dnorm_XTtheta = max(dnorm_XTtheta, sqrt(tmp) / weights[g])
 
     else:  # scaling only with features in C
         for g_idx in range(ws_size):
             if weights[g] == INFINITY:
                 continue
 
             g = C[g_idx]
@@ -105,16 +105,16 @@
                     if center:
                         Xj_theta -= theta_sum * X_mean[j]
                 else:
                     Xj_theta = fdot(&n_samples, &theta[0], &inc, &X[0, j],
                                     &inc)
                 tmp += Xj_theta ** 2
 
-            scal = max(scal, sqrt(tmp) / weights[g])
-    return scal
+            dnorm_XTtheta = max(dnorm_XTtheta, sqrt(tmp) / weights[g])
+    return dnorm_XTtheta
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.cdivision(True)
 cdef void set_prios_grp(
         bint is_sparse, int pb, floating[::1] theta, floating alpha, floating[::1, :] X,
@@ -209,20 +209,20 @@
 
     cdef floating[:] old_w_g = np.zeros(max_group_size, dtype=dtype)
 
     cdef floating[::1] gaps = np.zeros(max_iter, dtype=dtype)
     cdef floating[::1] theta_inner = np.zeros(n_samples, dtype=dtype)
     cdef floating[::1] thetacc = np.empty(n_samples, dtype=dtype)
 
-    cdef floating gap, p_obj, d_obj, scal, X_mean_j
+    cdef floating gap, p_obj, d_obj, dnorm_XTtheta, X_mean_j
     cdef floating gap_in, p_obj_in, d_obj_in, tol_in, d_obj_accel
     cdef floating d_obj_from_inner
     cdef floating highest_d_obj = 0.
     cdef floating highest_d_obj_in = 0.
-    cdef floating tmp, R_sum, norm_wg, bst_scal
+    cdef floating tmp, theta_scaling, R_sum, norm_wg, bst_scal
     cdef floating radius = INFINITY
 
     # acceleration variables:
     cdef int K = 6
     cdef floating[:, :] last_K_R = np.empty([K, n_samples], dtype=dtype)
     cdef floating[:, :] U = np.empty([K - 1, n_samples], dtype=dtype)
     cdef floating[:, :] UtU = np.empty([K - 1, K - 1], dtype=dtype)
@@ -233,33 +233,33 @@
     for t in range(max_iter):
         # if t != 0: TODO potential speedup at iteration 0
         fcopy(&n_samples, &R[0], &inc, &theta[0], &inc)
 
         tmp = 1. / n_samples
         fscal(&n_samples, &tmp, &theta[0], &inc)
 
-        scal = dnorm_grp(
+        dnorm_XTtheta = dnorm_grp(
             is_sparse, theta, grp_ptr, grp_indices, X, X_data, X_indices,
             X_indptr, X_mean, weights, n_groups, dummy_C, center)
 
-        if scal > alpha:
-            tmp = alpha / scal
-            fscal(&n_samples, &tmp, &theta[0], &inc)
+        if dnorm_XTtheta > alpha:
+            theta_scaling = alpha / dnorm_XTtheta
+            fscal(&n_samples, &theta_scaling, &theta[0], &inc)
 
         d_obj = dual(pb, n_samples, alpha, l1_ratio, norm_y2, norm_w2, &theta[0], &y[0])
 
         if t > 0:
             # also test dual point returned by inner solver after 1st iter:
-            scal = dnorm_grp(
+            dnorm_XTtheta = dnorm_grp(
                     is_sparse, theta_inner, grp_ptr, grp_indices, X, X_data,
                     X_indices, X_indptr, X_mean, weights, n_groups, dummy_C, center)
 
-            if scal > alpha:
-                tmp = alpha / scal
-                fscal(&n_samples, &tmp, &theta_inner[0], &inc)
+            if dnorm_XTtheta > alpha:
+                theta_scaling = alpha / dnorm_XTtheta
+                fscal(&n_samples, &theta_scaling, &theta_inner[0], &inc)
 
             d_obj_from_inner = dual(
                 pb, n_samples, alpha, l1_ratio, norm_y2, norm_w2, &theta_inner[0], &y[0])
 
             if d_obj_from_inner > d_obj:
                 d_obj = d_obj_from_inner
                 fcopy(&n_samples, &theta_inner[0], &inc, &theta[0], &inc)
@@ -337,43 +337,43 @@
         for epoch in range(max_epochs):
             if epoch != 0 and epoch % gap_freq == 0:
                 fcopy(&n_samples, &R[0], &inc, &theta_inner[0], &inc)
 
                 tmp = 1. / n_samples
                 fscal(&n_samples, &tmp, &theta_inner[0], &inc)
 
-                scal = dnorm_grp(
+                dnorm_XTtheta = dnorm_grp(
                     is_sparse, theta_inner, grp_ptr, grp_indices, X, X_data,
                     X_indices, X_indptr, X_mean, weights, ws_size, C, center)
 
-                if scal > alpha:
-                    tmp = alpha / scal
-                    fscal(&n_samples, &tmp, &theta_inner[0], &inc)
+                if dnorm_XTtheta > alpha:
+                    theta_scaling = alpha / dnorm_XTtheta
+                    fscal(&n_samples, &theta_scaling, &theta_inner[0], &inc)
 
                 # dual value is the same as for the Lasso
                 d_obj_in = dual(
                     pb, n_samples, alpha, l1_ratio, norm_y2, norm_w2, &theta_inner[0], &y[0])
 
                 if use_accel: # also compute accelerated dual_point
                     info_dposv = create_accel_pt(
                         LASSO, n_samples, epoch, gap_freq, &R[0],
                         &thetacc[0], &last_K_R[0, 0], U, UtU, onesK, y)
 
                     # if info_dposv != 0 and verbose:
                     #     print("linear system solving failed")
 
                     if epoch // gap_freq >= K:
-                        scal = dnorm_grp(
+                        dnorm_XTtheta = dnorm_grp(
                             is_sparse, thetacc, grp_ptr, grp_indices, X,
                             X_data, X_indices, X_indptr, X_mean, weights,
                             ws_size, C, center)
 
-                        if scal > alpha:
-                            tmp = alpha / scal
-                            fscal(&n_samples, &tmp, &thetacc[0], &inc)
+                        if dnorm_XTtheta > alpha:
+                            theta_scaling = alpha / dnorm_XTtheta
+                            fscal(&n_samples, &theta_scaling, &thetacc[0], &inc)
 
                         d_obj_accel = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
                                            norm_w2, &thetacc[0], &y[0])
                         if d_obj_accel > d_obj_in:
                             d_obj_in = d_obj_accel
                             fcopy(&n_samples, &thetacc[0], &inc,
                             &theta_inner[0], &inc)
```

### Comparing `celer-0.7.2/celer/homotopy.py` & `celer-0.7.3/celer/homotopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,24 +295,25 @@
 
             # different link equations and normalization scal for dual point:
             if pb in (LASSO, LOGREG):
                 if pb == LASSO:
                     theta = Xw.copy()
                 elif pb == LOGREG:
                     theta = y / (1 + np .exp(y * Xw)) / alpha
-                scal = dnorm_enet(X, theta, w, weights, X_sparse_scaling,
-                                  positive, alpha, l1_ratio)
+                dnorm = dnorm_enet(X, theta, w, weights, X_sparse_scaling,
+                                   positive, alpha, l1_ratio)
             elif pb == GRPLASSO:
                 theta = Xw.copy()
-                scal = dnorm_grp(
+                dnorm = dnorm_grp(
                     is_sparse, theta, grp_ptr, grp_indices, X_dense,
                     X_data, X_indices, X_indptr, X_sparse_scaling,
                     weights, len(grp_ptr) - 1, np.zeros(1, dtype=np.int32),
                     X_sparse_scaling.any())
-            theta *= alpha * l1_ratio / scal
+
+            theta /= max(dnorm / (alpha * l1_ratio), n_samples)
 
         # celer modifies w, Xw, and theta in place:
         if pb == GRPLASSO:
             # TODO this if else scheme is complicated
             sol = celer_grp(
                 is_sparse, LASSO, X_dense, grp_indices, grp_ptr, X_data,
                 X_indices, X_indptr, X_sparse_scaling, y, alpha, w, Xw, theta,
@@ -380,19 +381,19 @@
 
 
 def dnorm_enet(X, theta, w, weights, X_sparse_scaling,
                positive, alpha=1.0, l1_ratio=1.0):
     """Theta should be centered."""
     X_dense, X_data, X_indices, X_indptr = _sparse_and_dense(X)
     skip = np.zeros(X.shape[1], dtype=np.int32)
-    scal = dnorm_enet_cython(
+    dnorm = dnorm_enet_cython(
         sparse.issparse(X), theta, w, X_dense, X_data, X_indices, X_indptr,
         skip, X_sparse_scaling, weights, X_sparse_scaling.any(), positive,
         alpha, l1_ratio)
-    return scal
+    return dnorm
 
 
 def _alpha_max_grp(X, y, groups, center=False, normalize=False):
     """This costly function (copies X) should only be used for debug."""
     grp_ptr, grp_indices = _grp_converter(groups, X.shape[1])
     X, y, X_offset, _, X_scale = _preprocess_data(
         X, y, center, normalize, copy=True)
```

### Comparing `celer-0.7.2/celer/lasso_fast.pyx` & `celer-0.7.3/celer/lasso_fast.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     cdef int t = 0
     cdef int i, j, k, idx, startptr, endptr, epoch
     cdef int ws_size = 0
     cdef int nnz = 0
     cdef floating gap = -1  # initialized for the warning if max_iter=0
     cdef floating p_obj, d_obj, highest_d_obj, radius, tol_in
     cdef floating gap_in, p_obj_in, d_obj_in, d_obj_accel, highest_d_obj_in
-    cdef floating tmp, R_sum, tmp_exp, scal
+    cdef floating theta_scaling, R_sum, tmp, tmp_exp, dnorm_XTtheta
     cdef int n_screened = 0
     cdef bint center = False
     cdef floating old_w_j, X_mean_j
     cdef floating[:] prios = np.empty(n_features, dtype=dtype)
     cdef int[:] screened = np.zeros(n_features, dtype=np.int32)
     cdef int[:] notin_ws = np.zeros(n_features, dtype=np.int32)
 
@@ -95,15 +95,15 @@
             if pb == LOGREG:
                 inv_lc[j] = 4. / norms_X_col[j] ** 2
             else:
                 inv_lc[j] = 1. / norms_X_col[j] ** 2
 
     cdef floating norm_y2 = fnrm2(&n_samples, &y[0], &inc) ** 2
     cdef floating weighted_norm_w2 = fweighted_norm_w2(w, weights)
-    tmp = 1.0
+    theta_scaling = 1.0
 
     # max_iter + 1 is to deal with max_iter=0
     cdef floating[:] gaps = np.zeros(max_iter + 1, dtype=dtype)
     gaps[0] = -1
 
     cdef floating[:] theta_in = np.zeros(n_samples, dtype=dtype)
     cdef floating[:] thetacc = np.zeros(n_samples, dtype=dtype)
@@ -112,45 +112,47 @@
     cdef int[:] ws
     cdef int[:] all_features = np.arange(n_features, dtype=np.int32)
 
     for t in range(max_iter):
         if t != 0:
             create_dual_pt(pb, n_samples, &theta[0], &Xw[0], &y[0])
 
-            scal = dnorm_enet(
+            dnorm_XTtheta = dnorm_enet(
                 is_sparse, theta, w, X, X_data, X_indices, X_indptr, screened,
                 X_mean, weights, center, positive, alpha, l1_ratio)
 
-            if scal > alpha * l1_ratio:
-                tmp = alpha * l1_ratio / scal
-                fscal(&n_samples, &tmp, &theta[0], &inc)
+            if dnorm_XTtheta > alpha * l1_ratio:
+                theta_scaling = alpha * l1_ratio / dnorm_XTtheta
+                fscal(&n_samples, &theta_scaling, &theta[0], &inc)
             else:
-                tmp = 1.
+                theta_scaling = 1.
 
             #  compute ||w||^2 only for Enet
             if l1_ratio != 1:
                 weighted_norm_w2 = fweighted_norm_w2(w, weights)
 
-            d_obj = dual(pb, n_samples, alpha, l1_ratio, norm_y2, tmp**2*weighted_norm_w2, &theta[0], &y[0])
+            d_obj = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
+                theta_scaling**2*weighted_norm_w2, &theta[0], &y[0])
 
             # also test dual point returned by inner solver after 1st iter:
-            scal = dnorm_enet(
+            dnorm_XTtheta = dnorm_enet(
                 is_sparse, theta_in, w, X, X_data, X_indices, X_indptr,
                 screened, X_mean, weights, center, positive, alpha, l1_ratio)
 
-            if scal > alpha * l1_ratio:
-                tmp = alpha * l1_ratio / scal
-                fscal(&n_samples, &tmp, &theta_in[0], &inc)
+            if dnorm_XTtheta  > alpha * l1_ratio:
+                theta_scaling = alpha * l1_ratio / dnorm_XTtheta
+                fscal(&n_samples, &theta_scaling, &theta_in[0], &inc)
             else:
-                tmp = 1.
+                theta_scaling = 1.
 
-            d_obj_from_inner = dual(
-                pb, n_samples, alpha, l1_ratio, norm_y2, tmp**2*weighted_norm_w2, &theta_in[0], &y[0])
+            d_obj_from_inner = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
+                    theta_scaling**2*weighted_norm_w2, &theta_in[0], &y[0])
         else:
-            d_obj = dual(pb, n_samples, alpha, l1_ratio, norm_y2, tmp**2*weighted_norm_w2, &theta[0], &y[0])
+            d_obj = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
+                theta_scaling**2*weighted_norm_w2, &theta[0], &y[0])
 
         if d_obj_from_inner > d_obj:
             d_obj = d_obj_from_inner
             fcopy(&n_samples, &theta_in[0], &inc, &theta[0], &inc)
 
         highest_d_obj = d_obj  # TODO monotonicity could be enforced but it
         # would add yet another variable, best_theta. I'm not sure it brings
@@ -226,53 +228,53 @@
         # calling inner solver which will modify w and R inplace
         highest_d_obj_in = 0
         for epoch in range(max_epochs):
             if epoch != 0 and epoch % gap_freq == 0:
                 create_dual_pt(
                     pb, n_samples, &theta_in[0], &Xw[0], &y[0])
 
-                scal = dnorm_enet(
+                dnorm_XTtheta  = dnorm_enet(
                     is_sparse, theta_in, w, X, X_data, X_indices, X_indptr,
                     notin_ws, X_mean, weights, center, positive, alpha, l1_ratio)
 
-                if scal > alpha * l1_ratio:
-                    tmp = alpha * l1_ratio / scal
-                    fscal(&n_samples, &tmp, &theta_in[0], &inc)
+                if dnorm_XTtheta  > alpha * l1_ratio:
+                    theta_scaling = alpha * l1_ratio / dnorm_XTtheta
+                    fscal(&n_samples, &theta_scaling, &theta_in[0], &inc)
                 else:
-                    tmp = 1.
+                    theta_scaling = 1.
 
                 # update norm_w2 in inner loop for Enet only
                 if l1_ratio != 1:
                     weighted_norm_w2 = fweighted_norm_w2(w, weights)
-                d_obj_in = dual(
-                    pb, n_samples, alpha, l1_ratio, norm_y2, tmp**2*weighted_norm_w2, &theta_in[0], &y[0])
+                d_obj_in = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
+                    theta_scaling**2*weighted_norm_w2, &theta_in[0], &y[0])
 
                 if use_accel: # also compute accelerated dual_point
                     info_dposv = create_accel_pt(
                         pb, n_samples, epoch, gap_freq, &Xw[0],
                         &thetacc[0], &last_K_Xw[0, 0], U, UtU, onesK, y)
 
                     if info_dposv != 0 and verbose_in:
                         pass
                         # print("linear system solving failed")
 
                     if epoch // gap_freq >= K:
-                        scal = dnorm_enet(
+                        dnorm_XTtheta  = dnorm_enet(
                             is_sparse, thetacc, w, X, X_data, X_indices,
                             X_indptr, notin_ws, X_mean, weights, center,
                             positive, alpha, l1_ratio)
 
-                        if scal > alpha * l1_ratio:
-                            tmp = alpha * l1_ratio / scal
-                            fscal(&n_samples, &tmp, &thetacc[0], &inc)
+                        if dnorm_XTtheta  > alpha * l1_ratio:
+                            theta_scaling = alpha * l1_ratio / dnorm_XTtheta
+                            fscal(&n_samples, &theta_scaling, &thetacc[0], &inc)
                         else:
-                            tmp = 1.
+                            theta_scaling = 1.
 
-                        d_obj_accel = dual(
-                            pb, n_samples, alpha, l1_ratio, norm_y2, tmp**2*weighted_norm_w2, &thetacc[0], &y[0])
+                        d_obj_accel = dual(pb, n_samples, alpha, l1_ratio, norm_y2,
+                                theta_scaling**2*weighted_norm_w2, &thetacc[0], &y[0])
                         if d_obj_accel > d_obj_in:
                             d_obj_in = d_obj_accel
                             fcopy(&n_samples, &thetacc[0], &inc,
                                   &theta_in[0], &inc)
 
                 if d_obj_in > highest_d_obj_in:
                     highest_d_obj_in = d_obj_in
```

### Comparing `celer-0.7.2/celer/multitask_fast.pyx` & `celer-0.7.3/celer/multitask_fast.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -34,47 +34,46 @@
 cdef floating dual_scaling_mtl(
         int n_features, int n_samples, int n_tasks, floating[::1, :] theta,
         floating[::1, :] X, int ws_size, int * C, int * screened,
         floating * Xj_theta) nogil:
     cdef int ind, j, k
     cdef int inc = 1
     cdef floating tmp
-    cdef floating nrm = 0.
+    cdef floating dnorm_XTtheta = 0.
 
     if ws_size == n_features:
         for j in range(n_features):
             if screened[j]:
                 continue
             for k in range(n_tasks):
                 Xj_theta[k] = fdot(&n_samples, &theta[0, k], &inc, &X[0, j], &inc)
             tmp = fnrm2(&n_tasks, &Xj_theta[0], &inc)
-            if tmp > nrm:
-                nrm = tmp
+            if tmp > dnorm_XTtheta:
+                dnorm_XTtheta = tmp
     else:
         for ind in range(ws_size):
             j = C[ind]
             for k in range(n_tasks):
                 Xj_theta[k] = fdot(&n_samples, &theta[0, k], &inc, &X[0, j], &inc)
             tmp = fnrm2(&n_tasks, &Xj_theta[0], &inc)
-            if tmp > nrm:
-                nrm = tmp
-    return nrm
+            if tmp > dnorm_XTtheta:
+                dnorm_XTtheta = tmp
+    return dnorm_XTtheta
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.cdivision(True)
 cdef void set_prios_mtl(
         floating[:, ::1] W, int[:] screened,
         floating[::1, :] X, floating[::1, :] theta, floating alpha, floating[:] norms_X_col,
         floating[:] Xj_theta, floating[:] prios, floating radius,
         int * n_screened) nogil:
     cdef int j, k
     cdef int inc = 1
-    cdef floating tmp
     cdef floating nrm = 0.
     cdef int n_samples = X.shape[0]
     cdef int n_features = X.shape[1]
     cdef int n_tasks = W.shape[1]
 
     for j in range(n_features):
         if screened[j]:
@@ -156,20 +155,19 @@
 
 
     if p0 > n_features:
         p0 = n_features
 
     cdef int i, j, k, t
     cdef int inc = 1
-    cdef floating tmp
+    cdef floating tmp, theta_scaling
     cdef int n_obs = n_samples * n_tasks
     cdef int ws_size
     cdef int nnz = 0
-    cdef floating p_obj, d_obj, highes_d_obj, gap, radius
-    cdef floating scal
+    cdef floating p_obj, d_obj, highes_d_obj, gap, radius, dnorm_XTtheta
     cdef int n_screened = 0
     cdef floating[:] prios = np.empty(n_features, dtype=dtype)
     cdef int[:] screened = np.zeros(n_features, dtype=np.int32)
     cdef floating[:] Xj_theta = np.empty(n_tasks, dtype=dtype)
 
     cdef floating norm_Y2 = fnrm2(&n_obs, &Y[0, 0], &inc) ** 2
     # scale tolerance to account for small or large Y:
@@ -187,33 +185,31 @@
 
     for t in range(max_iter):
         # if t != 0: TODO
         p_obj = primal_mtl(n_samples, n_features, n_tasks, W, alpha, R)
         # theta = R :
         fcopy(&n_obs, &R[0, 0], &inc, &theta[0, 0], &inc)
 
-        tmp = 1.
-
-        scal = dual_scaling_mtl(
+        dnorm_XTtheta = dual_scaling_mtl(
             n_features, n_samples, n_tasks, theta, X, n_features,
             &dummy_C[0], &screened[0], &Xj_theta[0])
 
-        if scal > alpha:
-            tmp = alpha / scal
-            fscal(&n_obs, &tmp, &theta[0, 0], &inc)
+        if dnorm_XTtheta > alpha:
+            theta_scaling = alpha / dnorm_XTtheta
+            fscal(&n_obs, &theta_scaling, &theta[0, 0], &inc)
         d_obj = dual_mtl(n_samples, n_tasks, theta, Y, norm_Y2)
 
         if t > 0:
-            scal = dual_scaling_mtl(
+            dnorm_XTtheta = dual_scaling_mtl(
                 n_features, n_samples, n_tasks, theta_inner, X,
                 n_features, &dummy_C[0], &screened[0], &Xj_theta[0])
 
-            if scal > alpha:
-                tmp = alpha / scal
-                fscal(&n_obs, &tmp, &theta_inner[0, 0], &inc)
+            if dnorm_XTtheta > alpha:
+                theta_scaling = alpha / dnorm_XTtheta
+                fscal(&n_obs, &theta_scaling, &theta_inner[0, 0], &inc)
             d_obj_from_inner = dual_mtl(
                 n_samples, n_tasks, theta_inner, Y, norm_Y2)
             if d_obj_from_inner > d_obj:
                 d_obj = d_obj_from_inner
 
         gap = p_obj - d_obj
         if verbose:
@@ -299,15 +295,15 @@
 
     cdef floating p_obj, d_obj, gap
     cdef floating highest_d_obj = 0.
     cdef int i, j, k, epoch, ind
     cdef floating[:] old_Wj = np.empty(n_tasks, dtype=dtype)
     cdef int inc = 1
     cdef int n_obs = n_samples * n_tasks
-    cdef floating tmp, scal
+    cdef floating tmp, dnorm_XTtheta, theta_scaling
     cdef int[:] dummy_screened = np.zeros(1, dtype=np.int32)
     cdef floating[:] Xj_theta = np.empty(n_tasks, dtype=dtype)
 
 
     # acceleration:
     cdef floating[::1, :] theta_acc = np.empty([n_samples, n_tasks],
                                           dtype=dtype, order='F')
@@ -328,39 +324,39 @@
         if epoch > 0 and epoch % gap_freq == 0:
             p_obj = primal_mtl(n_samples, n_features, n_tasks, W, alpha, R)
             fcopy(&n_obs, &R[0, 0], &inc, &theta[0, 0], &inc)
 
             tmp = 1. / n_samples
             fscal(&n_obs, &tmp, &theta[0, 0], &inc)
 
-            scal = dual_scaling_mtl(
+            dnorm_XTtheta = dual_scaling_mtl(
                 n_features, n_samples, n_tasks, theta, X, ws_size,
                 &C[0], &dummy_screened[0], &Xj_theta[0])
 
-            if scal > alpha:
-                tmp = alpha / scal
-                fscal(&n_obs, &tmp, &theta[0, 0], &inc)
+            if dnorm_XTtheta > alpha:
+                theta_scaling = alpha / dnorm_XTtheta
+                fscal(&n_obs, &theta_scaling, &theta[0, 0], &inc)
             d_obj = dual_mtl(n_samples, n_tasks, theta, Y, norm_Y2)
 
             if use_accel:
                 create_accel_pt(
                     LASSO, n_obs, epoch, gap_freq,
                     &R[0, 0], &theta_acc[0, 0], &last_K_R[0, 0], U, UtU,
                     onesK, onesK)  # passing onesK as y which is ignored
                     # account for wrong n_samples passed to create_accel_pt
                 tmp = n_tasks
                 fscal(&n_obs, &tmp, &theta_acc[0, 0], &inc)
                 if epoch // gap_freq >= K:
-                    scal = dual_scaling_mtl(
+                    dnorm_XTtheta = dual_scaling_mtl(
                         n_features, n_samples, n_tasks, theta_acc, X, ws_size,
                         &C[0], &dummy_screened[0], &Xj_theta[0])
 
-                    if scal > alpha:
-                        tmp = alpha / scal
-                        fscal(&n_obs, &tmp, &theta_acc[0, 0], &inc)
+                    if dnorm_XTtheta > alpha:
+                        theta_scaling = alpha / dnorm_XTtheta
+                        fscal(&n_obs, &theta_scaling, &theta_acc[0, 0], &inc)
                     d_obj_acc = dual_mtl(
                         n_samples, n_tasks, theta_acc, Y, norm_Y2)
                     if d_obj_acc > d_obj:
                         d_obj = d_obj_acc
                         fcopy(&n_obs, &theta_acc[0, 0], &inc, &theta[0, 0],
                               &inc)
             highest_d_obj = max(highest_d_obj, d_obj)
```

### Comparing `celer-0.7.2/celer/plot_utils.py` & `celer-0.7.3/celer/plot_utils.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/tests/test_docstring_parameters.py` & `celer-0.7.3/celer/tests/test_docstring_parameters.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/tests/test_enet.py` & `celer-0.7.3/celer/tests/test_enet.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/tests/test_lasso.py` & `celer-0.7.3/celer/tests/test_lasso.py`

 * *Files 4% similar despite different names*

```diff
@@ -245,9 +245,23 @@
         assert_array_less(dual_gaps[0], tol * n_samples * np.log(2))
     else:
         assert_array_less(dual_gaps[0], tol * norm(y) ** 2 / 2.)
 
     assert_array_equal(coefs[inf_indices], 0)
 
 
+def test_one_iteration_alpha_max():
+    n_samples, n_features = 100, 50
+    X, y = build_dataset(n_samples, n_features)
+
+    alpha_max = norm(X.T @ y, ord=np.inf) / n_samples
+    m = 5
+    model = Lasso(alpha=m*alpha_max, fit_intercept=False)
+    model.fit(X, y)
+
+    assert_array_equal(model.coef_, np.zeros(n_features))
+    # solver exits right after computing first duality gap:
+    np.testing.assert_equal(model.n_iter_, 1)
+
+
 if __name__ == "__main__":
     pass
```

### Comparing `celer-0.7.2/celer/tests/test_logreg.py` & `celer-0.7.3/celer/tests/test_logreg.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/tests/test_mtl.py` & `celer-0.7.3/celer/tests/test_mtl.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer/utils/testing.py` & `celer-0.7.3/celer/utils/testing.py`

 * *Files identical despite different names*

### Comparing `celer-0.7.2/celer.egg-info/SOURCES.txt` & `celer-0.7.3/celer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
 whats_new.rst
 celer/PN_logreg.pyx
 celer/__init__.py
 celer/cython_utils.pxd
 celer/cython_utils.pyx
```

### Comparing `celer-0.7.2/whats_new.rst` & `celer-0.7.3/whats_new.rst`

 * *Files identical despite different names*

