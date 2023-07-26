# Comparing `tmp/rbi_tree-0.1.5.dev1.tar.gz` & `tmp/rbi_tree-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbi_tree-0.1.5.dev1.tar", last modified: Mon Jun 21 06:01:01 2021, max compression
+gzip compressed data, was "rbi_tree-0.2.tar", last modified: Wed Jul 26 03:54:03 2023, max compression
```

## Comparing `rbi_tree-0.1.5.dev1.tar` & `rbi_tree-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2021-06-21 06:01:01.449551 rbi_tree-0.1.5.dev1/
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1515 2021-06-21 06:01:01.449551 rbi_tree-0.1.5.dev1/PKG-INFO
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1173 2021-03-31 10:28:09.000000 rbi_tree-0.1.5.dev1/README.md
-drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2021-06-21 06:01:01.449551 rbi_tree-0.1.5.dev1/rbi_tree/
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)        0 2020-07-08 06:39:14.000000 rbi_tree-0.1.5.dev1/rbi_tree/__init__.py
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)    29607 2020-07-08 06:39:14.000000 rbi_tree-0.1.5.dev1/rbi_tree/intervaltree.hpp
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)     3691 2021-06-17 11:02:11.000000 rbi_tree-0.1.5.dev1/rbi_tree/test_tree.py
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)   365599 2021-06-21 05:58:56.000000 rbi_tree-0.1.5.dev1/rbi_tree/tree.cpp
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)     8973 2021-06-21 05:58:49.000000 rbi_tree-0.1.5.dev1/rbi_tree/tree.pyx
-drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2021-06-21 06:01:01.449551 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1515 2021-06-21 06:01:01.000000 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/PKG-INFO
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)      419 2021-06-21 06:01:01.000000 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/SOURCES.txt
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)        1 2021-06-21 06:01:01.000000 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/dependency_links.txt
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)        1 2020-07-08 06:46:24.000000 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/not-zip-safe
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)        9 2021-06-21 06:01:01.000000 rbi_tree-0.1.5.dev1/rbi_tree.egg-info/top_level.txt
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)      568 2021-06-21 06:01:01.449551 rbi_tree-0.1.5.dev1/setup.cfg
--rw-r--r--   0 mikpom    (1000) mikpom    (1000)      436 2021-06-21 05:58:49.000000 rbi_tree-0.1.5.dev1/setup.py
+drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2023-07-26 03:54:03.242584 rbi_tree-0.2/
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1485 2023-07-26 03:54:03.243584 rbi_tree-0.2/PKG-INFO
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1173 2021-03-31 10:28:09.000000 rbi_tree-0.2/README.md
+drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2023-07-26 03:54:03.242584 rbi_tree-0.2/rbi_tree/
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)        0 2020-07-08 06:39:14.000000 rbi_tree-0.2/rbi_tree/__init__.py
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)    29607 2020-07-08 06:39:14.000000 rbi_tree-0.2/rbi_tree/intervaltree.hpp
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)     3691 2021-06-17 11:02:11.000000 rbi_tree-0.2/rbi_tree/test_tree.py
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)   557780 2023-07-26 03:54:03.000000 rbi_tree-0.2/rbi_tree/tree.cpp
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)     8942 2023-07-26 03:22:16.000000 rbi_tree-0.2/rbi_tree/tree.pyx
+drwxr-xr-x   0 mikpom    (1000) mikpom    (1000)        0 2023-07-26 03:54:03.242584 rbi_tree-0.2/rbi_tree.egg-info/
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)     1485 2023-07-26 03:54:03.000000 rbi_tree-0.2/rbi_tree.egg-info/PKG-INFO
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)      356 2023-07-26 03:54:03.000000 rbi_tree-0.2/rbi_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)        1 2023-07-26 03:54:03.000000 rbi_tree-0.2/rbi_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)        1 2020-07-08 06:46:24.000000 rbi_tree-0.2/rbi_tree.egg-info/not-zip-safe
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)        9 2023-07-26 03:54:03.000000 rbi_tree-0.2/rbi_tree.egg-info/top_level.txt
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)      558 2023-07-26 03:54:03.243584 rbi_tree-0.2/setup.cfg
+-rw-r--r--   0 mikpom    (1000) mikpom    (1000)      436 2021-06-21 05:58:49.000000 rbi_tree-0.2/setup.py
```

### Comparing `rbi_tree-0.1.5.dev1/PKG-INFO` & `rbi_tree-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rbi_tree
-Version: 0.1.5.dev1
+Version: 0.2
 Summary: Cython-wrapped C++ red-black interval tree implementation
 Home-page: https://github.com/mikpom/rbi_tree
 Author: @mikpom
-Author-email: mikpom@fastmail.com
+Author-email: mikpom@mikpom.ru
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # Interval Tree for Python #
 
 This is a Cython-wrapped red-black interval tree from
 [IvanPinezhaninov/IntervalTree/](https://github.com/IvanPinezhaninov/IntervalTree).
@@ -65,9 +64,7 @@
 []
 >>> t.find_at(70) # search at point
 [(60, 80, 0)]
 >>> list(t.iter_ivl())
 [(60, 80, 0)]
 ```
 
-
-
```

### Comparing `rbi_tree-0.1.5.dev1/README.md` & `rbi_tree-0.2/README.md`

 * *Files identical despite different names*

### Comparing `rbi_tree-0.1.5.dev1/rbi_tree/intervaltree.hpp` & `rbi_tree-0.2/rbi_tree/intervaltree.hpp`

 * *Files identical despite different names*

### Comparing `rbi_tree-0.1.5.dev1/rbi_tree/test_tree.py` & `rbi_tree-0.2/rbi_tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `rbi_tree-0.1.5.dev1/rbi_tree/tree.cpp` & `rbi_tree-0.2/rbi_tree/tree.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.22 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "rbi_tree/intervaltree.hpp"
         ],
@@ -18,29 +18,43 @@
             "/home/mikpom/ownCloud/src/python/lib/rbi_tree/rbi_tree/tree.pyx"
         ]
     },
     "module_name": "rbi_tree.tree"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_22"
-#define CYTHON_HEX_VERSION 0x001D16F0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -51,30 +65,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -91,35 +109,167 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -134,54 +284,55 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -191,35 +342,68 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
-  #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -237,78 +421,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -324,99 +558,233 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return result;
+    }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -439,78 +807,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -531,16 +987,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -551,46 +1013,46 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
-#endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -602,16 +1064,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -626,33 +1090,39 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE__rbi_tree__tree
 #define __PYX_HAVE_API__rbi_tree__tree
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include <utility>
 
-    #if __cplusplus > 199711L
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
     #include <type_traits>
 
     namespace cython_std {
     template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
     template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
     }
 
@@ -726,54 +1196,111 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -787,15 +1314,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -852,31 +1379,32 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "rbi_tree/tree.pyx",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* #### Code section: numeric_typedefs ### */
+/* #### Code section: complex_type_declarations ### */
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8rbi_tree_4tree_ITree;
 struct __pyx_obj_8rbi_tree_4tree_ITreed;
 struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl;
 struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl;
 
@@ -943,32 +1471,32 @@
  */
 struct __pyx_obj_8rbi_tree_4tree_ITree {
   PyObject_HEAD
   __pyx_t_8rbi_tree_4tree_CTreeObj *tree;
 };
 
 
-/* "rbi_tree/tree.pyx":142
+/* "rbi_tree/tree.pyx":141
  *             inc(it)
  * 
  * cdef class ITreed():             # <<<<<<<<<<<<<<
- *     cdef CTreeInt* tree
- *     cdef Ivlmap ivldata
+ *     """Version of ITree supporting deletion
+ *     """
  */
 struct __pyx_obj_8rbi_tree_4tree_ITreed {
   PyObject_HEAD
   struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *__pyx_vtab;
   __pyx_t_8rbi_tree_4tree_CTreeInt *tree;
   __pyx_t_8rbi_tree_4tree_Ivlmap ivldata;
-  std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::iterator datapos;
+  std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::const_iterator datapos;
   PyObject *tot;
 };
 
 
-/* "rbi_tree/tree.pyx":133
+/* "rbi_tree/tree.pyx":132
  *         return a
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  */
 struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl {
@@ -976,15 +1504,15 @@
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj>  __pyx_v_intervals;
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj> ::iterator __pyx_v_it;
   struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self;
   PyObject *__pyx_v_val;
 };
 
 
-/* "rbi_tree/tree.pyx":240
+/* "rbi_tree/tree.pyx":241
  *         del ivl
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
  */
 struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl {
@@ -992,166 +1520,279 @@
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalInt>  __pyx_v_intervals;
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalInt> ::iterator __pyx_v_it;
   struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self;
 };
 
 
 
-/* "rbi_tree/tree.pyx":142
+/* "rbi_tree/tree.pyx":141
  *             inc(it)
  * 
  * cdef class ITreed():             # <<<<<<<<<<<<<<
- *     cdef CTreeInt* tree
- *     cdef Ivlmap ivldata
+ *     """Version of ITree supporting deletion
+ *     """
  */
 
 struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed {
   __pyx_t_8rbi_tree_4tree_CIntervalInt *(*_get_interval)(struct __pyx_obj_8rbi_tree_4tree_ITreed *, PyObject *);
 };
 static struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *__pyx_vtabptr_8rbi_tree_4tree_ITreed;
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
+#endif
+#endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
@@ -1175,71 +1816,71 @@
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* pep479.proto */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen);
+
+/* MoveIfSupported.proto */
+#if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+  #include <utility>
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
+#else
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
+#endif
 
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
+
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
-/* IncludeStringH.proto */
-#include <string.h>
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
+#endif
+
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
@@ -1248,39 +1889,165 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable);
+static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
+
+/* GetVTable.proto */
+static void* __Pyx_GetVtable(PyTypeObject *type);
+
+/* MergeVTables.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type);
+#endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
-/* ClassMethod.proto */
-#include "descrobject.h"
-static CYTHON_UNUSED PyObject* __Pyx_Method_ClassMethod(PyObject *method);
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
+/* ClassMethod.proto */
+#include "descrobject.h"
+CYTHON_UNUSED static PyObject* __Pyx_Method_ClassMethod(PyObject *method);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1301,26 +2068,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1332,37 +2099,39 @@
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* None.proto */
 #include <new>
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CppExceptionConversion.proto */
 #ifndef __Pyx_CppExn2PyErr
 #include <new>
 #include <typeinfo>
@@ -1406,38 +2175,52 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
-/* FetchCommonType.proto */
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
-
 /* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
@@ -1452,43 +2235,45 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* CoroutineBase.proto */
-typedef PyObject *(*__pyx_coroutine_body_t)(PyObject *, PyThreadState *, PyObject *);
+struct __pyx_CoroutineObject;
+typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
 #if CYTHON_USE_EXC_INFO_STACK
 #define __Pyx_ExcInfoStruct  _PyErr_StackItem
 #else
 typedef struct {
     PyObject *exc_type;
     PyObject *exc_value;
     PyObject *exc_traceback;
 } __Pyx_ExcInfoStruct;
 #endif
-typedef struct {
+typedef struct __pyx_CoroutineObject {
     PyObject_HEAD
     __pyx_coroutine_body_t body;
     PyObject *closure;
     __Pyx_ExcInfoStruct gi_exc_state;
     PyObject *gi_weakreflist;
     PyObject *classobj;
     PyObject *yieldfrom;
     PyObject *gi_name;
     PyObject *gi_qualname;
     PyObject *gi_modulename;
     PyObject *gi_code;
+    PyObject *gi_frame;
     int resume_label;
     char is_running;
 } __pyx_CoroutineObject;
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
     PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
     PyObject *name, PyObject *qualname, PyObject *module_name);
 static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
@@ -1526,109 +2311,123 @@
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
 
 /* PatchGeneratorABC.proto */
 static int __Pyx_patch_abc(void);
 
 /* Generator.proto */
 #define __Pyx_Generator_USED
-static PyTypeObject *__pyx_GeneratorType = 0;
-#define __Pyx_Generator_CheckExact(obj) (Py_TYPE(obj) == __pyx_GeneratorType)
+#define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
 #define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
     __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
 static PyObject *__Pyx_Generator_Next(PyObject *self);
-static int __pyx_Generator_init(void);
+static int __pyx_Generator_init(PyObject *module);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
 static __pyx_t_8rbi_tree_4tree_CIntervalInt *__pyx_f_8rbi_tree_4tree_6ITreed__get_interval(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, PyObject *__pyx_v_id); /* proto*/
 
-/* Module declarations from 'libcpp.vector' */
+/* Module declarations from "libcpp.vector" */
 
-/* Module declarations from 'libcpp.utility' */
+/* Module declarations from "libcpp.utility" */
 
-/* Module declarations from 'libcpp.map' */
+/* Module declarations from "libcpp.map" */
 
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'rbi_tree.tree' */
-static PyTypeObject *__pyx_ptype_8rbi_tree_4tree_ITree = 0;
-static PyTypeObject *__pyx_ptype_8rbi_tree_4tree_ITreed = 0;
-static PyTypeObject *__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl = 0;
-static PyTypeObject *__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl = 0;
+/* Module declarations from "rbi_tree.tree" */
+/* #### Code section: typeinfo ### */
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "rbi_tree.tree"
 extern int __pyx_module_is_main_rbi_tree__tree;
 int __pyx_module_is_main_rbi_tree__tree = 0;
 
-/* Implementation of 'rbi_tree.tree' */
+/* Implementation of "rbi_tree.tree" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_ValueError;
+/* #### Code section: string_decls ### */
+static const char __pyx_k_a[] = "a";
+static const char __pyx_k_gc[] = "gc";
+static const char __pyx_k_id[] = "id";
+static const char __pyx_k_it[] = "it";
+static const char __pyx_k__31[] = "?";
+static const char __pyx_k_cls[] = "cls";
 static const char __pyx_k_end[] = "end";
+static const char __pyx_k_ivl[] = "ivl";
+static const char __pyx_k_out[] = "out";
 static const char __pyx_k_tot[] = "tot";
+static const char __pyx_k_val[] = "val";
 static const char __pyx_k_args[] = "args";
+static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_find[] = "find";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_self[] = "self";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_tree[] = "tree";
 static const char __pyx_k_ITree[] = "ITree";
 static const char __pyx_k_close[] = "close";
+static const char __pyx_k_point[] = "point";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_ITreed[] = "ITreed";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_insert[] = "insert";
+static const char __pyx_k_ivl_id[] = "ivl_id";
+static const char __pyx_k_reduce[] = "__reduce__";
+static const char __pyx_k_remove[] = "remove";
+static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_find_at[] = "find_at";
+static const char __pyx_k_get_ivl[] = "get_ivl";
 static const char __pyx_k_insert_2[] = "_insert";
 static const char __pyx_k_iter_ivl[] = "iter_ivl";
 static const char __pyx_k_intervals[] = "intervals";
+static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_ITree_find[] = "ITree.find";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_ITreed_find[] = "ITreed.find";
+static const char __pyx_k_ITree_insert[] = "ITree.insert";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_ITree_find_at[] = "ITree.find_at";
+static const char __pyx_k_ITreed_insert[] = "ITreed.insert";
+static const char __pyx_k_ITreed_remove[] = "ITreed.remove";
 static const char __pyx_k_rbi_tree_tree[] = "rbi_tree.tree";
+static const char __pyx_k_ITree___reduce[] = "ITree.__reduce__";
 static const char __pyx_k_ITree_iter_ivl[] = "ITree.iter_ivl";
+static const char __pyx_k_ITreed__insert[] = "ITreed._insert";
+static const char __pyx_k_ITreed_find_at[] = "ITreed.find_at";
+static const char __pyx_k_ITreed_get_ivl[] = "ITreed.get_ivl";
 static const char __pyx_k_from_intervals[] = "_from_intervals";
+static const char __pyx_k_ITreed___reduce[] = "ITreed.__reduce__";
 static const char __pyx_k_ITreed_iter_ivl[] = "ITreed.iter_ivl";
