# Comparing `tmp/pxmcmc-0.1.5.tar.gz` & `tmp/pxmcmc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxmcmc-0.1.5.tar", max compression
+gzip compressed data, was "pxmcmc-1.0.0.tar", max compression
```

## Comparing `pxmcmc-0.1.5.tar` & `pxmcmc-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2021-07-22 08:20:25.513019 pxmcmc-0.1.5/LICENSE
--rw-r--r--   0        0        0      935 2022-06-06 09:33:25.280600 pxmcmc-0.1.5/README.md
--rw-r--r--   0        0        0       22 2022-06-06 09:33:25.282836 pxmcmc-0.1.5/pxmcmc/__init__.py
--rw-r--r--   0        0        0     5518 2023-03-30 05:07:33.968909 pxmcmc-0.1.5/pxmcmc/forward.py
--rw-r--r--   0        0        0    13473 2023-04-14 06:38:56.774037 pxmcmc-0.1.5/pxmcmc/mcmc.py
--rw-r--r--   0        0        0     8463 2022-06-13 08:58:38.009287 pxmcmc-0.1.5/pxmcmc/measurements.py
--rw-r--r--   0        0        0     6354 2023-03-30 05:07:33.971536 pxmcmc-0.1.5/pxmcmc/plotting.py
--rw-r--r--   0        0        0     5447 2023-04-14 06:53:29.509093 pxmcmc-0.1.5/pxmcmc/prior.py
--rw-r--r--   0        0        0     1757 2021-06-28 20:26:37.306610 pxmcmc-0.1.5/pxmcmc/saving.py
--rw-r--r--   0        0        0     4931 2023-03-30 05:07:33.973061 pxmcmc-0.1.5/pxmcmc/transforms.py
--rw-r--r--   0        0        0     2115 2021-06-28 20:26:37.313172 pxmcmc-0.1.5/pxmcmc/uncertainty.py
--rw-r--r--   0        0        0    10289 2023-03-30 05:07:33.973877 pxmcmc-0.1.5/pxmcmc/utils.py
--rw-r--r--   0        0        0     1060 2023-04-14 06:55:06.772156 pxmcmc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 pxmcmc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-20 23:11:44.322548 pxmcmc-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2312 2023-07-25 23:39:51.621264 pxmcmc-1.0.0/README.md
+-rw-r--r--   0        0        0       72 2023-07-25 23:39:51.671229 pxmcmc-1.0.0/pxmcmc/__init__.py
+-rw-r--r--   0        0        0     5518 2023-07-25 23:23:01.750935 pxmcmc-1.0.0/pxmcmc/forward.py
+-rw-r--r--   0        0        0    13473 2023-07-25 06:02:30.377303 pxmcmc-1.0.0/pxmcmc/mcmc.py
+-rw-r--r--   0        0        0     8463 2023-07-25 23:23:01.751246 pxmcmc-1.0.0/pxmcmc/measurements.py
+-rw-r--r--   0        0        0     6354 2023-07-25 23:23:01.751997 pxmcmc-1.0.0/pxmcmc/plotting.py
+-rw-r--r--   0        0        0     5447 2023-07-25 23:23:01.752808 pxmcmc-1.0.0/pxmcmc/prior.py
+-rw-r--r--   0        0        0     1757 2023-07-25 06:02:30.379974 pxmcmc-1.0.0/pxmcmc/saving.py
+-rw-r--r--   0        0        0     4931 2023-07-25 23:23:01.753432 pxmcmc-1.0.0/pxmcmc/transforms.py
+-rw-r--r--   0        0        0     2115 2023-07-25 23:23:01.753884 pxmcmc-1.0.0/pxmcmc/uncertainty.py
+-rw-r--r--   0        0        0    10289 2023-07-25 23:23:01.754380 pxmcmc-1.0.0/pxmcmc/utils.py
+-rw-r--r--   0        0        0     1060 2023-07-25 23:41:17.603538 pxmcmc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 pxmcmc-1.0.0/PKG-INFO
```

### Comparing `pxmcmc-0.1.5/LICENSE` & `pxmcmc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/forward.py` & `pxmcmc-1.0.0/pxmcmc/forward.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/mcmc.py` & `pxmcmc-1.0.0/pxmcmc/mcmc.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/measurements.py` & `pxmcmc-1.0.0/pxmcmc/measurements.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/plotting.py` & `pxmcmc-1.0.0/pxmcmc/plotting.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/prior.py` & `pxmcmc-1.0.0/pxmcmc/prior.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/saving.py` & `pxmcmc-1.0.0/pxmcmc/saving.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/transforms.py` & `pxmcmc-1.0.0/pxmcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/uncertainty.py` & `pxmcmc-1.0.0/pxmcmc/uncertainty.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pxmcmc/utils.py` & `pxmcmc-1.0.0/pxmcmc/utils.py`

 * *Files identical despite different names*

### Comparing `pxmcmc-0.1.5/pyproject.toml` & `pxmcmc-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PxMCMC"
-version = "0.1.5"
+version = "1.0.0"
 authors = ["Auggie Marignier <augustin.marignier.14@ucl.ac.uk>"]
 description = "Proximal Markov Chain Monte Carlo"
 homepage = "https://github.com/auggiemarignier/pxmcmc"
 repository = "https://github.com/auggiemarignier/pxmcmc"
 license = "GPL-3.0-or-later"
 documentation = "https://pxmcmc.readthedocs.io/en/latest/index.html"
 readme = "README.md"
```

