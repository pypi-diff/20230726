# Comparing `tmp/econia_sdk-0.1.0.tar.gz` & `tmp/econia_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econia_sdk-0.1.0.tar", max compression
+gzip compressed data, was "econia_sdk-1.0.0.tar", max compression
```

## Comparing `econia_sdk-0.1.0.tar` & `econia_sdk-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       61 2023-07-26 16:34:28.596521 econia_sdk-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854900 econia_sdk-0.1.0/econia_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-0.1.0/econia_sdk/entry/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-0.1.0/econia_sdk/entry/incentives.py
--rw-r--r--   0        0        0     9304 2023-07-26 14:37:08.196179 econia_sdk-0.1.0/econia_sdk/entry/market.py
--rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-0.1.0/econia_sdk/entry/registry.py
--rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-0.1.0/econia_sdk/entry/user.py
--rw-r--r--   0        0        0     3534 2023-07-26 14:37:08.196402 econia_sdk-0.1.0/econia_sdk/lib.py
--rw-r--r--   0        0        0      551 2023-07-26 14:37:08.196745 econia_sdk-0.1.0/econia_sdk/types.py
--rw-r--r--   0        0        0        0 2023-07-26 14:37:08.196805 econia_sdk-0.1.0/econia_sdk/view/__init__.py
--rw-r--r--   0        0        0     2639 2023-07-26 14:37:08.196949 econia_sdk-0.1.0/econia_sdk/view/incentives.py
--rw-r--r--   0        0        0     6789 2023-07-26 14:37:08.197100 econia_sdk-0.1.0/econia_sdk/view/market.py
--rw-r--r--   0        0        0     6936 2023-07-26 14:37:08.197229 econia_sdk-0.1.0/econia_sdk/view/registry.py
--rw-r--r--   0        0        0      263 2023-07-26 14:37:08.197565 econia_sdk-0.1.0/econia_sdk/view/resource_account.py
--rw-r--r--   0        0        0    17155 2023-07-26 14:37:08.197807 econia_sdk-0.1.0/econia_sdk/view/user.py
--rw-r--r--   0        0        0      371 2023-07-26 14:37:08.198276 econia_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 econia_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-26 16:34:28.596521 econia_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854900 econia_sdk-1.0.0/econia_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-1.0.0/econia_sdk/entry/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-1.0.0/econia_sdk/entry/incentives.py
+-rw-r--r--   0        0        0     9304 2023-07-26 14:37:08.196179 econia_sdk-1.0.0/econia_sdk/entry/market.py
+-rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-1.0.0/econia_sdk/entry/registry.py
+-rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-1.0.0/econia_sdk/entry/user.py
+-rw-r--r--   0        0        0     3534 2023-07-26 14:37:08.196402 econia_sdk-1.0.0/econia_sdk/lib.py
+-rw-r--r--   0        0        0      551 2023-07-26 14:37:08.196745 econia_sdk-1.0.0/econia_sdk/types.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:37:08.196805 econia_sdk-1.0.0/econia_sdk/view/__init__.py
+-rw-r--r--   0        0        0     2639 2023-07-26 14:37:08.196949 econia_sdk-1.0.0/econia_sdk/view/incentives.py
+-rw-r--r--   0        0        0     6789 2023-07-26 14:37:08.197100 econia_sdk-1.0.0/econia_sdk/view/market.py
+-rw-r--r--   0        0        0     6936 2023-07-26 14:37:08.197229 econia_sdk-1.0.0/econia_sdk/view/registry.py
+-rw-r--r--   0        0        0      263 2023-07-26 14:37:08.197565 econia_sdk-1.0.0/econia_sdk/view/resource_account.py
+-rw-r--r--   0        0        0    17155 2023-07-26 14:37:08.197807 econia_sdk-1.0.0/econia_sdk/view/user.py
+-rw-r--r--   0        0        0      378 2023-07-26 16:45:25.208179 econia_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 econia_sdk-1.0.0/PKG-INFO
```

### Comparing `econia_sdk-0.1.0/econia_sdk/entry/incentives.py` & `econia_sdk-1.0.0/econia_sdk/entry/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/entry/market.py` & `econia_sdk-1.0.0/econia_sdk/entry/market.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/entry/registry.py` & `econia_sdk-1.0.0/econia_sdk/entry/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/entry/user.py` & `econia_sdk-1.0.0/econia_sdk/entry/user.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/lib.py` & `econia_sdk-1.0.0/econia_sdk/lib.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/types.py` & `econia_sdk-1.0.0/econia_sdk/types.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/view/incentives.py` & `econia_sdk-1.0.0/econia_sdk/view/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/view/market.py` & `econia_sdk-1.0.0/econia_sdk/view/market.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/view/registry.py` & `econia_sdk-1.0.0/econia_sdk/view/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-0.1.0/econia_sdk/view/user.py` & `econia_sdk-1.0.0/econia_sdk/view/user.py`

 * *Files identical despite different names*