+static const char __pyx_k_rbi_tree_tree_pyx[] = "rbi_tree/tree.pyx";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static PyObject *__pyx_n_s_ITree;
-static PyObject *__pyx_n_s_ITree_iter_ivl;
-static PyObject *__pyx_n_s_ITreed;
-static PyObject *__pyx_n_s_ITreed_iter_ivl;
-static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_n_s_args;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_close;
-static PyObject *__pyx_n_s_end;
-static PyObject *__pyx_n_s_from_intervals;
-static PyObject *__pyx_n_s_insert;
-static PyObject *__pyx_n_s_insert_2;
-static PyObject *__pyx_n_s_intervals;
-static PyObject *__pyx_n_s_iter_ivl;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_pyx_vtable;
-static PyObject *__pyx_n_s_rbi_tree_tree;
-static PyObject *__pyx_n_s_send;
-static PyObject *__pyx_n_s_start;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_throw;
-static PyObject *__pyx_n_s_tot;
-static PyObject *__pyx_n_s_value;
+static const char __pyx_k_ITree__from_intervals[] = "ITree._from_intervals";
+static const char __pyx_k_ITreed__from_intervals[] = "ITreed._from_intervals";
+/* #### Code section: decls ### */
 static int __pyx_pf_8rbi_tree_4tree_5ITree___cinit__(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self); /* proto */
 static void __pyx_pf_8rbi_tree_4tree_5ITree_2__dealloc__(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_4__reduce__(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_6insert(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self, PyObject *__pyx_v_start, PyObject *__pyx_v_end, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_8find(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self, int __pyx_v_start, int __pyx_v_end); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_10_from_intervals(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_cls, PyObject *__pyx_v_intervals); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_12find_at(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self, int __pyx_v_point); /* proto */
@@ -1645,35 +2444,608 @@
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_18find_at(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, int __pyx_v_point); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_20remove(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, int __pyx_v_id); /* proto */
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_22iter_ivl(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self); /* proto */
 static PyObject *__pyx_tp_new_8rbi_tree_4tree_ITree(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8rbi_tree_4tree_ITreed(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct__iter_ivl(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_1;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_8rbi_tree_4tree_ITree;
+  PyObject *__pyx_type_8rbi_tree_4tree_ITreed;
+  PyObject *__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl;
+  PyObject *__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl;
+  #endif
+  PyTypeObject *__pyx_ptype_8rbi_tree_4tree_ITree;
+  PyTypeObject *__pyx_ptype_8rbi_tree_4tree_ITreed;
+  PyTypeObject *__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl;
+  PyTypeObject *__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl;
+  PyObject *__pyx_n_s_ITree;
+  PyObject *__pyx_n_s_ITree___reduce;
+  PyObject *__pyx_n_s_ITree__from_intervals;
+  PyObject *__pyx_n_s_ITree_find;
+  PyObject *__pyx_n_s_ITree_find_at;
+  PyObject *__pyx_n_s_ITree_insert;
+  PyObject *__pyx_n_s_ITree_iter_ivl;
+  PyObject *__pyx_n_s_ITreed;
+  PyObject *__pyx_n_s_ITreed___reduce;
+  PyObject *__pyx_n_s_ITreed__from_intervals;
+  PyObject *__pyx_n_s_ITreed__insert;
+  PyObject *__pyx_n_s_ITreed_find;
+  PyObject *__pyx_n_s_ITreed_find_at;
+  PyObject *__pyx_n_s_ITreed_get_ivl;
+  PyObject *__pyx_n_s_ITreed_insert;
+  PyObject *__pyx_n_s_ITreed_iter_ivl;
+  PyObject *__pyx_n_s_ITreed_remove;
+  PyObject *__pyx_n_s_ValueError;
+  PyObject *__pyx_n_s__31;
+  PyObject *__pyx_n_s_a;
+  PyObject *__pyx_n_s_args;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_close;
+  PyObject *__pyx_n_s_cls;
+  PyObject *__pyx_n_s_dict;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_end;
+  PyObject *__pyx_n_s_find;
+  PyObject *__pyx_n_s_find_at;
+  PyObject *__pyx_n_s_from_intervals;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_get_ivl;
+  PyObject *__pyx_n_s_id;
+  PyObject *__pyx_n_s_insert;
+  PyObject *__pyx_n_s_insert_2;
+  PyObject *__pyx_n_s_intervals;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_it;
+  PyObject *__pyx_n_s_iter_ivl;
+  PyObject *__pyx_n_s_ivl;
+  PyObject *__pyx_n_s_ivl_id;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_out;
+  PyObject *__pyx_n_s_point;
+  PyObject *__pyx_n_s_pyx_vtable;
+  PyObject *__pyx_n_s_rbi_tree_tree;
+  PyObject *__pyx_kp_s_rbi_tree_tree_pyx;
+  PyObject *__pyx_n_s_reduce;
+  PyObject *__pyx_n_s_remove;
+  PyObject *__pyx_n_s_self;
+  PyObject *__pyx_n_s_send;
+  PyObject *__pyx_n_s_start;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_throw;
+  PyObject *__pyx_n_s_tot;
+  PyObject *__pyx_n_s_tree;
+  PyObject *__pyx_n_s_val;
+  PyObject *__pyx_n_s_value;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_int_1;
+  PyObject *__pyx_codeobj_;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_tuple__12;
+  PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__16;
+  PyObject *__pyx_tuple__18;
+  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_tuple__30;
+  PyObject *__pyx_codeobj__2;
+  PyObject *__pyx_codeobj__4;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
+  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__17;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__26;
+  PyObject *__pyx_codeobj__28;
+  PyObject *__pyx_codeobj__29;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_8rbi_tree_4tree_ITree);
+  Py_CLEAR(clear_module_state->__pyx_type_8rbi_tree_4tree_ITree);
+  Py_CLEAR(clear_module_state->__pyx_ptype_8rbi_tree_4tree_ITreed);
+  Py_CLEAR(clear_module_state->__pyx_type_8rbi_tree_4tree_ITreed);
+  Py_CLEAR(clear_module_state->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree___reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree__from_intervals);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree_find);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree_find_at);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree_insert);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITree_iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed___reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed__from_intervals);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed__insert);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_find);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_find_at);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_get_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_insert);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ITreed_remove);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__31);
+  Py_CLEAR(clear_module_state->__pyx_n_s_a);
+  Py_CLEAR(clear_module_state->__pyx_n_s_args);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cls);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dict);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_end);
+  Py_CLEAR(clear_module_state->__pyx_n_s_find);
+  Py_CLEAR(clear_module_state->__pyx_n_s_find_at);
+  Py_CLEAR(clear_module_state->__pyx_n_s_from_intervals);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_id);
+  Py_CLEAR(clear_module_state->__pyx_n_s_insert);
+  Py_CLEAR(clear_module_state->__pyx_n_s_insert_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_intervals);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_it);
+  Py_CLEAR(clear_module_state->__pyx_n_s_iter_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ivl);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ivl_id);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_out);
+  Py_CLEAR(clear_module_state->__pyx_n_s_point);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rbi_tree_tree);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_rbi_tree_tree_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_remove);
+  Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_n_s_send);
+  Py_CLEAR(clear_module_state->__pyx_n_s_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_throw);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tot);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tree);
+  Py_CLEAR(clear_module_state->__pyx_n_s_val);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_codeobj_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__12);
+  Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__16);
+  Py_CLEAR(clear_module_state->__pyx_tuple__18);
+  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__30);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__2);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_8rbi_tree_4tree_ITree);
+  Py_VISIT(traverse_module_state->__pyx_type_8rbi_tree_4tree_ITree);
+  Py_VISIT(traverse_module_state->__pyx_ptype_8rbi_tree_4tree_ITreed);
+  Py_VISIT(traverse_module_state->__pyx_type_8rbi_tree_4tree_ITreed);
+  Py_VISIT(traverse_module_state->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree___reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree__from_intervals);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree_find);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree_find_at);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree_insert);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITree_iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed___reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed__from_intervals);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed__insert);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_find);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_find_at);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_get_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_insert);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ITreed_remove);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__31);
+  Py_VISIT(traverse_module_state->__pyx_n_s_a);
+  Py_VISIT(traverse_module_state->__pyx_n_s_args);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cls);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dict);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_end);
+  Py_VISIT(traverse_module_state->__pyx_n_s_find);
+  Py_VISIT(traverse_module_state->__pyx_n_s_find_at);
+  Py_VISIT(traverse_module_state->__pyx_n_s_from_intervals);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_id);
+  Py_VISIT(traverse_module_state->__pyx_n_s_insert);
+  Py_VISIT(traverse_module_state->__pyx_n_s_insert_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_intervals);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_it);
+  Py_VISIT(traverse_module_state->__pyx_n_s_iter_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ivl);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ivl_id);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_out);
+  Py_VISIT(traverse_module_state->__pyx_n_s_point);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rbi_tree_tree);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_rbi_tree_tree_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_remove);
+  Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_n_s_send);
+  Py_VISIT(traverse_module_state->__pyx_n_s_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_throw);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tot);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tree);
+  Py_VISIT(traverse_module_state->__pyx_n_s_val);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_codeobj_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__12);
+  Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__16);
+  Py_VISIT(traverse_module_state->__pyx_tuple__18);
+  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__30);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__2);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_8rbi_tree_4tree_ITree __pyx_mstate_global->__pyx_type_8rbi_tree_4tree_ITree
+#define __pyx_type_8rbi_tree_4tree_ITreed __pyx_mstate_global->__pyx_type_8rbi_tree_4tree_ITreed
+#define __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl __pyx_mstate_global->__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl
+#define __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl __pyx_mstate_global->__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl
+#endif
+#define __pyx_ptype_8rbi_tree_4tree_ITree __pyx_mstate_global->__pyx_ptype_8rbi_tree_4tree_ITree
+#define __pyx_ptype_8rbi_tree_4tree_ITreed __pyx_mstate_global->__pyx_ptype_8rbi_tree_4tree_ITreed
+#define __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl __pyx_mstate_global->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl
+#define __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl __pyx_mstate_global->__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl
+#define __pyx_n_s_ITree __pyx_mstate_global->__pyx_n_s_ITree
+#define __pyx_n_s_ITree___reduce __pyx_mstate_global->__pyx_n_s_ITree___reduce
+#define __pyx_n_s_ITree__from_intervals __pyx_mstate_global->__pyx_n_s_ITree__from_intervals
+#define __pyx_n_s_ITree_find __pyx_mstate_global->__pyx_n_s_ITree_find
+#define __pyx_n_s_ITree_find_at __pyx_mstate_global->__pyx_n_s_ITree_find_at
+#define __pyx_n_s_ITree_insert __pyx_mstate_global->__pyx_n_s_ITree_insert
+#define __pyx_n_s_ITree_iter_ivl __pyx_mstate_global->__pyx_n_s_ITree_iter_ivl
+#define __pyx_n_s_ITreed __pyx_mstate_global->__pyx_n_s_ITreed
+#define __pyx_n_s_ITreed___reduce __pyx_mstate_global->__pyx_n_s_ITreed___reduce
+#define __pyx_n_s_ITreed__from_intervals __pyx_mstate_global->__pyx_n_s_ITreed__from_intervals
+#define __pyx_n_s_ITreed__insert __pyx_mstate_global->__pyx_n_s_ITreed__insert
+#define __pyx_n_s_ITreed_find __pyx_mstate_global->__pyx_n_s_ITreed_find
+#define __pyx_n_s_ITreed_find_at __pyx_mstate_global->__pyx_n_s_ITreed_find_at
+#define __pyx_n_s_ITreed_get_ivl __pyx_mstate_global->__pyx_n_s_ITreed_get_ivl
+#define __pyx_n_s_ITreed_insert __pyx_mstate_global->__pyx_n_s_ITreed_insert
+#define __pyx_n_s_ITreed_iter_ivl __pyx_mstate_global->__pyx_n_s_ITreed_iter_ivl
+#define __pyx_n_s_ITreed_remove __pyx_mstate_global->__pyx_n_s_ITreed_remove
+#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
+#define __pyx_n_s__31 __pyx_mstate_global->__pyx_n_s__31
+#define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
+#define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
+#define __pyx_n_s_cls __pyx_mstate_global->__pyx_n_s_cls
+#define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_end __pyx_mstate_global->__pyx_n_s_end
+#define __pyx_n_s_find __pyx_mstate_global->__pyx_n_s_find
+#define __pyx_n_s_find_at __pyx_mstate_global->__pyx_n_s_find_at
+#define __pyx_n_s_from_intervals __pyx_mstate_global->__pyx_n_s_from_intervals
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_get_ivl __pyx_mstate_global->__pyx_n_s_get_ivl
+#define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
+#define __pyx_n_s_insert __pyx_mstate_global->__pyx_n_s_insert
+#define __pyx_n_s_insert_2 __pyx_mstate_global->__pyx_n_s_insert_2
+#define __pyx_n_s_intervals __pyx_mstate_global->__pyx_n_s_intervals
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_it __pyx_mstate_global->__pyx_n_s_it
+#define __pyx_n_s_iter_ivl __pyx_mstate_global->__pyx_n_s_iter_ivl
+#define __pyx_n_s_ivl __pyx_mstate_global->__pyx_n_s_ivl
+#define __pyx_n_s_ivl_id __pyx_mstate_global->__pyx_n_s_ivl_id
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_out __pyx_mstate_global->__pyx_n_s_out
+#define __pyx_n_s_point __pyx_mstate_global->__pyx_n_s_point
+#define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
+#define __pyx_n_s_rbi_tree_tree __pyx_mstate_global->__pyx_n_s_rbi_tree_tree
+#define __pyx_kp_s_rbi_tree_tree_pyx __pyx_mstate_global->__pyx_kp_s_rbi_tree_tree_pyx
+#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
+#define __pyx_n_s_remove __pyx_mstate_global->__pyx_n_s_remove
+#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
+#define __pyx_n_s_start __pyx_mstate_global->__pyx_n_s_start
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
+#define __pyx_n_s_tot __pyx_mstate_global->__pyx_n_s_tot
+#define __pyx_n_s_tree __pyx_mstate_global->__pyx_n_s_tree
+#define __pyx_n_s_val __pyx_mstate_global->__pyx_n_s_val
+#define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_codeobj_ __pyx_mstate_global->__pyx_codeobj_
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
+#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
+#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
+#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
+#define __pyx_codeobj__2 __pyx_mstate_global->__pyx_codeobj__2
+#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
+#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
+/* #### Code section: module_code ### */
 
 /* "rbi_tree/tree.pyx":62
  *     cdef CTreeObj* tree
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.tree = new CTreeObj()
  * 
  */
 
 /* Python wrapper */
 static int __pyx_pw_8rbi_tree_4tree_5ITree_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8rbi_tree_4tree_5ITree_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
-  if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
-  if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree___cinit__(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -1712,14 +3084,15 @@
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
  */
 
 /* Python wrapper */
 static void __pyx_pw_8rbi_tree_4tree_5ITree_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_8rbi_tree_4tree_5ITree_3__dealloc__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
   __pyx_pf_8rbi_tree_4tree_5ITree_2__dealloc__(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
@@ -1728,15 +3101,14 @@
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj>  __pyx_v_intervals;
   std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj> ::iterator __pyx_v_it;
   PyObject *__pyx_v_val = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "rbi_tree/tree.pyx":66
  * 
  *     def __dealloc__(self):
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
@@ -1757,15 +3129,15 @@
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
  * 
  *         while it != intervals.end():             # <<<<<<<<<<<<<<
  *             val  = <object>(deref(it).value)
  *             if not val is None:
  */
   while (1) {
-    __pyx_t_1 = ((__pyx_v_it != __pyx_v_intervals.end()) != 0);
+    __pyx_t_1 = (__pyx_v_it != __pyx_v_intervals.end());
     if (!__pyx_t_1) break;
 
     /* "rbi_tree/tree.pyx":70
  * 
  *         while it != intervals.end():
  *             val  = <object>(deref(it).value)             # <<<<<<<<<<<<<<
  *             if not val is None:
@@ -1781,16 +3153,15 @@
  *         while it != intervals.end():
  *             val  = <object>(deref(it).value)
  *             if not val is None:             # <<<<<<<<<<<<<<
  *                 Py_DECREF(val)
  *             inc(it)
  */
     __pyx_t_1 = (__pyx_v_val != Py_None);
-    __pyx_t_4 = (__pyx_t_1 != 0);
-    if (__pyx_t_4) {
+    if (__pyx_t_1) {
 
       /* "rbi_tree/tree.pyx":72
  *             val  = <object>(deref(it).value)
  *             if not val is None:
  *                 Py_DECREF(val)             # <<<<<<<<<<<<<<
  *             inc(it)
  * 
@@ -1843,33 +3214,54 @@
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         intervals = list(self.iter_ivl())
  *         return (ITree._from_intervals, (intervals,))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_5__reduce__ = {"__reduce__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce__", 0))) return NULL;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_4__reduce__(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_4__reduce__(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self) {
   PyObject *__pyx_v_intervals = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
   /* "rbi_tree/tree.pyx":78
  * 
@@ -1877,29 +3269,34 @@
  *         intervals = list(self.iter_ivl())             # <<<<<<<<<<<<<<
  *         return (ITree._from_intervals, (intervals,))
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_iter_ivl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_3, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_2 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_intervals = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "rbi_tree/tree.pyx":79
  *     def __reduce__(self):
@@ -1950,86 +3347,106 @@
   return __pyx_r;
 }
 
 /* "rbi_tree/tree.pyx":81
  *         return (ITree._from_intervals, (intervals,))
  * 
  *     def insert(self, start, end, value=None):             # <<<<<<<<<<<<<<
- *         """Insert an interval [start, end) and returns an id
- *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+ *         """Insert an interval [start, end) """
+ * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_7insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_5ITree_6insert[] = "Insert an interval [start, end) and returns an id\n        of the interval. Ids are incrementing integers, i.e. 0,1,2 etc.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_7insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_7insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_5ITree_6insert, "Insert an interval [start, end) ");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_7insert = {"insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_7insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_6insert};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_7insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_start = 0;
   PyObject *__pyx_v_end = 0;
   PyObject *__pyx_v_value = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("insert (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,&__pyx_n_s_value,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,&__pyx_n_s_value,0};
     PyObject* values[3] = {0,0,0};
     values[2] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("insert", 0, 2, 3, 1); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "insert") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "insert") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_start = values[0];
     __pyx_v_end = values[1];
     __pyx_v_value = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("insert", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 81, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("insert", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITree.insert", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_6insert(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self), __pyx_v_start, __pyx_v_end, __pyx_v_value);
 
@@ -2043,190 +3460,207 @@
   PyObject *__pyx_v_val = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
-  int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("insert", 0);
 
-  /* "rbi_tree/tree.pyx":86
+  /* "rbi_tree/tree.pyx":85
  * 
  *         cdef CIntervalObj* ivl = new CIntervalObj(
  *             start, end, <PyObject*>value)             # <<<<<<<<<<<<<<
  *         self.tree.insert(deref(ivl))
  *         val = <object>value
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_start); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_end); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_start); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_end); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  /* "rbi_tree/tree.pyx":85
- *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+  /* "rbi_tree/tree.pyx":84
+ *         """Insert an interval [start, end) """
  * 
  *         cdef CIntervalObj* ivl = new CIntervalObj(             # <<<<<<<<<<<<<<
  *             start, end, <PyObject*>value)
  *         self.tree.insert(deref(ivl))
  */
   __pyx_v_ivl = new __pyx_t_8rbi_tree_4tree_CIntervalObj(__pyx_t_1, __pyx_t_2, ((PyObject *)__pyx_v_value));
 
-  /* "rbi_tree/tree.pyx":87
+  /* "rbi_tree/tree.pyx":86
  *         cdef CIntervalObj* ivl = new CIntervalObj(
  *             start, end, <PyObject*>value)
  *         self.tree.insert(deref(ivl))             # <<<<<<<<<<<<<<
  *         val = <object>value
  *         if not val is None:
  */
   (void)(__pyx_v_self->tree->insert((*__pyx_v_ivl)));
 
-  /* "rbi_tree/tree.pyx":88
+  /* "rbi_tree/tree.pyx":87
  *             start, end, <PyObject*>value)
  *         self.tree.insert(deref(ivl))
  *         val = <object>value             # <<<<<<<<<<<<<<
  *         if not val is None:
  *             Py_INCREF(val)
  */
   __pyx_t_3 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_val = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "rbi_tree/tree.pyx":89
+  /* "rbi_tree/tree.pyx":88
  *         self.tree.insert(deref(ivl))
  *         val = <object>value
  *         if not val is None:             # <<<<<<<<<<<<<<
  *             Py_INCREF(val)
  *         del ivl
  */
   __pyx_t_4 = (__pyx_v_val != Py_None);
-  __pyx_t_5 = (__pyx_t_4 != 0);
-  if (__pyx_t_5) {
+  if (__pyx_t_4) {
 
-    /* "rbi_tree/tree.pyx":90
+    /* "rbi_tree/tree.pyx":89
  *         val = <object>value
  *         if not val is None:
  *             Py_INCREF(val)             # <<<<<<<<<<<<<<
  *         del ivl
  *         return
  */
     Py_INCREF(__pyx_v_val);
 
-    /* "rbi_tree/tree.pyx":89
+    /* "rbi_tree/tree.pyx":88
  *         self.tree.insert(deref(ivl))
  *         val = <object>value
  *         if not val is None:             # <<<<<<<<<<<<<<
  *             Py_INCREF(val)
  *         del ivl
  */
   }
 
-  /* "rbi_tree/tree.pyx":91
+  /* "rbi_tree/tree.pyx":90
  *         if not val is None:
  *             Py_INCREF(val)
  *         del ivl             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   delete __pyx_v_ivl;
 
-  /* "rbi_tree/tree.pyx":92
+  /* "rbi_tree/tree.pyx":91
  *             Py_INCREF(val)
  *         del ivl
  *         return             # <<<<<<<<<<<<<<
  * 
  *     def find(self, int start, int end):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
   /* "rbi_tree/tree.pyx":81
  *         return (ITree._from_intervals, (intervals,))
  * 
  *     def insert(self, start, end, value=None):             # <<<<<<<<<<<<<<
- *         """Insert an interval [start, end) and returns an id
- *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+ *         """Insert an interval [start, end) """
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("rbi_tree.tree.ITree.insert", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":94
+/* "rbi_tree/tree.pyx":93
  *         return
  * 
  *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_9find(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_5ITree_8find[] = "Search intervals overlapping [start, end). Returns list of \n        overlapping intervals' ids.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_9find(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_9find(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_5ITree_8find, "Search intervals overlapping [start, end). Returns list of \n        overlapping intervals' ids.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_9find = {"find", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_9find, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_8find};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_9find(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_start;
   int __pyx_v_end;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, 1); __PYX_ERR(0, 94, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, 1); __PYX_ERR(0, 93, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "find") < 0)) __PYX_ERR(0, 94, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "find") < 0)) __PYX_ERR(0, 93, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L3_error)
-    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
+    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 94, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 93, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITree.find", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_8find(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self), __pyx_v_start, __pyx_v_end);
 
@@ -2251,161 +3685,161 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find", 0);
 
-  /* "rbi_tree/tree.pyx":97
+  /* "rbi_tree/tree.pyx":96
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  *         cdef CIntervalObj* ivl = new CIntervalObj(start,end)             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalObj] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  */
   __pyx_v_ivl = new __pyx_t_8rbi_tree_4tree_CIntervalObj(__pyx_v_start, __pyx_v_end);
 
-  /* "rbi_tree/tree.pyx":99
+  /* "rbi_tree/tree.pyx":98
  *         cdef CIntervalObj* ivl = new CIntervalObj(start,end)
  *         cdef vector[CIntervalObj] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)             # <<<<<<<<<<<<<<
  *         del ivl
  *         a = []
  */
   __pyx_v_self->tree->findOverlappingIntervals((*__pyx_v_ivl), __pyx_v_out);
 
-  /* "rbi_tree/tree.pyx":100
+  /* "rbi_tree/tree.pyx":99
  *         cdef vector[CIntervalObj] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  *         del ivl             # <<<<<<<<<<<<<<
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  */
   delete __pyx_v_ivl;
 
-  /* "rbi_tree/tree.pyx":101
+  /* "rbi_tree/tree.pyx":100
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  *         del ivl
  *         a = []             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_a = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":102
+  /* "rbi_tree/tree.pyx":101
  *         del ivl
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()             # <<<<<<<<<<<<<<
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  */
   __pyx_v_it = __pyx_v_out.begin();
 
-  /* "rbi_tree/tree.pyx":103
+  /* "rbi_tree/tree.pyx":102
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():             # <<<<<<<<<<<<<<
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:
  */
   while (1) {
-    __pyx_t_2 = ((__pyx_v_it != __pyx_v_out.end()) != 0);
+    __pyx_t_2 = (__pyx_v_it != __pyx_v_out.end());
     if (!__pyx_t_2) break;
 
-    /* "rbi_tree/tree.pyx":105
+    /* "rbi_tree/tree.pyx":104
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:             # <<<<<<<<<<<<<<
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  */
-    __pyx_t_3 = (((*__pyx_v_it).high != __pyx_v_start) != 0);
+    __pyx_t_3 = ((*__pyx_v_it).high != __pyx_v_start);
     if (__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L6_bool_binop_done;
     }
-    __pyx_t_3 = (((*__pyx_v_it).low != __pyx_v_end) != 0);
+    __pyx_t_3 = ((*__pyx_v_it).low != __pyx_v_end);
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "rbi_tree/tree.pyx":106
+      /* "rbi_tree/tree.pyx":105
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:
  *                 val = <object>deref(it).value             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)
  */
       __pyx_t_4 = (*__pyx_v_it).value;
       __pyx_t_1 = ((PyObject *)__pyx_t_4);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "rbi_tree/tree.pyx":107
+      /* "rbi_tree/tree.pyx":106
  *             if deref(it).high!=start and deref(it).low!=end:
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )             # <<<<<<<<<<<<<<
  *             inc(it)
  *         return a
  */
-      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
       __Pyx_INCREF(__pyx_v_val);
       __Pyx_GIVEREF(__pyx_v_val);
       PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_val);
       __pyx_t_1 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 107, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "rbi_tree/tree.pyx":105
+      /* "rbi_tree/tree.pyx":104
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:             # <<<<<<<<<<<<<<
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  */
     }
 
-    /* "rbi_tree/tree.pyx":108
+    /* "rbi_tree/tree.pyx":107
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)             # <<<<<<<<<<<<<<
  *         return a
  * 
  */
     (void)((++__pyx_v_it));
   }
 
-  /* "rbi_tree/tree.pyx":109
+  /* "rbi_tree/tree.pyx":108
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)
  *         return a             # <<<<<<<<<<<<<<
  * 
  *     def _from_intervals(cls, intervals=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_a);
   __pyx_r = __pyx_v_a;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":94
+  /* "rbi_tree/tree.pyx":93
  *         return
  * 
  *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  */
 
@@ -2420,69 +3854,87 @@
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":111
+/* "rbi_tree/tree.pyx":110
  *         return a
  * 
  *     def _from_intervals(cls, intervals=None):             # <<<<<<<<<<<<<<
  *         tree = cls()
  *         if not intervals is None:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals(PyObject *__pyx_v_cls, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_11_from_intervals = {"_from_intervals", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals(PyObject *__pyx_v_cls, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_intervals = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_from_intervals (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_intervals,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_intervals,0};
     PyObject* values[1] = {0};
     values[0] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_intervals);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_intervals);
           if (value) { values[0] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_from_intervals") < 0)) __PYX_ERR(0, 111, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_from_intervals") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_intervals = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_from_intervals", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 111, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_from_intervals", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 110, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITree._from_intervals", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_10_from_intervals(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_cls), __pyx_v_intervals);
 
@@ -2505,110 +3957,113 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *(*__pyx_t_11)(PyObject *);
-  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_from_intervals", 0);
 
-  /* "rbi_tree/tree.pyx":112
+  /* "rbi_tree/tree.pyx":111
  * 
  *     def _from_intervals(cls, intervals=None):
  *         tree = cls()             # <<<<<<<<<<<<<<
  *         if not intervals is None:
  *             for start, end, val in intervals:
  */
-  __Pyx_INCREF(((PyObject *)__pyx_v_cls));
+  __Pyx_INCREF((PyObject *)__pyx_v_cls);
   __pyx_t_2 = ((PyObject *)__pyx_v_cls); __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_3, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   __pyx_v_tree = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":113
+  /* "rbi_tree/tree.pyx":112
  *     def _from_intervals(cls, intervals=None):
  *         tree = cls()
  *         if not intervals is None:             # <<<<<<<<<<<<<<
  *             for start, end, val in intervals:
  *                 tree.insert(start, end, val)
  */
-  __pyx_t_4 = (__pyx_v_intervals != Py_None);
-  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_5 = (__pyx_v_intervals != Py_None);
   if (__pyx_t_5) {
 
-    /* "rbi_tree/tree.pyx":114
+    /* "rbi_tree/tree.pyx":113
  *         tree = cls()
  *         if not intervals is None:
  *             for start, end, val in intervals:             # <<<<<<<<<<<<<<
  *                 tree.insert(start, end, val)
  *         return tree
  */
     if (likely(PyList_CheckExact(__pyx_v_intervals)) || PyTuple_CheckExact(__pyx_v_intervals)) {
       __pyx_t_1 = __pyx_v_intervals; __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_intervals); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_intervals); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 114, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_7(__pyx_t_1);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 114, __pyx_L1_error)
+            else __PYX_ERR(0, 113, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 3)) {
           if (size > 3) __Pyx_RaiseTooManyValuesError(3);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 114, __pyx_L1_error)
+          __PYX_ERR(0, 113, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_9 = PyTuple_GET_ITEM(sequence, 2); 
         } else {
@@ -2616,143 +4071,115 @@
           __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
           __pyx_t_9 = PyList_GET_ITEM(sequence, 2); 
         }
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_9);
         #else
-        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 114, __pyx_L1_error)
+        __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 114, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 114, __pyx_L1_error)
+        __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
+        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_10);
         index = 0; __pyx_t_3 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_3)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_3);
         index = 1; __pyx_t_8 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_8)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_8);
         index = 2; __pyx_t_9 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_9)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_9);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 3) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 3) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
         __pyx_t_11 = NULL;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L7_unpacking_done;
         __pyx_L6_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 114, __pyx_L1_error)
