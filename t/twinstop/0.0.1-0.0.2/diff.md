# Comparing `tmp/twinstop-0.0.1.tar.gz` & `tmp/twinstop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.0.1.tar", last modified: Tue Jul 25 14:16:30 2023, max compression
+gzip compressed data, was "twinstop-0.0.2.tar", last modified: Wed Jul 26 09:00:54 2023, max compression
```

## Comparing `twinstop-0.0.1.tar` & `twinstop-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-25 14:16:30.137727 twinstop-0.0.1/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.1/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-25 14:16:30.137727 twinstop-0.0.1/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.1/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.1/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1001 2023-07-25 14:16:30.137727 twinstop-0.0.1/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.1/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-25 14:16:30.137727 twinstop-0.0.1/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-25 14:16:30.137727 twinstop-0.0.1/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.1/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-25 10:30:56.000000 twinstop-0.0.1/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4384 2023-07-25 13:13:21.000000 twinstop-0.0.1/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-25 14:16:30.137727 twinstop-0.0.1/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.1/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111754 2023-07-25 14:15:48.000000 twinstop-0.0.1/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.1/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-25 14:16:30.137727 twinstop-0.0.1/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-25 14:16:30.000000 twinstop-0.0.1/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      439 2023-07-25 14:16:30.000000 twinstop-0.0.1/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-25 14:16:30.000000 twinstop-0.0.1/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      187 2023-07-25 14:16:30.000000 twinstop-0.0.1/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-25 14:16:30.000000 twinstop-0.0.1/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.2/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 09:00:54.426179 twinstop-0.0.2/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.2/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.2/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1057 2023-07-26 09:00:54.426179 twinstop-0.0.2/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.2/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.422179 twinstop-0.0.2/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.2/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 08:55:34.000000 twinstop-0.0.2/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4384 2023-07-25 13:13:21.000000 twinstop-0.0.2/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.2/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111754 2023-07-25 14:16:44.000000 twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.bkp.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.2/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:00:54.426179 twinstop-0.0.2/src/twinstop.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      693 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      209 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-26 09:00:54.000000 twinstop-0.0.2/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.0.1/LICENSE` & `twinstop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.1/setup.cfg` & `twinstop-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twinstop
-version = 0.0.1
+version = attr: twinstop._version.__version__
 author = Marco Mariotti and Sergio Sanchez Moragues
 author_email = marco.mariotti@ub.edu
 description = twinstop identifies selenoproteins in close related transcriptomes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/marco-mariotti/twinstop
 project_urls = 
@@ -17,21 +17,22 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	biopython >= 1.78
+	biopython >= 1.78, <=1.81
 	easyterm >= 1.0.0
 	easybioinfo >= 0.2.1
 	extend_orfs >= 0.0.27
 	file-chunk-iterators >= 0.0.1
 	pyranges >= 0.0.120
 	pandas >= 1.3.5
+	pyfaidx >= 0.7.2
 	multiprocess >= 0.70.14
 	numpy >= 1.21.5
 	scikit-learn >= 1.3.0
 
 [options.packages.find]
 where = src
```

### Comparing `twinstop-0.0.1/src/twinstop/block_selection.py` & `twinstop-0.0.2/src/twinstop/block_selection.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.1/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.0.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.1/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.0.2/src/twinstop/denovo_selenoproteins_h3.bkp.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.1/src/twinstop/test_alignment_methods.py` & `twinstop-0.0.2/src/twinstop/test_alignment_methods.py`

 * *Files identical despite different names*

