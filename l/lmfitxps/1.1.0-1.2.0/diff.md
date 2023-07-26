# Comparing `tmp/lmfitxps-1.1.0.tar.gz` & `tmp/lmfitxps-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/Julian Hochhaus/github/lmfit-additional-models/lmfitxps/dist/.tmp-liifhgro/lmfitxps-1.1.0.tar", last modified: Tue Jul 18 12:24:50 2023, max compression
+gzip compressed data, was "/home/julian/Desktop/lmfit-additional-models/dist/.tmp-x9u_r598/lmfitxps-1.2.0.tar", last modified: Wed Jul 26 15:01:05 2023, max compression
```

## Comparing `lmfitxps-1.1.0.tar` & `lmfitxps-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-18 12:24:50.776673 lmfitxps-1.1.0/
--rwxrwxrwx   0 julian    (1000) julian    (1000)     3057 2023-05-19 08:21:46.000000 lmfitxps-1.1.0/LICENSE
--rwxrwxrwx   0 julian    (1000) julian    (1000)     4807 2023-07-18 12:24:50.771673 lmfitxps-1.1.0/PKG-INFO
--rwxrwxrwx   0 julian    (1000) julian    (1000)      824 2023-07-18 11:25:59.000000 lmfitxps-1.1.0/README.md
--rwxrwxrwx   0 julian    (1000) julian    (1000)      583 2023-07-18 12:23:46.000000 lmfitxps-1.1.0/pyproject.toml
--rwxrwxrwx   0 julian    (1000) julian    (1000)       38 2023-07-18 12:24:50.777671 lmfitxps-1.1.0/setup.cfg
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-18 12:24:50.704714 lmfitxps-1.1.0/src/
--rwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-14 12:12:35.000000 lmfitxps-1.1.0/src/__init__.py
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-18 12:24:50.729699 lmfitxps-1.1.0/src/lmfitxps/
--rwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-14 14:03:11.000000 lmfitxps-1.1.0/src/lmfitxps/__init__.py
--rwxrwxrwx   0 julian    (1000) julian    (1000)     5489 2023-07-18 12:17:23.000000 lmfitxps-1.1.0/src/lmfitxps/functions.py
--rwxrwxrwx   0 julian    (1000) julian    (1000)    25426 2023-07-18 12:17:45.000000 lmfitxps-1.1.0/src/lmfitxps/models.py
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-18 12:24:50.766678 lmfitxps-1.1.0/src/lmfitxps.egg-info/
--rwxrwxrwx   0 julian    (1000) julian    (1000)     4807 2023-07-18 12:24:50.000000 lmfitxps-1.1.0/src/lmfitxps.egg-info/PKG-INFO
--rwxrwxrwx   0 julian    (1000) julian    (1000)      266 2023-07-18 12:24:50.000000 lmfitxps-1.1.0/src/lmfitxps.egg-info/SOURCES.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)        1 2023-07-18 12:24:50.000000 lmfitxps-1.1.0/src/lmfitxps.egg-info/dependency_links.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)       18 2023-07-18 12:24:50.000000 lmfitxps-1.1.0/src/lmfitxps.egg-info/top_level.txt
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/
+-rw-rw-r--   0 julian    (1000) julian    (1000)     3057 2023-07-25 12:03:21.000000 lmfitxps-1.2.0/LICENSE
+-rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)     1412 2023-07-25 12:04:12.000000 lmfitxps-1.2.0/README.md
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.360823 lmfitxps-1.2.0/lmfitxps/
+-rw-rw-r--   0 julian    (1000) julian    (1000)        0 2023-07-25 12:03:21.000000 lmfitxps-1.2.0/lmfitxps/__init__.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    12073 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/backgrounds.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     7048 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/lineshapes.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    12986 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/models.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.360823 lmfitxps-1.2.0/lmfitxps.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      273 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        9 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)      552 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/pyproject.toml
+-rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/setup.cfg
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/tests/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      209 2023-07-26 13:48:02.000000 lmfitxps-1.2.0/tests/test_backgrounds.py
```

### Comparing `lmfitxps-1.1.0/LICENSE` & `lmfitxps-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfitxps-1.1.0/PKG-INFO` & `lmfitxps-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfitxps
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package contains additional models for the lmfit package for fitting XPS spectra.
 Author-email: Julian Hochhaus <julian.hochhaus@tu-dortmund.de>
 License: MIT License
         
         Copyright (c) 2023 Julian-Hochhaus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,27 +61,30 @@
         CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
         SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
         INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
         CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
         ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
         POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: homepage, https://github.com/Julian-Hochhaus/lmfit-additional-models
