# Comparing `tmp/visokio_omniprint-1.1.1.tar.gz` & `tmp/visokio_omniprint-1.1.3.tar.gz`

## Comparing `visokio_omniprint-1.1.1.tar` & `visokio_omniprint-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/build.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/install.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/test_install.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/test_upload.sh
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/upload.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/DriverBase.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Image.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/ImagesPdf.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Pdf.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/README.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/scripts/build.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/scripts/install.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/scripts/test_install.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/scripts/test_upload.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/scripts/upload.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/DriverBase.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/Image.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/ImagesPdf.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/Pdf.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/Tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/visokio_omniprint/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/README.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.3/PKG-INFO
```

### Comparing `visokio_omniprint-1.1.1/visokio_omniprint/DriverBase.py` & `visokio_omniprint-1.1.3/visokio_omniprint/DriverBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return webdriver.Chrome(options=options, service=chrome_service)
 
     def get_driver_host(self, options):
         """
         This function creates a ChromeDriver instance to be used on the host machine.
         """
         version = self.get_compatible_chromedriver()
-        chrome_service = Service(ChromeDriverManager(version=version).install())
+        chrome_service = Service(ChromeDriverManager(driver_version=version).install())
         return webdriver.Chrome(options=options, service=chrome_service)
 
 
     def get_driver(self, is_docker):
         """
         This function creates and returns a ChromeDriver instance based on the provided configuration.
         """
```

### Comparing `visokio_omniprint-1.1.1/visokio_omniprint/Image.py` & `visokio_omniprint-1.1.3/visokio_omniprint/Image.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.1.1/visokio_omniprint/ImagesPdf.py` & `visokio_omniprint-1.1.3/visokio_omniprint/ImagesPdf.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.1.1/visokio_omniprint/Pdf.py` & `visokio_omniprint-1.1.3/visokio_omniprint/Pdf.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.1.1/visokio_omniprint/Tools.py` & `visokio_omniprint-1.1.3/visokio_omniprint/Tools.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.1.1/pyproject.toml` & `visokio_omniprint-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visokio-omniprint"
-version = "1.1.1"
+version = "1.1.3"
 description = "Visokio Omniscope PDF printing library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Visokio" },
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "selenium",
   "webdriver-manager",
-  "get-chrome-driver",
+  "get-chrome-driver>=1.3.19",
   "tinify",
   "fpdf",
   "urllib3"
 ]
 
 
 [project.urls]
```

### Comparing `visokio_omniprint-1.1.1/PKG-INFO` & `visokio_omniprint-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visokio-omniprint
-Version: 1.1.1
+Version: 1.1.3
 Summary: Visokio Omniscope PDF printing library
 Project-URL: Documentation, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint#readme
 Project-URL: Issues, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint/issues
 Project-URL: Source, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint
 Author: Visokio
 License-Expression: MIT
 License-File: LICENSE
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: fpdf
-Requires-Dist: get-chrome-driver
+Requires-Dist: get-chrome-driver>=1.3.19
 Requires-Dist: selenium
 Requires-Dist: tinify
 Requires-Dist: urllib3
 Requires-Dist: webdriver-manager
 Description-Content-Type: text/markdown
 
 Library providing pdf printing capabilities for Omniscope reports
```

