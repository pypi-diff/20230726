# Comparing `tmp/tstl-1.2.8-py3-none-any.whl.zip` & `tmp/tstl-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,32 @@
-Zip file size: 119102 bytes, number of entries: 27
+Zip file size: 123685 bytes, number of entries: 30
 -rw-r--r--  2.0 unx        0 b- defN 16-Dec-24 02:26 src/__init__.py
 -rw-r--r--  2.0 unx     1447 b- defN 17-Dec-08 21:35 src/analyzeprovenance.py
 -rw-r--r--  2.0 unx     3851 b- defN 17-Dec-08 21:35 src/exhaust.py
+-rw-r--r--  2.0 unx      820 b- defN 18-Apr-08 17:34 src/fromafl.py
 -rw-r--r--  2.0 unx     5193 b- defN 17-Dec-30 22:58 src/generalize.py
 -rw-r--r--  2.0 unx     6262 b- defN 17-Dec-30 22:58 src/graph.py
--rw-r--r--  2.0 unx    71500 b- defN 18-Apr-08 04:48 src/harnessmaker.py
+-rw-r--r--  2.0 unx    71572 b- defN 18-Apr-08 17:40 src/harnessmaker.py
+-rw-r--r--  2.0 unx     2606 b- defN 18-Apr-08 18:16 src/makecorpus.py
 -rw-r--r--  2.0 unx     2216 b- defN 17-Dec-30 22:58 src/markov.py
 -rw-r--r--  2.0 unx     1883 b- defN 17-Dec-08 21:35 src/provenance.py
 -rw-r--r--  2.0 unx    81725 b- defN 18-Apr-03 20:26 src/randomtester.py
--rw-r--r--  2.0 unx    13153 b- defN 18-Apr-05 03:21 src/reduce.py
--rw-r--r--  2.0 unx     6116 b- defN 18-Mar-23 06:59 src/replay.py
--rw-r--r--  2.0 unx     4226 b- defN 18-Apr-07 03:10 src/runregressions.py
--rw-r--r--  2.0 unx     5410 b- defN 17-Dec-30 23:00 src/standalone.py
--rw-r--r--  2.0 unx     1930 b- defN 18-Apr-08 04:33 src/tstl_afl.py
--rw-r--r--  2.0 unx    73277 b- defN 18-Apr-05 03:15 src/static/boilerplate.py
+-rw-r--r--  2.0 unx    13593 b- defN 18-Apr-08 17:44 src/reduce.py
+-rw-r--r--  2.0 unx     6509 b- defN 18-Apr-08 18:14 src/replay.py
+-rw-r--r--  2.0 unx     4567 b- defN 18-Apr-08 18:01 src/runregressions.py
+-rw-r--r--  2.0 unx     5631 b- defN 18-Apr-08 18:01 src/standalone.py
+-rw-r--r--  2.0 unx      689 b- defN 18-Apr-08 17:14 src/tocorpus.py
+-rw-r--r--  2.0 unx     2406 b- defN 18-Apr-08 18:21 src/tstl_afl.py
+-rw-r--r--  2.0 unx    74629 b- defN 18-Apr-08 18:15 src/static/boilerplate.py
 -rw-r--r--  2.0 unx     4481 b- defN 16-Dec-24 02:26 src/static/boilerplate.py~
 -rw-r--r--  2.0 unx     9645 b- defN 17-Dec-08 21:46 src/static/boilerplate_cov.py
 -rw-r--r--  2.0 unx      532 b- defN 16-Dec-24 02:26 src/static/countfsize.py
 -rw-r--r--  2.0 unx    59190 b- defN 17-May-01 08:55 src/static/oldboiler
 -rw-r--r--  2.0 unx    65438 b- defN 17-Sep-17 22:51 src/static/oldboiler.py
--rw-r--r--  2.0 unx    33673 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      390 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1388 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/metadata.json
--rw-r--r--  2.0 unx        4 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx    34115 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx     2109 b- defN 18-Apr-08 04:49 tstl-1.2.8.dist-info/RECORD
-27 files, 489246 bytes uncompressed, 115830 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx    35580 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      502 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1612 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/metadata.json
+-rw-r--r--  2.0 unx        4 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx    36022 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx     2327 b- defN 18-Apr-08 18:25 tstl-1.2.9.dist-info/RECORD
+30 files, 501024 bytes uncompressed, 120093 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -3,23 +3,29 @@
 
 Filename: src/analyzeprovenance.py
 Comment: 
 
 Filename: src/exhaust.py
 Comment: 
 
+Filename: src/fromafl.py
+Comment: 
+
 Filename: src/generalize.py
 Comment: 
 
 Filename: src/graph.py
 Comment: 
 
 Filename: src/harnessmaker.py
 Comment: 
 