+        __PYX_ERR(0, 113, __pyx_L1_error)
         __pyx_L7_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_start, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_end, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "rbi_tree/tree.pyx":115
+      /* "rbi_tree/tree.pyx":114
  *         if not intervals is None:
  *             for start, end, val in intervals:
  *                 tree.insert(start, end, val)             # <<<<<<<<<<<<<<
  *         return tree
  *     _from_intervals = classmethod(_from_intervals)
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_tree, __pyx_n_s_insert); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_tree, __pyx_n_s_insert); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_8 = NULL;
-      __pyx_t_12 = 0;
+      __pyx_t_4 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_12 = 1;
+          __pyx_t_4 = 1;
         }
       }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-      } else
-      #endif
       {
-        __pyx_t_3 = PyTuple_New(3+__pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        if (__pyx_t_8) {
-          __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_8); __pyx_t_8 = NULL;
-        }
-        __Pyx_INCREF(__pyx_v_start);
-        __Pyx_GIVEREF(__pyx_v_start);
-        PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_12, __pyx_v_start);
-        __Pyx_INCREF(__pyx_v_end);
-        __Pyx_GIVEREF(__pyx_v_end);
-        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_12, __pyx_v_end);
-        __Pyx_INCREF(__pyx_v_val);
-        __Pyx_GIVEREF(__pyx_v_val);
-        PyTuple_SET_ITEM(__pyx_t_3, 2+__pyx_t_12, __pyx_v_val);
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+        PyObject *__pyx_callargs[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "rbi_tree/tree.pyx":114
+      /* "rbi_tree/tree.pyx":113
  *         tree = cls()
  *         if not intervals is None:
  *             for start, end, val in intervals:             # <<<<<<<<<<<<<<
  *                 tree.insert(start, end, val)
  *         return tree
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "rbi_tree/tree.pyx":113
+    /* "rbi_tree/tree.pyx":112
  *     def _from_intervals(cls, intervals=None):
  *         tree = cls()
  *         if not intervals is None:             # <<<<<<<<<<<<<<
  *             for start, end, val in intervals:
  *                 tree.insert(start, end, val)
  */
   }
 
-  /* "rbi_tree/tree.pyx":116
+  /* "rbi_tree/tree.pyx":115
  *             for start, end, val in intervals:
  *                 tree.insert(start, end, val)
  *         return tree             # <<<<<<<<<<<<<<
  *     _from_intervals = classmethod(_from_intervals)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_tree);
   __pyx_r = __pyx_v_tree;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":111
+  /* "rbi_tree/tree.pyx":110
  *         return a
  * 
  *     def _from_intervals(cls, intervals=None):             # <<<<<<<<<<<<<<
  *         tree = cls()
  *         if not intervals is None:
  */
 
@@ -2772,43 +4199,88 @@
   __Pyx_XDECREF(__pyx_v_end);
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":119
+/* "rbi_tree/tree.pyx":118
  *     _from_intervals = classmethod(_from_intervals)
  * 
  *     def find_at(self, int point):             # <<<<<<<<<<<<<<
  *         """Search for intervals containing specified point. Returns list of
  *         overlapping intervals' ids."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_13find_at(PyObject *__pyx_v_self, PyObject *__pyx_arg_point); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_5ITree_12find_at[] = "Search for intervals containing specified point. Returns list of \n        overlapping intervals' ids.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_13find_at(PyObject *__pyx_v_self, PyObject *__pyx_arg_point) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_13find_at(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_5ITree_12find_at, "Search for intervals containing specified point. Returns list of \n        overlapping intervals' ids.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_13find_at = {"find_at", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_13find_at, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_12find_at};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_13find_at(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_point;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_at (wrapper)", 0);
-  assert(__pyx_arg_point); {
-    __pyx_v_point = __Pyx_PyInt_As_int(__pyx_arg_point); if (unlikely((__pyx_v_point == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_point,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "find_at") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_point = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_point == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("find_at", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITree.find_at", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_12find_at(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self), ((int)__pyx_v_point));
+  __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_12find_at(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self), __pyx_v_point);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_5ITree_12find_at(struct __pyx_obj_8rbi_tree_4tree_ITree *__pyx_v_self, int __pyx_v_point) {
@@ -2825,135 +4297,135 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_at", 0);
 
-  /* "rbi_tree/tree.pyx":123
+  /* "rbi_tree/tree.pyx":122
  *         overlapping intervals' ids."""
  *         cdef vector[CIntervalObj] out
  *         self.tree.findIntervalsContainPoint(point, out)             # <<<<<<<<<<<<<<
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  */
   __pyx_v_self->tree->findIntervalsContainPoint(__pyx_v_point, __pyx_v_out);
 
-  /* "rbi_tree/tree.pyx":124
+  /* "rbi_tree/tree.pyx":123
  *         cdef vector[CIntervalObj] out
  *         self.tree.findIntervalsContainPoint(point, out)
  *         a = []             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_a = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":125
+  /* "rbi_tree/tree.pyx":124
  *         self.tree.findIntervalsContainPoint(point, out)
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()             # <<<<<<<<<<<<<<
  *         while it != out.end():
  *             if not deref(it).high == point:
  */
   __pyx_v_it = __pyx_v_out.begin();
 
-  /* "rbi_tree/tree.pyx":126
+  /* "rbi_tree/tree.pyx":125
  *         a = []
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():             # <<<<<<<<<<<<<<
  *             if not deref(it).high == point:
  *                 val = <object>deref(it).value
  */
   while (1) {
-    __pyx_t_2 = ((__pyx_v_it != __pyx_v_out.end()) != 0);
+    __pyx_t_2 = (__pyx_v_it != __pyx_v_out.end());
     if (!__pyx_t_2) break;
 
-    /* "rbi_tree/tree.pyx":127
+    /* "rbi_tree/tree.pyx":126
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():
  *             if not deref(it).high == point:             # <<<<<<<<<<<<<<
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  */
-    __pyx_t_2 = ((!(((*__pyx_v_it).high == __pyx_v_point) != 0)) != 0);
+    __pyx_t_2 = (!((*__pyx_v_it).high == __pyx_v_point));
     if (__pyx_t_2) {
 
-      /* "rbi_tree/tree.pyx":128
+      /* "rbi_tree/tree.pyx":127
  *         while it != out.end():
  *             if not deref(it).high == point:
  *                 val = <object>deref(it).value             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)
  */
       __pyx_t_3 = (*__pyx_v_it).value;
       __pyx_t_1 = ((PyObject *)__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "rbi_tree/tree.pyx":129
+      /* "rbi_tree/tree.pyx":128
  *             if not deref(it).high == point:
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )             # <<<<<<<<<<<<<<
  *             inc(it)
  *         return a
  */
-      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
       __Pyx_INCREF(__pyx_v_val);
       __Pyx_GIVEREF(__pyx_v_val);
       PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_val);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "rbi_tree/tree.pyx":127
+      /* "rbi_tree/tree.pyx":126
  *         cdef vector[CIntervalObj].iterator it = out.begin()
  *         while it != out.end():
  *             if not deref(it).high == point:             # <<<<<<<<<<<<<<
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  */
     }
 
-    /* "rbi_tree/tree.pyx":130
+    /* "rbi_tree/tree.pyx":129
  *                 val = <object>deref(it).value
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)             # <<<<<<<<<<<<<<
  *         return a
  * 
  */
     (void)((++__pyx_v_it));
   }
 
-  /* "rbi_tree/tree.pyx":131
+  /* "rbi_tree/tree.pyx":130
  *                 a.append( (deref(it).low, deref(it).high, val) )
  *             inc(it)
  *         return a             # <<<<<<<<<<<<<<
  * 
  *     def iter_ivl(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_a);
   __pyx_r = __pyx_v_a;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":119
+  /* "rbi_tree/tree.pyx":118
  *     _from_intervals = classmethod(_from_intervals)
  * 
  *     def find_at(self, int point):             # <<<<<<<<<<<<<<
  *         """Search for intervals containing specified point. Returns list of
  *         overlapping intervals' ids."""
  */
 
@@ -2969,29 +4441,49 @@
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8rbi_tree_4tree_5ITree_16generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "rbi_tree/tree.pyx":133
+/* "rbi_tree/tree.pyx":132
  *         return a
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_5ITree_14iter_ivl[] = "Iterate over all intervals. Yields tuples (start, end, id).";
-static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_5ITree_14iter_ivl, "Iterate over all intervals. Yields tuples (start, end, id).");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_5ITree_15iter_ivl = {"iter_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_14iter_ivl};
+static PyObject *__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("iter_ivl (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("iter_ivl", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "iter_ivl", 0))) return NULL;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_5ITree_14iter_ivl(((struct __pyx_obj_8rbi_tree_4tree_ITree *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3003,33 +4495,33 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("iter_ivl", 0);
   __pyx_cur_scope = (struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *)__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct__iter_ivl(__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 133, __pyx_L1_error)
+    __PYX_ERR(0, 132, __pyx_L1_error)
   } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8rbi_tree_4tree_5ITree_16generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_ivl, __pyx_n_s_ITree_iter_ivl, __pyx_n_s_rbi_tree_tree); if (unlikely(!gen)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8rbi_tree_4tree_5ITree_16generator, __pyx_codeobj_, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_ivl, __pyx_n_s_ITree_iter_ivl, __pyx_n_s_rbi_tree_tree); if (unlikely(!gen)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITree.iter_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_gb_8rbi_tree_4tree_5ITree_16generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
@@ -3049,72 +4541,72 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 132, __pyx_L1_error)
 
-  /* "rbi_tree/tree.pyx":135
+  /* "rbi_tree/tree.pyx":134
  *     def iter_ivl(self):
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
  *         while it != intervals.end():
  */
   __pyx_cur_scope->__pyx_v_intervals = __pyx_cur_scope->__pyx_v_self->tree->intervals();
 
-  /* "rbi_tree/tree.pyx":136
+  /* "rbi_tree/tree.pyx":135
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()             # <<<<<<<<<<<<<<
  *         while it != intervals.end():
  *             val = <object>deref(it).value
  */
   __pyx_cur_scope->__pyx_v_it = __pyx_cur_scope->__pyx_v_intervals.begin();
 
-  /* "rbi_tree/tree.pyx":137
+  /* "rbi_tree/tree.pyx":136
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
  *         while it != intervals.end():             # <<<<<<<<<<<<<<
  *             val = <object>deref(it).value
  *             yield (deref(it).low, deref(it).high, val)
  */
   while (1) {
-    __pyx_t_1 = ((__pyx_cur_scope->__pyx_v_it != __pyx_cur_scope->__pyx_v_intervals.end()) != 0);
+    __pyx_t_1 = (__pyx_cur_scope->__pyx_v_it != __pyx_cur_scope->__pyx_v_intervals.end());
     if (!__pyx_t_1) break;
 
-    /* "rbi_tree/tree.pyx":138
+    /* "rbi_tree/tree.pyx":137
  *         cdef vector[CIntervalObj].iterator it = intervals.begin()
  *         while it != intervals.end():
  *             val = <object>deref(it).value             # <<<<<<<<<<<<<<
  *             yield (deref(it).low, deref(it).high, val)
  *             inc(it)
  */
     __pyx_t_2 = (*__pyx_cur_scope->__pyx_v_it).value;
     __pyx_t_3 = ((PyObject *)__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_val);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_val, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "rbi_tree/tree.pyx":139
+    /* "rbi_tree/tree.pyx":138
  *         while it != intervals.end():
  *             val = <object>deref(it).value
  *             yield (deref(it).low, deref(it).high, val)             # <<<<<<<<<<<<<<
  *             inc(it)
  * 
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).low); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).low); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_val);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_val);
@@ -3126,39 +4618,40 @@
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 139, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 138, __pyx_L1_error)
 
-    /* "rbi_tree/tree.pyx":140
+    /* "rbi_tree/tree.pyx":139
  *             val = <object>deref(it).value
  *             yield (deref(it).low, deref(it).high, val)
  *             inc(it)             # <<<<<<<<<<<<<<
  * 
  * cdef class ITreed():
  */
     (void)((++__pyx_cur_scope->__pyx_v_it));
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "rbi_tree/tree.pyx":133
+  /* "rbi_tree/tree.pyx":132
  *         return a
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("iter_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
@@ -3166,31 +4659,33 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":148
+/* "rbi_tree/tree.pyx":149
  *     cdef tot
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.tree = new CTreeInt()
  *         self.ivldata = Ivlmap()
  */
 
 /* Python wrapper */
 static int __pyx_pw_8rbi_tree_4tree_6ITreed_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8rbi_tree_4tree_6ITreed_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
-  if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
-  if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed___cinit__(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3199,61 +4694,61 @@
   __Pyx_RefNannyDeclarations
   __pyx_t_8rbi_tree_4tree_Ivlmap __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "rbi_tree/tree.pyx":149
+  /* "rbi_tree/tree.pyx":150
  * 
  *     def __cinit__(self):
  *         self.tree = new CTreeInt()             # <<<<<<<<<<<<<<
  *         self.ivldata = Ivlmap()
  *         self.datapos = self.ivldata.begin()
  */
   __pyx_v_self->tree = new __pyx_t_8rbi_tree_4tree_CTreeInt();
 
-  /* "rbi_tree/tree.pyx":150
+  /* "rbi_tree/tree.pyx":151
  *     def __cinit__(self):
  *         self.tree = new CTreeInt()
  *         self.ivldata = Ivlmap()             # <<<<<<<<<<<<<<
  *         self.datapos = self.ivldata.begin()
  *         self.tot = 0
  */
   try {
     __pyx_t_1 = __pyx_t_8rbi_tree_4tree_Ivlmap();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 150, __pyx_L1_error)
+    __PYX_ERR(0, 151, __pyx_L1_error)
   }
-  __pyx_v_self->ivldata = __pyx_t_1;
+  __pyx_v_self->ivldata = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1);
 
-  /* "rbi_tree/tree.pyx":151
+  /* "rbi_tree/tree.pyx":152
  *         self.tree = new CTreeInt()
  *         self.ivldata = Ivlmap()
  *         self.datapos = self.ivldata.begin()             # <<<<<<<<<<<<<<
  *         self.tot = 0
  * 
  */
-  __pyx_v_self->datapos = __pyx_v_self->ivldata.begin();
+  __pyx_v_self->datapos = ((std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::const_iterator)__pyx_v_self->ivldata.begin());
 
-  /* "rbi_tree/tree.pyx":152
+  /* "rbi_tree/tree.pyx":153
  *         self.ivldata = Ivlmap()
  *         self.datapos = self.ivldata.begin()
  *         self.tot = 0             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, tot=None):
  */
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   __Pyx_GOTREF(__pyx_v_self->tot);
   __Pyx_DECREF(__pyx_v_self->tot);
   __pyx_v_self->tot = __pyx_int_0;
 
-  /* "rbi_tree/tree.pyx":148
+  /* "rbi_tree/tree.pyx":149
  *     cdef tot
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.tree = new CTreeInt()
  *         self.ivldata = Ivlmap()
  */
 
@@ -3264,69 +4759,72 @@
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":154
+/* "rbi_tree/tree.pyx":155
  *         self.tot = 0
  * 
  *     def __init__(self, tot=None):             # <<<<<<<<<<<<<<
  *         if not tot is None:
  *             self.tot = tot
  */
 
 /* Python wrapper */
 static int __pyx_pw_8rbi_tree_4tree_6ITreed_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8rbi_tree_4tree_6ITreed_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_tot = 0;
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_tot,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_tot,0};
     PyObject* values[1] = {0};
     values[0] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tot);
+          PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tot);
           if (value) { values[0] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 154, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 155, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_tot = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 154, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 155, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_2__init__(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_tot);
 
@@ -3335,202 +4833,227 @@
   return __pyx_r;
 }
 
 static int __pyx_pf_8rbi_tree_4tree_6ITreed_2__init__(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, PyObject *__pyx_v_tot) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  int __pyx_t_2;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "rbi_tree/tree.pyx":155
+  /* "rbi_tree/tree.pyx":156
  * 
  *     def __init__(self, tot=None):
  *         if not tot is None:             # <<<<<<<<<<<<<<
  *             self.tot = tot
  * 
  */
   __pyx_t_1 = (__pyx_v_tot != Py_None);
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
+  if (__pyx_t_1) {
 
-    /* "rbi_tree/tree.pyx":156
+    /* "rbi_tree/tree.pyx":157
  *     def __init__(self, tot=None):
  *         if not tot is None:
  *             self.tot = tot             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
     __Pyx_INCREF(__pyx_v_tot);
     __Pyx_GIVEREF(__pyx_v_tot);
     __Pyx_GOTREF(__pyx_v_self->tot);
     __Pyx_DECREF(__pyx_v_self->tot);
     __pyx_v_self->tot = __pyx_v_tot;
 
-    /* "rbi_tree/tree.pyx":155
+    /* "rbi_tree/tree.pyx":156
  * 
  *     def __init__(self, tot=None):
  *         if not tot is None:             # <<<<<<<<<<<<<<
  *             self.tot = tot
  * 
  */
   }
 
