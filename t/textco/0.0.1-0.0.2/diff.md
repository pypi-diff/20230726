# Comparing `tmp/textco-0.0.1.tar.gz` & `tmp/textco-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textco-0.0.1.tar", last modified: Wed Jul 26 17:08:55 2023, max compression
+gzip compressed data, was "textco-0.0.2.tar", last modified: Wed Jul 26 17:15:48 2023, max compression
```

## Comparing `textco-0.0.1.tar` & `textco-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:08:55.800557 textco-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      731 2023-07-26 17:08:55.800557 textco-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 17:08:55.800557 textco-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-07-26 17:08:36.000000 textco-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:08:55.784935 textco-0.0.1/textco/
--rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.1/textco/__init__.py
--rw-rw-rw-   0        0        0      741 2023-07-26 16:56:47.000000 textco-0.0.1/textco/textco.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:08:55.800557 textco-0.0.1/textco.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-26 17:08:55.000000 textco-0.0.1/textco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-26 17:08:55.000000 textco-0.0.1/textco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:08:55.000000 textco-0.0.1/textco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 17:08:55.000000 textco-0.0.1/textco.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 17:15:48.380724 textco-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 textco-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      731 2023-07-26 17:15:48.380724 textco-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 textco-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:15:48.380724 textco-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-07-26 17:15:37.000000 textco-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:15:48.365099 textco-0.0.2/textco/
+-rw-rw-rw-   0        0        0       23 2023-07-26 16:54:05.000000 textco-0.0.2/textco/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-07-26 17:14:01.000000 textco-0.0.2/textco/textco.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:15:48.365099 textco-0.0.2/textco.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-07-26 17:15:48.000000 textco-0.0.2/textco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-26 17:15:48.000000 textco-0.0.2/textco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:15:48.000000 textco-0.0.2/textco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 17:15:48.000000 textco-0.0.2/textco.egg-info/top_level.txt
```

### Comparing `textco-0.0.1/LICENSE.txt` & `textco-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textco-0.0.1/PKG-INFO` & `textco-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `textco-0.0.1/setup.py` & `textco-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '00.00.01' 
+VERSION = '00.00.02' 
 DESCRIPTION = 'TEXT analytsis COpilot'
 LONG_DESCRIPTION = 'This Python package will help you to analyse text'
 
 
 setup(
         name="textco", 
         version=VERSION,
```

### Comparing `textco-0.0.1/textco/textco.py` & `textco-0.0.2/textco/textco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 #***********************************************************************************************************
 #*************************** WELCOME MESSAGE ****************************************************************
 #***********************************************************************************************************
 
-def textco()
+def textco():
 print("**********************************************************")
 print("Welcome to use TextCo: an innovative text analysis tool")
 print("**********************************************************")
 print("Contacts:")
 print("Dr Anna Sung - a.sung@chester.ac.uk")
 print("Prof Kelvin Leong - k.leong@@chester.ac.uk")
 print("**********************************************************")
```

### Comparing `textco-0.0.1/textco.egg-info/PKG-INFO` & `textco-0.0.2/textco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textco
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEXT analytsis COpilot
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

