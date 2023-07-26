# Comparing `tmp/ztool2-0.1.tar.gz` & `tmp/ztool2-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztool2-0.1.tar", last modified: Wed Jul 26 08:57:58 2023, max compression
+gzip compressed data, was "ztool2-0.2.tar", last modified: Wed Jul 26 09:53:57 2023, max compression
```

## Comparing `ztool2-0.1.tar` & `ztool2-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:57:58.099139 ztool2-0.1/
--rw-rw-rw-   0        0        0      140 2023-07-26 08:57:58.098139 ztool2-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 08:57:58.099139 ztool2-0.1/setup.cfg
--rw-rw-rw-   0        0        0      238 2023-07-26 08:57:34.000000 ztool2-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:57:58.095141 ztool2-0.1/ztool2.egg-info/
--rw-rw-rw-   0        0        0      140 2023-07-26 08:57:57.000000 ztool2-0.1/ztool2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-07-26 08:57:57.000000 ztool2-0.1/ztool2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:57:57.000000 ztool2-0.1/ztool2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:57:57.000000 ztool2-0.1/ztool2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:53:57.072586 ztool2-0.2/
+-rw-rw-rw-   0        0        0      140 2023-07-26 09:53:57.071586 ztool2-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:53:57.072586 ztool2-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-07-26 09:53:50.000000 ztool2-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:53:57.069587 ztool2-0.2/ztool2.egg-info/
+-rw-rw-rw-   0        0        0      140 2023-07-26 09:53:56.000000 ztool2-0.2/ztool2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2023-07-26 09:53:56.000000 ztool2-0.2/ztool2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:53:56.000000 ztool2-0.2/ztool2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:53:56.000000 ztool2-0.2/ztool2.egg-info/top_level.txt
```