-Project-URL: documentation, https://lmfit-additional-models.readthedocs.io/en/latest/#
+Project-URL: homepage, https://github.com/Julian-Hochhaus/lmfitxps
+Project-URL: documentation, https://lmfitxps.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lmfitxps
-__version__=
-This package contains additional models for the lmfit package. The
-models are designed for fitting XPS spectra.
+## Introduction
+Welcome to lmfitxps, a small Python package designed as an extension for the popular lmfit package , specifically tailored for X-ray Photoelectron Spectroscopy (XPS) data analysis.
 
-This package contains background models such as Shirley, Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models. In
-addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge.
+While lmfit provides simple tools to build complex fitting models for non-linear least-squares problems and applies these models to real data, as well as introduces several built-in models, lmfitxps acts as an extension to lmfit designed for XPS data analysis. lmfitxps provides a comprehensive set of functions and models that facilitate the fitting of XPS spectra. In particular, lmfitxps provides several models, which use the convolution of a gaussian with model functions of the lmfit-package.
 
-The models are based on the lmfit package and can be used in the same way as the models from lmfit. 
+In addition to models for fittig signals in XPS data, lmfitxps introduces several background models which can be included in the fit model for fitting the data rather then substracting a precalculated background. This is the so-called active approach as suggested by A. Herrera-Gomez and generally leads to better fit results.
+For further details, please refer to the documentation of [lmfitxps](https://lmfitxps.readthedocs.io/en/latest/index.html) and [lmfit](https://lmfit.github.io/lmfit-py/index.html)! 
 
-For more details, see the [documentation](https://lmfit-additional-models.readthedocs.io/en/latest/#). 
+## Installation
+To install lmfitxps, simply use pip:
+
+ `pip install lmfitxps`
+
+ ## How to cite
+ [![DOI](https://zenodo.org/badge/642726930.svg)](https://zenodo.org/badge/latestdoi/642726930)
 
-Feel free to contribute to this package by adding new models or improving existing ones. 
 
-Visit on GitHub: [lmfit-additional-models](https://github.com/Julian-Hochhaus/lmfit-additional-models)
```

### Comparing `lmfitxps-1.1.0/src/lmfitxps.egg-info/PKG-INFO` & `lmfitxps-1.2.0/lmfitxps.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfitxps
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package contains additional models for the lmfit package for fitting XPS spectra.
 Author-email: Julian Hochhaus <julian.hochhaus@tu-dortmund.de>
 License: MIT License
         
         Copyright (c) 2023 Julian-Hochhaus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,27 +61,30 @@
         CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
         SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
         INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
         CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
         ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
         POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: homepage, https://github.com/Julian-Hochhaus/lmfit-additional-models
-Project-URL: documentation, https://lmfit-additional-models.readthedocs.io/en/latest/#
+Project-URL: homepage, https://github.com/Julian-Hochhaus/lmfitxps
+Project-URL: documentation, https://lmfitxps.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lmfitxps
-__version__=
-This package contains additional models for the lmfit package. The
-models are designed for fitting XPS spectra.
+## Introduction
+Welcome to lmfitxps, a small Python package designed as an extension for the popular lmfit package , specifically tailored for X-ray Photoelectron Spectroscopy (XPS) data analysis.
 
-This package contains background models such as Shirley, Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models. In
-addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge.
+While lmfit provides simple tools to build complex fitting models for non-linear least-squares problems and applies these models to real data, as well as introduces several built-in models, lmfitxps acts as an extension to lmfit designed for XPS data analysis. lmfitxps provides a comprehensive set of functions and models that facilitate the fitting of XPS spectra. In particular, lmfitxps provides several models, which use the convolution of a gaussian with model functions of the lmfit-package.
 
-The models are based on the lmfit package and can be used in the same way as the models from lmfit. 
+In addition to models for fittig signals in XPS data, lmfitxps introduces several background models which can be included in the fit model for fitting the data rather then substracting a precalculated background. This is the so-called active approach as suggested by A. Herrera-Gomez and generally leads to better fit results.
+For further details, please refer to the documentation of [lmfitxps](https://lmfitxps.readthedocs.io/en/latest/index.html) and [lmfit](https://lmfit.github.io/lmfit-py/index.html)! 
 
-For more details, see the [documentation](https://lmfit-additional-models.readthedocs.io/en/latest/#). 
+## Installation
+To install lmfitxps, simply use pip:
+
+ `pip install lmfitxps`
+
+ ## How to cite
+ [![DOI](https://zenodo.org/badge/642726930.svg)](https://zenodo.org/badge/latestdoi/642726930)
 
-Feel free to contribute to this package by adding new models or improving existing ones. 
 
-Visit on GitHub: [lmfit-additional-models](https://github.com/Julian-Hochhaus/lmfit-additional-models)
```

