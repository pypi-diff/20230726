# Comparing `tmp/rchitect-0.3.9.tar.gz` & `tmp/rchitect-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rchitect-0.3.9.tar", last modified: Mon Sep 16 07:43:25 2019, max compression
+gzip compressed data, was "rchitect-0.4.1.tar", last modified: Tue Jul 25 22:30:26 2023, max compression
```

## Comparing `rchitect-0.3.9.tar` & `rchitect-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-16 07:43:25.000000 rchitect-0.3.9/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3088 2019-09-16 07:43:25.000000 rchitect-0.3.9/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2327 2019-09-16 07:43:21.000000 rchitect-0.3.9/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      356 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/callbacks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/completion.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1111 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/console.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3858 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/dispatch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21154 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/interface.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1460 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/py_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5453 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/py_tools.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      834 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/repl.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect/reticulate/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      908 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/reticulate/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1260 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/reticulate/config.R
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3069 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22841 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/R.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1519 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/build.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      484 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/gli.c
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/gli.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16113 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/libR.c
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1923 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/libR.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      695 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/parse.c
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/parse.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/process_events.c
--rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/src/process_events.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4708 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4240 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2019-09-16 07:43:21.000000 rchitect-0.3.9/rchitect/xptr.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3088 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      727 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2019-09-16 07:43:25.000000 rchitect-0.3.9/rchitect.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2019-09-16 07:43:25.000000 rchitect-0.3.9/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2019-09-16 07:43:21.000000 rchitect-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:30:26.458928 rchitect-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-25 22:30:14.000000 rchitect-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 22:30:14.000000 rchitect-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-25 22:30:26.458928 rchitect-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-25 22:30:14.000000 rchitect-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-25 22:30:14.000000 rchitect-0.4.1/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:30:26.454928 rchitect-0.4.1/rchitect/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24376 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/py_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:30:26.458928 rchitect-0.4.1/rchitect/reticulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/reticulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/reticulate/config.R
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/reticulate/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/reticulate/py_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:30:26.458928 rchitect-0.4.1/rchitect/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/R.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/gil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/libR.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/libR.h
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/process_events.c
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/src/process_events.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 22:30:14.000000 rchitect-0.4.1/rchitect/xptr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:30:26.458928 rchitect-0.4.1/rchitect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-25 22:30:26.000000 rchitect-0.4.1/rchitect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-25 22:30:26.000000 rchitect-0.4.1/rchitect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:30:26.000000 rchitect-0.4.1/rchitect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 22:30:26.000000 rchitect-0.4.1/rchitect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 22:30:26.000000 rchitect-0.4.1/rchitect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 22:30:26.458928 rchitect-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-25 22:30:14.000000 rchitect-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rchitect-0.3.9/PKG-INFO` & `rchitect-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rchitect
-Version: 0.3.9
+Version: 0.4.1
 Summary: Mapping R API to Python
 Home-page: https://github.com/randy3k/rchitect
 Author: Randy Lai
 Author-email: randy.cs.lai@gmail.com
 License: UNKNOWN
 Description: # Interoperate R with Python
         
