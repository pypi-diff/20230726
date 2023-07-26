# Comparing `tmp/logPPP-1.0.3.tar.gz` & `tmp/logPPP-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.0.3.tar", last modified: Wed Jul 12 11:34:35 2023, max compression
+gzip compressed data, was "logPPP-1.0.4.tar", last modified: Wed Jul 26 08:52:44 2023, max compression
```

## Comparing `logPPP-1.0.3.tar` & `logPPP-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.065303 logPPP-1.0.3/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:34:35.064333 logPPP-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.058323 logPPP-1.0.3/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-12 11:34:35.000000 logPPP-1.0.3/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:34:35.065303 logPPP-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.051378 logPPP-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.063337 logPPP-1.0.3/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.3/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1422 2023-07-12 11:34:34.000000 logPPP-1.0.3/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.3/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.3/src/logPPP/logPPPLevel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:52:44.740977 logPPP-1.0.4/
+-rw-rw-rw-   0        0        0      126 2023-07-26 08:52:44.740977 logPPP-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 08:52:44.740977 logPPP-1.0.4/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-26 08:52:44.000000 logPPP-1.0.4/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-26 08:52:44.000000 logPPP-1.0.4/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:52:44.000000 logPPP-1.0.4/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:52:44.000000 logPPP-1.0.4/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:52:44.740977 logPPP-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:52:44.725383 logPPP-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:52:44.740977 logPPP-1.0.4/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.4/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1771 2023-07-26 08:32:57.000000 logPPP-1.0.4/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.4/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.4/src/logPPP/logPPPLevel.py
```

