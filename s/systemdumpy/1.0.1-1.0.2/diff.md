# Comparing `tmp/systemdumpy-1.0.1.tar.gz` & `tmp/systemdumpy-1.0.2.tar.gz`

## Comparing `systemdumpy-1.0.1.tar` & `systemdumpy-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/requirements.txt
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/systemdumpy/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/systemdumpy/modules/__init__.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/systemdumpy/modules/report.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/systemdumpy/modules/web.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/LICENSE
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 systemdumpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/__init__.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/report.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/systemdumpy/modules/web.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 systemdumpy-1.0.2/PKG-INFO
```

### Comparing `systemdumpy-1.0.1/systemdumpy/__main__.py` & `systemdumpy-1.0.2/systemdumpy/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 ERROR_FILE_NOT_EXIST = 4
 ERROR_CREATING_REPORT = 5
 ERROR_EXTRACTING_LOGS = 6
 ERROR_UNEXPECTED = 99
 
 
 def parseCommandLine():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser( prog = 'systemdumpy', description= 'create and load a system dump for B&R PLC')
     parser.add_argument("target", help="remote PLC IP address or name or systemdump file (*.targ.gz)" )    
     parser.add_argument("-c", "--create", help="create a dump on (remote) target", action="store_true")
     parser.add_argument("-n", "--nofiles", help="don't include data files (logger, NCT etc.)", action="store_true")
     parser.add_argument("-u", "--upload", help="upload from (remote) target and store to file", action="store_true")
     parser.add_argument("-d", "--delete", help="delete dump from target", action="store_true")
     parser.add_argument("-p", "--prefix", help="prepend this PREFIX for system dump filename after upload", default = "" )
     parser.add_argument("-i", "--inventory", help="create a hardware inventory list (*.xlsx)", action="store_true")
-    parser.add_argument("-l", "--loggers", help="extract loggers to *.csv", action="store_true")
     parser.add_argument("-v", "--verbose", help="show messages", action="store_true")
-    parser.add_argument('--version', action='version', version='%(prog)s 1.0   (https://github.com/hilch/systemdump.py)')
+    parser.add_argument('--version', action='version', version='%(prog)s 1.0.2   (https://github.com/hilch/systemdump.py)')
 
     try:
         args = parser.parse_args()
 
         return args
 
     except argparse.ArgumentError:
@@ -106,19 +105,19 @@
                     return ERROR_CREATING_REPORT
 
         if args.loggers:
             if target_is_remote: # target is remote
                 if dumpfilename != "":
                     if args.verbose:
                             print(f"extract loggers from uploaded file: {dumpfilename}")                      
-                    ret = datafiles.extractLoggerFiles(dumpfilename )        
+       
             else: # target is a file
                 if args.verbose:
                     print(f"extract loggers from: {args.target}")               
-                ret = datafiles.extractLoggerFiles(args.target)
+
                 if ret['result'] != 'Ok':
                     return ERROR_EXTRACTING_LOGS                    
 
         if args.delete:
             if target_is_remote: # target is remote
                 ret = web.deleteFromTarget(args.target)
                 if args.verbose:
@@ -138,17 +137,17 @@
     except:
          exception = sys.exc_info()[0]
          print( f'Unexpected error (remote): {exception}' )
          return ERROR_UNEXPECTED
 
 
 # we start here
+if __name__ == '__main__':
+    args = parseCommandLine()
+    if args == None:
+        result = ERROR_UNEXPECTED
+    else:
+        result = executeCommands(args)
 
-args = parseCommandLine()
-if args == None:
-    result = ERROR_UNEXPECTED
-else:
-    result = executeCommands(args)
-
-sys.exit(result)
+    sys.exit(result)
```

### Comparing `systemdumpy-1.0.1/systemdumpy/modules/report.py` & `systemdumpy-1.0.2/systemdumpy/modules/report.py`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.1/systemdumpy/modules/web.py` & `systemdumpy-1.0.2/systemdumpy/modules/web.py`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.1/.gitignore` & `systemdumpy-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.1/LICENSE` & `systemdumpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.1/README.md` & `systemdumpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `systemdumpy-1.0.1/pyproject.toml` & `systemdumpy-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "systemdumpy"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Christoph Hilchenbach" },
 ]
 description = "create and load a system dump for B&R PLC from the command line"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `systemdumpy-1.0.1/PKG-INFO` & `systemdumpy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemdumpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: create and load a system dump for B&R PLC from the command line
 Project-URL: Homepage, https://github.com/hilch/systemdump.py
 Project-URL: Bug Tracker, https://github.com/hilch/systemdump.py/issues
 Author: Christoph Hilchenbach
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

