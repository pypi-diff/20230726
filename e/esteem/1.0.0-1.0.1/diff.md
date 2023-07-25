# Comparing `tmp/esteem-1.0.0.tar.gz` & `tmp/esteem-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/theory/phspvr/esteem_package/dist/.tmp-5b7ziw9p/esteem-1.0.0.tar", last modified: Tue Jul 25 17:47:26 2023, max compression
+gzip compressed data, was "esteem-1.0.1.tar", last modified: Tue Jul 25 22:10:50 2023, max compression
```

## Comparing `esteem-1.0.0.tar` & `esteem-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:26.319318 esteem-1.0.0/
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     1053 2023-07-25 17:16:58.000000 esteem-1.0.0/LICENSE
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     2238 2023-07-25 17:47:26.304318 esteem-1.0.0/PKG-INFO
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     1696 2021-12-14 12:43:09.000000 esteem-1.0.0/README.md
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)      630 2023-07-25 17:39:43.000000 esteem-1.0.0/pyproject.toml
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)       38 2023-07-25 17:47:26.334318 esteem-1.0.0/setup.cfg
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:24.679304 esteem-1.0.0/src/
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:25.016307 esteem-1.0.0/src/esteem/
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/__init__.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    25257 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/active_learning.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    78608 2023-07-25 17:14:18.000000 esteem-1.0.0/src/esteem/drivers.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    16076 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/parallel.py
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:25.663312 esteem-1.0.0/src/esteem/tasks/
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/__init__.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    56208 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/clusters.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     3695 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/ml_debugger.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    14480 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/ml_testing.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     9631 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/ml_training.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    12302 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/ml_trajectories.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     9443 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/qmd_trajectories.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    34357 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/solutes.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    14599 2023-07-25 17:14:18.000000 esteem-1.0.0/src/esteem/tasks/solvate.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    35242 2023-07-25 17:14:19.000000 esteem-1.0.0/src/esteem/tasks/spectra.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    37271 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/trajectories.py
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:26.258317 esteem-1.0.0/src/esteem/wrappers/
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/__init__.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    38013 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/amber.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     9071 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/amp.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     9200 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/ezfcf.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    14055 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/lammps.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    21902 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/mace.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    23065 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/nff.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    23361 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/nwchem.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    14050 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/onetep.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    21040 2023-07-25 17:14:21.000000 esteem-1.0.0/src/esteem/wrappers/orca.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)    23289 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/physnet.py
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     6010 2023-07-25 17:14:20.000000 esteem-1.0.0/src/esteem/wrappers/specpycode.py
-drwxr-xr-x   0 phspvr   (13069) phspvr   (13069)        0 2023-07-25 17:47:25.196308 esteem-1.0.0/src/esteem.egg-info/
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)     2238 2023-07-25 17:47:24.000000 esteem-1.0.0/src/esteem.egg-info/PKG-INFO
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)      958 2023-07-25 17:47:24.000000 esteem-1.0.0/src/esteem.egg-info/SOURCES.txt
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)        1 2023-07-25 17:47:24.000000 esteem-1.0.0/src/esteem.egg-info/dependency_links.txt
--rw-r--r--   0 phspvr   (13069) phspvr   (13069)        7 2023-07-25 17:47:24.000000 esteem-1.0.0/src/esteem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:50.178558 esteem-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 22:10:35.000000 esteem-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-25 22:10:50.178558 esteem-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 22:10:35.000000 esteem-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:50.170558 esteem-1.0.1/esteem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78608 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:50.174558 esteem-1.0.1/esteem/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/ml_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14480 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/ml_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/ml_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/ml_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/qmd_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/solutes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/solvate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35242 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/tasks/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37271 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/trajectories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:50.178558 esteem-1.0.1/esteem/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38013 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/amber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/ezfcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/mace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/nff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23361 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/onetep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/physnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-25 22:10:35.000000 esteem-1.0.1/esteem/wrappers/specpycode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:50.170558 esteem-1.0.1/esteem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-25 22:10:50.000000 esteem-1.0.1/esteem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 22:10:50.000000 esteem-1.0.1/esteem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:10:50.000000 esteem-1.0.1/esteem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 22:10:50.000000 esteem-1.0.1/esteem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-25 22:10:35.000000 esteem-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:10:50.178558 esteem-1.0.1/setup.cfg
```

### Comparing `esteem-1.0.0/LICENSE` & `esteem-1.0.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2023 Nicholas Hine
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 Nicholas Hine
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `esteem-1.0.0/PKG-INFO` & `esteem-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esteem
-Version: 1.0.0
+Version: 1.0.1
 Summary: Explicit Solvent Toolkit for Electronic Excitations of Molecules
 Author-email: Nicholas Hine <n.d.m.hine@warwick.ac.uk>
 Project-URL: Homepage, https://esteem.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://esteem.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,53 +13,57 @@
 License-File: LICENSE
 
 ESTEEM: Explicit Solvent Toolkit for Electronic Excitations in Molecules
 ========================================================================
 
 ## Contents of package:
 
-A set of Jupyter Notebooks, which compile to python scripts
-that use the Atomic Simulation Environment python packages,
-plus a set of atomistic modelling packages.
+A python package that uses the Atomic Simulation Environment python
+packages, and a range of optional calculators that ASE can make
+available, to perform calculations of excited states of explicitly-solvated
+solute molecules.
 
 ## Dependencies:
 
 * Python 3
 * ASE (tested on 3.19.0)
+
+## Codes which can be interfaced with (all optional):
 * NWChem >=6.6 (tested on 6.6, 6.8, 7.0)
+* ORCA >= 5.0.2
 * AMBER (tested on AmberTools 16.0 and 20.0)
+* LAMMPS
 * ONETEP (tested on 5.3.x and 6.0)
-* AMP (not currently core functionality)
+* PhysNet
+* MACE
+* AMP
+* SpecPyCode
+* EZFCF
 
 ## License:
 
 This package is distributed under the MIT License.
 
 ## Setup:
 
-Extract the package and run the ipynb -> py conversion by
-typing "python setup.py". This is also a test of whether your
-environment has everything required.
-
-You will need to add the directory containing the scripts to
-your PYTHONPATH. For example, in .bashrc you could add a line
-such as
-
-PYTHONPATH=$PYTHONPATH:~/esteem
-
-ONETEP: if ONETEP is uesd, the code assumes it will find a binary
-by the name "onetep" in $PATH or as an alias.
-
-AMBER Tools bin directory is assumed to be in $PATH (as AMBER
-installation recommends) - the code will use sander.MPI if
-available, otherwise sander. Also uses antechamber, cpptraj,
-tleap, and various other utilities.
-
-NWChem: the code assumes it will find a binary by the name "nwchem"
-
-Calculation choices are currently a mixture of some hard-wired,
-some user-modifiable. The DFT parameters and those associated
-with setup of the solvent box or cluster size can be tweaked
-script, but some of the MD parameters are hard-wired into
-Amber.ipynb - edit those directly and/or let me know what
-most needs to be on-the-fly editable.
+Install the package via pip:
+
+pip install esteem
+
+Write a script that imports esteem tasks and wrappers (or adapt something from
+/examples)
+
+Run the script, specifying the task, seedname and task_target
+
+python my_script.py <task> <seedname> <task_target>
+
+eg
+
+python cate.py solutes cate gs_PBE
+
+The script should invoke the main drivers routine once the tasks are set up.
+
+Some wrappers require only another python package: if this is correctly
+installed the code should work. Other wrappers require a binary, and
+in most cases this will need to be specified - see the instructions on 
+each wrapper for more details.
```