+Filename: src/makecorpus.py
+Comment: 
+
 Filename: src/markov.py
 Comment: 
 
 Filename: src/provenance.py
 Comment: 
 
 Filename: src/randomtester.py
@@ -33,14 +39,17 @@
 
 Filename: src/runregressions.py
 Comment: 
 
 Filename: src/standalone.py
 Comment: 
 
+Filename: src/tocorpus.py
+Comment: 
+
 Filename: src/tstl_afl.py
 Comment: 
 
 Filename: src/static/boilerplate.py
 Comment: 
 
 Filename: src/static/boilerplate.py~
@@ -54,29 +63,29 @@
 
 Filename: src/static/oldboiler
 Comment: 
 
 Filename: src/static/oldboiler.py
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/DESCRIPTION.rst
+Filename: tstl-1.2.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/entry_points.txt
+Filename: tstl-1.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/metadata.json
+Filename: tstl-1.2.9.dist-info/metadata.json
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/top_level.txt
+Filename: tstl-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/WHEEL
+Filename: tstl-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/METADATA
+Filename: tstl-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: tstl-1.2.8.dist-info/RECORD
+Filename: tstl-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/harnessmaker.py

```diff
@@ -384,15 +384,15 @@
     global poolPrefix
     global genCode
     global originalCode
 
     baseIndent = "    "
 
     if "-v" in sys.argv or "--version" in sys.argv:
-        print("TSTL, version 1.2.8")
+        print("TSTL, version 1.2.9")
         print("Documentation at https://github.com/agroce/tstl")
         sys.exit(0)
         
 
     
     parsed_args, parser = parse_args()
     config = make_config(parsed_args, parser)
@@ -416,15 +416,17 @@
     outf.write("import copy\n")
     outf.write("import traceback\n")
     outf.write("import inspect\n")    
     outf.write("import re\n")
     outf.write("import sys\n")
     outf.write("import time\n")
     outf.write("import glob\n")
-    outf.write("import subprocess\n")    
+    outf.write("import struct\n")
+    outf.write("import random\n")        
+    outf.write("import subprocess\n")
     outf.write("import os.path\n")        
     outf.write("from itertools import chain, combinations\n")    
 
     if not config.noCover:
         outf.write("import coverage\n")
 
     outf.write("# BEGIN STANDALONE CODE\n")
```

## src/reduce.py

```diff
@@ -76,15 +76,21 @@
     parser.add_argument('--verbose', type=str, default=None,
                         help='Level of verbosity for reduction.')
     parser.add_argument('--sandbox', action='store_true',
                         help="Use sandbox reduction.")
     parser.add_argument('--quietSandbox', action='store_true',
                         help="Run sandbox in a quieter mode.")
     parser.add_argument('--timeout', type=int, default=None,
-                        help='Timeout for sandbox reductions (only works on unix-like systems).')    
+                        help='Timeout for sandbox reductions (only works on unix-like systems).')
+    parser.add_argument('--afl', action='store_true',
+                        help="Read in tests in afl format.")
+    parser.add_argument('--aflswarm', action='store_true',
+                        help="afl tests are in swarm format.")    
+    parser.add_argument('--aflwrite', action='store_true',
+                        help="Write out tests in afl format.")    
     
     parsed_args = parser.parse_args(sys.argv[1:])
     return (parsed_args, parser)
 
 def make_config(pargs, parser):
     """
     Process the raw arguments, returning a namedtuple object holding the
@@ -151,15 +157,15 @@
     R = None
     if config.random:
         R = random.Random()
 
         if config.seed != None:
             R.seed(config.seed)
     
-    r = sut.loadTest(config.infile)
+    r = sut.loadTest(config.infile,afl=config.afl,swarm=config.aflswarm)
 
     f = None
     
     if config.matchException:
         print("EXECUTING TEST TO OBTAIN FAILURE FOR EXCEPTION MATCHING...")
         assert (sut.fails(r))
         f = sut.failure()
@@ -259,23 +265,23 @@
             rs = newrs
         print("NORMALIZED IN",time.time()-start,"SECONDS")
         if (not config.multiple) and (not config.decompose):
             print("NEW LENGTH",len(r))
         else:
             print("NEW LENGTHS",list(map(len,rs)))
     if (not config.multiple) and (not config.decompose):
-        sut.saveTest(r,config.outfile)
+        sut.saveTest(r,config.outfile,afl=config.writeafl)
         sut.prettyPrintTest(r)
         print()
         print("TEST WRITTEN TO",config.outfile)     
     else:
         i = 0
         for r in rs:
             print("TEST #"+str(i)+":")
-            sut.saveTest(r,config.outfile+"."+str(i)+".test")
+            sut.saveTest(r,config.outfile+"."+str(i)+".test",afl=config.writeafl)
             sut.prettyPrintTest(r)
             print()
             print("TEST WRITTEN TO",config.outfile+"."+str(i))
             print()
             i += 1
```

