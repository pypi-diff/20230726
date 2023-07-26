# Comparing `tmp/quant-alchemy-0.1.1.tar.gz` & `tmp/quant-alchemy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant-alchemy-0.1.1.tar", last modified: Wed Jul 26 17:46:52 2023, max compression
+gzip compressed data, was "quant-alchemy-0.1.2.tar", last modified: Wed Jul 26 18:54:28 2023, max compression
```

## Comparing `quant-alchemy-0.1.1.tar` & `quant-alchemy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:46:52.116909 quant-alchemy-0.1.1/
--rw-rw-rw-   0        0        0      400 2023-07-26 17:46:52.115906 quant-alchemy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 17:46:52.110392 quant-alchemy-0.1.1/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 17:45:57.000000 quant-alchemy-0.1.1/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.1/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    14526 2023-07-12 19:18:04.000000 quant-alchemy-0.1.1/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:46:52.114904 quant-alchemy-0.1.1/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-07-26 17:46:51.000000 quant-alchemy-0.1.1/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-26 17:46:52.000000 quant-alchemy-0.1.1/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:46:51.000000 quant-alchemy-0.1.1/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 17:46:51.000000 quant-alchemy-0.1.1/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 17:46:51.000000 quant-alchemy-0.1.1/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:46:52.116909 quant-alchemy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-07-26 17:46:28.000000 quant-alchemy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/
+-rw-rw-rw-   0        0        0      400 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.855736 quant-alchemy-0.1.2/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:53:42.000000 quant-alchemy-0.1.2/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.2/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    14526 2023-07-12 19:18:04.000000 quant-alchemy-0.1.2/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.860736 quant-alchemy-0.1.2/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-07-26 18:54:23.000000 quant-alchemy-0.1.2/setup.py
```

### Comparing `quant-alchemy-0.1.1/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.2/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.1/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.2/quant_alchemy/timeseries.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.1/setup.py` & `quant-alchemy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.1",
+    version="0.1.2",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

