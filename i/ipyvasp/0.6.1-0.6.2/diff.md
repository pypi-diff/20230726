# Comparing `tmp/ipyvasp-0.6.1.tar.gz` & `tmp/ipyvasp-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.6.1.tar", last modified: Mon Jul 10 18:46:45 2023, max compression
+gzip compressed data, was "ipyvasp-0.6.2.tar", last modified: Wed Jul 26 19:37:55 2023, max compression
```

## Comparing `ipyvasp-0.6.1.tar` & `ipyvasp-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.455264 ipyvasp-0.6.1/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     1862 2023-07-10 18:46:45.454265 ipyvasp-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.425717 ipyvasp-0.6.1/ipyvasp/
--rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.6.1/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.1/ipyvasp/__main__.py
--rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.1/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    93200 2023-07-05 18:49:40.000000 ipyvasp-0.6.1/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0       23 2023-07-10 18:46:22.000000 ipyvasp-0.6.1/ipyvasp/_version.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.1/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     3335 2023-07-10 18:45:22.000000 ipyvasp-0.6.1/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.453265 ipyvasp-0.6.1/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.1/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.1/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.6.1/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.6.1/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.1/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.1/ipyvasp/evals_dataframe.py
--rw-rw-rw-   0        0        0    22397 2023-07-04 23:42:24.000000 ipyvasp-0.6.1/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.1/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.1/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    15225 2023-07-10 18:26:17.000000 ipyvasp-0.6.1/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.1/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.448205 ipyvasp-0.6.1/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      203 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 18:46:45.455264 ipyvasp-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.096475 ipyvasp-0.6.2/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-07-26 19:37:55.095475 ipyvasp-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.066924 ipyvasp-0.6.2/ipyvasp/
+-rw-rw-rw-   0        0        0     1838 2023-07-24 19:58:23.000000 ipyvasp-0.6.2/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.2/ipyvasp/__main__.py
+-rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.2/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    97706 2023-07-26 19:34:10.000000 ipyvasp-0.6.2/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-07-26 19:37:09.000000 ipyvasp-0.6.2/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.2/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     3866 2023-07-26 16:58:27.000000 ipyvasp-0.6.2/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.094497 ipyvasp-0.6.2/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.2/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.2/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34192 2023-07-24 20:25:24.000000 ipyvasp-0.6.2/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    30507 2023-07-24 19:55:30.000000 ipyvasp-0.6.2/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.2/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.2/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    23229 2023-07-26 18:04:39.000000 ipyvasp-0.6.2/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.2/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.2/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15225 2023-07-10 18:26:17.000000 ipyvasp-0.6.2/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.2/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.089394 ipyvasp-0.6.2/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      203 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:37:55.096475 ipyvasp-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.2/setup.py
```

### Comparing `ipyvasp-0.6.1/LICENSE` & `ipyvasp-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/PKG-INFO` & `ipyvasp-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.1
+Version: 0.6.2
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.1/README.md` & `ipyvasp-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/__init__.py` & `ipyvasp-0.6.2/ipyvasp/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     plt2text,
     plt2html,
     iplot2html,
     iplot2widget,
     webshow,
 )
 
+show = plot_toolkit.plt.show  # for convenience (and already imported)
+savefig = plot_toolkit.plt.savefig  # for convenience
+
 version = __version__
 # Set global matplotlib settings for notebook.
 from cycler import cycler as __cycler
 
 global_matplotlib_settings(
     {
         "figure.dpi": 144,  # Better to See
@@ -59,8 +62,8 @@
                 "#FF6692",
                 "#B6E880",
                 "#FF97FF",
                 "#FECB52",
             ]
         ),
     }
-)
+)
```

### Comparing `ipyvasp-0.6.1/ipyvasp/_enplots.py` & `ipyvasp-0.6.2/ipyvasp/_enplots.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/_lattice.py` & `ipyvasp-0.6.2/ipyvasp/_lattice.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,22 +198,23 @@
 
     for i, j in inds:
         array[i] = _copy_array[j]
         names[i] = _copy_names[j]
 
     array = np.reshape(array, (10, 18, 3))
     names = np.reshape(names, (10, 18))