-        [![CircleCI](https://circleci.com/gh/randy3k/rchitect/tree/master.svg?style=shield)](https://circleci.com/gh/randy3k/rchitect/tree/master)
-        [![Build status](https://ci.appveyor.com/api/projects/status/4o9m8q61m755xc2a/branch/master?svg=true)](https://ci.appveyor.com/project/randy3k/rchitect/branch/master)
+        [![Main](https://github.com/randy3k/rchitect/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/rchitect/actions/workflows/main.yml)
         [![codecov](https://codecov.io/gh/randy3k/rchitect/branch/master/graph/badge.svg)](https://codecov.io/gh/randy3k/rchitect)
         [![pypi](https://img.shields.io/pypi/v/rchitect.svg)](https://pypi.org/project/rchitect/)
+        [![Conda version](https://img.shields.io/conda/vn/conda-forge/rchitect.svg)](https://anaconda.org/conda-forge/rchitect)
         
         
         ## Installation
         
         ```sh
         # install released version
         pip install -U rchitect
@@ -28,43 +28,45 @@
         
         You may be curious why I reinvented the wheel when there is [`rpy2`](https://github.com/rpy2/rpy2)?
         
         The main reason is to drive [`radian`](https://github.com/randy3k/radian).
         `rpy2` was not suitable because it is missing some key features for running
         the R REPL. Speaking of compatibility, `rchitect` has been thoroughly tested on
         multiple platforms such as Windows, macOS and Linux and we also provide binary
-        wheels for user convenience.
+        wheels for python 3.6+.
         
         ## Getting started
         
         ```py
         from rchitect import *
         a = reval("1:5")     # evaluate an R expression in the global environment
         b = rcopy(a)         # convert any RObject returned by `reval` to its python type
         c = robject(b)       # convert any python object to its R type
         d = rcall("sum", c)  # call an R function. Python objects are converted to RObjects implicitly.
         ```
         
         ## FAQ
         
-        If `rchitect` fails to open the R shared library, user should first
-        try to expose the path to R to the `PATH` vaiable.
+        #### How to switch to a different R or specify the version of R.
         
-        In Linux/macOS, you could also export the environment variable `R_HOME`. For example,
-        ```sh
-        $ export R_HOME=/usr/local/lib/R
-        $ radian
-        ```
-        Sometimes, you may also need to futher specify `LD_LIBRARY_PATH` if R fails to find some shared libraries,
+        There are a few options.
+        
+        - One could expose the path to the R binary in the `PATH` variable
+        - The environment variable `R_BINARY` could also be used to specify the path to R.
+        - The environment variable `R_HOME` could also be used to specify R home directory. Note that it is should be set as the result of `R.home()`, not the directory where `R` is located. For example, in Unix
         ```sh
-        export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:`R RHOME`/lib"
+        $ env R_HOME=/usr/local/lib/R radian
         ```
         
+        #### Cannot find shared library
+        
         Please also make sure that R was installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On Linux, the flag `--enable-R-shlib` may be needed to install R from the source.
         
+        
         ## Wiki
         
         [reticulate](https://github.com/randy3k/rchitect/wiki/Conversions-between-reticulate-and-rchitect-objects-are-seamless) conversions
         
 Platform: UNKNOWN
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `rchitect-0.3.9/README.md` & `rchitect-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Interoperate R with Python
 
-[![CircleCI](https://circleci.com/gh/randy3k/rchitect/tree/master.svg?style=shield)](https://circleci.com/gh/randy3k/rchitect/tree/master)
-[![Build status](https://ci.appveyor.com/api/projects/status/4o9m8q61m755xc2a/branch/master?svg=true)](https://ci.appveyor.com/project/randy3k/rchitect/branch/master)
+[![Main](https://github.com/randy3k/rchitect/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/rchitect/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/randy3k/rchitect/branch/master/graph/badge.svg)](https://codecov.io/gh/randy3k/rchitect)
 [![pypi](https://img.shields.io/pypi/v/rchitect.svg)](https://pypi.org/project/rchitect/)
+[![Conda version](https://img.shields.io/conda/vn/conda-forge/rchitect.svg)](https://anaconda.org/conda-forge/rchitect)
 
 
 ## Installation
 
 ```sh
 # install released version
 pip install -U rchitect
@@ -20,39 +20,40 @@
 
 You may be curious why I reinvented the wheel when there is [`rpy2`](https://github.com/rpy2/rpy2)?
 
 The main reason is to drive [`radian`](https://github.com/randy3k/radian).
 `rpy2` was not suitable because it is missing some key features for running
 the R REPL. Speaking of compatibility, `rchitect` has been thoroughly tested on
 multiple platforms such as Windows, macOS and Linux and we also provide binary
-wheels for user convenience.
+wheels for python 3.6+.
 
 ## Getting started
 
 ```py
 from rchitect import *
 a = reval("1:5")     # evaluate an R expression in the global environment
 b = rcopy(a)         # convert any RObject returned by `reval` to its python type
 c = robject(b)       # convert any python object to its R type
 d = rcall("sum", c)  # call an R function. Python objects are converted to RObjects implicitly.
 ```
 
 ## FAQ
 
-If `rchitect` fails to open the R shared library, user should first
-try to expose the path to R to the `PATH` vaiable.
+#### How to switch to a different R or specify the version of R.
 
-In Linux/macOS, you could also export the environment variable `R_HOME`. For example,
-```sh
-$ export R_HOME=/usr/local/lib/R
-$ radian
-```
-Sometimes, you may also need to futher specify `LD_LIBRARY_PATH` if R fails to find some shared libraries,
+There are a few options.
+
+- One could expose the path to the R binary in the `PATH` variable
+- The environment variable `R_BINARY` could also be used to specify the path to R.
+- The environment variable `R_HOME` could also be used to specify R home directory. Note that it is should be set as the result of `R.home()`, not the directory where `R` is located. For example, in Unix
 ```sh
-export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:`R RHOME`/lib"
+$ env R_HOME=/usr/local/lib/R radian
 ```
 
+#### Cannot find shared library
+
 Please also make sure that R was installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On Linux, the flag `--enable-R-shlib` may be needed to install R from the source.
 
+
 ## Wiki
 
 [reticulate](https://github.com/randy3k/rchitect/wiki/Conversions-between-reticulate-and-rchitect-objects-are-seamless) conversions
```

### Comparing `rchitect-0.3.9/rchitect/callbacks.py` & `rchitect-0.4.1/rchitect/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     setattr(callback, name, None)
 
 
 # prevent rstart being gc'ed
 _protected = {}
 
 
-def setup_rstart(args):
+def setup_rstart(rhome, args):
     rstart = ffi.new("Rstart")
     _protected["rstart"] = rstart
     SA_NORESTORE = 0
     SA_RESTORE = 1
     # SA_DEFAULT = 2
     SA_NOSAVE = 3
     SA_SAVE = 4
@@ -79,26 +79,27 @@
         rstart.RestoreAction = SA_RESTORE
     if "--no-save" in args:
         rstart.SaveAction = SA_NOSAVE
     elif "--save" in args:
         rstart.SaveAction = SA_SAVE
     else:
         rstart.SaveAction = SA_SAVEASK
-    rhome = ffi.new("char[]", ffi.string(lib.get_R_HOME()))
+    rhome = ffi.new("char[]", rhome.encode("utf-8"))
     _protected["rhome"] = rhome
     rstart.rhome = rhome
     home = ffi.new("char[]", ffi.string(lib.getRUser()))
     _protected["home"] = home
     rstart.home = home
     rstart._ReadConsole = ffi.addressof(lib, "cb_read_console_interruptible")
     rstart._WriteConsole = ffi.NULL
-    rstart.CallBack = ffi.addressof(lib, "cb_polled_events")
+    rstart.CallBack = ffi.addressof(lib, "cb_polled_events_interruptible")
     rstart.ShowMessage = ffi.addressof(lib, "cb_show_message")
     rstart.YesNoCancel = ffi.addressof(lib, "cb_yes_no_cancel")
     rstart.Busy = ffi.addressof(lib, "cb_busy")
+    # we cannot get it to RGui, otherwise `do_system` will clear the standard handlers
     rstart.CharacterMode = 1  # RTerm
     rstart.WriteConsoleEx = ffi.addressof(lib, "cb_write_console_capturable")
     lib.R_SetParams(rstart)
 
 
 def setup_callback(p, name, cb_name=None):
     if name is None:
@@ -112,69 +113,74 @@
     setup_callback("R_Outputfile", None)
     setup_callback("R_Consolefile", None)
 
     setup_callback("ptr_R_Suicide", "suicide")
     setup_callback("ptr_R_ShowMessage", "show_message")
     setup_callback("ptr_R_ReadConsole", "read_console", "cb_read_console_interruptible")
     setup_callback("ptr_R_WriteConsole", None)
-    setup_callback("ptr_R_WriteConsoleEx", "write_console_ex", "cb_write_console_capturable")
+    setup_callback("ptr_R_WriteConsoleEx", "write_console_ex", "cb_write_console_safe")
     setup_callback("ptr_R_ResetConsole", "reset_console")
     setup_callback("ptr_R_FlushConsole", "flush_console")
     setup_callback("ptr_R_ClearerrConsole", "clearerr_console")
-    setup_callback("ptr_R_Busy", "busy")
+    setup_callback("ptr_R_Busy", "busy", "cb_busy_safe")
     setup_callback("ptr_R_CleanUp", "clean_up")
     setup_callback("ptr_R_ShowFiles", "show_files")
     setup_callback("ptr_R_ChooseFile", "choose_file")
     setup_callback("ptr_R_EditFile", "edit_file")
     setup_callback("ptr_R_loadhistory", "loadhistory")
     setup_callback("ptr_R_savehistory", "savehistory")
     setup_callback("ptr_R_addhistory", "addhistory")
     setup_callback("ptr_R_EditFiles", "edit_files")
     setup_callback("ptr_do_selectlist", "do_selectlist")
     setup_callback("ptr_do_dataentry", "do_dataentry")
     setup_callback("ptr_do_dataviewer", "do_dataviewer")
     setup_callback("ptr_R_ProcessEvents", "process_events")
-    setup_callback("R_PolledEvents", "polled_events")
+    setup_callback("R_PolledEvents", "polled_events", "cb_polled_events_interruptible")
 
 
 @ffi.def_extern()
 def cb_show_message(buf):
     callback.show_message(rconsole2str(ffi.string(buf)))
 
 
-def on_read_console_error(exception, exc_value, traceback):
+def on_callback_error(exception, exc_value, traceback):
     if exception == KeyboardInterrupt:
-        lib.cb_read_console_interrupted = 1
+        lib.cb_interrupted = 1
     elif exception == EOFError:
         pass
     else:
-        print(exception, exc_value)
+        print("callback error:", exception, exc_value)
 
 
-_code = [""]
+_code = [b""]
 
 
-@ffi.def_extern(error=0, onerror=on_read_console_error)
+@ffi.def_extern(error=0, onerror=on_callback_error)
 def cb_read_console(p, buf, buflen, add_history):
     # cache the code as buflen is limited to 4096
     if _code[0]:
         code = _code[0]
     else:
         text = callback.read_console(rconsole2str(ffi.string(p)), add_history)
         if text is None:
             return 0
         code = utf8tosystem(text)
         _code[0] = code
 
     buf = ffi.cast("char*", buf)
-    nb = min(len(code), buflen - 2)
-    buf[0:nb] = code[0:nb]
-    if nb < buflen - 2:
+
+    if len(code) < buflen:
+        nb = len(code)
+        buf[0:nb] = code[0:nb]
         buf[nb] = b'\n'
         buf[nb + 1] = b'\x00'
+    elif len(code) >= buflen:
+        nb = buflen - 1
+        buf[0:nb] = code[0:nb]
+        buf[nb] = b'\x00'
 
     _code[0] = _code[0][nb:]
     return 1
 
 
 @ffi.def_extern()
 def cb_write_console_capturable(buf, bufline, otype):
@@ -188,16 +194,16 @@
 
 
 @ffi.def_extern()
 def cb_clean_up(saveact, status, run_last):
     callback.clean_up(saveact, status, run_last)
 
 
-@ffi.def_extern()
+@ffi.def_extern(error=None, onerror=on_callback_error)
 def cb_polled_events():
-    console.flush()
+    console.flush()  # needed for reval
     callback.polled_events()
 
 
 @ffi.def_extern()
 def cb_yes_no_cancel(p):
     return callback.yes_no_cancel(rconsole2str(ffi.string(p)))
```

### Comparing `rchitect-0.3.9/rchitect/dispatch.py` & `rchitect-0.4.1/rchitect/dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,22 @@
             if parent not in self._ordering:
                 raise TypeError(
                     AMBIGUITY.format(
                         str(types),
                         str(signature),
                         str(parent)))
 
-        p = 0
-        for signature in self._ordering:
+        q = 0
+        for p, signature in enumerate(self._ordering):
+            if len(signature) == n and all(map(issubclass, signature, types)):
+                q = p + 1
             if len(signature) == n and all(map(issubclass, types, signature)):
                 break
-            p = p + 1
-        self._ordering.insert(p, types)
+
+        self._ordering.insert(q, types)
 
     def add(self, types, func):
         # support union types
         if any(isinstance(typ, tuple) for typ in types):
             for typs in expand_tuples(types):
                 self.add(typs, func)
             return
```

### Comparing `rchitect-0.3.9/rchitect/interface.py` & `rchitect-0.4.1/rchitect/interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import unicode_literals, absolute_import
 from rchitect._cffi import ffi, lib
 from .dispatch import dispatch
 from .types import RObject, SEXP, RClass, sexptype, datatype
 from .types import NILSXP, CLOSXP, ENVSXP, BUILTINSXP, LGLSXP, INTSXP, REALSXP, CPLXSXP, STRSXP, \
     VECSXP, EXPRSXP, EXTPTRSXP, RAWSXP, S4SXP
 from .types import box, unbox
-from .xptr import new_xptr, new_xptr_p, from_xptr
-from .console import capture_console, read_stderr
+from .xptr import new_xptr_p, from_xptr
+from .console import capture_console, read_stdout, read_stderr
+from .utils import utf8tosystem
 
 
 import sys
 import ctypes
 import struct
 from contextlib import contextmanager
 from six import text_type, string_types
@@ -36,15 +37,15 @@
         value = default
     return value
 
 
 def ensure_initialized():
     if lib.Rf_initialize_R == ffi.NULL:
         from .setup import init
-        init()
+        init(register_callbacks=False, register_signal_handlers=False)
 
 
 @contextmanager
 def protected(*args):
     nprotect = 0
     for a in args:
         if isinstance(a, SEXP):
@@ -78,15 +79,15 @@
 
 def rdouble(s):
     return box(rdouble_p(s))
 
 
 def rchar_p(s):
     isascii = all(ord(c) < 128 for c in s)
-    b = s.encode("utf-8")
+    b = s.encode('utf-8')
     return lib.Rf_mkCharLenCE(b, len(b), lib.CE_NATIVE if isascii else lib.CE_UTF8)
 
 
 def rchar(s):
     return box(rchar_p(s))
 
 
@@ -98,66 +99,82 @@
     return box(rstring_p(s))
 
 
 def rsym_p(s, t=None):
     if t:
         return rlang_p("::", rsym_p(s), rsym_p(t))
     else:
-        return lib.Rf_install(s.encode("utf-8"))
+        return lib.Rf_install(utf8tosystem(s))
 
 
 def rsym(s, t=None):
     return box(rsym_p(s, t))
 
 
+def parse_text(s):
+    status = ffi.new("ParseStatus[1]")
+    s = lib.Rf_mkString(utf8tosystem(s))
+    with protected(s), capture_console():  # need to capture stderr
+        ret = lib.R_ParseVector(s, -1, status, lib.R_NilValue)
+        if status[0] != lib.PARSE_OK:
+            err = read_stderr().strip() or "Error"
+        else:
+            err = None
+        return ret, status[0], err
+
+
+def parse_text_incomplete(s):
+    _, status, _ = parse_text(s)
+    return status == lib.PARSE_INCOMPLETE
+
+
+def parse_text_complete(s):
+    return not parse_text_incomplete(s)
+
+
 def rparse_p(s):
     ensure_initialized()
-    status = ffi.new("ParseStatus[1]")
-    s = rstring_p(s)
-    with protected(s):
-        with capture_console():
-            ret = lib.R_ParseVector(s, -1, status, lib.R_NilValue)
-            if status[0] != lib.PARSE_OK:
-                err = read_stderr().strip() or "Error"
-                raise RuntimeError("{}".format(err))
+    ret, status, err = parse_text(s)
+    if status != lib.PARSE_OK:
+        raise RuntimeError("{}".format(err))
     return ret
 
 
 def rparse(s):
     return box(rparse_p(s))
 
 
 @dispatch(EXPRSXP)
 def reval_p(s, envir=None):
     ensure_initialized()
-    if envir:
-        # `sys.frame()` doesn't work with R_tryEval as it doesn't create R stacks,
-        # we use `base::eval` instead.
-        ret = rcall_p(("base", "eval"), s, _envir=envir)
-    else:
-        ret = lib.R_NilValue
-        status = ffi.new("int[1]")
-        with protected(s):
-            with capture_console():
+    with protected(s):
+        if envir:
+            # `sys.frame()` doesn't work with R_tryEval as it doesn't create R stacks,
+            # we use `base::eval` instead.
+            ret = rcall_p(("base", "eval"), s, _envir=envir)
+        else:
+            ret = lib.R_NilValue
+            status = ffi.new("int[1]")
+            with capture_console():  # need to capture stderr
                 for i in range(0, lib.Rf_length(s)):
                     ret = lib.R_tryEval(lib.VECTOR_ELT(s, i), lib.R_GlobalEnv, status)
                     if status[0] != 0:
                         err = read_stderr().strip() or "Error"
                         raise RuntimeError("{}".format(err))
     return ret
 
 
-@dispatch(RObject)  # noqa
-def reval_p(s, envir=None):
+@dispatch(RObject)
+def reval_p(s, envir=None): # noqa
     with protected(envir):
         return reval_p(unbox(s), envir=envir)
 
 
-@dispatch(string_types)  # noqa
-def reval_p(s, envir=None):
+@dispatch(string_types)
+def reval_p(s, envir=None): # noqa
     with protected(envir):
         return reval_p(rparse_p(s), envir=envir)
 
 
 def reval(s, envir=None):
     return box(reval_p(s, envir=envir))
 
@@ -188,103 +205,118 @@
 
             for a in args:
                 s = lib.CDR(s)
                 lib.SETCAR(s, unbox(a))
             for k, v in kwargs.items():
                 s = lib.CDR(s)
                 lib.SETCAR(s, unbox(v))
-                lib.SET_TAG(s, lib.Rf_install(k.encode("utf-8")))
+                lib.SET_TAG(s, lib.Rf_install(utf8tosystem(k)))
 
             ret = t
     return ret
 
 
 def rlang(*args, **kwargs):
     return box(rlang_p(*args, **kwargs))
 
 
 @contextmanager
-def sexp_args(args, kwargs):
+def sexp_args(args, kwargs, asis=False):
     nprotect = 0
     try:
+        for a in args:
+            if isinstance(a, SEXP):
+                lib.Rf_protect(a)
+                nprotect += 1
+        for _, v in kwargs.items():
+            if isinstance(v, SEXP):
+                lib.Rf_protect(v)
+                nprotect += 1
         _args = []
         for a in args:
-            _a = sexp(a)
-            if isinstance(_a, SEXP):
-                lib.Rf_protect(_a)
+            if not isinstance(a, SEXP):
+                a = sexp_as_py_object(a) if asis else sexp(a)
+                lib.Rf_protect(a)
                 nprotect += 1
-            _args.append(_a)
-
+            _args.append(a)
         _kwargs = {}
         for k, v in kwargs.items():
-            _v = sexp(v)
-            if isinstance(_v, SEXP):
-                lib.Rf_protect(_v)
+            if not isinstance(v, SEXP):
+                v = sexp_as_py_object(v) if asis else sexp(v)
+                lib.Rf_protect(v)
                 nprotect += 1
-            _kwargs[k] = _v
+            _kwargs[k] = v
 
         yield _args, _kwargs
     finally:
         lib.Rf_unprotect(nprotect)
 
 
 def rcall_p(f, *args, **kwargs):
     ensure_initialized()
     _envir = extract(kwargs, "_envir")
+    _asis = extract(kwargs, "_asis")
     if _envir:
         _envir = unbox(_envir)
     else:
         _envir = lib.R_GlobalEnv
 
-    with protected(_envir):
-        with sexp_args(args, kwargs) as (a, k):
-            with capture_console():
+    with protected(f, _envir):
+        with sexp_args(args, kwargs, _asis) as (a, k):
+            with capture_console():  # need to capture stderr
                 status = ffi.new("int[1]")
-                val = lib.R_tryEval(rlang_p(f, *a, **k), _envir, status)
-                if status[0] != 0:
-                    err = read_stderr().strip() or "Error"
-                    raise RuntimeError("{}".format(err))
+                lang = rlang_p(f, *a, **k)
+                with protected(lang):
+                    val = lib.R_tryEval(lang, _envir, status)
+                    if status[0] != 0:
+                        err = read_stderr().strip() or "Error"
+                        raise RuntimeError("{}".format(err))
     return val
 
 
 def rcall(*args, **kwargs):
     _convert = extract(kwargs, "_convert")
     s = rcall_p(*args, **kwargs)
-    return rcopy(s) if _convert else box(s)
+    with protected(s):
+        return rcopy(s) if _convert else box(s)
 
 
-def rprint(s):
-    new_env = rcall(("base", "new.env"))
-    lib.Rf_defineVar(rsym_p("x"), unbox(s), unbox(new_env))
+def rprint(s, envir=None):
     with protected(s):
-        try:
-            rcall(("base", "print"), rsym("x"), _envir=new_env)
-        finally:
-            lib.Rf_defineVar(rsym_p("x"), lib.R_NilValue, unbox(new_env))
+        symx = rsym_p("x")
+        with protected(symx):
+            if not envir:
+                envir = new_env()
+            lib.Rf_defineVar(symx, unbox(s), unbox(envir))
+            try:
+                rcall(("base", "print"), symx, _envir=envir)
+            finally:
+                lib.Rf_defineVar(symx, lib.R_NilValue, unbox(envir))
 
 
 def _repr(self):
     s = self.s
-    new_env = rcall(("base", "new.env"))
-    lib.Rf_defineVar(rsym_p("x"), unbox(s), unbox(new_env))
-    try:
-        output = rcall(("utils", "capture.output"), rlang(("base", "print"), rsym_p("x")), _envir=new_env)
-    finally:
-        lib.Rf_defineVar(rsym_p("x"), lib.R_NilValue, unbox(new_env))
+    envir = new_env(parent=getoption_p("rchitect.py_tools"))
+    with capture_console(flushable=False):  # need to capture stdout
+        rprint(s, envir=envir)
+        output = read_stdout() or ""
 
     name = "RObject{{{}}}".format(str(sexptype(s)))
-    if not lib.Rf_isNull(unbox(output)) and lib.Rf_length(unbox(output)) > 0:
-        try:
-            return name + "\n" + "\n".join(rcopy(list, output))
-        except Exception:
-            pass
-    return name
+    if output:
+        return name + "\n" + output.rstrip()
+    else:
+        return name
+
+
+def _call(self, *args, **kwargs):
+    return rcall(self, *args, **kwargs)
 
 
 RObject.__repr__ = _repr
+RObject.__call__ = _call
 
 
 def getoption_p(key):
     return lib.Rf_GetOption1(rsym_p(key))
 
 
 def getoption(key):
@@ -331,14 +363,33 @@
     return rcopy(text_type if singleString else list, getclass_p(s, singleString))
 
 
 def process_events():
     lib.process_events()
 
 
+def polled_events():
+    lib.polled_events()
+
+
+def peek_event():
+    return lib.peek_event()
+
+
+def new_env_p(parent=None):
+    with protected(parent):
+        if not parent:
+            parent = lib.R_GlobalEnv
+        return lib.Rf_NewEnvironment(lib.R_NilValue, lib.R_NilValue, unbox(parent))
+
+
+def new_env(parent=None):
+    return box(new_env_p(parent))
+
+
 def set_hook(event, fun):
     rcall(("base", "setHook"), event, fun)
 
 
 def package_event(pkg, event):
     return rcall(("base", "packageEvent"), pkg, event)
 
@@ -348,403 +399,424 @@
     return "{} -- \"{}\"\nPlatform: {} ({}-bit)\n".format(
         info["version.string"], info["nickname"], info["platform"], 8 * struct.calcsize("P"))
 
 
 # R to Py
 
 
-@dispatch(datatype(type(None)), NILSXP)  # noqa
-def rcopy(_, s):
+@contextmanager
+def rcopy_context(**kwargs):
+    old_context = rcopy_context.context.copy()
+    rcopy_context.context.update(kwargs)
+    yield rcopy_context.context
+    rcopy_context.context = old_context
+
+
+rcopy_context.context = {}
+
+
+@dispatch(datatype(type(None)), NILSXP)
+def rcopy(_, s): # noqa
     return None
 
 
-@dispatch(datatype(list), NILSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), NILSXP)
+def rcopy(_, s): # noqa
     return []
 
 
-@dispatch(datatype(int), INTSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(int), INTSXP)
+def rcopy(_, s): # noqa
     return lib.INTEGER(s)[0]
 
 
-@dispatch(datatype(list), INTSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), INTSXP)
+def rcopy(_, s): # noqa
     return [lib.INTEGER(s)[i] for i in range(lib.Rf_length(s))]
 
 
-@dispatch(datatype(bool), LGLSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(bool), LGLSXP)
+def rcopy(_, s): # noqa
     return bool(lib.LOGICAL(s)[0])
 
 
-@dispatch(datatype(list), LGLSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), LGLSXP)
+def rcopy(_, s): # noqa
     return [bool(lib.LOGICAL(s)[i]) for i in range(lib.Rf_length(s))]
 
 
-@dispatch(datatype(float), REALSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(float), REALSXP)
+def rcopy(_, s): # noqa
     return lib.REAL(s)[0]
 
 
-@dispatch(datatype(list), REALSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), REALSXP)
+def rcopy(_, s): # noqa
     return [lib.REAL(s)[i] for i in range(lib.Rf_length(s))]
 
 
-@dispatch(datatype(complex), CPLXSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(complex), CPLXSXP)
+def rcopy(_, s): # noqa
     z = lib.COMPLEX(s)[0]
     return complex(z.r, z.i)
 
 
-@dispatch(datatype(list), CPLXSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), CPLXSXP)
+def rcopy(_, s): # noqa
     return [complex(lib.COMPLEX(s)[i].r, lib.COMPLEX(s)[i].i) for i in range(lib.Rf_length(s))]
 
 
 def _string(s):
     return text_type(ffi.string(lib.Rf_translateCharUTF8(s)).decode("utf-8"))
 
 
-@dispatch(datatype(bytes), RAWSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(bytes), RAWSXP)
+def rcopy(_, s): # noqa
     return ffi.string(lib.RAW(s), lib.Rf_length(s))
 
 
-@dispatch(datatype(text_type), STRSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(text_type), STRSXP)
+def rcopy(_, s): # noqa
     return _string(lib.STRING_ELT(s, 0))
 
 
-@dispatch(datatype(list), STRSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), STRSXP)
+def rcopy(_, s): # noqa
     return [_string(lib.STRING_ELT(s, i)) for i in range(lib.Rf_length(s))]
 
 
-@dispatch(datatype(list), VECSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(list), VECSXP)
+def rcopy(_, s): # noqa
     return [rcopy(lib.VECTOR_ELT(s, i)) for i in range(lib.Rf_length(s))]
 
 
-@dispatch(datatype(tuple), VECSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(tuple), VECSXP)
+def rcopy(_, s): # noqa
     return tuple(rcopy(list, s))
 
 
-@dispatch(datatype(dict), VECSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(dict), VECSXP)
+def rcopy(_, s): # noqa
     ret = dict()
     names = rnames(s)
     for i in range(lib.Rf_length(s)):
         ret[names[i]] = rcopy(lib.VECTOR_ELT(s, i))
     return ret
 
 
-@dispatch(datatype(OrderedDict), VECSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(OrderedDict), VECSXP)
+def rcopy(_, s): # noqa
     ret = OrderedDict()
     names = rnames(s)
     for i in range(lib.Rf_length(s)):
         ret[names[i]] = rcopy(lib.VECTOR_ELT(s, i))
     return ret
 
 
-@dispatch(datatype(FunctionType), (CLOSXP, BUILTINSXP))  # noqa
-def rcopy(_, s, envir=None, convert=True):
+@dispatch(datatype(FunctionType), (CLOSXP, BUILTINSXP))
+def rcopy(_, s): # noqa
     r = RObject(s)  # preserve the closure
 
-    def _(*args, **kwargs):
-        return rcall(r, *args, _envir=envir, _convert=convert, **kwargs)
+    def f(*args, **kwargs):
+        return rcall(s, *args, _asis=f.asis, _convert=f.convert, **kwargs)
 
-    return _
+    f.__robject__ = r
+    with rcopy_context() as context:
+        f.asis = context.get('asis', False)
+        f.convert = context.get('convert', True)
+
+    return f
 
 
 # PyObject
-@dispatch(datatype(object), EXTPTRSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(object), EXTPTRSXP)
+def rcopy(_, s): # noqa
+    # FIXME: check if s really is a PyObject
     return from_xptr(s)
 
 
 # reticulate's python.builtin.object
-@dispatch(datatype(object), ENVSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(object), ENVSXP)
+def rcopy(_, s): # noqa
     x = rcall(("base", "get"), "pyobj", s)
     p = ffi.cast("uintptr_t", lib.R_ExternalPtrAddr(unbox(x)))
     d = long(p)
     obj = ctypes.cast(d, ctypes.py_object)
     return obj.value
 
 
 # PyCallable or reticulate's python.builtin.function
-@dispatch(datatype(object), CLOSXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(object), CLOSXP)
+def rcopy(_, s): # noqa
     return rcopy(getattrib_p(s, "py_object"))
 
 
-@dispatch(datatype(RObject), SEXP)  # noqa
-def rcopy(_, s):
+@dispatch(datatype(RObject), SEXP)
+def rcopy(_, s): # noqa
     return box(s)
 
 
-@dispatch(datatype(RObject), RObject)  # noqa
-def rcopy(_, s):
-    return s
-
-
-@dispatch(object, RObject)  # noqa
-def rcopy(t, r, **kwargs):
-    return rcopy(t, unbox(r), **kwargs)
-
-
 # default conversions
 default = RClass("default")
 
 
-@dispatch(SEXP)  # noqa
-def rcopy(s, **kwargs):
-    ensure_initialized()
+@dispatch(SEXP)
+def rcopy(s): # noqa
     for cls in rclass(s):
         T = rcopytype(RClass(cls), s)
         if T is not RObject:
-            return rcopy(T, s, **kwargs)
+            return rcopy(T, s)
     T = rcopytype(default, s)
-    return rcopy(T, s, **kwargs)
+    return rcopy(T, s)
+
 
+@dispatch(object, RObject)
+def rcopy(t, r, **kwargs): # noqa
+    with rcopy_context(**kwargs):
+        return rcopy(t, unbox(r))
 
-@dispatch(RObject)  # noqa
-def rcopy(r, **kwargs):
-    return rcopy(unbox(r), **kwargs)
+
+@dispatch(RObject)
+def rcopy(r, **kwargs): # noqa
+    with rcopy_context(**kwargs):
+        return rcopy(unbox(r))
 
 
 # PyObject
-@dispatch(datatype(RClass("PyObject")), EXTPTRSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(RClass("PyObject")), EXTPTRSXP)
+def rcopytype(_, s): # noqa
     return object
 
 
 # PyCallable
-@dispatch(datatype(RClass("PyCallable")), CLOSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(RClass("PyCallable")), CLOSXP)
+def rcopytype(_, s): # noqa
     return object
 
 
 # reticulate class
-@dispatch(datatype(RClass("python.builtin.object")), ENVSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(RClass("python.builtin.object")), ENVSXP)
+def rcopytype(_, s): # noqa
     return object
 
 
 # reticulate function
-@dispatch(datatype(RClass("python.builtin.function")), CLOSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(RClass("python.builtin.function")), CLOSXP)
+def rcopytype(_, s): # noqa
     return object
 
 
-@dispatch(datatype(default), NILSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), NILSXP)
+def rcopytype(_, s): # noqa
     return type(None)
 
 
-@dispatch(datatype(default), INTSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), INTSXP)
+def rcopytype(_, s): # noqa
     return int if lib.Rf_length(s) == 1 else list
 
 
-@dispatch(datatype(default), LGLSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), LGLSXP)
+def rcopytype(_, s): # noqa
     return bool if lib.Rf_length(s) == 1 else list
 
 
-@dispatch(datatype(default), REALSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), REALSXP)
+def rcopytype(_, s): # noqa
     return float if lib.Rf_length(s) == 1 else list
 
 
-@dispatch(datatype(default), CPLXSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), CPLXSXP)
+def rcopytype(_, s): # noqa
     return complex if lib.Rf_length(s) == 1 else list
 
 
-@dispatch(datatype(default), RAWSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), RAWSXP)
+def rcopytype(_, s): # noqa
     return bytes
 
 
-@dispatch(datatype(default), STRSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), STRSXP)
+def rcopytype(_, s): # noqa
     return text_type if lib.Rf_length(s) == 1 else list
 
 
-@dispatch(datatype(default), VECSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), VECSXP)
+def rcopytype(_, s): # noqa
     return list if lib.Rf_isNull(getnames_p(s)) else OrderedDict
 
 
-@dispatch(datatype(default), BUILTINSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), BUILTINSXP)
+def rcopytype(_, s): # noqa
     return FunctionType
 
 
-@dispatch(datatype(default), CLOSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), CLOSXP)
+def rcopytype(_, s): # noqa
     return FunctionType
 
 
-@dispatch(datatype(default), EXTPTRSXP)  # noqa
-def rcopytype(_, s):
+@dispatch(datatype(default), EXTPTRSXP)
+def rcopytype(_, s): # noqa
     return RObject
 
 
-@dispatch(object, SEXP)  # noqa
-def rcopytype(_, s):
+@dispatch(object, SEXP)
+def rcopytype(_, s): # noqa
     return RObject
 
 
 # Py to R
 
+@contextmanager
+def sexp_context(**kwargs):
+    old_context = sexp_context.context.copy()
+    sexp_context.context.update(kwargs)
+    yield sexp_context.context
+    sexp_context.context = old_context
+
+
+sexp_context.context = {}
 
-# python to r conversions
 
 def robject(*args, **kwargs):
     ensure_initialized()
-    if len(args) == 2 and isinstance(args[0], string_types):
-        return RObject(sexp(RClass(args[0]), args[1], **kwargs))
-    elif len(args) == 1:
-        return RObject(sexp(args[0], **kwargs))
-    else:
-        raise TypeError("wrong number of arguments or argument types")
+    with sexp_context(**kwargs):
+        if len(args) == 2 and isinstance(args[0], string_types):
+            return RObject(sexp(RClass(args[0]), args[1]))
+        elif len(args) == 1:
+            return RObject(sexp(args[0]))
+        else:
+            raise TypeError("wrong number of arguments or argument types")
 
 
-@dispatch(datatype(RClass("NULL")), type(None))  # noqa
-def sexp(_, n):
+@dispatch(datatype(RClass("NULL")), type(None))
+def sexp(_, n): # noqa
     return lib.R_NilValue
 
 
-@dispatch(datatype(RClass("logical")), bool)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("logical")), bool)
+def sexp(_, s): # noqa
     return rlogical_p(s)
 
 
-@dispatch(datatype(RClass("integer")), int)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("integer")), int)
+def sexp(_, s): # noqa
     return rint_p(s)
 
 
-@dispatch(datatype(RClass("numeric")), float)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("numeric")), float)
+def sexp(_, s): # noqa
     return rdouble_p(s)
 
 