-  /* "rbi_tree/tree.pyx":154
+  /* "rbi_tree/tree.pyx":155
  *         self.tot = 0
  * 
  *     def __init__(self, tot=None):             # <<<<<<<<<<<<<<
  *         if not tot is None:
  *             self.tot = tot
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":158
+/* "rbi_tree/tree.pyx":159
  *             self.tot = tot
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         del self.tree
  * 
  */
 
 /* Python wrapper */
 static void __pyx_pw_8rbi_tree_4tree_6ITreed_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_8rbi_tree_4tree_6ITreed_5__dealloc__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
   __pyx_pf_8rbi_tree_4tree_6ITreed_4__dealloc__(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8rbi_tree_4tree_6ITreed_4__dealloc__(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "rbi_tree/tree.pyx":159
+  /* "rbi_tree/tree.pyx":160
  * 
  *     def __dealloc__(self):
  *         del self.tree             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
   delete __pyx_v_self->tree;
 
-  /* "rbi_tree/tree.pyx":158
+  /* "rbi_tree/tree.pyx":159
  *             self.tot = tot
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         del self.tree
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbi_tree/tree.pyx":161
+/* "rbi_tree/tree.pyx":162
  *         del self.tree
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         intervals = list(self.iter_ivl())
  *         return (ITreed._from_intervals, (intervals, self.tot))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_7__reduce__ = {"__reduce__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce__", 0))) return NULL;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_6__reduce__(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_6__reduce__(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self) {
   PyObject *__pyx_v_intervals = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
-  /* "rbi_tree/tree.pyx":162
+  /* "rbi_tree/tree.pyx":163
  * 
  *     def __reduce__(self):
  *         intervals = list(self.iter_ivl())             # <<<<<<<<<<<<<<
  *         return (ITreed._from_intervals, (intervals, self.tot))
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_iter_ivl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_iter_ivl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_3, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_2 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_intervals = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "rbi_tree/tree.pyx":163
+  /* "rbi_tree/tree.pyx":164
  *     def __reduce__(self):
  *         intervals = list(self.iter_ivl())
  *         return (ITreed._from_intervals, (intervals, self.tot))             # <<<<<<<<<<<<<<
  * 
  *     def _from_intervals(cls, intervals=None, tot=0):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed), __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed), __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_intervals);
   __Pyx_GIVEREF(__pyx_v_intervals);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_intervals);
   __Pyx_INCREF(__pyx_v_self->tot);
   __Pyx_GIVEREF(__pyx_v_self->tot);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_self->tot);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":161
+  /* "rbi_tree/tree.pyx":162
  *         del self.tree
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         intervals = list(self.iter_ivl())
  *         return (ITreed._from_intervals, (intervals, self.tot))
  */
 
@@ -3544,82 +5067,101 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_intervals);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":165
+/* "rbi_tree/tree.pyx":166
  *         return (ITreed._from_intervals, (intervals, self.tot))
  * 
  *     def _from_intervals(cls, intervals=None, tot=0):             # <<<<<<<<<<<<<<
  *         tree = cls(tot)
  *         if not intervals is None:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals(PyObject *__pyx_v_cls, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_9_from_intervals = {"_from_intervals", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals(PyObject *__pyx_v_cls, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_intervals = 0;
   PyObject *__pyx_v_tot = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_from_intervals (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_intervals,&__pyx_n_s_tot,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_intervals,&__pyx_n_s_tot,0};
     PyObject* values[2] = {0,0};
     values[0] = ((PyObject *)Py_None);
     values[1] = ((PyObject *)__pyx_int_0);
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_intervals);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_intervals);
           if (value) { values[0] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tot);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tot);
           if (value) { values[1] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_from_intervals") < 0)) __PYX_ERR(0, 165, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_from_intervals") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_intervals = values[0];
     __pyx_v_tot = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_from_intervals", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 165, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_from_intervals", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 166, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed._from_intervals", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_8_from_intervals(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_cls), __pyx_v_intervals, __pyx_v_tot);
 
@@ -3642,110 +5184,113 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *(*__pyx_t_11)(PyObject *);
-  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_from_intervals", 0);
 
-  /* "rbi_tree/tree.pyx":166
+  /* "rbi_tree/tree.pyx":167
  * 
  *     def _from_intervals(cls, intervals=None, tot=0):
  *         tree = cls(tot)             # <<<<<<<<<<<<<<
  *         if not intervals is None:
  *             for start, end, val in intervals:
  */
-  __Pyx_INCREF(((PyObject *)__pyx_v_cls));
+  __Pyx_INCREF((PyObject *)__pyx_v_cls);
   __pyx_t_2 = ((PyObject *)__pyx_v_cls); __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_tot) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_tot);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_tot};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   __pyx_v_tree = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":167
+  /* "rbi_tree/tree.pyx":168
  *     def _from_intervals(cls, intervals=None, tot=0):
  *         tree = cls(tot)
  *         if not intervals is None:             # <<<<<<<<<<<<<<
  *             for start, end, val in intervals:
  *                 tree._insert(start, end, val)
  */
-  __pyx_t_4 = (__pyx_v_intervals != Py_None);
-  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_5 = (__pyx_v_intervals != Py_None);
   if (__pyx_t_5) {
 
-    /* "rbi_tree/tree.pyx":168
+    /* "rbi_tree/tree.pyx":169
  *         tree = cls(tot)
  *         if not intervals is None:
  *             for start, end, val in intervals:             # <<<<<<<<<<<<<<
  *                 tree._insert(start, end, val)
  * 
  */
     if (likely(PyList_CheckExact(__pyx_v_intervals)) || PyTuple_CheckExact(__pyx_v_intervals)) {
       __pyx_t_1 = __pyx_v_intervals; __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_intervals); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_intervals); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 169, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 169, __pyx_L1_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_7(__pyx_t_1);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 168, __pyx_L1_error)
+            else __PYX_ERR(0, 169, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 3)) {
           if (size > 3) __Pyx_RaiseTooManyValuesError(3);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 168, __pyx_L1_error)
+          __PYX_ERR(0, 169, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_9 = PyTuple_GET_ITEM(sequence, 2); 
         } else {
@@ -3753,143 +5298,115 @@
           __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
           __pyx_t_9 = PyList_GET_ITEM(sequence, 2); 
         }
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_9);
         #else
-        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 169, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 169, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+        __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 169, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
+        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_10);
         index = 0; __pyx_t_3 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_3)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_3);
         index = 1; __pyx_t_8 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_8)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_8);
         index = 2; __pyx_t_9 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_9)) goto __pyx_L6_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_9);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 3) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 3) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
         __pyx_t_11 = NULL;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L7_unpacking_done;
         __pyx_L6_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 168, __pyx_L1_error)
+        __PYX_ERR(0, 169, __pyx_L1_error)
         __pyx_L7_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_start, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_end, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "rbi_tree/tree.pyx":169
+      /* "rbi_tree/tree.pyx":170
  *         if not intervals is None:
  *             for start, end, val in intervals:
  *                 tree._insert(start, end, val)             # <<<<<<<<<<<<<<
  * 
  *         return tree
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_tree, __pyx_n_s_insert_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_tree, __pyx_n_s_insert_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_8 = NULL;
-      __pyx_t_12 = 0;
+      __pyx_t_4 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_12 = 1;
+          __pyx_t_4 = 1;
         }
       }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-      } else
-      #endif
       {
-        __pyx_t_3 = PyTuple_New(3+__pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        if (__pyx_t_8) {
-          __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_8); __pyx_t_8 = NULL;
-        }
-        __Pyx_INCREF(__pyx_v_start);
-        __Pyx_GIVEREF(__pyx_v_start);
-        PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_12, __pyx_v_start);
-        __Pyx_INCREF(__pyx_v_end);
-        __Pyx_GIVEREF(__pyx_v_end);
-        PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_12, __pyx_v_end);
-        __Pyx_INCREF(__pyx_v_val);
-        __Pyx_GIVEREF(__pyx_v_val);
-        PyTuple_SET_ITEM(__pyx_t_3, 2+__pyx_t_12, __pyx_v_val);
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+        PyObject *__pyx_callargs[4] = {__pyx_t_8, __pyx_v_start, __pyx_v_end, __pyx_v_val};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "rbi_tree/tree.pyx":168
+      /* "rbi_tree/tree.pyx":169
  *         tree = cls(tot)
  *         if not intervals is None:
  *             for start, end, val in intervals:             # <<<<<<<<<<<<<<
  *                 tree._insert(start, end, val)
  * 
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "rbi_tree/tree.pyx":167
+    /* "rbi_tree/tree.pyx":168
  *     def _from_intervals(cls, intervals=None, tot=0):
  *         tree = cls(tot)
  *         if not intervals is None:             # <<<<<<<<<<<<<<
  *             for start, end, val in intervals:
  *                 tree._insert(start, end, val)
  */
   }
 
-  /* "rbi_tree/tree.pyx":171
+  /* "rbi_tree/tree.pyx":172
  *                 tree._insert(start, end, val)
  * 
  *         return tree             # <<<<<<<<<<<<<<
  *     _from_intervals = classmethod(_from_intervals)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_tree);
   __pyx_r = __pyx_v_tree;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":165
+  /* "rbi_tree/tree.pyx":166
  *         return (ITreed._from_intervals, (intervals, self.tot))
  * 
  *     def _from_intervals(cls, intervals=None, tot=0):             # <<<<<<<<<<<<<<
  *         tree = cls(tot)
  *         if not intervals is None:
  */
 
@@ -3909,85 +5426,105 @@
   __Pyx_XDECREF(__pyx_v_end);
   __Pyx_XDECREF(__pyx_v_val);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":175
+/* "rbi_tree/tree.pyx":176
  * 
  * 
  *     def _insert(self, start, end, value):             # <<<<<<<<<<<<<<
  *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
  *         self.tree.insert(deref(ivl))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_11_insert = {"_insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_start = 0;
   PyObject *__pyx_v_end = 0;
   PyObject *__pyx_v_value = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_insert (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,&__pyx_n_s_value,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,&__pyx_n_s_value,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, 1); __PYX_ERR(0, 175, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, 1); __PYX_ERR(0, 176, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, 2); __PYX_ERR(0, 175, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, 2); __PYX_ERR(0, 176, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_insert") < 0)) __PYX_ERR(0, 175, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_insert") < 0)) __PYX_ERR(0, 176, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+    } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_start = values[0];
     __pyx_v_end = values[1];
     __pyx_v_value = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 175, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_insert", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 176, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed._insert", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_10_insert(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_start, __pyx_v_end, __pyx_v_value);
 
@@ -4006,65 +5543,65 @@
   __pyx_t_8rbi_tree_4tree_keyval __pyx_t_4;
   std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::iterator __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_insert", 0);
 
-  /* "rbi_tree/tree.pyx":176
+  /* "rbi_tree/tree.pyx":177
  * 
  *     def _insert(self, start, end, value):
  *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)             # <<<<<<<<<<<<<<
  *         self.tree.insert(deref(ivl))
  *         self.datapos = self.ivldata.insert(self.datapos,
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_start); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_end); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_start); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_end); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
   __pyx_v_ivl = new __pyx_t_8rbi_tree_4tree_CIntervalInt(__pyx_t_1, __pyx_t_2, __pyx_t_3);
 
-  /* "rbi_tree/tree.pyx":177
+  /* "rbi_tree/tree.pyx":178
  *     def _insert(self, start, end, value):
  *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
  *         self.tree.insert(deref(ivl))             # <<<<<<<<<<<<<<
  *         self.datapos = self.ivldata.insert(self.datapos,
  *                             keyval(ivl.value, ivl))
  */
   (void)(__pyx_v_self->tree->insert((*__pyx_v_ivl)));
 
-  /* "rbi_tree/tree.pyx":179
+  /* "rbi_tree/tree.pyx":180
  *         self.tree.insert(deref(ivl))
  *         self.datapos = self.ivldata.insert(self.datapos,
  *                             keyval(ivl.value, ivl))             # <<<<<<<<<<<<<<
  * 
  *     def insert(self, start, end):
  */
   try {
     __pyx_t_4 = __pyx_t_8rbi_tree_4tree_keyval(__pyx_v_ivl->value, __pyx_v_ivl);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 179, __pyx_L1_error)
+    __PYX_ERR(0, 180, __pyx_L1_error)
   }
 
-  /* "rbi_tree/tree.pyx":178
+  /* "rbi_tree/tree.pyx":179
  *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
  *         self.tree.insert(deref(ivl))
  *         self.datapos = self.ivldata.insert(self.datapos,             # <<<<<<<<<<<<<<
  *                             keyval(ivl.value, ivl))
  * 
  */
   try {
     __pyx_t_5 = __pyx_v_self->ivldata.insert(__pyx_v_self->datapos, __pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 178, __pyx_L1_error)
+    __PYX_ERR(0, 179, __pyx_L1_error)
   }
-  __pyx_v_self->datapos = __pyx_t_5;
+  __pyx_v_self->datapos = __PYX_STD_MOVE_IF_SUPPORTED(((std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::const_iterator)__pyx_t_5));
 
-  /* "rbi_tree/tree.pyx":175
+  /* "rbi_tree/tree.pyx":176
  * 
  * 
  *     def _insert(self, start, end, value):             # <<<<<<<<<<<<<<
  *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
  *         self.tree.insert(deref(ivl))
  */
 
@@ -4076,75 +5613,94 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":181
+/* "rbi_tree/tree.pyx":182
  *                             keyval(ivl.value, ivl))
  * 
  *     def insert(self, start, end):             # <<<<<<<<<<<<<<
  *         """Insert an interval [start, end) and returns an id
  *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_13insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_12insert[] = "Insert an interval [start, end) and returns an id\n        of the interval. Ids are incrementing integers, i.e. 0,1,2 etc.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_13insert(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_13insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_12insert, "Insert an interval [start, end) and returns an id\n        of the interval. Ids are incrementing integers, i.e. 0,1,2 etc.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_13insert = {"insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_13insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_12insert};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_13insert(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_start = 0;
   PyObject *__pyx_v_end = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("insert (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("insert", 1, 2, 2, 1); __PYX_ERR(0, 181, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("insert", 1, 2, 2, 1); __PYX_ERR(0, 182, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "insert") < 0)) __PYX_ERR(0, 181, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "insert") < 0)) __PYX_ERR(0, 182, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_start = values[0];
     __pyx_v_end = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("insert", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 181, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("insert", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 182, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.insert", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_12insert(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_start, __pyx_v_end);
 
@@ -4158,146 +5714,115 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("insert", 0);
 
-  /* "rbi_tree/tree.pyx":184
+  /* "rbi_tree/tree.pyx":185
  *         """Insert an interval [start, end) and returns an id
  *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
  *         cdef int ivl_id = self.tot             # <<<<<<<<<<<<<<
  *         self._insert(start, end, ivl_id)
  *         self.tot += 1
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_self->tot); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_self->tot); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L1_error)
   __pyx_v_ivl_id = __pyx_t_1;
 
-  /* "rbi_tree/tree.pyx":185
+  /* "rbi_tree/tree.pyx":186
  *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
  *         cdef int ivl_id = self.tot
  *         self._insert(start, end, ivl_id)             # <<<<<<<<<<<<<<
  *         self.tot += 1
  *         return ivl_id
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ivl_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ivl_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_1 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_1 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_start, __pyx_v_end, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_1, 3+__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_start, __pyx_v_end, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_1, 3+__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[4] = {__pyx_t_5, __pyx_v_start, __pyx_v_end, __pyx_t_4};
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 3+__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
-    }
-    __Pyx_INCREF(__pyx_v_start);
-    __Pyx_GIVEREF(__pyx_v_start);
-    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_1, __pyx_v_start);
-    __Pyx_INCREF(__pyx_v_end);
-    __Pyx_GIVEREF(__pyx_v_end);
-    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_1, __pyx_v_end);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_1, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "rbi_tree/tree.pyx":186
+  /* "rbi_tree/tree.pyx":187
  *         cdef int ivl_id = self.tot
  *         self._insert(start, end, ivl_id)
  *         self.tot += 1             # <<<<<<<<<<<<<<
  *         return ivl_id
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_self->tot, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_self->tot, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->tot);
   __Pyx_DECREF(__pyx_v_self->tot);
   __pyx_v_self->tot = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "rbi_tree/tree.pyx":187
+  /* "rbi_tree/tree.pyx":188
  *         self._insert(start, end, ivl_id)
  *         self.tot += 1
  *         return ivl_id             # <<<<<<<<<<<<<<
  * 
  *     cdef CIntervalInt* _get_interval(self, id):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ivl_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ivl_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":181
+  /* "rbi_tree/tree.pyx":182
  *                             keyval(ivl.value, ivl))
  * 
  *     def insert(self, start, end):             # <<<<<<<<<<<<<<
  *         """Insert an interval [start, end) and returns an id
  *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.insert", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":189
+/* "rbi_tree/tree.pyx":190
  *         return ivl_id
  * 
  *     cdef CIntervalInt* _get_interval(self, id):             # <<<<<<<<<<<<<<
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)
  *         if it != self.ivldata.end():
  */
 
@@ -4308,143 +5833,162 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_interval", 0);
 
-  /* "rbi_tree/tree.pyx":190
+  /* "rbi_tree/tree.pyx":191
  * 
  *     cdef CIntervalInt* _get_interval(self, id):
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)             # <<<<<<<<<<<<<<
  *         if it != self.ivldata.end():
  *             return deref(it).second
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_id); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_id); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_v_it = __pyx_v_self->ivldata.find(__pyx_t_1);
 
-  /* "rbi_tree/tree.pyx":191
+  /* "rbi_tree/tree.pyx":192
  *     cdef CIntervalInt* _get_interval(self, id):
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)
  *         if it != self.ivldata.end():             # <<<<<<<<<<<<<<
  *             return deref(it).second
  *         else:
  */
-  __pyx_t_2 = ((__pyx_v_it != __pyx_v_self->ivldata.end()) != 0);
+  __pyx_t_2 = (__pyx_v_it != __pyx_v_self->ivldata.end());
   if (__pyx_t_2) {
 
-    /* "rbi_tree/tree.pyx":192
+    /* "rbi_tree/tree.pyx":193
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)
  *         if it != self.ivldata.end():
  *             return deref(it).second             # <<<<<<<<<<<<<<
  *         else:
  *             return NULL
  */
     __pyx_r = (*__pyx_v_it).second;
     goto __pyx_L0;
 
-    /* "rbi_tree/tree.pyx":191
+    /* "rbi_tree/tree.pyx":192
  *     cdef CIntervalInt* _get_interval(self, id):
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)
  *         if it != self.ivldata.end():             # <<<<<<<<<<<<<<
  *             return deref(it).second
  *         else:
  */
   }
 
-  /* "rbi_tree/tree.pyx":194
+  /* "rbi_tree/tree.pyx":195
  *             return deref(it).second
  *         else:
  *             return NULL             # <<<<<<<<<<<<<<
  * 
  *     def find(self, int start, int end):
  */
   /*else*/ {
     __pyx_r = NULL;
     goto __pyx_L0;
   }
 
-  /* "rbi_tree/tree.pyx":189
+  /* "rbi_tree/tree.pyx":190
  *         return ivl_id
  * 
  *     cdef CIntervalInt* _get_interval(self, id):             # <<<<<<<<<<<<<<
  *         cdef map[int, CIntervalInt*].iterator it = self.ivldata.find(id)
  *         if it != self.ivldata.end():
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_WriteUnraisable("rbi_tree.tree.ITreed._get_interval", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_AddTraceback("rbi_tree.tree.ITreed._get_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":196
+/* "rbi_tree/tree.pyx":197
  *             return NULL
  * 
  *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_15find(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_14find[] = "Search intervals overlapping [start, end). Returns list of \n        overlapping intervals' ids.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_15find(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_15find(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_14find, "Search intervals overlapping [start, end). Returns list of \n        overlapping intervals' ids.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_15find = {"find", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_15find, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_14find};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_15find(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_start;
   int __pyx_v_end;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_start,&__pyx_n_s_end,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, 1); __PYX_ERR(0, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, 1); __PYX_ERR(0, 197, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "find") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "find") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L3_error)
-    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 196, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("find", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 197, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.find", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_14find(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_start, __pyx_v_end);
 
@@ -4468,150 +6012,150 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find", 0);
 
-  /* "rbi_tree/tree.pyx":199
+  /* "rbi_tree/tree.pyx":200
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  *         cdef CIntervalInt* ivl = new CIntervalInt(start,end)             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalInt] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  */
   __pyx_v_ivl = new __pyx_t_8rbi_tree_4tree_CIntervalInt(__pyx_v_start, __pyx_v_end);
 