-    ax = ptk.get_axes((9, 4.5))
+    ax = ptk.get_axes((8, 4.5))
     ax.imshow(array)
 
     for i in range(18):
         for j in range(10):
             c = "k" if np.linalg.norm(array[j, i]) > 1 else "w"
             plt.text(i, j, names[j, i], color=c, ha="center", va="center")
     ax.set_axis_off()
+    plt.tight_layout(pad=0.5)
     return ax
 
 
 def write_poscar(poscar_data, outfile=None, selective_dynamics=None, overwrite=False):
     """Writes POSCAR data to a file or returns string
 
     Parameters
@@ -2269,14 +2270,18 @@
     You may find errors due to missing atoms in the new basis, use `zoom` to increase the size of given cell to include any possible site in new cell.
 
     Examples
     --------
     - FCC primitive → 111 hexagonal cell: ``lambda a,b,c: (a-c,b-c,a+b+c) ~ [[1,0,-1],[0,1,-1],[1,1,1]]``
     - FCC primitive → FCC unit cell: ``lambda a,b,c: (b+c -a,a+c-b,a+b-c) ~ [[-1,1,1],[1,-1,1],[1,1,-1]]``
     - FCC unit cell → 110 tetragonal cell: ``lambda a,b,c: (a-b,a+b,c) ~ [[1,-1,0],[1,1,0],[0,0,1]]``
+
+
+    .. note::
+        This function keeps underlying lattice same.
     """
     if callable(transformation):
         new_basis = np.array(transformation(*poscar_data.basis))  # mostly a tuple
         if new_basis.shape != (3, 3):
             raise Exception(
                 "transformation function should return a tuple equivalent to 3x3 matrix"
             )
@@ -2432,29 +2437,143 @@
     data["metadata"][
         "comment"
     ] = f'{data["metadata"]["comment"]} + Added {name!r}'  # Update comment
 
     return serializer.PoscarData(data)  # Return new POSCAR
 
 
-def strain_poscar(poscar_data, strain_matrix):
-    "Strain a POSCAR by a given 3x3 `strain_matrix` to be multiplied with basis (elementwise) and return a new POSCAR."
-    if not isinstance(strain_matrix, np.ndarray):
-        strain_matrix = np.array(strain_matrix)
+def _validate_func(func, nargs, return_type):
+    if not callable(func):
+        raise ValueError("`func` must be a callable function.")
+
+    if len(inspect.signature(func).parameters) != nargs:
+        raise ValueError(
+            f"`func` must be a function with {nargs} arguments, got {len(inspect.signature(func).parameters)}."
+        )
+    ret = func(*range(nargs))
+    if not isinstance(ret, return_type):
+        raise ValueError(
+            f"`func` must be a function that returns {return_type}, got {type(ret)}."
+        )
+
+
+def replace_atoms(poscar_data, func, name):
+    """Replace atoms satisfying a `func(i,x,y,z) -> bool` with a new `name`"""
+    if name in poscar_data.types.keys():
+        return poscar_data  # no change
 
