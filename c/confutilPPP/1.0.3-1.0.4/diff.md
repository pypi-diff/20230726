# Comparing `tmp/confutilPPP-1.0.3.tar.gz` & `tmp/confutilPPP-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confutilPPP-1.0.3.tar", last modified: Tue Jul 25 14:06:59 2023, max compression
+gzip compressed data, was "confutilPPP-1.0.4.tar", last modified: Wed Jul 26 08:58:32 2023, max compression
```

## Comparing `confutilPPP-1.0.3.tar` & `confutilPPP-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/
--rw-rw-rw-   0        0        0      157 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-07-25 13:32:01.000000 confutilPPP-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/confutilPPP.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-12 10:58:48.000000 confutilPPP-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/src/confutilPPP/
--rw-rw-rw-   0        0        0      205 2023-07-25 14:05:05.000000 confutilPPP-1.0.3/src/confutilPPP/__init__.py
--rw-rw-rw-   0        0        0     2310 2023-07-25 13:26:52.000000 confutilPPP-1.0.3/src/confutilPPP/_confutil.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:58:32.515397 confutilPPP-1.0.4/
+-rw-rw-rw-   0        0        0      157 2023-07-26 08:58:32.515397 confutilPPP-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-07-25 13:32:01.000000 confutilPPP-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 08:58:32.515397 confutilPPP-1.0.4/confutilPPP.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-26 08:58:32.000000 confutilPPP-1.0.4/confutilPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-26 08:58:32.000000 confutilPPP-1.0.4/confutilPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:58:32.000000 confutilPPP-1.0.4/confutilPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 08:58:32.000000 confutilPPP-1.0.4/confutilPPP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 08:58:32.000000 confutilPPP-1.0.4/confutilPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:58:32.515397 confutilPPP-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-12 10:58:48.000000 confutilPPP-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:58:32.499776 confutilPPP-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:58:32.515397 confutilPPP-1.0.4/src/confutilPPP/
+-rw-rw-rw-   0        0        0      205 2023-07-26 08:57:58.000000 confutilPPP-1.0.4/src/confutilPPP/__init__.py
+-rw-rw-rw-   0        0        0     2310 2023-07-25 13:26:52.000000 confutilPPP-1.0.4/src/confutilPPP/_confutil.py
```

### Comparing `confutilPPP-1.0.3/src/confutilPPP/_confutil.py` & `confutilPPP-1.0.4/src/confutilPPP/_confutil.py`

 * *Files identical despite different names*

