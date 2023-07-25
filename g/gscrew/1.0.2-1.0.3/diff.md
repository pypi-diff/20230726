# Comparing `tmp/gscrew-1.0.2.tar.gz` & `tmp/gscrew-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscrew-1.0.2.tar", last modified: Tue Jul 25 10:02:09 2023, max compression
+gzip compressed data, was "gscrew-1.0.3.tar", last modified: Tue Jul 25 21:57:00 2023, max compression
```

## Comparing `gscrew-1.0.2.tar` & `gscrew-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:02:09.519647 gscrew-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:01:57.000000 gscrew-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-25 10:02:09.519647 gscrew-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 10:01:57.000000 gscrew-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:02:09.519647 gscrew-1.0.2/gscrew/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 10:01:57.000000 gscrew-1.0.2/gscrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 10:01:57.000000 gscrew-1.0.2/gscrew/geometric_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-25 10:01:57.000000 gscrew-1.0.2/gscrew/screw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:02:09.519647 gscrew-1.0.2/gscrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-25 10:02:09.000000 gscrew-1.0.2/gscrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 10:02:09.000000 gscrew-1.0.2/gscrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:02:09.000000 gscrew-1.0.2/gscrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 10:02:09.000000 gscrew-1.0.2/gscrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 10:02:09.000000 gscrew-1.0.2/gscrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 10:01:57.000000 gscrew-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:01:57.000000 gscrew-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:02:09.519647 gscrew-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 10:01:57.000000 gscrew-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:00.787596 gscrew-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:56:45.000000 gscrew-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 21:57:00.783596 gscrew-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 21:56:45.000000 gscrew-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:00.783596 gscrew-1.0.3/gscrew/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 21:56:45.000000 gscrew-1.0.3/gscrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 21:56:45.000000 gscrew-1.0.3/gscrew/geometric_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-25 21:56:45.000000 gscrew-1.0.3/gscrew/screw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:00.783596 gscrew-1.0.3/gscrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 21:57:00.000000 gscrew-1.0.3/gscrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 21:57:00.000000 gscrew-1.0.3/gscrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:57:00.000000 gscrew-1.0.3/gscrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 21:57:00.000000 gscrew-1.0.3/gscrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 21:57:00.000000 gscrew-1.0.3/gscrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 21:56:45.000000 gscrew-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:56:45.000000 gscrew-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:57:00.787596 gscrew-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 21:56:45.000000 gscrew-1.0.3/setup.py
```

### Comparing `gscrew-1.0.2/LICENSE` & `gscrew-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gscrew-1.0.2/PKG-INFO` & `gscrew-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
 [![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
-A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
+A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
 - [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
 - [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
```

### Comparing `gscrew-1.0.2/README.md` & `gscrew-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
 [![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
-A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
+A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
 - [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
 - [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
```

### Comparing `gscrew-1.0.2/gscrew/geometric_algebra.py` & `gscrew-1.0.3/gscrew/geometric_algebra.py`

 * *Files identical despite different names*

### Comparing `gscrew-1.0.2/gscrew/screw.py` & `gscrew-1.0.3/gscrew/screw.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,16 @@
             raise TypeError(f"other must be a Screw instance instead of {type(other)}")
 
         if self.ref_point != other.ref_point:
             other = other.change_point(self.ref_point)
 
         return Screw(
                 self.ref_point,
-                self.direction ^ other.moment + self.moment.grade_involution() ^ other.direction,
+                (self.direction ^ other.moment) + (self.moment.grade_involution() ^
+                        other.direction),
                 self.moment ^ other.moment
             )
 
 
 class CoScrew(ScrewBase):
     """Coscrew object
```

### Comparing `gscrew-1.0.2/gscrew.egg-info/PKG-INFO` & `gscrew-1.0.3/gscrew.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
 [![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
-A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
+A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
 - [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
 - [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
```

### Comparing `gscrew-1.0.2/pyproject.toml` & `gscrew-1.0.3/pyproject.toml`

 * *Files identical despite different names*

