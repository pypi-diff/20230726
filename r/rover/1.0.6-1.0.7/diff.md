# Comparing `tmp/rover-1.0.6.tar.gz` & `tmp/rover-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover-1.0.6.tar", last modified: Tue Jul 25 22:11:30 2023, max compression
+gzip compressed data, was "rover-1.0.7.tar", last modified: Tue Jul 25 22:18:54 2023, max compression
```

## Comparing `rover-1.0.6.tar` & `rover-1.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.253178 rover-1.0.6/
--rw-r--r--   0 chad       (501) staff       (20)    35213 2023-07-25 22:11:11.000000 rover-1.0.6/LICENSE
--rw-r--r--   0 chad       (501) staff       (20)     1337 2023-07-25 22:11:30.252756 rover-1.0.6/PKG-INFO
--rw-r--r--   0 chad       (501) staff       (20)      477 2023-07-25 22:11:11.000000 rover-1.0.6/README.md
-drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.244909 rover-1.0.6/rover/
--rw-r--r--   0 chad       (501) staff       (20)        6 2023-07-25 22:11:03.000000 rover-1.0.6/rover/VERSION
--rw-r--r--   0 chad       (501) staff       (20)     6242 2023-07-25 22:11:04.000000 rover-1.0.6/rover/__init__.py
--rw-r--r--   0 chad       (501) staff       (20)      337 2023-07-25 22:11:04.000000 rover-1.0.6/rover/__main__.py
--rw-r--r--   0 chad       (501) staff       (20)    30000 2023-07-25 22:11:05.000000 rover-1.0.6/rover/args.py
--rw-r--r--   0 chad       (501) staff       (20)     6391 2023-07-25 22:11:05.000000 rover-1.0.6/rover/asdf.py
--rw-r--r--   0 chad       (501) staff       (20)     9180 2023-07-25 22:11:05.000000 rover-1.0.6/rover/config.py
--rw-r--r--   0 chad       (501) staff       (20)    11222 2023-07-25 22:11:06.000000 rover-1.0.6/rover/coverage.py
--rw-r--r--   0 chad       (501) staff       (20)     8166 2023-07-25 22:11:06.000000 rover-1.0.6/rover/daemon.py
--rw-r--r--   0 chad       (501) staff       (20)     6440 2023-07-25 22:11:06.000000 rover-1.0.6/rover/download.py
--rw-r--r--   0 chad       (501) staff       (20)     9403 2023-07-25 22:11:06.000000 rover-1.0.6/rover/help.py
--rw-r--r--   0 chad       (501) staff       (20)    13285 2023-07-25 22:11:06.000000 rover-1.0.6/rover/index.py
--rw-r--r--   0 chad       (501) staff       (20)     7413 2023-07-25 22:11:07.000000 rover-1.0.6/rover/ingest.py
--rw-r--r--   0 chad       (501) staff       (20)     5092 2023-07-25 22:11:07.000000 rover-1.0.6/rover/lock.py
--rw-r--r--   0 chad       (501) staff       (20)     4354 2023-07-25 22:11:07.000000 rover-1.0.6/rover/logs.py
--rw-r--r--   0 chad       (501) staff       (20)    41967 2023-07-25 22:11:08.000000 rover-1.0.6/rover/manager.py
--rw-r--r--   0 chad       (501) staff       (20)     6435 2023-07-25 22:11:08.000000 rover-1.0.6/rover/process.py
--rw-r--r--   0 chad       (501) staff       (20)     7379 2023-07-25 22:11:08.000000 rover-1.0.6/rover/report.py
--rw-r--r--   0 chad       (501) staff       (20)     7407 2023-07-25 22:11:08.000000 rover-1.0.6/rover/request.py
--rw-r--r--   0 chad       (501) staff       (20)     7980 2023-07-25 22:11:08.000000 rover-1.0.6/rover/retrieve.py
--rw-r--r--   0 chad       (501) staff       (20)     8015 2023-07-25 22:11:09.000000 rover-1.0.6/rover/retrieve_metadata.py
--rw-r--r--   0 chad       (501) staff       (20)     7172 2023-07-25 22:11:09.000000 rover-1.0.6/rover/scan.py
--rw-r--r--   0 chad       (501) staff       (20)     4533 2023-07-25 22:11:09.000000 rover-1.0.6/rover/sqlite.py
--rw-r--r--   0 chad       (501) staff       (20)    11092 2023-07-25 22:11:09.000000 rover-1.0.6/rover/subscribe.py
--rw-r--r--   0 chad       (501) staff       (20)     7464 2023-07-25 22:11:09.000000 rover-1.0.6/rover/summary.py
--rw-r--r--   0 chad       (501) staff       (20)    21905 2023-07-25 22:11:10.000000 rover-1.0.6/rover/utils.py
--rw-r--r--   0 chad       (501) staff       (20)     9359 2023-07-25 22:11:10.000000 rover-1.0.6/rover/web.py
--rw-r--r--   0 chad       (501) staff       (20)     3930 2023-07-25 22:11:10.000000 rover-1.0.6/rover/workers.py
-drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.247700 rover-1.0.6/rover.egg-info/
--rw-r--r--   0 chad       (501) staff       (20)     1337 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/PKG-INFO
--rw-r--r--   0 chad       (501) staff       (20)      812 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/SOURCES.txt
--rw-r--r--   0 chad       (501) staff       (20)        1 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/dependency_links.txt
--rw-r--r--   0 chad       (501) staff       (20)       37 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/entry_points.txt
--rw-r--r--   0 chad       (501) staff       (20)       68 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/requires.txt
--rw-r--r--   0 chad       (501) staff       (20)       12 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/top_level.txt
--rw-r--r--   0 chad       (501) staff       (20)       38 2023-07-25 22:11:30.253306 rover-1.0.6/setup.cfg
--rw-r--r--   0 chad       (501) staff       (20)     1673 2023-07-25 22:11:11.000000 rover-1.0.6/setup.py
-drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.252193 rover-1.0.6/tests/
--rw-r--r--   0 chad       (501) staff       (20)        0 2023-07-25 22:11:03.000000 rover-1.0.6/tests/__init__.py
--rw-r--r--   0 chad       (501) staff       (20)     4842 2023-07-25 22:11:10.000000 rover-1.0.6/tests/config.py
--rw-r--r--   0 chad       (501) staff       (20)     5898 2023-07-25 22:11:11.000000 rover-1.0.6/tests/coverage.py
--rw-r--r--   0 chad       (501) staff       (20)     1186 2023-07-25 22:11:11.000000 rover-1.0.6/tests/download.py
--rw-r--r--   0 chad       (501) staff       (20)     2423 2023-07-25 22:11:11.000000 rover-1.0.6/tests/index.py
--rw-r--r--   0 chad       (501) staff       (20)     1097 2023-07-25 22:11:11.000000 rover-1.0.6/tests/ingest.py
--rw-r--r--   0 chad       (501) staff       (20)     2474 2023-07-25 22:11:11.000000 rover-1.0.6/tests/logs.py
--rw-r--r--   0 chad       (501) staff       (20)     1500 2023-07-25 22:11:11.000000 rover-1.0.6/tests/retrieve.py
--rw-r--r--   0 chad       (501) staff       (20)     3391 2023-07-25 22:11:11.000000 rover-1.0.6/tests/test_utils.py
--rw-r--r--   0 chad       (501) staff       (20)     1442 2023-07-25 22:11:11.000000 rover-1.0.6/tests/utils.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:18:54.331726 rover-1.0.7/
+-rw-r--r--   0 chad       (501) staff       (20)    35213 2023-07-25 22:18:50.000000 rover-1.0.7/LICENSE
+-rw-r--r--   0 chad       (501) staff       (20)     1335 2023-07-25 22:18:54.331332 rover-1.0.7/PKG-INFO
+-rw-r--r--   0 chad       (501) staff       (20)      475 2023-07-25 22:18:50.000000 rover-1.0.7/README.md
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:18:54.323475 rover-1.0.7/rover/
+-rw-r--r--   0 chad       (501) staff       (20)        6 2023-07-25 22:18:42.000000 rover-1.0.7/rover/VERSION
+-rw-r--r--   0 chad       (501) staff       (20)     6242 2023-07-25 22:18:43.000000 rover-1.0.7/rover/__init__.py
+-rw-r--r--   0 chad       (501) staff       (20)      337 2023-07-25 22:18:43.000000 rover-1.0.7/rover/__main__.py
+-rw-r--r--   0 chad       (501) staff       (20)    30000 2023-07-25 22:18:44.000000 rover-1.0.7/rover/args.py
+-rw-r--r--   0 chad       (501) staff       (20)     6391 2023-07-25 22:18:44.000000 rover-1.0.7/rover/asdf.py
+-rw-r--r--   0 chad       (501) staff       (20)     9180 2023-07-25 22:18:44.000000 rover-1.0.7/rover/config.py
+-rw-r--r--   0 chad       (501) staff       (20)    11222 2023-07-25 22:18:45.000000 rover-1.0.7/rover/coverage.py
+-rw-r--r--   0 chad       (501) staff       (20)     8166 2023-07-25 22:18:45.000000 rover-1.0.7/rover/daemon.py
+-rw-r--r--   0 chad       (501) staff       (20)     6440 2023-07-25 22:18:45.000000 rover-1.0.7/rover/download.py
+-rw-r--r--   0 chad       (501) staff       (20)     9403 2023-07-25 22:18:45.000000 rover-1.0.7/rover/help.py
+-rw-r--r--   0 chad       (501) staff       (20)    13285 2023-07-25 22:18:46.000000 rover-1.0.7/rover/index.py
+-rw-r--r--   0 chad       (501) staff       (20)     7413 2023-07-25 22:18:46.000000 rover-1.0.7/rover/ingest.py
+-rw-r--r--   0 chad       (501) staff       (20)     5092 2023-07-25 22:18:46.000000 rover-1.0.7/rover/lock.py
+-rw-r--r--   0 chad       (501) staff       (20)     4354 2023-07-25 22:18:46.000000 rover-1.0.7/rover/logs.py
+-rw-r--r--   0 chad       (501) staff       (20)    41967 2023-07-25 22:18:47.000000 rover-1.0.7/rover/manager.py
+-rw-r--r--   0 chad       (501) staff       (20)     6435 2023-07-25 22:18:47.000000 rover-1.0.7/rover/process.py
+-rw-r--r--   0 chad       (501) staff       (20)     7379 2023-07-25 22:18:47.000000 rover-1.0.7/rover/report.py
+-rw-r--r--   0 chad       (501) staff       (20)     7407 2023-07-25 22:18:47.000000 rover-1.0.7/rover/request.py
+-rw-r--r--   0 chad       (501) staff       (20)     7980 2023-07-25 22:18:48.000000 rover-1.0.7/rover/retrieve.py
+-rw-r--r--   0 chad       (501) staff       (20)     8015 2023-07-25 22:18:48.000000 rover-1.0.7/rover/retrieve_metadata.py
+-rw-r--r--   0 chad       (501) staff       (20)     7172 2023-07-25 22:18:48.000000 rover-1.0.7/rover/scan.py
+-rw-r--r--   0 chad       (501) staff       (20)     4533 2023-07-25 22:18:48.000000 rover-1.0.7/rover/sqlite.py
+-rw-r--r--   0 chad       (501) staff       (20)    11092 2023-07-25 22:18:48.000000 rover-1.0.7/rover/subscribe.py
+-rw-r--r--   0 chad       (501) staff       (20)     7464 2023-07-25 22:18:48.000000 rover-1.0.7/rover/summary.py
+-rw-r--r--   0 chad       (501) staff       (20)    21905 2023-07-25 22:18:49.000000 rover-1.0.7/rover/utils.py
+-rw-r--r--   0 chad       (501) staff       (20)     9359 2023-07-25 22:18:49.000000 rover-1.0.7/rover/web.py
+-rw-r--r--   0 chad       (501) staff       (20)     3930 2023-07-25 22:18:50.000000 rover-1.0.7/rover/workers.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:18:54.326340 rover-1.0.7/rover.egg-info/
+-rw-r--r--   0 chad       (501) staff       (20)     1335 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/PKG-INFO
+-rw-r--r--   0 chad       (501) staff       (20)      812 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/SOURCES.txt
+-rw-r--r--   0 chad       (501) staff       (20)        1 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/dependency_links.txt
+-rw-r--r--   0 chad       (501) staff       (20)       37 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/entry_points.txt
+-rw-r--r--   0 chad       (501) staff       (20)       68 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/requires.txt
+-rw-r--r--   0 chad       (501) staff       (20)       12 2023-07-25 22:18:54.000000 rover-1.0.7/rover.egg-info/top_level.txt
+-rw-r--r--   0 chad       (501) staff       (20)       38 2023-07-25 22:18:54.331846 rover-1.0.7/setup.cfg
+-rw-r--r--   0 chad       (501) staff       (20)     1673 2023-07-25 22:18:50.000000 rover-1.0.7/setup.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:18:54.330774 rover-1.0.7/tests/
+-rw-r--r--   0 chad       (501) staff       (20)        0 2023-07-25 22:18:42.000000 rover-1.0.7/tests/__init__.py
+-rw-r--r--   0 chad       (501) staff       (20)     4842 2023-07-25 22:18:50.000000 rover-1.0.7/tests/config.py
+-rw-r--r--   0 chad       (501) staff       (20)     5898 2023-07-25 22:18:50.000000 rover-1.0.7/tests/coverage.py
+-rw-r--r--   0 chad       (501) staff       (20)     1186 2023-07-25 22:18:50.000000 rover-1.0.7/tests/download.py
+-rw-r--r--   0 chad       (501) staff       (20)     2423 2023-07-25 22:18:50.000000 rover-1.0.7/tests/index.py
+-rw-r--r--   0 chad       (501) staff       (20)     1097 2023-07-25 22:18:50.000000 rover-1.0.7/tests/ingest.py
+-rw-r--r--   0 chad       (501) staff       (20)     2474 2023-07-25 22:18:50.000000 rover-1.0.7/tests/logs.py
+-rw-r--r--   0 chad       (501) staff       (20)     1500 2023-07-25 22:18:50.000000 rover-1.0.7/tests/retrieve.py
+-rw-r--r--   0 chad       (501) staff       (20)     3391 2023-07-25 22:18:50.000000 rover-1.0.7/tests/test_utils.py
+-rw-r--r--   0 chad       (501) staff       (20)     1442 2023-07-25 22:18:50.000000 rover-1.0.7/tests/utils.py
```

### Comparing `rover-1.0.6/LICENSE` & `rover-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/PKG-INFO` & `rover-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tool for the robust retrieval of seismic data
 Home-page: https://earthscope.github.io/rover
 Author: EarthScope
 Author-email: software@earthscope.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -19,10 +19,10 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mseedindex
 License-File: LICENSE
 
 # rover 
 
-Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](https://service.iris.edu/fdsnws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
+Tool for the robust retrieval of seismic (and other) data from a data center such as the [EarthScope](https://www.earthscope.org/data).  For this tool to work the data center must offer both a [fdsnws-availability](https://service.iris.edu/fdsnws/availability/1/) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
 
 For more installation instructions and quick start see the [User Guide](https://earthscope.github.io/rover/).
```

### Comparing `rover-1.0.6/rover/__init__.py` & `rover-1.0.7/rover/__init__.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/args.py` & `rover-1.0.7/rover/args.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/asdf.py` & `rover-1.0.7/rover/asdf.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/config.py` & `rover-1.0.7/rover/config.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/coverage.py` & `rover-1.0.7/rover/coverage.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/daemon.py` & `rover-1.0.7/rover/daemon.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/download.py` & `rover-1.0.7/rover/download.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/help.py` & `rover-1.0.7/rover/help.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/index.py` & `rover-1.0.7/rover/index.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/ingest.py` & `rover-1.0.7/rover/ingest.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/lock.py` & `rover-1.0.7/rover/lock.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/logs.py` & `rover-1.0.7/rover/logs.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/manager.py` & `rover-1.0.7/rover/manager.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/process.py` & `rover-1.0.7/rover/process.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/report.py` & `rover-1.0.7/rover/report.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/request.py` & `rover-1.0.7/rover/request.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/retrieve.py` & `rover-1.0.7/rover/retrieve.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/retrieve_metadata.py` & `rover-1.0.7/rover/retrieve_metadata.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/scan.py` & `rover-1.0.7/rover/scan.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/sqlite.py` & `rover-1.0.7/rover/sqlite.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/subscribe.py` & `rover-1.0.7/rover/subscribe.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/summary.py` & `rover-1.0.7/rover/summary.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/utils.py` & `rover-1.0.7/rover/utils.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/web.py` & `rover-1.0.7/rover/web.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover/workers.py` & `rover-1.0.7/rover/workers.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/rover.egg-info/PKG-INFO` & `rover-1.0.7/rover.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tool for the robust retrieval of seismic data
 Home-page: https://earthscope.github.io/rover
 Author: EarthScope
 Author-email: software@earthscope.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -19,10 +19,10 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mseedindex
 License-File: LICENSE
 
 # rover 
 
-Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](https://service.iris.edu/fdsnws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
+Tool for the robust retrieval of seismic (and other) data from a data center such as the [EarthScope](https://www.earthscope.org/data).  For this tool to work the data center must offer both a [fdsnws-availability](https://service.iris.edu/fdsnws/availability/1/) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
 
 For more installation instructions and quick start see the [User Guide](https://earthscope.github.io/rover/).
```

### Comparing `rover-1.0.6/rover.egg-info/SOURCES.txt` & `rover-1.0.7/rover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/setup.py` & `rover-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/config.py` & `rover-1.0.7/tests/config.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/coverage.py` & `rover-1.0.7/tests/coverage.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/download.py` & `rover-1.0.7/tests/download.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/index.py` & `rover-1.0.7/tests/index.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/ingest.py` & `rover-1.0.7/tests/ingest.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/logs.py` & `rover-1.0.7/tests/logs.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/retrieve.py` & `rover-1.0.7/tests/retrieve.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/test_utils.py` & `rover-1.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rover-1.0.6/tests/utils.py` & `rover-1.0.7/tests/utils.py`

 * *Files identical despite different names*

