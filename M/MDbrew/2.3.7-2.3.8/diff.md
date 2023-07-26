# Comparing `tmp/MDbrew-2.3.7.tar.gz` & `tmp/MDbrew-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.7.tar", last modified: Sat Jun 24 09:44:21 2023, max compression
+gzip compressed data, was "MDbrew-2.3.8.tar", last modified: Wed Jul 26 14:46:40 2023, max compression
```

## Comparing `MDbrew-2.3.7.tar` & `MDbrew-2.3.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.650387 MDbrew-2.3.7/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.7/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.646122 MDbrew-2.3.7/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      182 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.647844 MDbrew-2.3.7/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     6171 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.648211 MDbrew-2.3.7/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)       20 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10136 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/application/cp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.648756 MDbrew-2.3.7/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5769 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.649635 MDbrew-2.3.7/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      940 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      933 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      848 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4427 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     2959 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)     1226 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1695 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/opener.py
--rw-r--r--   0 minu       (501) staff       (20)     1353 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/writer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.650260 MDbrew-2.3.7/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1579 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      765 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      695 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.647081 MDbrew-2.3.7/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      758 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-08 11:08:00.000000 MDbrew-2.3.7/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-24 09:44:21.650483 MDbrew-2.3.7/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.7/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-06-24 09:44:21.650768 MDbrew-2.3.7/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      665 2023-06-24 09:44:10.000000 MDbrew-2.3.7/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799761 MDbrew-2.3.8/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.8/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.796117 MDbrew-2.3.8/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      182 2023-07-26 14:46:38.000000 MDbrew-2.3.8/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.797358 MDbrew-2.3.8/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     5594 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.797679 MDbrew-2.3.8/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       20 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10136 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/application/cp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.798230 MDbrew-2.3.8/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5772 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799073 MDbrew-2.3.8/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      974 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)     1304 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4427 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     2959 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)     1226 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1695 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/opener.py
+-rw-r--r--   0 minu       (501) staff       (20)     1353 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/writer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799643 MDbrew-2.3.8/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1579 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      765 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      695 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.796925 MDbrew-2.3.8/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      758 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-26 14:46:29.000000 MDbrew-2.3.8/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-26 14:46:40.799815 MDbrew-2.3.8/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.8/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-07-26 14:46:40.800009 MDbrew-2.3.8/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      665 2023-07-26 14:46:11.000000 MDbrew-2.3.8/setup.py
```

### Comparing `MDbrew-2.3.7/MDbrew/analysis/msd.py` & `MDbrew-2.3.8/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/application/cp2k.py` & `MDbrew-2.3.8/MDbrew/application/cp2k.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/brewery.py` & `MDbrew-2.3.8/MDbrew/main/brewery.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .filetype.pdb import pdbOpener
 from .filetype.vasp import vaspOpener, POSCARWriter
 from .filetype.xyz import xyzOpener, xyzWriter
 from .filetype.trr import trrOpener
 from ..tool.colorfont import color
 from ..tool.decorator import color_print_verbose
 
+
 class Brewery(object):
     __support_opener__ = {
         "auto": None,
         "pdb": pdbOpener,
         "xyz": xyzOpener,
         "vasp": vaspOpener,
         "lmps": lmpsOpener,
@@ -111,25 +112,25 @@
 
     def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
     @color_print_verbose(name=__print_option__["b_brewing"])
-    def brew(self, cols = None, what: str = None, dtype: str = "float64", verbose: bool = False):
+    def brew(self, cols=None, what: str = None, dtype: str = "float64", verbose: bool = False):
         data = pd.DataFrame(data=self.data, columns=self.columns)
         data = data.query(self._what) if self._what is not None else data
         data = data.query(what) if what is not None else data
         data = data.loc[:, cols] if cols is not None else data
         return data.to_numpy(dtype=dtype)
 
     def reset(self):
         self._opener.reset()
 
-    def order(self, what: str = None, verbose:bool=False):
+    def order(self, what: str = None, verbose: bool = False):
         return Brewery(trj_file=self._path, fmt=self._fmt, what=what, verbose=verbose)
 
     def reorder(self):
         return Brewery(trj_file=self._path, fmt=self._fmt, what=self._what, verbose=False)
 
     def frange(self, start: int = 0, end: int = None, step: int = 1):
         self.move_frame(num=start)
```

### Comparing `MDbrew-2.3.7/MDbrew/main/filetype/gro.py` & `MDbrew-2.3.8/MDbrew/main/filetype/gro.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.8/MDbrew/main/filetype/lmps.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,18 @@
         self._atom_keyword = "type"
         super().gen_db()
 
     def _make_one_frame_data(self, file):
         self.skip_line(file=file, num=3)
         atom_num = int(file.readline().split()[0])
         self.skip_line(file=file, num=1)
-        self.box_size = [sum([float(box_length) * ((-1)**(idx+1)) for idx, box_length in enumerate(file.readline().split())]) for _ in range(3)]
+        self.box_size = [
+            sum([float(box_length) * ((-1) ** (idx + 1)) for idx, box_length in enumerate(file.readline().split())])
+            for _ in range(3)
+        ]
         self.column = file.readline().split()[2:]
         self.total_line_num = 9 + atom_num
         return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
 
     def skip_line(self, file, num):
         for _ in range(num):
             file.readline()
```

### Comparing `MDbrew-2.3.7/MDbrew/main/filetype/trr.py` & `MDbrew-2.3.8/MDbrew/main/filetype/trr.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.8/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/filetype/xyz.py` & `MDbrew-2.3.8/MDbrew/main/filetype/xyz.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/opener.py` & `MDbrew-2.3.8/MDbrew/main/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/main/writer.py` & `MDbrew-2.3.8/MDbrew/main/writer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/tool/colorfont.py` & `MDbrew-2.3.8/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/tool/decorator.py` & `MDbrew-2.3.8/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/tool/doctor.py` & `MDbrew-2.3.8/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew/tool/spacer.py` & `MDbrew-2.3.8/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.8/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.7/setup.py` & `MDbrew-2.3.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.7",
+    version="2.3.8",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.7.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.8.tar.gz",
     install_requies=[
         "numpy>=1.19.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
```

