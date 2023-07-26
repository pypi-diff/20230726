# Comparing `tmp/voyagerpy-0.1.0.tar.gz` & `tmp/voyagerpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyagerpy-0.1.0.tar", max compression
+gzip compressed data, was "voyagerpy-0.1.1.tar", max compression
```

## Comparing `voyagerpy-0.1.0.tar` & `voyagerpy-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     4199 2023-04-26 22:38:47.388221 voyagerpy-0.1.0/README.md
--rw-r--r--   0        0        0      857 2023-04-26 22:38:47.388807 voyagerpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-04-26 22:38:47.389039 voyagerpy-0.1.0/voyagerpy/__init__.py
--rw-r--r--   0        0        0       47 2023-04-24 13:36:12.176202 voyagerpy-0.1.0/voyagerpy/metrics/__init__.py
--rw-r--r--   0        0        0       47 2023-04-24 13:36:12.176359 voyagerpy-0.1.0/voyagerpy/metrics/metrics.py
--rw-r--r--   0        0        0     1019 2023-04-26 22:38:47.389229 voyagerpy-0.1.0/voyagerpy/metrics/univariates.py
--rw-r--r--   0        0        0     2213 2023-04-26 22:38:47.389550 voyagerpy-0.1.0/voyagerpy/plotting/__init__.py
--rw-r--r--   0        0        0      535 2023-04-26 22:38:47.389724 voyagerpy-0.1.0/voyagerpy/plotting/blues_colors.py
--rw-r--r--   0        0        0     1731 2023-04-26 22:38:47.389897 voyagerpy-0.1.0/voyagerpy/plotting/cmap_helper.py
--rw-r--r--   0        0        0      619 2023-04-26 22:38:47.390141 voyagerpy-0.1.0/voyagerpy/plotting/ditto_colors.py
--rw-r--r--   0        0        0    67047 2023-04-26 22:38:47.390519 voyagerpy-0.1.0/voyagerpy/plotting/plot.py
--rw-r--r--   0        0        0     2658 2023-02-07 15:40:49.812108 voyagerpy-0.1.0/voyagerpy/plotting/rectangleplot.py
--rw-r--r--   0        0        0     3858 2023-04-26 22:38:47.390910 voyagerpy-0.1.0/voyagerpy/plotting/roma_colors.py
--rw-r--r--   0        0        0     7683 2023-04-26 22:38:47.391227 voyagerpy-0.1.0/voyagerpy/read.py
--rw-r--r--   0        0        0     1168 2023-04-26 22:38:47.391495 voyagerpy-0.1.0/voyagerpy/spatial/__init__.py
--rw-r--r--   0        0        0     4187 2023-04-26 22:38:47.391718 voyagerpy-0.1.0/voyagerpy/spatial/graphs.py
--rw-r--r--   0        0        0    30857 2023-04-26 22:38:47.392044 voyagerpy-0.1.0/voyagerpy/spatial/spatial.py
--rw-r--r--   0        0        0      782 2023-04-26 22:38:47.392332 voyagerpy-0.1.0/voyagerpy/utils/__init__.py
--rw-r--r--   0        0        0    10687 2023-04-26 22:38:47.393142 voyagerpy-0.1.0/voyagerpy/utils/hvg.py
--rw-r--r--   0        0        0    11932 2023-04-26 22:38:47.393295 voyagerpy-0.1.0/voyagerpy/utils/markers.py
--rw-r--r--   0        0        0     6307 2023-04-26 22:38:47.393609 voyagerpy-0.1.0/voyagerpy/utils/utils.py
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 voyagerpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4199 2023-07-25 21:38:19.279801 voyagerpy-0.1.1/README.md
+-rw-r--r--   0        0        0     1245 2023-07-25 22:10:57.725241 voyagerpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      357 2023-07-25 21:38:19.311164 voyagerpy-0.1.1/voyagerpy/__init__.py
+-rw-r--r--   0        0        0     1284 2023-07-25 21:38:19.311428 voyagerpy-0.1.1/voyagerpy/_core/voyagerpy.py
+-rw-r--r--   0        0        0       47 2023-07-25 21:38:19.311662 voyagerpy-0.1.1/voyagerpy/metrics/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-25 21:38:19.311764 voyagerpy-0.1.1/voyagerpy/metrics/metrics.py
+-rw-r--r--   0        0        0     1019 2023-07-25 21:38:19.312003 voyagerpy-0.1.1/voyagerpy/metrics/univariates.py
+-rw-r--r--   0        0        0     2280 2023-07-25 21:38:19.312269 voyagerpy-0.1.1/voyagerpy/plotting/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-25 21:38:19.312580 voyagerpy-0.1.1/voyagerpy/plotting/blues_colors.py
+-rw-r--r--   0        0        0     1731 2023-07-25 21:38:19.312836 voyagerpy-0.1.1/voyagerpy/plotting/cmap_helper.py
+-rw-r--r--   0        0        0      619 2023-07-25 21:38:19.313210 voyagerpy-0.1.1/voyagerpy/plotting/ditto_colors.py
+-rw-r--r--   0        0        0   109921 2023-07-25 21:38:19.314029 voyagerpy-0.1.1/voyagerpy/plotting/plot.py
+-rw-r--r--   0        0        0     2658 2023-02-07 15:40:49.812108 voyagerpy-0.1.1/voyagerpy/plotting/rectangleplot.py
+-rw-r--r--   0        0        0     3858 2023-07-25 21:38:19.314222 voyagerpy-0.1.1/voyagerpy/plotting/roma_colors.py
+-rw-r--r--   0        0        0     7740 2023-07-25 21:38:19.314564 voyagerpy-0.1.1/voyagerpy/read.py
+-rw-r--r--   0        0        0     1289 2023-07-25 21:38:19.314958 voyagerpy-0.1.1/voyagerpy/spatial/__init__.py
+-rw-r--r--   0        0        0     4928 2023-07-25 21:38:19.315287 voyagerpy-0.1.1/voyagerpy/spatial/graphs.py
+-rw-r--r--   0        0        0    55204 2023-07-25 21:38:19.315705 voyagerpy-0.1.1/voyagerpy/spatial/spatial.py
+-rw-r--r--   0        0        0      814 2023-07-25 21:38:19.315883 voyagerpy-0.1.1/voyagerpy/utils/__init__.py
+-rw-r--r--   0        0        0    12785 2023-07-25 21:38:19.316157 voyagerpy-0.1.1/voyagerpy/utils/hvg.py
+-rw-r--r--   0        0        0    12646 2023-07-25 21:38:19.316510 voyagerpy-0.1.1/voyagerpy/utils/markers.py
+-rw-r--r--   0        0        0    14594 2023-07-25 21:38:19.316800 voyagerpy-0.1.1/voyagerpy/utils/utils.py
+-rw-r--r--   0        0        0     5786 1970-01-01 00:00:00.000000 voyagerpy-0.1.1/PKG-INFO
```

### Comparing `voyagerpy-0.1.0/README.md` & `voyagerpy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/metrics/univariates.py` & `voyagerpy-0.1.1/voyagerpy/metrics/univariates.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/__init__.py` & `voyagerpy-0.1.1/voyagerpy/plotting/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from matplotlib.pyplot import rcParams
 
 from voyagerpy.plotting.cmap_helper import register_listed_cmap, register_segmented_cmap
 from voyagerpy.plotting.plot import (
+    draw_graph,
     elbow_plot,
     grouped_violinplot,
     imshow,
     moran_plot,
     plot_barcode_data,
     plot_barcode_histogram,
     plot_barcodes_bin2d,
@@ -24,23 +25,31 @@
     plot_pca,
     plot_spatial_feature,
     scatter,
     simple_violinplot,
     spatial_reduced_dim,
 )
 
