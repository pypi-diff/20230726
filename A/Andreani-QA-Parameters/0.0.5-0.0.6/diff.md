# Comparing `tmp/Andreani_QA_Parameters-0.0.5.tar.gz` & `tmp/Andreani_QA_Parameters-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Parameters-0.0.5.tar", last modified: Mon Jul 17 18:57:14 2023, max compression
+gzip compressed data, was "Andreani_QA_Parameters-0.0.6.tar", last modified: Wed Jul 26 17:44:29 2023, max compression
```

## Comparing `Andreani_QA_Parameters-0.0.5.tar` & `Andreani_QA_Parameters-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:57:14.811938 Andreani_QA_Parameters-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:57:14.803355 Andreani_QA_Parameters-0.0.5/Andreani_QA_Parameters.egg-info/
--rw-rw-rw-   0        0        0      317 2023-07-17 18:57:14.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_Parameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-07-17 18:57:14.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_Parameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:57:14.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_Parameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-17 18:57:14.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_Parameters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 18:57:14.808665 Andreani_QA_Parameters-0.0.5/Andreani_QA_parameters/
--rw-rw-rw-   0        0        0     3108 2023-06-09 20:32:20.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_parameters/Parameters.py
--rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.5/Andreani_QA_parameters/__init__.py
--rw-rw-rw-   0        0        0      317 2023-07-17 18:57:14.810932 Andreani_QA_Parameters-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 18:57:14.812983 Andreani_QA_Parameters-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-07-17 18:57:04.000000 Andreani_QA_Parameters-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.719469 Andreani_QA_Parameters-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.710523 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-26 17:44:29.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_Parameters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 17:44:29.716053 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/
+-rw-rw-rw-   0        0        0     3107 2023-07-26 17:42:01.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/Parameters.py
+-rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/__init__.py
+-rw-rw-rw-   0        0        0      278 2023-07-26 17:44:29.718457 Andreani_QA_Parameters-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:44:29.719469 Andreani_QA_Parameters-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-07-26 17:42:28.000000 Andreani_QA_Parameters-0.0.6/setup.py
```

### Comparing `Andreani_QA_Parameters-0.0.5/Andreani_QA_parameters/Parameters.py` & `Andreani_QA_Parameters-0.0.6/Andreani_QA_parameters/Parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import platform
 
 
 class Parameters:
     # CONFIGURACION PATH Y TESTCASE
-    current_path = os.path.abspath(os.path.join(__file__, "../../../../../"))
+    current_path = os.path.abspath(os.path.join(os.getcwd(), "../../../.."))
     file_name_stored = None
     env = None
 
     # CONFIGURACION PARA UTILIZAR CSV DESDE SHAREPOINT
     #sharepoint_data_jmeter=None
 
     # CONFIGURACION FORMATO DE FECHA
```

### Comparing `Andreani_QA_Parameters-0.0.5/setup.py` & `Andreani_QA_Parameters-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.5'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.6'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'Andreani_QA_Parameters'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Parametros + Encriptor para ejecución de casos automatizados'  # Descripción corta
```

