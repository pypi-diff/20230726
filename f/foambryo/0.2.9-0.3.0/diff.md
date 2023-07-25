# Comparing `tmp/foambryo-0.2.9.tar.gz` & `tmp/foambryo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-tly5_f6v/foambryo-0.2.9.tar", last modified: Mon Jul 17 10:47:15 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-dggk_44j/foambryo-0.3.0.tar", last modified: Tue Jul 25 22:28:24 2023, max compression
```

## Comparing `foambryo-0.2.9.tar` & `foambryo-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.291154 foambryo-0.2.9/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11201 2023-07-17 10:47:15.291274 foambryo-0.2.9/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.9/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.9/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      851 2023-07-17 10:47:15.292110 foambryo-0.2.9/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.280659 foambryo-0.2.9/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.288269 foambryo-0.2.9/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.9/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.9/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.9/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.290804 foambryo-0.2.9/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11201 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.481934 foambryo-0.3.0/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12110 2023-07-25 22:28:24.482112 foambryo-0.3.0/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11557 2023-07-25 22:26:11.000000 foambryo-0.3.0/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-07-25 22:24:28.000000 foambryo-0.3.0/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      851 2023-07-25 22:28:24.483620 foambryo-0.3.0/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.452952 foambryo-0.3.0/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.468706 foambryo-0.3.0/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-07-25 22:24:28.000000 foambryo-0.3.0/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-25 22:28:24.481319 foambryo-0.3.0/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12110 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-25 22:28:24.000000 foambryo-0.3.0/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.9/PKG-INFO` & `foambryo-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-Metadata-Version: 2.1
-Name: foambryo
-Version: 0.2.9
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
+# foambryo
 