-    if strain_matrix.shape != (3, 3):
-        raise ValueError("`strain_matrix` must be a 3x3 matrix to multiply with basis.")
+    _validate_func(func, 4, bool)
+    data = poscar_data.to_dict()  # Copy data to avoid modifying original
+    mask = _masked_data(poscar_data, func)
+    new_types = {**{k: [] for k in poscar_data.types.keys()}, name: []}
+
+    for k, vs in data["types"].items():
+        for idx in vs:
+            if idx in mask:
+                new_types[name].append(idx)
+            else:
+                new_types[k].append(idx)
+
+    data["positions"] = np.vstack([data["positions"][t] for t in new_types.values()])
+    idxs = np.cumsum([0, *map(len, new_types.values())])
+    data["types"] = {
+        k: range(idxs[i], idxs[i + 1])
+        for i, k in enumerate(new_types.keys())
+        if len(new_types[k]) != 0
+    }
+    return serializer.PoscarData(data)  # Return new POSCAR
+
+
+def remove_atoms(poscar_data, func, fillby=None):
+    """Remove atoms that satisfy `func(x,y,z) -> bool` on their fractional coordinates x,y,z.
+    If `fillby` is given, it will fill the removed atoms with atoms from fillby POSCAR.
+
+    .. note::
+        The coordinates of fillby POSCAR are transformed to basis of given POSCAR, before filling.
+        So a good filling is only guaranteed if both POSCARs have smaller lattice mismatch.
+    """
+    _validate_func(func, 3, bool)
+    data = poscar_data.to_dict()  # Copy data to avoid modifying original
+    positions = data["positions"]
+    mask = _masked_data(poscar_data, lambda i, x, y, z: not func(x, y, z))
+
+    new_types = {k: [] for k in poscar_data.types.keys()}
+    for k, vs in data["types"].items():
+        for idx in vs:
+            if idx in mask:
+                new_types[k].append(idx)
+
+    if fillby:
+        if not isinstance(fillby, serializer.PoscarData):
+            raise ValueError("`fillby` must be instance of PoscarData class.")
+
+        filldata = fillby.to_dict()
+        positions = np.vstack(
+            [data["positions"], to_basis(poscar_data.basis, fillby.coords)]
+        )  # update positions of fillby in given data basis, not fillby basis
+
+        def keep_pos(i, x, y, z):  # keep positions in basis of given data
+            u, v, w = to_basis(poscar_data.basis, to_R3(fillby.basis, [[x, y, z]]))[0]
+            return bool(func(u, v, w))
+
+        mask = _masked_data(fillby, keep_pos)
+        N_prev = len(data["positions"])  # before filling
+        new_types = {
+            **{k: [] for k in filldata["types"]},
+            **new_types,
+        }  # Add new types from fillby but keep old types values
+
+        for k, vs in filldata["types"].items():
+            for idx in vs:
+                if idx in mask:
+                    new_types[k].append(N_prev + idx)
+
+    data["positions"] = np.vstack([positions[t] for t in new_types.values()])
+    idxs = np.cumsum([0, *map(len, new_types.values())])
+    data["types"] = {
+        k: range(idxs[i], idxs[i + 1])
+        for i, k in enumerate(new_types.keys())
+        if len(new_types[k]) != 0
+    }
+
+    return serializer.PoscarData(data)  # Return new POSCAR
+
+
+def deform_poscar(poscar_data, deformation):
+    """Deform a POSCAR by a deformation as 3x3 ArrayLike, or a function that takee basis and returns a 3x3 ArrayLike,
+    to be multiplied with basis (elementwise) and return a new POSCAR.
+
+    .. note::
+        This function can change underlying crystal structure if cell shape changes, to just change cell shape, use `transform` function instead.
+    """
+    if callable(deformation):
+        try:
+            dmatrix = deformation(*poscar_data.basis)
+        except:
+            raise ValueError(
+                "`deformation` function must be a function(a,b,c) -> 3x3 matrix to multiply with basis."
+            )
+    else:
+        dmatrix = deformation
+
+    if not isinstance(dmatrix, np.ndarray):
+        dmatrix = np.array(dmatrix)
+
+    if dmatrix.shape != (3, 3):
+        raise ValueError(
+            "`deformation` must be a 3x3 matrix or a function(a,b,c) -> 3x3 matrix to multiply with basis."
+        )
 
     poscar_data = poscar_data.to_dict()  #
     poscar_data["basis"] = (
-        poscar_data["basis"] * strain_matrix
+        poscar_data["basis"] * dmatrix
     )  # Update basis by elemetwise multiplication
     poscar_data["metadata"][
         "comment"
-    ] = f'{poscar_data["metadata"]["comment"]} + Strained POSCAR'  # Update comment
+    ] = f'{poscar_data["metadata"]["comment"]} + Deformed POSCAR'  # Update comment
     return serializer.PoscarData(poscar_data)  # Return new POSCAR
 
 
 def view_poscar(poscar_data, **kwargs):
     "View a POSCAR in a jupyter notebook. kwargs are passed to splot_lattice. After setting a view, you can do view.f(**view.kwargs) to get same plot in a cell."
 
     def view(elev=30, azim=30, roll=0):
```

### Comparing `ipyvasp-0.6.1/ipyvasp/bsdos.py` & `ipyvasp-0.6.2/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/cli.py` & `ipyvasp-0.6.2/ipyvasp/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Testing a flexible command line interface for ipyvasp
+from typing import List
+from pathlib import Path
 
 import typer
