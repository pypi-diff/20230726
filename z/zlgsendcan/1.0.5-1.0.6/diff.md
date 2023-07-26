# Comparing `tmp/zlgsendcan-1.0.5.tar.gz` & `tmp/zlgsendcan-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.0.5.tar", last modified: Wed Jul 26 07:02:43 2023, max compression
+gzip compressed data, was "zlgsendcan-1.0.6.tar", last modified: Wed Jul 26 08:00:42 2023, max compression
```

## Comparing `zlgsendcan-1.0.5.tar` & `zlgsendcan-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:02:43.975394 zlgsendcan-1.0.5/
--rw-rw-rw-   0        0        0      220 2023-07-26 07:02:43.974369 zlgsendcan-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 07:02:43.975394 zlgsendcan-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      395 2023-07-26 07:02:23.000000 zlgsendcan-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:02:43.966368 zlgsendcan-1.0.5/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.5/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.5/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.5/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.5/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.5/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.5/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.5/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:02:43.973368 zlgsendcan-1.0.5/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 07:02:43.000000 zlgsendcan-1.0.5/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 07:02:43.000000 zlgsendcan-1.0.5/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:02:43.000000 zlgsendcan-1.0.5/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 07:02:43.000000 zlgsendcan-1.0.5/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 07:02:43.000000 zlgsendcan-1.0.5/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:00:42.191364 zlgsendcan-1.0.6/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:00:42.190364 zlgsendcan-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:00:42.191364 zlgsendcan-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-07-26 08:00:38.000000 zlgsendcan-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:00:42.180366 zlgsendcan-1.0.6/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.6/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.6/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.6/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.6/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.6/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.6/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.6/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:00:42.189365 zlgsendcan-1.0.6/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:00:42.000000 zlgsendcan-1.0.6/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 08:00:42.000000 zlgsendcan-1.0.6/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:00:42.000000 zlgsendcan-1.0.6/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 08:00:42.000000 zlgsendcan-1.0.6/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 08:00:42.000000 zlgsendcan-1.0.6/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.0.5/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.0.6/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.5/zlgsendcan/parseDBC.py` & `zlgsendcan-1.0.6/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.5/zlgsendcan/yaml_util.py` & `zlgsendcan-1.0.6/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.5/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.0.6/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.5/zlgsendcan/zlgserver.py` & `zlgsendcan-1.0.6/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

