# Comparing `tmp/pypose-0.5.0.tar.gz` & `tmp/pypose-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.5.0.tar", last modified: Wed Jul 26 15:47:32 2023, max compression
+gzip compressed data, was "pypose-0.5.0b0.tar", last modified: Mon Jun 19 06:08:47 2023, max compression
```

## Comparing `pypose-0.5.0.tar` & `pypose-0.5.0b0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.577858 pypose-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-07-26 15:47:21.000000 pypose-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-26 15:47:32.573858 pypose-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-26 15:47:21.000000 pypose-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.561858 pypose-0.5.0/pypose/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.565858 pypose-0.5.0/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.565858 pypose-0.5.0/pypose/function/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/function/checking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/function/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/function/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/function/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.565858 pypose-0.5.0/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    43346 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.569858 pypose-0.5.0/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/pnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.573858 pypose-0.5.0/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.573858 pypose-0.5.0/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-26 15:47:21.000000 pypose-0.5.0/pypose/utils/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.561858 pypose-0.5.0/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:47:32.000000 pypose-0.5.0/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:47:32.573858 pypose-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 15:47:21.000000 pypose-0.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 15:47:21.000000 pypose-0.5.0/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:47:32.577858 pypose-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-26 15:47:21.000000 pypose-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-19 06:08:37.000000 pypose-0.5.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-19 06:08:47.789939 pypose-0.5.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-19 06:08:37.000000 pypose-0.5.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43346 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 06:08:37.000000 pypose-0.5.0b0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 06:08:37.000000 pypose-0.5.0b0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:08:47.789939 pypose-0.5.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-19 06:08:37.000000 pypose-0.5.0b0/setup.py
```

### Comparing `pypose-0.5.0/LICENSE` & `pypose-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/PKG-INFO` & `pypose-0.5.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.5.0
+Version: 0.5.0b0
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.5.0/README.md` & `pypose-0.5.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/__init__.py` & `pypose-0.5.0b0/pypose/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/basics/ops.py` & `pypose-0.5.0b0/pypose/basics/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/function/checking.py` & `pypose-0.5.0b0/pypose/function/checking.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/function/geometry.py` & `pypose-0.5.0b0/pypose/function/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,69 +107,49 @@
     else:
         assert is_lietensor(extrinsics) and extrinsics.shape[-1] == 7, "Type incorrect."
         torch.broadcast_shapes(points.shape[:-2], intrinsics.shape[:-2], extrinsics.shape[:-1])
         points = extrinsics.unsqueeze(-2) @ points
     return homo2cart(points @ intrinsics.mT)
 
 
-def reprojerr(points, pixels, intrinsics, extrinsics=None, reduction='none'):
+def reprojerr(points, pixels, intrinsics, extrinsics=None):
     r'''
     Calculates batched per-pixel reprojection error (pixel distance) for points either in
     the camera or world frame given camera intrinsics or extrinsics, respectively.
 
     Args:
         points (``torch.Tensor``): The 3D coordinate of points. Assumed to be in the
             camera frame if ``extrinsics`` is ``None``, otherwiwse in the world frame.
             The shape has to be (..., N, 3).
         pixels (``torch.Tensor``): The image points. The associated pixel.
             The shape has to be (..., N, 2).
         intrinsics (``torch.Tensor``): intrinsic matrices.
             The shape has to be (..., 3, 3).
         extrinsics (``LieTensor``, optional): The camera extrinsics.
             The shape has to be (..., 7). Default: ``None``.
-        reduction (``str``, optional): The reduction to apply on the output: ``'none'``
-            | ``'sum'`` | ``'norm'``
-
-            ``'none'``: No reduction is applied
-
-            ``'sum'``: The reprojection error on each component (u, v) is summed for
-            each pixel (L1 Norm)
-
-            ``'norm'``: The reprojection error's L2 norm for each pixel
     Returns:
-        Per-pixel reprojection error.
-
-        The shape is (..., N) if reduction is ``'sum'`` or ``'norm'``.
-
-        The shape is (..., N, 2) if reduction is ``'none'``.
+        Per-pixel reprojection error. The shape is (..., N).
 
     Example:
         >>> import torch, pypose as pp
         >>> f, (H, W) = 2, (9, 9) # focal length and image height, width
         >>> intrinsics = torch.tensor([[f, 0, H / 2],
         ...                            [0, f, W / 2],
         ...                            [0, 0,   1  ]])
         >>> object = torch.randn(6, 3)
         >>> pose = pp.randn_SE3()
         >>> pixels = pp.point2pixel(object, intrinsics, pose)
-        >>> err = pp.reprojerr(object, pixels, intrinsics, pose, reduction='norm')
+        >>> err = pp.reprojerr(object, pixels, intrinsics, pose)
         tensor([0., 0., 0., 0., 0., 0.])
     '''
     torch.broadcast_shapes(points.shape[:-2], pixels.shape[:-2], intrinsics.shape[:-2])
     assert points.size(-1) == 3 and pixels.size(-1) == 2 and \
            intrinsics.size(-1) == intrinsics.size(-2) == 3, "Shape not compatible."