## src/replay.py

```diff
@@ -36,26 +36,28 @@
     print('Call to %s on line %s of %s' % (func_name, line_no, filename))
     sys.stdout.flush()    
     return trace_lines
     
 def main():
 
     if "--help" in sys.argv:
-        print("Usage:  tstl_replay <test file> [--noCheck] [--logging loglevel] [--verbose] [--showActions] [--coverage] [--internal] [--html directory] [--delay secs] [--trace]")
+        print("Usage:  tstl_replay <test file> [--noCheck] [--logging loglevel] [--verbose] [--showActions] [--coverage] [--internal] [--html directory] [--delay secs] [--trace] [--afl] [--aflswarm]")
         print("Options:")
         print("--noCheck:      do not run property checks")
         print("--logging:      set the logging level for the test")
         print("--verbose:      run with verbose action output")
         print("--hideOpaque:   hide opaque values in verbose actions")
         print("--showActions:  show all actions")        
         print("--coverage:     report code coverage")        
         print("--internal:     report detailed code coverage information")
         print("--html:         produce HTML report on coverage")
         print("--delay:        delay to inject between steps")        
         print("--trace:        trace lines executed (does not work with SUTs compiled with coverage)")
+        print("--afl:          test is in afl format")
+        print("--aflswarm:     test is in afl swarm format")                
         sys.exit(0)
 
     sut = SUT.sut()
         
     if not (("--coverage" in sys.argv) or ("--internal" in sys.argv)):
         try:
             sut.stopCoverage()
@@ -114,15 +116,21 @@
     if logLevel != None:
         sut.setLog(logLevel)
     i = 0
     if verbose:
         sut.verbose(True)
     if "--hideOpaque" in sys.argv:
         sut.verboseOpaque(False)
-    for l in open(file):
+    if not "--afl" in sys.argv:
+        with open(file,'r') as f:
+            theTest = f.readlines()
+    else:
+        readTest = sut.loadTest(file,afl=True,swarm=("--aflswarm" in sys.argv))
+        theTest = map(lambda x:x[0]+"\n",readTest)
+    for l in theTest:
         name = l[:-1]
         if name == "<<RESTART>>":
             if "--showActions" in sys.argv:
                 print("<<RESTART>>")
             #print "RESTART"
             rout.write("<<RESTART>>\n")
             rout.flush()
```

## src/runregressions.py

```diff
@@ -11,30 +11,34 @@
 
 if not "--help" in sys.argv:
     import sut as SUT
 
 def main():
     
     if "--help" in sys.argv:
-        print("Usage:  tstl_regress <test files> [--noCheck] [--html dir] [--noCover] [--verbose] [--running]")
+        print("Usage:  tstl_regress <test files> [--noCheck] [--html dir] [--noCover] [--verbose] [--running] [--afl] [--aflswarm]")
         print("Options:")
         print(" --noCheck:      do not run property checks")
         print(" --html:         output an HTML coverage report to the chosen directory")
         print(" --noCover:      do not compute code coverage")
         print(" --verbose:      make actions verbose")
         print(" --running:      give a running report on code coverage")
         print(" --keepGoing:    don't stop on failed test")
+        print(" --afl:          tests are in afl format")
+        print(" --aflswarm:          tests are in afl swarm format")                
         sys.exit(0)
     
     sut = SUT.sut()
 
     nocover = False
     verbose = False
     running = False
     keepGoing = False
+    afl = False
+    aflswarm = False
     ignoreProps = False
     lastWasHtml = False
     files = []
     htmlOut = None
     for f in sys.argv[1:]:
         if lastWasHtml:
             htmlOut = f
@@ -56,14 +60,18 @@
         verbose = True
     if "--noCheck" in sys.argv:
         ignoreProps = True
     if "--running" in sys.argv:
         running = True
     if "--keepGoing" in sys.argv:
         keepGoing = True
+    if "--afl" in sys.argv:
+       afl = True
+    if "--aflswarm" in sys.argv:
+       aflswarm = True               
 
     if verbose:
         sut.verbose(True)
 
     failedTests = []
     anyFailed = False
 
@@ -74,15 +82,15 @@
     invalidTests = []
     
     stime = time.time()
     for f in files:
         totalTests += 1
         print("RUNNING TEST",f)
         try:
-            t = sut.loadTest(f)
+            t = sut.loadTest(f,afl=afl,swarm=aflswarm)
         except KeyError:
             print("INVALID TEST, SKIPPING...")
             invalidTests.append(f)
             continue
         ok = False
         try:
             ok = sut.replay(t, checkProp=(not ignoreProps))
```