-@dispatch(datatype(RClass("complex")), complex)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("complex")), complex)
+def sexp(_, s): # noqa
     c = ffi.new("Rcomplex*")
     c.r = s.real
     c.i = s.imag
     return lib.Rf_ScalarComplex(c[0])
 
 
-@dispatch(datatype(RClass("character")), string_types)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("character")), string_types)
+def sexp(_, s): # noqa
     return rstring_p(s)
 
 
 if sys.version >= "3":
-    @dispatch(datatype(RClass("raw")), bytes)  # noqa
-    def sexp(_, s):
+    @dispatch(datatype(RClass("raw")), bytes)
+    def sexp(_, s): # noqa
         n = len(s)
         x = lib.Rf_allocVector(lib.RAWSXP, n)
         with protected(x):
             p = lib.RAW(x)
             for i in range(n):
                 p[i] = s[i]
         return x
 else:
-    @dispatch(datatype(RClass("raw")), bytes)  # noqa
-    def sexp(_, s):
+    @dispatch(datatype(RClass("raw")), bytes)
+    def sexp(_, s): # noqa
         n = len(s)
         x = lib.Rf_allocVector(lib.RAWSXP, n)
         with protected(x):
             p = lib.RAW(x)
             for i in range(n):
                 p[i] = ord(s[i])
         return x
 
 
