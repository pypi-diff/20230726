# Comparing `tmp/pydactim-0.0.1.tar.gz` & `tmp/pydactim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydactim-0.0.1.tar", last modified: Wed Jul 26 09:14:52 2023, max compression
+gzip compressed data, was "dist\pydactim-0.0.2.tar", last modified: Wed Jul 26 09:17:29 2023, max compression
```

## Comparing `pydactim-0.0.1.tar` & `pydactim-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:14:52.702952 pydactim-0.0.1/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:14:52.702952 pydactim-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 09:14:52.701951 pydactim-0.0.1/pydactim.egg-info/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:14:52.000000 pydactim-0.0.1/pydactim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-26 09:14:52.000000 pydactim-0.0.1/pydactim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:14:52.000000 pydactim-0.0.1/pydactim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-26 09:14:52.000000 pydactim-0.0.1/pydactim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:14:52.000000 pydactim-0.0.1/pydactim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      174 2023-07-26 09:14:52.703951 pydactim-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-07-26 09:14:38.000000 pydactim-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:17:29.734625 pydactim-0.0.2/
+-rw-rw-rw-   0        0        0      384 2023-07-26 09:17:29.734625 pydactim-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 09:17:29.724619 pydactim-0.0.2/pydactim.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-07-26 09:17:29.000000 pydactim-0.0.2/pydactim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-26 09:17:29.000000 pydactim-0.0.2/pydactim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:17:29.000000 pydactim-0.0.2/pydactim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-26 09:17:29.000000 pydactim-0.0.2/pydactim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 09:17:29.000000 pydactim-0.0.2/pydactim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      174 2023-07-26 09:17:29.735650 pydactim-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-07-26 09:17:15.000000 pydactim-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:17:29.733619 pydactim-0.0.2/src/
+-rw-rw-rw-   0        0        0      158 2023-07-26 08:07:58.000000 pydactim-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     4245 2023-05-04 09:31:52.000000 pydactim-0.0.2/src/anonymization.py
+-rw-rw-rw-   0        0        0    30210 2023-06-19 09:22:31.000000 pydactim-0.0.2/src/brain_extraction.py
+-rw-rw-rw-   0        0        0      927 2023-07-26 08:11:37.000000 pydactim-0.0.2/src/computation.py
+-rw-rw-rw-   0        0        0     3935 2023-05-03 14:18:41.000000 pydactim-0.0.2/src/conversion.py
+-rw-rw-rw-   0        0        0     1744 2023-07-26 07:37:37.000000 pydactim-0.0.2/src/data.py
+-rw-rw-rw-   0        0        0    24158 2023-07-26 07:52:07.000000 pydactim-0.0.2/src/new_transformation.py
+-rw-rw-rw-   0        0        0     2413 2023-05-03 13:53:07.000000 pydactim-0.0.2/src/sorting.py
+-rw-rw-rw-   0        0        0     3102 2023-01-26 16:07:29.000000 pydactim-0.0.2/src/spectroscopy.py
+-rw-rw-rw-   0        0        0    23291 2023-07-26 07:56:30.000000 pydactim-0.0.2/src/transformation.py
+-rw-rw-rw-   0        0        0      996 2022-12-12 13:23:53.000000 pydactim-0.0.2/src/utils.py
+-rw-rw-rw-   0        0        0     6363 2023-07-26 08:20:05.000000 pydactim-0.0.2/src/visualization.py
```

### Comparing `pydactim-0.0.1/README.md` & `pydactim-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.1/setup.py` & `pydactim-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # from sphinx.setup_command import BuildDoc
 # cmdclass = {'build_sphinx': BuildDoc}
 
 from setuptools import setup, find_packages
 
 setup(name='pydactim',
       python_requires='>=3.7',
-      version='0.0.1',
+      version='0.0.2',
       packages=find_packages(),
       install_requires=[
         "torch>=1.13.1",
         "torchio>=0.18.86",
         "SimpleITK",
         "numpy",
         "nibabel",
```

