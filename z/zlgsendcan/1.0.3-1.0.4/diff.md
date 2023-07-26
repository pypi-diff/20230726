# Comparing `tmp/zlgsendcan-1.0.3.tar.gz` & `tmp/zlgsendcan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.0.3.tar", last modified: Wed Jul 26 06:28:11 2023, max compression
+gzip compressed data, was "zlgsendcan-1.0.4.tar", last modified: Wed Jul 26 06:40:11 2023, max compression
```

## Comparing `zlgsendcan-1.0.3.tar` & `zlgsendcan-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 06:28:11.539978 zlgsendcan-1.0.3/
--rw-rw-rw-   0        0        0      220 2023-07-26 06:28:11.538971 zlgsendcan-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 06:28:11.540987 zlgsendcan-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      328 2023-07-26 06:28:05.000000 zlgsendcan-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:28:11.537971 zlgsendcan-1.0.3/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 06:28:11.000000 zlgsendcan-1.0.3/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-26 06:28:11.000000 zlgsendcan-1.0.3/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 06:28:11.000000 zlgsendcan-1.0.3/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 06:28:11.000000 zlgsendcan-1.0.3/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 06:28:11.000000 zlgsendcan-1.0.3/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 06:40:11.006154 zlgsendcan-1.0.4/
+-rw-rw-rw-   0        0        0      220 2023-07-26 06:40:11.006154 zlgsendcan-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 06:40:11.007087 zlgsendcan-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      363 2023-07-26 06:39:39.000000 zlgsendcan-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:40:10.995065 zlgsendcan-1.0.4/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.4/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.4/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.4/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.4/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.4/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.4/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.4/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:40:11.004154 zlgsendcan-1.0.4/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 06:40:10.000000 zlgsendcan-1.0.4/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 06:40:10.000000 zlgsendcan-1.0.4/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 06:40:10.000000 zlgsendcan-1.0.4/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 06:40:10.000000 zlgsendcan-1.0.4/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 06:40:10.000000 zlgsendcan-1.0.4/zlgsendcan.egg-info/top_level.txt
```