## src/standalone.py

```diff
@@ -10,34 +10,38 @@
 
 if not "--help" in sys.argv:
     import sut as SUT
 
 def main():
 
     if "--help" in sys.argv:
-        print("Usage:  tstl_standalone <test file> <output Python file> [<sut file>] [--noCheck] [--noRefs] [--regression] [--verbose]")
+        print("Usage:  tstl_standalone <test file> <output Python file> [<sut file>] [--noCheck] [--noRefs] [--regression] [--verbose] [--afl] [--aflswarm]")
         print("  default for <sut file> is sut.py")
         print("Options:")
         print(" --noCheck:      do not include property checks")
         print(" --noRefs:       do not include reference actions")
         print(" --regression:   produce a regression test that captures values")
         print(" --verbose:      produce a verbose test that shows actions taken")
+        print(" --afl:          test is in afl format")
+        print(" --aflswarm:     test is in afl swarm format")        
         sys.exit(0)
     
     testFile = sys.argv[1]
     outFile = sys.argv[2]
     if (len(sys.argv) > 3) and (".py" in sys.argv[3]):
         sutFile = sys.argv[3]
     else:
         sutFile = "sut.py"
 
     checkProps = not "--noCheck" in sys.argv
     checkRefs = not "--noRefs" in sys.argv
     makeRegression = "--regression" in sys.argv
     verbose = "--verbose" in sys.argv
+    afl = "--afl" in sys.argv
+    aflswarm = "--aflswarm" in sys.argv    
 
     t = SUT.sut()
 
     def globalCheck(str):
         if " # CHECK POOL INIT" not in str:
             return str
```

## src/tstl_afl.py

```diff
@@ -18,14 +18,25 @@
         return int(s)
     except:
         return None
 
 
 def main():
 
+    if "--help" in sys.argv:
+        print("Usage:  tstl_afl [--noCheck] [--swarm] [--verbose] [--showActions] [--noSave] [--alwaysSave]")
+        print("Options:")
+        print(" --noCheck:      do not run property checks")
+        print(" --swarm         use first four bytes to determine a swarm configuration")
+        print(" --verbose:      make actions verbose")
+        print(" --showActions:  show actions in test")
+        print(" --noSave:       don't save failing tests as standard TSTL tests")
+        print(" --alwaysSave:   save even non-failing tests")        
+        sys.exit(0)
+    
     sut = SUT.sut()
     saveFile = "aflfail." + str(os.getpid()) + ".test"
     
     try:
         sut.stopCoverage()
     except:
         pass
@@ -37,51 +48,42 @@
         R = random.Random()
     else:
         swarm = False
     showActions = "--showActions" in sys.argv
     if "--verbose" in sys.argv:
         sut.verbose(True)
     noSave = "--noSave" in sys.argv
+    alwaysSave = "--alwaysSave" in sys.argv        
     noCheck = "--noCheck" in sys.argv
-    bytes = 2
-    fmt = "<H"
-    if "--32" in sys.argv:
-        bytes = 4
-        fmt = "<L"
-    if "--64" in sys.argv:
-        bytes = 8
-        fmt = "<Q"
 
     afl.init()
 
     bytesin = sys.stdin.read()
 
     if len(bytesin) < 4:
         os._exit(0)        
 
     if swarm:
-        R.seed(struct.unpack(">L",bytesin[0:4]))
+        R.seed(struct.unpack("<L",bytesin[0:4])[0])
         sut.standardSwarm(R)
         bytesin = bytesin[4:]
 
     alen = len(sut.actions())
 
-    test = []
-    for i in range(0,len(bytesin)/bytes):
-        test.append(struct.unpack(fmt,bytesin[i:i+bytes])[0] % alen)
+    test = sut.bytesToTest(bytesin)
     
-    for s in test:
-        a = sut.actions()[s]
+    for a in test:
         if a[1]():
             if showActions:
-                print (a[0])
+                print (sut.prettyName(a[0]))
             ok = sut.safely(a)
             if (not noSave) and not ok:
                 sut.saveTest(sut.test(),saveFile)
             assert(ok)
             if not noCheck:
                 checkResult = sut.check()
                 if (not noSave) and not checkResult:
                     sut.saveTest(sut.test(),saveFile)            
                 assert(checkResult)
-            
+    if alwaysSave:
+        sut.saveTest(sut.test(),saveFile.replace("aflfail","afltest"))
     os._exit(0)
```

## src/static/boilerplate.py