-  /* "rbi_tree/tree.pyx":201
+  /* "rbi_tree/tree.pyx":202
  *         cdef CIntervalInt* ivl = new CIntervalInt(start,end)
  *         cdef vector[CIntervalInt] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)             # <<<<<<<<<<<<<<
  *         del ivl
  *         a = []
  */
   __pyx_v_self->tree->findOverlappingIntervals((*__pyx_v_ivl), __pyx_v_out);
 
-  /* "rbi_tree/tree.pyx":202
+  /* "rbi_tree/tree.pyx":203
  *         cdef vector[CIntervalInt] out
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  *         del ivl             # <<<<<<<<<<<<<<
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  */
   delete __pyx_v_ivl;
 
-  /* "rbi_tree/tree.pyx":203
+  /* "rbi_tree/tree.pyx":204
  *         self.tree.findOverlappingIntervals(deref(ivl), out)
  *         del ivl
  *         a = []             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_a = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":204
+  /* "rbi_tree/tree.pyx":205
  *         del ivl
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()             # <<<<<<<<<<<<<<
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  */
   __pyx_v_it = __pyx_v_out.begin();
 
-  /* "rbi_tree/tree.pyx":205
+  /* "rbi_tree/tree.pyx":206
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():             # <<<<<<<<<<<<<<
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:
  */
   while (1) {
-    __pyx_t_2 = ((__pyx_v_it != __pyx_v_out.end()) != 0);
+    __pyx_t_2 = (__pyx_v_it != __pyx_v_out.end());
     if (!__pyx_t_2) break;
 
-    /* "rbi_tree/tree.pyx":207
+    /* "rbi_tree/tree.pyx":208
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  */
-    __pyx_t_3 = (((*__pyx_v_it).high != __pyx_v_start) != 0);
+    __pyx_t_3 = ((*__pyx_v_it).high != __pyx_v_start);
     if (__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L6_bool_binop_done;
     }
-    __pyx_t_3 = (((*__pyx_v_it).low != __pyx_v_end) != 0);
+    __pyx_t_3 = ((*__pyx_v_it).low != __pyx_v_end);
     __pyx_t_2 = __pyx_t_3;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "rbi_tree/tree.pyx":208
+      /* "rbi_tree/tree.pyx":209
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )             # <<<<<<<<<<<<<<
  *             inc(it)
  *         return a
  */
-      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_int((*__pyx_v_it).value); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int((*__pyx_v_it).value); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_5);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 208, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "rbi_tree/tree.pyx":207
+      /* "rbi_tree/tree.pyx":208
  *         while it != out.end():
  *             # Have to exclude for the sake of half-openness
  *             if deref(it).high!=start and deref(it).low!=end:             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  */
     }
 
-    /* "rbi_tree/tree.pyx":209
+    /* "rbi_tree/tree.pyx":210
  *             if deref(it).high!=start and deref(it).low!=end:
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)             # <<<<<<<<<<<<<<
  *         return a
  * 
  */
     (void)((++__pyx_v_it));
   }
 
-  /* "rbi_tree/tree.pyx":210
+  /* "rbi_tree/tree.pyx":211
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  *         return a             # <<<<<<<<<<<<<<
  * 
  *     def get_ivl(self, id):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_a);
   __pyx_r = __pyx_v_a;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":196
+  /* "rbi_tree/tree.pyx":197
  *             return NULL
  * 
  *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
  *         """Search intervals overlapping [start, end). Returns list of
  *         overlapping intervals' ids."""
  */
 
@@ -4626,131 +6170,236 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":212
+/* "rbi_tree/tree.pyx":213
  *         return a
  * 
  *     def get_ivl(self, id):             # <<<<<<<<<<<<<<
  *         """Return a list [start,end] of the interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl(PyObject *__pyx_v_self, PyObject *__pyx_v_id); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_16get_ivl[] = "Return a list [start,end] of the interval with specified id.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl(PyObject *__pyx_v_self, PyObject *__pyx_v_id) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_16get_ivl, "Return a list [start,end] of the interval with specified id.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_17get_ivl = {"get_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_16get_ivl};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_id = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_ivl (wrapper)", 0);
-  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_16get_ivl(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), ((PyObject *)__pyx_v_id));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_id,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_id)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_ivl") < 0)) __PYX_ERR(0, 213, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_id = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("get_ivl", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 213, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rbi_tree.tree.ITreed.get_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_16get_ivl(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_id);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_16get_ivl(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, PyObject *__pyx_v_id) {
   __pyx_t_8rbi_tree_4tree_CIntervalInt *__pyx_v_ivl;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  __pyx_t_8rbi_tree_4tree_CIntervalInt *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_ivl", 0);
 
-  /* "rbi_tree/tree.pyx":214
+  /* "rbi_tree/tree.pyx":215
  *     def get_ivl(self, id):
  *         """Return a list [start,end] of the interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)             # <<<<<<<<<<<<<<
  *         return [deref(ivl).low, deref(ivl).high]
  * 
  */
-  __pyx_v_ivl = ((struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *)__pyx_v_self->__pyx_vtab)->_get_interval(__pyx_v_self, __pyx_v_id);
+  __pyx_t_1 = ((struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *)__pyx_v_self->__pyx_vtab)->_get_interval(__pyx_v_self, __pyx_v_id); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_v_ivl = __pyx_t_1;
 
-  /* "rbi_tree/tree.pyx":215
+  /* "rbi_tree/tree.pyx":216
  *         """Return a list [start,end] of the interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  *         return [deref(ivl).low, deref(ivl).high]             # <<<<<<<<<<<<<<
  * 
  *     def find_at(self, int point):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_ivl).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int((*__pyx_v_ivl).high); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int((*__pyx_v_ivl).low); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_v_ivl).high); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
-  __pyx_t_1 = 0;
+  PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":212
+  /* "rbi_tree/tree.pyx":213
  *         return a
  * 
  *     def get_ivl(self, id):             # <<<<<<<<<<<<<<
  *         """Return a list [start,end] of the interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.get_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":217
+/* "rbi_tree/tree.pyx":218
  *         return [deref(ivl).low, deref(ivl).high]
  * 
  *     def find_at(self, int point):             # <<<<<<<<<<<<<<
  *         """Search for intervals containing specified point. Returns list of
  *         overlapping intervals' ids."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at(PyObject *__pyx_v_self, PyObject *__pyx_arg_point); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_18find_at[] = "Search for intervals containing specified point. Returns list of \n        overlapping intervals' ids.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at(PyObject *__pyx_v_self, PyObject *__pyx_arg_point) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_18find_at, "Search for intervals containing specified point. Returns list of \n        overlapping intervals' ids.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_19find_at = {"find_at", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_18find_at};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_point;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_at (wrapper)", 0);
-  assert(__pyx_arg_point); {
-    __pyx_v_point = __Pyx_PyInt_As_int(__pyx_arg_point); if (unlikely((__pyx_v_point == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_point,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_point)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "find_at") < 0)) __PYX_ERR(0, 218, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_point = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_point == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("find_at", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 218, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.find_at", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_18find_at(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), ((int)__pyx_v_point));
+  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_18find_at(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_point);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_18find_at(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, int __pyx_v_point) {
@@ -4766,124 +6415,124 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_at", 0);
 
-  /* "rbi_tree/tree.pyx":221
+  /* "rbi_tree/tree.pyx":222
  *         overlapping intervals' ids."""
  *         cdef vector[CIntervalInt] out
  *         self.tree.findIntervalsContainPoint(point, out)             # <<<<<<<<<<<<<<
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  */
   __pyx_v_self->tree->findIntervalsContainPoint(__pyx_v_point, __pyx_v_out);
 
-  /* "rbi_tree/tree.pyx":222
+  /* "rbi_tree/tree.pyx":223
  *         cdef vector[CIntervalInt] out
  *         self.tree.findIntervalsContainPoint(point, out)
  *         a = []             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_a = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbi_tree/tree.pyx":223
+  /* "rbi_tree/tree.pyx":224
  *         self.tree.findIntervalsContainPoint(point, out)
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()             # <<<<<<<<<<<<<<
  *         while it != out.end():
  *             if not deref(it).high == point:
  */
   __pyx_v_it = __pyx_v_out.begin();
 
-  /* "rbi_tree/tree.pyx":224
+  /* "rbi_tree/tree.pyx":225
  *         a = []
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():             # <<<<<<<<<<<<<<
  *             if not deref(it).high == point:
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  */
   while (1) {
-    __pyx_t_2 = ((__pyx_v_it != __pyx_v_out.end()) != 0);
+    __pyx_t_2 = (__pyx_v_it != __pyx_v_out.end());
     if (!__pyx_t_2) break;
 
-    /* "rbi_tree/tree.pyx":225
+    /* "rbi_tree/tree.pyx":226
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():
  *             if not deref(it).high == point:             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  */
-    __pyx_t_2 = ((!(((*__pyx_v_it).high == __pyx_v_point) != 0)) != 0);
+    __pyx_t_2 = (!((*__pyx_v_it).high == __pyx_v_point));
     if (__pyx_t_2) {
 
-      /* "rbi_tree/tree.pyx":226
+      /* "rbi_tree/tree.pyx":227
  *         while it != out.end():
  *             if not deref(it).high == point:
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )             # <<<<<<<<<<<<<<
  *             inc(it)
  *         return a
  */
-      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_int((*__pyx_v_it).low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_v_it).high); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_v_it).value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
       __pyx_t_1 = 0;
       __pyx_t_3 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 226, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_a, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 227, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "rbi_tree/tree.pyx":225
+      /* "rbi_tree/tree.pyx":226
  *         cdef vector[CIntervalInt].iterator it = out.begin()
  *         while it != out.end():
  *             if not deref(it).high == point:             # <<<<<<<<<<<<<<
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  */
     }
 
-    /* "rbi_tree/tree.pyx":227
+    /* "rbi_tree/tree.pyx":228
  *             if not deref(it).high == point:
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)             # <<<<<<<<<<<<<<
  *         return a
  * 
  */
     (void)((++__pyx_v_it));
   }
 
-  /* "rbi_tree/tree.pyx":228
+  /* "rbi_tree/tree.pyx":229
  *                 a.append( (deref(it).low, deref(it).high, deref(it).value) )
  *             inc(it)
  *         return a             # <<<<<<<<<<<<<<
  * 
  *     def remove(self, int id):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_a);
   __pyx_r = __pyx_v_a;
   goto __pyx_L0;
 
-  /* "rbi_tree/tree.pyx":217
+  /* "rbi_tree/tree.pyx":218
  *         return [deref(ivl).low, deref(ivl).high]
  * 
  *     def find_at(self, int point):             # <<<<<<<<<<<<<<
  *         """Search for intervals containing specified point. Returns list of
  *         overlapping intervals' ids."""
  */
 
@@ -4898,133 +6547,180 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbi_tree/tree.pyx":230
+/* "rbi_tree/tree.pyx":231
  *         return a
  * 
  *     def remove(self, int id):             # <<<<<<<<<<<<<<
  *         """Delete interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_21remove(PyObject *__pyx_v_self, PyObject *__pyx_arg_id); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_20remove[] = "Delete interval with specified id.";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_21remove(PyObject *__pyx_v_self, PyObject *__pyx_arg_id) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_21remove(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_20remove, "Delete interval with specified id.");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_21remove = {"remove", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_21remove, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_20remove};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_21remove(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_id;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("remove (wrapper)", 0);
-  assert(__pyx_arg_id); {
-    __pyx_v_id = __Pyx_PyInt_As_int(__pyx_arg_id); if (unlikely((__pyx_v_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_id,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_id)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "remove") < 0)) __PYX_ERR(0, 231, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_id = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("remove", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 231, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.remove", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_20remove(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), ((int)__pyx_v_id));
+  __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_20remove(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self), __pyx_v_id);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8rbi_tree_4tree_6ITreed_20remove(struct __pyx_obj_8rbi_tree_4tree_ITreed *__pyx_v_self, int __pyx_v_id) {
   __pyx_t_8rbi_tree_4tree_CIntervalInt *__pyx_v_ivl;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  __pyx_t_8rbi_tree_4tree_CIntervalInt *__pyx_t_2;
+  int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("remove", 0);
 
-  /* "rbi_tree/tree.pyx":232
+  /* "rbi_tree/tree.pyx":233
  *     def remove(self, int id):
  *         """Delete interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)             # <<<<<<<<<<<<<<
  *         if not ivl is NULL:
  *             self.tree.remove(deref(ivl))
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_ivl = ((struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *)__pyx_v_self->__pyx_vtab)->_get_interval(__pyx_v_self, __pyx_t_1);
+  __pyx_t_2 = ((struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed *)__pyx_v_self->__pyx_vtab)->_get_interval(__pyx_v_self, __pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_ivl = __pyx_t_2;
 
-  /* "rbi_tree/tree.pyx":233
+  /* "rbi_tree/tree.pyx":234
  *         """Delete interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  *         if not ivl is NULL:             # <<<<<<<<<<<<<<
  *             self.tree.remove(deref(ivl))
  *         else:
  */