+from typing_extensions import Annotated
+
 from .core.parser import minify_vasprun
 from .lattice import POSCAR, get_kpath
 from .utils import _sig_kwargs
 
 app = typer.Typer(no_args_is_help=True)
 poscar_app = typer.Typer(no_args_is_help=True)
 app.add_typer(poscar_app, name="poscar", help="POSCAR related operations")
@@ -52,49 +56,63 @@
         return get_kpath(kpoints, n=n, **kwargs)
 
 
 vasprun_app.command("minify")(minify_vasprun)
 
 
 @vasprun_app.command("get-gap")
-def get_gap(glob: str = "vasprun.xml"):
-    from pathlib import Path
+def get_gap(glob: List[Path]):
     from .core.parser import Vasprun
-    from .utils import list_files
     from .widgets import summarize
 
     def gap_summary(path):
         gap = Vasprun(path).bands.gap
         delattr(gap, "coords")  # remove coords info
         d = gap.to_dict()
-        d["kvbm"] = "|".join(str(round(k, 4)) for k in d["kvbm"])
-        d["kcbm"] = "|".join(str(round(k, 4)) for k in d["kcbm"])
+        d["kvbm"] = "(" + ",".join(str(round(k, 4)) for k in d["kvbm"]) + ")"
+        d["kcbm"] = "(" + ",".join(str(round(k, 4)) for k in d["kcbm"]) + ")"
         return d
 
     name = str(Path(".").absolute())
     print("\n", name, "\n", "=" * len(name), "\n")
-    print(summarize(list_files(glob=glob), gap_summary))
+    print(summarize(glob, gap_summary).to_string())  # make all data visible
 
 
 @vasprun_app.command("get-summary")
-def get_summary(glob: str = "vasprun.xml"):
+def get_summary(glob: List[Path]):
     from .core.parser import Vasprun
-    from .utils import list_files
 
-    for path in list_files(glob=glob):
+    for path in glob:
         name = str(path.absolute())
         print("\n", name, "\n", "=" * len(name))
         print(Vasprun(path).summary)
 
 
 @app.command("set-dir")
-def _set_dir(glob: str = "*", command: str = ""):
+def _set_dir(glob: List[Path], command: str = ""):
+    from platform import system
     from subprocess import Popen
-    from .utils import set_dir, list_files
+    from .utils import set_dir
+
+    os = system()  # operating system
 
-    for path in list_files(glob=glob, dirs_only=True):
+    dirs = [f.absolute() for f in glob if f.is_dir()]  # only dirs
+    if not dirs:
+        raise RuntimeError(
+            "Provided paths do not exist or are not directories. Exiting..."
+        )
+
+    for path in dirs:
         with set_dir(path) as p:
-            print("Working in : ", p)  # to give info about the cwd
-            p = Popen(command, shell=False)
+            print("Working in -> ", p)  # to give info about the cwd
+            if os == "Windows":
+                try:
+                    p = Popen("pwsh.exe -NoProfile -c " + command, shell=False)
+                except:
+                    p = Popen("powershell.exe -NoProfile -c " + command, shell=False)
+
+            else:
+                p = Popen(command, shell=False)  # Linux, MacOS
+
             p.wait()
             if p.returncode != 0:
                 raise RuntimeError(f"Command {command} failed in {path}. Exiting...")
```

### Comparing `ipyvasp-0.6.1/ipyvasp/core/parser.py` & `ipyvasp-0.6.2/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.6.2/ipyvasp/core/plot_toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -918,23 +918,25 @@
         height = int(height / 2)  #
         chars = [".", ":", ";", "+", "*", "?", "%", "S", "#", "@"]
         chars = chars[::-1] if invert else chars  # Inversion
         img = img.resize((width, height)).convert("L")  # grayscale
         pixels = [chars[int(v * len(chars) / 255) - 1] for v in img.getdata()]
         pixels = np.reshape(pixels, (height, -1))  # Make row/columns
 
-    out_str = "\n".join(["".join([p for p in ps]) for ps in pixels])
+    out_str = " " + "\n ".join(["".join([p for p in ps]) for ps in pixels])
 
     if outfile:
         with open(outfile, "w", encoding="utf-8") as f:  # unicode
             f.write(out_str)
     else:
