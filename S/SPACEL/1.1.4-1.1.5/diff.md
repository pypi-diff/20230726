# Comparing `tmp/SPACEL-1.1.4.tar.gz` & `tmp/SPACEL-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPACEL-1.1.4.tar", last modified: Thu Jul 13 02:22:31 2023, max compression
+gzip compressed data, was "SPACEL-1.1.5.tar", last modified: Wed Jul 26 13:43:28 2023, max compression
```

## Comparing `SPACEL-1.1.4.tar` & `SPACEL-1.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.770411 SPACEL-1.1.4/
--rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 02:22:31.769992 SPACEL-1.1.4/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)     3708 2023-07-12 13:44:19.000000 SPACEL-1.1.4/README.md
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.662074 SPACEL-1.1.4/SPACEL/
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.689779 SPACEL-1.1.4/SPACEL/Scube/
--rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Scube/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.4/SPACEL/Scube/alignment.py
--rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.4/SPACEL/Scube/gpr.py
--rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Scube/plot.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.4/SPACEL/Scube/utils_3d.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.747946 SPACEL-1.1.4/SPACEL/Splane/
--rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.4/SPACEL/Splane/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/graph.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.763519 SPACEL-1.1.4/SPACEL/Splane/kegra/
--rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/gnn.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/kegra/gnn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Splane/pygcn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.4/SPACEL/Splane/utils.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.768054 SPACEL-1.1.4/SPACEL/Spoint/
--rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.4/SPACEL/Spoint/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_augmentation.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_downsample.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/data_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/metrics.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/Spoint/spatial_simulation.py
--rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.4/SPACEL/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-13 02:21:25.000000 SPACEL-1.1.4/SPACEL/_version.py
--rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.4/SPACEL/setting.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 02:22:31.664270 SPACEL-1.1.4/SPACEL.egg-info/
--rw-r--r--   0 xuhao      (501) staff       (20)     4009 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/SOURCES.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/dependency_links.txt
--rw-r--r--   0 xuhao      (501) staff       (20)      108 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/requires.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-13 02:22:31.000000 SPACEL-1.1.4/SPACEL.egg-info/top_level.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-13 02:22:31.770517 SPACEL-1.1.4/setup.cfg
--rw-r--r--   0 xuhao      (501) staff       (20)      885 2023-07-13 02:20:15.000000 SPACEL-1.1.4/setup.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.489902 SPACEL-1.1.5/
+-rw-r--r--   0 xuhao      (501) staff       (20)     5069 2023-07-26 13:43:28.489531 SPACEL-1.1.5/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)     4768 2023-07-26 13:34:25.000000 SPACEL-1.1.5/README.md
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.314942 SPACEL-1.1.5/SPACEL/
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.408151 SPACEL-1.1.5/SPACEL/Scube/
+-rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Scube/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.5/SPACEL/Scube/alignment.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.5/SPACEL/Scube/gpr.py
+-rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Scube/plot.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.5/SPACEL/Scube/utils_3d.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.482003 SPACEL-1.1.5/SPACEL/Splane/
+-rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    14649 2023-07-26 13:07:52.000000 SPACEL-1.1.5/SPACEL/Splane/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/graph.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.483791 SPACEL-1.1.5/SPACEL/Splane/kegra/
+-rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/gnn.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/gnn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/pygcn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.5/SPACEL/Splane/utils.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.488694 SPACEL-1.1.5/SPACEL/Spoint/
+-rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.5/SPACEL/Spoint/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_augmentation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_downsample.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/metrics.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/spatial_simulation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.5/SPACEL/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-26 13:42:03.000000 SPACEL-1.1.5/SPACEL/_version.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/setting.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.316779 SPACEL-1.1.5/SPACEL.egg-info/
+-rw-r--r--   0 xuhao      (501) staff       (20)     5069 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       82 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/requires.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/top_level.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-26 13:43:28.489997 SPACEL-1.1.5/setup.cfg
+-rw-r--r--   0 xuhao      (501) staff       (20)      815 2023-07-14 02:56:55.000000 SPACEL-1.1.5/setup.py
```

### Comparing `SPACEL-1.1.4/PKG-INFO` & `SPACEL-1.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.4
+Version: 1.1.5
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -19,55 +19,67 @@
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
-    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/Visium_human_DLPFC_Spoint.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/Visium_human_breast_cancer_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Identify uniform spatial domain on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Scube.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on mouse embryo Stereo-seq dataset](docs/tutorials/Stereo-seq_Scube.ipynb)
+    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/STARmap_mouse_brain_GPR.ipynb)
+    * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
+    * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
+    * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.5 2023-07-26
+#### Fixed Bugs
+- Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
+#### Features
+- Optimized the time and memory consumption of the Splane training process for large datasets.
+
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
 
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
+**Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
 conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