-  __pyx_t_2 = ((__pyx_v_ivl != NULL) != 0);
-  if (likely(__pyx_t_2)) {
+  __pyx_t_3 = (__pyx_v_ivl != NULL);
+  if (likely(__pyx_t_3)) {
 
-    /* "rbi_tree/tree.pyx":234
+    /* "rbi_tree/tree.pyx":235
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  *         if not ivl is NULL:
  *             self.tree.remove(deref(ivl))             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError
  */
     (void)(__pyx_v_self->tree->remove((*__pyx_v_ivl)));
 
-    /* "rbi_tree/tree.pyx":233
+    /* "rbi_tree/tree.pyx":234
  *         """Delete interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  *         if not ivl is NULL:             # <<<<<<<<<<<<<<
  *             self.tree.remove(deref(ivl))
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "rbi_tree/tree.pyx":236
+  /* "rbi_tree/tree.pyx":237
  *             self.tree.remove(deref(ivl))
  *         else:
  *             raise ValueError             # <<<<<<<<<<<<<<
  *         self.ivldata.erase(id)
  *         del ivl
  */
   /*else*/ {
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-    __PYX_ERR(0, 236, __pyx_L1_error)
+    __PYX_ERR(0, 237, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "rbi_tree/tree.pyx":237
+  /* "rbi_tree/tree.pyx":238
  *         else:
  *             raise ValueError
  *         self.ivldata.erase(id)             # <<<<<<<<<<<<<<
  *         del ivl
  * 
  */
   (void)(__pyx_v_self->ivldata.erase(__pyx_v_id));
 
-  /* "rbi_tree/tree.pyx":238
+  /* "rbi_tree/tree.pyx":239
  *             raise ValueError
  *         self.ivldata.erase(id)
  *         del ivl             # <<<<<<<<<<<<<<
  * 
  *     def iter_ivl(self):
  */
   delete __pyx_v_ivl;
 
-  /* "rbi_tree/tree.pyx":230
+  /* "rbi_tree/tree.pyx":231
  *         return a
  * 
  *     def remove(self, int id):             # <<<<<<<<<<<<<<
  *         """Delete interval with specified id."""
  *         cdef CIntervalInt* ivl = self._get_interval(id)
  */
 
@@ -5038,29 +6734,49 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8rbi_tree_4tree_6ITreed_24generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "rbi_tree/tree.pyx":240
+/* "rbi_tree/tree.pyx":241
  *         del ivl
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_8rbi_tree_4tree_6ITreed_22iter_ivl[] = "Iterate over all intervals. Yields tuples (start, end, id).";
-static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_8rbi_tree_4tree_6ITreed_22iter_ivl, "Iterate over all intervals. Yields tuples (start, end, id).");
+static PyMethodDef __pyx_mdef_8rbi_tree_4tree_6ITreed_23iter_ivl = {"iter_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_22iter_ivl};
+static PyObject *__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("iter_ivl (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("iter_ivl", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "iter_ivl", 0))) return NULL;
   __pyx_r = __pyx_pf_8rbi_tree_4tree_6ITreed_22iter_ivl(((struct __pyx_obj_8rbi_tree_4tree_ITreed *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5072,33 +6788,33 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("iter_ivl", 0);
   __pyx_cur_scope = (struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl(__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 240, __pyx_L1_error)
+    __PYX_ERR(0, 241, __pyx_L1_error)
   } else {
-    __Pyx_GOTREF(__pyx_cur_scope);
+    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8rbi_tree_4tree_6ITreed_24generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_ivl, __pyx_n_s_ITreed_iter_ivl, __pyx_n_s_rbi_tree_tree); if (unlikely(!gen)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8rbi_tree_4tree_6ITreed_24generator1, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter_ivl, __pyx_n_s_ITreed_iter_ivl, __pyx_n_s_rbi_tree_tree); if (unlikely(!gen)) __PYX_ERR(0, 241, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbi_tree.tree.ITreed.iter_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
-  __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
+  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_gb_8rbi_tree_4tree_6ITreed_24generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
@@ -5118,58 +6834,58 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 240, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 241, __pyx_L1_error)
 
-  /* "rbi_tree/tree.pyx":242
+  /* "rbi_tree/tree.pyx":243
  *     def iter_ivl(self):
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()             # <<<<<<<<<<<<<<
  *         cdef vector[CIntervalInt].iterator it = intervals.begin()
  *         while it != intervals.end():
  */
   __pyx_cur_scope->__pyx_v_intervals = __pyx_cur_scope->__pyx_v_self->tree->intervals();
 
-  /* "rbi_tree/tree.pyx":243
+  /* "rbi_tree/tree.pyx":244
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
  *         cdef vector[CIntervalInt].iterator it = intervals.begin()             # <<<<<<<<<<<<<<
  *         while it != intervals.end():
  *             yield (deref(it).low, deref(it).high, deref(it).value)
  */
   __pyx_cur_scope->__pyx_v_it = __pyx_cur_scope->__pyx_v_intervals.begin();
 
-  /* "rbi_tree/tree.pyx":244
+  /* "rbi_tree/tree.pyx":245
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
  *         cdef vector[CIntervalInt].iterator it = intervals.begin()
  *         while it != intervals.end():             # <<<<<<<<<<<<<<
  *             yield (deref(it).low, deref(it).high, deref(it).value)
  *             inc(it)
  */
   while (1) {
-    __pyx_t_1 = ((__pyx_cur_scope->__pyx_v_it != __pyx_cur_scope->__pyx_v_intervals.end()) != 0);
+    __pyx_t_1 = (__pyx_cur_scope->__pyx_v_it != __pyx_cur_scope->__pyx_v_intervals.end());
     if (!__pyx_t_1) break;
 
-    /* "rbi_tree/tree.pyx":245
+    /* "rbi_tree/tree.pyx":246
  *         cdef vector[CIntervalInt].iterator it = intervals.begin()
  *         while it != intervals.end():
  *             yield (deref(it).low, deref(it).high, deref(it).value)             # <<<<<<<<<<<<<<
  *             inc(it)
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).low); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).low); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).high); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).high); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int((*__pyx_cur_scope->__pyx_v_it).value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
@@ -5181,37 +6897,38 @@
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 245, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 246, __pyx_L1_error)
 
-    /* "rbi_tree/tree.pyx":246
+    /* "rbi_tree/tree.pyx":247
  *         while it != intervals.end():
  *             yield (deref(it).low, deref(it).high, deref(it).value)
  *             inc(it)             # <<<<<<<<<<<<<<
  */
     (void)((++__pyx_cur_scope->__pyx_v_it));
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "rbi_tree/tree.pyx":240
+  /* "rbi_tree/tree.pyx":241
  *         del ivl
  * 
  *     def iter_ivl(self):             # <<<<<<<<<<<<<<
  *         """Iterate over all intervals. Yields tuples (start, end, id)."""
  *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_Generator_Replace_StopIteration(0);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("iter_ivl", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
@@ -5222,57 +6939,79 @@
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_tp_new_8rbi_tree_4tree_ITree(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   if (unlikely(__pyx_pw_8rbi_tree_4tree_5ITree_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_8rbi_tree_4tree_ITree(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8rbi_tree_4tree_ITree) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_8rbi_tree_4tree_5ITree_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_8rbi_tree_4tree_ITree[] = {
-  {"__reduce__", (PyCFunction)__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__, METH_NOARGS, 0},
-  {"insert", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_7insert, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_6insert},
-  {"find", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_9find, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_8find},
-  {"_from_intervals", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals, METH_VARARGS|METH_KEYWORDS, 0},
-  {"find_at", (PyCFunction)__pyx_pw_8rbi_tree_4tree_5ITree_13find_at, METH_O, __pyx_doc_8rbi_tree_4tree_5ITree_12find_at},
-  {"iter_ivl", (PyCFunction)__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl, METH_NOARGS, __pyx_doc_8rbi_tree_4tree_5ITree_14iter_ivl},
+  {"__reduce__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_5__reduce__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_7insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_6insert},
+  {"find", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_9find, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_8find},
+  {"_from_intervals", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_11_from_intervals, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"find_at", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_13find_at, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_12find_at},
+  {"iter_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_5ITree_15iter_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_5ITree_14iter_ivl},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8rbi_tree_4tree_ITree_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8rbi_tree_4tree_ITree},
+  {Py_tp_methods, (void *)__pyx_methods_8rbi_tree_4tree_ITree},
+  {Py_tp_new, (void *)__pyx_tp_new_8rbi_tree_4tree_ITree},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8rbi_tree_4tree_ITree_spec = {
+  "rbi_tree.tree.ITree",
+  sizeof(struct __pyx_obj_8rbi_tree_4tree_ITree),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
+  __pyx_type_8rbi_tree_4tree_ITree_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_8rbi_tree_4tree_ITree = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rbi_tree.tree.ITree", /*tp_name*/
+  "rbi_tree.tree.""ITree", /*tp_name*/
   sizeof(struct __pyx_obj_8rbi_tree_4tree_ITree), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8rbi_tree_4tree_ITree, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -5307,65 +7046,85 @@
   __pyx_methods_8rbi_tree_4tree_ITree, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_8rbi_tree_4tree_ITree, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 static struct __pyx_vtabstruct_8rbi_tree_4tree_ITreed __pyx_vtable_8rbi_tree_4tree_ITreed;
 
 static PyObject *__pyx_tp_new_8rbi_tree_4tree_ITreed(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8rbi_tree_4tree_ITreed *p;
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   p = ((struct __pyx_obj_8rbi_tree_4tree_ITreed *)o);
   p->__pyx_vtab = __pyx_vtabptr_8rbi_tree_4tree_ITreed;
   new((void*)&(p->ivldata)) __pyx_t_8rbi_tree_4tree_Ivlmap();
-  new((void*)&(p->datapos)) std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::iterator();
+  new((void*)&(p->datapos)) std::map<int,__pyx_t_8rbi_tree_4tree_CIntervalInt *> ::const_iterator();
   p->tot = Py_None; Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_8rbi_tree_4tree_6ITreed_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_8rbi_tree_4tree_ITreed(PyObject *o) {
   struct __pyx_obj_8rbi_tree_4tree_ITreed *p = (struct __pyx_obj_8rbi_tree_4tree_ITreed *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8rbi_tree_4tree_ITreed) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -5394,29 +7153,48 @@
   tmp = ((PyObject*)p->tot);
   p->tot = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyMethodDef __pyx_methods_8rbi_tree_4tree_ITreed[] = {
-  {"__reduce__", (PyCFunction)__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__, METH_NOARGS, 0},
-  {"_from_intervals", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_insert", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert, METH_VARARGS|METH_KEYWORDS, 0},
-  {"insert", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_13insert, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_12insert},
-  {"find", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_15find, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_14find},
-  {"get_ivl", (PyCFunction)__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl, METH_O, __pyx_doc_8rbi_tree_4tree_6ITreed_16get_ivl},
-  {"find_at", (PyCFunction)__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at, METH_O, __pyx_doc_8rbi_tree_4tree_6ITreed_18find_at},
-  {"remove", (PyCFunction)__pyx_pw_8rbi_tree_4tree_6ITreed_21remove, METH_O, __pyx_doc_8rbi_tree_4tree_6ITreed_20remove},
-  {"iter_ivl", (PyCFunction)__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl, METH_NOARGS, __pyx_doc_8rbi_tree_4tree_6ITreed_22iter_ivl},
+  {"__reduce__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_7__reduce__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"_from_intervals", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_9_from_intervals, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"_insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_11_insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"insert", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_13insert, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_12insert},
+  {"find", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_15find, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_14find},
+  {"get_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_17get_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_16get_ivl},
+  {"find_at", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_19find_at, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_18find_at},
+  {"remove", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_21remove, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_20remove},
+  {"iter_ivl", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8rbi_tree_4tree_6ITreed_23iter_ivl, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8rbi_tree_4tree_6ITreed_22iter_ivl},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8rbi_tree_4tree_ITreed_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8rbi_tree_4tree_ITreed},
+  {Py_tp_doc, (void *)PyDoc_STR("Version of ITree supporting deletion\n    ")},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_8rbi_tree_4tree_ITreed},
+  {Py_tp_clear, (void *)__pyx_tp_clear_8rbi_tree_4tree_ITreed},
+  {Py_tp_methods, (void *)__pyx_methods_8rbi_tree_4tree_ITreed},
+  {Py_tp_init, (void *)__pyx_pw_8rbi_tree_4tree_6ITreed_3__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_8rbi_tree_4tree_ITreed},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8rbi_tree_4tree_ITreed_spec = {
+  "rbi_tree.tree.ITreed",
+  sizeof(struct __pyx_obj_8rbi_tree_4tree_ITreed),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
+  __pyx_type_8rbi_tree_4tree_ITreed_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_8rbi_tree_4tree_ITreed = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rbi_tree.tree.ITreed", /*tp_name*/
+  "rbi_tree.tree.""ITreed", /*tp_name*/
   sizeof(struct __pyx_obj_8rbi_tree_4tree_ITreed), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8rbi_tree_4tree_ITreed, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -5437,81 +7215,106 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  0, /*tp_doc*/
+  PyDoc_STR("Version of ITree supporting deletion\n    "), /*tp_doc*/
   __pyx_tp_traverse_8rbi_tree_4tree_ITreed, /*tp_traverse*/
   __pyx_tp_clear_8rbi_tree_4tree_ITreed, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_8rbi_tree_4tree_ITreed, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   __pyx_pw_8rbi_tree_4tree_6ITreed_3__init__, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_8rbi_tree_4tree_ITreed, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *__pyx_freelist_8rbi_tree_4tree___pyx_scope_struct__iter_ivl[8];
 static int __pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl = 0;
 
 static PyObject *__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct__iter_ivl(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *p;
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl)))) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((int)(__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl)))) {
     o = (PyObject*)__pyx_freelist_8rbi_tree_4tree___pyx_scope_struct__iter_ivl[--__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl];
     memset(o, 0, sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
+  #endif
   p = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *)o);
   new((void*)&(p->__pyx_v_intervals)) std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj> ();
   new((void*)&(p->__pyx_v_it)) std::vector<__pyx_t_8rbi_tree_4tree_CIntervalObj> ::iterator();
   return o;
 }
 
 static void __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct__iter_ivl(PyObject *o) {
   struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *p = (struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct__iter_ivl) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_intervals);
   __Pyx_call_destructor(p->__pyx_v_it);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_val);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl)))) {
+  if (CYTHON_COMPILING_IN_CPYTHON && ((int)(__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl)))) {
     __pyx_freelist_8rbi_tree_4tree___pyx_scope_struct__iter_ivl[__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct__iter_ivl++] = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct__iter_ivl(PyObject *o, visitproc v, void *a) {
@@ -5521,18 +7324,33 @@
     e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
   }
   if (p->__pyx_v_val) {
     e = (*v)(p->__pyx_v_val, a); if (e) return e;
   }
   return 0;
 }
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct__iter_ivl},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct__iter_ivl},
+  {Py_tp_new, (void *)__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct__iter_ivl},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl_spec = {
+  "rbi_tree.tree.__pyx_scope_struct__iter_ivl",
+  sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rbi_tree.tree.__pyx_scope_struct__iter_ivl", /*tp_name*/
+  "rbi_tree.tree.""__pyx_scope_struct__iter_ivl", /*tp_name*/
   sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct__iter_ivl), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct__iter_ivl, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -5552,99 +7370,139 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct__iter_ivl, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct__iter_ivl, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *__pyx_freelist_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl[8];
 static int __pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl = 0;
 
 static PyObject *__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *p;
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl)))) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((int)(__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl)))) {
     o = (PyObject*)__pyx_freelist_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl[--__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl];
     memset(o, 0, sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
+  #endif
   p = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)o);
   new((void*)&(p->__pyx_v_intervals)) std::vector<__pyx_t_8rbi_tree_4tree_CIntervalInt> ();
   new((void*)&(p->__pyx_v_it)) std::vector<__pyx_t_8rbi_tree_4tree_CIntervalInt> ::iterator();
   return o;
 }
 
 static void __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl(PyObject *o) {
   struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *p = (struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_intervals);
   __Pyx_call_destructor(p->__pyx_v_it);
   Py_CLEAR(p->__pyx_v_self);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl)))) {
+  if (CYTHON_COMPILING_IN_CPYTHON && ((int)(__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl)))) {
     __pyx_freelist_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl[__pyx_freecount_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl++] = ((struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *p = (struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl *)o;
   if (p->__pyx_v_self) {
     e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
   }
   return 0;
 }
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl},
+  {Py_tp_new, (void *)__pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl_spec = {
+  "rbi_tree.tree.__pyx_scope_struct_1_iter_ivl",
+  sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
+  __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rbi_tree.tree.__pyx_scope_struct_1_iter_ivl", /*tp_name*/
+  "rbi_tree.tree.""__pyx_scope_struct_1_iter_ivl", /*tp_name*/
   sizeof(struct __pyx_obj_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -5664,147 +7522,362 @@
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_tree(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_tree},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "tree",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_ITree, __pyx_k_ITree, sizeof(__pyx_k_ITree), 0, 0, 1, 1},
-  {&__pyx_n_s_ITree_iter_ivl, __pyx_k_ITree_iter_ivl, sizeof(__pyx_k_ITree_iter_ivl), 0, 0, 1, 1},
-  {&__pyx_n_s_ITreed, __pyx_k_ITreed, sizeof(__pyx_k_ITreed), 0, 0, 1, 1},
-  {&__pyx_n_s_ITreed_iter_ivl, __pyx_k_ITreed_iter_ivl, sizeof(__pyx_k_ITreed_iter_ivl), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
-  {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
-  {&__pyx_n_s_from_intervals, __pyx_k_from_intervals, sizeof(__pyx_k_from_intervals), 0, 0, 1, 1},
-  {&__pyx_n_s_insert, __pyx_k_insert, sizeof(__pyx_k_insert), 0, 0, 1, 1},
-  {&__pyx_n_s_insert_2, __pyx_k_insert_2, sizeof(__pyx_k_insert_2), 0, 0, 1, 1},
-  {&__pyx_n_s_intervals, __pyx_k_intervals, sizeof(__pyx_k_intervals), 0, 0, 1, 1},
-  {&__pyx_n_s_iter_ivl, __pyx_k_iter_ivl, sizeof(__pyx_k_iter_ivl), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-  {&__pyx_n_s_rbi_tree_tree, __pyx_k_rbi_tree_tree, sizeof(__pyx_k_rbi_tree_tree), 0, 0, 1, 1},
-  {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
-  {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
-  {&__pyx_n_s_tot, __pyx_k_tot, sizeof(__pyx_k_tot), 0, 0, 1, 1},
-  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_ITree, __pyx_k_ITree, sizeof(__pyx_k_ITree), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree___reduce, __pyx_k_ITree___reduce, sizeof(__pyx_k_ITree___reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree__from_intervals, __pyx_k_ITree__from_intervals, sizeof(__pyx_k_ITree__from_intervals), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree_find, __pyx_k_ITree_find, sizeof(__pyx_k_ITree_find), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree_find_at, __pyx_k_ITree_find_at, sizeof(__pyx_k_ITree_find_at), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree_insert, __pyx_k_ITree_insert, sizeof(__pyx_k_ITree_insert), 0, 0, 1, 1},
+    {&__pyx_n_s_ITree_iter_ivl, __pyx_k_ITree_iter_ivl, sizeof(__pyx_k_ITree_iter_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed, __pyx_k_ITreed, sizeof(__pyx_k_ITreed), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed___reduce, __pyx_k_ITreed___reduce, sizeof(__pyx_k_ITreed___reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed__from_intervals, __pyx_k_ITreed__from_intervals, sizeof(__pyx_k_ITreed__from_intervals), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed__insert, __pyx_k_ITreed__insert, sizeof(__pyx_k_ITreed__insert), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_find, __pyx_k_ITreed_find, sizeof(__pyx_k_ITreed_find), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_find_at, __pyx_k_ITreed_find_at, sizeof(__pyx_k_ITreed_find_at), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_get_ivl, __pyx_k_ITreed_get_ivl, sizeof(__pyx_k_ITreed_get_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_insert, __pyx_k_ITreed_insert, sizeof(__pyx_k_ITreed_insert), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_iter_ivl, __pyx_k_ITreed_iter_ivl, sizeof(__pyx_k_ITreed_iter_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_ITreed_remove, __pyx_k_ITreed_remove, sizeof(__pyx_k_ITreed_remove), 0, 0, 1, 1},
+    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__31, __pyx_k__31, sizeof(__pyx_k__31), 0, 0, 1, 1},
+    {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
+    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+    {&__pyx_n_s_cls, __pyx_k_cls, sizeof(__pyx_k_cls), 0, 0, 1, 1},
+    {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
+    {&__pyx_n_s_find, __pyx_k_find, sizeof(__pyx_k_find), 0, 0, 1, 1},
+    {&__pyx_n_s_find_at, __pyx_k_find_at, sizeof(__pyx_k_find_at), 0, 0, 1, 1},
+    {&__pyx_n_s_from_intervals, __pyx_k_from_intervals, sizeof(__pyx_k_from_intervals), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get_ivl, __pyx_k_get_ivl, sizeof(__pyx_k_get_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
+    {&__pyx_n_s_insert, __pyx_k_insert, sizeof(__pyx_k_insert), 0, 0, 1, 1},
+    {&__pyx_n_s_insert_2, __pyx_k_insert_2, sizeof(__pyx_k_insert_2), 0, 0, 1, 1},
+    {&__pyx_n_s_intervals, __pyx_k_intervals, sizeof(__pyx_k_intervals), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_it, __pyx_k_it, sizeof(__pyx_k_it), 0, 0, 1, 1},
+    {&__pyx_n_s_iter_ivl, __pyx_k_iter_ivl, sizeof(__pyx_k_iter_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_ivl, __pyx_k_ivl, sizeof(__pyx_k_ivl), 0, 0, 1, 1},
+    {&__pyx_n_s_ivl_id, __pyx_k_ivl_id, sizeof(__pyx_k_ivl_id), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_out, __pyx_k_out, sizeof(__pyx_k_out), 0, 0, 1, 1},
+    {&__pyx_n_s_point, __pyx_k_point, sizeof(__pyx_k_point), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+    {&__pyx_n_s_rbi_tree_tree, __pyx_k_rbi_tree_tree, sizeof(__pyx_k_rbi_tree_tree), 0, 0, 1, 1},
+    {&__pyx_kp_s_rbi_tree_tree_pyx, __pyx_k_rbi_tree_tree_pyx, sizeof(__pyx_k_rbi_tree_tree_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_remove, __pyx_k_remove, sizeof(__pyx_k_remove), 0, 0, 1, 1},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
+    {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
+    {&__pyx_n_s_tot, __pyx_k_tot, sizeof(__pyx_k_tot), 0, 0, 1, 1},
+    {&__pyx_n_s_tree, __pyx_k_tree, sizeof(__pyx_k_tree), 0, 0, 1, 1},
+    {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 237, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
+
+  /* "rbi_tree/tree.pyx":77
+ *         del self.tree
+ * 
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         intervals = list(self.iter_ivl())
+ *         return (ITree._from_intervals, (intervals,))
+ */
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_intervals); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_reduce, 77, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 77, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":81
+ *         return (ITree._from_intervals, (intervals,))
+ * 
+ *     def insert(self, start, end, value=None):             # <<<<<<<<<<<<<<
+ *         """Insert an interval [start, end) """
+ * 
+ */
+  __pyx_tuple__5 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_value, __pyx_n_s_ivl, __pyx_n_s_val); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_insert, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+
+  /* "rbi_tree/tree.pyx":93
+ *         return
+ * 
+ *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search intervals overlapping [start, end). Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_tuple__8 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_ivl, __pyx_n_s_out, __pyx_n_s_a, __pyx_n_s_it, __pyx_n_s_val); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_find, 93, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 93, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":110
+ *         return a
+ * 
+ *     def _from_intervals(cls, intervals=None):             # <<<<<<<<<<<<<<
+ *         tree = cls()
+ *         if not intervals is None:
+ */
+  __pyx_tuple__10 = PyTuple_Pack(6, __pyx_n_s_cls, __pyx_n_s_intervals, __pyx_n_s_tree, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_val); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_from_intervals, 110, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 110, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":118
+ *     _from_intervals = classmethod(_from_intervals)
+ * 
+ *     def find_at(self, int point):             # <<<<<<<<<<<<<<
+ *         """Search for intervals containing specified point. Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_tuple__12 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_out, __pyx_n_s_a, __pyx_n_s_it, __pyx_n_s_val); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_find_at, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 118, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":132
+ *         return a
+ * 
+ *     def iter_ivl(self):             # <<<<<<<<<<<<<<
+ *         """Iterate over all intervals. Yields tuples (start, end, id)."""
+ *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
+ */
+  __pyx_tuple__14 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_intervals, __pyx_n_s_it, __pyx_n_s_val); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_iter_ivl, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 132, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":162
+ *         del self.tree
+ * 
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         intervals = list(self.iter_ivl())
+ *         return (ITreed._from_intervals, (intervals, self.tot))
+ */
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_reduce, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 162, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":166
+ *         return (ITreed._from_intervals, (intervals, self.tot))
+ * 
+ *     def _from_intervals(cls, intervals=None, tot=0):             # <<<<<<<<<<<<<<
+ *         tree = cls(tot)
+ *         if not intervals is None:
+ */
+  __pyx_tuple__16 = PyTuple_Pack(7, __pyx_n_s_cls, __pyx_n_s_intervals, __pyx_n_s_tot, __pyx_n_s_tree, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_val); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_from_intervals, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(2, Py_None, __pyx_int_0); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+
+  /* "rbi_tree/tree.pyx":176
+ * 
+ * 
+ *     def _insert(self, start, end, value):             # <<<<<<<<<<<<<<
+ *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
+ *         self.tree.insert(deref(ivl))
+ */
+  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_value, __pyx_n_s_ivl); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_insert_2, 176, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 176, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":182
+ *                             keyval(ivl.value, ivl))
+ * 
+ *     def insert(self, start, end):             # <<<<<<<<<<<<<<
+ *         """Insert an interval [start, end) and returns an id
+ *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+ */
+  __pyx_tuple__21 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_ivl_id); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_insert, 182, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 182, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":197
+ *             return NULL
+ * 
+ *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search intervals overlapping [start, end). Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_tuple__23 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_ivl, __pyx_n_s_out, __pyx_n_s_a, __pyx_n_s_it); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_find, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 197, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":213
+ *         return a
+ * 
+ *     def get_ivl(self, id):             # <<<<<<<<<<<<<<
+ *         """Return a list [start,end] of the interval with specified id."""
+ *         cdef CIntervalInt* ivl = self._get_interval(id)
+ */
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_id, __pyx_n_s_ivl); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_get_ivl, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 213, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":218
+ *         return [deref(ivl).low, deref(ivl).high]
+ * 
+ *     def find_at(self, int point):             # <<<<<<<<<<<<<<
+ *         """Search for intervals containing specified point. Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_point, __pyx_n_s_out, __pyx_n_s_a, __pyx_n_s_it); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_find_at, 218, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 218, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":231
+ *         return a
+ * 
+ *     def remove(self, int id):             # <<<<<<<<<<<<<<
+ *         """Delete interval with specified id."""
+ *         cdef CIntervalInt* ivl = self._get_interval(id)
+ */
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_remove, 231, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 231, __pyx_L1_error)
+
+  /* "rbi_tree/tree.pyx":241
+ *         del ivl
+ * 
+ *     def iter_ivl(self):             # <<<<<<<<<<<<<<
+ *         """Iterate over all intervals. Yields tuples (start, end, id)."""
+ *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
+ */
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_intervals, __pyx_n_s_it); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbi_tree_tree_pyx, __pyx_n_s_iter_ivl, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  return 0;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -5837,51 +7910,98 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_8rbi_tree_4tree_ITree) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8rbi_tree_4tree_ITree.tp_print = 0;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8rbi_tree_4tree_ITree = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8rbi_tree_4tree_ITree_spec, NULL); if (unlikely(!__pyx_ptype_8rbi_tree_4tree_ITree)) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8rbi_tree_4tree_ITree_spec, __pyx_ptype_8rbi_tree_4tree_ITree) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  #else
+  __pyx_ptype_8rbi_tree_4tree_ITree = &__pyx_type_8rbi_tree_4tree_ITree;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8rbi_tree_4tree_ITree) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8rbi_tree_4tree_ITree->tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8rbi_tree_4tree_ITree.tp_dictoffset && __pyx_type_8rbi_tree_4tree_ITree.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8rbi_tree_4tree_ITree.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8rbi_tree_4tree_ITree->tp_dictoffset && __pyx_ptype_8rbi_tree_4tree_ITree->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8rbi_tree_4tree_ITree->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ITree, (PyObject *)&__pyx_type_8rbi_tree_4tree_ITree) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
-  __pyx_ptype_8rbi_tree_4tree_ITree = &__pyx_type_8rbi_tree_4tree_ITree;
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ITree, (PyObject *) __pyx_ptype_8rbi_tree_4tree_ITree) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
   __pyx_vtabptr_8rbi_tree_4tree_ITreed = &__pyx_vtable_8rbi_tree_4tree_ITreed;
   __pyx_vtable_8rbi_tree_4tree_ITreed._get_interval = (__pyx_t_8rbi_tree_4tree_CIntervalInt *(*)(struct __pyx_obj_8rbi_tree_4tree_ITreed *, PyObject *))__pyx_f_8rbi_tree_4tree_6ITreed__get_interval;
-  if (PyType_Ready(&__pyx_type_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8rbi_tree_4tree_ITreed.tp_print = 0;
-  #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8rbi_tree_4tree_ITreed.tp_dictoffset && __pyx_type_8rbi_tree_4tree_ITreed.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8rbi_tree_4tree_ITreed.tp_getattro = __Pyx_PyObject_GenericGetAttr;
-  }
-  if (__Pyx_SetVtable(__pyx_type_8rbi_tree_4tree_ITreed.tp_dict, __pyx_vtabptr_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ITreed, (PyObject *)&__pyx_type_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8rbi_tree_4tree_ITreed = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8rbi_tree_4tree_ITreed_spec, NULL); if (unlikely(!__pyx_ptype_8rbi_tree_4tree_ITreed)) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8rbi_tree_4tree_ITreed_spec, __pyx_ptype_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #else
   __pyx_ptype_8rbi_tree_4tree_ITreed = &__pyx_type_8rbi_tree_4tree_ITreed;
-  if (PyType_Ready(&__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl.tp_dictoffset && __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8rbi_tree_4tree_ITreed->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dictoffset && __pyx_ptype_8rbi_tree_4tree_ITreed->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8rbi_tree_4tree_ITreed->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
+  #endif
+  if (__Pyx_SetVtable(__pyx_ptype_8rbi_tree_4tree_ITreed, __pyx_vtabptr_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_MergeVtables(__pyx_ptype_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ITreed, (PyObject *) __pyx_ptype_8rbi_tree_4tree_ITreed) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl_spec, NULL); if (unlikely(!__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl)) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl_spec, __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  #else
   __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl = &__pyx_type_8rbi_tree_4tree___pyx_scope_struct__iter_ivl;
-  if (PyType_Ready(&__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl.tp_dictoffset && __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl->tp_dictoffset && __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct__iter_ivl->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl_spec, NULL); if (unlikely(!__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl)) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl_spec, __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  #else
   __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl = &__pyx_type_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl->tp_dictoffset && __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8rbi_tree_4tree___pyx_scope_struct_1_iter_ivl->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  }
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5891,22 +8011,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5925,14 +8046,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_tree(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_tree},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "tree",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -5975,42 +8145,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -6018,29 +8202,63 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_tree(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'tree' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("tree", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to tree pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -6051,156 +8269,361 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("tree", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_rbi_tree__tree) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "rbi_tree.tree")) {
-      if (unlikely(PyDict_SetItemString(modules, "rbi_tree.tree", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "rbi_tree.tree", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "rbi_tree/tree.pyx":117
+  /* "rbi_tree/tree.pyx":77
+ *         del self.tree
+ * 
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         intervals = list(self.iter_ivl())
+ *         return (ITree._from_intervals, (intervals,))
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_5__reduce__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree___reduce, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_reduce, __pyx_t_2) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":81
+ *         return (ITree._from_intervals, (intervals,))
+ * 
+ *     def insert(self, start, end, value=None):             # <<<<<<<<<<<<<<
+ *         """Insert an interval [start, end) """
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_7insert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree_insert, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__7);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_insert, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":93
+ *         return
+ * 
+ *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search intervals overlapping [start, end). Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_9find, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree_find, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_find, __pyx_t_2) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":110
+ *         return a
+ * 
+ *     def _from_intervals(cls, intervals=None):             # <<<<<<<<<<<<<<
+ *         tree = cls()
+ *         if not intervals is None:
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_11_from_intervals, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree__from_intervals, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__7);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_from_intervals, __pyx_t_2) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":116
  *                 tree.insert(start, end, val)
  *         return tree
  *     _from_intervals = classmethod(_from_intervals)             # <<<<<<<<<<<<<<
  * 
  *     def find_at(self, int point):
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree, __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Method_ClassMethod(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree, __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_from_intervals, __pyx_t_2) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_from_intervals, __pyx_t_3) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
 
-  /* "rbi_tree/tree.pyx":172
+  /* "rbi_tree/tree.pyx":118
+ *     _from_intervals = classmethod(_from_intervals)
+ * 
+ *     def find_at(self, int point):             # <<<<<<<<<<<<<<
+ *         """Search for intervals containing specified point. Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_13find_at, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree_find_at, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_find_at, __pyx_t_3) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":132
+ *         return a
+ * 
+ *     def iter_ivl(self):             # <<<<<<<<<<<<<<
+ *         """Iterate over all intervals. Yields tuples (start, end, id)."""
+ *         cdef vector[CIntervalObj] intervals = self.tree.intervals()
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_5ITree_15iter_ivl, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITree_iter_ivl, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITree->tp_dict, __pyx_n_s_iter_ivl, __pyx_t_3) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITree);
+
+  /* "rbi_tree/tree.pyx":162
+ *         del self.tree
+ * 
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         intervals = list(self.iter_ivl())
+ *         return (ITreed._from_intervals, (intervals, self.tot))
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_7__reduce__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed___reduce, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_reduce, __pyx_t_3) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":166
+ *         return (ITreed._from_intervals, (intervals, self.tot))
+ * 
+ *     def _from_intervals(cls, intervals=None, tot=0):             # <<<<<<<<<<<<<<
+ *         tree = cls(tot)
+ *         if not intervals is None:
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_9_from_intervals, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed__from_intervals, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__18);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_from_intervals, __pyx_t_3) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":173
  * 
  *         return tree
  *     _from_intervals = classmethod(_from_intervals)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed, __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed, __pyx_n_s_from_intervals); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_Method_ClassMethod(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_from_intervals, __pyx_t_2) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":176
+ * 
+ * 
+ *     def _insert(self, start, end, value):             # <<<<<<<<<<<<<<
+ *         cdef CIntervalInt* ivl = new CIntervalInt(start, end, value)
+ *         self.tree.insert(deref(ivl))
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_11_insert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed__insert, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_insert_2, __pyx_t_2) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":182
+ *                             keyval(ivl.value, ivl))
+ * 
+ *     def insert(self, start, end):             # <<<<<<<<<<<<<<
+ *         """Insert an interval [start, end) and returns an id
+ *         of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_13insert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_insert, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_insert, __pyx_t_2) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":197
+ *             return NULL
+ * 
+ *     def find(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search intervals overlapping [start, end). Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_15find, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_find, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_find, __pyx_t_2) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":213
+ *         return a
+ * 
+ *     def get_ivl(self, id):             # <<<<<<<<<<<<<<
+ *         """Return a list [start,end] of the interval with specified id."""
+ *         cdef CIntervalInt* ivl = self._get_interval(id)
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_17get_ivl, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_get_ivl, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_get_ivl, __pyx_t_2) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":218
+ *         return [deref(ivl).low, deref(ivl).high]
+ * 
+ *     def find_at(self, int point):             # <<<<<<<<<<<<<<
+ *         """Search for intervals containing specified point. Returns list of
+ *         overlapping intervals' ids."""
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_19find_at, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_find_at, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_find_at, __pyx_t_2) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":231
+ *         return a
+ * 
+ *     def remove(self, int id):             # <<<<<<<<<<<<<<
+ *         """Delete interval with specified id."""
+ *         cdef CIntervalInt* ivl = self._get_interval(id)
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_21remove, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_remove, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_remove, __pyx_t_2) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
+
+  /* "rbi_tree/tree.pyx":241
+ *         del ivl
+ * 
+ *     def iter_ivl(self):             # <<<<<<<<<<<<<<
+ *         """Iterate over all intervals. Yields tuples (start, end, id)."""
+ *         cdef vector[CIntervalInt] intervals = self.tree.intervals()
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8rbi_tree_4tree_6ITreed_23iter_ivl, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ITreed_iter_ivl, NULL, __pyx_n_s_rbi_tree_tree, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_iter_ivl, __pyx_t_2) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_8rbi_tree_4tree_ITreed->tp_dict, __pyx_n_s_from_intervals, __pyx_t_1) < 0) __PYX_ERR(0, 172, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_8rbi_tree_4tree_ITreed);
 
   /* "rbi_tree/tree.pyx":1
  * # Copyright 2020-2021 Mikhail Pomaznoy             # <<<<<<<<<<<<<<
  * #
  * # Permission is hereby granted, free of charge, to any person
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init rbi_tree.tree", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init rbi_tree.tree");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -6212,42 +8635,371 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -6268,54 +9020,71 @@
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
-    PyObject *kwdict,
+    PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
-    if (!kw_allowed && PyDict_Next(kwdict, &pos, &key, 0))
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
         goto invalid_keyword;
     return 1;
 #else
-    while (PyDict_Next(kwdict, &pos, &key, 0)) {
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
+            return 1;
+        if (!kw_allowed) {
+            key = PyTuple_GET_ITEM(kw, 0);
+            goto invalid_keyword;
+        }
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
+            key = PyTuple_GET_ITEM(kw, pos);
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+        }
+#endif
+        return 1;
+    }
+    while (PyDict_Next(kw, &pos, &key, 0)) {
         #if PY_MAJOR_VERSION < 3
         if (unlikely(!PyString_Check(key)))
         #endif
             if (unlikely(!PyUnicode_Check(key)))
                 goto invalid_keyword_type;
     }
-    if ((!kw_allowed) && unlikely(key))
+    if (!kw_allowed && unlikely(key))
         goto invalid_keyword;
     return 1;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     return 0;
 #endif
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -6336,15 +9105,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -6352,15 +9120,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -6423,21 +9191,20 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -6465,98 +9232,90 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
     }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
 #else
-    if (likely(PyCFunction_Check(func)))
+        if (PyCFunction_Check(func))
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
     }
-}
 #endif
-
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-#endif
 
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
@@ -6567,25 +9326,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -6611,19 +9382,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -6654,19 +9426,20 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
@@ -6681,183 +9454,260 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject* exc_type = tstate->curexc_type;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
-        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
-            PyObject *exc_value, *exc_tb;
-            exc_value = tstate->curexc_value;
-            exc_tb = tstate->curexc_traceback;
-            tstate->curexc_type = 0;
-            tstate->curexc_value = 0;
-            tstate->curexc_traceback = 0;
-            Py_DECREF(exc_type);
-            Py_XDECREF(exc_value);
-            Py_XDECREF(exc_tb);
-            return 0;
-        } else {
+        if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
-        }
-    }
-    return 0;
-#else
-    if (unlikely(PyErr_Occurred())) {
-        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
-            PyErr_Clear();
-            return 0;
-        } else {
-            return -1;
-        }
+        __Pyx_PyErr_Clear();
+        return 0;
     }
     return 0;
-#endif
 }
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
     }
     #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
     }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
     #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* pep479 */
+static void __Pyx_Generator_Replace_StopIteration(int in_async_gen) {
+    PyObject *exc, *val, *tb, *cur_exc;
+    __Pyx_PyThreadState_declare
+    #ifdef __Pyx_StopAsyncIteration_USED
+    int is_async_stopiteration = 0;
+    #endif
+    CYTHON_MAYBE_UNUSED_VAR(in_async_gen);
+    cur_exc = PyErr_Occurred();
+    if (likely(!__Pyx_PyErr_GivenExceptionMatches(cur_exc, PyExc_StopIteration))) {
+        #ifdef __Pyx_StopAsyncIteration_USED
+        if (in_async_gen && unlikely(__Pyx_PyErr_GivenExceptionMatches(cur_exc, __Pyx_PyExc_StopAsyncIteration))) {
+            is_async_stopiteration = 1;
+        } else
+        #endif
+            return;
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_GetException(&exc, &val, &tb);
+    Py_XDECREF(exc);
+    Py_XDECREF(val);
+    Py_XDECREF(tb);
+    PyErr_SetString(PyExc_RuntimeError,
+        #ifdef __Pyx_StopAsyncIteration_USED
+        is_async_stopiteration ? "async generator raised StopAsyncIteration" :
+        in_async_gen ? "async generator raised StopIteration" :
+        #endif
+        "generator raised StopIteration");
 }
 
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
         long a = PyInt_AS_LONG(op1);
-            x = (long)((unsigned long)a + b);
+        
+            x = (long)((unsigned long)a + (unsigned long)b);
             if (likely((x^a) >= 0 || (x^b) >= 0))
                 return PyInt_FromLong(x);
             return PyLong_Type.tp_as_number->nb_add(op1, op2);
     }
     #endif
     #if CYTHON_USE_PYLONG_INTERNALS
     if (likely(PyLong_CheckExact(op1))) {
         const long b = intval;
         long a, x;
 #ifdef HAVE_LONG_LONG
         const PY_LONG_LONG llb = intval;
         PY_LONG_LONG lla, llx;
 #endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
+        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
+            return __Pyx_NewRef(op2);
+        }
+        if (likely(__Pyx_PyLong_IsCompact(op1))) {
+            a = __Pyx_PyLong_CompactValue(op1);
         } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
             switch (size) {
                 case -2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
             }
         }
                 x = a + b;
             return PyLong_FromLong(x);
@@ -6868,96 +9718,35 @@
 #endif
         
         
     }
     #endif
     if (PyFloat_CheckExact(op1)) {
         const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
         double a = PyFloat_AS_DOUBLE(op1);
+#endif
             double result;
+            
             PyFPE_START_PROTECT("add", return NULL)
             result = ((double)a) + (double)b;
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
-    }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
-    }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
-#endif
-}
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -7082,47 +9871,377 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* FixUpExtensionType */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    for (i = 1; i < n; i++)
+    {
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+    }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -7155,107 +10274,1248 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
-#if PY_VERSION_HEX >= 0x02070000
+static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
+    if (unlikely(!ob))
+        goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
 #else
-    PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
+    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
 #endif
-    if (!ob)
-        goto bad;
-    if (PyDict_SetItem(dict, __pyx_n_s_pyx_vtable, ob) < 0)
         goto bad;
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
+/* GetVTable */
+static void* __Pyx_GetVtable(PyTypeObject *type) {
+    void* ptr;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
+#else
+    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
+#endif
+    if (!ob)
+        goto bad;
+    ptr = PyCapsule_GetPointer(ob, 0);
+    if (!ptr && !PyErr_Occurred())
+        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
+    Py_DECREF(ob);
+    return ptr;
+bad:
+    Py_XDECREF(ob);
+    return NULL;
+}
+
+/* MergeVTables */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type) {
+    int i;
+    void** base_vtables;
+    __Pyx_TypeName tp_base_name;
+    __Pyx_TypeName base_name;
+    void* unknown = (void*)-1;
+    PyObject* bases = type->tp_bases;
+    int base_depth = 0;
+    {
+        PyTypeObject* base = type->tp_base;
+        while (base) {
+            base_depth += 1;
+            base = base->tp_base;
+        }
+    }
+    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
+    base_vtables[0] = unknown;
+    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
+        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
+        if (base_vtable != NULL) {
+            int j;
+            PyTypeObject* base = type->tp_base;
+            for (j = 0; j < base_depth; j++) {
+                if (base_vtables[j] == unknown) {
+                    base_vtables[j] = __Pyx_GetVtable(base);
+                    base_vtables[j + 1] = unknown;
+                }
+                if (base_vtables[j] == base_vtable) {
+                    break;
+                } else if (base_vtables[j] == NULL) {
+                    goto bad;
+                }
+                base = base->tp_base;
+            }
+        }
+    }
+    PyErr_Clear();
+    free(base_vtables);
+    return 0;
+bad:
+    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
+    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
+    PyErr_Format(PyExc_TypeError,
+        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
+    __Pyx_DECREF_TypeName(tp_base_name);
+    __Pyx_DECREF_TypeName(base_name);
+    free(base_vtables);
+    return -1;
+}
+#endif
+
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
+/* FetchSharedCythonModule */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+#if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* ClassMethod */
 static PyObject* __Pyx_Method_ClassMethod(PyObject *method) {
 #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM <= 0x05080000
     if (PyObject_TypeCheck(method, &PyWrapperDescr_Type)) {
         return PyClassMethod_New(method);
     }
 #else
-#if CYTHON_COMPILING_IN_PYSTON || CYTHON_COMPILING_IN_PYPY
+#if CYTHON_COMPILING_IN_PYPY
     if (PyMethodDescr_Check(method))
 #else
     #if PY_MAJOR_VERSION == 2
     static PyTypeObject *methoddescr_type = NULL;
-    if (methoddescr_type == NULL) {
+    if (unlikely(methoddescr_type == NULL)) {
        PyObject *meth = PyObject_GetAttrString((PyObject*)&PyList_Type, "append");
-       if (!meth) return NULL;
+       if (unlikely(!meth)) return NULL;
        methoddescr_type = Py_TYPE(meth);
        Py_DECREF(meth);
     }
     #else
     PyTypeObject *methoddescr_type = &PyMethodDescr_Type;
     #endif
     if (__Pyx_TypeCheck(method, methoddescr_type))
@@ -7274,39 +11534,14 @@
         return PyClassMethod_New(PyMethod_GET_FUNCTION(method));
     }
     else {
         return PyClassMethod_New(method);
     }
 }
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -7342,14 +11577,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -7361,76 +11604,81 @@
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* GetNameInClass */
-static PyObject *__Pyx_GetGlobalNameAfterAttributeLookup(PyObject *name) {
-    PyObject *result;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        return NULL;
-    __Pyx_PyErr_Clear();
-    __Pyx_GetModuleGlobalNameUncached(result, name);
-    return result;
-}
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name) {
     PyObject *result;
-    result = __Pyx_PyObject_GetAttrStr(nmspace, name);
-    if (!result) {
-        result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
+    PyObject *dict;
+    assert(PyType_Check(nmspace));
+#if CYTHON_USE_TYPE_SLOTS
+    dict = ((PyTypeObject*)nmspace)->tp_dict;
+    Py_XINCREF(dict);
+#else
+    dict = PyObject_GetAttr(nmspace, __pyx_n_s_dict);
+#endif
+    if (likely(dict)) {
+        result = PyObject_GetItem(dict, name);
+        Py_DECREF(dict);
+        if (result) {
+            return result;
+        }
     }
+    PyErr_Clear();
+    __Pyx_GetModuleGlobalNameUncached(result, name);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -7501,84 +11749,118 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7586,14 +11868,15 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
@@ -7622,177 +11905,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -7843,14 +12203,29 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__31));
+    }
+    return name;
+}
+#endif
+
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -7894,177 +12269,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -8081,15 +12533,15 @@
     return (long) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -8102,14 +12554,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -8126,19 +12594,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -8177,86 +12645,72 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
-/* FetchCommonType */
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
-    PyObject* fake_module;
-    PyTypeObject* cached_type = NULL;
-    fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
-    if (!fake_module) return NULL;
-    Py_INCREF(fake_module);
-    cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
-    if (cached_type) {
-        if (!PyType_Check((PyObject*)cached_type)) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s is not a type object",
-                type->tp_name);
-            goto bad;
-        }
-        if (cached_type->tp_basicsize != type->tp_basicsize) {
-            PyErr_Format(PyExc_TypeError,
-                "Shared Cython type %.200s has the wrong size, try recompiling",
-                type->tp_name);
-            goto bad;
-        }
-    } else {
-        if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-        PyErr_Clear();
-        if (PyType_Ready(type) < 0) goto bad;
-        if (PyObject_SetAttrString(fake_module, type->tp_name, (PyObject*) type) < 0)
-            goto bad;
-        Py_INCREF(type);
-        cached_type = type;
-    }
-done:
-    Py_DECREF(fake_module);
-    return cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-
 /* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
         exc_info = exc_info->previous_item;
     }
     return exc_info;
 }
 #endif
 
 /* SaveResetException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
     *type = exc_info->exc_type;
     *value = exc_info->exc_value;
     *tb = exc_info->exc_traceback;
-    #else
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
     *type = tstate->exc_type;
     *value = tstate->exc_value;
     *tb = tstate->exc_traceback;
-    #endif
     Py_XINCREF(*type);
     Py_XINCREF(*value);
     Py_XINCREF(*tb);
+  #endif
 }
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = type;
@@ -8269,37 +12723,57 @@
     tstate->exc_type = type;
     tstate->exc_value = value;
     tstate->exc_traceback = tb;
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+  #endif
 }
 #endif
 
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
+        tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
     exc_info->exc_value = *value;
     exc_info->exc_traceback = *tb;
-    #else
+  #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = *type;
     tstate->exc_value = *value;
     tstate->exc_traceback = *tb;
-    #endif
+  #endif
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -8307,108 +12781,18 @@
     PyErr_SetExcInfo(*type, *value, *tb);
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (descr != NULL) {
-        *method = descr;
-        return 0;
-    }
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
-#endif
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectCallMethod1 */
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
@@ -8422,35 +12806,41 @@
         return result;
     }
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
-#include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
-static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
+static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
+    CYTHON_UNUSED_VAR(__pyx_tstate);
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
         Py_XDECREF(ev);
         Py_INCREF(Py_None);
         *pvalue = Py_None;
         return 0;
     }
     if (likely(et == PyExc_StopIteration)) {
         if (!ev) {
             Py_INCREF(Py_None);
             value = Py_None;
         }
 #if PY_VERSION_HEX >= 0x030300A0
-        else if (Py_TYPE(ev) == (PyTypeObject*)PyExc_StopIteration) {
+        else if (likely(__Pyx_IS_TYPE(ev, (PyTypeObject*)PyExc_StopIteration))) {
             value = ((PyStopIterationObject *)ev)->value;
             Py_INCREF(value);
             Py_DECREF(ev);
         }
 #endif
         else if (unlikely(PyTuple_Check(ev))) {
             if (PyTuple_GET_SIZE(ev) >= 1) {
@@ -8506,28 +12896,33 @@
     }
 #endif
     *pvalue = value;
     return 0;
 }
 static CYTHON_INLINE
 void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_CLEAR(exc_state->exc_value);
+#else
     PyObject *t, *v, *tb;
     t = exc_state->exc_type;
     v = exc_state->exc_value;
     tb = exc_state->exc_traceback;
     exc_state->exc_type = NULL;
     exc_state->exc_value = NULL;
     exc_state->exc_traceback = NULL;
     Py_XDECREF(t);
     Py_XDECREF(v);
     Py_XDECREF(tb);
+#endif
 }
 #define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyRunningError(CYTHON_UNUSED __pyx_CoroutineObject *gen) {
+static void __Pyx__Coroutine_AlreadyRunningError(__pyx_CoroutineObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
         msg = "coroutine already executing";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
@@ -8535,16 +12930,17 @@
     #endif
     } else {
         msg = "generator already executing";
     }
     PyErr_SetString(PyExc_ValueError, msg);
 }
 #define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_NotStartedError(CYTHON_UNUSED PyObject *gen) {