-        # For loop is important for printing lines, otherwise breaks appear.
-        for line in out_str.splitlines():
-            print(line)
+        if colorful:
+            for line in out_str.splitlines():
+                print(line)  # for loop to give time to termail to adjust
+        else:
+            print(out_str)
 
 
 def plt2html(plt_fig=None, transparent=True):
     """Returns ``ipython.display.HTML(<svg of figure>)``. It clears figure after use. So ``plt.show()`` will not work after this.
 
     Parameters
     ----------
```

### Comparing `ipyvasp-0.6.1/ipyvasp/core/serializer.py` & `ipyvasp-0.6.2/ipyvasp/core/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     angle_deg,
     to_basis,
     to_R3,
     kpoints2bz,
     order,
     coplanar,
     angle_deg,
+    get_TM,
     ConvexHull,
 )
 from ..utils import _sub_doc
 
 
 def dict2tuple(name: str, d: dict):
     """
@@ -533,23 +534,32 @@
         "Converts cartesian coordinates to fractional coordinates in the basis of the brillouin zone."
         return to_basis(self.basis, coords)
 
     def to_cartesian(self, points):
         "Converts fractional coordinates in the basis of the brillouin zone to cartesian coordinates."
         return to_R3(self.basis, points)
 
-    def map_kpoints(self, other, kpoints):
+    def map_kpoints(self, other, kpoints, fold=True):
         """Map kpoints (fractional) from this to other Brillouin zone.
+        In simple words, how other BZ sees the kpoints of this BZ into their basis.
         This operation is useful when you do POSCAR.transform() and want to map kpoints between given and transformed BZ.
+
+        .. note::
+            Points outside the first BZ of `other` BZ will be mapped to the first BZ of `other` if `fold` is True (defualt).
         """
         if not isinstance(other, self.__class__):
             raise TypeError(
                 f"other must be a {self.__class__} object, got {type(other)}"
             )
-        return other.to_fractional(self.to_cartesian(kpoints))
+        pts = other.to_fractional(self.to_cartesian(kpoints))
+        if fold:
+            # remove integer part to bring back in first BZ by using .round(0)
+            # I tried .astype(int) but it left 1 as it is, so strange.
+            pts = pts - pts.round(0)
+        return pts
 
     @_sub_doc(kpoints2bz, {"bz_data :.*kpoints :": "kpoints :"})
     def translate_inside(self, kpoints, shift=0, keep_geometry=False):
         return kpoints2bz(self, kpoints, shift=shift, keep_geomerty=keep_geometry)
 
     def subzone(self, func, loop=True):
         """Returns a subzone of the brillouin zone by applying a function on the fractional special points of the zone.
```

### Comparing `ipyvasp-0.6.1/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.6.2/ipyvasp/core/spatial_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/evals_dataframe.py` & `ipyvasp-0.6.2/ipyvasp/evals_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/lattice.py` & `ipyvasp-0.6.2/ipyvasp/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
         if plot_vectors:
             for i, b in enumerate(cell.basis, start=1):
                 tail = b - b / np.linalg.norm(b)
                 shape.add_cone(
                     tail.tolist(), b.tolist(), _color, linewidth * 3, f"a{i}"
                 )
-                shape.add_text((b / 2).tolist(), [0.2, 0.15, 0.2], 2, f"a{i}")
     if dashboard:
         view.gui_style = "NGL"
     return view
 
 
 class POSCAR:
     _cb_instance = {}  # Loads last clipboard data if not changed
@@ -340,26 +339,33 @@
             cif_str = f.read()
             poscar_content = plat._cif_str_to_poscar_str(
                 cif_str, "Exported from cif file using ipyvasp"
             )
 
         return cls.from_string(poscar_content)
 
+    def to_dict(self):
+        "Returns a dictionary that can be modified generally and passed to `POSCAR.new` method."
+        data = self.data.copy()  # avoid overwriting numpy arrays
+        out = {"system": data.SYSTEM, "basis": data.basis}
+        out["sites"] = {k: data.positions[v] for k, v in data.types.items()}
+        return out
+
     @classmethod
-    def new(cls, basis, sites, scale=1, name=None):
+    def new(cls, basis, sites, scale=1, system=None):
         """
         Crate a new POSCAR instance from basis and sites.
 
         Parameters
         ----------
         basis : array_like of shape (3, 3)
         sites : dict, key is element and value is array_like of shape (n, 3)
             For example, {'Mg': [[0, 0, 0]], 'Cl': [[1/3, 2/3,0.214],[2/3,1/3,0.786]]} for MgCl2.
         scale : int or float used to scale basis and kept in metadata to use when writing to file.