+# https://github.com/cran/RColorBrewer
+from .blues_colors import (
+    blues3,
+    blues4,
+    blues5,
+    blues6,
+    blues7,
+    blues8,
+    blues9,
+)
+
 # https://github.com/dtm2451/dittoSeq
 from .ditto_colors import ditto_colors
 
 # https://github.com/thomasp85/scico
 from .roma_colors import roma_colors
 
-# https://github.com/cran/RColorBrewer
-from .blues_colors import blues3, blues4, blues5, blues6, blues7, blues8, blues9
-
 
 def set_default_cmap(cmap_name: str) -> None:
     rcParams["image.cmap"] = cmap_name
 
 
 register_segmented_cmap("roma", roma_colors, reverse=True)  # type: ignore
 register_segmented_cmap("Blues3", blues3, reverse=False)  # type: ignore
@@ -55,14 +64,15 @@
 register_listed_cmap("dittoseq", ditto_colors, reverse=False) # type: ignore
 set_default_cmap("dittoseq")
 
 __all__ = [
     "elbow_plot",
     "grouped_violinplot",
     "imshow",
+    "draw_graph",
     "moran_plot",
     "plot_barcode_data",
     "plot_barcode_histogram",
     "plot_barcodes_bin2d",
     "plot_bin2d",
     "plot_correlogram",
     "plot_dim_loadings",
```

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/blues_colors.py` & `voyagerpy-0.1.1/voyagerpy/plotting/blues_colors.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/cmap_helper.py` & `voyagerpy-0.1.1/voyagerpy/plotting/cmap_helper.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/ditto_colors.py` & `voyagerpy-0.1.1/voyagerpy/plotting/ditto_colors.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/rectangleplot.py` & `voyagerpy-0.1.1/voyagerpy/plotting/rectangleplot.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/plotting/roma_colors.py` & `voyagerpy-0.1.1/voyagerpy/plotting/roma_colors.py`

 * *Files identical despite different names*

### Comparing `voyagerpy-0.1.0/voyagerpy/read.py` & `voyagerpy-0.1.1/voyagerpy/read.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,37 @@
 
 import h5py
 import pandas as pd
 from anndata import AnnData, read_mtx
 from matplotlib.pyplot import imread
 from .spatial import set_geometry, to_points
 from .utils import get_scale
+import warnings
 
 
-def read_img_data(path: Union[Path, PathLike], adata: AnnData, res: str = "high") -> AnnData:
+def read_img_data(path: Union[Path, PathLike], adata: AnnData, res: str = "hires") -> AnnData:
     path = Path(path)
 
-    loc = "hires" if res == "high" else "lowres"
-    spatial_path = path / "spatial"
-    scalefactors_path = spatial_path / "scalefactors_json.json"
-    img_path = spatial_path / f"tissue_{loc}_image.png"
+    scalefactors_path = path / "scalefactors_json.json"
+    img_path = path / f"tissue_{res}_image.png"
 
-    if img_path.exists() and scalefactors_path.exists():
+    spatial_dict = adata.uns.setdefault("spatial", {})
+
+    if img_path.exists():
         image = imread(str(img_path))
-        adata.uns.setdefault("spatial", {}).setdefault("img", {})
-        adata.uns["spatial"]["img"][loc] = image
-        adata.uns["spatial"]["scale"] = json.load(scalefactors_path.open("rt"))
+        img_dict = spatial_dict.setdefault("img", {})
+        img_dict[res] = image
+    else:
+        warnings.warn(f"Could not find image {img_path}")
+
+    if scalefactors_path.exists():
+        spatial_dict["scale"] = json.load(scalefactors_path.open("rt"))
     else:
-        raise ValueError("Cannot read tissue image or scaling file")
+        warnings.warn(f"Could not find scalefactors_json.json in {scalefactors_path}")
+
     return adata
 
 
 def _read_10x_h5(path: PathLike, symbol_as_index: bool = False, dtype: str = "float64") -> Optional[AnnData]:
     """
     Parameters
     ----------
@@ -196,27 +202,27 @@
 
     """
     path = Path(path)
     adata = read_10x_counts(path, datatype, raw, prefix, symbol_as_index, dtype=dtype)
 
     # spatial
     tissue_pos_path = path / "spatial" / "tissue_positions.csv"
-    tissue_alt_path = tissue_pos_path.with_stem("tissue_positions_list")
+    tissue_alt_path = tissue_pos_path.with_name("tissue_positions_list").with_suffix(".csv")
 
     if tissue_pos_path.exists():
         version = 2
         adata.obs = pd.concat([adata.obs, pd.read_csv(tissue_pos_path).set_index(["barcode"])], axis=1)
     elif tissue_alt_path.exists():
         version = 1
         colnames = ["barcode", "in_tissue", "array_row", "array_col", "pxl_row_in_fullres", "pxl_col_in_fullres"]
         adata.obs = pd.concat([adata.obs, pd.read_csv(tissue_pos_path, header=None, names=colnames).set_index(["barcode"])], axis=1)
     else:
         raise ValueError("Cannot read file tissue_positions.csv")
 
-    adata = read_img_data(path, adata, res=res)
+    adata = read_img_data(path / "spatial", adata, res=res)
     metadata = {
         "data_source": "visium",
         "img_res": [res for res in ("lowres", "hires") if (path / "spatial" / f"tissue_{res}_image.png").exists()],
         "version": version,
     }
     adata.uns["metadata"] = metadata
     return adata
```

### Comparing `voyagerpy-0.1.0/voyagerpy/spatial/__init__.py` & `voyagerpy-0.1.1/voyagerpy/spatial/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from voyagerpy.spatial.graphs import find_visium_graph
+from voyagerpy.spatial.graphs import compute_visium_graph, find_visium_graph
 from voyagerpy.spatial.spatial import (
     apply_transforms,
     cancel_transforms,
     compute_correlogram,
     compute_higher_order_neighbors,
     compute_spatial_lag,
     detect_tissue_threshold,
     get_approx_tissue_boundary,
     get_default_graph,
     get_geom,
     get_spot_coords,
     get_tissue_boundary,
     get_tissue_contour_score,
+    get_visium_spots,
     local_moran,
     losh,
     mirror_img,
     moran,
     rollback_transforms,
     rotate_img90,
     set_default_graph,
@@ -27,23 +28,26 @@
     to_spatial_weights,
 )
 
 __all__ = [
     "apply_transforms",
     "cancel_transforms",
     "compute_correlogram",
+    "compute_visium_graph",
     "compute_higher_order_neighbors",
     "compute_spatial_lag",
     "detect_tissue_threshold",
+    "find_visium_graph",
     "get_approx_tissue_boundary",
     "get_default_graph",
     "get_geom",
     "get_spot_coords",
     "get_tissue_boundary",
     "get_tissue_contour_score",
+    "get_visium_spots",
     "local_moran",
     "losh",
     "mirror_img",
     "moran",
     "rollback_transforms",
     "rotate_img90",
     "set_default_graph",
```

### Comparing `voyagerpy-0.1.0/voyagerpy/utils/__init__.py` & `voyagerpy-0.1.1/voyagerpy/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from voyagerpy.utils.utils import (
     add_per_cell_qcmetrics,
     add_per_gene_qcmetrics,
     get_scale,
     is_highres,
+    is_lowres,
     kurtosis,
     listify,
     log_norm_counts,
     make_unique,
     normalize_csr,
     scale,
 )
@@ -23,14 +24,15 @@
     "find_markers",
     "get_marker_genes",
     "get_p_clusters",
     "get_top_hvgs",
     "get_scale",
     "get_stat_clusters",
     "is_highres",
+    "is_lowres",
     "kurtosis",
     "listify",
     "log_norm_counts",
     "make_unique",
     "model_gene_var",
     "normalize_csr",
     "scale",
```

### Comparing `voyagerpy-0.1.0/voyagerpy/utils/hvg.py` & `voyagerpy-0.1.1/voyagerpy/utils/hvg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
+import warnings
 from math import exp
 
 import numpy as np
 import pandas as pd
 
+from anndata import AnnData
 from scipy.optimize import least_squares
 from scipy import sparse
 from scipy.stats import iqr, norm
 from sklearn.linear_model import LinearRegression
 
 from statsmodels.stats.multitest import fdrcorrection
 from statsmodels.nonparametric.kde import KDEUnivariate
-from scanpy.preprocessing._utils import _get_mean_var
+
+from typing import Optional, Tuple, Union
 
 
 def get_parametric_start(_means, _vars, left_n=100, left_prop=0.1, grid_length=10, b_grid_range=5, n_grid_max=10):
     """Get initial guess of parameters a,b,n in for for nonlinear optimization of function f.
 
     Parameters
     ----------
@@ -58,35 +61,38 @@
     x = _means[keep]
     lm = LinearRegression(fit_intercept=False)
     grad = lm.fit(x.reshape(-1, 1), y).coef_[0]
 
     b_grid_pts = 2 ** np.linspace(-b_grid_range, b_grid_range, n_grid_max)
     n_grid_pts = 2 ** np.linspace(0, n_grid_max, grid_length)
     hits = np.array([(x, y) for x in b_grid_pts for y in n_grid_pts], dtype=np.float64)
-
-    possible_vals = np.apply_along_axis(lambda x: sum((_vars - (1.13 * x[0] * _means) / ((_means ** x[1]) + x[0] + 0.001)) ** 2), 1, hits)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        possible_vals = np.apply_along_axis(
+            lambda x: sum((_vars - (1.13 * x[0] * _means) / ((_means ** x[1]) + x[0] + 0.001)) ** 2), 1, hits
+        )
 
     min_ind = np.argmin(possible_vals)
     b_start = np.log(hits[min_ind][0])
     n_start = np.log(max(1e-8, hits[min_ind][1] - 1))
     a_start = np.log(grad * hits[min_ind][0])
 
     return a_start, b_start, n_start
 
 
-def inverse_density_weights(x, adjust=1):
+def inverse_density_weights(x: np.ndarray, adjust: int = 1):
     """\
     Calculate inverse density weights for data x.
 
     Parameters
     ----------
     x : ndarray
         Array of points, in this case means.
     adjust : int, optional
-        DESCRIPTION. The default is 1.
+        Currently not used. The default is 1.
 
     Raises
     ------
     Exception
         Fail if zero length of means.
 
     Returns
@@ -258,17 +264,16 @@
         return x[n]
     else:
         return (x[n] + x[n + 1]) / 2
 
     # return n
 
 
-def decompose_log_exprs(_means, _vars, fit_means, fit_vars, names=None):
-    """\
-    Decompose the variance into technical and biological.
+def decompose_log_exprs(_means, _vars, fit_means, fit_vars, names=None) -> pd.DataFrame:
+    """Decompose the variance into technical and biological variance.
 
     Parameters
     ----------
     _means : ndarray
         Means.
     _vars : ndarray
         Variances.
@@ -285,33 +290,71 @@
         Returns dataframe with relevant columns.
 
     """
     fit, std_dev = fit_trend_var(fit_means, fit_vars)
 
     output = pd.DataFrame({"mean": _means, "total": _vars, "tech": fit(_means)}, index=names)
     output["bio"] = output["total"] - output["tech"]
-    output["p_value"] = 1 - norm.cdf(output["bio"] / output["tech"], scale=std_dev)
-    filt_out = output[~output["p_value"].isna()]
-    # filt_out["FDR"] = fdrcorrection(filt_out["p_value"])[1]
-    _, pval_corr = fdrcorrection(filt_out["p_value"])
+    output["p.value"] = 1 - norm.cdf(output["bio"] / output["tech"], scale=std_dev)
+    filt_out = output[~output["p.value"].isna()]
+    # filt_out["FDR"] = fdrcorrection(filt_out["p.value"])[1]
+    _, pval_corr = fdrcorrection(filt_out["p.value"])
     output.loc[filt_out.index, "FDR"] = pval_corr
 
     return output
     # 1 - norm().cdf(0.1)
 
 
-def model_gene_var(adata, block=None, design=None, subset_row=None, subset_fit=None, gene_names=None):
+def get_mean_var(X: Union[np.ndarray, sparse.csr_matrix, sparse.csc_matrix], axis=0, ddof=1) -> Tuple[np.ndarray, np.ndarray]:
     """\
-    Return the modelled gene variance.
+    Calculate mean and variance of X.
+
+    Parameters
+    ----------
+    X : Union[np.ndarray, sparse.csr_matrix, sparse.csc_matrix]
+        The array to compute the mean and variance over.
+    axis : int, optional
+        Axis to calculate mean and variance. The default is 0.
+
+    Returns
+    -------
+    mean : ndarray
+        Mean of X over axis.
+    var : ndarray
+        Variance of X over axis.
+
+    """
+    if sparse.issparse(X):
+        mean = X.mean(axis=axis).A.reshape(-1)
+        var = X.A.var(axis=axis, ddof=ddof)
+    else:
+        mean = X.mean(axis=axis).reshape(-1)
+        var = X.var(axis=axis, ddof=ddof)
+
+    return mean.squeeze(), var.squeeze()
+
+
+def model_gene_var(
+    adata: AnnData,
+    block=None,
+    design=None,
+    subset_row=None,
+    subset_fit=None,
+    gene_names=None,
+    layer: Optional[str] = None,
+    ddof: int = 1,
+) -> pd.DataFrame:
+    """Return the modelled gene variance.
 
     Modelled on similar method in SCRAN package.
+
     Parameters
     ----------
     adata : AnnData
-        DESCRIPTION.
+        The annotated data matrix.
     block : None, optional
         Compatibility with R. The default is None.
     design : None, optional
         Compatibility with R. The default is None.
     subset_row : ndarray, optional
         If only a subset of the rows are used. The default is None.
     subset_fit : bool, optional
@@ -320,22 +363,33 @@
         If gene names are provided. The default is None.
 
     Returns
     -------
     collected : DataFrame
         Information on modelled variance into biological and technical.
 
+    Note
+    ----
+    The following parameters are not implemented:
+        - block
+        - design
+        - subset_row
+        - subset_fit
     """
-    if sparse.issparse(adata):
-        x_means, x_vars = _get_mean_var(adata, axis=0)
-        names = gene_names
+
+    if isinstance(adata, AnnData):
+        X = adata.X if layer is None else adata.layers[layer]
+        names = adata.var_names
     else:
-        x_means, x_vars = _get_mean_var(adata.X, axis=0)
-        names = adata.var.index
-    # decompose_log_exprs(x_means, x_vars)
+        X = adata
+        names = gene_names
+
+    del adata
+    x_means, x_vars = get_mean_var(X, axis=0, ddof=ddof)
+
     if subset_fit is None:
         fit_stats_means = x_means
         fit_stats_vars = x_vars
     else:
         return None
 
     collected = decompose_log_exprs(x_means, x_vars, fit_stats_means, fit_stats_vars, names=names)
@@ -387,19 +441,45 @@
     if parametric:
         a_start, b_start, n_start = get_parametric_start(m, v)
         a, b, n = parametric_fit(m, v, w, [a_start, b_start, n_start])
         # to_fit = to_fit - np.log(f(m, a, b, n))
         PARAMFUN = lambda x: f_predict(x, a, b, n)
         # return PARAMFUN
 
+    UNSCALEDFUN = PARAMFUN
     if lowess:
         # idx = np.round(np.linspace(0, len(m) - 1, 200)).astype(int)
         # ll = lowess(to_fit, exog=m, xvals=idx, resid_weights=w)
-        pass
-    else:
-        UNSCALEDFUN = PARAMFUN
+        warnings.warn("Lowess not implemented.")
+
     fit, std_dev = correct_logged_expectation(m, v, w, UNSCALEDFUN)
     return fit, std_dev
 
 
-def get_top_hvgs(stats, n=2000, stat="bio", var_threshold=0):
-    return np.array(stats.nlargest(n, "bio").index, dtype="str")
+def get_top_hvgs(stats: pd.DataFrame, n: int = 2000, stat: str = "bio", var_threshold: float = 0) -> np.ndarray:
+    """Get the `n` genes with the largest biological variance.
+
+    Parameters
+    ----------
+    stats : pd.DataFrame
+        The stats dataframe. Computed via `model_gene_var`.
+    n : int, optional
+        The number of genes to return, by default 2000
+    stat : str, optional
+        The statistic to use for getting the `n` largest values, by default "bio".
+    var_threshold : float, optional
+        The variance threshold to use. This parameter is not used, by default 0.
+
+    Returns
+    -------
+    np.ndarray
+        An array of gene names with the largest statistic specified.
+
+    Note
+    ----
+    The `var_threshold` parameter is not used. It is included for compatibility with the R implementation.
+
+    See also
+    --------
+    :py:func:`model_gene_var`
+    """
+    return np.array(stats.nlargest(n, stat).index, dtype="str")
```

### Comparing `voyagerpy-0.1.0/voyagerpy/utils/markers.py` & `voyagerpy-0.1.1/voyagerpy/utils/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,35 @@
 
     return p_vals, test_stat, effect_size
 
 
 def get_p_clusters(
     adata: AnnData, clust: Union[str, int], skip_precalc: bool = False, pval_type: str = "all", cluster: str = "cluster"
 ) -> Union[DataFrame, ndarray]:
+    """Get the p values for a given cluster.
+
+    Parameters
+    ----------
+    adata : AnnData
+        Annotation data matrix.
+    clust : Union[str, int]
+        The cluster to test against all other clusters.
+    skip_precalc : bool, optional
+        Skip pre calculations, by default False
+    pval_type : str, optional
+        The p-value type, by default "all"
+    cluster : str, optional
+        The column name containing the clusters, by default "cluster"
+
+    Returns
+    -------
+    Union[DataFrame, ndarray]
+        Dataframe of p-values for each gene, or array of p-values for each gene.
+    """
+    # TODO: Add better documentation.
     # rows = adata.X.shape[0]
     pval_arrs = []
     # nr_clust = adata.obs["cluster"].cat.codes
     colnames = []
     if skip_precalc:
         first = False
         skip_index = None
@@ -294,15 +315,15 @@
         index_of_maxs = stat_dict["p_values"].columns.get_indexer(stat_dict["p_values"].idxmax(axis=1))
         stat_dict["effect_size"]
         sort_order = np.argsort(pval_max)
         es = np.array(stat_dict["effect_size"])[np.arange(len(stat_dict["effect_size"])), index_of_maxs]
         res[f"{cluster}_{i}"] = pd.DataFrame(
             {"p_vals": pval_max[sort_order], "FDR": p_adjust_bh(pval_max)[sort_order], "summary_es": es[sort_order]},
             index=np.array(pval_max[sort_order].index, dtype=str),
-        )
+        ).rename(columns={"summary_es": "summary.AUC", "p_vals": "p.value"})
 
     return res
 
 
 # taken from https://stackoverflow.com/questions/7450957/how-to-implement-rs-p-adjust-in-python/33532498#33532498
 def p_adjust_bh(p):
     """Benjamini-Hochberg p-value correction for multiple hypothesis testing."""
```

### Comparing `voyagerpy-0.1.0/PKG-INFO` & `voyagerpy-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: voyagerpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for Voyager, the geo-spatialist R library.
 Home-page: https://pmelsted.github.io/voyagerpy
 License: BSD-3-Clause
 Keywords: Single-Cell,Spatial,voyager
 Author: Pall Melsted
 Author-email: pmelsted@hi.is
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anndata (>=0.6.22)
-Requires-Dist: geopandas (>=0.12)
+Provides-Extra: notebooks
+Requires-Dist: anndata (>=0.8)
+Requires-Dist: esda (>=2.4.3,<3.0.0)
+Requires-Dist: fiona (>=1.9,<2.0)
+Requires-Dist: geopandas (>=0.13,<0.14)
+Requires-Dist: h5py (>=3.0,<4.0)
+Requires-Dist: igraph (>=0.10.4) ; extra == "notebooks"
+Requires-Dist: leidenalg (>=0.9.1,<0.10.0) ; extra == "notebooks"
+Requires-Dist: libpysal (>=4.7.0,<5.0.0)
 Requires-Dist: matplotlib (>=3.6,<3.7)
 Requires-Dist: networkx (>=3.0)
-Requires-Dist: numpy (>=1.23)
-Requires-Dist: opencv-python (>=4.7)
-Requires-Dist: scipy (>=1.9)
-Requires-Dist: seaborn (>=0.12)
-Requires-Dist: shapely (>=1.8.5)
+Requires-Dist: numpy (>=1.22,<1.24)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: scanpy (>=1.9.3,<2.0.0) ; extra == "notebooks"
+Requires-Dist: scikit-learn (>=1.2)
+Requires-Dist: scipy (>=1.10) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: shapely (>=1.7)
+Requires-Dist: statsmodels (>=0.13)
 Project-URL: Bug Tracker, https://github.com/pmelsted/voyagerpy/issues
 Project-URL: Repository, https://github.com/pmelsted/voyagerpy
 Description-Content-Type: text/markdown
 
 # VoyagerPy
 
 This repo manages the VoyagerPy Python package, a Python implementation of the R package [Voyager](https://github.com/pachterlab/voyager)
```

