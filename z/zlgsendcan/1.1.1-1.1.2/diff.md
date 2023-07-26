# Comparing `tmp/zlgsendcan-1.1.1.tar.gz` & `tmp/zlgsendcan-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.1.tar", last modified: Wed Jul 26 09:04:30 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.2.tar", last modified: Wed Jul 26 09:09:22 2023, max compression
```

## Comparing `zlgsendcan-1.1.1.tar` & `zlgsendcan-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:04:30.157580 zlgsendcan-1.1.1/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:04:30.156581 zlgsendcan-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 09:04:30.157580 zlgsendcan-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-07-26 09:04:28.000000 zlgsendcan-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:04:30.147690 zlgsendcan-1.1.1/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.1/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.1/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.1/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.1/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.1/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.1.1/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.1/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:04:30.154629 zlgsendcan-1.1.1/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:04:30.000000 zlgsendcan-1.1.1/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 09:04:30.000000 zlgsendcan-1.1.1/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:04:30.000000 zlgsendcan-1.1.1/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 09:04:30.000000 zlgsendcan-1.1.1/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 09:04:30.000000 zlgsendcan-1.1.1/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.117669 zlgsendcan-1.1.2/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:09:22.116670 zlgsendcan-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:09:22.117669 zlgsendcan-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-26 09:09:16.000000 zlgsendcan-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.109890 zlgsendcan-1.1.2/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.2/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.2/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.2/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.2/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.2/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.1.2/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.2/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.115689 zlgsendcan-1.1.2/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.1/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.2/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.1/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.2/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.1/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.2/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.1/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.2/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.1/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.2/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

