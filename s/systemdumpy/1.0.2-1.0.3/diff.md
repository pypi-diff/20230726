# Comparing `tmp/systemdumpy-1.0.2.tar.gz` & `tmp/systemdumpy-1.0.3.tar.gz`

## Comparing `systemdumpy-1.0.2.tar` & `systemdumpy-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/requirements.txt
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/__init__.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/report.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/web.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/LICENSE
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/whatsnew.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/__about__.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/__main__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/BrDataObjectFile.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/BrFile.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/BrLoggerFile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/datafiles.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/report.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/systemdumpy/modules/web.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 systemdumpy-1.0.3/PKG-INFO
```

### Comparing `systemdumpy-1.0.2/systemdumpy/__main__.py` & `systemdumpy-1.0.3/systemdumpy/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import argparse
 import sys
 import os
 import re
 from systemdumpy.modules import web
 from systemdumpy.modules import report
+from systemdumpy.__about__ import __version__
 
 
 ERROR_OK = 0
 ERROR_CREATING_DUMP = 1
 ERROR_UPLOADING_DUMP = 2
 ERROR_DELETING_DUMP = 3
 ERROR_FILE_NOT_EXIST = 4
@@ -28,15 +29,15 @@
     parser.add_argument("-c", "--create", help="create a dump on (remote) target", action="store_true")
     parser.add_argument("-n", "--nofiles", help="don't include data files (logger, NCT etc.)", action="store_true")
     parser.add_argument("-u", "--upload", help="upload from (remote) target and store to file", action="store_true")
     parser.add_argument("-d", "--delete", help="delete dump from target", action="store_true")
     parser.add_argument("-p", "--prefix", help="prepend this PREFIX for system dump filename after upload", default = "" )
     parser.add_argument("-i", "--inventory", help="create a hardware inventory list (*.xlsx)", action="store_true")
     parser.add_argument("-v", "--verbose", help="show messages", action="store_true")
-    parser.add_argument('--version', action='version', version='%(prog)s 1.0.2   (https://github.com/hilch/systemdump.py)')
+    parser.add_argument('--version', action='version', version= f'%(prog)s {__version__}   (https://github.com/hilch/systemdump.py)')
 
     try:
         args = parser.parse_args()
 
         return args
 
     except argparse.ArgumentError:
@@ -99,27 +100,15 @@
                     ret = report.report(dumpfilename, ('inventory') )        
             else: # target is a file
                 if args.verbose:
                     print(f"create an inventory list from: {args.target}")               
                 ret = report.report(args.target, ('inventory'))
                 if ret['result'] != 'Ok':
                     return ERROR_CREATING_REPORT
-
-        if args.loggers:
-            if target_is_remote: # target is remote
-                if dumpfilename != "":
-                    if args.verbose:
-                            print(f"extract loggers from uploaded file: {dumpfilename}")                      
-       
-            else: # target is a file
-                if args.verbose:
-                    print(f"extract loggers from: {args.target}")               
-
-                if ret['result'] != 'Ok':
-                    return ERROR_EXTRACTING_LOGS                    
+                           
 
         if args.delete:
             if target_is_remote: # target is remote
                 ret = web.deleteFromTarget(args.target)
                 if args.verbose:
                     print(f"delete systemdump from {args.target}")     
                 if ret['result'] != 'Ok':