-@dispatch(datatype(RClass("logical")), list)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("logical")), list)
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.LGLSXP, n)
     with protected(x):
         p = lib.LOGICAL(x)
         for i in range(n):
             p[i] = s[i]
     return x
 
 
-@dispatch(datatype(RClass("integer")), list)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("integer")), list)
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.INTSXP, n)
     with protected(x):
         p = lib.INTEGER(x)
         for i in range(n):
             p[i] = s[i]
     return x
 
 
-@dispatch(datatype(RClass("numeric")), list)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("numeric")), list)
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.REALSXP, n)
     with protected(x):
         p = lib.REAL(x)
         for i in range(n):
             p[i] = s[i]
     return x
 
 
-@dispatch(datatype(RClass("complex")), list)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("complex")), list)
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.CPLXSXP, n)
     with protected(x):
         p = lib.COMPLEX(x)
         for i in range(n):
             p[i].r = s[i].real
             p[i].i = s[i].imag
     return x
 
 
-@dispatch(datatype(RClass("character")), list)  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("character")), list)
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.STRSXP, n)
     with protected(x):
         for i in range(n):
             isascii = all(ord(c) < 128 for c in s[i])
-            b = s[i].encode("utf-8")
+            b = s[i].encode('utf-8')
             lib.SET_STRING_ELT(x, i, lib.Rf_mkCharLenCE(b, len(b), 0 if isascii else 1))
     return x
 
 
