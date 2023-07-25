# Comparing `tmp/rover-1.0.5.tar.gz` & `tmp/rover-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rover-1.0.5.tar", last modified: Sat Dec  7 00:47:20 2019, max compression
+gzip compressed data, was "rover-1.0.6.tar", last modified: Tue Jul 25 22:11:30 2023, max compression
```

## Comparing `rover-1.0.5.tar` & `rover-1.0.6.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 chad       (502) staff       (20)        0 2019-12-07 00:47:20.000000 rover-1.0.5/
--rw-r--r--   0 chad       (502) staff       (20)     1403 2019-12-07 00:47:20.000000 rover-1.0.5/PKG-INFO
--rw-r--r--   0 chad       (502) staff       (20)      474 2019-12-07 00:47:08.000000 rover-1.0.5/README.md
-drwxr-xr-x   0 chad       (502) staff       (20)        0 2019-12-07 00:47:20.000000 rover-1.0.5/rover/
--rw-r--r--   0 chad       (502) staff       (20)        6 2019-12-07 00:46:41.000000 rover-1.0.5/rover/VERSION
--rw-r--r--   0 chad       (502) staff       (20)     6242 2019-12-07 00:46:42.000000 rover-1.0.5/rover/__init__.py
--rw-r--r--   0 chad       (502) staff       (20)      337 2019-12-07 00:46:42.000000 rover-1.0.5/rover/__main__.py
--rw-r--r--   0 chad       (502) staff       (20)    30000 2019-12-07 00:46:45.000000 rover-1.0.5/rover/args.py
--rw-r--r--   0 chad       (502) staff       (20)     6391 2019-12-07 00:46:46.000000 rover-1.0.5/rover/asdf.py
--rw-r--r--   0 chad       (502) staff       (20)     9180 2019-12-07 00:46:47.000000 rover-1.0.5/rover/config.py
--rw-r--r--   0 chad       (502) staff       (20)    11222 2019-12-07 00:46:48.000000 rover-1.0.5/rover/coverage.py
--rw-r--r--   0 chad       (502) staff       (20)     8166 2019-12-07 00:46:49.000000 rover-1.0.5/rover/daemon.py
--rw-r--r--   0 chad       (502) staff       (20)     6440 2019-12-07 00:46:49.000000 rover-1.0.5/rover/download.py
--rw-r--r--   0 chad       (502) staff       (20)     9403 2019-12-07 00:46:50.000000 rover-1.0.5/rover/help.py
--rw-r--r--   0 chad       (502) staff       (20)    13285 2019-12-07 00:46:51.000000 rover-1.0.5/rover/index.py
--rw-r--r--   0 chad       (502) staff       (20)     7413 2019-12-07 00:46:52.000000 rover-1.0.5/rover/ingest.py
--rw-r--r--   0 chad       (502) staff       (20)     5092 2019-12-07 00:46:52.000000 rover-1.0.5/rover/lock.py
--rw-r--r--   0 chad       (502) staff       (20)     4354 2019-12-07 00:46:52.000000 rover-1.0.5/rover/logs.py
--rw-r--r--   0 chad       (502) staff       (20)    41967 2019-12-07 00:46:55.000000 rover-1.0.5/rover/manager.py
--rw-r--r--   0 chad       (502) staff       (20)     6435 2019-12-07 00:46:56.000000 rover-1.0.5/rover/process.py
--rw-r--r--   0 chad       (502) staff       (20)     7379 2019-12-07 00:46:57.000000 rover-1.0.5/rover/report.py
--rw-r--r--   0 chad       (502) staff       (20)     7407 2019-12-07 00:46:58.000000 rover-1.0.5/rover/request.py
--rw-r--r--   0 chad       (502) staff       (20)     7980 2019-12-07 00:46:58.000000 rover-1.0.5/rover/retrieve.py
--rw-r--r--   0 chad       (502) staff       (20)     8015 2019-12-07 00:46:59.000000 rover-1.0.5/rover/retrieve_metadata.py
--rw-r--r--   0 chad       (502) staff       (20)     7172 2019-12-07 00:46:59.000000 rover-1.0.5/rover/scan.py
--rw-r--r--   0 chad       (502) staff       (20)     4533 2019-12-07 00:47:00.000000 rover-1.0.5/rover/sqlite.py
--rw-r--r--   0 chad       (502) staff       (20)    11092 2019-12-07 00:47:00.000000 rover-1.0.5/rover/subscribe.py
--rw-r--r--   0 chad       (502) staff       (20)     7464 2019-12-07 00:47:01.000000 rover-1.0.5/rover/summary.py
--rw-r--r--   0 chad       (502) staff       (20)    21905 2019-12-07 00:47:03.000000 rover-1.0.5/rover/utils.py
--rw-r--r--   0 chad       (502) staff       (20)     9359 2019-12-07 00:47:04.000000 rover-1.0.5/rover/web.py
--rw-r--r--   0 chad       (502) staff       (20)     3930 2019-12-07 00:47:05.000000 rover-1.0.5/rover/workers.py
-drwxr-xr-x   0 chad       (502) staff       (20)        0 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/
--rw-r--r--   0 chad       (502) staff       (20)     1403 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/PKG-INFO
--rw-r--r--   0 chad       (502) staff       (20)      804 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/SOURCES.txt
--rw-r--r--   0 chad       (502) staff       (20)        1 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/dependency_links.txt
--rw-r--r--   0 chad       (502) staff       (20)       38 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/entry_points.txt
--rw-r--r--   0 chad       (502) staff       (20)       68 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/requires.txt
--rw-r--r--   0 chad       (502) staff       (20)       12 2019-12-07 00:47:20.000000 rover-1.0.5/rover.egg-info/top_level.txt
--rw-r--r--   0 chad       (502) staff       (20)       38 2019-12-07 00:47:20.000000 rover-1.0.5/setup.cfg
--rw-r--r--   0 chad       (502) staff       (20)     1676 2019-12-07 00:47:08.000000 rover-1.0.5/setup.py
-drwxr-xr-x   0 chad       (502) staff       (20)        0 2019-12-07 00:47:20.000000 rover-1.0.5/tests/
--rw-r--r--   0 chad       (502) staff       (20)        0 2019-12-07 00:46:41.000000 rover-1.0.5/tests/__init__.py
--rw-r--r--   0 chad       (502) staff       (20)     4842 2019-12-07 00:47:06.000000 rover-1.0.5/tests/config.py
--rw-r--r--   0 chad       (502) staff       (20)     5898 2019-12-07 00:47:06.000000 rover-1.0.5/tests/coverage.py
--rw-r--r--   0 chad       (502) staff       (20)     1186 2019-12-07 00:47:06.000000 rover-1.0.5/tests/download.py
--rw-r--r--   0 chad       (502) staff       (20)     2423 2019-12-07 00:47:07.000000 rover-1.0.5/tests/index.py
--rw-r--r--   0 chad       (502) staff       (20)     1097 2019-12-07 00:47:07.000000 rover-1.0.5/tests/ingest.py
--rw-r--r--   0 chad       (502) staff       (20)     2474 2019-12-07 00:47:07.000000 rover-1.0.5/tests/logs.py
--rw-r--r--   0 chad       (502) staff       (20)     1500 2019-12-07 00:47:07.000000 rover-1.0.5/tests/retrieve.py
--rw-r--r--   0 chad       (502) staff       (20)     3391 2019-12-07 00:47:07.000000 rover-1.0.5/tests/test_utils.py
--rw-r--r--   0 chad       (502) staff       (20)     1442 2019-12-07 00:47:07.000000 rover-1.0.5/tests/utils.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.253178 rover-1.0.6/
+-rw-r--r--   0 chad       (501) staff       (20)    35213 2023-07-25 22:11:11.000000 rover-1.0.6/LICENSE
+-rw-r--r--   0 chad       (501) staff       (20)     1337 2023-07-25 22:11:30.252756 rover-1.0.6/PKG-INFO
+-rw-r--r--   0 chad       (501) staff       (20)      477 2023-07-25 22:11:11.000000 rover-1.0.6/README.md
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.244909 rover-1.0.6/rover/
+-rw-r--r--   0 chad       (501) staff       (20)        6 2023-07-25 22:11:03.000000 rover-1.0.6/rover/VERSION
+-rw-r--r--   0 chad       (501) staff       (20)     6242 2023-07-25 22:11:04.000000 rover-1.0.6/rover/__init__.py
+-rw-r--r--   0 chad       (501) staff       (20)      337 2023-07-25 22:11:04.000000 rover-1.0.6/rover/__main__.py
+-rw-r--r--   0 chad       (501) staff       (20)    30000 2023-07-25 22:11:05.000000 rover-1.0.6/rover/args.py
+-rw-r--r--   0 chad       (501) staff       (20)     6391 2023-07-25 22:11:05.000000 rover-1.0.6/rover/asdf.py
+-rw-r--r--   0 chad       (501) staff       (20)     9180 2023-07-25 22:11:05.000000 rover-1.0.6/rover/config.py
+-rw-r--r--   0 chad       (501) staff       (20)    11222 2023-07-25 22:11:06.000000 rover-1.0.6/rover/coverage.py
+-rw-r--r--   0 chad       (501) staff       (20)     8166 2023-07-25 22:11:06.000000 rover-1.0.6/rover/daemon.py
+-rw-r--r--   0 chad       (501) staff       (20)     6440 2023-07-25 22:11:06.000000 rover-1.0.6/rover/download.py
+-rw-r--r--   0 chad       (501) staff       (20)     9403 2023-07-25 22:11:06.000000 rover-1.0.6/rover/help.py
+-rw-r--r--   0 chad       (501) staff       (20)    13285 2023-07-25 22:11:06.000000 rover-1.0.6/rover/index.py
+-rw-r--r--   0 chad       (501) staff       (20)     7413 2023-07-25 22:11:07.000000 rover-1.0.6/rover/ingest.py
+-rw-r--r--   0 chad       (501) staff       (20)     5092 2023-07-25 22:11:07.000000 rover-1.0.6/rover/lock.py
+-rw-r--r--   0 chad       (501) staff       (20)     4354 2023-07-25 22:11:07.000000 rover-1.0.6/rover/logs.py
+-rw-r--r--   0 chad       (501) staff       (20)    41967 2023-07-25 22:11:08.000000 rover-1.0.6/rover/manager.py
+-rw-r--r--   0 chad       (501) staff       (20)     6435 2023-07-25 22:11:08.000000 rover-1.0.6/rover/process.py
+-rw-r--r--   0 chad       (501) staff       (20)     7379 2023-07-25 22:11:08.000000 rover-1.0.6/rover/report.py
+-rw-r--r--   0 chad       (501) staff       (20)     7407 2023-07-25 22:11:08.000000 rover-1.0.6/rover/request.py
+-rw-r--r--   0 chad       (501) staff       (20)     7980 2023-07-25 22:11:08.000000 rover-1.0.6/rover/retrieve.py
+-rw-r--r--   0 chad       (501) staff       (20)     8015 2023-07-25 22:11:09.000000 rover-1.0.6/rover/retrieve_metadata.py
+-rw-r--r--   0 chad       (501) staff       (20)     7172 2023-07-25 22:11:09.000000 rover-1.0.6/rover/scan.py
+-rw-r--r--   0 chad       (501) staff       (20)     4533 2023-07-25 22:11:09.000000 rover-1.0.6/rover/sqlite.py
+-rw-r--r--   0 chad       (501) staff       (20)    11092 2023-07-25 22:11:09.000000 rover-1.0.6/rover/subscribe.py
+-rw-r--r--   0 chad       (501) staff       (20)     7464 2023-07-25 22:11:09.000000 rover-1.0.6/rover/summary.py
+-rw-r--r--   0 chad       (501) staff       (20)    21905 2023-07-25 22:11:10.000000 rover-1.0.6/rover/utils.py
+-rw-r--r--   0 chad       (501) staff       (20)     9359 2023-07-25 22:11:10.000000 rover-1.0.6/rover/web.py
+-rw-r--r--   0 chad       (501) staff       (20)     3930 2023-07-25 22:11:10.000000 rover-1.0.6/rover/workers.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.247700 rover-1.0.6/rover.egg-info/
+-rw-r--r--   0 chad       (501) staff       (20)     1337 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/PKG-INFO
+-rw-r--r--   0 chad       (501) staff       (20)      812 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/SOURCES.txt
+-rw-r--r--   0 chad       (501) staff       (20)        1 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/dependency_links.txt
+-rw-r--r--   0 chad       (501) staff       (20)       37 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/entry_points.txt
+-rw-r--r--   0 chad       (501) staff       (20)       68 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/requires.txt
+-rw-r--r--   0 chad       (501) staff       (20)       12 2023-07-25 22:11:30.000000 rover-1.0.6/rover.egg-info/top_level.txt
+-rw-r--r--   0 chad       (501) staff       (20)       38 2023-07-25 22:11:30.253306 rover-1.0.6/setup.cfg
+-rw-r--r--   0 chad       (501) staff       (20)     1673 2023-07-25 22:11:11.000000 rover-1.0.6/setup.py
+drwxr-xr-x   0 chad       (501) staff       (20)        0 2023-07-25 22:11:30.252193 rover-1.0.6/tests/
+-rw-r--r--   0 chad       (501) staff       (20)        0 2023-07-25 22:11:03.000000 rover-1.0.6/tests/__init__.py
+-rw-r--r--   0 chad       (501) staff       (20)     4842 2023-07-25 22:11:10.000000 rover-1.0.6/tests/config.py
+-rw-r--r--   0 chad       (501) staff       (20)     5898 2023-07-25 22:11:11.000000 rover-1.0.6/tests/coverage.py
+-rw-r--r--   0 chad       (501) staff       (20)     1186 2023-07-25 22:11:11.000000 rover-1.0.6/tests/download.py
+-rw-r--r--   0 chad       (501) staff       (20)     2423 2023-07-25 22:11:11.000000 rover-1.0.6/tests/index.py
+-rw-r--r--   0 chad       (501) staff       (20)     1097 2023-07-25 22:11:11.000000 rover-1.0.6/tests/ingest.py
+-rw-r--r--   0 chad       (501) staff       (20)     2474 2023-07-25 22:11:11.000000 rover-1.0.6/tests/logs.py
+-rw-r--r--   0 chad       (501) staff       (20)     1500 2023-07-25 22:11:11.000000 rover-1.0.6/tests/retrieve.py
+-rw-r--r--   0 chad       (501) staff       (20)     3391 2023-07-25 22:11:11.000000 rover-1.0.6/tests/test_utils.py
+-rw-r--r--   0 chad       (501) staff       (20)     1442 2023-07-25 22:11:11.000000 rover-1.0.6/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rover-1.0.5/PKG-INFO` & `rover-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: rover
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for the robust retrieval of seismic data
-Home-page: https://iris-edu.github.io/rover
-Author: IRIS
-Author-email: software-owner@iris.washington.edu
-License: UNKNOWN
-Description: # rover 
-        
-        Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](http://service.iris.edu/irisws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
-        
-        For more installation instructions and quick start see the [User Guide](https://iris-edu.github.io/rover/).
-        
-Platform: UNKNOWN
+Home-page: https://earthscope.github.io/rover
+Author: EarthScope
+Author-email: software@earthscope.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mseedindex
+License-File: LICENSE
+
+# rover 
+
+Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](https://service.iris.edu/fdsnws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
+
+For more installation instructions and quick start see the [User Guide](https://earthscope.github.io/rover/).
```

### Comparing `rover-1.0.5/rover/__init__.py` & `rover-1.0.6/rover/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import open
 from builtins import dict
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 pkg_path = __file__
```

### Comparing `rover-1.0.5/rover/args.py` & `rover-1.0.6/rover/args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import open
 from builtins import super
 from builtins import str
 from builtins import object
 from future import standard_library
 standard_library.install_aliases()
```

### Comparing `rover-1.0.5/rover/asdf.py` & `rover-1.0.6/rover/asdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 from future import standard_library
 standard_library.install_aliases()
 import os
 from .args import FORCE_METADATA_RELOAD, UserFeedback, \
     fail_early
 from .config import asdf_container, timeseries_db
 from .utils import safe_unlink
```

### Comparing `rover-1.0.5/rover/config.py` & `rover-1.0.6/rover/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import open
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from argparse import Namespace
```

### Comparing `rover-1.0.5/rover/coverage.py` & `rover-1.0.6/rover/coverage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import division
-from __future__ import unicode_literals
-from __future__ import print_function
 from __future__ import absolute_import
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import map
 from builtins import next
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
```

### Comparing `rover-1.0.5/rover/daemon.py` & `rover-1.0.6/rover/daemon.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from sqlite3 import OperationalError
 from time import sleep, time
```

### Comparing `rover-1.0.5/rover/download.py` & `rover-1.0.6/rover/download.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 import os
 import json
 import sys
```

### Comparing `rover-1.0.5/rover/help.py` & `rover-1.0.6/rover/help.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from re import sub
```

### Comparing `rover-1.0.5/rover/index.py` & `rover-1.0.6/rover/index.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import int
 from future import standard_library
 standard_library.install_aliases()
 import sys
 from re import match, sub
 from sqlite3 import OperationalError
```

### Comparing `rover-1.0.5/rover/ingest.py` & `rover-1.0.6/rover/ingest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 from builtins import open
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 from datetime import datetime
 from os import getpid
 from os.path import exists, join
```

### Comparing `rover-1.0.5/rover/lock.py` & `rover-1.0.6/rover/lock.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 from os import getpid
 from sqlite3 import OperationalError, IntegrityError
 from time import sleep
```

### Comparing `rover-1.0.5/rover/logs.py` & `rover-1.0.6/rover/logs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 import sys
 from io import StringIO
 from logging import getLogger, StreamHandler, Formatter, DEBUG, addLevelName
 from logging.handlers import RotatingFileHandler
```

### Comparing `rover-1.0.5/rover/manager.py` & `rover-1.0.6/rover/manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import division
 from __future__ import print_function
-from __future__ import unicode_literals
 from __future__ import absolute_import
+from __future__ import unicode_literals
 from builtins import super
 from builtins import next
 from builtins import map
 from builtins import open
 from builtins import str
 from builtins import int
 from future import standard_library
```

### Comparing `rover-1.0.5/rover/process.py` & `rover-1.0.6/rover/process.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import next
 from future import standard_library
 standard_library.install_aliases()
 from os import getpid, kill
```

### Comparing `rover-1.0.5/rover/report.py` & `rover-1.0.6/rover/report.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import division
-from __future__ import unicode_literals
-from __future__ import print_function
 from __future__ import absolute_import
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from os import getpid
 from socket import gethostname
 from sys import version_info
```

### Comparing `rover-1.0.5/rover/request.py` & `rover-1.0.6/rover/request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import open
 from builtins import range
 from builtins import zip
 from builtins import next
 from builtins import map
 from future import standard_library
```

### Comparing `rover-1.0.5/rover/retrieve.py` & `rover-1.0.6/rover/retrieve.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 import datetime
 from shutil import copyfile
```

### Comparing `rover-1.0.5/rover/retrieve_metadata.py` & `rover-1.0.6/rover/retrieve_metadata.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 from builtins import open
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 import os
 import shutil
 from collections import namedtuple
```

### Comparing `rover-1.0.5/rover/scan.py` & `rover-1.0.6/rover/scan.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import next
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from genericpath import isdir
```

### Comparing `rover-1.0.5/rover/sqlite.py` & `rover-1.0.6/rover/sqlite.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import object
 from future import standard_library
 standard_library.install_aliases()
 from sqlite3 import connect
```

### Comparing `rover-1.0.5/rover/subscribe.py` & `rover-1.0.6/rover/subscribe.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import range
 from builtins import int
 from builtins import map
 from future import standard_library
 standard_library.install_aliases()
```

### Comparing `rover-1.0.5/rover/summary.py` & `rover-1.0.6/rover/summary.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 import sys
 from re import match, sub
 from sqlite3 import OperationalError
```

### Comparing `rover-1.0.5/rover/utils.py` & `rover-1.0.6/rover/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 from builtins import open
 from builtins import next
 from builtins import map
 from builtins import int
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
```

### Comparing `rover-1.0.5/rover/web.py` & `rover-1.0.6/rover/web.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import division
-from __future__ import unicode_literals
-from __future__ import print_function
 from __future__ import absolute_import
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import int
 from builtins import object
 from future import standard_library
 standard_library.install_aliases()
 import os
```

### Comparing `rover-1.0.5/rover/workers.py` & `rover-1.0.6/rover/workers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 from builtins import open
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 import json
 import os
```

### Comparing `rover-1.0.5/rover.egg-info/PKG-INFO` & `rover-1.0.6/rover.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: rover
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for the robust retrieval of seismic data
-Home-page: https://iris-edu.github.io/rover
-Author: IRIS
-Author-email: software-owner@iris.washington.edu
-License: UNKNOWN
-Description: # rover 
-        
-        Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](http://service.iris.edu/irisws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
-        
-        For more installation instructions and quick start see the [User Guide](https://iris-edu.github.io/rover/).
-        
-Platform: UNKNOWN
+Home-page: https://earthscope.github.io/rover
+Author: EarthScope
+Author-email: software@earthscope.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mseedindex
+License-File: LICENSE
+
+# rover 
+
+Tool for the robust retrieval of seismic (and other) data from a data center such as the [IRIS DMC](https://ds.iris.edu).  For this tool to work the data center must offer both a [irisws-availability](https://service.iris.edu/fdsnws/availability/1/) (or compatible) service and an [fdsnws-dataselect](http://service.iris.edu/fdsnws/dataselect/1/) service.
+
+For more installation instructions and quick start see the [User Guide](https://earthscope.github.io/rover/).
```

### Comparing `rover-1.0.5/rover.egg-info/SOURCES.txt` & `rover-1.0.6/rover.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 rover/VERSION
 rover/__init__.py
 rover/__main__.py
 rover/args.py
 rover/asdf.py
```

### Comparing `rover-1.0.5/setup.py` & `rover-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 with open(os.path.join(here, module_name, 'VERSION')) as vf:
     version = vf.read().strip()
 
 setup(
     name=module_name,
     version=version,
-    author="IRIS",
-    author_email="software-owner@iris.washington.edu",
+    author="EarthScope",
+    author_email="software@earthscope.org",
     description="Tool for the robust retrieval of seismic data",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://iris-edu.github.io/rover",
+    url="https://earthscope.github.io/rover",
     packages=find_packages(),
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
     classifiers=(
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `rover-1.0.5/tests/config.py` & `rover-1.0.6/tests/config.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 
 from builtins import open
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from os.path import join, dirname
```

### Comparing `rover-1.0.5/tests/coverage.py` & `rover-1.0.6/tests/coverage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import print_function
-from __future__ import unicode_literals
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import unicode_literals
 from builtins import range
 from builtins import map
 from future import standard_library
 standard_library.install_aliases()
 from random import randint, seed
 from sys import version_info
```

### Comparing `rover-1.0.5/tests/download.py` & `rover-1.0.6/tests/download.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 from sys import version_info
 from os.path import join
 
 from rover.args import DATADIR
```

### Comparing `rover-1.0.5/tests/index.py` & `rover-1.0.6/tests/index.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import int
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 from sys import version_info
 if version_info[0] >= 3:
```

### Comparing `rover-1.0.5/tests/ingest.py` & `rover-1.0.6/tests/ingest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 from sys import version_info
 from os.path import join
 
 from rover.args import DATADIR
```

### Comparing `rover-1.0.5/tests/logs.py` & `rover-1.0.6/tests/logs.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import open
 from future import standard_library
 standard_library.install_aliases()
 from io import StringIO
 from os.path import join
 from re import sub
```

### Comparing `rover-1.0.5/tests/retrieve.py` & `rover-1.0.6/tests/retrieve.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 from sys import version_info
 
 from rover import ProcessManager
```

### Comparing `rover-1.0.5/tests/test_utils.py` & `rover-1.0.6/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from builtins import super
 from builtins import dict
 from future import standard_library
 standard_library.install_aliases()
 from builtins import object
 from fnmatch import fnmatch
```

### Comparing `rover-1.0.5/tests/utils.py` & `rover-1.0.6/tests/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
 
 from future import standard_library
 standard_library.install_aliases()
 from os.path import join, exists
 from sys import version_info
 
 if version_info[0] >= 3:
```

