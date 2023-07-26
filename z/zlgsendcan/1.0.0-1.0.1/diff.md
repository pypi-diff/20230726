# Comparing `tmp/zlgsendcan-1.0.0.tar.gz` & `tmp/zlgsendcan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.0.0.tar", last modified: Wed Jul 26 05:45:24 2023, max compression
+gzip compressed data, was "zlgsendcan-1.0.1.tar", last modified: Wed Jul 26 05:57:29 2023, max compression
```

## Comparing `zlgsendcan-1.0.0.tar` & `zlgsendcan-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 05:45:24.581623 zlgsendcan-1.0.0/
--rw-rw-rw-   0        0        0      220 2023-07-26 05:45:24.580623 zlgsendcan-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 05:45:24.581623 zlgsendcan-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      326 2023-07-26 05:43:59.000000 zlgsendcan-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 05:45:24.578641 zlgsendcan-1.0.0/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 05:45:24.000000 zlgsendcan-1.0.0/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-26 05:45:24.000000 zlgsendcan-1.0.0/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 05:45:24.000000 zlgsendcan-1.0.0/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 05:45:24.000000 zlgsendcan-1.0.0/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 05:45:24.000000 zlgsendcan-1.0.0/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 05:57:29.761340 zlgsendcan-1.0.1/
+-rw-rw-rw-   0        0        0      220 2023-07-26 05:57:29.761340 zlgsendcan-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 05:57:29.761340 zlgsendcan-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      328 2023-07-26 05:57:17.000000 zlgsendcan-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 05:57:29.759349 zlgsendcan-1.0.1/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 05:57:29.000000 zlgsendcan-1.0.1/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-07-26 05:57:29.000000 zlgsendcan-1.0.1/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 05:57:29.000000 zlgsendcan-1.0.1/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 05:57:29.000000 zlgsendcan-1.0.1/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 05:57:29.000000 zlgsendcan-1.0.1/zlgsendcan.egg-info/top_level.txt
```