```diff
@@ -637,21 +637,76 @@
     if len(step) > 3:
         ser += ";;;"+step[3]
     return ser
 
 def annotate(self,text):
     self.__test[-1] = self.__test[-1]+(text,)
 
-def saveTest(self, test, filename):
-    outf = open(filename,'w')
+def testToBytes(self, test):
+    alen = len(self.actions())
+    bytes = 2
+    fmt = "<H"
+    if alen < 256:
+        bytes = 1
+        fmt = "<B"    
+    if alen > 2**16:
+        bytes = 4
+        fmt = "<L"
+    data = b""
     for s in test:
-        outf.write(self.serializable(s) + "\n")
+        index = 0
+        for a in self.actions():
+            if a == s:
+                break
+            index += 1
+        p = struct.pack(fmt,index)
+        data += p
+    return data
+        
+def saveTest(self, test, filename, afl=False):
+    if not afl:
+        outf = open(filename,'w')
+    else:
+        outf = open(filename,'wb')
+    if not afl:
+        for s in test:
+            outf.write(self.serializable(s) + "\n")
+    else:
+        outf.write(self.testToBytes(test))
     outf.close()
+    
 
-def loadTest(self, filename):
+def bytesToTest(self, data, swarm=False):
+    alen = len(self.actions())
+    bytes = 2
+    fmt = "<H"
+    if alen < 256:
+        bytes = 1
+        fmt = "<B"
+    if alen > 2**16:
+        bytes = 4
+        fmt = "<L"
+    test = []
+    if swarm:
+        R = random.Random()
+        seed = struct.unpack("<L",data[0:4])[0]
+        R.seed(seed)
+        self.standardSwarm(R)
+        data = data[4:]
+        alen = len(self.actions())
+    for i in range(0,(len(data)/bytes)):
+        index = struct.unpack(fmt,data[i*bytes:(i*bytes)+bytes])[0] % alen
+        test.append(self.actions()[index])
+    return test
+        
+def loadTest(self, filename, afl=False, swarm=False):
+    if afl:
+        with open(filename,'rb') as f:
+            return self.bytesToTest(f.read(),swarm=swarm)
+        
     test = []
     with open(filename) as f:
         for l in f:
             test.append(self.playable(l[:-1]))
     return test
 
 def playable(self, name):
```

## Comparing `tstl-1.2.8.dist-info/DESCRIPTION.rst` & `tstl-1.2.9.dist-info/DESCRIPTION.rst`

 * *Files 3% similar despite different names*

```diff
@@ -454,21 +454,46 @@
 results, in our experience.  In fact, a five minute run will suffice
 for good localization, often, is five minutes is sufficient to find
 your bug a few times.
 
 TSTL and afl
 ---------
 
-So far it hasn't proven clearly useful, but you can even use afl to generate TSTL tests.  You need to install afl itself and the `python-afl` pip package.  Then you can fuzz using afl with a command like:
+You can even use afl (http://lcamtuf.coredump.cx/afl/) to generate TSTL tests.  You need to install afl itself and the `python-afl` pip package.  Then you can fuzz using afl with a command like:
 
 `py-afl-fuzz -o <outputdir> -i <inputdir> -- tstl_afl`
 
-`tstl_afl` takes a file of bytes and interprets it them as indices of TSTL actions, using `sut.py` as usual.  You can even use `--swarm` to interpret the first 4 bytes as a seed to control swarm testing.  When `tstl_afl` detects a failure it also produces a conventional TSTL test file under the name `aflfail.<PID>.test`.  
-
-Unfortunately, afl has no way to distinguish exploring the TSTL harness code and exploring SUT code, so it doesn't seem to be extremely effective as a way to generate tests.
+`tstl_afl` takes a file of bytes and interprets every two bytes as the
+index of a TSTL action (modulo the number of actions), using `sut.py`
+as usual.  When `tstl_afl` detects a failure
+it also produces a conventional TSTL test file under the name
+`aflfail.<PID>.test`.  You can even use `--swarm` to interpret the first 4 bytes
+as a seed to control swarm testing, thus allowing afl to use swarm testing; this has the drawback that the
+file will be interpreted incorrectly by other TSTL tools, unless you
+pass them the `--aflswarm` option.  Most TSTL tools take an
+`--afl` option that indicates tests to be read in are in afl format,
+and `--aflswarm` to indicate they are swarm tests.
+
+`tstl_afl` is also useful for turning a single
+afl byte file into a normal TSTL test file, using the `--alwaysSave` option, which dumps a TSTL test file in the current directory, created from the byte-based input.
+
+In theory, this is a powerful testing option, as it lets you use afl's great heuristics to fuzz things that are at best highly inconvenient with just afl.  You can set up complex TSTL properties, mix grammar generation and API-call sequences, and do differential testing TSTL-style, but use afl's tuned input generation methods.
+
+Unfortunately, afl has no way to distinguish exploring the TSTL harness code and exploring SUT code, so at least for a long initial period, it may be much less effective than the TSTL random tester.  Potentially, once it's saturated coverage of the harness, it can start picking on the SUT better, though even then the structure of the bytes may be hard to explore well using the usual afl methods.  I haven't played with it enough to know, yet.
+
+There are also tools for converting large numbers of files to and from afl format.
+`tstl_toafl` simply takes existing TSTL test files and
+converts them to afl byte inputs, and `tstl_fromafl` does the expected
+opposite (and takes an argument indicating the files are in swarm format).    `tstl_aflcorpus` randomly generates inputs that trigger novel SUT
+coverage to get afl started, but it is usually easier to just generate quick tests with
+`tstl_rt --quickTests` and convert those with `tstl_toafl`.
+`tstl_aflcorpus` does allow using the afl swarm format, however; just
+run it with `--swarm`.  Because of the way the swarm format works, it
+is unfortunately currently not possible to extract a swarm format test
+from a standard TSTL test.
 
 TSTL and Hypothesis
 ------------------------
 
 Some of you may be asking: "How does TSTL differ from the Hypothesis
 https://hypothesis.readthedocs.io/en/latest/ testing tool?"  There are a few
 answers.  First, TSTL is probably much less polished than Hypothesis,
```