-* Test if [PyTorch](https://pytorch.org) for GPU available:
-```
-python
->>> import torch
->>> torch.cuda.is_available()
-```
-If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
 
 Note: If you want to run 3D expression GPR model in Scube, you need to install the [Open3D](http://www.open3d.org/docs/release/) python library first.
 
 ## Installation
 * Install `SPACEL`:
 ```
 pip install SPACEL
 ```
+* Test if [PyTorch](https://pytorch.org) for GPU available:
+```
+python
+>>> import torch
+>>> torch.cuda.is_available()
+```
+If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
```

### Comparing `SPACEL-1.1.4/README.md` & `SPACEL-1.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -9,55 +9,67 @@
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
-    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/Visium_human_DLPFC_Spoint.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/Visium_human_breast_cancer_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Identify uniform spatial domain on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Scube.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on mouse embryo Stereo-seq dataset](docs/tutorials/Stereo-seq_Scube.ipynb)
+    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/STARmap_mouse_brain_GPR.ipynb)
+    * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
+    * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
+    * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.5 2023-07-26
+#### Fixed Bugs
+- Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
+#### Features
+- Optimized the time and memory consumption of the Splane training process for large datasets.
+
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
 
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
+**Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
 conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
-* Test if [PyTorch](https://pytorch.org) for GPU available:
-```
-python
->>> import torch
->>> torch.cuda.is_available()
-```
-If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
 
 Note: If you want to run 3D expression GPR model in Scube, you need to install the [Open3D](http://www.open3d.org/docs/release/) python library first.
 
 ## Installation
 * Install `SPACEL`:
 ```
 pip install SPACEL
 ```
+* Test if [PyTorch](https://pytorch.org) for GPU available:
+```
+python
+>>> import torch
+>>> torch.cuda.is_available()
+```
+If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
```

### Comparing `SPACEL-1.1.4/SPACEL/Scube/alignment.py` & `SPACEL-1.1.5/SPACEL/Scube/alignment.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Scube/gpr.py` & `SPACEL-1.1.5/SPACEL/Scube/gpr.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Scube/plot.py` & `SPACEL-1.1.5/SPACEL/Scube/plot.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Scube/utils_3d.py` & `SPACEL-1.1.5/SPACEL/Scube/utils_3d.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/base_model.py` & `SPACEL-1.1.5/SPACEL/Splane/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,28 +191,18 @@
         self.model_g.train()
         self.optimizer_g.zero_grad()
         encoded, decoded = self.model_g(self.graph[0],self.graph[1:])
         y_disc = self.model_d(encoded)
         d_loss = F.cross_entropy(self.slice_class_onehot, y_disc)
         decoded_mask = decoded[self.train_idx]
         x_mask = self.graph[0][self.train_idx]
-        f_adj = torch.matmul(encoded, torch.transpose(encoded,0,1))
-        simi_loss = -torch.mean(f_adj[self.nb_mask[0],self.nb_mask[1]]) + torch.mean(torch.abs(encoded[self.nb_mask[0]]-encoded[self.nb_mask[1]]))
-        g_loss = torch.sum(self.celltype_weights*F.cosine_similarity(x_mask, decoded_mask,dim=0))+torch.sum(self.celltype_weights*self.kl_divergence(x_mask, decoded_mask, dim=0)) + simi_l*simi_loss
-        
-        regularization_params = torch.cat([
-            torch.cat([x.view(-1) for x in self.model_g.encode_gc1.parameters()]),
-            torch.cat([x.view(-1) for x in self.model_g.decode_gc1.parameters()])
-        ])
-        l1_regularization = self.l1 * torch.norm(regularization_params, 1)
-        l2_regularization = self.l2 * torch.norm(regularization_params, 2)
+        simi_loss = -torch.mean(torch.sum(encoded[self.nb_mask[0]] * encoded[self.nb_mask[1]], dim=1)) + torch.mean(torch.abs(encoded[self.nb_mask[0]]-encoded[self.nb_mask[1]]))
+        g_loss = -torch.sum(self.celltype_weights*F.cosine_similarity(x_mask, decoded_mask,dim=0))+torch.sum(self.celltype_weights*self.kl_divergence(x_mask, decoded_mask, dim=0)) + simi_l*simi_loss
 
-        l1_l2_loss = l1_regularization + l2_regularization
-        
-        total_loss = g_loss - d_l*d_loss # + l1_l2_loss
+        total_loss = g_loss - d_l*d_loss
         total_loss.backward()
         self.optimizer_g.step()
         return total_loss
     
     def train_model_d(self,):
         self.model_d.train()
         self.optimizer_d.zero_grad()
@@ -229,17 +219,16 @@
         encoded, decoded = self.model_g(self.graph[0],self.graph[1:])
         y_disc = self.model_d(encoded)
         d_loss = F.cross_entropy(self.slice_class_onehot, y_disc)
         decoded_mask = decoded[self.test_idx]
         x_mask = self.graph[0][self.test_idx]
         ll = torch.eq(torch.argmax(self.slice_class_onehot, -1), torch.argmax(y_disc, -1))
         accuarcy = ll.to(torch.float32).mean()
-        f_adj = torch.matmul(encoded, torch.transpose(encoded,0,1))
-        simi_loss = -torch.mean(f_adj[self.nb_mask[0],self.nb_mask[1]]) + torch.mean(torch.abs(encoded[self.nb_mask[0]]-encoded[self.nb_mask[1]]))
-        g_loss = torch.sum(self.celltype_weights*F.cosine_similarity(x_mask, decoded_mask,dim=0))+torch.sum(self.celltype_weights*self.kl_divergence(x_mask, decoded_mask, dim=0)) + simi_l*simi_loss
+        simi_loss = -torch.mean(torch.sum(encoded[self.nb_mask[0]] * encoded[self.nb_mask[1]], dim=1)) + torch.mean(torch.abs(encoded[self.nb_mask[0]]-encoded[self.nb_mask[1]]))
+        g_loss = -torch.sum(self.celltype_weights*F.cosine_similarity(x_mask, decoded_mask,dim=0))+torch.sum(self.celltype_weights*self.kl_divergence(x_mask, decoded_mask, dim=0)) + simi_l*simi_loss
         total_loss = g_loss - d_l*d_loss
         db_loss = clustering(self.Cluster, encoded.cpu().detach().numpy())
         return total_loss, g_loss, d_loss, accuarcy, simi_loss, db_loss, encoded, decoded
     
     def train(
         self,
         max_epochs=300,
```

### Comparing `SPACEL-1.1.4/SPACEL/Splane/graph.py` & `SPACEL-1.1.5/SPACEL/Splane/graph.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/kegra/gnn.py` & `SPACEL-1.1.5/SPACEL/Splane/kegra/gnn.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/kegra/gnn_utils.py` & `SPACEL-1.1.5/SPACEL/Splane/kegra/gnn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/model.py` & `SPACEL-1.1.5/SPACEL/Splane/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/pygcn_utils.py` & `SPACEL-1.1.5/SPACEL/Splane/pygcn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Splane/utils.py` & `SPACEL-1.1.5/SPACEL/Splane/utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/base_model.py` & `SPACEL-1.1.5/SPACEL/Spoint/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/data_augmentation.py` & `SPACEL-1.1.5/SPACEL/Spoint/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/data_downsample.py` & `SPACEL-1.1.5/SPACEL/Spoint/data_downsample.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/data_utils.py` & `SPACEL-1.1.5/SPACEL/Spoint/data_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/metrics.py` & `SPACEL-1.1.5/SPACEL/Spoint/metrics.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/model.py` & `SPACEL-1.1.5/SPACEL/Spoint/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/Spoint/spatial_simulation.py` & `SPACEL-1.1.5/SPACEL/Spoint/spatial_simulation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL/setting.py` & `SPACEL-1.1.5/SPACEL/setting.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/SPACEL.egg-info/PKG-INFO` & `SPACEL-1.1.5/SPACEL.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.4
+Version: 1.1.5
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -19,55 +19,67 @@
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
-    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/Visium_human_DLPFC_Spoint.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/Visium_human_breast_cancer_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Identify uniform spatial domain on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Splane.ipynb)
+    * [Splane&Scube tutorial (1/2): Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/MERFISH_mouse_brain_Scube.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on mouse embryo Stereo-seq dataset](docs/tutorials/Stereo-seq_Scube.ipynb)
+    * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/STARmap_mouse_brain_GPR.ipynb)
+    * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
+    * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
+    * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.5 2023-07-26
+#### Fixed Bugs
+- Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
+#### Features
+- Optimized the time and memory consumption of the Splane training process for large datasets.
+
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
 
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
+**Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
 conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
-* Test if [PyTorch](https://pytorch.org) for GPU available:
-```
-python
->>> import torch
->>> torch.cuda.is_available()
-```
-If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
 
 Note: If you want to run 3D expression GPR model in Scube, you need to install the [Open3D](http://www.open3d.org/docs/release/) python library first.
 
 ## Installation
 * Install `SPACEL`:
 ```
 pip install SPACEL
 ```
+* Test if [PyTorch](https://pytorch.org) for GPU available:
+```
+python
+>>> import torch
+>>> torch.cuda.is_available()
+```
+If these command line have not return `True`, please check your gpu driver version and `cudatoolkit` version. For more detail, look at [CUDA Toolkit Major Component Versions](https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html#cuda-major-component-versions).
```

### Comparing `SPACEL-1.1.4/SPACEL.egg-info/SOURCES.txt` & `SPACEL-1.1.5/SPACEL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.4/setup.py` & `SPACEL-1.1.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,20 +16,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/QuKunLab/SPACEL",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
         "pip",
-        "squidpy",
-        "scvi-tools",
-        "scipy",
+        "squidpy<1.3",
+        "scvi-tools<=0.20.3",
         "scikit-learn",
-        "matplotlib",
-        "seaborn",
         "scanpy",
         "numba",
         "torch<=1.13",
         "gpytorch",
-        "torchmetrics",
     ],
 )
```

