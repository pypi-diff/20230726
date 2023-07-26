# Comparing `tmp/nlproc-tools-0.0.1.tar.gz` & `tmp/nlproc_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\heine\Documents\research\nlproc.tools\helper\dist\.tmp-g9fbofi9\nlproc-tools-0.0.1.tar", last modified: Sun Jul 23 23:58:09 2023, max compression
+gzip compressed data, was "C:\Users\heine\Documents\research\nlproc.tools\data_tools\dist\.tmp-twkdh_6j\nlproc_tools-0.0.2.tar", last modified: Wed Jul 26 07:19:21 2023, max compression
```

## Comparing `nlproc-tools-0.0.1.tar` & `nlproc_tools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 23:58:09.867741 nlproc-tools-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-23 23:56:05.000000 nlproc-tools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      669 2023-07-23 23:58:09.867741 nlproc-tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-07-23 23:56:54.000000 nlproc-tools-0.0.1/README.md
--rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 nlproc-tools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      720 2023-07-23 23:58:09.877267 nlproc-tools-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-23 23:58:09.822111 nlproc-tools-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 23:58:09.842185 nlproc-tools-0.0.1/src/nlproc-tools/
--rw-rw-rw-   0        0        0        0 2023-07-23 23:51:23.000000 nlproc-tools-0.0.1/src/nlproc-tools/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-23 23:51:23.000000 nlproc-tools-0.0.1/src/nlproc-tools/main.py
-drwxrwxrwx   0        0        0        0 2023-07-23 23:58:09.865733 nlproc-tools-0.0.1/src/nlproc_tools.egg-info/
--rw-rw-rw-   0        0        0      669 2023-07-23 23:58:09.000000 nlproc-tools-0.0.1/src/nlproc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-07-23 23:58:09.000000 nlproc-tools-0.0.1/src/nlproc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 23:58:09.000000 nlproc-tools-0.0.1/src/nlproc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-23 23:58:09.000000 nlproc-tools-0.0.1/src/nlproc_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.488420 nlproc_tools-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 23:56:05.000000 nlproc_tools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      770 2023-07-26 07:19:21.489419 nlproc_tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-24 01:33:17.000000 nlproc_tools-0.0.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 nlproc_tools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      720 2023-07-26 07:19:21.491418 nlproc_tools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.441112 nlproc_tools-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.457418 nlproc_tools-0.0.2/src/nlproc_tools/
+-rw-rw-rw-   0        0        0      108 2023-07-26 06:12:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/__init__.py
+-rw-rw-rw-   0        0        0     2469 2023-07-26 05:03:26.000000 nlproc_tools-0.0.2/src/nlproc_tools/convert.py
+-rw-rw-rw-   0        0        0     2555 2023-07-26 06:34:44.000000 nlproc_tools-0.0.2/src/nlproc_tools/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.487421 nlproc_tools-0.0.2/src/nlproc_tools/datasets/
+-rw-rw-rw-   0        0        0        0 2023-07-24 00:28:54.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2160 2023-07-23 23:48:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/da-san-martino-etal-2019.py
+-rw-rw-rw-   0        0        0      895 2023-07-23 23:32:07.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/frank.py
+-rw-rw-rw-   0        0        0     3910 2023-07-23 23:48:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/mqm.py
+-rw-rw-rw-   0        0        0       33 2023-07-23 23:32:28.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/salsa.py
+-rw-rw-rw-   0        0        0     2048 2023-07-23 23:48:49.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/scarecrow.py
+-rw-rw-rw-   0        0        0     1277 2023-07-24 00:39:40.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/snac.py
+-rw-rw-rw-   0        0        0     2336 2023-07-23 23:47:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/datasets/wu-etal-2023.py
+-rw-rw-rw-   0        0        0     1783 2023-07-26 06:09:42.000000 nlproc_tools-0.0.2/src/nlproc_tools/names.py
+-rw-rw-rw-   0        0        0      768 2023-07-26 06:29:10.000000 nlproc_tools-0.0.2/src/nlproc_tools/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:19:21.474429 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 07:19:21.000000 nlproc_tools-0.0.2/src/nlproc_tools.egg-info/top_level.txt
```

### Comparing `nlproc-tools-0.0.1/LICENSE` & `nlproc_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlproc-tools-0.0.1/PKG-INFO` & `nlproc_tools-0.0.2/src/nlproc_tools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nlproc-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A helper package for loading / managing data collection with nlproc.tools
 Home-page: https://github.com/davidheineman/nlproc.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/nlproc.tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## nlproc-tools
+## nlproc_tools
 
-This is a helper library for [nlproc.tools](https://nlproc.tools/).
+This is a helper library for [**nlproc.tools**](https://nlproc.tools/). Please see the [**main repo**](https://github.com/davidheineman/nlproc.tools) for documentation.
```

### Comparing `nlproc-tools-0.0.1/setup.cfg` & `nlproc_tools-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 6c70 726f 632d 746f 6f6c 730d   = nlproc-tools.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000010: 203d 206e 6c70 726f 635f 746f 6f6c 730d   = nlproc_tools.
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
 00000030: 0d0a 6175 7468 6f72 203d 2044 6176 6964  ..author = David
 00000040: 2048 6569 6e65 6d61 6e0d 0a61 7574 686f   Heineman..autho
 00000050: 725f 656d 6169 6c20 3d20 6468 6569 6e65  r_email = dheine
 00000060: 6d61 6e33 4067 6174 6563 682e 6564 750d  man3@gatech.edu.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2068 656c 7065 7220 7061 636b 6167 6520   helper package 
 00000090: 666f 7220 6c6f 6164 696e 6720 2f20 6d61  for loading / ma
```

### Comparing `nlproc-tools-0.0.1/src/nlproc_tools.egg-info/PKG-INFO` & `nlproc_tools-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: nlproc-tools
-Version: 0.0.1
+Name: nlproc_tools
+Version: 0.0.2
 Summary: A helper package for loading / managing data collection with nlproc.tools
 Home-page: https://github.com/davidheineman/nlproc.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/nlproc.tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## nlproc-tools
+## nlproc_tools
 
-This is a helper library for [nlproc.tools](https://nlproc.tools/).
+This is a helper library for [**nlproc.tools**](https://nlproc.tools/). Please see the [**main repo**](https://github.com/davidheineman/nlproc.tools) for documentation.
```