+static void __Pyx__Coroutine_NotStartedError(PyObject *gen) {
     const char *msg;
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if ((0)) {
     #ifdef __Pyx_Coroutine_USED
     } else if (__Pyx_Coroutine_Check(gen)) {
         msg = "can't send non-None value to a just-started coroutine";
     #endif
     #ifdef __Pyx_AsyncGen_USED
     } else if (__Pyx_AsyncGen_CheckExact(gen)) {
@@ -8552,15 +12948,17 @@
     #endif
     } else {
         msg = "can't send non-None value to a just-started generator";
     }
     PyErr_SetString(PyExc_TypeError, msg);
 }
 #define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyTerminatedError(CYTHON_UNUSED PyObject *gen, PyObject *value, CYTHON_UNUSED int closing) {
+static void __Pyx__Coroutine_AlreadyTerminatedError(PyObject *gen, PyObject *value, int closing) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
+    CYTHON_MAYBE_UNUSED_VAR(closing);
     #ifdef __Pyx_Coroutine_USED
     if (!closing && __Pyx_Coroutine_Check(gen)) {
         PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
     } else
     #endif
     if (value) {
         #ifdef __Pyx_AsyncGen_USED
@@ -8589,23 +12987,38 @@
 #if CYTHON_FAST_THREAD_STATE
     __Pyx_PyThreadState_assign
     tstate = __pyx_tstate;
 #else
     tstate = __Pyx_PyThreadState_Current;
 #endif
     exc_state = &self->gi_exc_state;
-    if (exc_state->exc_type) {
-        #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+    if (exc_state->exc_value) {
+        #if CYTHON_COMPILING_IN_PYPY
+        #else
+        PyObject *exc_tb;
+        #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
+        exc_tb = PyException_GetTraceback(exc_state->exc_value);
+        #elif PY_VERSION_HEX >= 0x030B00a4
+        exc_tb = ((PyBaseExceptionObject*) exc_state->exc_value)->traceback;
         #else
-        if (exc_state->exc_traceback) {
-            PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
+        exc_tb = exc_state->exc_traceback;
+        #endif
+        if (exc_tb) {
+            PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
+            #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
+            Py_DECREF(exc_tb);
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -8613,37 +13026,48 @@
         __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     } else {
         __Pyx_Coroutine_ExceptionClear(exc_state);
         __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
     }
 #endif
     self->is_running = 1;
-    retval = self->body((PyObject *) self, tstate, value);
+    retval = self->body(self, tstate, value);
     self->is_running = 0;
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state = &self->gi_exc_state;
     tstate->exc_info = exc_state->previous_item;
     exc_state->previous_item = NULL;
     __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
 #endif
     return retval;
 }
 static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
-    PyObject *exc_tb = exc_state->exc_traceback;
-    if (likely(exc_tb)) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+#if CYTHON_COMPILING_IN_PYPY
+    CYTHON_UNUSED_VAR(exc_state);
 #else
+    PyObject *exc_tb;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    if (!exc_state->exc_value) return;
+    exc_tb = PyException_GetTraceback(exc_state->exc_value);
+    #else
+    exc_tb = exc_state->exc_traceback;
+    #endif
+    if (likely(exc_tb)) {
         PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
         PyFrameObject *f = tb->tb_frame;
         Py_CLEAR(f->f_back);
-#endif
+        #if PY_VERSION_HEX >= 0x030B00a4
+        Py_DECREF(exc_tb);
+        #endif
     }
+#endif
 }
 static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_MethodReturn(CYTHON_UNUSED PyObject* gen, PyObject *retval) {
+PyObject *__Pyx_Coroutine_MethodReturn(PyObject* gen, PyObject *retval) {
+    CYTHON_MAYBE_UNUSED_VAR(gen);
     if (unlikely(!retval)) {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         if (!__Pyx_PyErr_Occurred()) {
             PyObject *exc = PyExc_StopIteration;
             #ifdef __Pyx_AsyncGen_USED
             if (__Pyx_AsyncGen_CheckExact(gen))
@@ -8720,15 +13144,15 @@
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyCoro_CheckExact(yf)) {
             ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         {
             if (value == Py_None)
-                ret = Py_TYPE(yf)->tp_iternext(yf);
+                ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
             else
                 ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
         }
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
@@ -8767,24 +13191,23 @@
     if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
         retval = __Pyx_async_gen_athrow_close(yf, NULL);
     } else
     #endif
     {
         PyObject *meth;
         gen->is_running = 1;
-        meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_close);
+        meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_close);
         if (unlikely(!meth)) {
-            if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+            if (unlikely(PyErr_Occurred())) {
                 PyErr_WriteUnraisable(yf);
             }
-            PyErr_Clear();
         } else {
-            retval = PyObject_CallFunction(meth, NULL);
+            retval = __Pyx_PyObject_CallNoArg(meth);
             Py_DECREF(meth);
-            if (!retval)
+            if (unlikely(!retval))
                 err = -1;
         }
         gen->is_running = 0;
     }
     Py_XDECREF(retval);
     return err;
 }
@@ -8807,24 +13230,25 @@
         } else
         #endif
         #ifdef __Pyx_Coroutine_USED
         if (__Pyx_Coroutine_Check(yf)) {
             ret = __Pyx_Coroutine_Send(yf, Py_None);
         } else
         #endif
