# Comparing `tmp/logPPP-1.0.5.tar.gz` & `tmp/logPPP-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.0.5.tar", last modified: Wed Jul 26 09:35:43 2023, max compression
+gzip compressed data, was "logPPP-1.0.6.tar", last modified: Wed Jul 26 09:50:00 2023, max compression
```

## Comparing `logPPP-1.0.5.tar` & `logPPP-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:35:43.582687 logPPP-1.0.5/
--rw-rw-rw-   0        0        0      126 2023-07-26 09:35:43.582687 logPPP-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 09:35:43.567097 logPPP-1.0.5/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-26 09:35:43.000000 logPPP-1.0.5/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-26 09:35:43.000000 logPPP-1.0.5/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:35:43.000000 logPPP-1.0.5/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 09:35:43.000000 logPPP-1.0.5/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 09:35:43.582687 logPPP-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:35:43.567097 logPPP-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:35:43.582687 logPPP-1.0.5/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.5/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1718 2023-07-26 09:35:22.000000 logPPP-1.0.5/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.5/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.5/src/logPPP/logPPPLevel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:50:00.857734 logPPP-1.0.6/
+-rw-rw-rw-   0        0        0      126 2023-07-26 09:50:00.857734 logPPP-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 09:50:00.857734 logPPP-1.0.6/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-26 09:50:00.000000 logPPP-1.0.6/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-26 09:50:00.000000 logPPP-1.0.6/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:50:00.000000 logPPP-1.0.6/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 09:50:00.000000 logPPP-1.0.6/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:50:00.857734 logPPP-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:50:00.842112 logPPP-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 09:50:00.857734 logPPP-1.0.6/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.6/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1667 2023-07-26 09:48:59.000000 logPPP-1.0.6/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.6/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.6/src/logPPP/logPPPLevel.py
```

