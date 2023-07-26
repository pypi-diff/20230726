# Comparing `tmp/vinhvh_package-0.0.8.tar.gz` & `tmp/vinhvh_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinhvh_package-0.0.8.tar", last modified: Tue Jul 25 05:19:12 2023, max compression
+gzip compressed data, was "vinhvh_package-0.0.9.tar", last modified: Wed Jul 26 07:34:38 2023, max compression
```

## Comparing `vinhvh_package-0.0.8.tar` & `vinhvh_package-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.253771 vinhvh_package-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      557 2023-07-25 05:19:12.250759 vinhvh_package-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.8/README.md
--rw-rw-rw-   0        0        0      612 2023-07-25 05:18:38.000000 vinhvh_package-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 05:19:12.254272 vinhvh_package-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.191601 vinhvh_package-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.200625 vinhvh_package-0.0.8/src/vinhvh_package/
--rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.8/src/vinhvh_package/__init__.py
--rw-rw-rw-   0        0        0    17789 2023-07-24 05:12:22.000000 vinhvh_package-0.0.8/src/vinhvh_package/test_module.py
--rw-rw-rw-   0        0        0    17662 2023-07-25 05:16:37.000000 vinhvh_package-0.0.8/src/vinhvh_package/vinhvh.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.244753 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/
--rw-rw-rw-   0        0        0      557 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 07:34:38.458907 vinhvh_package-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-07-26 07:34:38.457904 vinhvh_package-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.9/README.md
+-rw-rw-rw-   0        0        0      612 2023-07-26 07:14:33.000000 vinhvh_package-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:34:38.458907 vinhvh_package-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 07:34:38.327717 vinhvh_package-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:34:38.442861 vinhvh_package-0.0.9/src/vinhvh_package/
+-rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.9/src/vinhvh_package/__init__.py
+-rw-rw-rw-   0        0        0    17789 2023-07-24 05:12:22.000000 vinhvh_package-0.0.9/src/vinhvh_package/test_module.py
+-rw-rw-rw-   0        0        0    17604 2023-07-26 07:32:35.000000 vinhvh_package-0.0.9/src/vinhvh_package/vinhvh.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:34:38.456901 vinhvh_package-0.0.9/src/vinhvh_package.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-07-26 07:34:38.000000 vinhvh_package-0.0.9/src/vinhvh_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-07-26 07:34:38.000000 vinhvh_package-0.0.9/src/vinhvh_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:34:38.000000 vinhvh_package-0.0.9/src/vinhvh_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-26 07:34:38.000000 vinhvh_package-0.0.9/src/vinhvh_package.egg-info/top_level.txt
```

### Comparing `vinhvh_package-0.0.8/LICENSE` & `vinhvh_package-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vinhvh_package-0.0.8/PKG-INFO` & `vinhvh_package-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh_package
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vinhvh_package-0.0.8/pyproject.toml` & `vinhvh_package-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vinhvh_package"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="VinhVH", email="vinhvh89.dc@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vinhvh_package-0.0.8/src/vinhvh_package/test_module.py` & `vinhvh_package-0.0.9/src/vinhvh_package/test_module.py`

 * *Files identical despite different names*

### Comparing `vinhvh_package-0.0.8/src/vinhvh_package/vinhvh.py` & `vinhvh_package-0.0.9/src/vinhvh_package/vinhvh.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import openpyxl
 from openpyxl.styles import Font, Alignment, Border, Side, PatternFill
 from datetime import datetime, timedelta
 import time
 import os
 from pathlib import Path
 import logging
-import sys
 from pykml import parser
 
 
 def select_file(file: list = None, value: list = None, option: dict = None, checkbox: list = None, mode: str = 'single', title: str = 'File Selector'):
     """
     This function create a interface for user with different option input
 
@@ -110,19 +109,17 @@
 
             # Return the list of file paths
         return file_paths
 
     # If the user clicked the Cancel button, print a message and exit the program
     elif event == 'Cancel':
         print('File selection cancelled.')
-        sys.exit()
     # If the user closed the window, print a message and exit the program
     elif event == sg.WIN_CLOSED:
         print('File selection closed.')
-        sys.exit()
     # If the user didn't select any files, return None
     else:
         return None
 
 
 def read_file(filepath: str, sheet_name: str = None, skip_row: int = 0):
     """
@@ -340,14 +337,15 @@
     # Calculate the number of whole days remaining in the license period
     days_remaining = int(time_compare / 86400)
 
     # Determine the status of the license based on the number of days remaining
     if days_remaining < 0:
         print('Your program license has been expired, please contact to provider for more information!')
         return False
+        time.sleep(10)
     elif days_remaining == 0 or days_remaining == 1:
         print(f'License: {days_remaining} day')
         return True
     elif days_remaining <= 30 and days_remaining > 1:
         print('Lic = True')
         print(f'License: {days_remaining} days')
         return True
@@ -483,17 +481,16 @@
     return
     ----------
     Dict of common value
     """
 
     site_types = {
         'IBC': ['7', '8', '9', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'I4BA', 'I4BB', 'I4BC', 'I4BD', 'I4BE', 'I4BF', 'I4BJ', 'I4BK', 'I4CA', 'I4CB', 'I4CC', 'I4CD', 'I4CE', 'I4CF', 'I4CJ', 'I4CK'],
-        'Macro': ['1', '2', '3', '4', '5', '6', 'A', 'B', 'D', 'E', 'F', 'G', 'H', 'I', 'M4BA', 'M4BB', 'M4BC', 'M4BD', 'M4BE', 'M4BF', 'M4BG', 'M4BH', 'M4BI', 'M4CA', 'M4CB', 'M4CC', 'M4CD', 'M4CE', 'U4BA', 'U4BB', 'U4BC', 'U4CA', 'U4CB', 'U4CC', 'A_LTE', 'B_LTE', 'C_LTE', 'D_LTE', 'E_LTE', 'F_LTE'],
-        'CRAN - indoor': ['J4BA', 'J4BB', 'J4BC', 'J4CA', 'J4CB', 'J4CC'],
-        'CRAN - outdoor': ['C4BA', 'C4BB', 'C4BC', 'C4CA', 'C4CB', 'C4CC'],
+        'Macro': ['1', '2', '3', '4', '5', '6', 'A', 'B', 'D', 'E', 'F', 'G', 'H', 'I', 'M4BA', 'M4BB', 'M4BC', 'M4BD', 'M4BE', 'M4BF', 'M4BG', 'M4BH', 'M4BI', 'M4CA', 'M4CB', 'M4CC', 'M4CD', 'M4CE', 'U4BA', 'U4BB', 'U4BC', 'U4CA', 'U4CB', 'U4CC', 'A_LTE', 'B_LTE', 'C_LTE', 'D_LTE', 'E_LTE', 'F_LTE', '_LTE'],
+        'CRAN': ['J4BA', 'J4BB', 'J4BC', 'J4CA', 'J4CB', 'J4CC', 'C4BA', 'C4BB', 'C4BC', 'C4CA', 'C4CB', 'C4CC'],
         'Smallcell': ['S']
     }
     for site_type, codes in site_types.items():
         if x in codes:
             return site_type
     return 'Other'
```

### Comparing `vinhvh_package-0.0.8/src/vinhvh_package.egg-info/PKG-INFO` & `vinhvh_package-0.0.9/src/vinhvh_package.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh-package
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