-
-@dispatch(datatype(RClass("list")), (list, tuple))  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("list")), (list, tuple))
+def sexp(_, s): # noqa
     n = len(s)
     x = lib.Rf_allocVector(lib.VECSXP, n)
     with protected(x):
         for i in range(n):
             lib.SET_VECTOR_ELT(x, i, sexp(s[i]))
     return x
 
 
-@dispatch(datatype(RClass("list")), (dict, OrderedDict))  # noqa
-def sexp(_, s):
+@dispatch(datatype(RClass("list")), (dict, OrderedDict))
+def sexp(_, s): # noqa
     v = sexp(RClass("list"), list(s.values()))
     with protected(v):
         k = sexp(RClass("character"), list(s.keys()))
         with protected(k):
             lib.Rf_setAttrib(v, lib.R_NamesSymbol, k)
     return v
 
@@ -753,23 +825,27 @@
     s = lib.Rf_list1(lib.R_MissingArg)
     with protected(s):
         lib.SET_TAG(s, lib.R_DotsSymbol)
     return s
 
 
 def sexp_as_py_object(obj):
-    if callable(obj):
+    if isinstance(obj, SEXP):
+        return obj
+    elif isinstance(obj, RObject):
+        return unbox(obj)
+    elif callable(obj):
         return sexp(RClass("PyCallable"), obj)
     else:
         return sexp(RClass("PyObject"), obj)
 
 
 def on_xptr_callback_error(exception, exc_value, traceback):
     lib.xptr_callback_error_occured = 1
-    lib.xptr_callback_error_message = str(exc_value)[0:100].encode("utf-8")
+    lib.xptr_callback_error_message = utf8tosystem(str(exc_value)[0:100])
 
 
 @ffi.def_extern(error=ffi.NULL, onerror=on_xptr_callback_error)
 def xptr_callback(exptr, arglist, asis, convert):
     asis = rcopy(bool, asis)
     convert = rcopy(bool, convert)
     f = from_xptr(exptr)
@@ -785,120 +861,166 @@
         else:
             if names and names[i]:
                 kwargs[names[i]] = rcopy(lib.VECTOR_ELT(arglist, i))
             else:
                 args.append(rcopy(lib.VECTOR_ELT(arglist, i)))
 
     ret = f(*args, **kwargs)
-    return sexp(ret) if convert else sexp_as_py_object(ret)
+    with sexp_context(asis=asis, convert=convert):
+        return sexp(ret) if convert else sexp_as_py_object(ret)
 
 
-@dispatch(datatype(RClass("function")), Callable)  # noqa
-def sexp(_, f, invisible=False, asis=False, convert=True):
-    fextptr = new_xptr(f)
-    dotlist = rlang("list", lib.R_DotsSymbol)
-    body = rlang(
-        ".Call", rstring("_libR_xptr_callback"), fextptr, dotlist,
-        rlogical(asis), rlogical(convert))
-    if invisible:
-        body = rlang("invisible", body)
-    lang = rlang_p(rsym("function"), sexp_dots(), body)
-    status = ffi.new("int[1]")
-    val = lib.R_tryEval(lang, lib.R_GlobalEnv, status)
-    return val
+@dispatch(datatype(RClass("function")), Callable)
+def sexp(_, f): # noqa
+    if hasattr(f, "__robject__"):
+        # R function wrapped by python function
+        return unbox(f.__robject__)
+
+    with sexp_context() as context:
+        nprotect = 0
+        invisible = context.get('invisible', False)
+        env = new_env_p()
+        lib.Rf_protect(env)
+        nprotect += 1
+        fp = new_xptr_p(f)
+        lib.Rf_protect(fp)
+        nprotect += 1
+        setclass(fp, "PyObject")
+
+        lib.Rf_defineVar(rsym_p("pointer"), fp, env)
+        dotlist = rlang("list", lib.R_DotsSymbol)
+        xptr_callback = rstring_p("_libR_xptr_callback")
+        lib.Rf_protect(xptr_callback)
+        nprotect += 1
+        body = rlang_p(
+            ".Call",
+            xptr_callback,
+            rsym_p("pointer"),
+            dotlist,
+            rlogical(context.get("asis", False)),
+            rlogical(context.get("convert", True)))
+        lib.Rf_protect(body)
+        nprotect += 1
+        if invisible:
+            body = rlang_p("invisible", body)
+            lib.Rf_protect(body)
+            nprotect += 1
+
+        lang = rlang_p(rsym_p("function"), sexp_dots(), body)
+        lib.Rf_protect(lang)
+        nprotect += 1
 
+        status = ffi.new("int[1]")
+        val = lib.R_tryEval(lang, env, status)
+        lib.Rf_protect(val)
+        nprotect += 1
+        setattrib(val, "py_object", fp)
+        lib.Rf_unprotect(nprotect)
+        return val
 
-@dispatch(datatype(RClass("PyObject")), object)  # noqa
-def sexp(_, s):
+
+@dispatch(datatype(RClass("PyObject")), object)
+def sexp(_, s): # noqa
     if (isinstance(s, RObject) or isinstance(s, SEXP)) and "PyObject" in rclass(s):
         return unbox(s)
     p = new_xptr_p(s)
-    setclass(p, "PyObject")
+    with protected(p):
+        setclass(p, "PyObject")
+        with sexp_context() as context:
+            setattrib(p, "convert", sexp(context.get('convert', True)))
     return p
 
 
-@dispatch(datatype(RClass("PyCallable")), Callable)  # noqa
-def sexp(_, f, invisible=False, asis=False, convert=True):
-    p = sexp(RClass("function"), f, invisible=invisible, asis=asis, convert=convert)
-    setattrib(p, "py_object", sexp(RClass("PyObject"), f))
-    setclass(p, ["PyCallable", "PyObject"])
+@dispatch(datatype(RClass("PyCallable")), Callable)
+def sexp(_, f): # noqa
+    with sexp_context() as context:
+        asis = context.get("asis", False)
+        convert = context.get("convert", False)
+        with sexp_context(asis=asis, convert=convert):
+            p = sexp(RClass("function"), f)
+            lib.Rf_protect(p)
+            setclass(p, ["PyCallable", "PyObject"])
+            lib.Rf_unprotect(1)
     return p
 
 
 # default conversions
 
 
-@dispatch(type(None))  # noqa
-def sexp(n):
+@dispatch(type(None))
+def sexp(n): # noqa
     return lib.R_NilValue
 
 
-@dispatch(SEXP)  # noqa
-def sexp(x):
+@dispatch(SEXP)
+def sexp(x):  # noqa
     return x
 
 
-@dispatch(RObject)  # noqa
-def sexp(r):
+@dispatch(RObject)
+def sexp(r): # noqa
     return unbox(r)
 
 
-@dispatch(object)  # noqa
-def sexp(s, **kwargs):
+@dispatch(object)
+def sexp(s): # noqa
     rcls = sexpclass(s)
-    return sexp(RClass(rcls), s, **kwargs)
+    return sexp(RClass(rcls), s)
 
 
-@dispatch(bool)  # noqa
-def sexpclass(s):
+@dispatch(bool)
+def sexpclass(s): # noqa
     return "logical"
 
 
-@dispatch(int)  # noqa
-def sexpclass(s):
+@dispatch(int)
+def sexpclass(s): # noqa
     return "integer"
 
 
-@dispatch(float)  # noqa
-def sexpclass(s):
+@dispatch(float)
+def sexpclass(s): # noqa
     return "numeric"
 
 
-@dispatch(complex)  # noqa
-def sexpclass(s):
+@dispatch(complex)
+def sexpclass(s): # noqa
     return "complex"
 
 
-@dispatch(string_types)  # noqa
-def sexpclass(s):
+@dispatch(string_types)
+def sexpclass(s): # noqa
     return "character"
 
 
-@dispatch(list)  # noqa
-def sexpclass(s):
+@dispatch(list)
+def sexpclass(s): # noqa
     if all(isinstance(x, bool) for x in s):
         return "logical"
     elif all(isinstance(x, int) for x in s):
         return "integer"
     elif all(isinstance(x, float) for x in s):
         return "numeric"
     elif all(isinstance(x, complex) for x in s):
         return "complex"
     elif all(isinstance(x, string_types) for x in s):
         return "character"
 
     return "list"
 
 
-@dispatch((tuple, dict, OrderedDict))  # noqa
-def sexpclass(s):
+@dispatch((tuple, dict, OrderedDict))
+def sexpclass(s): # noqa
     return "list"
 
 
-@dispatch(Callable)  # noqa
-def sexpclass(f):
-    return "PyCallable"
+@dispatch(Callable)
+def sexpclass(f): # noqa
+    if hasattr(f, "__robject__"):
+        return "function"
+    else:
+        return "PyCallable"
 
 
-@dispatch(object)  # noqa
-def sexpclass(f):
+@dispatch(object)
+def sexpclass(f): # noqa
     return "PyObject"
