# Comparing `tmp/probaforms-0.1.0.tar.gz` & `tmp/probaforms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probaforms-0.1.0.tar", max compression
+gzip compressed data, was "probaforms-0.2.0.tar", max compression
```

## Comparing `probaforms-0.1.0.tar` & `probaforms-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1107 2023-03-27 05:40:55.010197 probaforms-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-03-27 05:40:55.012355 probaforms-0.1.0/probaforms/__init__.py
--rw-r--r--   0        0        0      606 2023-04-01 10:00:38.563896 probaforms-0.1.0/probaforms/metrics/__init__.py
--rw-r--r--   0        0        0     5056 2023-04-01 09:40:45.937003 probaforms-0.1.0/probaforms/metrics/div1d.py
--rw-r--r--   0        0        0     1902 2023-03-31 07:24:39.463070 probaforms-0.1.0/probaforms/metrics/fd.py
--rw-r--r--   0        0        0     4721 2023-04-01 10:05:14.525896 probaforms-0.1.0/probaforms/metrics/ks1d.py
--rw-r--r--   0        0        0     1708 2023-04-01 09:44:04.857412 probaforms-0.1.0/probaforms/metrics/mmd.py
--rw-r--r--   0        0        0       59 2023-03-27 05:40:55.012561 probaforms-0.1.0/probaforms/models/__init__.py
--rw-r--r--   0        0        0      923 2023-03-27 05:40:55.012698 probaforms-0.1.0/probaforms/models/interfaces.py
--rw-r--r--   0        0        0     3458 2023-03-27 05:40:55.012799 probaforms-0.1.0/probaforms/models/nflow.py
--rw-r--r--   0        0        0     7863 2023-03-27 05:40:55.012946 probaforms-0.1.0/probaforms/models/realnvp.py
--rw-r--r--   0        0        0      649 2023-06-13 06:48:56.162789 probaforms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 probaforms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-07-26 18:12:00.604336 probaforms-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2510 2023-07-26 18:12:00.604453 probaforms-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 18:12:00.609541 probaforms-0.2.0/probaforms/__init__.py
+-rw-r--r--   0        0        0      606 2023-07-26 18:12:00.609820 probaforms-0.2.0/probaforms/metrics/__init__.py
+-rw-r--r--   0        0        0     5056 2023-07-26 18:12:00.609967 probaforms-0.2.0/probaforms/metrics/div1d.py
+-rw-r--r--   0        0        0     1902 2023-07-26 18:12:00.610178 probaforms-0.2.0/probaforms/metrics/fd.py
+-rw-r--r--   0        0        0     4721 2023-07-26 18:12:00.610452 probaforms-0.2.0/probaforms/metrics/ks1d.py
+-rw-r--r--   0        0        0     1708 2023-07-26 18:12:00.610656 probaforms-0.2.0/probaforms/metrics/mmd.py
+-rw-r--r--   0        0        0      151 2023-07-26 18:12:00.610877 probaforms-0.2.0/probaforms/models/__init__.py
+-rw-r--r--   0        0        0     8486 2023-07-26 18:12:00.611281 probaforms-0.2.0/probaforms/models/cvae.py
+-rw-r--r--   0        0        0      923 2023-07-26 18:12:00.611506 probaforms-0.2.0/probaforms/models/interfaces.py
+-rw-r--r--   0        0        0     3458 2023-07-26 18:12:00.611624 probaforms-0.2.0/probaforms/models/nflow.py
+-rw-r--r--   0        0        0     7863 2023-07-26 18:12:00.611848 probaforms-0.2.0/probaforms/models/realnvp.py
+-rw-r--r--   0        0        0    10383 2023-07-26 18:12:00.612327 probaforms-0.2.0/probaforms/models/wgan.py
+-rw-r--r--   0        0        0      850 2023-07-26 18:12:00.612473 probaforms-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 probaforms-0.2.0/PKG-INFO
```

### Comparing `probaforms-0.1.0/LICENSE` & `probaforms-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/metrics/__init__.py` & `probaforms-0.2.0/probaforms/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/metrics/div1d.py` & `probaforms-0.2.0/probaforms/metrics/div1d.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/metrics/fd.py` & `probaforms-0.2.0/probaforms/metrics/fd.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/metrics/ks1d.py` & `probaforms-0.2.0/probaforms/metrics/ks1d.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/metrics/mmd.py` & `probaforms-0.2.0/probaforms/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/models/interfaces.py` & `probaforms-0.2.0/probaforms/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/models/nflow.py` & `probaforms-0.2.0/probaforms/models/nflow.py`

 * *Files identical despite different names*

### Comparing `probaforms-0.1.0/probaforms/models/realnvp.py` & `probaforms-0.2.0/probaforms/models/realnvp.py`

 * *Files identical despite different names*