### Comparing `esteem-1.0.0/pyproject.toml` & `esteem-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "esteem"
-version = "1.0.0"
+version = "1.0.1"
 authors = [ { name="Nicholas Hine", email="n.d.m.hine@warwick.ac.uk" }, ]
 description = "Explicit Solvent Toolkit for Electronic Excitations of Molecules"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `esteem-1.0.0/src/esteem/active_learning.py` & `esteem-1.0.1/esteem/active_learning.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/drivers.py` & `esteem-1.0.1/esteem/drivers.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/parallel.py` & `esteem-1.0.1/esteem/parallel.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/clusters.py` & `esteem-1.0.1/esteem/tasks/clusters.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/ml_debugger.py` & `esteem-1.0.1/esteem/tasks/ml_debugger.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/ml_testing.py` & `esteem-1.0.1/esteem/tasks/ml_testing.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/ml_training.py` & `esteem-1.0.1/esteem/tasks/ml_training.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/ml_trajectories.py` & `esteem-1.0.1/esteem/tasks/ml_trajectories.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/qmd_trajectories.py` & `esteem-1.0.1/esteem/tasks/qmd_trajectories.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/solutes.py` & `esteem-1.0.1/esteem/tasks/solutes.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/solvate.py` & `esteem-1.0.1/esteem/tasks/solvate.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/tasks/spectra.py` & `esteem-1.0.1/esteem/tasks/spectra.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/trajectories.py` & `esteem-1.0.1/esteem/trajectories.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/amber.py` & `esteem-1.0.1/esteem/wrappers/amber.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/amp.py` & `esteem-1.0.1/esteem/wrappers/amp.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/ezfcf.py` & `esteem-1.0.1/esteem/wrappers/ezfcf.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/lammps.py` & `esteem-1.0.1/esteem/wrappers/lammps.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/mace.py` & `esteem-1.0.1/esteem/wrappers/mace.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/nff.py` & `esteem-1.0.1/esteem/wrappers/nff.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/nwchem.py` & `esteem-1.0.1/esteem/wrappers/nwchem.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/onetep.py` & `esteem-1.0.1/esteem/wrappers/onetep.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/orca.py` & `esteem-1.0.1/esteem/wrappers/orca.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/physnet.py` & `esteem-1.0.1/esteem/wrappers/physnet.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem/wrappers/specpycode.py` & `esteem-1.0.1/esteem/wrappers/specpycode.py`

 * *Files identical despite different names*