```

### Comparing `rchitect-0.3.9/rchitect/py_config.py` & `rchitect-0.4.1/rchitect/reticulate/py_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,21 @@
     libdl.dladdr.argtypes = (ctypes.c_void_p, ctypes.POINTER(Dl_info))
     info = Dl_info()
     libdl.dladdr(libc.Py_IsInitialized, ctypes.byref(info))
 
     python = sys.executable
     libpython = info.dli_fname.decode()
 
-    lib = ctypes.PyDLL(libpython)
-    if lib.Py_IsInitialized() == 0:
+    try:
+        lib = ctypes.PyDLL(libpython)
+    except OSError:
         libpython = ""
+    else:
+        if lib.Py_IsInitialized() == 0:
+            libpython = ""
 
     try:
         import sysconfig
         pythonhome = sysconfig.get_config_vars('prefix')[0] + ":" + \
             sysconfig.get_config_vars('exec_prefix')[0]
     except Exception:
         pythonhome = None
```

### Comparing `rchitect-0.3.9/rchitect/repl.py` & `rchitect-0.4.1/rchitect/repl.py`

 * *Files identical despite different names*

### Comparing `rchitect-0.3.9/rchitect/src/R.h` & `rchitect-0.4.1/rchitect/src/R.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #ifndef LIBR
 #define RAPI_EXTERN extern
 #else
 #define RAPI_EXTERN
 #endif
 
 // begin cdef
-RAPI_EXTERN int R_MAJOR;
-
 typedef unsigned char Rbyte;
 
 typedef enum {Bytes, Chars, Width} nchar_type;
 typedef void * (*DL_FUNC)();
 
 typedef int R_len_t;
 
@@ -390,14 +388,24 @@
 
 RAPI_EXTERN void (*R_RegisterFinalizer)(SEXP s, SEXP fun);
 RAPI_EXTERN void (*R_RegisterCFinalizer)(SEXP s, R_CFinalizer_t fun);
 RAPI_EXTERN void (*R_RegisterFinalizerEx)(SEXP s, SEXP fun, Rboolean onexit);
 RAPI_EXTERN void (*R_RegisterCFinalizerEx)(SEXP s, R_CFinalizer_t fun, Rboolean onexit);
 RAPI_EXTERN void (*R_RunPendingFinalizers)(void);
 
+RAPI_EXTERN SEXP (*R_MakeWeakRef)(SEXP key, SEXP val, SEXP fin, Rboolean onexit);
+RAPI_EXTERN SEXP (*R_MakeWeakRefC)(SEXP key, SEXP val, R_CFinalizer_t fin, Rboolean onexit);
+RAPI_EXTERN SEXP (*R_WeakRefKey)(SEXP w);
+RAPI_EXTERN SEXP (*R_WeakRefValue)(SEXP w);
+RAPI_EXTERN void (*R_RunWeakRefFinalizer)(SEXP w);
+
+RAPI_EXTERN SEXP (*R_PromiseExpr)(SEXP);
+RAPI_EXTERN SEXP (*R_ClosureExpr)(SEXP);
+RAPI_EXTERN SEXP (*R_BytecodeExpr)(SEXP e);
+
 RAPI_EXTERN Rboolean (*R_ToplevelExec)(void (*fun)(void *), void *data);
 RAPI_EXTERN SEXP (*R_tryCatch)(SEXP (*)(void *), void *, SEXP, SEXP (*)(SEXP, void *), void *, void (*)(void *), void *);
 RAPI_EXTERN SEXP (*R_tryCatchError)(SEXP (*)(void *), void *, SEXP (*)(SEXP, void *), void *);
 
 RAPI_EXTERN void (*R_RestoreHashCount)(SEXP rho);
 RAPI_EXTERN Rboolean (*R_IsPackageEnv)(SEXP rho);
 RAPI_EXTERN SEXP (*R_PackageEnvName)(SEXP rho);
@@ -483,19 +491,19 @@
 RAPI_EXTERN R_xlen_t  (*Rf_xlength)(SEXP);
 RAPI_EXTERN R_xlen_t  (*XTRUELENGTH)(SEXP x);
 // RAPI_EXTERN int (*LENGTH_EX)(SEXP x, const char *file, int line);
 // RAPI_EXTERN R_xlen_t (*XLENGTH_EX)(SEXP x);
 
 
 // Arith.h
