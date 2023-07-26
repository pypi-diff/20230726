# Comparing `tmp/imgMS-0.2.7.tar.gz` & `tmp/imgMS-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgMS-0.2.7.tar", last modified: Thu May  4 20:04:05 2023, max compression
+gzip compressed data, was "imgMS-0.2.8.tar", last modified: Wed Jul 26 16:11:48 2023, max compression
```

## Comparing `imgMS-0.2.7.tar` & `imgMS-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 20:04:05.893142 imgMS-0.2.7/
--rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.7/LICENSE
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 20:04:05.892745 imgMS-0.2.7/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.7/README.md
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 20:04:05.890163 imgMS-0.2.7/imgMS/
--rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.7/imgMS/MSData.py
--rw-r--r--   0 nika       (501) staff       (20)    13416 2023-05-04 19:53:52.000000 imgMS-0.2.7/imgMS/MSEval.py
--rw-r--r--   0 nika       (501) staff       (20)     3603 2023-05-04 20:02:06.000000 imgMS-0.2.7/imgMS/MSStats.py
--rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.7/imgMS/__init__.py
--rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.7/imgMS/side_functions.py
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 20:04:05.892072 imgMS-0.2.7/imgMS.egg-info/
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 20:04:05.000000 imgMS-0.2.7/imgMS.egg-info/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 20:04:05.000000 imgMS-0.2.7/imgMS.egg-info/SOURCES.txt
--rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 20:04:05.000000 imgMS-0.2.7/imgMS.egg-info/dependency_links.txt
--rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 20:04:05.000000 imgMS-0.2.7/imgMS.egg-info/requires.txt
--rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 20:04:05.000000 imgMS-0.2.7/imgMS.egg-info/top_level.txt
--rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 20:04:05.893300 imgMS-0.2.7/setup.cfg
--rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 20:03:04.000000 imgMS-0.2.7/setup.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-07-26 16:11:48.117231 imgMS-0.2.8/
+-rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.8/LICENSE
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-07-26 16:11:48.116745 imgMS-0.2.8/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.8/README.md
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-07-26 16:11:48.113486 imgMS-0.2.8/imgMS/
+-rw-r--r--   0 nika       (501) staff       (20)    38943 2023-07-26 13:11:04.000000 imgMS-0.2.8/imgMS/MSData.py
+-rw-r--r--   0 nika       (501) staff       (20)    13416 2023-05-04 19:53:52.000000 imgMS-0.2.8/imgMS/MSEval.py
+-rw-r--r--   0 nika       (501) staff       (20)     6005 2023-07-26 16:09:15.000000 imgMS-0.2.8/imgMS/MSStats.py
+-rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.8/imgMS/__init__.py
+-rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.8/imgMS/side_functions.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-07-26 16:11:48.116026 imgMS-0.2.8/imgMS.egg-info/
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-07-26 16:11:48.000000 imgMS-0.2.8/imgMS.egg-info/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)      261 2023-07-26 16:11:48.000000 imgMS-0.2.8/imgMS.egg-info/SOURCES.txt
+-rw-r--r--   0 nika       (501) staff       (20)        1 2023-07-26 16:11:48.000000 imgMS-0.2.8/imgMS.egg-info/dependency_links.txt
+-rw-r--r--   0 nika       (501) staff       (20)       92 2023-07-26 16:11:48.000000 imgMS-0.2.8/imgMS.egg-info/requires.txt
+-rw-r--r--   0 nika       (501) staff       (20)        6 2023-07-26 16:11:48.000000 imgMS-0.2.8/imgMS.egg-info/top_level.txt
+-rw-r--r--   0 nika       (501) staff       (20)       38 2023-07-26 16:11:48.117369 imgMS-0.2.8/setup.cfg
+-rw-r--r--   0 nika       (501) staff       (20)      953 2023-07-26 15:54:53.000000 imgMS-0.2.8/setup.py
```

### Comparing `imgMS-0.2.7/LICENSE` & `imgMS-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.7/PKG-INFO` & `imgMS-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.7
+Version: 0.2.8
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.7/README.md` & `imgMS-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.7/imgMS/MSData.py` & `imgMS-0.2.8/imgMS/MSData.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
 
         if self.corrected_TS is not None:
             data['corrected_TS'] = self.corrected_TS
 
         for key, df in data.items():
             df.to_excel(writer, sheet_name=key)
 
-        writer.save()
+        writer.close()
 
     def formated_export(self, path, table='quantified'):
         """
         Export all data to excel file in a formated style, containing means, sd, max and min for repeated samples.
 
         Parameters
         ----------
@@ -577,15 +577,15 @@
             if quantified is False:
                 df = pd.DataFrame(isotope.elmap.matrix,
                                   index=isotope.elmap.y, columns=isotope.elmap.x)
             else:
                 df = pd.DataFrame(isotope.elmap.qmap,
                                   index=isotope.elmap.y, columns=isotope.elmap.x)
             df.to_excel(writer, sheet_name=el)
-        writer.save()
+        writer.close()
 
     def import_matrices(self, path):
         """
         Import all elemental distribution data from excel file. Each isotope
         will be a matrix on one sheet.
 
         Parameters
@@ -1053,15 +1053,15 @@
         el: str
             Name of isotope to export. Will be used as sheet name.
         """
 
         writer = pd.ExcelWriter(path, engine='xlsxwriter')
         df = pd.DataFrame(self.matrix, index=self.y, columns=self.x)
         df.to_excel(writer, sheet_name=el)
-        writer.save()
+        writer.close()
 
     def rotate(self):
         """
         Rotate map by 90 degrees.
         """
 
         self.matrix = np.rot90(self.matrix)
```

### Comparing `imgMS-0.2.7/imgMS/MSEval.py` & `imgMS-0.2.8/imgMS/MSEval.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.7/imgMS/side_functions.py` & `imgMS-0.2.8/imgMS/side_functions.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.7/imgMS.egg-info/PKG-INFO` & `imgMS-0.2.8/imgMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.7
+Version: 0.2.8
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.7/setup.py` & `imgMS-0.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='imgMS',
-    version='0.2.7',
+    version='0.2.8',
     author='nikadilli',
     author_email='nikadilli@gmail.com',
     url="https://github.com/nikadilli/imgMS",
     packages=setuptools.find_packages(),
     scripts=[],
     license='LICENSE.txt',
     description='Package for data reduction of LA-ICP-MS data.',
```