## Comparing `tstl-1.2.8.dist-info/metadata.json` & `tstl-1.2.9.dist-info/metadata.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9527972027972027%*

 * *Differences: {"'extensions'": "{'python.commands': {'wrap_console': {'tstl_aflcorpus': 'src.makecorpus:main', "*

 * *                 "'tstl_fromafl': 'src.fromafl:main', 'tstl_toafl': 'src.tocorpus:main'}}, "*

 * *                 "'python.exports': {'console_scripts': {'tstl_aflcorpus': 'src.makecorpus:main', "*

 * *                 "'tstl_fromafl': 'src.fromafl:main', 'tstl_toafl': 'src.tocorpus:main'}}}",*

 * * "'version'": "'1.2.9'"}*

```diff
@@ -6,44 +6,50 @@
         "Programming Language :: Python :: 3"
     ],
     "extensions": {
         "python.commands": {
             "wrap_console": {
                 "tstl": "src.harnessmaker:main",
                 "tstl_afl": "src.tstl_afl:main",
+                "tstl_aflcorpus": "src.makecorpus:main",
+                "tstl_fromafl": "src.fromafl:main",
                 "tstl_generalize": "src.generalize:main",
                 "tstl_graph": "src.graph:main",
                 "tstl_markov": "src.markov:main",
                 "tstl_reduce": "src.reduce:main",
                 "tstl_regress": "src.runregressions:main",
                 "tstl_replay": "src.replay:main",
                 "tstl_rt": "src.randomtester:main",
-                "tstl_standalone": "src.standalone:main"
+                "tstl_standalone": "src.standalone:main",
+                "tstl_toafl": "src.tocorpus:main"
             }
         },
         "python.details": {
             "document_names": {
                 "description": "DESCRIPTION.rst"
             },
             "project_urls": {
                 "Home": "https://github.com/agroce/tstl"
             }
         },
         "python.exports": {
             "console_scripts": {
                 "tstl": "src.harnessmaker:main",
                 "tstl_afl": "src.tstl_afl:main",
+                "tstl_aflcorpus": "src.makecorpus:main",
+                "tstl_fromafl": "src.fromafl:main",
                 "tstl_generalize": "src.generalize:main",
                 "tstl_graph": "src.graph:main",
                 "tstl_markov": "src.markov:main",
                 "tstl_reduce": "src.reduce:main",
                 "tstl_regress": "src.runregressions:main",
                 "tstl_replay": "src.replay:main",
                 "tstl_rt": "src.randomtester:main",
-                "tstl_standalone": "src.standalone:main"
+                "tstl_standalone": "src.standalone:main",
+                "tstl_toafl": "src.tocorpus:main"
             }
         }
     },
     "extras": [],
     "generator": "bdist_wheel (0.30.0)",
     "keywords": [
         "testing",
@@ -56,9 +62,9 @@
         {
             "requires": [
                 "coverage"
             ]
         }
     ],
     "summary": "Template scripting testing language (TSTL)",
-    "version": "1.2.8"
+    "version": "1.2.9"
 }
```

## Comparing `tstl-1.2.8.dist-info/METADATA` & `tstl-1.2.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: tstl
-Version: 1.2.8
+Version: 1.2.9
 Summary: Template scripting testing language (TSTL)
 Home-page: https://github.com/agroce/tstl
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Keywords: testing tstl
 Platform: UNKNOWN
@@ -470,21 +470,46 @@
 results, in our experience.  In fact, a five minute run will suffice
 for good localization, often, is five minutes is sufficient to find
 your bug a few times.
 
 TSTL and afl
 ---------
 
