# Comparing `tmp/pydactim-0.0.5.tar.gz` & `tmp/pydactim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydactim-0.0.5.tar", last modified: Wed Jul 26 09:23:51 2023, max compression
+gzip compressed data, was "dist\pydactim-0.0.6.tar", last modified: Wed Jul 26 09:24:49 2023, max compression
```

## Comparing `pydactim-0.0.5.tar` & `pydactim-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:23:51.965686 pydactim-0.0.5/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:23:51.965686 pydactim-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 09:23:51.949686 pydactim-0.0.5/pydactim/
--rw-rw-rw-   0        0        0      158 2023-07-26 08:07:58.000000 pydactim-0.0.5/pydactim/__init__.py
--rw-rw-rw-   0        0        0     4245 2023-05-04 09:31:52.000000 pydactim-0.0.5/pydactim/anonymization.py
--rw-rw-rw-   0        0        0    30210 2023-06-19 09:22:31.000000 pydactim-0.0.5/pydactim/brain_extraction.py
--rw-rw-rw-   0        0        0      927 2023-07-26 08:11:37.000000 pydactim-0.0.5/pydactim/computation.py
--rw-rw-rw-   0        0        0     3935 2023-05-03 14:18:41.000000 pydactim-0.0.5/pydactim/conversion.py
--rw-rw-rw-   0        0        0     1744 2023-07-26 07:37:37.000000 pydactim-0.0.5/pydactim/data.py
--rw-rw-rw-   0        0        0    24158 2023-07-26 07:52:07.000000 pydactim-0.0.5/pydactim/new_transformation.py
--rw-rw-rw-   0        0        0     2411 2023-07-26 09:22:09.000000 pydactim-0.0.5/pydactim/sorting.py
--rw-rw-rw-   0        0        0     3100 2023-07-26 09:22:13.000000 pydactim-0.0.5/pydactim/spectroscopy.py
--rw-rw-rw-   0        0        0    23291 2023-07-26 07:56:30.000000 pydactim-0.0.5/pydactim/transformation.py
--rw-rw-rw-   0        0        0      996 2022-12-12 13:23:53.000000 pydactim-0.0.5/pydactim/utils.py
--rw-rw-rw-   0        0        0     6361 2023-07-26 09:22:21.000000 pydactim-0.0.5/pydactim/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:23:51.963685 pydactim-0.0.5/pydactim.egg-info/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:23:51.000000 pydactim-0.0.5/pydactim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-07-26 09:23:51.000000 pydactim-0.0.5/pydactim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:23:51.000000 pydactim-0.0.5/pydactim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-26 09:23:51.000000 pydactim-0.0.5/pydactim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 09:23:51.000000 pydactim-0.0.5/pydactim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      174 2023-07-26 09:23:51.966685 pydactim-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-07-26 09:23:40.000000 pydactim-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:24:49.486411 pydactim-0.0.6/
+-rw-rw-rw-   0        0        0      384 2023-07-26 09:24:49.486411 pydactim-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 09:24:49.473411 pydactim-0.0.6/pydactim/
+-rw-rw-rw-   0        0        0      158 2023-07-26 08:07:58.000000 pydactim-0.0.6/pydactim/__init__.py
+-rw-rw-rw-   0        0        0     4245 2023-05-04 09:31:52.000000 pydactim-0.0.6/pydactim/anonymization.py
+-rw-rw-rw-   0        0        0    30210 2023-06-19 09:22:31.000000 pydactim-0.0.6/pydactim/brain_extraction.py
+-rw-rw-rw-   0        0        0      927 2023-07-26 08:11:37.000000 pydactim-0.0.6/pydactim/computation.py
+-rw-rw-rw-   0        0        0     3935 2023-05-03 14:18:41.000000 pydactim-0.0.6/pydactim/conversion.py
+-rw-rw-rw-   0        0        0     1744 2023-07-26 07:37:37.000000 pydactim-0.0.6/pydactim/data.py
+-rw-rw-rw-   0        0        0    24158 2023-07-26 07:52:07.000000 pydactim-0.0.6/pydactim/new_transformation.py
+-rw-rw-rw-   0        0        0     2411 2023-07-26 09:22:09.000000 pydactim-0.0.6/pydactim/sorting.py
+-rw-rw-rw-   0        0        0     3100 2023-07-26 09:22:13.000000 pydactim-0.0.6/pydactim/spectroscopy.py
+-rw-rw-rw-   0        0        0    23291 2023-07-26 07:56:30.000000 pydactim-0.0.6/pydactim/transformation.py
+-rw-rw-rw-   0        0        0      996 2022-12-12 13:23:53.000000 pydactim-0.0.6/pydactim/utils.py
+-rw-rw-rw-   0        0        0     6361 2023-07-26 09:22:21.000000 pydactim-0.0.6/pydactim/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:24:49.485412 pydactim-0.0.6/pydactim.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-07-26 09:24:49.000000 pydactim-0.0.6/pydactim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-07-26 09:24:49.000000 pydactim-0.0.6/pydactim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:24:49.000000 pydactim-0.0.6/pydactim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-26 09:24:49.000000 pydactim-0.0.6/pydactim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 09:24:49.000000 pydactim-0.0.6/pydactim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      174 2023-07-26 09:24:49.487411 pydactim-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-07-26 09:24:41.000000 pydactim-0.0.6/setup.py
```

### Comparing `pydactim-0.0.5/README.md` & `pydactim-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/anonymization.py` & `pydactim-0.0.6/pydactim/anonymization.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/brain_extraction.py` & `pydactim-0.0.6/pydactim/brain_extraction.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/computation.py` & `pydactim-0.0.6/pydactim/computation.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/conversion.py` & `pydactim-0.0.6/pydactim/conversion.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/data.py` & `pydactim-0.0.6/pydactim/data.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/new_transformation.py` & `pydactim-0.0.6/pydactim/new_transformation.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/sorting.py` & `pydactim-0.0.6/pydactim/sorting.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/spectroscopy.py` & `pydactim-0.0.6/pydactim/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/transformation.py` & `pydactim-0.0.6/pydactim/transformation.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/utils.py` & `pydactim-0.0.6/pydactim/utils.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/pydactim/visualization.py` & `pydactim-0.0.6/pydactim/visualization.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.5/setup.py` & `pydactim-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # from sphinx.setup_command import BuildDoc
 # cmdclass = {'build_sphinx': BuildDoc}
 
 from setuptools import setup, find_packages
 
 setup(name='pydactim',
       python_requires='>=3.7',
-      version='0.0.5',
+      version='0.0.6',
       packages=find_packages(),
       install_requires=[
         "torch>=1.13.1",
         "torchio>=0.18.86",
         "SimpleITK",
         "numpy",
         "nibabel",
```

