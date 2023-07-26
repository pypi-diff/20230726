# Comparing `tmp/textco-0.0.5.tar.gz` & `tmp/textco-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textco-0.0.5.tar", last modified: Wed Jul 26 17:37:39 2023, max compression
+gzip compressed data, was "textco-0.0.6.tar", last modified: Wed Jul 26 18:14:04 2023, max compression
```

## Comparing `textco-0.0.5.tar` & `textco-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:37:39.169274 textco-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      731 2023-07-26 17:37:39.169274 textco-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 17:37:39.169274 textco-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-07-26 17:36:33.000000 textco-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:37:39.131525 textco-0.0.5/textco/
--rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.5/textco/__init__.py
--rw-rw-rw-   0        0        0     3652 2023-07-26 17:37:07.000000 textco-0.0.5/textco/textco.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:37:39.162768 textco-0.0.5/textco.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-26 17:37:39.000000 textco-0.0.5/textco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-26 17:37:39.000000 textco-0.0.5/textco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:37:39.000000 textco-0.0.5/textco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-26 17:37:39.000000 textco-0.0.5/textco.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 17:37:39.000000 textco-0.0.5/textco.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 18:14:04.493556 textco-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      731 2023-07-26 18:14:04.493556 textco-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:14:04.493556 textco-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2023-07-26 18:13:56.000000 textco-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:14:04.478204 textco-0.0.6/textco/
+-rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.6/textco/__init__.py
+-rw-rw-rw-   0        0        0    14631 2023-07-26 18:09:31.000000 textco-0.0.6/textco/textco.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:14:04.493556 textco-0.0.6/textco.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-07-26 18:14:04.000000 textco-0.0.6/textco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-26 18:14:04.000000 textco-0.0.6/textco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:14:04.000000 textco-0.0.6/textco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-26 18:14:04.000000 textco-0.0.6/textco.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 18:14:04.000000 textco-0.0.6/textco.egg-info/top_level.txt
```

### Comparing `textco-0.0.5/LICENSE.txt` & `textco-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textco-0.0.5/PKG-INFO` & `textco-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.5
+Version: 0.0.6
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `textco-0.0.5/textco.egg-info/PKG-INFO` & `textco-0.0.6/textco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.5
+Version: 0.0.6
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

