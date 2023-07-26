# Comparing `tmp/RACS-tools-2.2.6.tar.gz` & `tmp/RACS-tools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RACS-tools-2.2.6.tar", last modified: Wed Jul 26 00:09:18 2023, max compression
+gzip compressed data, was "RACS-tools-2.3.0.tar", last modified: Wed Jul 26 02:29:28 2023, max compression
```

## Comparing `RACS-tools-2.2.6.tar` & `RACS-tools-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 00:09:18.349315 RACS-tools-2.2.6/
--rw-------   0 tho822   (728663) staff       (20)     1520 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/LICENSE
--rw-r--r--   0 tho822   (728663) staff       (20)    10024 2023-07-26 00:09:18.349108 RACS-tools-2.2.6/PKG-INFO
-drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 00:09:18.345498 RACS-tools-2.2.6/RACS_tools.egg-info/
--rw-------   0 tho822   (728663) staff       (20)    10024 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/PKG-INFO
--rw-------   0 tho822   (728663) staff       (20)      467 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/SOURCES.txt
--rw-------   0 tho822   (728663) staff       (20)        1 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/dependency_links.txt
--rw-------   0 tho822   (728663) staff       (20)      141 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/entry_points.txt
--rw-------   0 tho822   (728663) staff       (20)       82 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/requires.txt
--rw-------   0 tho822   (728663) staff       (20)       11 2023-07-26 00:09:18.000000 RACS-tools-2.2.6/RACS_tools.egg-info/top_level.txt
--rw-------   0 tho822   (728663) staff       (20)     9371 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/README.md
--rw-------   0 tho822   (728663) staff       (20)      116 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/pyproject.toml
-drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 00:09:18.347929 RACS-tools-2.2.6/racs_tools/
--rw-------   0 tho822   (728663) staff       (20)        0 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/racs_tools/__init__.py
--rw-------   0 tho822   (728663) staff       (20)     5078 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/racs_tools/au2.py
--rw-------   0 tho822   (728663) staff       (20)    24699 2023-07-26 00:08:39.000000 RACS-tools-2.2.6/racs_tools/beamcon_2D.py
--rw-------   0 tho822   (728663) staff       (20)    45668 2023-07-26 00:08:04.000000 RACS-tools-2.2.6/racs_tools/beamcon_3D.py
--rw-------   0 tho822   (728663) staff       (20)     5334 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/racs_tools/convolve_uv.py
--rw-------   0 tho822   (728663) staff       (20)     4351 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/racs_tools/gaussft.f
--rw-------   0 tho822   (728663) staff       (20)     8308 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/racs_tools/getnoise_list.py
--rw-r--r--   0 tho822   (728663) staff       (20)       38 2023-07-26 00:09:18.349376 RACS-tools-2.2.6/setup.cfg
--rw-------   0 tho822   (728663) staff       (20)     4283 2023-07-26 00:08:52.000000 RACS-tools-2.2.6/setup.py
-drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 00:09:18.348747 RACS-tools-2.2.6/tests/
--rw-------   0 tho822   (728663) staff       (20)     5831 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/tests/test_2d.py
--rw-------   0 tho822   (728663) staff       (20)     6843 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/tests/test_3d.py
--rw-------   0 tho822   (728663) staff       (20)     4349 2023-05-22 00:36:00.000000 RACS-tools-2.2.6/tests/test_noise.py
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 02:29:28.056094 RACS-tools-2.3.0/
+-rw-------   0 tho822   (728663) staff       (20)     1520 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/LICENSE
+-rw-r--r--   0 tho822   (728663) staff       (20)    10024 2023-07-26 02:29:28.055884 RACS-tools-2.3.0/PKG-INFO
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 02:29:28.053636 RACS-tools-2.3.0/RACS_tools.egg-info/
+-rw-------   0 tho822   (728663) staff       (20)    10024 2023-07-26 02:29:27.000000 RACS-tools-2.3.0/RACS_tools.egg-info/PKG-INFO
+-rw-------   0 tho822   (728663) staff       (20)      489 2023-07-26 02:29:28.000000 RACS-tools-2.3.0/RACS_tools.egg-info/SOURCES.txt
+-rw-------   0 tho822   (728663) staff       (20)        1 2023-07-26 02:29:27.000000 RACS-tools-2.3.0/RACS_tools.egg-info/dependency_links.txt
+-rw-------   0 tho822   (728663) staff       (20)      141 2023-07-26 02:29:27.000000 RACS-tools-2.3.0/RACS_tools.egg-info/entry_points.txt
+-rw-------   0 tho822   (728663) staff       (20)       82 2023-07-26 02:29:27.000000 RACS-tools-2.3.0/RACS_tools.egg-info/requires.txt
+-rw-------   0 tho822   (728663) staff       (20)       11 2023-07-26 02:29:27.000000 RACS-tools-2.3.0/RACS_tools.egg-info/top_level.txt
+-rw-------   0 tho822   (728663) staff       (20)     9371 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/README.md
+-rw-------   0 tho822   (728663) staff       (20)      116 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/pyproject.toml
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 02:29:28.055228 RACS-tools-2.3.0/racs_tools/
+-rw-------   0 tho822   (728663) staff       (20)        0 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/racs_tools/__init__.py
+-rw-------   0 tho822   (728663) staff       (20)     5078 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/racs_tools/au2.py
+-rw-r--r--   0 tho822   (728663) staff       (20)    24406 2023-07-26 02:29:06.000000 RACS-tools-2.3.0/racs_tools/beamcon_2D.py
+-rw-r--r--   0 tho822   (728663) staff       (20)    45606 2023-07-26 02:29:06.000000 RACS-tools-2.3.0/racs_tools/beamcon_3D.py
+-rw-------   0 tho822   (728663) staff       (20)     5334 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/racs_tools/convolve_uv.py
+-rw-------   0 tho822   (728663) staff       (20)     4351 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/racs_tools/gaussft.f
+-rw-r--r--   0 tho822   (728663) staff       (20)     8669 2023-07-26 02:29:06.000000 RACS-tools-2.3.0/racs_tools/getnoise_list.py
+-rw-r--r--   0 tho822   (728663) staff       (20)     1038 2023-07-26 02:29:06.000000 RACS-tools-2.3.0/racs_tools/logging.py
+-rw-r--r--   0 tho822   (728663) staff       (20)       38 2023-07-26 02:29:28.056131 RACS-tools-2.3.0/setup.cfg
+-rw-------   0 tho822   (728663) staff       (20)     4283 2023-07-26 02:29:11.000000 RACS-tools-2.3.0/setup.py
+drwxr-xr-x   0 tho822   (728663) staff       (20)        0 2023-07-26 02:29:28.055645 RACS-tools-2.3.0/tests/
+-rw-------   0 tho822   (728663) staff       (20)     5831 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/tests/test_2d.py
+-rw-------   0 tho822   (728663) staff       (20)     6843 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/tests/test_3d.py
+-rw-------   0 tho822   (728663) staff       (20)     4349 2023-05-22 00:36:00.000000 RACS-tools-2.3.0/tests/test_noise.py
```

### Comparing `RACS-tools-2.2.6/LICENSE` & `RACS-tools-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/PKG-INFO` & `RACS-tools-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RACS-tools
-Version: 2.2.6
+Version: 2.3.0
 Summary: Useful scripts for RACS.
 Home-page: https://github.com/AlecThomson/RACS-tools
 Author: Alec Thomson
 Author-email: alec.thomson@csiro.au
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `RACS-tools-2.2.6/RACS_tools.egg-info/PKG-INFO` & `RACS-tools-2.3.0/RACS_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RACS-tools
-Version: 2.2.6
+Version: 2.3.0
 Summary: Useful scripts for RACS.
 Home-page: https://github.com/AlecThomson/RACS-tools
 Author: Alec Thomson
 Author-email: alec.thomson@csiro.au
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `RACS-tools-2.2.6/README.md` & `RACS-tools-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/racs_tools/au2.py` & `RACS-tools-2.3.0/racs_tools/au2.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/racs_tools/beamcon_2D.py` & `RACS-tools-2.3.0/racs_tools/beamcon_2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 from astropy.wcs.utils import proj_plane_pixel_scales
 from radio_beam import Beam, Beams
 from radio_beam.utils import BeamError
 from tqdm import tqdm
 
 from racs_tools import au2
 from racs_tools.convolve_uv import smooth
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
-
+from racs_tools.logging import logger, setup_logger
 
 #############################################
 #### ADAPTED FROM SCRIPT BY T. VERNSTROM ####
 #############################################
 
 
 def round_up(n: float, decimals: int = 0) -> float:
@@ -796,29 +793,20 @@
         help="Number of processes (uses multiprocessing).",
     )
     group.add_argument(
         "--mpi", dest="mpi", default=False, action="store_true", help="Run with MPI."
     )
 
     args = parser.parse_args()
-    if args.mpi:
-        from mpi4py import MPI
+    # Set up logging
+    logger = setup_logger(
+        verbosity=args.verbosity,
+        filename=args.logfile,
+    )
 
-        comm = MPI.COMM_WORLD
-        myPE = comm.Get_rank()
-    else:
-        try:
-            myPE = psutil.Process().cpu_num()
-        except AttributeError:
-            myPE = 0
-    if args.verbosity == 1:
-        logger.setLevel(
-            level=logging.INFO)
-    elif args.verbosity >= 2:
-        logger.basicConfig(level=logger.DEBUG)
     pool = schwimmbad.choose_pool(mpi=args.mpi, processes=args.n_cores)
     if args.mpi:
         if not pool.is_master():
             pool.wait()
             sys.exit(0)
 
     arg_dict = vars(args)
```

### Comparing `RACS-tools-2.2.6/racs_tools/beamcon_3D.py` & `RACS-tools-2.3.0/racs_tools/beamcon_3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 from spectral_cube import SpectralCube
 from spectral_cube.utils import SpectralCubeWarning
 from tqdm import tqdm, trange
 
 from racs_tools import au2
 from racs_tools.beamcon_2D import my_ceil, round_up
 from racs_tools.convolve_uv import smooth
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
+from racs_tools.logging import logger, setup_logger
 
 mpiSwitch = False
 if (
     os.environ.get("OMPI_COMM_WORLD_SIZE") is not None
     or int(os.environ.get("SLURM_NTASKS") or 1) > 1
 ):
     mpiSwitch = True