-        name : str, name of the structure, if None, will be inferred from sites.
+        system : str, name of the structure, if None, will be inferred from sites.
         """
         if np.ndim(basis) != 2 and np.shape(basis) != (3, 3):
             raise ValueError("basis should be a 3x3 array")
         if not isinstance(scale, (int, float, np.integer)):
             raise ValueError("scale should be a number")
 
         basis = np.array(basis) * scale  # scale basis, we add scale to metdata later
@@ -381,15 +387,15 @@
             type_dict[key] = range(start, start + len(value))
             positions.extend(value)  # direct stacking of positions
             start += len(value)
 
         positions = np.array(positions)
 
         out_dict = {
-            "SYSTEM": name if name else "".join(type_dict.keys()),
+            "SYSTEM": system if system else "".join(type_dict.keys()),
             "basis": basis,
             "metadata": {
                 "scale": scale,
                 "cartesian": False,
                 "comment": "Created using ipyvasp.lattice.POSCAR.new method",
             },
             "positions": positions,
@@ -571,30 +577,45 @@
 
     @_sub_doc(plat.add_atoms)
     def add_atoms(self, name, positions):
         return self.__class__(
             data=plat.add_atoms(self.data, name=name, positions=positions)
         )
 
+    @_sub_doc(plat.remove_atoms)
+    def remove_atoms(self, func, fillby=None):
+        if fillby and not isinstance(fillby, POSCAR):
+            raise TypeError("fillby should be an instance of POSCAR class.")
+
+        return self.__class__(
+            data=plat.remove_atoms(
+                self.data, func=func, fillby=fillby.data if fillby else None
+            )
+        )
+
+    @_sub_doc(plat.replace_atoms)
+    def replace_atoms(self, func, name):
+        return self.__class__(data=plat.replace_atoms(self.data, func=func, name=name))
+
     @_sub_doc(plat.convert_poscar)
     def convert(self, atoms_mapping, basis_factor):
         return self.__class__(
             data=plat.convert_poscar(
                 self.data, atoms_mapping=atoms_mapping, basis_factor=basis_factor
             )
         )
 
-    @_sub_doc(plat.strain_poscar)
-    def strain(self, strain_matrix):
+    @_sub_doc(plat.deform_poscar)
+    def deform(self, deformation):
         return self.__class__(
-            data=plat.strain_poscar(self.data, strain_matrix=strain_matrix)
+            data=plat.deform_poscar(self.data, deformation=deformation)
         )
 
     @_sub_doc(get_kmesh, {"poscar_data :.*\*args :": "*args :"})
     @_sig_kwargs(get_kmesh, ("poscar_data",))
     def get_kmesh(self, *args, **kwargs):
         return get_kmesh(self.data, *args, **kwargs)
 
     @_sub_doc(get_kpath, {"rec_basis :.*\n\n": "\n\n"})
     @_sig_kwargs(get_kpath, ("rec_basis",))
-    def get_kpath(self, kpoints, n : int=5, **kwargs):
+    def get_kpath(self, kpoints, n: int = 5, **kwargs):
         return get_kpath(kpoints, n=n, **kwargs, rec_basis=self.data.rec_basis)
```

### Comparing `ipyvasp-0.6.1/ipyvasp/misc.py` & `ipyvasp-0.6.2/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/potential.py` & `ipyvasp-0.6.2/ipyvasp/potential.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/utils.py` & `ipyvasp-0.6.2/ipyvasp/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp/widgets.py` & `ipyvasp-0.6.2/ipyvasp/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/ipyvasp.egg-info/PKG-INFO` & `ipyvasp-0.6.2/ipyvasp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.1
+Version: 0.6.2
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.1/ipyvasp.egg-info/SOURCES.txt` & `ipyvasp-0.6.2/ipyvasp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.1/setup.py` & `ipyvasp-0.6.2/setup.py`

 * *Files identical despite different names*