-            ret = Py_TYPE(yf)->tp_iternext(yf);
+            ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
         gen->is_running = 0;
         if (likely(ret)) {
             return ret;
         }
         return __Pyx_Coroutine_FinishDelegation(gen);
     }
     return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
 }
-static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, PyObject *arg) {
+    CYTHON_UNUSED_VAR(arg);
     return __Pyx_Coroutine_Close(self);
 }
 static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject *retval, *raised_exception;
     PyObject *yf = gen->yieldfrom;
     int err = 0;
@@ -8897,30 +13321,30 @@
             ) {
             ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
         #ifdef __Pyx_Coroutine_USED
         } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
             ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
         #endif
         } else {
-            PyObject *meth = __Pyx_PyObject_GetAttrStr(yf, __pyx_n_s_throw);
+            PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_throw);
             if (unlikely(!meth)) {
                 Py_DECREF(yf);
-                if (!PyErr_ExceptionMatches(PyExc_AttributeError)) {
+                if (unlikely(PyErr_Occurred())) {
                     gen->is_running = 0;
                     return NULL;
                 }
-                PyErr_Clear();
                 __Pyx_Coroutine_Undelegate(gen);
                 gen->is_running = 0;
                 goto throw_here;
             }
             if (likely(args)) {
-                ret = PyObject_CallObject(meth, args);
+                ret = __Pyx_PyObject_Call(meth, args, NULL);
             } else {
-                ret = PyObject_CallFunctionObjArgs(meth, typ, val, tb, NULL);
+                PyObject *cargs[4] = {NULL, typ, val, tb};
+                ret = __Pyx_PyObject_FastCall(meth, cargs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
             }
             Py_DECREF(meth);
         }
         gen->is_running = 0;
         Py_DECREF(yf);
         if (!ret) {
             ret = __Pyx_Coroutine_FinishDelegation(gen);
@@ -8931,22 +13355,26 @@
     __Pyx_Raise(typ, val, tb, NULL);
     return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
 }
 static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
     PyObject *typ;
     PyObject *val = NULL;
     PyObject *tb = NULL;
-    if (!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb))
+    if (unlikely(!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb)))
         return NULL;
     return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
 }
 static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030B00a4
+    Py_VISIT(exc_state->exc_value);
+#else
     Py_VISIT(exc_state->exc_type);
     Py_VISIT(exc_state->exc_value);
     Py_VISIT(exc_state->exc_traceback);
+#endif
     return 0;
 }
 static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
     Py_VISIT(gen->closure);
     Py_VISIT(gen->classobj);
     Py_VISIT(gen->yieldfrom);
     return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
@@ -8959,31 +13387,32 @@
     __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
     }
 #endif
     Py_CLEAR(gen->gi_code);
+    Py_CLEAR(gen->gi_frame);
     Py_CLEAR(gen->gi_name);
     Py_CLEAR(gen->gi_qualname);
     Py_CLEAR(gen->gi_modulename);
     return 0;
 }
 static void __Pyx_Coroutine_dealloc(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     PyObject_GC_UnTrack(gen);
     if (gen->gi_weakreflist != NULL)
         PyObject_ClearWeakRefs(self);
     if (gen->resume_label >= 0) {
         PyObject_GC_Track(self);
 #if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
-        if (PyObject_CallFinalizerFromDealloc(self))
+        if (unlikely(PyObject_CallFinalizerFromDealloc(self)))
 #else
         Py_TYPE(gen)->tp_del(self);
-        if (self->ob_refcnt > 0)
+        if (unlikely(Py_REFCNT(self) > 0))
 #endif
         {
             return;
         }
         PyObject_GC_UnTrack(self);
     }
 #ifdef __Pyx_AsyncGen_USED
@@ -8991,15 +13420,15 @@
         /* We have to handle this case for asynchronous generators
            right here, because this code has to be between UNTRACK
            and GC_Del. */
         Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
     }
 #endif
     __Pyx_Coroutine_clear(self);
-    PyObject_GC_Del(gen);
+    __Pyx_PyHeapTypeObject_GC_Del(gen);
 }
 static void __Pyx_Coroutine_del(PyObject *self) {
     PyObject *error_type, *error_value, *error_traceback;
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     __Pyx_PyThreadState_declare
     if (gen->resume_label < 0) {
         return;
@@ -9069,90 +13498,110 @@
                 PyErr_WriteUnraisable(self);
         } else {
             Py_DECREF(res);
         }
     }
     __Pyx_ErrRestore(error_type, error_value, error_traceback);
 #if !CYTHON_USE_TP_FINALIZE
-    assert(self->ob_refcnt > 0);
-    if (--self->ob_refcnt == 0) {
+    assert(Py_REFCNT(self) > 0);
+    if (likely(--self->ob_refcnt == 0)) {
         return;
     }
     {
-        Py_ssize_t refcnt = self->ob_refcnt;
+        Py_ssize_t refcnt = Py_REFCNT(self);
         _Py_NewReference(self);
         __Pyx_SET_REFCNT(self, refcnt);
     }
 #if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(self->ob_type) &&
+    assert(PyType_IS_GC(Py_TYPE(self)) &&
            _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
     _Py_DEC_REFTOTAL;
 #endif
 #ifdef COUNT_ALLOCS
     --Py_TYPE(self)->tp_frees;
     --Py_TYPE(self)->tp_allocs;
 #endif
 #endif
 }
 static PyObject *
-__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_name;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__name__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_name;
     Py_INCREF(value);
-    self->gi_name = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_name, value);
     return 0;
 }
 static PyObject *
-__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, void *context)
 {
     PyObject *name = self->gi_qualname;
+    CYTHON_UNUSED_VAR(context);
     if (unlikely(!name)) name = Py_None;
     Py_INCREF(name);
     return name;
 }
 static int
-__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, CYTHON_UNUSED void *context)
+__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, void *context)
 {
-    PyObject *tmp;
+    CYTHON_UNUSED_VAR(context);
 #if PY_MAJOR_VERSION >= 3
     if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
     if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
     {
         PyErr_SetString(PyExc_TypeError,
                         "__qualname__ must be set to a string object");
         return -1;
     }
-    tmp = self->gi_qualname;
     Py_INCREF(value);
-    self->gi_qualname = value;
-    Py_XDECREF(tmp);
+    __Pyx_Py_XDECREF_SET(self->gi_qualname, value);
     return 0;
 }
+static PyObject *
+__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, void *context)
+{
+    PyObject *frame = self->gi_frame;
+    CYTHON_UNUSED_VAR(context);
+    if (!frame) {
+        if (unlikely(!self->gi_code)) {
+            Py_RETURN_NONE;
+        }
+        frame = (PyObject *) PyFrame_New(
+            PyThreadState_Get(),            /*PyThreadState *tstate,*/
+            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
+            __pyx_d,                 /*PyObject *globals,*/
+            0                               /*PyObject *locals*/
+        );
+        if (unlikely(!frame))
+            return NULL;
+        self->gi_frame = frame;
+    }
+    Py_INCREF(frame);
+    return frame;
+}
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
             PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
             PyObject *name, PyObject *qualname, PyObject *module_name) {
     __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
     if (unlikely(!gen))
         return NULL;
     return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
@@ -9163,29 +13612,34 @@
     gen->body = body;
     gen->closure = closure;
     Py_XINCREF(closure);
     gen->is_running = 0;
     gen->resume_label = 0;
     gen->classobj = NULL;
     gen->yieldfrom = NULL;
+    #if PY_VERSION_HEX >= 0x030B00a4
+    gen->gi_exc_state.exc_value = NULL;
+    #else
     gen->gi_exc_state.exc_type = NULL;
     gen->gi_exc_state.exc_value = NULL;
     gen->gi_exc_state.exc_traceback = NULL;
+    #endif
 #if CYTHON_USE_EXC_INFO_STACK
     gen->gi_exc_state.previous_item = NULL;
 #endif
     gen->gi_weakreflist = NULL;
     Py_XINCREF(qualname);
     gen->gi_qualname = qualname;
     Py_XINCREF(name);
     gen->gi_name = name;
     Py_XINCREF(module_name);
     gen->gi_modulename = module_name;
     Py_XINCREF(code);
     gen->gi_code = code;
+    gen->gi_frame = NULL;
     PyObject_GC_Track(gen);
     return gen;
 }
 
 /* PatchModuleWithCoroutine */
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
@@ -9249,15 +13703,15 @@
 #endif
 static int __Pyx_patch_abc(void) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
     static int abc_patched = 0;
     if (CYTHON_REGISTER_ABCS && !abc_patched) {
         PyObject *module;
         module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
-        if (!module) {
+        if (unlikely(!module)) {
             PyErr_WriteUnraisable(NULL);
             if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
                     ((PY_MAJOR_VERSION >= 3) ?
                         "Cython module failed to register with collections.abc module" :
                         "Cython module failed to register with collections module"), 1) < 0)) {
                 return -1;
             }
@@ -9294,26 +13748,55 @@
     {0, 0, 0, 0}
 };
 static PyMemberDef __pyx_Generator_memberlist[] = {
     {(char *) "gi_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
     {(char*) "gi_yieldfrom", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
      (char*) PyDoc_STR("object being iterated by 'yield from', or None")},
     {(char*) "gi_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
+    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyGetSetDef __pyx_Generator_getsets[] = {
     {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the generator"), 0},
     {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the generator"), 0},
+    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
+     (char*) PyDoc_STR("Frame of the generator"), 0},
     {0, 0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_GeneratorType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
+    {Py_tp_traverse, (void *)__Pyx_Coroutine_traverse},
+    {Py_tp_iter, (void *)PyObject_SelfIter},
+    {Py_tp_iternext, (void *)__Pyx_Generator_Next},
+    {Py_tp_methods, (void *)__pyx_Generator_methods},
+    {Py_tp_members, (void *)__pyx_Generator_memberlist},
+    {Py_tp_getset, (void *)__pyx_Generator_getsets},
+    {Py_tp_getattro, (void *) __Pyx_PyObject_GenericGetAttrNoDict},
+#if CYTHON_USE_TP_FINALIZE
+    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
+#endif
+    {0, 0},
+};
+static PyType_Spec __pyx_GeneratorType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "generator",
+    sizeof(__pyx_CoroutineObject),
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
+    __pyx_GeneratorType_slots
+};
+#else
 static PyTypeObject __pyx_GeneratorType_type = {
     PyVarObject_HEAD_INIT(0, 0)
-    "generator",
+    __PYX_TYPE_MODULE_PREFIX "generator",
     sizeof(__pyx_CoroutineObject),
     0,
     (destructor) __Pyx_Coroutine_dealloc,
     0,
     0,
     0,
     0,
@@ -9360,75 +13843,119 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
-static int __pyx_Generator_init(void) {
+#endif
+static int __pyx_Generator_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_GeneratorType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_GeneratorType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
+#endif
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
+#if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -9482,15 +14009,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -9511,30 +14038,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -9592,21 +14123,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -9641,16 +14170,41 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `rbi_tree-0.1.5.dev1/rbi_tree/tree.pyx` & `rbi_tree-0.2/rbi_tree/tree.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,15 @@
         del self.tree
 
     def __reduce__(self):
         intervals = list(self.iter_ivl())
         return (ITree._from_intervals, (intervals,))
 
     def insert(self, start, end, value=None):
-        """Insert an interval [start, end) and returns an id
-        of the interval. Ids are incrementing integers, i.e. 0,1,2 etc."""
+        """Insert an interval [start, end) """
         
         cdef CIntervalObj* ivl = new CIntervalObj(
             start, end, <PyObject*>value)
         self.tree.insert(deref(ivl))
         val = <object>value
         if not val is None:
             Py_INCREF(val)
@@ -136,17 +135,19 @@
         cdef vector[CIntervalObj].iterator it = intervals.begin()
         while it != intervals.end():
             val = <object>deref(it).value
             yield (deref(it).low, deref(it).high, val)
             inc(it)
 
 cdef class ITreed():
+    """Version of ITree supporting deletion
+    """
     cdef CTreeInt* tree
     cdef Ivlmap ivldata
-    cdef map[int, CIntervalInt*].iterator datapos
+    cdef map[int, CIntervalInt*].const_iterator datapos
     cdef tot
 
     def __cinit__(self):
         self.tree = new CTreeInt()
         self.ivldata = Ivlmap()
         self.datapos = self.ivldata.begin()
         self.tot = 0
```

### Comparing `rbi_tree-0.1.5.dev1/rbi_tree.egg-info/PKG-INFO` & `rbi_tree-0.2/rbi_tree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rbi-tree
-Version: 0.1.5.dev1
+Version: 0.2
 Summary: Cython-wrapped C++ red-black interval tree implementation
 Home-page: https://github.com/mikpom/rbi_tree
 Author: @mikpom
-Author-email: mikpom@fastmail.com
+Author-email: mikpom@mikpom.ru
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # Interval Tree for Python #
 
 This is a Cython-wrapped red-black interval tree from
 [IvanPinezhaninov/IntervalTree/](https://github.com/IvanPinezhaninov/IntervalTree).
@@ -65,9 +64,7 @@
 []
 >>> t.find_at(70) # search at point
 [(60, 80, 0)]
 >>> list(t.iter_ivl())
 [(60, 80, 0)]
 ```
 
-
-
```

### Comparing `rbi_tree-0.1.5.dev1/setup.cfg` & `rbi_tree-0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build_ext]
 inplace = 1
 
 [metadata]
 name = rbi_tree
-version = 0.1.5-dev1
+version = 0.2
 license = MIT
 author = @mikpom
-author_email = mikpom@fastmail.com
+author_email = mikpom@mikpom.ru
 description = Cython-wrapped C++ red-black interval tree implementation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikpom/rbi_tree
 python_requires = >=3.6
 classifiers = Programming Language :: Python :: 3
```

