# Comparing `tmp/pypeims-0.0.3.tar.gz` & `tmp/pypeims-0.0.31.tar.gz`

## Comparing `pypeims-0.0.3.tar` & `pypeims-0.0.31.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/__init__.py
--rw-r--r--   0        0        0    84075 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx
--rw-r--r--   0        0        0   190464 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls
--rw-r--r--   0        0        0    72044 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/instruments/__init__.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pypeims-0.0.3/src/instruments/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pypeims-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pypeims-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pypeims-0.0.3/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pypeims-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pypeims-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.31/__init__.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/__init__.py
+-rw-r--r--   0        0        0    84075 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx
+-rw-r--r--   0        0        0   190464 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls
+-rw-r--r--   0        0        0    72044 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/instruments/__init__.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pypeims-0.0.31/src/pypeims/instruments/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pypeims-0.0.31/tests/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pypeims-0.0.31/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypeims-0.0.31/LICENSE.txt
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pypeims-0.0.31/README.md
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 pypeims-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pypeims-0.0.31/PKG-INFO
```

### Comparing `pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx` & `pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls` & `pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.3/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx` & `pypeims-0.0.31/src/pypeims/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.3/src/instruments/utils.py` & `pypeims-0.0.31/src/pypeims/instruments/utils.py`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.3/.gitignore` & `pypeims-0.0.31/.gitignore`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.3/LICENSE.txt` & `pypeims-0.0.31/LICENSE.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Copyright (c) 2023-present Alejandro Pena <adpena@gmail.com>
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

