# Comparing `tmp/mcptbr-0.1.1.tar.gz` & `tmp/mcptbr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.1.tar", last modified: Tue Jul 25 14:14:46 2023, max compression
+gzip compressed data, was "mcptbr-0.1.2.tar", last modified: Wed Jul 26 01:25:58 2023, max compression
```

## Comparing `mcptbr-0.1.1.tar` & `mcptbr-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:14:46.223852 mcptbr-0.1.1/
--rw-rw-rw-   0        0        0      176 2023-07-25 14:14:46.208229 mcptbr-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 14:14:46.192638 mcptbr-0.1.1/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.1/mcptbr/__init__.py
--rw-rw-rw-   0        0        0      167 2023-07-25 14:13:47.000000 mcptbr-0.1.1/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:14:46.208229 mcptbr-0.1.1/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-25 14:14:46.000000 mcptbr-0.1.1/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-25 14:14:46.000000 mcptbr-0.1.1/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:14:46.000000 mcptbr-0.1.1/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 14:14:46.000000 mcptbr-0.1.1/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 14:14:46.000000 mcptbr-0.1.1/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:14:46.223852 mcptbr-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-07-25 14:14:11.000000 mcptbr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.791399 mcptbr-0.1.2/
+-rw-rw-rw-   0        0        0      176 2023-07-26 01:25:58.789403 mcptbr-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.724577 mcptbr-0.1.2/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.2/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0      723 2023-07-26 01:24:25.000000 mcptbr-0.1.2/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:25:58.787407 mcptbr-0.1.2/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 01:25:58.000000 mcptbr-0.1.2/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:25:58.791399 mcptbr-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-07-26 01:25:18.000000 mcptbr-0.1.2/setup.py
```