@@ -1349,19 +1347,19 @@
         type=int,
         default=200,
         help="nsamps for radio_beam.commonbeam.",
     )
 
     args = parser.parse_args()
 
-    if args.verbosity == 1:
-        logger.setLevel(
-            level=logging.INFO)
-    elif args.verbosity >= 2:
-        logger.basicConfig(level=logger.DEBUG)
+    # Set up logging
+    logger = setup_logger(
+        verbosity=args.verbosity,
+        filename=args.logfile,
+    )
 
     arg_dict = vars(args)
     # Pop the verbosity argument
     _ = arg_dict.pop("verbosity")
     # Pop the logfile argument
     _ = arg_dict.pop("logfile")
```

### Comparing `RACS-tools-2.2.6/racs_tools/convolve_uv.py` & `RACS-tools-2.3.0/racs_tools/convolve_uv.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/racs_tools/gaussft.f` & `RACS-tools-2.3.0/racs_tools/gaussft.f`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/racs_tools/getnoise_list.py` & `RACS-tools-2.3.0/racs_tools/getnoise_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 import astropy.units as u
 import numpy as np
 from astropy.stats import mad_std
 from spectral_cube import SpectralCube
 from spectral_cube.utils import SpectralCubeWarning
 
-warnings.filterwarnings(action="ignore", category=SpectralCubeWarning, append=True)
+from racs_tools.logging import logger, setup_logger
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
+warnings.filterwarnings(action="ignore", category=SpectralCubeWarning, append=True)
 
 
 #############################################
 ####### ADAPTED FROM SCRIPT BY G. HEALD #####
 #############################################
 def getcube(filename: str) -> SpectralCube:
     """Read FITS file as SpectralCube
@@ -241,17 +240,32 @@
     parser.add_argument(
         "-f",
         "--file",
         help="Filename to write bad channel indices to file [None --  do not write]",
         default=None,
         type=str,
     )
+    parser.add_argument(
+        "-v", "--verbosity", default=0, action="count", help="Increase output verbosity"
+    )
+    parser.add_argument(
+        "--logfile",
+        default=None,
+        type=str,
+        help="Save logging output to file",
+    )
 
     args = parser.parse_args()
 
+    # Set up logging
+    logger = setup_logger(
+        verbosity=args.verbosity,
+        filename=args.logfile,
+    )
+
     main(
         qfile=args.qfile,
         ufile=args.ufile,
         blank=args.blank,
         cliplev=args.cliplev,
         iterate=args.iterate,
         outfile=args.file,
```

### Comparing `RACS-tools-2.2.6/setup.py` & `RACS-tools-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Package meta-data.
 NAME = "RACS-tools"
 DESCRIPTION = "Useful scripts for RACS."
 URL = "https://github.com/AlecThomson/RACS-tools"
 EMAIL = "alec.thomson@csiro.au"
 AUTHOR = "Alec Thomson"
 REQUIRES_PYTHON = ">=3.8.0"
-VERSION = "2.2.6"
+VERSION = "2.3.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "numpy",
     "astropy",
     "radio_beam",
     "schwimmbad",
```

### Comparing `RACS-tools-2.2.6/tests/test_2d.py` & `RACS-tools-2.3.0/tests/test_2d.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/tests/test_3d.py` & `RACS-tools-2.3.0/tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `RACS-tools-2.2.6/tests/test_noise.py` & `RACS-tools-2.3.0/tests/test_noise.py`

 * *Files identical despite different names*

