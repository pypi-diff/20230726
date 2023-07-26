# Comparing `tmp/zlgsendcan-1.0.7.tar.gz` & `tmp/zlgsendcan-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.0.7.tar", last modified: Wed Jul 26 08:06:16 2023, max compression
+gzip compressed data, was "zlgsendcan-1.0.8.tar", last modified: Wed Jul 26 08:11:26 2023, max compression
```

## Comparing `zlgsendcan-1.0.7.tar` & `zlgsendcan-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:06:16.497820 zlgsendcan-1.0.7/
--rw-rw-rw-   0        0        0      220 2023-07-26 08:06:16.496948 zlgsendcan-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 08:06:16.497820 zlgsendcan-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-07-26 08:06:11.000000 zlgsendcan-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:06:16.488842 zlgsendcan-1.0.7/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.7/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.7/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.7/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.7/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.7/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.7/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.7/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:06:16.495833 zlgsendcan-1.0.7/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 08:06:16.000000 zlgsendcan-1.0.7/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 08:06:16.000000 zlgsendcan-1.0.7/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:06:16.000000 zlgsendcan-1.0.7/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 08:06:16.000000 zlgsendcan-1.0.7/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 08:06:16.000000 zlgsendcan-1.0.7/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:11:26.361010 zlgsendcan-1.0.8/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:11:26.360010 zlgsendcan-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:11:26.361010 zlgsendcan-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      470 2023-07-26 08:11:19.000000 zlgsendcan-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:11:26.351011 zlgsendcan-1.0.8/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.8/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.8/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.8/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.8/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.8/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.8/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.8/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:11:26.359010 zlgsendcan-1.0.8/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:11:26.000000 zlgsendcan-1.0.8/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 08:11:26.000000 zlgsendcan-1.0.8/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:11:26.000000 zlgsendcan-1.0.8/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 08:11:26.000000 zlgsendcan-1.0.8/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 08:11:26.000000 zlgsendcan-1.0.8/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.0.7/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.0.8/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.7/zlgsendcan/parseDBC.py` & `zlgsendcan-1.0.8/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.7/zlgsendcan/yaml_util.py` & `zlgsendcan-1.0.8/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.7/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.0.8/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.7/zlgsendcan/zlgserver.py` & `zlgsendcan-1.0.8/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

