# Comparing `tmp/foambryo-0.3.0.tar.gz` & `tmp/foambryo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-dggk_44j/foambryo-0.3.0.tar", last modified: Tue Jul 25 22:28:24 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-6qg7_my4/foambryo-0.3.1.tar", last modified: Tue Jul 25 22:36:39 2023, max compression
```

## Comparing `foambryo-0.3.0.tar` & `foambryo-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.481934 foambryo-0.3.0/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12110 2023-07-25 22:28:24.482112 foambryo-0.3.0/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11557 2023-07-25 22:26:11.000000 foambryo-0.3.0/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-07-25 22:24:28.000000 foambryo-0.3.0/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      851 2023-07-25 22:28:24.483620 foambryo-0.3.0/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.452952 foambryo-0.3.0/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.468706 foambryo-0.3.0/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.481319 foambryo-0.3.0/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12110 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:36:39.177649 foambryo-0.3.1/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12349 2023-07-25 22:36:39.177785 foambryo-0.3.1/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11796 2023-07-25 22:35:49.000000 foambryo-0.3.1/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-07-25 22:24:28.000000 foambryo-0.3.1/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      851 2023-07-25 22:36:39.178408 foambryo-0.3.1/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:36:39.166837 foambryo-0.3.1/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:36:39.174979 foambryo-0.3.1/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-07-25 22:24:28.000000 foambryo-0.3.1/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:36:39.177381 foambryo-0.3.1/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12349 2023-07-25 22:36:39.000000 foambryo-0.3.1/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-25 22:36:39.000000 foambryo-0.3.1/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-25 22:36:39.000000 foambryo-0.3.1/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-25 22:36:39.000000 foambryo-0.3.1/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-25 22:36:39.000000 foambryo-0.3.1/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.3.0/PKG-INFO` & `foambryo-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: foambryo
-Version: 0.3.0
-Summary: Tension inference for 3D cell assemblies
-Home-page: https://github.com/sacha-ichbiah/foambryo
-Author: Sacha Ichbiah
-Author-email: sacha.ichbiah@college-de-france.fr
-License: CC BY-NC-SA 4.0
-Project-URL: Team website, https://www.turlierlab.com/
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # foambryo
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 [![DOI](https://zenodo.org/badge/625305276.svg)](https://zenodo.org/badge/latestdoi/625305276)
 
 **foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
 foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
 If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+
+
 
 
 Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
 
 We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
@@ -68,21 +54,21 @@
 ```shell
 pip install foambryo
 ```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
 
 They minimize, under conservation of volume an energy 
 $\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Young-Dupré Law:** $\gamma_{ij} + \gamma_{ik} + \gamma_{jk} = 0$ .
 - **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
@@ -134,29 +120,30 @@
 
 ---
 ### Biological examples
 #### *P. mammillata* early embryo
 *Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### *C. elegans* early embryo
 *Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
 We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
```

### Comparing `foambryo-0.3.0/README.md` & `foambryo-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: foambryo
+Version: 0.3.1
+Summary: Tension inference for 3D cell assemblies
+Home-page: https://github.com/sacha-ichbiah/foambryo
+Author: Sacha Ichbiah
+Author-email: sacha.ichbiah@college-de-france.fr
+License: CC BY-NC-SA 4.0
+Project-URL: Team website, https://www.turlierlab.com/
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # foambryo
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 [![DOI](https://zenodo.org/badge/625305276.svg)](https://zenodo.org/badge/latestdoi/625305276)
 
 **foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
 foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
 If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+
+
 
 
 Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
 
 We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
@@ -52,21 +70,21 @@
 ```shell
 pip install foambryo
 ```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
 
 They minimize, under conservation of volume an energy 
 $\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Young-Dupré Law:** $\gamma_{ij} + \gamma_{ik} + \gamma_{jk} = 0$ .
 - **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
@@ -118,29 +136,30 @@
 
 ---
 ### Biological examples
 #### *P. mammillata* early embryo
 *Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### *C. elegans* early embryo
 *Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
 We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
```

### Comparing `foambryo-0.3.0/setup.cfg` & `foambryo-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.3.0
+version = 0.3.1
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls =
```

### Comparing `foambryo-0.3.0/src/foambryo/Force_viewer.py` & `foambryo-0.3.1/src/foambryo/Force_viewer.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo/Inference_utilities.py` & `foambryo-0.3.1/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo/Mesh_utilities.py` & `foambryo-0.3.1/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo/Plotting_utilities.py` & `foambryo-0.3.1/src/foambryo/Plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo/Pressure_inference.py` & `foambryo-0.3.1/src/foambryo/Pressure_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo/Tension_inference.py` & `foambryo-0.3.1/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.3.0/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.3.1/src/foambryo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,17 @@
 **foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
 foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
 If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
-<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+
+
 
 
 Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
 
 We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
@@ -68,21 +70,21 @@
 ```shell
 pip install foambryo
 ```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
 
 They minimize, under conservation of volume an energy 
 $\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Young-Dupré Law:** $\gamma_{ij} + \gamma_{ik} + \gamma_{jk} = 0$ .
 - **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
@@ -134,29 +136,30 @@
 
 ---
 ### Biological examples
 #### *P. mammillata* early embryo
 *Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
 We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
 #### *C. elegans* early embryo
 *Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
 Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
 We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="https://github.com/VirtualEmbryo/foambryo/blob/main/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
```

