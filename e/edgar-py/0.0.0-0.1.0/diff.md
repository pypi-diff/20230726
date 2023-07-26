# Comparing `tmp/edgar-py-0.0.0.tar.gz` & `tmp/edgar-py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgar-py-0.0.0.tar", last modified: Wed Jul 26 02:53:13 2023, max compression
+gzip compressed data, was "edgar-py-0.1.0.tar", last modified: Wed Jul 26 06:17:16 2023, max compression
```

## Comparing `edgar-py-0.0.0.tar` & `edgar-py-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 02:53:13.623418 edgar-py-0.0.0/
--rw-rw-rw-   0        0        0     1087 2023-07-19 23:13:03.000000 edgar-py-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     2210 2023-07-26 02:53:13.621419 edgar-py-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-19 23:08:24.000000 edgar-py-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 02:53:13.603414 edgar-py-0.0.0/edgar/
--rw-rw-rw-   0        0        0        0 2023-07-19 23:08:10.000000 edgar-py-0.0.0/edgar/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-19 23:08:10.000000 edgar-py-0.0.0/edgar/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 02:53:13.619419 edgar-py-0.0.0/edgar_py.egg-info/
--rw-rw-rw-   0        0        0     2210 2023-07-26 02:53:13.000000 edgar-py-0.0.0/edgar_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-07-26 02:53:13.000000 edgar-py-0.0.0/edgar_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 02:53:13.000000 edgar-py-0.0.0/edgar_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 02:53:13.000000 edgar-py-0.0.0/edgar_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-07-19 23:19:17.000000 edgar-py-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 02:53:13.623418 edgar-py-0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.753755 edgar-py-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-19 23:13:03.000000 edgar-py-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2109 2023-07-26 06:17:16.753755 edgar-py-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-19 23:08:24.000000 edgar-py-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.627907 edgar-py-0.1.0/edgar/
+-rw-rw-rw-   0        0        0       40 2023-07-26 06:12:34.000000 edgar-py-0.1.0/edgar/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-19 23:08:10.000000 edgar-py-0.1.0/edgar/__main__.py
+-rw-rw-rw-   0        0        0     2526 2023-07-26 06:12:34.000000 edgar-py-0.1.0/edgar/cik.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.745755 edgar-py-0.1.0/edgar_py.egg-info/
+-rw-rw-rw-   0        0        0     2109 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      479 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1714 2023-07-26 06:14:42.000000 edgar-py-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 06:17:16.753755 edgar-py-0.1.0/setup.cfg
```

### Comparing `edgar-py-0.0.0/LICENSE` & `edgar-py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgar-py-0.0.0/PKG-INFO` & `edgar-py-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-py
-Version: 0.0.0
+Version: 0.1.0
 Summary: Web scraper and API wrapper for the SEC EDGAR tool.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,24 +22,22 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/JacobLee23/EDGAR-py
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EDGAR-py
```

### Comparing `edgar-py-0.0.0/edgar_py.egg-info/PKG-INFO` & `edgar-py-0.1.0/edgar_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-py
-Version: 0.0.0
+Version: 0.1.0
 Summary: Web scraper and API wrapper for the SEC EDGAR tool.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,24 +22,22 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/JacobLee23/EDGAR-py
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EDGAR-py
```

### Comparing `edgar-py-0.0.0/pyproject.toml` & `edgar-py-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="edgar-py"
-version="0.0.0"
+version="0.1.0"
 description = "Web scraper and API wrapper for the SEC EDGAR tool."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Office/Business :: Financial :: Investment",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 dependencies = [
+    "beautifulsoup4==4.12.2",
+    "certifi==2023.7.22 ; python_version >= '3.6'",
+    "charset-normalizer==3.2.0 ; python_full_version >= '3.7.0'",
+    "idna==3.4 ; python_version >= '3.5'",
+    "lxml==4.9.3",
+    "numpy==1.25.1 ; python_version >= '3.10'",
+    "pandas==2.0.3",
+    "python-dateutil==2.8.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+    "pytz==2023.3",
+    "requests==2.31.0",
+    "six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+    "soupsieve==2.4.1 ; python_version >= '3.7'",
+    "tzdata==2023.3 ; python_version >= '2'",
+    "urllib3==2.0.4 ; python_version >= '3.7'"
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/EDGAR-py"
 
 [tools.setuptools.packages.find]
 where = ["."]
```