-So far it hasn't proven clearly useful, but you can even use afl to generate TSTL tests.  You need to install afl itself and the `python-afl` pip package.  Then you can fuzz using afl with a command like:
+You can even use afl (http://lcamtuf.coredump.cx/afl/) to generate TSTL tests.  You need to install afl itself and the `python-afl` pip package.  Then you can fuzz using afl with a command like:
 
 `py-afl-fuzz -o <outputdir> -i <inputdir> -- tstl_afl`
 
-`tstl_afl` takes a file of bytes and interprets it them as indices of TSTL actions, using `sut.py` as usual.  You can even use `--swarm` to interpret the first 4 bytes as a seed to control swarm testing.  When `tstl_afl` detects a failure it also produces a conventional TSTL test file under the name `aflfail.<PID>.test`.  
-
-Unfortunately, afl has no way to distinguish exploring the TSTL harness code and exploring SUT code, so it doesn't seem to be extremely effective as a way to generate tests.
+`tstl_afl` takes a file of bytes and interprets every two bytes as the
+index of a TSTL action (modulo the number of actions), using `sut.py`
+as usual.  When `tstl_afl` detects a failure
+it also produces a conventional TSTL test file under the name
+`aflfail.<PID>.test`.  You can even use `--swarm` to interpret the first 4 bytes
+as a seed to control swarm testing, thus allowing afl to use swarm testing; this has the drawback that the
+file will be interpreted incorrectly by other TSTL tools, unless you
+pass them the `--aflswarm` option.  Most TSTL tools take an
+`--afl` option that indicates tests to be read in are in afl format,
+and `--aflswarm` to indicate they are swarm tests.
+
+`tstl_afl` is also useful for turning a single
+afl byte file into a normal TSTL test file, using the `--alwaysSave` option, which dumps a TSTL test file in the current directory, created from the byte-based input.
+
+In theory, this is a powerful testing option, as it lets you use afl's great heuristics to fuzz things that are at best highly inconvenient with just afl.  You can set up complex TSTL properties, mix grammar generation and API-call sequences, and do differential testing TSTL-style, but use afl's tuned input generation methods.
+
+Unfortunately, afl has no way to distinguish exploring the TSTL harness code and exploring SUT code, so at least for a long initial period, it may be much less effective than the TSTL random tester.  Potentially, once it's saturated coverage of the harness, it can start picking on the SUT better, though even then the structure of the bytes may be hard to explore well using the usual afl methods.  I haven't played with it enough to know, yet.
+
+There are also tools for converting large numbers of files to and from afl format.
+`tstl_toafl` simply takes existing TSTL test files and
+converts them to afl byte inputs, and `tstl_fromafl` does the expected
+opposite (and takes an argument indicating the files are in swarm format).    `tstl_aflcorpus` randomly generates inputs that trigger novel SUT
+coverage to get afl started, but it is usually easier to just generate quick tests with
+`tstl_rt --quickTests` and convert those with `tstl_toafl`.
+`tstl_aflcorpus` does allow using the afl swarm format, however; just
+run it with `--swarm`.  Because of the way the swarm format works, it
+is unfortunately currently not possible to extract a swarm format test
+from a standard TSTL test.
 
 TSTL and Hypothesis
 ------------------------
 
 Some of you may be asking: "How does TSTL differ from the Hypothesis
 https://hypothesis.readthedocs.io/en/latest/ testing tool?"  There are a few
 answers.  First, TSTL is probably much less polished than Hypothesis,
```

## Comparing `tstl-1.2.8.dist-info/RECORD` & `tstl-1.2.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/analyzeprovenance.py,sha256=GtpExXdVr-Xm3Dg5YPFQHfhSyQ4psz7zXfP5zQWTrwk,1447
 src/exhaust.py,sha256=7dY6dEm5E7Cvtk4C0cgLEFz0Qvfe81OpkU3xh3ksKAw,3851
+src/fromafl.py,sha256=v7_5_O7q801JQ-82-lswbKMBJh6LcFnezNFIpxm5vg0,820
 src/generalize.py,sha256=A3Xzo9hRxWoNS6u87r_uwEctrjHZ1GKHVd1kyXiJDhI,5193
 src/graph.py,sha256=tFKqXBvIK-JRiBNP5ymSUcNDCB-aWffxK-by0tRTzso,6262
-src/harnessmaker.py,sha256=bCQ2GnBghig5UsKXcR7eSYV8WBD1Ajw2Gs1DDZsMy30,71500
+src/harnessmaker.py,sha256=L0fZXw08g06ibkn2UFKw1zW9Qeqf6B1pMLcdL8UzllE,71572
+src/makecorpus.py,sha256=cZ0aC2KWbWg1TNqsORWRdI9SklBho9yoHVXqRpATEiE,2606
 src/markov.py,sha256=3uyURj_B7xWzo5sHEZA539WleYMyzZv6PtIGL8XJhM4,2216
 src/provenance.py,sha256=5iagzyuBk_thgI-zor3FmsYXeLEfZLk730CDKDLHpls,1883
 src/randomtester.py,sha256=h5Vqd9lcP8lGXTBy1jDQkvdcJ1NugZp7mMYQnwvefOg,81725
-src/reduce.py,sha256=86hrdUhFdPqmRVL5Ns9D5JzPoP35wh1VQnakE2zWaNY,13153
-src/replay.py,sha256=etXydmYFlwo1cuMDukxL_89-_LPog-oDfXQqAcGUlrw,6116
-src/runregressions.py,sha256=RQJ_g6VVy3EMAiESXbU0X0LPabr2CRAqPnSvYnYOt0Y,4226
-src/standalone.py,sha256=xJPcq0adsQ0aFonpBgfO7w8tPvn6ZVdzcj3-liafTAU,5410
-src/tstl_afl.py,sha256=85qMM9SeAVKliHaBk0tTCbPPwaGruoqVX46btURqcLU,1930
-src/static/boilerplate.py,sha256=zr6_7wvsBkUxPTnQ0DBRAan-5Icj-YW1iFh-qjgjScM,73277
+src/reduce.py,sha256=acHj5foEvWWo-2egP4keWW9LmK3_elfl6NYc40qjQWo,13593
+src/replay.py,sha256=6L_lR87G2JTG9IYtR0gHf9kNEDaMusIC54z7B7MltuI,6509
+src/runregressions.py,sha256=ojoy5OcRi34G_xbnkh1-utjd399FM3xlBmPKcd4R6WY,4567
+src/standalone.py,sha256=710P5ItRST72uX1yWUv1Zk0DuhkLa-PqtlorIiOss-0,5631
+src/tocorpus.py,sha256=iZL3dvV0Y0iDlxf98BoRbarYD2AYfXQs3lBI6n1ss3Q,689
+src/tstl_afl.py,sha256=3GkpGVzZFlbPsUdVvzmDqLJI4YbnDDzPnfpsbQK7PR8,2406
+src/static/boilerplate.py,sha256=5y7VTSHxwGRMoB0lgYt-5ff1SGT5pfExd3hr9Z1XLYY,74629
 src/static/boilerplate.py~,sha256=VjWtloxTctHZD4w6PNtAHASYVCJZaFfZnVeTacliYUM,4481
 src/static/boilerplate_cov.py,sha256=SOhZqoKwfXEldilVgFuuJNRrJ3jUIvFGAQy7nQ028fA,9645
 src/static/countfsize.py,sha256=8wvECgRn5fxJrCUVTHMPz-N3kKTWoGi1-SlW6WF2Ukw,532
 src/static/oldboiler,sha256=pvnQbG__55dDkhibHdaq1Ipnf4pQaKwYWiyblObOMLo,59190
 src/static/oldboiler.py,sha256=BI1dNXItezTNcGFTTIPTr1hwiLiGzpdG7pwmxE43T4M,65438
-tstl-1.2.8.dist-info/DESCRIPTION.rst,sha256=4BcUhmt7R8Ew4TdM7nN8rs5Toeow2nrwkQqxboHGbXg,33673
-tstl-1.2.8.dist-info/METADATA,sha256=GottGCEGwEpRfxmZcg9_yZP6fkxgb6zqMFH38VfX8mA,34115
-tstl-1.2.8.dist-info/RECORD,,
-tstl-1.2.8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-tstl-1.2.8.dist-info/entry_points.txt,sha256=au3KVaKxazWV7IMrBqKL9f4u1yg5UvB4NnK2Blq1mtg,390
-tstl-1.2.8.dist-info/metadata.json,sha256=4632WbHltx0G_51KE2S_A2o9pJ3EdZQo2R9GKyl7WUA,1388
-tstl-1.2.8.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
+tstl-1.2.9.dist-info/DESCRIPTION.rst,sha256=HO38owdjo79zp6RUYMlEEOT26WYygSSqHbaeiZzPhV4,35580
+tstl-1.2.9.dist-info/METADATA,sha256=wFYyLzbsyWeTBSWho7LRhEvtK5Q_nbQgyb7ThamLWO0,36022
+tstl-1.2.9.dist-info/RECORD,,
+tstl-1.2.9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+tstl-1.2.9.dist-info/entry_points.txt,sha256=MocWnb5fzA4e5AxFb3woiKWRoHxX-9DxKIzjh0MYCkg,502
+tstl-1.2.9.dist-info/metadata.json,sha256=VgYT0X7YjGQYndbb8KRytrr8sMBDgNm3E_XHirLIqK0,1612
+tstl-1.2.9.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
```

