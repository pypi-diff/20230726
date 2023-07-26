# Comparing `tmp/multisig_ci-0.6.1.tar.gz` & `tmp/multisig_ci-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.1.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.2.tar", max compression
```

## Comparing `multisig_ci-0.6.1.tar` & `multisig_ci-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/__main__.py
--rw-r--r--   0        0        0     8308 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-26 08:02:36.638547 multisig_ci-0.6.1/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      509 2023-07-26 08:02:36.642547 multisig_ci-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 multisig_ci-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     8308 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.2/PKG-INFO
```

### Comparing `multisig_ci-0.6.1/LICENSE` & `multisig_ci-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/__main__.py` & `multisig_ci-0.6.2/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/ci_override.py` & `multisig_ci-0.6.2/multisig_ci/ci_override.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.2/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/run_brownie.py` & `multisig_ci-0.6.2/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/safes.py` & `multisig_ci-0.6.2/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/sign.py` & `multisig_ci-0.6.2/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/telegram.py` & `multisig_ci-0.6.2/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.2/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.1/PKG-INFO` & `multisig_ci-0.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.1
+Version: 0.6.2
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
-Requires-Python: >=3.8,<=3.10
+Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: brownie_safe (>=0.8.0)
 Requires-Dist: eth-brownie (==1.19.2)
```