-    assert reduction in {'norm', 'sum', 'none'}, \
-           "Reduction method can only be 'norm'|'sum'|'none'."
     img_repj = point2pixel(points, intrinsics, extrinsics)
-
-    if reduction == 'norm':
-        return (img_repj - pixels).norm(dim=-1)
-    elif reduction == 'sum':
-        return (img_repj - pixels).sum(dim=-1)
-    return img_repj - pixels
+    return (img_repj - pixels).norm(dim=-1)
 
 
 def knn(ref, nbr, k=1, ord=2, dim=-1, largest=False, sorted=True):
     r'''
     Select the k nearest neighbor points of reference from neighbors in each batch.
 
     Args:
```

### Comparing `pypose-0.5.0/pypose/function/linalg.py` & `pypose-0.5.0b0/pypose/function/linalg.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/lietensor/__init__.py` & `pypose-0.5.0b0/pypose/lietensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/lietensor/basics.py` & `pypose-0.5.0b0/pypose/lietensor/basics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/lietensor/convert.py` & `pypose-0.5.0b0/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/lietensor/lietensor.py` & `pypose-0.5.0b0/pypose/lietensor/lietensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -904,25 +904,25 @@
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs={}):
         ltypes = (torch.Tensor if t is LieTensor or Parameter else t for t in types)
         data = torch.Tensor.__torch_function__(func, ltypes, args, kwargs)
         if data is not None and func.__name__ in HANDLED_FUNCTIONS:
             args, spec = tree_flatten(args)
             ltype = [arg.ltype for arg in args if isinstance(arg, LieTensor)][0]
-            def wrap(t):
+            def warp(t):
                 if isinstance(t, torch.Tensor) and not isinstance(t, cls):
                     lt = torch.Tensor.as_subclass(t, LieTensor)
                     lt.ltype = ltype
                     if lt.shape[-1:] != lt.ltype.dimension:
                         link = 'https://pypose.org/docs/main/generated/pypose.LieTensor'
                         warnings.warn('Tensor Shape Invalid by calling {}, ' \
                             'go to {}'.format(func, link))
                     return lt
                 return t
-            return tree_map(wrap, data)
+            return tree_map(warp, data)
         return data
 
     @property
     def lshape(self) -> torch.Size:
         r'''
         LieTensor Shape (shape of torch.Tensor by ignoring the last dimension)
```

### Comparing `pypose-0.5.0/pypose/lietensor/operation.py` & `pypose-0.5.0b0/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/lietensor/utils.py` & `pypose-0.5.0b0/pypose/lietensor/utils.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/module/dynamics.py` & `pypose-0.5.0b0/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/module/ekf.py` & `pypose-0.5.0b0/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/module/icp.py` & `pypose-0.5.0b0/pypose/module/icp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import torch
-from torch import nn
 from .. import knn, svdtf, is_SE3
 from ..utils.stepper import ReduceToBason
 
 
