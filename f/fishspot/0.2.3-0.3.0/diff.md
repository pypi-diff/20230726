# Comparing `tmp/fishspot-0.2.3.tar.gz` & `tmp/fishspot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fishspot-0.2.3.tar", last modified: Wed Oct 26 14:03:24 2022, max compression
+gzip compressed data, was "fishspot-0.3.0.tar", last modified: Wed Jul 26 19:15:42 2023, max compression
```

## Comparing `fishspot-0.2.3.tar` & `fishspot-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2022-10-26 14:03:24.127112 fishspot-0.2.3/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     1067 2021-03-04 14:54:34.000000 fishspot-0.2.3/LICENSE
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      287 2022-10-26 14:03:24.125664 fishspot-0.2.3/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     1933 2022-02-18 19:24:55.000000 fishspot-0.2.3/README.md
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2022-10-26 14:03:24.104758 fishspot-0.2.3/fishspot/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)        5 2021-03-04 14:54:34.000000 fishspot-0.2.3/fishspot/__init__.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     4742 2022-10-17 17:10:23.000000 fishspot-0.2.3/fishspot/assign.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     1277 2022-04-06 20:05:04.000000 fishspot-0.2.3/fishspot/detect.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     4684 2022-10-12 21:30:44.000000 fishspot-0.2.3/fishspot/distribute.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     5083 2022-10-10 18:45:27.000000 fishspot-0.2.3/fishspot/filter.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     4540 2022-06-23 19:06:00.000000 fishspot-0.2.3/fishspot/psf.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      331 2022-02-18 16:43:35.000000 fishspot-0.2.3/fishspot/visualize.py
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2022-10-26 14:03:24.121765 fishspot-0.2.3/fishspot.egg-info/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      287 2022-10-26 14:03:23.000000 fishspot-0.2.3/fishspot.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      324 2022-10-26 14:03:23.000000 fishspot-0.2.3/fishspot.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)        1 2022-10-26 14:03:23.000000 fishspot-0.2.3/fishspot.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)       59 2022-10-26 14:03:23.000000 fishspot-0.2.3/fishspot.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)        9 2022-10-26 14:03:23.000000 fishspot-0.2.3/fishspot.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)       38 2022-10-26 14:03:24.127955 fishspot-0.2.3/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      531 2022-10-26 14:02:01.000000 fishspot-0.2.3/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-26 19:15:32.253268 fishspot-0.3.0/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1067 2021-03-04 14:54:34.000000 fishspot-0.3.0/LICENSE
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      259 2023-07-26 19:15:32.251783 fishspot-0.3.0/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1933 2022-02-18 19:24:55.000000 fishspot-0.3.0/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-26 19:15:32.227930 fishspot-0.3.0/fishspot/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2021-03-04 14:54:34.000000 fishspot-0.3.0/fishspot/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    10622 2023-04-05 22:16:16.000000 fishspot-0.3.0/fishspot/assign.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1100 2023-06-26 23:35:25.000000 fishspot-0.3.0/fishspot/detect.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    12660 2023-03-29 17:57:13.000000 fishspot-0.3.0/fishspot/distribute.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     5001 2023-06-02 13:56:23.000000 fishspot-0.3.0/fishspot/filter.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4540 2022-06-23 19:06:00.000000 fishspot-0.3.0/fishspot/psf.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      331 2022-02-18 16:43:35.000000 fishspot-0.3.0/fishspot/visualize.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-26 19:15:32.246797 fishspot-0.3.0/fishspot.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      259 2023-07-26 19:15:31.000000 fishspot-0.3.0/fishspot.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      324 2023-07-26 19:15:32.000000 fishspot-0.3.0/fishspot.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-26 19:15:31.000000 fishspot-0.3.0/fishspot.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       59 2023-07-26 19:15:31.000000 fishspot-0.3.0/fishspot.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        9 2023-07-26 19:15:31.000000 fishspot-0.3.0/fishspot.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-26 19:15:32.255014 fishspot-0.3.0/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      531 2023-07-26 19:14:31.000000 fishspot-0.3.0/setup.py
```

### Comparing `fishspot-0.2.3/LICENSE` & `fishspot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fishspot-0.2.3/README.md` & `fishspot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fishspot-0.2.3/fishspot/filter.py` & `fishspot-0.3.0/fishspot/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         kwargs['filter_epsilon'] = 1e-6
 
     # run decon, renormalize, return
     decon = richardson_lucy(norm_image, psf, **kwargs)
     return rescale_intensity(decon, in_range=(0, 1), out_range=(0, mx))
 
 
-def apply_foreground_mask(spots, mask, ratio):
+def apply_foreground_mask(spots, mask, ratio=1):
     """
     """
 
     # get spot locations in mask voxel coordinates
     x = np.round(spots[:, :3] * ratio).astype(np.uint16)
 
     # correct out of range rounding errors
@@ -61,15 +61,15 @@
 def filter_by_range(spots, origin, span):
     """
     """
 
     # operate on a copy, filter lower/upper range all axes
     result = np.copy(spots)
     for i in range(3):
-        result = result[result[:, i] > origin[i] - 1]
+        result = result[result[:, i] >= origin[i]]
         result = result[result[:, i] < origin[i] + span[i]]
     return result
 
 
 def percentile_filter(spots, percentile):
     """
     """
@@ -81,21 +81,20 @@
 def density_filter(spots, radius, neighbor_threshold):
     """
     """
 
     # get spot-to-spot distances
     tree = cKDTree(spots[:, :3])
     dok = tree.sparse_distance_matrix(tree, radius)
-    dok.setdiag(np.finfo(spots.dtype).eps)  # to distinguish from fill value
     csr = dok.tocsr()
 
     # determine loner spots, remove them and return
     density_filter = np.ones(spots.shape[0], dtype=bool)
     for iii in range(spots.shape[0]):
-        if csr[iii].count_nonzero() - 1 < neighbor_threshold:
+        if csr[iii].count_nonzero() < neighbor_threshold:
             density_filter[iii] = False
     return spots[density_filter]
 
 
 def remove_duplicates(spots1, spots2, radius, return_duplicate_indices=False):
     """
     """
```

### Comparing `fishspot-0.2.3/fishspot/psf.py` & `fishspot-0.3.0/fishspot/psf.py`

 * *Files identical despite different names*

### Comparing `fishspot-0.2.3/setup.py` & `fishspot-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="fishspot",
-    version="0.2.3",
+    version="0.3.0",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for finding discrete bright spots in images",
     url="https://github.com/GFleishman/fishspot",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