```

### Comparing `systemdumpy-1.0.2/systemdumpy/modules/report.py` & `systemdumpy-1.0.3/systemdumpy/modules/report.py`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.2/systemdumpy/modules/web.py` & `systemdumpy-1.0.3/systemdumpy/modules/web.py`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.2/.gitignore` & `systemdumpy-1.0.3/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -124,7 +124,10 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .vscode
+
+# system dump files
+*.gz
```

### Comparing `systemdumpy-1.0.2/LICENSE` & `systemdumpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.2/README.md` & `systemdumpy-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,46 +13,44 @@
 So I wrote this Python script to automate this work with e.g. a batchfile.
 
 
 # Installation
 install Python from web page [https://www.python.org/](https://www.python.org/). I used the 3.9.6.
 
 ```
-python -m pip install systemdumpy
+py -m pip install systemdumpy
 ```
 
 
 # Examples
 
 ## create a dump and store it
 ```
-python -m systemdumpy 192.168.0.100 -cuv -p MyCPU_
+py -m systemdumpy 192.168.0.100 -cuv -p MyCPU_
 
 create a systemdump on 192.168.0.100
 upload systemdump from 192.168.0.100
 saving MyCPU_BuR_SDM_Sysdump_2021-07-09_11-51-55.tar.gz (2820986) bytes
 ```
 
 ## delete the last systemdump from PLC
 ```
-python -m systemdumpy 192.168.0.100 -dv
+py -m systemdumpy 192.168.0.100 -dv
 ```
 
 ## create a inventory list (*xlsx) from file
 ```
-python -m systemdumpy BuR_SDM_Sysdump_2021-07-09_17-43-05.tar.gz -iv
+py -m systemdumpy BuR_SDM_Sysdump_2021-07-09_17-43-05.tar.gz -iv
 ```
 
 
-
-
 # usage
 
 ```
-usage: systemdumppy [-h] [-c] [-n] [-u] [-d] [-p PREFIX] [-i] [-v] [--version] target
+usage: systemdumpy [-h] [-c] [-n] [-u] [-d] [-p PREFIX] [-i] [-v] [--version] target
 
 positional arguments:
   target                remote PLC IP address or name or systemdump file (*.targ.gz)
 
 optional arguments:
   -h, --help            show this help message and exit
   -c, --create          create a dump on (remote) target
```

### Comparing `systemdumpy-1.0.2/pyproject.toml` & `systemdumpy-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "systemdumpy"
-version = "1.0.2"
+dynamic = ["version"]
 authors = [
   { name="Christoph Hilchenbach" },
 ]
 description = "create and load a system dump for B&R PLC from the command line"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -17,14 +17,17 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	"openpyxl >=3.1.2",
 	"requests >=2.31.0"
 ]
 
+[tool.hatch.version]
+path = "systemdumpy/__about__.py"
+
 [tool.hatch.build.targets.wheel]
 only-include = ["systemdumpy"]
 require-runtime-dependencies = true
 
 
 
 [project.urls]
```

### Comparing `systemdumpy-1.0.2/PKG-INFO` & `systemdumpy-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemdumpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: create and load a system dump for B&R PLC from the command line
 Project-URL: Homepage, https://github.com/hilch/systemdump.py
 Project-URL: Bug Tracker, https://github.com/hilch/systemdump.py/issues
 Author: Christoph Hilchenbach
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,46 +29,44 @@
 So I wrote this Python script to automate this work with e.g. a batchfile.
 
 
 # Installation
 install Python from web page [https://www.python.org/](https://www.python.org/). I used the 3.9.6.
 
 ```
-python -m pip install systemdumpy
+py -m pip install systemdumpy
 ```
 
 
 # Examples
 
 ## create a dump and store it
 ```
-python -m systemdumpy 192.168.0.100 -cuv -p MyCPU_
+py -m systemdumpy 192.168.0.100 -cuv -p MyCPU_
 
 create a systemdump on 192.168.0.100
 upload systemdump from 192.168.0.100
 saving MyCPU_BuR_SDM_Sysdump_2021-07-09_11-51-55.tar.gz (2820986) bytes
 ```
 
 ## delete the last systemdump from PLC
 ```
-python -m systemdumpy 192.168.0.100 -dv
+py -m systemdumpy 192.168.0.100 -dv
 ```
 
 ## create a inventory list (*xlsx) from file
 ```
-python -m systemdumpy BuR_SDM_Sysdump_2021-07-09_17-43-05.tar.gz -iv
+py -m systemdumpy BuR_SDM_Sysdump_2021-07-09_17-43-05.tar.gz -iv
 ```
 
 
-
-
 # usage
 
 ```
-usage: systemdumppy [-h] [-c] [-n] [-u] [-d] [-p PREFIX] [-i] [-v] [--version] target
+usage: systemdumpy [-h] [-c] [-n] [-u] [-d] [-p PREFIX] [-i] [-v] [--version] target
 
 positional arguments:
   target                remote PLC IP address or name or systemdump file (*.targ.gz)
 
 optional arguments:
   -h, --help            show this help message and exit
   -c, --create          create a dump on (remote) target
```