-RAPI_EXTERN double R_NaN;
-RAPI_EXTERN double R_PosInf;
-RAPI_EXTERN double R_NegInf;
-RAPI_EXTERN double R_NaReal;
-RAPI_EXTERN int    R_NaInt;
+// RAPI_EXTERN double R_NaN;
+// RAPI_EXTERN double R_PosInf;
+// RAPI_EXTERN double R_NegInf;
+// RAPI_EXTERN double R_NaReal;
+// RAPI_EXTERN int    R_NaInt;
 RAPI_EXTERN int (*R_IsNA)(double);
 RAPI_EXTERN int (*R_IsNaN)(double);
 RAPI_EXTERN int (*R_finite)(double);
 
 
 // Parse.h
 typedef enum {
@@ -540,14 +548,15 @@
 // RAPI_EXTERN double (*Rf_RealFromComplex)(Rcomplex, int*);
 // RAPI_EXTERN Rcomplex (*Rf_ComplexFromLogical)(int, int*);
 // RAPI_EXTERN Rcomplex (*Rf_ComplexFromInteger)(int, int*);
 // RAPI_EXTERN Rcomplex (*Rf_ComplexFromReal)(double, int*);
 
 RAPI_EXTERN void (*R_ProcessEvents)(void);
 
+RAPI_EXTERN SEXP (*Rf_NewEnvironment)(SEXP, SEXP, SEXP);
 // RAPI_EXTERN void (*Rf_PrintVersion)(char *, size_t len);
 // RAPI_EXTERN void (*Rf_PrintVersion_part_1)(char *, size_t len);
 // RAPI_EXTERN void (*Rf_PrintVersionString)(char *, size_t len);
 RAPI_EXTERN SEXP (*R_data_class)(SEXP , Rboolean);
 
 // Utils.h
 RAPI_EXTERN void (*R_CheckUserInterrupt)(void);
@@ -588,14 +597,15 @@
 RAPI_EXTERN void (*R_DefParams)(Rstart);
 RAPI_EXTERN void (*R_SetParams)(Rstart);
 RAPI_EXTERN void (*R_set_command_line_arguments)(int argc, char **argv);
 
 // Rinterface.h
 
 RAPI_EXTERN int (*Rstd_CleanUp)(int saveact, int status, int RunLast);
+RAPI_EXTERN int *R_SignalHandlers_t;
 
 
 // Rembedded.h
 RAPI_EXTERN int (*Rf_initialize_R)(int ac, char **av);
 RAPI_EXTERN void (*setup_Rmainloop)(void);
 RAPI_EXTERN void (*_run_Rmainloop)(void);
 
@@ -616,17 +626,23 @@
 // end cdef
 
 
 #ifdef _WIN32
 RAPI_EXTERN char *(*get_R_HOME)(void);
 RAPI_EXTERN char *(*getRUser)(void);
 RAPI_EXTERN int* UserBreak_t;
+RAPI_EXTERN int* CharacterMode_t;
+RAPI_EXTERN int* EmitEmbeddedUTF8_t;
+RAPI_EXTERN int (*GA_peekevent)(void);
+RAPI_EXTERN int (*GA_initapp)(int, char **);
 #else
 // eventloop.h
-RAPI_EXTERN void* (*R_InputHandlers);
+RAPI_EXTERN void* R_InputHandlers;
+RAPI_EXTERN void (**R_PolledEvents_t)(void);
+
 RAPI_EXTERN void* (*R_checkActivity)(int usec, int ignore_stdin);
 RAPI_EXTERN void (*R_runHandlers)(void* handlers, void* mask);
 
 RAPI_EXTERN int* R_interrupts_pending_t;
 #endif
 
 #endif /* end of include guard: R_H__ */
```

### Comparing `rchitect-0.3.9/rchitect/src/build.py` & `rchitect-0.4.1/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import os
 import re
 import sys
 from cffi import FFI
 ffibuilder = FFI()
 
-cwd = os.path.dirname(os.path.realpath(__file__))
+# cwd = os.path.dirname(os.path.realpath(__file__))
 cdef_pattern = re.compile("// begin cdef([^$]*)// end cdef")
 cb_cdef_pattern = re.compile("// begin cb cdef([^$]*)// end cb cdef")
 
 
-for header_file in ["R.h", "libR.h", "gli.h", "parse.h", "process_events.h"]:
-    with open(os.path.join(cwd, header_file), "r") as f:
+for header_file in ["R.h", "libR.h", "gil.h", "parse.h", "process_events.h"]:
+    with open(os.path.join("rchitect", "src", header_file), "r") as f:
         m = cdef_pattern.search(f.read(), re.M)
-        ffibuilder.cdef(m.group(1).replace("RAPI_EXTERN", ""))
+        ffibuilder.cdef(m.group(1).replace("RAPI_EXTERN", "extern"))
 
 if sys.platform.startswith("win"):
     ffibuilder.cdef("""
-        char *(*get_R_HOME)(void);
-        char *(*getRUser)(void);
-        int* UserBreak_t;
+        extern char *(*get_R_HOME)(void);
+        extern char *(*getRUser)(void);
+        extern int* UserBreak_t;
+        extern int* CharacterMode_t;
+        extern int* EmitEmbeddedUTF8_t;
+        extern int (*GA_peekevent)(void);
+        extern int (*GA_initapp)(int, char **);
     """)
 else:
     ffibuilder.cdef("""
-        void* (*R_InputHandlers);
-        void* (*R_checkActivity)(int usec, int ignore_stdin);
-        void (*R_runHandlers)(void* handlers, void* mask);
-        int* R_interrupts_pending_t;
+        extern void* (*R_InputHandlers);
+        extern void (**R_PolledEvents_t)(void);
+        extern void* (*R_checkActivity)(int usec, int ignore_stdin);
+        extern void (*R_runHandlers)(void* handlers, void* mask);
+        extern int* R_interrupts_pending_t;
     """)
 
-with open(os.path.join(cwd, "libR.h"), "r") as f:
+with open(os.path.join("rchitect", "src", "libR.h"), "r") as f:
     m = cb_cdef_pattern.search(f.read(), re.M)
     ffibuilder.cdef("""
         extern "Python+C" {{
             {}
         }}
     """.format(m.group(1)))
 
 ffibuilder.set_source(
     "rchitect._cffi",
     """
-    # include "gli.h"
+    # include "gil.h"
     # include "libR.h"
     # include "parse.h"
     # include "process_events.h"
     """,
     include_dirs=['rchitect/src'],
     sources=[
         'rchitect/src/libR.c',
-        'rchitect/src/gli.c',
+        'rchitect/src/gil.c',
         'rchitect/src/parse.c',
         'rchitect/src/process_events.c'
     ])
 
 if __name__ == "__main__":
     ffibuilder.compile(verbose=True)
```

### Comparing `rchitect-0.3.9/rchitect/src/libR.h` & `rchitect-0.4.1/rchitect/src/libR.h`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 #else
 #define WIN32_LEAN_AND_MEAN 1
 #include <windows.h>
 #endif
 
 // begin cdef
 
+extern int cb_interrupted;
+
 char* _libR_last_loaded_symbol(void);
 char* _libR_dl_error_message(void);
-int _libR_load(const char* libpath);
+int _libR_load(const char* rhome);
 int _libR_is_initialized(void);
 int _libR_load_symbols(void);
 int _libR_load_constants(void);
 void _libR_set_callback(char* name, void* cb);
 
 int cb_read_console_interruptible(const char *, unsigned char *, int, int);
-extern int cb_read_console_interrupted;
 
+void cb_polled_events_interruptible();
+
+void cb_write_console_safe(const char *, int, int);
+void cb_busy_safe(int);
 
 void _libR_setup_xptr_callback();
 SEXP _libR_xptr_callback(SEXP, SEXP, SEXP, SEXP);
 extern int xptr_callback_error_occured;
 extern char xptr_callback_error_message[100];
 
 // end cdef
@@ -59,11 +64,12 @@
 SEXP cb_do_dataentry(SEXP, SEXP, SEXP, SEXP);
 SEXP cb_do_dataviewer(SEXP, SEXP, SEXP, SEXP);
 void cb_process_events();
 void cb_polled_events();
 int  cb_yes_no_cancel(const char *s);
 
 SEXP xptr_callback(SEXP, SEXP, SEXP, SEXP);
+void xptr_finalizer(SEXP);
 
 // end cb cdef
 
 #endif /* end of include guard: LIBR_H__ */
```

### Comparing `rchitect-0.3.9/rchitect/src/parse.c` & `rchitect-0.4.1/rchitect/src/parse.c`

 * *Files identical despite different names*

### Comparing `rchitect-0.3.9/rchitect/types.py` & `rchitect-0.4.1/rchitect/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,23 +105,29 @@
     def __del__(self):
         try:
             # it might cause AttributeError when the program exits
             lib.R_ReleaseObject(self.s)
         except AttributeError:
             pass
 
+    def __repr__(self):
+        pass
+
+    def __call__(self, *args, **kwargs):
+        pass
+
 
 class RClass(object):
     _rclasses = {}
 
     def __new__(cls, rcls):
         try:
             return cls._rclasses[rcls]
         except KeyError:
-            T = type(str("RClass_" + rcls), (RClass,), {"__new__": lambda cls: None})
+            T = type(str("RClass_" + rcls), (RClass,), {"__new__": (lambda cls: None)})
             cls._rclasses[rcls] = T
             return T
 
 
 class datatype(type):
     """
     We introduce a `datatype` function to allow different values from `datatype(str)` and
@@ -135,15 +141,15 @@
             t = args[0]
             try:
                 return cls._datatypes[t]
             except KeyError:
                 T = datatype(
                     str("datatype_{}".format(t.__name__)),
                     (type,),
-                    {"t": t, "__new__": lambda cls: cls.t})
+                    {"t": t, "__new__": (lambda cls: cls.t)})
                 cls._datatypes[t] = T
                 return T
         else:
             return super(datatype, cls).__new__(cls, *args)
 
     def __instancecheck__(self, instance):
         return self.t == instance
```

### Comparing `rchitect-0.3.9/rchitect/utils.py` & `rchitect-0.4.1/rchitect/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,206 @@
 from __future__ import unicode_literals
 import os
 import re
 import subprocess
 import sys
 import ctypes
+import locale
 from distutils.version import LooseVersion
-
+if sys.version_info[0] >= 3:
+    from shutil import which
+else:
+    from backports.shutil_which import which
 
 if sys.platform.startswith('win'):
     if sys.version_info[0] >= 3:
         from winreg import OpenKey, QueryValueEx, HKEY_LOCAL_MACHINE, KEY_READ
     else:
         from _winreg import OpenKey, QueryValueEx, HKEY_LOCAL_MACHINE, KEY_READ
 
 
 def read_registry(key, valueex):
     reg_key = OpenKey(HKEY_LOCAL_MACHINE, key, 0, KEY_READ)
     return QueryValueEx(reg_key, valueex)
 
 
-def Rhome():
-    if 'R_HOME' not in os.environ:
-        try:
-            rhome = system2utf8(subprocess.check_output(["R", "RHOME"])).strip()
-        except Exception:
-            rhome = ""
-        try:
-            if sys.platform.startswith("win") and not rhome:
-                rhome = read_registry("Software\\R-Core\\R", "InstallPath")[0]
-        except Exception:
-            rhome = ""
+def getRhome(path, throw=False):
+    rhome = ""
 
-        if rhome:
-            os.environ['R_HOME'] = rhome
-    else:
-        rhome = os.environ['R_HOME']
+    if sys.platform.startswith("win") and path and not path.endswith(".exe"):
+        path = path + ".exe"
+
+    if not which(path):
+        return None
+    try:
+        rhome = subprocess.check_output([path, "RHOME"]).decode("utf-8").strip()
+    except Exception:
+        rhome = None
 
     return rhome
 
 
-def libRpath(rhome):
+def verify_Rhome(rhome):
     if sys.platform.startswith("win"):
         path = os.path.join(rhome, "bin", "x64" if sys.maxsize > 2**32 else "i386", "R.dll")
     elif sys.platform == "darwin":
         path = os.path.join(rhome, "lib", "libR.dylib")
     else:
         path = os.path.join(rhome, "lib", "libR.so")
 
     if not os.path.exists(path):
-        raise RuntimeError("Cannot locate R share library.")
+        if sys.platform.startswith("win"):
+            another_path = os.path.join(
+                rhome, "bin", "i386" if sys.maxsize > 2**32 else "x64", "R.dll")
+            if os.path.exists(another_path):
+                raise RuntimeError("R and python architectures do not match.")
+        raise RuntimeError("R share library ({}) does not exist.".format(path))
+
+
+def Rhome():
+    rhome = None
+
+    if 'R_BINARY' in os.environ:
+        rhome = getRhome(os.environ['R_BINARY'], throw=True)
+        if not rhome:
+            raise RuntimeError("R binary ({}) does not exist.".format(os.environ['R_BINARY']))
+
+    if not rhome and 'R_HOME' in os.environ:
+        rhome = os.environ['R_HOME']
+        if not os.path.isdir(rhome):
+            raise RuntimeError("R_HOME ({}) does not exist.".format(rhome))
+        return rhome
+
+    if not rhome:
+        rhome = getRhome("R")
 
-    return path
+    try:
+        if sys.platform.startswith("win") and not rhome:
+            rhome = read_registry("Software\\R-Core\\R", "InstallPath")[0]
+    except Exception:
+        rhome = ""
+
+    if rhome:
+        os.environ['R_HOME'] = rhome
+    else:
+        raise RuntimeError("Cannot determine R HOME.")
+
+    verify_Rhome(rhome)
+
+    return rhome
 
 
 def ensure_path(rhome=None):
     if not rhome:
         rhome = Rhome()
     if sys.platform.startswith("win"):
         libRdir = os.path.join(rhome, "bin", "x64" if sys.maxsize > 2**32 else "i386")
 
         # make sure Rblas.dll can be reached
         try:
             msvcrt = ctypes.cdll.msvcrt
-            msvcrt.getenv.restype = ctypes.c_char_p
-            path = system2utf8(msvcrt.getenv("PATH".encode()))
+            msvcrt._wgetenv.restype = ctypes.c_wchar_p
+            path = msvcrt._wgetenv(ctypes.c_wchar_p("PATH"))
             if libRdir not in path:
                 path = libRdir + ";" + path
-                msvcrt._putenv(utf8tosystem("PATH={}".format(path)))
+                msvcrt._wputenv(ctypes.c_wchar_p("PATH={}".format(path)))
         except Exception as e:
             print(e)
             pass
 
 
-R_RELEASE = re.compile(r"R version ([0-9]+\.[0-9]+\.[0-9]+)")
-R_DEVEL = re.compile(r"R Under development \(unstable\) \(([^)]*)\)")
-
-
 def rversion(rhome=None):
     if not rhome:
         rhome = Rhome()
     try:
-        output = system2utf8(subprocess.check_output(
-            [os.path.join(rhome, "bin", "R"), "--version"],
-            stderr=subprocess.STDOUT)).strip()
-        m = R_RELEASE.match(output)
-        if not m:
-            m = R_DEVEL.match(output)
-        version = LooseVersion(m.group(1))
+        output = subprocess.check_output(
+            [os.path.join(rhome, "bin", "R"), "--slave", "-e", "cat(as.character(getRversion()))"],
+            stderr=subprocess.STDOUT).decode("utf-8").strip()
+        version = LooseVersion(output)
     except Exception:
         version = LooseVersion("1000.0.0")
     return version
 
 
-UTFPATTERN = re.compile(b"\x02\xff\xfe(.*?)\x03\xff\xfe")
+UTFPATTERN = re.compile(b"\x02\xff\xfe(.*?)\x03\xff\xfe", re.S)
+if sys.version_info[0] >= 3:
+    DECODE_ERROR_HANDLER = "backslashreplace"
+else:
+    DECODE_ERROR_HANDLER = "replace"
 
 
 def rconsole2str(buf):
     ret = ""
     m = UTFPATTERN.search(buf)
     while m:
         a, b = m.span()
-        ret += system2utf8(buf[:a]) + m.group(1).decode("utf-8", "backslashreplace")
+        ret += system2utf8(buf[:a]) + m.group(1).decode("utf-8", DECODE_ERROR_HANDLER)
         buf = buf[b:]
         m = UTFPATTERN.search(buf)
     ret += system2utf8(buf)
     return ret
 
 
 if sys.platform == "win32":
+    """
+    The following only works after setlocale in C and
+    R will initialize it for us. To mimic the behaviour, consider
+    ```
+    ctypes.cdll.msvcrt.setlocale(0, ctypes.c_char_p("chinese-traditional"))
+    ```
+    """
+
     mbtowc = ctypes.cdll.msvcrt.mbtowc
     mbtowc.argtypes = [
         ctypes.POINTER(ctypes.c_wchar),
         ctypes.POINTER(ctypes.c_char),
         ctypes.c_size_t]
     mbtowc.restype = ctypes.c_int
 
     wctomb = ctypes.cdll.msvcrt.wctomb
     wctomb.argtypes = [ctypes.POINTER(ctypes.c_char), ctypes.c_wchar]
     wctomb.restype = ctypes.c_int
 
     def system2utf8(buf):
+        loc = locale.getlocale()
+        if loc[1] == "UTF-8" or loc[1] == "utf8" or loc[1] == "65001":
+            return buf.decode("utf-8", DECODE_ERROR_HANDLER)
+
         wcbuf = ctypes.create_unicode_buffer(1)
         text = ""
         while buf:
             n = mbtowc(wcbuf, buf, len(buf))
             if n <= 0:
                 break
             text += wcbuf[0]
             buf = buf[n:]
         return text
 
     def utf8tosystem(text):
+        loc = locale.getlocale()
+        if loc[1] == "UTF-8" or loc[1] == "utf8" or loc[1] == "65001":
+            return text.encode("utf-8", "backslashreplace")
+
         s = ctypes.create_string_buffer(10)
         buf = b""
         for c in text:
-            n = wctomb(s, c)
+            try:
+                n = wctomb(s, c)
+            except Exception:
+                n = -1
+
             if n > 0:
                 buf += s[:n]
             else:
                 buf += "\\u{{{}}}".format(hex(ord(c))[2:]).encode("ascii")
         return buf
 
 else:
     def system2utf8(buf):
-        return buf.decode("utf-8", "backslashreplace")
+        return buf.decode("utf-8", DECODE_ERROR_HANDLER)
 
     def utf8tosystem(text):
         return text.encode("utf-8", "backslashreplace")
 
 
 def id_str(x):
     return str(id(x))
-
-
-def identity(x):
-    return x
```

### Comparing `rchitect-0.3.9/rchitect/xptr.py` & `rchitect-0.4.1/rchitect/xptr.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from rchitect._cffi import ffi, lib
 from .types import box, unbox
 
 
 _global_set = dict()
 
 
-@ffi.callback("void(SEXP)")
-def finalizer(s):
+@ffi.def_extern()
+def xptr_finalizer(s):
     h = lib.R_ExternalPtrAddr(s)
     del _global_set[h]
 
 
 def new_xptr_p(x):
     h = ffi.new_handle(x)
     hp = ffi.cast("void*", h)
     _global_set[hp] = h
     s = lib.R_MakeExternalPtr(hp, lib.R_NilValue, lib.R_NilValue)
-    lib.R_RegisterCFinalizerEx(s, finalizer, 1)
+    lib.Rf_protect(s)
+    lib.R_RegisterCFinalizerEx(s, ffi.addressof(lib, "xptr_finalizer"), 1)
+    lib.Rf_unprotect(1)
     return s
 
 
 def new_xptr(x):
     return box(new_xptr_p(x))
```

### Comparing `rchitect-0.3.9/rchitect.egg-info/PKG-INFO` & `rchitect-0.4.1/rchitect.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rchitect
-Version: 0.3.9
+Version: 0.4.1
 Summary: Mapping R API to Python
 Home-page: https://github.com/randy3k/rchitect
 Author: Randy Lai
 Author-email: randy.cs.lai@gmail.com
 License: UNKNOWN
 Description: # Interoperate R with Python
         
-        [![CircleCI](https://circleci.com/gh/randy3k/rchitect/tree/master.svg?style=shield)](https://circleci.com/gh/randy3k/rchitect/tree/master)
-        [![Build status](https://ci.appveyor.com/api/projects/status/4o9m8q61m755xc2a/branch/master?svg=true)](https://ci.appveyor.com/project/randy3k/rchitect/branch/master)
+        [![Main](https://github.com/randy3k/rchitect/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/rchitect/actions/workflows/main.yml)
         [![codecov](https://codecov.io/gh/randy3k/rchitect/branch/master/graph/badge.svg)](https://codecov.io/gh/randy3k/rchitect)
         [![pypi](https://img.shields.io/pypi/v/rchitect.svg)](https://pypi.org/project/rchitect/)
+        [![Conda version](https://img.shields.io/conda/vn/conda-forge/rchitect.svg)](https://anaconda.org/conda-forge/rchitect)
         
         
         ## Installation
         
         ```sh
         # install released version
         pip install -U rchitect
@@ -28,43 +28,45 @@
         
         You may be curious why I reinvented the wheel when there is [`rpy2`](https://github.com/rpy2/rpy2)?
         
         The main reason is to drive [`radian`](https://github.com/randy3k/radian).
         `rpy2` was not suitable because it is missing some key features for running
         the R REPL. Speaking of compatibility, `rchitect` has been thoroughly tested on
         multiple platforms such as Windows, macOS and Linux and we also provide binary
-        wheels for user convenience.
+        wheels for python 3.6+.
         
         ## Getting started
         
         ```py
         from rchitect import *
         a = reval("1:5")     # evaluate an R expression in the global environment
         b = rcopy(a)         # convert any RObject returned by `reval` to its python type
         c = robject(b)       # convert any python object to its R type
         d = rcall("sum", c)  # call an R function. Python objects are converted to RObjects implicitly.
         ```
         
         ## FAQ
         
-        If `rchitect` fails to open the R shared library, user should first
-        try to expose the path to R to the `PATH` vaiable.
+        #### How to switch to a different R or specify the version of R.
         
-        In Linux/macOS, you could also export the environment variable `R_HOME`. For example,
-        ```sh
-        $ export R_HOME=/usr/local/lib/R
-        $ radian
-        ```
-        Sometimes, you may also need to futher specify `LD_LIBRARY_PATH` if R fails to find some shared libraries,
+        There are a few options.
+        
+        - One could expose the path to the R binary in the `PATH` variable
+        - The environment variable `R_BINARY` could also be used to specify the path to R.
+        - The environment variable `R_HOME` could also be used to specify R home directory. Note that it is should be set as the result of `R.home()`, not the directory where `R` is located. For example, in Unix
         ```sh
-        export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:`R RHOME`/lib"
+        $ env R_HOME=/usr/local/lib/R radian
         ```
         
+        #### Cannot find shared library
+        
         Please also make sure that R was installed with the R shared library `libR.so` or `libR.dylib` or `libR.dll`. On Linux, the flag `--enable-R-shlib` may be needed to install R from the source.
         
+        
         ## Wiki
         
         [reticulate](https://github.com/randy3k/rchitect/wiki/Conversions-between-reticulate-and-rchitect-objects-are-seamless) conversions
         
 Platform: UNKNOWN
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `rchitect-0.3.9/rchitect.egg-info/SOURCES.txt` & `rchitect-0.4.1/rchitect.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+LICENSE
+MANIFEST.in
 README.md
+build.py
 setup.cfg
 setup.py
 rchitect/__init__.py
 rchitect/callbacks.py
 rchitect/completion.py
 rchitect/console.py
 rchitect/dispatch.py
 rchitect/interface.py
-rchitect/py_config.py
 rchitect/py_tools.py
 rchitect/repl.py
 rchitect/setup.py
 rchitect/types.py
 rchitect/utils.py
 rchitect/xptr.py
 rchitect.egg-info/PKG-INFO
 rchitect.egg-info/SOURCES.txt
 rchitect.egg-info/dependency_links.txt
 rchitect.egg-info/requires.txt
 rchitect.egg-info/top_level.txt
 rchitect/reticulate/__init__.py
 rchitect/reticulate/config.R
+rchitect/reticulate/path.py
+rchitect/reticulate/py_config.py
 rchitect/src/R.h
-rchitect/src/build.py
-rchitect/src/gli.c
-rchitect/src/gli.h
+rchitect/src/gil.c
+rchitect/src/gil.h
 rchitect/src/libR.c
 rchitect/src/libR.h
 rchitect/src/parse.c
 rchitect/src/parse.h
 rchitect/src/process_events.c
 rchitect/src/process_events.h
```

### Comparing `rchitect-0.3.9/setup.py` & `rchitect-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import sys
 from setuptools import setup, find_packages
 
 
 def get_long_description():
     with open('README.md', 'rb') as f:
         desc = f.read().decode('utf-8')
 
@@ -16,34 +17,37 @@
     """
     path = os.path.join(os.path.dirname(__file__), package, '__init__.py')
     with open(path, 'rb') as f:
         init_py = f.read().decode('utf-8')
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 
+install_requires = [
+    'cffi>=1.10.0',
+    'six>=1.9.0'
+]
+
 setup(
     name='rchitect',
     author='Randy Lai',
     author_email="randy.cs.lai@gmail.com",
     version=get_version("rchitect"),
     url='https://github.com/randy3k/rchitect',
     description='Mapping R API to Python',
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     packages=find_packages('.', exclude=["tests"]),
     package_data={'rchitect': ['reticulate/*.R', 'src/*']},
-    cffi_modules=["rchitect/src/build.py:ffibuilder"],
+    cffi_modules=["build.py:ffibuilder"],
+    python_requires='>=3.6',
+    install_requires=install_requires,
     setup_requires=[
         'cffi>=1.10.0',
         "pytest-runner"
     ],
-    install_requires=[
-        'cffi>=1.10.0',
-        'six>=1.9.0'
-    ],
     extras_require={
         "test": [
             "pytest",
             "pytest-mock",
             "pytest-cov"
         ]
     }
```