-class ICP(nn.Module):
+class ICP(torch.nn.Module):
     r'''
     Batched Iterative Closest Point (ICP) algorithm to find a rigid transformation
     between two sets of points using Singular Value Decomposition (SVD).
 
     Args:
         init (``LieTensor``, optional): the initial transformation :math:`T_{\text{init}}`
             in ``SE3type LieTensor``. Default: ``None``.
```

### Comparing `pypose-0.5.0/pypose/module/imu_preintegrator.py` & `pypose-0.5.0b0/pypose/module/imu_preintegrator.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/module/lqr.py` & `pypose-0.5.0b0/pypose/module/lqr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
-from torch import nn
+import torch.nn as nn
 from .. import bmv, bvmv
-from torch.linalg import cholesky, vecdot
+from torch.linalg import vecdot
 
 
 class LQR(nn.Module):
     r'''
     Linear Quadratic Regulator (LQR) with Dynamic Programming.
 
     Args:
@@ -300,14 +300,15 @@
         Returns:
             List of :obj:`Tensor`: A list of tensors including the solved state sequence
             :math:`\mathbf{x}`, the solved input sequence :math:`\mathbf{u}`, and the
             associated quadratic costs :math:`\mathbf{c}` over the time horizon.
         '''
         K, k = self.lqr_backward(x_init, dt, u_traj, u_lower, u_upper, du)
         x, u, cost = self.lqr_forward(x_init, K, k, u_lower, u_upper, du)
+
         return x, u, cost
 
     def lqr_backward(self, x_init, dt, u_traj=None, u_lower=None, u_upper=None, du=None):
 
         ns, nsc = x_init.size(-1), self.p.size(-1)
         nc = nsc - ns
 
@@ -340,19 +341,18 @@
                 F = torch.cat((A, B), dim=-1)
                 Qt = self.Q[...,t,:,:] + F.mT @ V @ F
                 qt = p[...,t,:] + bmv(F.mT, v)
 
             Qxx, Qxu = Qt[..., :ns, :ns], Qt[..., :ns, ns:]
             Qux, Quu = Qt[..., ns:, :ns], Qt[..., ns:, ns:]
             qx, qu = qt[..., :ns], qt[..., ns:]
+            Quu_inv = torch.linalg.pinv(Quu)
 
-            L = cholesky(Quu)
-            K[...,t,:,:] = Kt = -torch.cholesky_solve(Qux, L)
-            k[...,t,:] = kt = -torch.cholesky_solve(qu.unsqueeze(-1), L).squeeze(-1)
-
+            K[...,t,:,:] = Kt = - Quu_inv @ Qux
+            k[...,t,:] = kt = - bmv(Quu_inv, qu)
             V = Qxx + Qxu @ Kt + Kt.mT @ Qux + Kt.mT @ Quu @ Kt
             v = qx  + bmv(Qxu, kt) + bmv(Kt.mT, qu) + bmv(Kt.mT @ Quu, kt)
 
         return K, k
 
     def lqr_forward(self, x_init, K, k, u_lower=None, u_upper=None, du=None):
```

### Comparing `pypose-0.5.0/pypose/module/mpc.py` & `pypose-0.5.0b0/pypose/module/mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from .lqr import LQR
-from torch import nn
+import torch.nn as nn
 from ..utils.stepper import ReduceToBason
 
 
 class MPC(nn.Module):
     r'''
     Model Predictive Control (MPC) based on iterative LQR.
```

### Comparing `pypose-0.5.0/pypose/module/pf.py` & `pypose-0.5.0b0/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/module/pnp.py` & `pypose-0.5.0b0/pypose/module/pnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import torch
-from torch import nn
 from torch.linalg import vecdot
 from torch import broadcast_shapes
 
 from .. import bmv
 from ..optim import GaussNewton
 from ..optim.solver import LSTSQ
 from ..optim.scheduler import StopOnPlateau
 from ..function import reprojerr, cart2homo, svdtf
 
 
