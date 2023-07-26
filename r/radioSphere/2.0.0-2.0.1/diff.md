# Comparing `tmp/radioSphere-2.0.0.tar.gz` & `tmp/radioSphere-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioSphere-2.0.0.tar", last modified: Wed Jul 26 08:05:05 2023, max compression
+gzip compressed data, was "radioSphere-2.0.1.tar", last modified: Wed Jul 26 11:10:02 2023, max compression
```

## Comparing `radioSphere-2.0.0.tar` & `radioSphere-2.0.1.tar`

### file list

```diff
@@ -1,85 +1,92 @@
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.838757 radioSphere-2.0.0/
--rw-r--r--   0 ed        (1000) users      (100)    32359 2021-03-15 20:37:50.000000 radioSphere-2.0.0/LICENSE.md
--rw-r--r--   0 ed        (1000) users      (100)       40 2023-07-26 07:54:01.000000 radioSphere-2.0.0/MANIFEST.in
--rw-r--r--   0 ed        (1000) users      (100)     5387 2023-07-26 08:05:05.838757 radioSphere-2.0.0/PKG-INFO
--rw-r--r--   0 ed        (1000) users      (100)     4222 2023-07-26 07:54:01.000000 radioSphere-2.0.0/README.md
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/docs/
--rw-r--r--   0 ed        (1000) users      (100)      639 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/Makefile
--rw-r--r--   0 ed        (1000) users      (100)       71 2021-06-03 07:11:07.000000 radioSphere-2.0.0/docs/index.html
--rw-r--r--   0 ed        (1000) users      (100)      800 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/make.bat
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/docs/source/
--rw-r--r--   0 ed        (1000) users      (100)     2455 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/source/conf.py
--rw-r--r--   0 ed        (1000) users      (100)     1465 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/source/index.rst
--rw-r--r--   0 ed        (1000) users      (100)     4798 2021-06-03 07:11:07.000000 radioSphere-2.0.0/docs/source/logo.png
--rw-r--r--   0 ed        (1000) users      (100)      991 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/source/modules.rst
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/docs/source/notebooks/
--rw-r--r--   0 ed        (1000) users      (100)   244003 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/source/notebooks/Running radioSphere on artificial data.ipynb
--rw-r--r--   0 ed        (1000) users      (100)   478025 2023-07-26 07:54:01.000000 radioSphere-2.0.0/docs/source/notebooks/Running radioSphere on experimental data.ipynb
--rw-r--r--   0 ed        (1000) users      (100)     2630 2023-07-26 07:54:01.000000 radioSphere-2.0.0/pyproject.toml
--rw-r--r--   0 ed        (1000) users      (100)       38 2023-07-26 08:05:05.838757 radioSphere-2.0.0/setup.cfg
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.826757 radioSphere-2.0.0/src/
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/src/radioSphere/
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/src/radioSphere/DEM/
--rw-r--r--   0 ed        (1000) users      (100)     2013 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/DEM/DEM.py
--rw-r--r--   0 ed        (1000) users      (100)      142 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/DEM/__init__.py
--rw-r--r--   0 ed        (1000) users      (100)     5558 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/DEM/mercury.py
--rw-r--r--   0 ed        (1000) users      (100)     1132 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/DEM/nddem.py
--rw-r--r--   0 ed        (1000) users      (100)      456 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/__init__.py
--rwxr-xr-x   0 ed        (1000) users      (100)     4206 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/blender_viewer.py
--rw-r--r--   0 ed        (1000) users      (100)    15136 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/calibrateAttenuation.py
--rw-r--r--   0 ed        (1000) users      (100)    50796 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/detectSpheres.py
--rw-r--r--   0 ed        (1000) users      (100)    36010 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/optimisePositions.py
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.834757 radioSphere-2.0.0/src/radioSphere/projectSphere/
--rw-r--r--   0 ed        (1000) users      (100)     7885 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/projectSphere/CupyProjector.py
--rw-r--r--   0 ed        (1000) users      (100)     2943 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/projectSphere/NumbaProjector.py
--rw-r--r--   0 ed        (1000) users      (100)      259 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/projectSphere/__init__.py
--rw-r--r--   0 ed        (1000) users      (100)    33513 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/projectSphere/projectSphere.py
--rw-r--r--   0 ed        (1000) users      (100)      979 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/projectSphere/projectorSpeedTest.py
--rw-r--r--   0 ed        (1000) users      (100)      539 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/radioSphere.mplstyle
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.834757 radioSphere-2.0.0/src/radioSphere/scripts/
--rw-r--r--   0 ed        (1000) users      (100)      136 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/__init__.py
--rw-r--r--   0 ed        (1000) users      (100)     2775 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/calibrateManyParticles.py
--rw-r--r--   0 ed        (1000) users      (100)     2951 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/calibrateSingleParticle.py
--rw-r--r--   0 ed        (1000) users      (100)     3495 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/findParticles.py
--rw-r--r--   0 ed        (1000) users      (100)     8177 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/generate_particles_with_shells.py
--rw-r--r--   0 ed        (1000) users      (100)     3674 2023-07-26 07:54:01.000000 radioSphere-2.0.0/src/radioSphere/scripts/optimiseParticles.py
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.830757 radioSphere-2.0.0/src/radioSphere.egg-info/
--rw-r--r--   0 ed        (1000) users      (100)     5387 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) users      (100)     2919 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) users      (100)        1 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) users      (100)      284 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) users      (100)      168 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) users      (100)       12 2023-07-26 08:05:05.000000 radioSphere-2.0.0/src/radioSphere.egg-info/top_level.txt
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.834757 radioSphere-2.0.0/tests/
--rw-r--r--   0 ed        (1000) users      (100)      159 2023-07-26 07:54:01.000000 radioSphere-2.0.0/tests/__init__.py
-drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 08:05:05.838757 radioSphere-2.0.0/tests/__pycache__/
--rw-r--r--   0 ed        (1000) users      (100)      303 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 ed        (1000) users      (100)      307 2022-01-25 10:37:51.000000 radioSphere-2.0.0/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 ed        (1000) users      (100)     1673 2020-05-10 18:54:14.000000 radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     2076 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0 ed        (1000) users      (100)     1564 2020-10-15 11:40:21.000000 radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     1747 2022-01-25 10:37:51.000000 radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     2522 2021-12-03 12:54:18.000000 radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     2484 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-37-pytest-7.1.2.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     2863 2022-01-25 10:37:52.000000 radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     6910 2021-12-03 12:54:20.000000 radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     7252 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-37-pytest-7.1.2.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     6916 2022-01-25 10:37:52.000000 radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     8588 2021-12-03 12:54:20.000000 radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     8656 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0 ed        (1000) users      (100)     6939 2020-10-15 11:40:20.000000 radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     8221 2022-01-25 10:37:52.000000 radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     5406 2020-05-10 18:54:15.000000 radioSphere-2.0.0/tests/__pycache__/test_optimiser_sensitivityField.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     9030 2021-12-03 12:54:20.000000 radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     9591 2023-07-25 08:38:19.000000 radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37-pytest-7.1.2.pyc
--rw-r--r--   0 ed        (1000) users      (100)     7856 2020-10-15 11:40:21.000000 radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     9181 2022-01-25 10:37:52.000000 radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     1616 2021-12-03 12:54:20.000000 radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-37-pytest-5.4.1.pyc
--rw-r--r--   0 ed        (1000) users      (100)     1620 2023-07-25 08:38:20.000000 radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-37-pytest-7.1.2.pyc
--rw-rw-r--   0 ed        (1000) users      (100)     1642 2022-01-25 10:37:52.000000 radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 ed        (1000) users      (100)     2104 2023-07-26 07:54:01.000000 radioSphere-2.0.0/tests/test_DEM.py
--rw-r--r--   0 ed        (1000) users      (100)     3743 2023-07-26 07:54:01.000000 radioSphere-2.0.0/tests/test_cleaner.py
--rw-r--r--   0 ed        (1000) users      (100)    12664 2023-07-26 07:54:01.000000 radioSphere-2.0.0/tests/test_detection.py
--rw-r--r--   0 ed        (1000) users      (100)    17446 2023-07-26 07:54:01.000000 radioSphere-2.0.0/tests/test_optimiser.py
--rw-r--r--   0 ed        (1000) users      (100)    19746 2023-07-26 07:55:29.000000 radioSphere-2.0.0/tests/test_projector.py
--rw-r--r--   0 ed        (1000) users      (100)     1993 2021-04-12 16:42:36.000000 radioSphere-2.0.0/tests/test_tomopack.py
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/
+-rw-r--r--   0 ed        (1000) users      (100)    32359 2021-03-15 20:37:50.000000 radioSphere-2.0.1/LICENSE.md
+-rw-r--r--   0 ed        (1000) users      (100)       40 2023-07-26 07:54:01.000000 radioSphere-2.0.1/MANIFEST.in
+-rw-r--r--   0 ed        (1000) users      (100)     4788 2023-07-26 11:10:02.516046 radioSphere-2.0.1/PKG-INFO
+-rw-r--r--   0 ed        (1000) users      (100)     3573 2023-07-26 09:53:15.000000 radioSphere-2.0.1/README.md
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.512046 radioSphere-2.0.1/docs/
+-rw-r--r--   0 ed        (1000) users      (100)      639 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/Makefile
+-rw-r--r--   0 ed        (1000) users      (100)       71 2021-06-03 07:11:07.000000 radioSphere-2.0.1/docs/index.html
+-rw-r--r--   0 ed        (1000) users      (100)      800 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/make.bat
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/docs/source/
+-rw-r--r--   0 ed        (1000) users      (100)     2455 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/source/conf.py
+-rw-r--r--   0 ed        (1000) users      (100)     1465 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/source/index.rst
+-rw-r--r--   0 ed        (1000) users      (100)     4798 2021-06-03 07:11:07.000000 radioSphere-2.0.1/docs/source/logo.png
+-rw-r--r--   0 ed        (1000) users      (100)      991 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/source/modules.rst
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/docs/source/notebooks/
+-rw-r--r--   0 ed        (1000) users      (100)   244003 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/source/notebooks/Running radioSphere on artificial data.ipynb
+-rw-r--r--   0 ed        (1000) users      (100)   478025 2023-07-26 07:54:01.000000 radioSphere-2.0.1/docs/source/notebooks/Running radioSphere on experimental data.ipynb
+-rw-r--r--   0 ed        (1000) users      (100)     2693 2023-07-26 10:01:59.000000 radioSphere-2.0.1/pyproject.toml
+-rw-r--r--   0 ed        (1000) users      (100)       38 2023-07-26 11:10:02.516046 radioSphere-2.0.1/setup.cfg
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.512046 radioSphere-2.0.1/src/
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/src/radioSphere/
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/src/radioSphere/DEM/
+-rw-r--r--   0 ed        (1000) users      (100)     2013 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/DEM/DEM.py
+-rw-r--r--   0 ed        (1000) users      (100)      142 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/DEM/__init__.py
+-rw-r--r--   0 ed        (1000) users      (100)     5559 2023-07-26 09:38:31.000000 radioSphere-2.0.1/src/radioSphere/DEM/mercury.py
+-rw-r--r--   0 ed        (1000) users      (100)     1132 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/DEM/nddem.py
+-rw-r--r--   0 ed        (1000) users      (100)      456 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/__init__.py
+-rwxr-xr-x   0 ed        (1000) users      (100)     4206 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/blender_viewer.py
+-rw-r--r--   0 ed        (1000) users      (100)    15116 2023-07-26 09:35:09.000000 radioSphere-2.0.1/src/radioSphere/calibrateAttenuation.py
+-rw-r--r--   0 ed        (1000) users      (100)    50798 2023-07-26 09:38:07.000000 radioSphere-2.0.1/src/radioSphere/detectSpheres.py
+-rw-r--r--   0 ed        (1000) users      (100)    36010 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/optimisePositions.py
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/src/radioSphere/projectSphere/
+-rw-r--r--   0 ed        (1000) users      (100)     7885 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/projectSphere/CupyProjector.py
+-rw-r--r--   0 ed        (1000) users      (100)     2943 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/projectSphere/NumbaProjector.py
+-rw-r--r--   0 ed        (1000) users      (100)      259 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/projectSphere/__init__.py
+-rw-r--r--   0 ed        (1000) users      (100)    33513 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/projectSphere/projectSphere.py
+-rw-r--r--   0 ed        (1000) users      (100)      979 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/projectSphere/projectorSpeedTest.py
+-rw-r--r--   0 ed        (1000) users      (100)      539 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/radioSphere.mplstyle
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/src/radioSphere/scripts/
+-rw-r--r--   0 ed        (1000) users      (100)      136 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/__init__.py
+-rw-r--r--   0 ed        (1000) users      (100)     2775 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/calibrateManyParticles.py
+-rw-r--r--   0 ed        (1000) users      (100)     2951 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/calibrateSingleParticle.py
+-rw-r--r--   0 ed        (1000) users      (100)     3495 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/findParticles.py
+-rw-r--r--   0 ed        (1000) users      (100)     8177 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/generate_particles_with_shells.py
+-rw-r--r--   0 ed        (1000) users      (100)     3674 2023-07-26 07:54:01.000000 radioSphere-2.0.1/src/radioSphere/scripts/optimiseParticles.py
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/src/radioSphere.egg-info/
+-rw-r--r--   0 ed        (1000) users      (100)     4788 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) users      (100)     3325 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) users      (100)        1 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) users      (100)      284 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) users      (100)      172 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) users      (100)       12 2023-07-26 11:10:02.000000 radioSphere-2.0.1/src/radioSphere.egg-info/top_level.txt
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/tests/
+-rw-r--r--   0 ed        (1000) users      (100)      159 2023-07-26 07:54:01.000000 radioSphere-2.0.1/tests/__init__.py
+drwxr-xr-x   0 ed        (1000) users      (100)        0 2023-07-26 11:10:02.516046 radioSphere-2.0.1/tests/__pycache__/
+-rw-r--r--   0 ed        (1000) users      (100)      309 2023-07-26 09:12:18.000000 radioSphere-2.0.1/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ed        (1000) users      (100)      303 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ed        (1000) users      (100)      307 2022-01-25 10:37:51.000000 radioSphere-2.0.1/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2160 2023-07-26 09:12:18.000000 radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     1673 2020-05-10 18:54:14.000000 radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2076 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37-pytest-7.1.2.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     1564 2020-10-15 11:40:21.000000 radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     1747 2022-01-25 10:37:51.000000 radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2901 2023-07-26 09:12:19.000000 radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2522 2021-12-03 12:54:18.000000 radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2484 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-37-pytest-7.1.2.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     2863 2022-01-25 10:37:52.000000 radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     7169 2023-07-26 09:12:19.000000 radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     6910 2021-12-03 12:54:20.000000 radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     7252 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-37-pytest-7.1.2.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     6916 2022-01-25 10:37:52.000000 radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     8339 2023-07-26 09:12:19.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     8588 2021-12-03 12:54:20.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     8656 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37-pytest-7.1.2.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     6939 2020-10-15 11:40:20.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     8221 2022-01-25 10:37:52.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     5406 2020-05-10 18:54:15.000000 radioSphere-2.0.1/tests/__pycache__/test_optimiser_sensitivityField.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     9937 2023-07-26 09:12:19.000000 radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     9030 2021-12-03 12:54:20.000000 radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     9591 2023-07-25 08:38:19.000000 radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37-pytest-7.1.2.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     7856 2020-10-15 11:40:21.000000 radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     9181 2022-01-25 10:37:52.000000 radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     1654 2023-07-26 09:12:19.000000 radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     1616 2021-12-03 12:54:20.000000 radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-37-pytest-5.4.1.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     1620 2023-07-25 08:38:20.000000 radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-37-pytest-7.1.2.pyc
+-rw-rw-r--   0 ed        (1000) users      (100)     1642 2022-01-25 10:37:52.000000 radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 ed        (1000) users      (100)     2104 2023-07-26 07:54:01.000000 radioSphere-2.0.1/tests/test_DEM.py
+-rw-r--r--   0 ed        (1000) users      (100)     3743 2023-07-26 07:54:01.000000 radioSphere-2.0.1/tests/test_cleaner.py
+-rw-r--r--   0 ed        (1000) users      (100)    12664 2023-07-26 07:54:01.000000 radioSphere-2.0.1/tests/test_detection.py
+-rw-r--r--   0 ed        (1000) users      (100)    17446 2023-07-26 07:54:01.000000 radioSphere-2.0.1/tests/test_optimiser.py
+-rw-r--r--   0 ed        (1000) users      (100)    19746 2023-07-26 07:55:29.000000 radioSphere-2.0.1/tests/test_projector.py
+-rw-r--r--   0 ed        (1000) users      (100)     1993 2021-04-12 16:42:36.000000 radioSphere-2.0.1/tests/test_tomopack.py
```

### Comparing `radioSphere-2.0.0/LICENSE.md` & `radioSphere-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/PKG-INFO` & `radioSphere-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 Metadata-Version: 2.1
 Name: radioSphere
