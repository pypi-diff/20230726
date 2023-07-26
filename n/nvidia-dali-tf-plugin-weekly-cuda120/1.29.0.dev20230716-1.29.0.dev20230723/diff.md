# Comparing `tmp/nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716.tar.gz` & `tmp/nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716.tar", last modified: Mon Jul 17 07:03:33 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723.tar", last modified: Wed Jul 26 00:03:32 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716.tar` & `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-17 07:03:33.927240 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      468 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       36 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1704 2023-07-17 07:03:33.927240 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      313 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-17 07:03:33.927240 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1704 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      293 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-17 07:03:33.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-17 07:03:33.927240 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 00:03:32.934933 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      468 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       36 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1704 2023-07-26 00:03:32.934933 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      313 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 00:03:32.934933 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1704 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      293 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-26 00:03:32.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-26 00:03:32.934933 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/setup.py
```

### Comparing `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/LICENSE.md` & `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/PKG-INFO` & `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-weekly-cuda120
-Version: 1.29.0.dev20230716
+Version: 1.29.0.dev20230723
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/nvidia_dali_tf_plugin_weekly_cuda120.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-weekly-cuda120
-Version: 1.29.0.dev20230716
+Version: 1.29.0.dev20230723
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230716/setup.py` & `nvidia-dali-tf-plugin-weekly-cuda120-1.29.0.dev20230723/setup.py`

 * *Files identical despite different names*