-class BetaObjective(nn.Module):
+class BetaObjective(torch.nn.Module):
     # Optimize the beta according to the objective in the ePnP paper.
     def __init__(self, beta):
         super().__init__()
         self.beta = torch.nn.Parameter(beta)
         self.i = (0, 0, 0, 1, 1, 2)
         self.j = (1, 2, 3, 2, 3, 3)
 
@@ -22,15 +21,15 @@
         # See Eq. 15 in the paper
         base_c = bmv(nullv.mT, self.beta).unflatten(dim=-1, sizes=(4, 3))
         dist_c = (base_c[..., self.i, :] - base_c[..., self.j, :]).norm(dim=-1)
         dist_w = (base_w[..., self.i, :] - base_w[..., self.j, :]).norm(dim=-1)
         return dist_w - dist_c
 
 
-class EPnP(nn.Module):
+class EPnP(torch.nn.Module):
     r'''
     Batched EPnP Solver - a non-iterative :math:`\mathcal{O}(n)` solution to the
     Perspective-:math:`n`-Point (PnP) problem for :math:`n \geq 4`.
 
     Args:
         intrinsics (``torch.Tensor``, optional): The camera intrinsics.
             The shape is (..., 3, 3). Default: None
@@ -155,15 +154,15 @@
         # Select naive and calculate alpha in the world coordinate
         bases = self._svd_basis(points)
         alpha = self._compute_alpha(points, bases)
         nullv = self._compute_nullv(pixels, alpha, intrinsics)
         l_mat, rho = self._compute_lrho(nullv, bases)
         betas = self._compute_betas(l_mat, rho)
         poses, scales = self._compute_solution(betas, nullv, alpha, points)
-        errors = reprojerr(points, pixels, intrinsics, poses, reduction='norm')
+        errors = reprojerr(points, pixels, intrinsics, poses)
         pose, beta, scale = self._best_solution(errors, poses, betas, scales)
 
         if self.refine:
             beta = self._refine(beta * scale, nullv, bases)
             pose, scale = self._compute_solution(beta, nullv, alpha, points)
 
         return pose
```

### Comparing `pypose-0.5.0/pypose/module/ukf.py` & `pypose-0.5.0b0/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/corrector.py` & `pypose-0.5.0b0/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/functional.py` & `pypose-0.5.0b0/pypose/optim/functional.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/kernel.py` & `pypose-0.5.0b0/pypose/optim/kernel.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/optimizer.py` & `pypose-0.5.0b0/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/scheduler.py` & `pypose-0.5.0b0/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/solver.py` & `pypose-0.5.0b0/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/optim/strategy.py` & `pypose-0.5.0b0/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/utils/collect_env.py` & `pypose-0.5.0b0/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose/utils/stepper.py` & `pypose-0.5.0b0/pypose/utils/stepper.py`

 * *Files identical despite different names*

### Comparing `pypose-0.5.0/pypose.egg-info/PKG-INFO` & `pypose-0.5.0b0/pypose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.5.0
+Version: 0.5.0b0
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.5.0/pypose.egg-info/SOURCES.txt` & `pypose-0.5.0b0/pypose.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 pypose.egg-info/zip-safe
 pypose/basics/__init__.py
 pypose/basics/ops.py
 pypose/function/__init__.py
 pypose/function/checking.py
 pypose/function/geometry.py
 pypose/function/linalg.py
-pypose/function/spline.py
 pypose/lietensor/__init__.py
 pypose/lietensor/basics.py
 pypose/lietensor/convert.py
 pypose/lietensor/lietensor.py
 pypose/lietensor/operation.py
 pypose/lietensor/utils.py
 pypose/module/__init__.py
```

### Comparing `pypose-0.5.0/setup.py` & `pypose-0.5.0b0/setup.py`

 * *Files identical despite different names*