-Version: 2.0.0
+Version: 2.0.1
 Summary: Software for the Practical Analysis of Materials
 Author-email: Edward Andò <edward.ando@epfl.ch>, Benjy Marks <benjy.marks@sydney.edu.au>
 Maintainer-email: Edward Andò <edward.ando@epfl.ch>, Benjy Marks <benjy.marks@sydney.edu.au>
 License: GPLv3
 Project-URL: Blog, https://medium.com/@RadioSphere
 Project-URL: Repository, https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere
 Keywords: reconstruction,deconvolution,spheres,image analysis,synthetic images
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.md
 
-Welcome to radioSphere
-=======================
+# Welcome to radioSphere
+
+[![license](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/blob/main/LICENSE.md)
+[![pipeline status](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/badges/main/pipeline.svg)](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/pipelines)
+[![pypi](https://badge.fury.io/py/radioSphere.svg)](https://pypi.org/project/radioSphere/)
 
 [Join the chat room for support here.](https://matrix.to/#/#radioSphere:matrix.org)
 
 This project contains a series of tools for the analysis of divergent radiographs containing spherical particles, in particular to measure 3D positions from *a single radiograph* like this one:
 
-![Sample Radiograph](figures/nano/sample.jpg "Radiography of a small collection of same-size spheres")
-
-`radioSphere` is mostly a collection of python libraries (currently bound with a bit of C for the projector).
-
-The technique has been developed by Edward Andò (CNRS), [Benjy Marks](http://www.benjymarks.com/), and Stéphane Roux (CNRS), there is a paper under review in Measurement Science and Technology at the moment.
+![Sample Radiograph](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/raw/main/figures/nano/sample.jpg "Radiography of a small collection of same-size spheres")
 
-The technique proposed is a two-step approach:
+The reconstruction technique proposed is a two-step approach:
 
   - **Step 1**: is a technique called `tomopack` which is an FFT-based pattern matching approach.
   It uses a template image, or "structuring element" that we call ψ to pick out spheres.
   Since the size of ψ needs to be very close to the correct size, this allows us to distinguish different sized projections of spheres.
 
   - **Step 2**: Position optimisation: Starting from a guess of particle positions, the projection is computed and compared to the measured projection. Particle positions are modified iteratively in order to minimise the difference between computed projection and measured one.
 
 Geometry in `radioSphere` is everything: the coordinate systems defined are as follows:
 
 ![Geometry](figures/projectedCoords_v2.png "Coordinate Systems")
 
-Notes on the repository
-------------------------
+See the [online documentation](https://ttk.gricad-pages.univ-grenoble-alpes.fr/radioSphere/) to learn about the functions.
+
+## Contributors
+
+The technique has been developed by Edward Andò (EPFL), [Benjy Marks](http://www.benjymarks.com/), and Stéphane Roux (CNRS) and published in [Measurement Science and Technology](https://doi.org/10.1088/1361-6501/abfbfe).
+
+The technique has been developed thanks to UGA Tec21 funding further by Olga Stamati (ESRF), resulting in a publication in [The Journal of Multiphase Flow](https://doi.org/10.1016/j.ijmultiphaseflow.2023.104406), and by Leonard Turpin (Diamond).
+
+The numba projector was contributed by [Youssef Haouchat](https://github.com/HaouchatY) (EPFL),which is faster than the original C code and allows us to distribute the package on pypi, thanks!
+
+
+## Notes on the repository
 
  - `src/radioSphere`: this folder contains the core functions of radioSphere:
 
     - `detectSpheres`: functions related to `tomopack` (Step 1)
 
     - `optimisePositions`: functions related to the optimiser (Step 2)
 
@@ -68,46 +78,21 @@
 
  - `figures`: figures for paper and this website
 
  - `paper`: will contain final sources to the paper
 
  - `presentations`: sources for presentations given about this topic
 
+## Installing radioSphere
 
-Todo next in Sydney
----------------------
+### For users:
+`pip install radioSphere`
 
- - Separate analysis of Benjy's 25mm and 14mm experiments
- - Attempt to measure transformation matrix between two source-detector setups (is same SSD assumed)
- - Attempt a two-source-detector optimisation that should elimiate X-drection error
- - Evaluate attenuation difference between 25 and 14mm particles
- - Attempt a mix of 25 and 14mm, by eyeballing it, they should separate nicely (no overlap), for each angle separately
-    - Does the residual need to be computed with a different attenuation curve for each one?
- - Attemps a non-separatable mix using both source informations + non-overlapping together
-
-Todo next in the Alps
-----------------------
- - Do a physical ψ-scan with about 1/20 particle diameter steps
- - Don't forget the calibration sphere
- - No need to do a noise-scan, but a sample rotation (in a cylindrical holder) would be good
- - Attempt to measure L vs I/I0 directly on a tomopack reconstruction
-   -> Recognise 3D positions from tomopack-scan
-      - assemble ψ-scan
-      - run ψ-scan on the centred ψ-image to get fXseries and compute characteristic template for one particle
-      - chop this off on detector and in X-direction and save this as a convolution kernel
-      - run ψ-scan on real pack of spheres to get fXseries, and run kernel on it
-      - threshold centres, that's your 3D reconstruction!
-   -> compute P (in mm) and plot, for (every?) pixel on the detector P vs I/I0
-   -> Fit attenuation (hopefully a nice line) and look at fitting residuals on the detector
-   -> do optimisation in greylevels to avoid ln(I/I0)
-   -> party
-
-Installing radioSphere
------------------------
 
+### For developers:
 Please clone this repository once checked out, activate your virtual environment, and then:
-`pip install .`
+`pip install -e ".[dev]"`
 
 run the tests to make sure everything is OK:
-`pytest tests/`
-or
-`python setup.py test`
+`pytest`
+
+
```

### Comparing `radioSphere-2.0.0/docs/Makefile` & `radioSphere-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/make.bat` & `radioSphere-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/conf.py` & `radioSphere-2.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/index.rst` & `radioSphere-2.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/logo.png` & `radioSphere-2.0.1/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/modules.rst` & `radioSphere-2.0.1/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/notebooks/Running radioSphere on artificial data.ipynb` & `radioSphere-2.0.1/docs/source/notebooks/Running radioSphere on artificial data.ipynb`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/docs/source/notebooks/Running radioSphere on experimental data.ipynb` & `radioSphere-2.0.1/docs/source/notebooks/Running radioSphere on experimental data.ipynb`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/pyproject.toml` & `radioSphere-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "radioSphere"
 # If you bump this, remember to say what changed at the bottom of README.md
-version = "2.0.0"
+version = "2.0.1"
 description = "Software for the Practical Analysis of Materials"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv3"}
 keywords = [
     "reconstruction",
     "deconvolution",
@@ -25,41 +25,44 @@
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
     "numpy",
     "scipy",
     "scikit-image",
     "ipython",
     "tifffile",
     "matplotlib",
-    "progressbar2",
+    "tqdm",
     "notebook",
     "json5",
     "numba"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "sphinx",
     "sphinx-rtd-theme",
     "nbsphinx",
     "numpydoc",
     "black",
+    "build",
+    "twine",
     #"pip-tools",
     #"docutils>=0.16",
     #"Jinja2>=3.0.3", # fix jinja version to avoid https://github.com/readthedocs/readthedocs.org/issues/9038
     #"pre-commit",
     #"pip-tools",
 ]
 test = [
```

### Comparing `radioSphere-2.0.0/src/radioSphere/DEM/DEM.py` & `radioSphere-2.0.1/src/radioSphere/DEM/DEM.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/DEM/mercury.py` & `radioSphere-2.0.1/src/radioSphere/DEM/mercury.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             + str(pixelsPerDiameterZoomed)
             + "/thickness-"
             + str(numberOfParticleLayers)
             + "/"
         )
         if not os.path.exists(foldername):
             os.makedirs(foldername)
-        tifffile.imsave(foldername + str(tstep).zfill(4) + ".tiff", radioXmm)
+        tifffile.imwrite(foldername + str(tstep).zfill(4) + ".tiff", radioXmm)
 
     return radioMM, spheresMM, radiiMM, sourceObjectDistMM
 
 
 if __name__ == "__main__":
     fname = "./data/lees_edwards_nu_0.6_R_1_M_1.data"
     # Constant system parameters
```

### Comparing `radioSphere-2.0.0/src/radioSphere/DEM/nddem.py` & `radioSphere-2.0.1/src/radioSphere/DEM/nddem.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/blender_viewer.py` & `radioSphere-2.0.1/src/radioSphere/blender_viewer.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/calibrateAttenuation.py` & `radioSphere-2.0.1/src/radioSphere/calibrateAttenuation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import numpy
 import matplotlib.pyplot as plt
 import tifffile
 import radioSphere
 from scipy.optimize import curve_fit, minimize
-from progressbar import progressbar
+from tqdm import tqdm
 
 
 def cubicFit(x, l, n, m, c):
     return l * x**3 + n * x**2 + m * x + c
 
 
 def quadraticFit(x, n, m, c):
@@ -260,15 +260,15 @@
     focalSpotSize=0,
     verbose=True,
     GRAPH=False
 ):
     calibration_args = numpy.array(args[:-1])
     scattering = args[-1]
 
-    for i in progressbar(range(iterations)):
+    for i in tqdm(range(iterations)):
 
         # Update our calibration curve
         bounds = [[0,numpy.inf]]*len(args)
         res = minimize(
             testCalibration,
             args,
             args=(
@@ -498,8 +498,8 @@
         verbose=True,
     )
 
     print("Linear attenuation law:")
     print(f"    Location: {location_guess}")
     print(f"    Calibration: {calibration_args}")
     print(f"    Scattering: {scattering}")
-    
+
```

### Comparing `radioSphere-2.0.0/src/radioSphere/detectSpheres.py` & `radioSphere-2.0.1/src/radioSphere/detectSpheres.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import scipy.stats
 from scipy.spatial import distance
 
 import matplotlib.pyplot as plt
 import tifffile
 
 import multiprocessing
-import progressbar
+from tqdm import tqdm
 
 # Global number of processes
 nProcessesDefault = multiprocessing.cpu_count()
 
 
 # helper projector function operating on fx (approximation of "indicator" function)
 def _PIprojector(f):
@@ -516,15 +516,15 @@
         pixelSizeMM=pixelSizeMM,
         sourceDetectorDistMM=sourceDetectorDistMM,
         blur=blur,
         projector=projector,
         scattering=scattering
     )
 
-    pbar = progressbar.ProgressBar(max_value=len(CORxPositions)).start()
+    pbar = tqdm(total=len(CORxPositions))
     finishedPos = 0
 
     # Loop over CORx
     # global computeOneCOR
 
     def computeOneCOR(pos):
         CORxPos = CORxPositions[pos]
@@ -554,15 +554,15 @@
             radioMM, psiMM, maxIterations=maxIterations, l=l, kTrustMethod=kTrustMethod, kTrustRatio=kTrustRatio, epsilon=epsilon, kTrust=kTrust
         )
         psiX = radioSphere.detectSpheres.tomopack(
             psiRefMM, psiMM, maxIterations=maxIterations, l=l, kTrustMethod=kTrustMethod, kTrustRatio=kTrustRatio, epsilon=epsilon, kTrust=kTrust
         )
 
         return pos, fX, psiX
-    
+
     for i in range(len(CORxPositions)):
         tt, fX, psiX = computeOneCOR(i)
         fXseries[i] = fX
         psiXseries[i] = psiX
         pbar.update(i)
 
     # Run multiprocessing
@@ -572,14 +572,15 @@
     #         psiXseries[returns[0]] = returns[2]
     #         finishedPos += 1
     #         pbar.update(finishedPos)
 
     #     pool.close()
     #     pool.join()x
     # pbar.finish()
+    pbar.close()
 
     return fXseries, psiXseries
 
 
 def tomopackDivergentScanTo3DPositions(
     radioMM,
     radiusMM,
@@ -772,16 +773,16 @@
             epsilon=epsilon,
             kTrustRatio=kTrustRatio,
             SNRCutoff=SNRCutoff,
             nProcesses=nProcesses,
         )
 
         if saveSeries:
-            tifffile.imsave(saveSeriesDirectory + "/fXseries.tif", fXseries.astype("<f4"))
-            tifffile.imsave(saveSeriesDirectory + "/psiXseries.tif", psiXseries.astype("<f4"))
+            tifffile.imwrite(saveSeriesDirectory + "/fXseries.tif", fXseries.astype("<f4"))
+            tifffile.imwrite(saveSeriesDirectory + "/psiXseries.tif", psiXseries.astype("<f4"))
 
     #############################################################################
     # Clean resonance peaks of fx series
     # by a convolution with a SE extracted from the psi series
     #############################################################################
     # if verbose: print("\nConvolving fx with psi series...", end="")
     ##Lx  = 20 # TODO: SCALING IN X DIRECTION SHOULD BE A FUNCTION OF THE CONE ANGLE
@@ -803,16 +804,16 @@
     ## OS 2021-11-19: Let's do a fourier convolution which should be way faster
     ##fXconvolvedSeries = scipy.ndimage.convolve(fXseries,struct/struct.sum())
     fXconvolvedSeries = scipy.signal.convolve(fXseries, struct / struct.sum(), mode="same")
     if verbose:
         print(" done.")
 
     if saveSeries:
-        tifffile.imsave(saveSeriesDirectory + "/psiXseries-convolutionSE.tif", struct.astype("<f4"))
-        tifffile.imsave(
+        tifffile.imwrite(saveSeriesDirectory + "/psiXseries-convolutionSE.tif", struct.astype("<f4"))
+        tifffile.imwrite(
             saveSeriesDirectory + "/fXconvolvedSeries.tif", fXconvolvedSeries.astype("<f4")
         )
 
     # fXconvolvedSeries = fXseries.copy()
     ##############################################################################
     # Filter maxima of cleaned fx series
     ##############################################################################
@@ -831,17 +832,17 @@
 
     allPeaks = fXconvolvedSeries == fXconvolvedMaximumFiltered
     masses = allPeaks * fXconvolvedSeries
     if verbose:
         print(" done.")
 
     if saveSeries:
-        tifffile.imsave(saveSeriesDirectory + "/masses.tif", masses.astype("<f4"))
-        tifffile.imsave(saveSeriesDirectory + "/peaks.tif", allPeaks.astype("<f4"))
-        tifffile.imsave(
+        tifffile.imwrite(saveSeriesDirectory + "/masses.tif", masses.astype("<f4"))
+        tifffile.imwrite(saveSeriesDirectory + "/peaks.tif", allPeaks.astype("<f4"))
+        tifffile.imwrite(
             saveSeriesDirectory + "/fXconvolvedSeriesMaxFiltered.tif",
             fXconvolvedMaximumFiltered.astype("<f4"),
         )
 
     ##############################################################################
     # Find filtered peaks on the detector
     ##############################################################################
@@ -1295,15 +1296,15 @@
             radio,
             psiXseries[posN],
             GRAPH=0,
             maxIterations=maxIterations,
             l=l,
             kTrustRatio=kTrustRatio,
         )
-    tifffile.imsave(cacheFile, fXseries.astype("float"))
+    tifffile.imwrite(cacheFile, fXseries.astype("float"))
     print(f"saved {cacheFile}")
     # loadedCache = False
 
     # if useCache:
     # cachePsiFile = cacheFile[:-4] + '_psi.tif'
     # if os.path.isfile(cacheFile) and os.path.isfile(cachePsiFile):
     # print("Loading previous indicator functions... ", end="")
@@ -1338,29 +1339,29 @@
     # blur=blur)
 
     # fXseries[posN] = radioSphere.detectSpheres.tomopack(radioMM, psiMM, GRAPH=0, maxIterations=maxIterations, l=l, kTrustRatio=kTrustRatio)
     # psiXseries[posN] = radioSphere.detectSpheres.tomopack(psiRefMM, psiMM, GRAPH=0, maxIterations=maxIterations, l=l, kTrustRatio=kTrustRatio)
 
     # if useCache and not loadedCache:
     # print("Saving indicator functions for next time... ", end="")
-    # tifffile.imsave(cacheFile, fXseries.astype('<f4'))
-    # tifffile.imsave(cachePsiFile, psiXseries.astype('<f4'))
+    # tifffile.imwrite(cacheFile, fXseries.astype('<f4'))
+    # tifffile.imwrite(cachePsiFile, psiXseries.astype('<f4'))
     # print("done.")
 
     # L_x  = 20 # TODO: SCALING IN X DIRECTION SHOULD BE A FUNCTION OF THE CONE ANGLE
     # L_yz =  2 # TODO: THIS SHOULD BE A FUNCTION OF THE PIXELS PER RADIUS
 
     # struct = psiXseries[(psiXseries.shape[0])//2 -  L_x:(psiXseries.shape[0])//2 + L_x  + 1,
     # (psiXseries.shape[1])//2 - L_yz:(psiXseries.shape[1])//2 + L_yz + 1,
     # (psiXseries.shape[2])//2 - L_yz:(psiXseries.shape[2])//2 + L_yz + 1]
 
     # fXconvolvedSeries = scipy.ndimage.convolve(fXseries,struct/struct.sum())
     ##if useCache and not loadedCache:
-    ##tifffile.imsave(f'{cacheFile[:-4]}_struct.tif', struct.astype('<f4'))
-    ##tifffile.imsave(f'{cacheFile[:-4]}_fXconvolvedSeries.tif', fXconvolvedSeries.astype('<f4'))
+    ##tifffile.imwrite(f'{cacheFile[:-4]}_struct.tif', struct.astype('<f4'))
+    ##tifffile.imwrite(f'{cacheFile[:-4]}_fXconvolvedSeries.tif', fXconvolvedSeries.astype('<f4'))
 
     # binaryPeaks = fXconvolvedSeries > massThreshold
 
     zoomLevel = sourceDetectorDistMM / ((CORxPositions[0] + CORxPositions[-1]) / 2)
     CORxDelta = numpy.abs(CORxPositions[0] - CORxPositions[1])
     # Look in a volume of +/- half a radius in all directions for the highest value (+/- 1 radius keeps overlapping and causing issues, half a radius doesn't overlap particles, but still contains one clean peak)
     fXseriesMaximumFiltered = scipy.ndimage.maximum_filter(
@@ -1371,18 +1372,18 @@
             int(numpy.floor(radiusMM / pixelSizeMM * zoomLevel)),
         ),
     )
     allPeaks = fXseries == fXseriesMaximumFiltered
     masses = allPeaks * fXseries
 
     if verbose:
-        tifffile.imsave(cacheFile[:-4] + "_masses.tif", masses.astype("<f4"))
-        tifffile.imsave(cacheFile[:-4] + "_peaks.tif", allPeaks.astype("<f4"))
-        tifffile.imsave(cacheFile[:-4] + "_fXseries.tif", fXseries.astype("<f4"))
-        tifffile.imsave(
+        tifffile.imwrite(cacheFile[:-4] + "_masses.tif", masses.astype("<f4"))
+        tifffile.imwrite(cacheFile[:-4] + "_peaks.tif", allPeaks.astype("<f4"))
+        tifffile.imwrite(cacheFile[:-4] + "_fXseries.tif", fXseries.astype("<f4"))
+        tifffile.imwrite(
             cacheFile[:-4] + "_fXseriesMaximumFiltered.tif", fXseriesMaximumFiltered.astype("<f4")
         )
 
     if scanFixedNumber:
         # get the indices of all of the peaks, from highest to lowest
         sortedPeakIndices = numpy.argsort(masses, axis=None)[::-1]
         # print(sortedPeakIndices.shape)
@@ -1392,15 +1393,15 @@
         ).T
         # print(peaksCORxPOSnJI.shape)
     else:
         filteredPeaks = masses > massThreshold
         peaksCORxPOSnJI = numpy.argwhere(filteredPeaks)
 
         if verbose:
-            tifffile.imsave(cacheFile[:-4] + "_filteredPeaks.tif", filteredPeaks.astype("<f4"))
+            tifffile.imwrite(cacheFile[:-4] + "_filteredPeaks.tif", filteredPeaks.astype("<f4"))
     # print(peaksCORxPOSnJI)
 
     ###############################################################
     ### Now we have guesses for all particle according to detector
     ###   (IJ) and position along the X-scanning direction
     ### We're going to convert that to spatial XYZ
     ###############################################################
```

### Comparing `radioSphere-2.0.0/src/radioSphere/optimisePositions.py` & `radioSphere-2.0.1/src/radioSphere/optimisePositions.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/projectSphere/CupyProjector.py` & `radioSphere-2.0.1/src/radioSphere/projectSphere/CupyProjector.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/projectSphere/NumbaProjector.py` & `radioSphere-2.0.1/src/radioSphere/projectSphere/NumbaProjector.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/projectSphere/projectSphere.py` & `radioSphere-2.0.1/src/radioSphere/projectSphere/projectSphere.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/projectSphere/projectorSpeedTest.py` & `radioSphere-2.0.1/src/radioSphere/projectSphere/projectorSpeedTest.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/radioSphere.mplstyle` & `radioSphere-2.0.1/src/radioSphere/radioSphere.mplstyle`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/scripts/calibrateManyParticles.py` & `radioSphere-2.0.1/src/radioSphere/scripts/calibrateManyParticles.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/scripts/calibrateSingleParticle.py` & `radioSphere-2.0.1/src/radioSphere/scripts/calibrateSingleParticle.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/scripts/findParticles.py` & `radioSphere-2.0.1/src/radioSphere/scripts/findParticles.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/scripts/generate_particles_with_shells.py` & `radioSphere-2.0.1/src/radioSphere/scripts/generate_particles_with_shells.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere/scripts/optimiseParticles.py` & `radioSphere-2.0.1/src/radioSphere/scripts/optimiseParticles.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/src/radioSphere.egg-info/PKG-INFO` & `radioSphere-2.0.1/src/radioSphere.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 Metadata-Version: 2.1
 Name: radioSphere
-Version: 2.0.0
+Version: 2.0.1
 Summary: Software for the Practical Analysis of Materials
 Author-email: Edward Andò <edward.ando@epfl.ch>, Benjy Marks <benjy.marks@sydney.edu.au>
 Maintainer-email: Edward Andò <edward.ando@epfl.ch>, Benjy Marks <benjy.marks@sydney.edu.au>
 License: GPLv3
 Project-URL: Blog, https://medium.com/@RadioSphere
 Project-URL: Repository, https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere
 Keywords: reconstruction,deconvolution,spheres,image analysis,synthetic images
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.md
 
-Welcome to radioSphere
-=======================
+# Welcome to radioSphere
+
+[![license](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/blob/main/LICENSE.md)
+[![pipeline status](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/badges/main/pipeline.svg)](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/pipelines)
+[![pypi](https://badge.fury.io/py/radioSphere.svg)](https://pypi.org/project/radioSphere/)
 
 [Join the chat room for support here.](https://matrix.to/#/#radioSphere:matrix.org)
 
 This project contains a series of tools for the analysis of divergent radiographs containing spherical particles, in particular to measure 3D positions from *a single radiograph* like this one:
 
-![Sample Radiograph](figures/nano/sample.jpg "Radiography of a small collection of same-size spheres")
-
-`radioSphere` is mostly a collection of python libraries (currently bound with a bit of C for the projector).
-
-The technique has been developed by Edward Andò (CNRS), [Benjy Marks](http://www.benjymarks.com/), and Stéphane Roux (CNRS), there is a paper under review in Measurement Science and Technology at the moment.
+![Sample Radiograph](https://gricad-gitlab.univ-grenoble-alpes.fr/ttk/radioSphere/-/raw/main/figures/nano/sample.jpg "Radiography of a small collection of same-size spheres")
 
-The technique proposed is a two-step approach:
+The reconstruction technique proposed is a two-step approach:
 
   - **Step 1**: is a technique called `tomopack` which is an FFT-based pattern matching approach.
   It uses a template image, or "structuring element" that we call ψ to pick out spheres.
   Since the size of ψ needs to be very close to the correct size, this allows us to distinguish different sized projections of spheres.
 
   - **Step 2**: Position optimisation: Starting from a guess of particle positions, the projection is computed and compared to the measured projection. Particle positions are modified iteratively in order to minimise the difference between computed projection and measured one.
 
 Geometry in `radioSphere` is everything: the coordinate systems defined are as follows:
 
 ![Geometry](figures/projectedCoords_v2.png "Coordinate Systems")
 
-Notes on the repository
-------------------------
+See the [online documentation](https://ttk.gricad-pages.univ-grenoble-alpes.fr/radioSphere/) to learn about the functions.
+
+## Contributors
+
+The technique has been developed by Edward Andò (EPFL), [Benjy Marks](http://www.benjymarks.com/), and Stéphane Roux (CNRS) and published in [Measurement Science and Technology](https://doi.org/10.1088/1361-6501/abfbfe).
+
+The technique has been developed thanks to UGA Tec21 funding further by Olga Stamati (ESRF), resulting in a publication in [The Journal of Multiphase Flow](https://doi.org/10.1016/j.ijmultiphaseflow.2023.104406), and by Leonard Turpin (Diamond).
+
+The numba projector was contributed by [Youssef Haouchat](https://github.com/HaouchatY) (EPFL),which is faster than the original C code and allows us to distribute the package on pypi, thanks!
+
+
+## Notes on the repository
 
  - `src/radioSphere`: this folder contains the core functions of radioSphere:
 
     - `detectSpheres`: functions related to `tomopack` (Step 1)
 
     - `optimisePositions`: functions related to the optimiser (Step 2)
 
@@ -68,46 +78,21 @@
 
  - `figures`: figures for paper and this website
 
  - `paper`: will contain final sources to the paper
 
  - `presentations`: sources for presentations given about this topic
 
+## Installing radioSphere
 
-Todo next in Sydney
----------------------
+### For users:
+`pip install radioSphere`
 
- - Separate analysis of Benjy's 25mm and 14mm experiments
- - Attempt to measure transformation matrix between two source-detector setups (is same SSD assumed)
- - Attempt a two-source-detector optimisation that should elimiate X-drection error
- - Evaluate attenuation difference between 25 and 14mm particles
- - Attempt a mix of 25 and 14mm, by eyeballing it, they should separate nicely (no overlap), for each angle separately
-    - Does the residual need to be computed with a different attenuation curve for each one?
- - Attemps a non-separatable mix using both source informations + non-overlapping together
-
-Todo next in the Alps
-----------------------
- - Do a physical ψ-scan with about 1/20 particle diameter steps
- - Don't forget the calibration sphere
- - No need to do a noise-scan, but a sample rotation (in a cylindrical holder) would be good
- - Attempt to measure L vs I/I0 directly on a tomopack reconstruction
-   -> Recognise 3D positions from tomopack-scan
-      - assemble ψ-scan
-      - run ψ-scan on the centred ψ-image to get fXseries and compute characteristic template for one particle
-      - chop this off on detector and in X-direction and save this as a convolution kernel
-      - run ψ-scan on real pack of spheres to get fXseries, and run kernel on it
-      - threshold centres, that's your 3D reconstruction!
-   -> compute P (in mm) and plot, for (every?) pixel on the detector P vs I/I0
-   -> Fit attenuation (hopefully a nice line) and look at fitting residuals on the detector
-   -> do optimisation in greylevels to avoid ln(I/I0)
-   -> party
-
-Installing radioSphere
------------------------
 
+### For developers:
 Please clone this repository once checked out, activate your virtual environment, and then:
-`pip install .`
+`pip install -e ".[dev]"`
 
 run the tests to make sure everything is OK:
-`pytest tests/`
-or
-`python setup.py test`
+`pytest`
+
+
```

### Comparing `radioSphere-2.0.0/src/radioSphere.egg-info/SOURCES.txt` & `radioSphere-2.0.1/src/radioSphere.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -41,31 +41,38 @@
 tests/__init__.py
 tests/test_DEM.py
 tests/test_cleaner.py
 tests/test_detection.py
 tests/test_optimiser.py
 tests/test_projector.py
 tests/test_tomopack.py
+tests/__pycache__/__init__.cpython-310.pyc
 tests/__pycache__/__init__.cpython-37.pyc
 tests/__pycache__/__init__.cpython-39.pyc
+tests/__pycache__/test_DEM.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_DEM.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_DEM.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_DEM.cpython-37.pyc
 tests/__pycache__/test_DEM.cpython-39-pytest-6.2.5.pyc
+tests/__pycache__/test_cleaner.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_cleaner.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_cleaner.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_cleaner.cpython-39-pytest-6.2.5.pyc
+tests/__pycache__/test_detection.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_detection.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_detection.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_detection.cpython-39-pytest-6.2.5.pyc
+tests/__pycache__/test_optimiser.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_optimiser.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_optimiser.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_optimiser.cpython-37.pyc
 tests/__pycache__/test_optimiser.cpython-39-pytest-6.2.5.pyc
 tests/__pycache__/test_optimiser_sensitivityField.cpython-37-pytest-5.4.1.pyc
+tests/__pycache__/test_projector.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_projector.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_projector.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_projector.cpython-37.pyc
 tests/__pycache__/test_projector.cpython-39-pytest-6.2.5.pyc
+tests/__pycache__/test_tomopack.cpython-310-pytest-7.4.0.pyc
 tests/__pycache__/test_tomopack.cpython-37-pytest-5.4.1.pyc
 tests/__pycache__/test_tomopack.cpython-37-pytest-7.1.2.pyc
 tests/__pycache__/test_tomopack.cpython-39-pytest-6.2.5.pyc
```

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-37.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_DEM.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_DEM.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_cleaner.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_cleaner.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_detection.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_detection.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-37.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_optimiser.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_optimiser.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_optimiser_sensitivityField.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_optimiser_sensitivityField.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-37.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_projector.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_projector.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-37-pytest-5.4.1.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-37-pytest-5.4.1.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-37-pytest-7.1.2.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/__pycache__/test_tomopack.cpython-39-pytest-6.2.5.pyc` & `radioSphere-2.0.1/tests/__pycache__/test_tomopack.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_DEM.py` & `radioSphere-2.0.1/tests/test_DEM.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_cleaner.py` & `radioSphere-2.0.1/tests/test_cleaner.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_detection.py` & `radioSphere-2.0.1/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_optimiser.py` & `radioSphere-2.0.1/tests/test_optimiser.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_projector.py` & `radioSphere-2.0.1/tests/test_projector.py`

 * *Files identical despite different names*

### Comparing `radioSphere-2.0.0/tests/test_tomopack.py` & `radioSphere-2.0.1/tests/test_tomopack.py`

 * *Files identical despite different names*