### Comparing `esteem-1.0.0/src/esteem.egg-info/PKG-INFO` & `esteem-1.0.1/esteem.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esteem
-Version: 1.0.0
+Version: 1.0.1
 Summary: Explicit Solvent Toolkit for Electronic Excitations of Molecules
 Author-email: Nicholas Hine <n.d.m.hine@warwick.ac.uk>
 Project-URL: Homepage, https://esteem.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://esteem.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,53 +13,57 @@
 License-File: LICENSE
 
 ESTEEM: Explicit Solvent Toolkit for Electronic Excitations in Molecules
 ========================================================================
 
 ## Contents of package:
 
-A set of Jupyter Notebooks, which compile to python scripts
-that use the Atomic Simulation Environment python packages,
-plus a set of atomistic modelling packages.
+A python package that uses the Atomic Simulation Environment python
+packages, and a range of optional calculators that ASE can make
+available, to perform calculations of excited states of explicitly-solvated
+solute molecules.
 
 ## Dependencies:
 
 * Python 3
 * ASE (tested on 3.19.0)
+
+## Codes which can be interfaced with (all optional):
 * NWChem >=6.6 (tested on 6.6, 6.8, 7.0)
+* ORCA >= 5.0.2
 * AMBER (tested on AmberTools 16.0 and 20.0)
+* LAMMPS
 * ONETEP (tested on 5.3.x and 6.0)
-* AMP (not currently core functionality)
+* PhysNet
+* MACE
+* AMP
+* SpecPyCode
+* EZFCF
 
 ## License:
 
 This package is distributed under the MIT License.
 
 ## Setup:
 
-Extract the package and run the ipynb -> py conversion by
-typing "python setup.py". This is also a test of whether your
-environment has everything required.
-
-You will need to add the directory containing the scripts to
-your PYTHONPATH. For example, in .bashrc you could add a line
-such as
-
-PYTHONPATH=$PYTHONPATH:~/esteem
-
-ONETEP: if ONETEP is uesd, the code assumes it will find a binary
-by the name "onetep" in $PATH or as an alias.
-
-AMBER Tools bin directory is assumed to be in $PATH (as AMBER
-installation recommends) - the code will use sander.MPI if
-available, otherwise sander. Also uses antechamber, cpptraj,
-tleap, and various other utilities.
-
-NWChem: the code assumes it will find a binary by the name "nwchem"
-
-Calculation choices are currently a mixture of some hard-wired,
-some user-modifiable. The DFT parameters and those associated
-with setup of the solvent box or cluster size can be tweaked
-script, but some of the MD parameters are hard-wired into
-Amber.ipynb - edit those directly and/or let me know what
-most needs to be on-the-fly editable.
+Install the package via pip:
+
+pip install esteem
+
+Write a script that imports esteem tasks and wrappers (or adapt something from
+/examples)
+
+Run the script, specifying the task, seedname and task_target
+
+python my_script.py <task> <seedname> <task_target>
+
+eg
+
+python cate.py solutes cate gs_PBE
+
+The script should invoke the main drivers routine once the tasks are set up.
+
+Some wrappers require only another python package: if this is correctly
+installed the code should work. Other wrappers require a binary, and
+in most cases this will need to be specified - see the instructions on 
+each wrapper for more details.
```