-### foambryo
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
+[![DOI](https://zenodo.org/badge/625305276.svg)](https://zenodo.org/badge/latestdoi/625305276)
 
-**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
+**foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
-Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
-Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
+Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
+If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
+<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
 
+Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
 
-We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
+We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
-### Example 
+### Quick start example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
 pip install foambryo
 ```
 
@@ -56,59 +45,63 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install foambryo
+```shell
+pip install foambryo
+```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+
+They minimize, under conservation of volume an energy 
+$\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
-They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
-- **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
+- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
-#### 1 - Creating a Mesh object
+#### 1 - Loading a multimaterial mesh
 The first step is to load your multimaterial mesh into a `DCEL_Data` object via the builder `DCEL_Data(Verts, Faces_multimaterial)`. 
-    - `Verts` is an V x 3 numpy array of vertex positions
+    - `Verts` is an V x 3 Numpy array of vertex positions
     - `Faces_multimaterial` is an F x 5 numpy array of face and material indices, where at each row the 3 first indices refers to a vertex and the 2 last refer to a given material, 0 being the exterior media
 
-#### 2 - Infer the forces
+#### 2 - Infer tensions and pressures
  Then the second step is to use this `Mesh` object to infer the tensions and pressions
 - `infer_tension(Mesh,mean_tension=1,mode='YD')`: 
-We infer tensions ratios by inverting junctional equilibrium relations
+We infer relative tensions by inverting junctional equilibrium relations
     - `Mesh` is a `DCEL_Data` object
     - `mean_tension` has to be defined as we only infer ratio between tensions
     - `mode` is the formula used to infer the tensions. It has to be choosen among: `YD`, `Eq`, `Projection_YD`,  `cotan`, `inv_cotan`, `Lamy`, `inv_Lamy`, `Lamy_Log`, `Variational`
 
 - `infer_pressures(Mesh,dict_tensions,mode='Variational', P0 = 0)`: 
-We infer relative pressures by inverting membrane equilibrium relation
+We infer pressures relative to the exterior (of zero pressure) by inverting membrane equilibrium relation
     - `Mesh` is a `DCEL_Data` object
     -  `dict_tensions` is the dictionnary obtained with `infer_tension`
     - `P0` has to be defined as we only infer relative pressures
     - `mode` is the formula used to infer the pressures. It has to be choosen among: `Variational`, `Laplace`
 
 #### 3 - Visualize
 
-This package is then built around several functions, each of them taking as an entry a `Mesh` object: 
+The viewer part of the package is built around several functions, each of them taking as an entry a `Mesh` object: 
 - `plot_tension_inference(Mesh,dict_tensions=None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions by inverting Young-Dupré relations
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
     - `alpha` : p_value threshold when displaying values: Values beyond the alpha and 1-alpha quantiles are clipped 
-    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
+    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, Gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
     - `scattered`: scattered view of the mesh
     - `scatter_coeff`: amount of displacement if scattered is activated
 
  
 - `plot_force_inference(Mesh,dict_tensions = None, dict_pressure = None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions, pressures and principal directions of the stress tensor
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
@@ -119,37 +112,35 @@
     - `scatter_coeff`: amount of displacement if scattered is activated
  
 - `plot_valid_junctions(Mesh)`: Valid junctions are plotted in green, and unstable junctions are plotted in red. This is used to assess the validity of the inference
     - `Mesh` is a `DCEL_Data` object
 
 
 
-
-
 ---
-### Biological use-cases
-#### Phallusia mammillata
-Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
-We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
+### Biological examples
+#### *P. mammillata* early embryo
+*Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
+We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
-#### C.elegans, constrained within a shell
-Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
+#### *C. elegans* early embryo
+*Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
-Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
-We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
+Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
+We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -173,10 +164,17 @@
 	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+### License
 
+This work is licensed under a
+[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
 
+[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
+[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
+[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
```

### Comparing `foambryo-0.2.9/README.md` & `foambryo-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,45 @@
-### foambryo
+Metadata-Version: 2.1
+Name: foambryo
+Version: 0.3.0
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
 
-**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
+# foambryo
 
-Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
-Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
+[![DOI](https://zenodo.org/badge/625305276.svg)](https://zenodo.org/badge/latestdoi/625305276)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+**foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
+Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
+foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
+If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
+<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
-We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
+
+Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
+
+We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
-### Example 
+### Quick start example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
 pip install foambryo
 ```
 
@@ -40,59 +61,63 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install foambryo
+```shell
+pip install foambryo
+```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+
+They minimize, under conservation of volume an energy 
+$\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
-They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
-- **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
+- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
-#### 1 - Creating a Mesh object
+#### 1 - Loading a multimaterial mesh
 The first step is to load your multimaterial mesh into a `DCEL_Data` object via the builder `DCEL_Data(Verts, Faces_multimaterial)`. 
-    - `Verts` is an V x 3 numpy array of vertex positions
+    - `Verts` is an V x 3 Numpy array of vertex positions
     - `Faces_multimaterial` is an F x 5 numpy array of face and material indices, where at each row the 3 first indices refers to a vertex and the 2 last refer to a given material, 0 being the exterior media
 
-#### 2 - Infer the forces
+#### 2 - Infer tensions and pressures
  Then the second step is to use this `Mesh` object to infer the tensions and pressions
 - `infer_tension(Mesh,mean_tension=1,mode='YD')`: 
-We infer tensions ratios by inverting junctional equilibrium relations
+We infer relative tensions by inverting junctional equilibrium relations
     - `Mesh` is a `DCEL_Data` object
     - `mean_tension` has to be defined as we only infer ratio between tensions
     - `mode` is the formula used to infer the tensions. It has to be choosen among: `YD`, `Eq`, `Projection_YD`,  `cotan`, `inv_cotan`, `Lamy`, `inv_Lamy`, `Lamy_Log`, `Variational`
 
 - `infer_pressures(Mesh,dict_tensions,mode='Variational', P0 = 0)`: 
-We infer relative pressures by inverting membrane equilibrium relation
+We infer pressures relative to the exterior (of zero pressure) by inverting membrane equilibrium relation
     - `Mesh` is a `DCEL_Data` object
     -  `dict_tensions` is the dictionnary obtained with `infer_tension`
     - `P0` has to be defined as we only infer relative pressures
     - `mode` is the formula used to infer the pressures. It has to be choosen among: `Variational`, `Laplace`
 
 #### 3 - Visualize
 
-This package is then built around several functions, each of them taking as an entry a `Mesh` object: 
+The viewer part of the package is built around several functions, each of them taking as an entry a `Mesh` object: 
 - `plot_tension_inference(Mesh,dict_tensions=None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions by inverting Young-Dupré relations
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
     - `alpha` : p_value threshold when displaying values: Values beyond the alpha and 1-alpha quantiles are clipped 
-    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
+    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, Gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
     - `scattered`: scattered view of the mesh
     - `scatter_coeff`: amount of displacement if scattered is activated
 
  
 - `plot_force_inference(Mesh,dict_tensions = None, dict_pressure = None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions, pressures and principal directions of the stress tensor
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
@@ -103,37 +128,35 @@
     - `scatter_coeff`: amount of displacement if scattered is activated
  
 - `plot_valid_junctions(Mesh)`: Valid junctions are plotted in green, and unstable junctions are plotted in red. This is used to assess the validity of the inference
     - `Mesh` is a `DCEL_Data` object
 
 
 
-
-
 ---
-### Biological use-cases
-#### Phallusia mammillata
-Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
-We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
+### Biological examples
+#### *P. mammillata* early embryo
+*Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
+We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
-#### C.elegans, constrained within a shell
-Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
+#### *C. elegans* early embryo
+*Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
-Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
-We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
+Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
+We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -157,10 +180,17 @@
 	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+### License
 
+This work is licensed under a
+[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
 
+[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
+[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
+[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
```

### Comparing `foambryo-0.2.9/setup.cfg` & `foambryo-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.2.9
+version = 0.3.0
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls = 
@@ -22,15 +22,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.21.6
 	polyscope>=1.2.0
 	scipy>=1.4.1
-	delaunay-watershed-3d>=0.2.5
+	delaunay-watershed-3d>=0.2.8
 	networkx>=2.5.1
 	matplotlib>=3.3.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `foambryo-0.2.9/src/foambryo/Force_viewer.py` & `foambryo-0.3.0/src/foambryo/Force_viewer.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo/Inference_utilities.py` & `foambryo-0.3.0/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo/Mesh_utilities.py` & `foambryo-0.3.0/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo/Plotting_utilities.py` & `foambryo-0.3.0/src/foambryo/Plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo/Pressure_inference.py` & `foambryo-0.3.0/src/foambryo/Pressure_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo/Tension_inference.py` & `foambryo-0.3.0/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.9/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.3.0/src/foambryo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.9
+Version: 0.3.0
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-### foambryo
+# foambryo
 
-**foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
+[![DOI](https://zenodo.org/badge/625305276.svg)](https://zenodo.org/badge/latestdoi/625305276)
 
-Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
-Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
+**foambryo** is a python package based on Polyscope designed to infer relative surface tensions, cell pressures and cell stress tensors from the geometry of foam-like cell clusters, such as early-embryos, many tissues and stem-cell derived organoids and embryoids.
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
+Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. Mechanics is at the heart of the development of these structures, yet tools to investigate the forces at play in 3D remain scarse. Inferring forces or stresses from cell shapes allows allows one to reveal the fundamental mechanics shaping cells. This software makes the classical hypothesis that cells in many embryos, tissues or aggregates are akin to heterogeneous foam-like structures (see [Physical model](README.md/#Physical-model)).
 
+foambryo was created by Sacha Ichbiah during his PhD in [Turlier Lab](https://www.turlierlab.com), and is maintained by Sacha Ichbiah and Hervé Turlier. For support, please open an issue.
+If you use this library in your work please cite the [paper](https://doi.org/10.1101/2023.04.12.536641).
 
+<img src="Images_github_repo/Window_76_cells.png" alt="drawing" width="650"/>
 
 
-We rely on **delaunay-watershed**, a tool we designed to reconstruct efficiently multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junctional angles and surfaces curvatures, and invert **Young-Dupré** and **Laplace** laws, to find back the physical parameters involved in the mechanical equilibrium: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
+Foambryo requires the prior segmentation of the aggregate into cell segmentation mask images using your favorite algorithm (watershed, [cellpose](https://www.cellpose.org) or others)
+
+We rely on our companion tool [**delaunay-watershed**](https://github.com/VirtualEmbryo/delaunay-watershed) to construct precise multimaterial meshes from instance segmentations. From these multimaterial meshes, we can efficiently and robustly extract junction angles and interface curvatures, and invert the **Young-Dupré** and **Laplace** laws, to retrieve the fundamental forces involved in the mechanical equilibrium of foam-like cell aggregates: **surface tensions** $\gamma_{ij}$ and **cell pressures** $p_i$.
 
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
-### Example 
+### Quick start example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
 pip install foambryo
 ```
 
@@ -56,59 +61,63 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install foambryo
+```shell
+pip install foambryo
+```
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
+<img src="Images_github_repo/Equilibrium.png" alt="drawing" width="175"/>
+
+They minimize, under conservation of volume an energy 
+$\mathcal{E}=\underset{ij}{\sum}\gamma_{ij}$.
 
-They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
 The two main laws involved are: 
-- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$
-- **Laplace Law:** $P_j - P_i = 2 \gamma_{ij} h_{ij}$ where $h_{ij}$ is the mean curvature of the interface between the cell i and j. `
+- **Young-Dupré Law:** $\vec{\gamma}_{ij} + \vec{\gamma}_{ik} + \vec{\gamma}_{jk} = \vec{0}$ .
+- **Laplace Law:** $p_j - p_i = 2 \gamma_{ij} H_{ij}$ where $H_{ij}$ is the mean curvature of the interface between the cell i and j.
 
 
 ---
 
 ### API and Documentation
 
-#### 1 - Creating a Mesh object
+#### 1 - Loading a multimaterial mesh
 The first step is to load your multimaterial mesh into a `DCEL_Data` object via the builder `DCEL_Data(Verts, Faces_multimaterial)`. 
-    - `Verts` is an V x 3 numpy array of vertex positions
+    - `Verts` is an V x 3 Numpy array of vertex positions
     - `Faces_multimaterial` is an F x 5 numpy array of face and material indices, where at each row the 3 first indices refers to a vertex and the 2 last refer to a given material, 0 being the exterior media
 
-#### 2 - Infer the forces
+#### 2 - Infer tensions and pressures
  Then the second step is to use this `Mesh` object to infer the tensions and pressions
 - `infer_tension(Mesh,mean_tension=1,mode='YD')`: 
-We infer tensions ratios by inverting junctional equilibrium relations
+We infer relative tensions by inverting junctional equilibrium relations
     - `Mesh` is a `DCEL_Data` object
     - `mean_tension` has to be defined as we only infer ratio between tensions
     - `mode` is the formula used to infer the tensions. It has to be choosen among: `YD`, `Eq`, `Projection_YD`,  `cotan`, `inv_cotan`, `Lamy`, `inv_Lamy`, `Lamy_Log`, `Variational`
 
 - `infer_pressures(Mesh,dict_tensions,mode='Variational', P0 = 0)`: 
-We infer relative pressures by inverting membrane equilibrium relation
+We infer pressures relative to the exterior (of zero pressure) by inverting membrane equilibrium relation
     - `Mesh` is a `DCEL_Data` object
     -  `dict_tensions` is the dictionnary obtained with `infer_tension`
     - `P0` has to be defined as we only infer relative pressures
     - `mode` is the formula used to infer the pressures. It has to be choosen among: `Variational`, `Laplace`
 
 #### 3 - Visualize
 
-This package is then built around several functions, each of them taking as an entry a `Mesh` object: 
+The viewer part of the package is built around several functions, each of them taking as an entry a `Mesh` object: 
 - `plot_tension_inference(Mesh,dict_tensions=None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions by inverting Young-Dupré relations
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
     - `alpha` : p_value threshold when displaying values: Values beyond the alpha and 1-alpha quantiles are clipped 
-    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
+    - `scalar_quantities`: plot of vertex volume and area derivatives, of mean, Gaussian curvatures, and principal curvatures discrepancy. Can be quite long for big meshes
     - `scattered`: scattered view of the mesh
     - `scatter_coeff`: amount of displacement if scattered is activated
 
  
 - `plot_force_inference(Mesh,dict_tensions = None, dict_pressure = None,alpha = 0.05, scalar_quantities = False, scattered = False, scatter_coeff=0.2)`: Which plots surface tensions, pressures and principal directions of the stress tensor
     - `Mesh` is a `DCEL_Data` object
     - `dict_tensions` is the dictionnary obtained with `infer_tension`, and is computed automatically if unspecified. 
@@ -119,37 +128,35 @@
     - `scatter_coeff`: amount of displacement if scattered is activated
  
 - `plot_valid_junctions(Mesh)`: Valid junctions are plotted in green, and unstable junctions are plotted in red. This is used to assess the validity of the inference
     - `Mesh` is a `DCEL_Data` object
 
 
 
-
-
 ---
-### Biological use-cases
-#### Phallusia mammillata
-Phallusia mammillata is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
-We use data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
+### Biological examples
+#### *P. mammillata* early embryo
+*Phallusia mammillata* is a solitary marine tunicate of the ascidian class known for its stereotypical development. As the embryo develops freely, without any constraint, we can do a full force inference and infer its tensions, pressures and stresses.
+We use segmentation data from [Guignard, L., Fiúza, U. et al.](https://www.science.org/doi/10.1126/science.aar5663)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/Ascidians.png" alt="drawing" width="900"/>
 
 
-#### C.elegans, constrained within a shell
-Caenorhabditis elegans is a widely studied model organism, with one of the most reproducible development. This earthworm is developing in a shell. As the shell topology is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to deduce the surface tensions of the membranes. We use data from the [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
+#### *C. elegans* early embryo
+*Caenorhabditis elegans* is a widely studied model organism, with one of the most reproducible development. The embryo of this earthworm is developing within a shell. As the shell shape and mechanics is unknown, the pressures are not accessible. However we can still use Young-Dupré relationships to retrieve surface tensions at cell membranes. Here we use segmentation data from [Cao, J., Guan, G., Ho, V.W.S. et al.](https://doi.org/10.1038/s41467-020-19863-x)
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/CElegans.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/CElegans.png" alt="drawing" width="900"/>
 
 #### View scalar quantities on surface meshes
 
-Gaussian and mean curvature can be plotted on our meshes, and are useful to study the properties of surfaces obtained from simulations. 
-We also plot the vertex area and volume derivatives, that appears in our variational formulas, the difference between the two principal curvatures and the sphere-fit residual that can be used to detect robust non-spherical CMC surfaces (see our paper for more details)
+Gaussian and mean curvature can be plotted on our meshes, and may be useful to study the geometric properties of interfaces between cells. 
+We can also plot the vertex area and volume derivatives, that appear in our variational formulas, the difference between the two principal curvatures and the residual of the best sphere-fit that can be used to detect non-spherical constant-mean-curvature surfaces.
 They can be obtained by putting the option `scalar_quantities = True` when viewing the forces. 
 
-<img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
+<img src="Images_github_repo/scalar_quantities.png" alt="drawing" width="900"/>
 
 - Gaussian Curvature is computed using the angle defect formula.
 - Mean Curvature is computed using the cotan formula.
 
 To see the code of each of these use-cases, please load the associated jupyter notebooks in the folder Notebooks
 
 ---
@@ -173,10 +180,17 @@
 	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+### License
 
+This work is licensed under a
+[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
+[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
 
+[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
+[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
+[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
```

