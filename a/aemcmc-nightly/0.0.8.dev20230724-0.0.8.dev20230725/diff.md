# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230724.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230725.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230724.tar", last modified: Mon Jul 24 01:03:52 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230725.tar", last modified: Tue Jul 25 01:07:19 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230724.tar` & `aemcmc-nightly-0.0.8.dev20230725.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:03:52.246416 aemcmc-nightly-0.0.8.dev20230724/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 01:03:52.250416 aemcmc-nightly-0.0.8.dev20230724/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:03:52.250416 aemcmc-nightly-0.0.8.dev20230724/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-24 01:03:52.250416 aemcmc-nightly-0.0.8.dev20230724/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:03:52.246416 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 01:03:52.000000 aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 01:03:52.250416 aemcmc-nightly-0.0.8.dev20230724/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:03:52.246416 aemcmc-nightly-0.0.8.dev20230724/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-07-24 01:03:40.000000 aemcmc-nightly-0.0.8.dev20230724/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:07:19.962700 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 01:07:19.000000 aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:07:19.966700 aemcmc-nightly-0.0.8.dev20230725/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-07-25 01:07:07.000000 aemcmc-nightly-0.0.8.dev20230725/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230724/LICENSE` & `aemcmc-nightly-0.0.8.dev20230725/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230725/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230724
+Version: 0.0.8.dev20230725
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230724/README.md` & `aemcmc-nightly-0.0.8.dev20230725/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230724
+Version: 0.0.8.dev20230725
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230724/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230725/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230725/setup.cfg`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/setup.py` & `aemcmc-nightly-0.0.8.dev20230725/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230725/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230724/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230725/versioneer.py`

 * *Files identical despite different names*

