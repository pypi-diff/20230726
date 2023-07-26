# Comparing `tmp/multimcts-0.3.1.tar.gz` & `tmp/multimcts-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.3.1.tar", last modified: Tue Jul 25 18:52:12 2023, max compression
+gzip compressed data, was "multimcts-0.4.tar", last modified: Wed Jul 26 20:09:30 2023, max compression
```

## Comparing `multimcts-0.3.1.tar` & `multimcts-0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.032456 multimcts-0.3.1/
--rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.3.1/LICENSE
--rw-r--r--   0 taylorvance   (501) staff       (20)     2805 2023-07-25 18:52:12.032320 multimcts-0.3.1/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     2489 2023-07-25 16:42:00.000000 multimcts-0.3.1/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.031629 multimcts-0.3.1/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.3.1/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   430223 2023-07-25 17:39:23.000000 multimcts-0.3.1/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)     9693 2023-07-24 19:46:18.000000 multimcts-0.3.1/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:52:12.032128 multimcts-0.3.1/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2805 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      231 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-25 18:52:12.000000 multimcts-0.3.1/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.3.1/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-25 18:52:12.032501 multimcts-0.3.1/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      619 2023-07-25 18:51:52.000000 multimcts-0.3.1/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.548791 multimcts-0.4/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.4/LICENSE
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2988 2023-07-26 20:09:30.548644 multimcts-0.4/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2674 2023-07-26 13:34:49.000000 multimcts-0.4/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.547936 multimcts-0.4/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.4/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   543355 2023-07-26 20:06:50.000000 multimcts-0.4/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)   544050 2023-07-26 20:06:46.000000 multimcts-0.4/multimcts/mcts.cpp
+-rw-r--r--   0 taylorvance   (501) staff       (20)    11549 2023-07-26 20:06:41.000000 multimcts-0.4/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.548455 multimcts-0.4/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2988 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      250 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.4/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-26 20:09:30.548837 multimcts-0.4/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      617 2023-07-26 20:09:15.000000 multimcts-0.4/setup.py
```

### Comparing `multimcts-0.3.1/LICENSE` & `multimcts-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multimcts-0.3.1/PKG-INFO` & `multimcts-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: multimcts
-Version: 0.3.1
-Summary: Monte Carlo Tree Search for multiple teams
-Home-page: https://github.com/taylorvance/multimcts
-Author: Taylor Vance
-Author-email: mirrors.cities0w@icloud.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
 
 
 ## Features
 
@@ -40,21 +28,26 @@
 ```bash
 pip install multimcts
 ```
 
 
 ## Usage
 
-To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
+Then you can use MCTS to search for the best move. It will search until some limit is reached.
+```python
+state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
+```
+
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
 
@@ -81,9 +74,7 @@
     python setup.py sdist
     ```
 1. Install the updated package to use in your projects.
     ```bash
     pip install dist/multimcts-0.1.0.tar.gz
     ```
     Replace `multimcts-0.1.0` with the actual filename and version from the `dist/` directory.
-
-
```

### Comparing `multimcts-0.3.1/README.md` & `multimcts-0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: multimcts
+Version: 0.4
+Summary: Monte Carlo Tree Search for multiple teams
+Home-page: https://github.com/taylorvance/multimcts
+Author: Taylor Vance
+Author-email: mirrors.cities0w@icloud.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
 
 
 ## Features
 
@@ -28,21 +40,26 @@
 ```bash
 pip install multimcts
 ```
 
 
 ## Usage
 
-To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
+Then you can use MCTS to search for the best move. It will search until some limit is reached.
+```python
+state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
+```
+
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
 
@@ -69,7 +86,9 @@
     python setup.py sdist
     ```
 1. Install the updated package to use in your projects.
     ```bash
     pip install dist/multimcts-0.1.0.tar.gz
     ```
     Replace `multimcts-0.1.0` with the actual filename and version from the `dist/` directory.
+
+
```

### Comparing `multimcts-0.3.1/multimcts/mcts.c` & `multimcts-0.4/multimcts/mcts.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,21 @@
 /* Generated by Cython 0.29.36 */
 
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "depends": [],
-        "name": "multimcts.mcts",
-        "sources": [
-            "multimcts/mcts.pyx"
-        ]
-    },
-    "module_name": "multimcts.mcts"
-}
-END: Cython Metadata */
-
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
 #define CYTHON_ABI "0_29_36"
 #define CYTHON_HEX_VERSION 0x001D24F0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -757,14 +744,34 @@
   #endif
 #endif
 
 #define __PYX_HAVE__multimcts__mcts
 #define __PYX_HAVE_API__multimcts__mcts
 /* Early includes */
 #include <math.h>
+#include "ios"
+#include "new"
+#include "stdexcept"
+#include "typeinfo"
+#include <utility>
+
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
+    #include <type_traits>
+
+    namespace cython_std {
+    template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
+    template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
+    }
+
+    #endif
+    
+#include <map>
+#include <string.h>
+#include <string>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -967,17 +974,56 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "multimcts/mcts.pyx",
+  "stringsource",
 };
 
 /*--- Type declarations ---*/
+struct __pyx_obj_9multimcts_4mcts_Node;
+struct __pyx_obj_9multimcts_4mcts_MCTS;
+
+/* "multimcts/mcts.pyx":49
+ * 
+ * 
+ * cdef class Node:             # <<<<<<<<<<<<<<
+ *     """Represents a game state node in the MCTS search tree.
+ * 
+ */
+struct __pyx_obj_9multimcts_4mcts_Node {
+  PyObject_HEAD
+  PyObject *_state;
+  PyObject *_move;
+  std::string _team;
+  struct __pyx_obj_9multimcts_4mcts_Node *_parent;
+  PyObject *_children;
+  PyObject *_remaining_moves;
+  std::map<std::string,float>  _total_reward;
+  int _num_visits;
+  double log_visits;
+  int _is_terminal;
+  int _is_fully_expanded;
+};
+
+
+/* "multimcts/mcts.pyx":114
+ * 
+ * 
+ * cdef class MCTS:             # <<<<<<<<<<<<<<
+ *     cdef double exploration_bias
+ * 
+ */
+struct __pyx_obj_9multimcts_4mcts_MCTS {
+  PyObject_HEAD
+  double exploration_bias;
+};
+
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1103,23 +1149,73 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if CYTHON_FAST_PYCALL
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
+#endif
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
+/* PyCFunctionFastCall.proto */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
+#else
+#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
+#endif
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1159,111 +1255,40 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
-#endif
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
-
-/* UnpackUnboundCMethod.proto */
-typedef struct {
-    PyObject *type;
-    PyObject **method_name;
-    PyCFunction func;
-    PyObject *method;
-    int flag;
-} __Pyx_CachedCFunction;
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
-/* CallUnboundCMethod0.proto */
-static PyObject* __Pyx__CallUnboundCMethod0(__Pyx_CachedCFunction* cfunc, PyObject* self);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_CallUnboundCMethod0(cfunc, self)\
-    (likely((cfunc)->func) ?\
-        (likely((cfunc)->flag == METH_NOARGS) ?  (*((cfunc)->func))(self, NULL) :\
-         (PY_VERSION_HEX >= 0x030600B1 && likely((cfunc)->flag == METH_FASTCALL) ?\
-            (PY_VERSION_HEX >= 0x030700A0 ?\
-                (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0) :\
-                (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0, NULL)) :\
-          (PY_VERSION_HEX >= 0x030700A0 && (cfunc)->flag == (METH_FASTCALL | METH_KEYWORDS) ?\
-            (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0, NULL) :\
-            (likely((cfunc)->flag == (METH_VARARGS | METH_KEYWORDS)) ?  ((*(PyCFunctionWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, __pyx_empty_tuple, NULL)) :\
-               ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
-               __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
-        __Pyx__CallUnboundCMethod0(cfunc, self))
-#else
-#define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
-#endif
+/* GetAttr3.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* pyfrozenset_new.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it);
 
 /* PySetContains.proto */
 static CYTHON_INLINE int __Pyx_PySet_ContainsTF(PyObject* key, PyObject* set, int eq);
 
+/* PyUnicode_Unicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj);
+
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -1291,20 +1316,16 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* StrEquals.proto */
-#if PY_MAJOR_VERSION >= 3
-#define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
-#else
-#define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
-#endif
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
@@ -1315,14 +1336,43 @@
 #define __Pyx_PyObject_Pop(L) (likely(PyList_CheckExact(L)) ?\
     __Pyx_PyList_Pop(L) : __Pyx__PyObject_Pop(L))
 #else
 #define __Pyx_PyList_Pop(L)  __Pyx__PyObject_Pop(L)
 #define __Pyx_PyObject_Pop(L)  __Pyx__PyObject_Pop(L)
 #endif
 
+/* UnpackUnboundCMethod.proto */
+typedef struct {
+    PyObject *type;
+    PyObject **method_name;
+    PyCFunction func;
+    PyObject *method;
+    int flag;
+} __Pyx_CachedCFunction;
+
+/* CallUnboundCMethod0.proto */
+static PyObject* __Pyx__CallUnboundCMethod0(__Pyx_CachedCFunction* cfunc, PyObject* self);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CallUnboundCMethod0(cfunc, self)\
+    (likely((cfunc)->func) ?\
+        (likely((cfunc)->flag == METH_NOARGS) ?  (*((cfunc)->func))(self, NULL) :\
+         (PY_VERSION_HEX >= 0x030600B1 && likely((cfunc)->flag == METH_FASTCALL) ?\
+            (PY_VERSION_HEX >= 0x030700A0 ?\
+                (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0) :\
+                (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0, NULL)) :\
+          (PY_VERSION_HEX >= 0x030700A0 && (cfunc)->flag == (METH_FASTCALL | METH_KEYWORDS) ?\
+            (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, &__pyx_empty_tuple, 0, NULL) :\
+            (likely((cfunc)->flag == (METH_VARARGS | METH_KEYWORDS)) ?  ((*(PyCFunctionWithKeywords)(void*)(PyCFunction)(cfunc)->func)(self, __pyx_empty_tuple, NULL)) :\
+               ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
+               __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
+        __Pyx__CallUnboundCMethod0(cfunc, self))
+#else
+#define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
+#endif
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1331,22 +1381,14 @@
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
 /* GetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -1373,36 +1415,61 @@
 
 /* append.proto */
 static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
+/* IterFinish.proto */
+static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
-/* IterFinish.proto */
-static CYTHON_INLINE int __Pyx_IterFinish(void);
+/* RaiseTooManyValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
-/* PyIntCompare.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_NeObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
-#endif
+/* UnpackTupleError.proto */
+static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
+
+/* UnpackTuple2.proto */
+#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
+    (likely(is_tuple || PyTuple_Check(tuple)) ?\
+        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
+            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
+            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
+        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
+static int __Pyx_unpack_tuple2_generic(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
+
+/* dict_iter.proto */
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_is_dict);
+static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
+                                              PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
+
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
@@ -1418,27 +1485,44 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+
+/* PyObject_GenericGetAttrNoDict.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
+#endif
+
+/* PyObject_GenericGetAttr.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* SetupReduce.proto */
+static int __Pyx_setup_reduce(PyObject* type_obj);
+
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1514,14 +1598,18 @@
 
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
+/* GetNameInClass.proto */
+#define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
+static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1540,28 +1628,76 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* None.proto */
+#include <new>
+
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+/* CppExceptionConversion.proto */
+#ifndef __Pyx_CppExn2PyErr
+#include <new>
+#include <typeinfo>
+#include <stdexcept>
+#include <ios>
+static void __Pyx_CppExn2PyErr() {
+  try {
+    if (PyErr_Occurred())
+      ; // let the latest Python exn pass through and ignore the current one
+    else
+      throw;
+  } catch (const std::bad_alloc& exn) {
+    PyErr_SetString(PyExc_MemoryError, exn.what());
+  } catch (const std::bad_cast& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::bad_typeid& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::domain_error& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::invalid_argument& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::ios_base::failure& exn) {
+    PyErr_SetString(PyExc_IOError, exn.what());
+  } catch (const std::out_of_range& exn) {
+    PyErr_SetString(PyExc_IndexError, exn.what());
+  } catch (const std::overflow_error& exn) {
+    PyErr_SetString(PyExc_OverflowError, exn.what());
+  } catch (const std::range_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::underflow_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::exception& exn) {
+    PyErr_SetString(PyExc_RuntimeError, exn.what());
+  }
+  catch (...)
+  {
+    PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
+  }
+}
+#endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
@@ -1574,301 +1710,325 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
-/* Module declarations from 'cython' */
-
 /* Module declarations from 'libc.math' */
 
+/* Module declarations from 'libcpp.utility' */
+
+/* Module declarations from 'libcpp.map' */
+
+/* Module declarations from 'libc.string' */
+
+/* Module declarations from 'libcpp.string' */
+
+/* Module declarations from 'libcpp.pair' */
+
+/* Module declarations from 'cython' */
+
 /* Module declarations from 'multimcts.mcts' */
+static PyTypeObject *__pyx_ptype_9multimcts_4mcts_Node = 0;
+static PyTypeObject *__pyx_ptype_9multimcts_4mcts_MCTS = 0;
+static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(struct __pyx_obj_9multimcts_4mcts_Node *, PyObject *); /*proto*/
+static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *, PyObject *); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
+static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &); /*proto*/
+static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "multimcts.mcts"
 extern int __pyx_module_is_main_multimcts__mcts;
 int __pyx_module_is_main_multimcts__mcts = 0;
 
 /* Implementation of 'multimcts.mcts' */
 static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_IndexError;
-static const char __pyx_k_i[] = "i";
-static const char __pyx_k_k[] = "k";
-static const char __pyx_k_v[] = "v";
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
+static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_pop[] = "pop";
-static const char __pyx_k_str[] = "str";
-static const char __pyx_k_ucb[] = "ucb";
+static const char __pyx_k_val[] = "val";
 static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_List[] = "List";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Move[] = "Move";
 static const char __pyx_k_Node[] = "Node";
+static const char __pyx_k_None[] = "None";
 static const char __pyx_k_Team[] = "Team";
-static const char __pyx_k_best[] = "best";
-static const char __pyx_k_init[] = "__init__";
+static const char __pyx_k_ckey[] = "ckey";
+static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_item[] = "item";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_move[] = "move";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_child[] = "child";
-static const char __pyx_k_float[] = "float";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_state[] = "state";
+static const char __pyx_k_visit[] = "visit";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_choice[] = "choice";
 static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_parent[] = "parent";
+static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_random[] = "random";
+static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_reward[] = "reward";
-static const char __pyx_k_search[] = "search";
 static const char __pyx_k_select[] = "select";
 static const char __pyx_k_typing[] = "typing";
-static const char __pyx_k_values[] = "values";
-static const char __pyx_k_visits[] = "visits";
+static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Rewards[] = "Rewards";
+static const char __pyx_k_creward[] = "creward";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_shuffle[] = "shuffle";
 static const char __pyx_k_children[] = "children";
-static const char __pyx_k_cur_team[] = "cur_team";
-static const char __pyx_k_end_time[] = "end_time";
+static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_max_time[] = "max_time";
+static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_qualname[] = "__qualname__";
+static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_GameState[] = "GameState";
 static const char __pyx_k_heuristic[] = "heuristic";
+static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_make_move[] = "make_move";
 static const char __pyx_k_metaclass[] = "__metaclass__";
-static const char __pyx_k_subreward[] = "subreward";
+static const char __pyx_k_pyx_state[] = "__pyx_state";
+static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
-static const char __pyx_k_best_child[] = "best_child";
-static const char __pyx_k_best_score[] = "best_score";
 static const char __pyx_k_get_reward[] = "get_reward";
-static const char __pyx_k_num_visits[] = "num_visits";
-static const char __pyx_k_MCTS___init[] = "MCTS.__init__";
-static const char __pyx_k_MCTS_expand[] = "MCTS.expand";
-static const char __pyx_k_MCTS_search[] = "MCTS.search";
-static const char __pyx_k_MCTS_select[] = "MCTS.select";
-static const char __pyx_k_Node___init[] = "Node.__init__";
-static const char __pyx_k_collections[] = "collections";
-static const char __pyx_k_defaultdict[] = "defaultdict";
+static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_is_terminal[] = "is_terminal";
 static const char __pyx_k_return_type[] = "return_type";
+static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_staticmethod[] = "staticmethod";
-static const char __pyx_k_total_reward[] = "total_reward";
-static const char __pyx_k_MCTS_simulate[] = "MCTS.simulate";
+static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_backpropagate[] = "backpropagate";
-static const char __pyx_k_terminal_team[] = "terminal_team";
+static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_get_best_child[] = "get_best_child";
 static const char __pyx_k_max_iterations[] = "max_iterations";
 static const char __pyx_k_multimcts_mcts[] = "multimcts.mcts";
 static const char __pyx_k_must_be_one_of[] = ", must be one of ";
 static const char __pyx_k_get_legal_moves[] = "get_legal_moves";
+static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_remaining_moves[] = "remaining_moves";
+static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_exploration_bias[] = "exploration_bias";
 static const char __pyx_k_get_current_team[] = "get_current_team";
-static const char __pyx_k_ln_parent_visits[] = "ln_parent_visits";
-static const char __pyx_k_is_fully_expanded[] = "is_fully_expanded";
-static const char __pyx_k_MCTS_backpropagate[] = "MCTS.backpropagate";
-static const char __pyx_k_VALID_RETURN_TYPES[] = "VALID_RETURN_TYPES";
+static const char __pyx_k_pyx_unpickle_MCTS[] = "__pyx_unpickle_MCTS";
+static const char __pyx_k_pyx_unpickle_Node[] = "__pyx_unpickle_Node";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_multimcts_mcts_pyx[] = "multimcts/mcts.pyx";
 static const char __pyx_k_GameState_make_move[] = "GameState.make_move";
 static const char __pyx_k_Invalid_return_type[] = "Invalid return type: ";
-static const char __pyx_k_MCTS_get_best_child[] = "MCTS.get_best_child";
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_GameState_get_reward[] = "GameState.get_reward";
 static const char __pyx_k_GameState_is_terminal[] = "GameState.is_terminal";
 static const char __pyx_k_GameState_get_legal_moves[] = "GameState.get_legal_moves";
 static const char __pyx_k_GameState_get_current_team[] = "GameState.get_current_team";
-static const char __pyx_k_Represents_a_game_state_node_in[] = "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n\n    Attributes:\n        children (list): The child nodes of the current node. These represent legal moves that have been visited.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ";
 static const char __pyx_k_GameState_must_implement_get_cur[] = "GameState must implement get_current_team.";
 static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
 static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
 static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
 static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
 static const char __pyx_k_Tried_to_expand_a_node_with_no_r[] = "Tried to expand a node with no remaining moves.";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))";
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_GameState;
+static PyObject *__pyx_n_u_GameState;
 static PyObject *__pyx_n_s_GameState_get_current_team;
 static PyObject *__pyx_n_s_GameState_get_legal_moves;
 static PyObject *__pyx_n_s_GameState_get_reward;
 static PyObject *__pyx_n_s_GameState_is_terminal;
 static PyObject *__pyx_n_s_GameState_make_move;
-static PyObject *__pyx_kp_s_GameState_must_implement_get_cur;
-static PyObject *__pyx_kp_s_GameState_must_implement_get_leg;
-static PyObject *__pyx_kp_s_GameState_must_implement_get_rew;
-static PyObject *__pyx_kp_s_GameState_must_implement_is_term;
-static PyObject *__pyx_kp_s_GameState_must_implement_make_mo;
+static PyObject *__pyx_kp_u_GameState_must_implement_get_cur;
+static PyObject *__pyx_kp_u_GameState_must_implement_get_leg;
+static PyObject *__pyx_kp_u_GameState_must_implement_get_rew;
+static PyObject *__pyx_kp_u_GameState_must_implement_is_term;
+static PyObject *__pyx_kp_u_GameState_must_implement_make_mo;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_u_Invalid_return_type;
 static PyObject *__pyx_n_s_List;
 static PyObject *__pyx_n_s_MCTS;
-static PyObject *__pyx_n_s_MCTS___init;
-static PyObject *__pyx_n_s_MCTS_backpropagate;
-static PyObject *__pyx_n_s_MCTS_expand;
-static PyObject *__pyx_n_s_MCTS_get_best_child;
-static PyObject *__pyx_n_s_MCTS_search;
-static PyObject *__pyx_n_s_MCTS_select;
-static PyObject *__pyx_n_s_MCTS_simulate;
 static PyObject *__pyx_n_s_Move;
 static PyObject *__pyx_n_s_Node;
-static PyObject *__pyx_n_s_Node___init;
+static PyObject *__pyx_kp_u_None;
 static PyObject *__pyx_n_s_NotImplementedError;
-static PyObject *__pyx_kp_s_One_or_more_of_max_time_max_iter;
-static PyObject *__pyx_kp_s_Represents_a_game_state_node_in;
+static PyObject *__pyx_kp_u_One_or_more_of_max_time_max_iter;
+static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Rewards;
 static PyObject *__pyx_n_s_Team;
-static PyObject *__pyx_kp_s_Tried_to_expand_a_node_with_no_r;
+static PyObject *__pyx_kp_u_Tried_to_expand_a_node_with_no_r;
 static PyObject *__pyx_n_s_Union;
-static PyObject *__pyx_n_s_VALID_RETURN_TYPES;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_backpropagate;
-static PyObject *__pyx_n_s_best;
-static PyObject *__pyx_n_s_best_child;
-static PyObject *__pyx_n_s_best_score;
 static PyObject *__pyx_n_s_child;
 static PyObject *__pyx_n_s_children;
 static PyObject *__pyx_n_s_choice;
+static PyObject *__pyx_n_s_ckey;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_collections;
-static PyObject *__pyx_n_s_cur_team;
-static PyObject *__pyx_n_s_defaultdict;
+static PyObject *__pyx_n_s_creward;
+static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_end_time;
 static PyObject *__pyx_n_s_expand;
 static PyObject *__pyx_n_s_exploration_bias;
-static PyObject *__pyx_n_u_float;
 static PyObject *__pyx_n_s_get_best_child;
 static PyObject *__pyx_n_s_get_current_team;
 static PyObject *__pyx_n_s_get_legal_moves;
 static PyObject *__pyx_n_s_get_reward;
+static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_heuristic;
-static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_u_int;
-static PyObject *__pyx_n_s_is_fully_expanded;
 static PyObject *__pyx_n_s_is_terminal;
+static PyObject *__pyx_n_s_item;
 static PyObject *__pyx_n_s_items;
-static PyObject *__pyx_n_s_k;
+static PyObject *__pyx_n_s_iteritems;
 static PyObject *__pyx_n_s_key;
-static PyObject *__pyx_n_s_ln_parent_visits;
 static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_make_move;
 static PyObject *__pyx_n_s_max_iterations;
 static PyObject *__pyx_n_s_max_time;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_move;
+static PyObject *__pyx_n_u_move;
 static PyObject *__pyx_n_s_multimcts_mcts;
 static PyObject *__pyx_kp_s_multimcts_mcts_pyx;
 static PyObject *__pyx_kp_u_must_be_one_of;
 static PyObject *__pyx_n_s_name;
+static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_node;
-static PyObject *__pyx_n_s_num_visits;
+static PyObject *__pyx_n_u_node;
 static PyObject *__pyx_n_s_parent;
+static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pop;
 static PyObject *__pyx_n_s_prepare;
+static PyObject *__pyx_n_s_pyx_PickleError;
+static PyObject *__pyx_n_s_pyx_checksum;
+static PyObject *__pyx_n_s_pyx_result;
+static PyObject *__pyx_n_s_pyx_state;
+static PyObject *__pyx_n_s_pyx_type;
+static PyObject *__pyx_n_s_pyx_unpickle_MCTS;
+static PyObject *__pyx_n_s_pyx_unpickle_Node;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_random;
+static PyObject *__pyx_n_s_reduce;
+static PyObject *__pyx_n_s_reduce_cython;
+static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_remaining_moves;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_return_type;
 static PyObject *__pyx_n_s_reward;
-static PyObject *__pyx_n_s_search;
 static PyObject *__pyx_n_s_select;
 static PyObject *__pyx_n_s_self;
+static PyObject *__pyx_n_s_setstate;
+static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_simulate;
 static PyObject *__pyx_n_s_state;
+static PyObject *__pyx_n_u_state;
 static PyObject *__pyx_n_s_staticmethod;
-static PyObject *__pyx_n_u_str;
-static PyObject *__pyx_n_s_subreward;
-static PyObject *__pyx_n_s_terminal_team;
+static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_time;
-static PyObject *__pyx_n_s_total_reward;
 static PyObject *__pyx_n_s_typing;
-static PyObject *__pyx_n_s_ucb;
-static PyObject *__pyx_n_s_v;
-static PyObject *__pyx_n_s_values;
-static PyObject *__pyx_n_s_visits;
+static PyObject *__pyx_n_s_update;
+static PyObject *__pyx_n_s_val;
+static PyObject *__pyx_n_s_visit;
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_parent, PyObject *__pyx_v_move); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_exploration_bias); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4select(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_node, PyObject *__pyx_v_heuristic); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
+static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type); /* proto */
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
-static __Pyx_CachedCFunction __pyx_umethod_PyString_Type_lower = {0, &__pyx_n_s_lower, 0, 0, 0};
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_1;
-static PyObject *__pyx_int_2;
+static PyObject *__pyx_int_24284988;
+static PyObject *__pyx_int_53904430;
+static PyObject *__pyx_int_82662024;
+static PyObject *__pyx_int_203704333;
+static PyObject *__pyx_int_227935910;
+static PyObject *__pyx_int_231097371;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__23;
-static PyObject *__pyx_tuple__25;
-static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__31;
-static PyObject *__pyx_tuple__33;
-static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__13;
 static PyObject *__pyx_codeobj__15;
 static PyObject *__pyx_codeobj__17;
 static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__22;
-static PyObject *__pyx_codeobj__24;
-static PyObject *__pyx_codeobj__26;
-static PyObject *__pyx_codeobj__28;
-static PyObject *__pyx_codeobj__30;
-static PyObject *__pyx_codeobj__32;
-static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__21;
+static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_codeobj__27;
 /* Late includes */
 
-/* "multimcts/mcts.pyx":17
+/* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
 
@@ -1892,28 +2052,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_team", 0);
 
-  /* "multimcts/mcts.pyx":19
+  /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 19, __pyx_L1_error)
+  __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":17
+  /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
 
@@ -1923,15 +2083,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":21
+/* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
@@ -1955,28 +2115,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_legal_moves", 0);
 
-  /* "multimcts/mcts.pyx":23
+  /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 23, __pyx_L1_error)
+  __PYX_ERR(0, 28, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":21
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
@@ -1986,15 +2146,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":25
+/* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
@@ -2030,32 +2190,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, 1); __PYX_ERR(0, 25, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, 1); __PYX_ERR(0, 30, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_move") < 0)) __PYX_ERR(0, 25, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_move") < 0)) __PYX_ERR(0, 30, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_move = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 30, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_4make_move(__pyx_self, __pyx_v_self, __pyx_v_move);
 
@@ -2069,28 +2229,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_move", 0);
 
-  /* "multimcts/mcts.pyx":29
+  /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 29, __pyx_L1_error)
+  __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
@@ -2100,15 +2260,15 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":31
+/* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
@@ -2132,28 +2292,28 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_terminal", 0);
 
-  /* "multimcts/mcts.pyx":33
+  /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
- *     def get_reward(self) -> Union[float, Rewards]:
+ *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 33, __pyx_L1_error)
+  __PYX_ERR(0, 38, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":31
+  /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
@@ -2163,18 +2323,18 @@
   __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":35
+/* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Rewards]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_9GameState_8get_reward[] = "Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}\n        Note: This method is only called on terminal states.\n        ";
@@ -2195,1302 +2355,2070 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_reward", 0);
 
-  /* "multimcts/mcts.pyx":41
+  /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 41, __pyx_L1_error)
+  __PYX_ERR(0, 46, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":35
+  /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Rewards]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":60
- *         remaining_moves (list): A list of moves that have not yet been tried.
- *     """
+/* "multimcts/mcts.pyx":75
+ *     cdef bint _is_fully_expanded
+ * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self.state = state
- *         self.parent = parent
+ *         self._state = state
+ *         self._parent = parent
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4Node_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4Node_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_self = 0;
+static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
-  PyObject *__pyx_v_parent = 0;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent = 0;
   PyObject *__pyx_v_move = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
+  int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_state,&__pyx_n_s_parent,&__pyx_n_s_move,0};
-    PyObject* values[4] = {0,0,0,0};
-    values[2] = ((PyObject *)((PyObject *)Py_None));
-    values[3] = ((PyObject *)((PyObject *)Py_None));
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_state,&__pyx_n_s_parent,&__pyx_n_s_move,0};
+    PyObject* values[3] = {0,0,0};
+    values[1] = (PyObject *)((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None);
+    values[2] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 60, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parent);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[1] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
-        case  3:
+        case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move);
-          if (value) { values[3] = value; kw_args--; }
+          if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 60, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_self = values[0];
-    __pyx_v_state = values[1];
-    __pyx_v_parent = values[2];
-    __pyx_v_move = values[3];
+    __pyx_v_state = values[0];
+    __pyx_v_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[1]);
+    __pyx_v_move = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 60, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
-  return NULL;
+  return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(__pyx_self, __pyx_v_self, __pyx_v_state, __pyx_v_parent, __pyx_v_move);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parent), __pyx_ptype_9multimcts_4mcts_Node, 1, "parent", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), __pyx_v_state, __pyx_v_parent, __pyx_v_move);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = -1;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_parent, PyObject *__pyx_v_move) {
-  PyObject *__pyx_r = NULL;
+static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move) {
+  int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  std::string __pyx_t_4;
+  std::map<std::string,float>  __pyx_t_5;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "multimcts/mcts.pyx":61
- *     """
+  /* "multimcts/mcts.pyx":76
+ * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self.state = state             # <<<<<<<<<<<<<<
- *         self.parent = parent
- *         self.move = move
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+ *         self._state = state             # <<<<<<<<<<<<<<
+ *         self._parent = parent
+ *         self._move = move
+ */
+  __Pyx_INCREF(__pyx_v_state);
+  __Pyx_GIVEREF(__pyx_v_state);
+  __Pyx_GOTREF(__pyx_v_self->_state);
+  __Pyx_DECREF(__pyx_v_self->_state);
+  __pyx_v_self->_state = __pyx_v_state;
 
-  /* "multimcts/mcts.pyx":62
+  /* "multimcts/mcts.pyx":77
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self.state = state
- *         self.parent = parent             # <<<<<<<<<<<<<<
- *         self.move = move
+ *         self._state = state
+ *         self._parent = parent             # <<<<<<<<<<<<<<
+ *         self._move = move
+ *         self._team = str(self._state.get_current_team()).encode()
+ */
+  __Pyx_INCREF(((PyObject *)__pyx_v_parent));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_parent));
+  __Pyx_GOTREF(__pyx_v_self->_parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v_self->_parent));
+  __pyx_v_self->_parent = __pyx_v_parent;
+
+  /* "multimcts/mcts.pyx":78
+ *         self._state = state
+ *         self._parent = parent
+ *         self._move = move             # <<<<<<<<<<<<<<
+ *         self._team = str(self._state.get_current_team()).encode()
+ * 
+ */
+  __Pyx_INCREF(__pyx_v_move);
+  __Pyx_GIVEREF(__pyx_v_move);
+  __Pyx_GOTREF(__pyx_v_self->_move);
+  __Pyx_DECREF(__pyx_v_self->_move);
+  __pyx_v_self->_move = __pyx_v_move;
+
+  /* "multimcts/mcts.pyx":79
+ *         self._parent = parent
+ *         self._move = move
+ *         self._team = str(self._state.get_current_team()).encode()             # <<<<<<<<<<<<<<
  * 
+ *         self._children:List['Node'] = []
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_2), NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_self->_team = __pyx_t_4;
 
-  /* "multimcts/mcts.pyx":63
- *         self.state = state
- *         self.parent = parent
- *         self.move = move             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":81
+ *         self._team = str(self._state.get_current_team()).encode()
  * 
- *         self.children:List['Node'] = []
+ *         self._children:List['Node'] = []             # <<<<<<<<<<<<<<
+ *         self._num_visits = 0
+ *         self.log_visits = -INFINITY
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->_children);
+  __Pyx_DECREF(__pyx_v_self->_children);
+  __pyx_v_self->_children = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":65
- *         self.move = move
+  /* "multimcts/mcts.pyx":82
  * 
- *         self.children:List['Node'] = []             # <<<<<<<<<<<<<<
- *         self.num_visits:int = 0
- *         self.total_reward = defaultdict(float)
+ *         self._children:List['Node'] = []
+ *         self._num_visits = 0             # <<<<<<<<<<<<<<
+ *         self.log_visits = -INFINITY
+ *         self._total_reward = map[string,float]()
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_self->_num_visits = 0;
 
-  /* "multimcts/mcts.pyx":66
+  /* "multimcts/mcts.pyx":83
+ *         self._children:List['Node'] = []
+ *         self._num_visits = 0
+ *         self.log_visits = -INFINITY             # <<<<<<<<<<<<<<
+ *         self._total_reward = map[string,float]()
  * 
- *         self.children:List['Node'] = []
- *         self.num_visits:int = 0             # <<<<<<<<<<<<<<
- *         self.total_reward = defaultdict(float)
+ */
+  __pyx_v_self->log_visits = (-INFINITY);
+
+  /* "multimcts/mcts.pyx":84
+ *         self._num_visits = 0
+ *         self.log_visits = -INFINITY
+ *         self._total_reward = map[string,float]()             # <<<<<<<<<<<<<<
  * 
+ *         self._is_terminal = self._state.is_terminal()
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  try {
+    __pyx_t_5 = std::map<std::string,float> ();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 84, __pyx_L1_error)
+  }
+  __pyx_v_self->_total_reward = __pyx_t_5;
 
-  /* "multimcts/mcts.pyx":67
- *         self.children:List['Node'] = []
- *         self.num_visits:int = 0
- *         self.total_reward = defaultdict(float)             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":86
+ *         self._total_reward = map[string,float]()
  * 
- *         self.is_terminal:bool = self.state.is_terminal()
+ *         self._is_terminal = self._state.is_terminal()             # <<<<<<<<<<<<<<
+ *         if self._is_terminal:
+ *             self._is_fully_expanded = True
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)(&PyFloat_Type)));
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_total_reward, __pyx_t_1) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_self->_is_terminal = __pyx_t_6;
 
-  /* "multimcts/mcts.pyx":69
- *         self.total_reward = defaultdict(float)
- * 
- *         self.is_terminal:bool = self.state.is_terminal()             # <<<<<<<<<<<<<<
- *         self.is_fully_expanded:bool = self.is_terminal
+  /* "multimcts/mcts.pyx":87
  * 
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal, __pyx_t_1) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "multimcts/mcts.pyx":70
- * 
- *         self.is_terminal:bool = self.state.is_terminal()
- *         self.is_fully_expanded:bool = self.is_terminal             # <<<<<<<<<<<<<<
- * 
- *         if self.is_fully_expanded:
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded, __pyx_t_1) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "multimcts/mcts.pyx":72
- *         self.is_fully_expanded:bool = self.is_terminal
- * 
- *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
- *             self.remaining_moves = []
+ *         self._is_terminal = self._state.is_terminal()
+ *         if self._is_terminal:             # <<<<<<<<<<<<<<
+ *             self._is_fully_expanded = True
+ *             self._remaining_moves = []
+ */
+  __pyx_t_6 = (__pyx_v_self->_is_terminal != 0);
+  if (__pyx_t_6) {
+
+    /* "multimcts/mcts.pyx":88
+ *         self._is_terminal = self._state.is_terminal()
+ *         if self._is_terminal:
+ *             self._is_fully_expanded = True             # <<<<<<<<<<<<<<
+ *             self._remaining_moves = []
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__pyx_t_4) {
+    __pyx_v_self->_is_fully_expanded = 1;
 
-    /* "multimcts/mcts.pyx":73
- * 
- *         if self.is_fully_expanded:
- *             self.remaining_moves = []             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":89
+ *         if self._is_terminal:
+ *             self._is_fully_expanded = True
+ *             self._remaining_moves = []             # <<<<<<<<<<<<<<
  *         else:
- *             self.remaining_moves = self.state.get_legal_moves()
+ *             self._is_fully_expanded = False
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
+    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":72
- *         self.is_fully_expanded:bool = self.is_terminal
+    /* "multimcts/mcts.pyx":87
  * 
- *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
- *             self.remaining_moves = []
- *         else:
+ *         self._is_terminal = self._state.is_terminal()
+ *         if self._is_terminal:             # <<<<<<<<<<<<<<
+ *             self._is_fully_expanded = True
+ *             self._remaining_moves = []
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":75
- *             self.remaining_moves = []
+  /* "multimcts/mcts.pyx":91
+ *             self._remaining_moves = []
  *         else:
- *             self.remaining_moves = self.state.get_legal_moves()             # <<<<<<<<<<<<<<
- *             shuffle(self.remaining_moves)
- * 
+ *             self._is_fully_expanded = False             # <<<<<<<<<<<<<<
+ *             self._remaining_moves = self._state.get_legal_moves()
+ *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_v_self->_is_fully_expanded = 0;
+
+    /* "multimcts/mcts.pyx":92
+ *         else:
+ *             self._is_fully_expanded = False
+ *             self._remaining_moves = self._state.get_legal_moves()             # <<<<<<<<<<<<<<
+ *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
+ * 
+ */
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
+    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":76
- *         else:
- *             self.remaining_moves = self.state.get_legal_moves()
- *             shuffle(self.remaining_moves)             # <<<<<<<<<<<<<<
- * 
+    /* "multimcts/mcts.pyx":93
+ *             self._is_fully_expanded = False
+ *             self._remaining_moves = self._state.get_legal_moves()
+ *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?             # <<<<<<<<<<<<<<
  * 
+ *     @property
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = NULL;
+    __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_remaining_moves) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_remaining_moves);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":60
- *         remaining_moves (list): A list of moves that have not yet been tried.
- *     """
+  /* "multimcts/mcts.pyx":75
+ *     cdef bint _is_fully_expanded
+ * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self.state = state
- *         self.parent = parent
+ *         self._state = state
+ *         self._parent = parent
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":96
+ * 
+ *     @property
+ *     def state(self) -> GameState: return self._state             # <<<<<<<<<<<<<<
+ *     @property
+ *     def parent(self) -> 'Node': return self._parent
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_5state___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_state);
+  __pyx_r = __pyx_v_self->_state;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":98
+ *     def state(self) -> GameState: return self._state
+ *     @property
+ *     def parent(self) -> 'Node': return self._parent             # <<<<<<<<<<<<<<
+ *     @property
+ *     def move(self) -> Move: return self._move
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6parent___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
+  __pyx_r = ((PyObject *)__pyx_v_self->_parent);
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":100
+ *     def parent(self) -> 'Node': return self._parent
+ *     @property
+ *     def move(self) -> Move: return self._move             # <<<<<<<<<<<<<<
+ *     @property
+ *     def children(self) -> List['Node']: return self._children
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4move___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_move);
+  __pyx_r = __pyx_v_self->_move;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":102
+ *     def move(self) -> Move: return self._move
+ *     @property
+ *     def children(self) -> List['Node']: return self._children             # <<<<<<<<<<<<<<
+ *     @property
+ *     def remaining_moves(self) -> List[Move]: return self._remaining_moves
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_8children___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_children);
+  __pyx_r = __pyx_v_self->_children;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":104
+ *     def children(self) -> List['Node']: return self._children
+ *     @property
+ *     def remaining_moves(self) -> List[Move]: return self._remaining_moves             # <<<<<<<<<<<<<<
+ * 
+ *     @cython.cdivision(True)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
+  __pyx_r = __pyx_v_self->_remaining_moves;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":109
+ *     @cython.boundscheck(False)
+ *     @cython.wraparound(False)
+ *     def visit(self):             # <<<<<<<<<<<<<<
+ *         self._num_visits += 1
+ *         self.log_visits = log(self._num_visits)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("visit (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_2visit(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("visit", 0);
+
+  /* "multimcts/mcts.pyx":110
+ *     @cython.wraparound(False)
+ *     def visit(self):
+ *         self._num_visits += 1             # <<<<<<<<<<<<<<
+ *         self.log_visits = log(self._num_visits)
+ * 
+ */
+  __pyx_v_self->_num_visits = (__pyx_v_self->_num_visits + 1);
+
+  /* "multimcts/mcts.pyx":111
+ *     def visit(self):
+ *         self._num_visits += 1
+ *         self.log_visits = log(self._num_visits)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_v_self->log_visits = log(__pyx_v_self->_num_visits);
+
+  /* "multimcts/mcts.pyx":109
+ *     @cython.boundscheck(False)
+ *     @cython.wraparound(False)
+ *     def visit(self):             # <<<<<<<<<<<<<<
+ *         self._num_visits += 1
+ *         self.log_visits = log(self._num_visits)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ */
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_self->_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __pyx_convert_map_to_py_std_3a__3a_string____float(__pyx_v_self->_total_reward); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_self->log_visits); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = PyTuple_New(11); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_INCREF(__pyx_v_self->_children);
+  __Pyx_GIVEREF(__pyx_v_self->_children);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_self->_children);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2);
+  __Pyx_INCREF(__pyx_v_self->_move);
+  __Pyx_GIVEREF(__pyx_v_self->_move);
+  PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_v_self->_move);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_t_3);
+  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->_parent));
+  PyTuple_SET_ITEM(__pyx_t_7, 5, ((PyObject *)__pyx_v_self->_parent));
+  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
+  __Pyx_GIVEREF(__pyx_v_self->_remaining_moves);
+  PyTuple_SET_ITEM(__pyx_t_7, 6, __pyx_v_self->_remaining_moves);
+  __Pyx_INCREF(__pyx_v_self->_state);
+  __Pyx_GIVEREF(__pyx_v_self->_state);
+  PyTuple_SET_ITEM(__pyx_t_7, 7, __pyx_v_self->_state);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_7, 8, __pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_7, 9, __pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_7, 10, __pyx_t_6);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_4 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_6 = 0;
+  __pyx_v_state = ((PyObject*)__pyx_t_7);
+  __pyx_t_7 = 0;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_7 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_v__dict = __pyx_t_7;
+  __pyx_t_7 = 0;
+
+  /* "(tree fragment)":7
+ *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_8 = (__pyx_v__dict != Py_None);
+  __pyx_t_9 = (__pyx_t_8 != 0);
+  if (__pyx_t_9) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v__dict);
+    __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_6));
+    __pyx_t_6 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ */
+  /*else*/ {
+    __pyx_t_8 = (__pyx_v_self->_children != Py_None);
+    __pyx_t_10 = (__pyx_t_8 != 0);
+    if (!__pyx_t_10) {
+    } else {
+      __pyx_t_9 = __pyx_t_10;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_10 = (__pyx_v_self->_move != Py_None);
+    __pyx_t_8 = (__pyx_t_10 != 0);
+    if (!__pyx_t_8) {
+    } else {
+      __pyx_t_9 = __pyx_t_8;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_8 = (((PyObject *)__pyx_v_self->_parent) != Py_None);
+    __pyx_t_10 = (__pyx_t_8 != 0);
+    if (!__pyx_t_10) {
+    } else {
+      __pyx_t_9 = __pyx_t_10;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_10 = (__pyx_v_self->_remaining_moves != Py_None);
+    __pyx_t_8 = (__pyx_t_10 != 0);
+    if (!__pyx_t_8) {
+    } else {
+      __pyx_t_9 = __pyx_t_8;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_8 = (__pyx_v_self->_state != Py_None);
+    __pyx_t_10 = (__pyx_t_8 != 0);
+    __pyx_t_9 = __pyx_t_10;
+    __pyx_L4_bool_binop_done:;
+    __pyx_v_use_setstate = __pyx_t_9;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *     else:
+ */
+  __pyx_t_9 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_9) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *     if use_setstate:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_24284988);
+    __Pyx_GIVEREF(__pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_7, 2, Py_None);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    __pyx_t_6 = 0;
+    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *     else:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_Node__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_24284988);
+    __Pyx_GIVEREF(__pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_state);
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
+    __pyx_t_5 = 0;
+    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("multimcts.mcts.Node.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":80
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Node__set_state(self, __pyx_state)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_Node__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ */
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Node__set_state(self, __pyx_state)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.Node.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":117
+ *     cdef double exploration_bias
  * 
- * class MCTS:
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n\n        Args:\n            exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.\n                It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).\n                Default is 1.414, which is sqrt(2) and often used in practice.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS___init__};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_self = 0;
+static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n\n        Args:\n            exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.\n                It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).\n                The default \342\210\2322 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.\n        ";
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
+struct wrapperbase __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
+#endif
+static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_exploration_bias;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
+  int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_exploration_bias,0};
-    PyObject* values[2] = {0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_exploration_bias,0};
+    PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias);
-          if (value) { values[1] = value; kw_args--; }
+          if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 80, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
+        CYTHON_FALLTHROUGH;
+        case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_self = values[0];
-    if (values[1]) {
-      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L3_error)
+    if (values[0]) {
+      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
     } else {
-      __pyx_v_exploration_bias = ((double)((double)1.414));
+      __pyx_v_exploration_bias = ((double)1.414);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 80, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
-  return NULL;
+  return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(__pyx_self, __pyx_v_self, __pyx_v_exploration_bias);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_exploration_bias);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__init__", 0);
+
+  /* "multimcts/mcts.pyx":125
+ *                 The default 2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
+ *         """
+ *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  __pyx_v_self->exploration_bias = __pyx_v_exploration_bias;
+
+  /* "multimcts/mcts.pyx":117
+ *     cdef double exploration_bias
+ * 
+ *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
+ *         """Initializes an MCTS agent.
+ * 
+ */
 
   /* function exit code */
+  __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_exploration_bias) {
+/* "multimcts/mcts.pyx":128
+ * 
+ *     @property
+ *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
+ *         return self.exploration_bias
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "multimcts/mcts.pyx":88
- *                 Default is 1.414, which is sqrt(2) and often used in practice.
- *         """
- *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":129
+ *     @property
+ *     def exploration_bias(self) -> float:
+ *         return self.exploration_bias             # <<<<<<<<<<<<<<
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
  */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias, __pyx_t_1) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":80
+  /* "multimcts/mcts.pyx":128
  * 
- * class MCTS:
- *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
- *         """Initializes an MCTS agent.
+ *     @property
+ *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
+ *         return self.exploration_bias
  * 
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.exploration_bias.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":90
- *         self.exploration_bias = exploration_bias
+/* "multimcts/mcts.pyx":131
+ *         return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_2search[] = "Searches for this state's best move until some limit has been reached.\n\n        Args:\n            state (GameState): The game state for which to find the best move.\n            max_time (int|float): The maximum time to search, in seconds.\n            max_iterations (int): The maximum number of selections/simulations to perform.\n            heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.\n            return_type (str): One of \"state\", \"move\", or \"node\".\n        Returns:\n            GameState: A new game state which is the result of applying the best move to the given state.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_3search = {"search", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_3search, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_2search};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_self = 0;
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v_max_time = 0;
   PyObject *__pyx_v_max_iterations = 0;
   PyObject *__pyx_v_heuristic = 0;
   PyObject *__pyx_v_return_type = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("search (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_state,&__pyx_n_s_max_time,&__pyx_n_s_max_iterations,&__pyx_n_s_heuristic,&__pyx_n_s_return_type,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
-    values[2] = ((PyObject *)((PyObject *)Py_None));
-    values[3] = ((PyObject *)((PyObject *)Py_None));
-    values[4] = ((PyObject *)((PyObject *)Py_None));
-    values[5] = ((PyObject*)((PyObject*)__pyx_n_s_state));
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_state,&__pyx_n_s_max_time,&__pyx_n_s_max_iterations,&__pyx_n_s_heuristic,&__pyx_n_s_return_type,0};
+    PyObject* values[5] = {0,0,0,0,0};
+    values[1] = ((PyObject *)Py_None);
+    values[2] = ((PyObject *)Py_None);
+    values[3] = ((PyObject *)Py_None);
+    values[4] = ((PyObject*)__pyx_n_u_state);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, 1); __PYX_ERR(0, 90, __pyx_L3_error)
-        }
       }
       if (kw_args > 0 && likely(kw_args <= 4)) {
         Py_ssize_t index;
-        for (index = 2; index < 6 && kw_args > 0; index++) {
+        for (index = 1; index < 5 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 131, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_state = values[1];
-    __pyx_v_max_time = values[2];
-    __pyx_v_max_iterations = values[3];
-    __pyx_v_heuristic = values[4];
-    __pyx_v_return_type = ((PyObject*)values[5]);
+    __pyx_v_state = values[0];
+    __pyx_v_max_time = values[1];
+    __pyx_v_max_iterations = values[2];
+    __pyx_v_heuristic = values[3];
+    __pyx_v_return_type = ((PyObject*)values[4]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 131, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyString_Type), 1, "return_type", 1))) __PYX_ERR(0, 90, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(__pyx_self, __pyx_v_self, __pyx_v_state, __pyx_v_max_time, __pyx_v_max_iterations, __pyx_v_heuristic, __pyx_v_return_type);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyUnicode_Type), 1, "return_type", 1))) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_state, __pyx_v_max_time, __pyx_v_max_iterations, __pyx_v_heuristic, __pyx_v_return_type);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type) {
   PyObject *__pyx_v_VALID_RETURN_TYPES = NULL;
-  PyObject *__pyx_v_node = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = NULL;
+  double __pyx_v_exploration_bias;
   double __pyx_v_end_time;
   int __pyx_v_i;
   PyObject *__pyx_v_child = NULL;
   PyObject *__pyx_v_reward = NULL;
   PyObject *__pyx_v_best = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  Py_UCS4 __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  Py_ssize_t __pyx_t_6;
+  Py_UCS4 __pyx_t_7;
+  int __pyx_t_8;
   double __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
   __Pyx_INCREF(__pyx_v_return_type);
 
-  /* "multimcts/mcts.pyx":102
+  /* "multimcts/mcts.pyx":143
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         return_type = return_type.lower()             # <<<<<<<<<<<<<<
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  */
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyString_Type_lower, __pyx_v_return_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_return_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_return_type, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":103
+  /* "multimcts/mcts.pyx":144
  *         """
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}             # <<<<<<<<<<<<<<
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_n_s_state) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_s_move) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_s_node) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_state) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_move) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_node) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __pyx_v_VALID_RETURN_TYPES = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":104
+  /* "multimcts/mcts.pyx":145
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
-  __pyx_t_2 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (unlikely(__pyx_t_3)) {
+  __pyx_t_4 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":105
+    /* "multimcts/mcts.pyx":146
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')             # <<<<<<<<<<<<<<
  * 
  *         if max_time is None and max_iterations is None:
  */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = 0;
-    __pyx_t_5 = 127;
+    __pyx_t_6 = 0;
+    __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_return_type);
-    __pyx_t_4 += 21;
+    __pyx_t_6 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_return_type);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_return_type);
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_return_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
-    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_return_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
+    __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+    __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_must_be_one_of);
-    __pyx_t_4 += 17;
+    __pyx_t_6 += 17;
     __Pyx_GIVEREF(__pyx_kp_u_must_be_one_of);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_must_be_one_of);
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
-    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
+    __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
+    __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 105, __pyx_L1_error)
+    __PYX_ERR(0, 146, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":104
+    /* "multimcts/mcts.pyx":145
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":107
+  /* "multimcts/mcts.pyx":148
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
-  __pyx_t_2 = (__pyx_v_max_time == Py_None);
-  __pyx_t_7 = (__pyx_t_2 != 0);
-  if (__pyx_t_7) {
+  __pyx_t_4 = (__pyx_v_max_time == Py_None);
+  __pyx_t_8 = (__pyx_t_4 != 0);
+  if (__pyx_t_8) {
   } else {
-    __pyx_t_3 = __pyx_t_7;
+    __pyx_t_5 = __pyx_t_8;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_7 = (__pyx_v_max_iterations == Py_None);
-  __pyx_t_2 = (__pyx_t_7 != 0);
-  __pyx_t_3 = __pyx_t_2;
+  __pyx_t_8 = (__pyx_v_max_iterations == Py_None);
+  __pyx_t_4 = (__pyx_t_8 != 0);
+  __pyx_t_5 = __pyx_t_4;
   __pyx_L5_bool_binop_done:;
-  if (unlikely(__pyx_t_3)) {
+  if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":108
+    /* "multimcts/mcts.pyx":149
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 108, __pyx_L1_error)
+    __PYX_ERR(0, 149, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":107
+    /* "multimcts/mcts.pyx":148
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":110
+  /* "multimcts/mcts.pyx":151
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
- *         cdef double end_time
+ *         cdef double exploration_bias = self.exploration_bias
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_8, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_state);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_v_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_v_node = __pyx_t_1;
+  __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":114
+  /* "multimcts/mcts.pyx":153
+ *         node = Node(state)
+ * 
+ *         cdef double exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
+ * 
+ *         cdef double end_time
+ */
+  __pyx_t_9 = __pyx_v_self->exploration_bias;
+  __pyx_v_exploration_bias = __pyx_t_9;
+
+  /* "multimcts/mcts.pyx":157
  *         cdef double end_time
  *         cdef int i
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  */
-  __pyx_t_3 = (__pyx_v_max_time != Py_None);
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_5 = (__pyx_v_max_time != Py_None);
+  __pyx_t_4 = (__pyx_t_5 != 0);
+  if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":115
+    /* "multimcts/mcts.pyx":158
  *         cdef int i
  *         if max_time is not None:
  *             end_time = time() + max_time             # <<<<<<<<<<<<<<
  *         if max_iterations is not None:
  *             i = max_iterations
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 115, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_8);
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 115, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_end_time = __pyx_t_9;
 
-    /* "multimcts/mcts.pyx":114
+    /* "multimcts/mcts.pyx":157
  *         cdef double end_time
  *         cdef int i
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  */
   }
 
-  /* "multimcts/mcts.pyx":116
+  /* "multimcts/mcts.pyx":159
  *         if max_time is not None:
  *             end_time = time() + max_time
  *         if max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = max_iterations
  * 
  */
-  __pyx_t_2 = (__pyx_v_max_iterations != Py_None);
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_4 = (__pyx_v_max_iterations != Py_None);
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":117
+    /* "multimcts/mcts.pyx":160
  *             end_time = time() + max_time
  *         if max_iterations is not None:
  *             i = max_iterations             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
     __pyx_v_i = __pyx_t_10;
 
-    /* "multimcts/mcts.pyx":116
+    /* "multimcts/mcts.pyx":159
  *         if max_time is not None:
  *             end_time = time() + max_time
  *         if max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = max_iterations
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":119
+  /* "multimcts/mcts.pyx":162
  *             i = max_iterations
  * 
  *         while True:             # <<<<<<<<<<<<<<
- *             child = self.select(node)
+ *             child = self.select(node, exploration_bias)
  *             reward = self.simulate(child, heuristic=heuristic)
  */
   while (1) {
 
-    /* "multimcts/mcts.pyx":120
+    /* "multimcts/mcts.pyx":163
  * 
  *         while True:
- *             child = self.select(node)             # <<<<<<<<<<<<<<
+ *             child = self.select(node, exploration_bias)             # <<<<<<<<<<<<<<
  *             reward = self.simulate(child, heuristic=heuristic)
  *             self.backpropagate(child, reward)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_select); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = NULL;
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_11 = NULL;
+    __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_8)) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
+        __pyx_t_10 = 1;
       }
     }
-    __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_node);
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 120, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_1)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_12 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_12);
+      if (__pyx_t_11) {
+        __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
+      }
+      __Pyx_INCREF(((PyObject *)__pyx_v_node));
+      __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
+      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_10, __pyx_t_3);
+      __pyx_t_3 = 0;
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_2);
+    __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":121
+    /* "multimcts/mcts.pyx":164
  *         while True:
- *             child = self.select(node)
+ *             child = self.select(node, exploration_bias)
  *             reward = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
  *             self.backpropagate(child, reward)
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simulate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_child);
     __Pyx_GIVEREF(__pyx_v_child);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_child);
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 121, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_11);
-    __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_3);
+    __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":122
- *             child = self.select(node)
+    /* "multimcts/mcts.pyx":165
+ *             child = self.select(node, exploration_bias)
  *             reward = self.simulate(child, heuristic=heuristic)
  *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
  * 
  *             if max_time is not None and time() >= end_time:
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 122, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
     __pyx_t_1 = NULL;
     __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_12, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_8)) {
+    if (PyFunction_Check(__pyx_t_12)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_11 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_11 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 122, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_2 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       if (__pyx_t_1) {
-        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1); __pyx_t_1 = NULL;
+        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1); __pyx_t_1 = NULL;
       }
       __Pyx_INCREF(__pyx_v_child);
       __Pyx_GIVEREF(__pyx_v_child);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_10, __pyx_v_child);
+      PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_10, __pyx_v_child);
       __Pyx_INCREF(__pyx_v_reward);
       __Pyx_GIVEREF(__pyx_v_reward);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_10, __pyx_v_reward);
-      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_6, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 122, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_10, __pyx_v_reward);
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":124
+    /* "multimcts/mcts.pyx":167
  *             self.backpropagate(child, reward)
  * 
  *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if max_iterations is not None:
  */
-    __pyx_t_2 = (__pyx_v_max_time != Py_None);
-    __pyx_t_7 = (__pyx_t_2 != 0);
-    if (__pyx_t_7) {
+    __pyx_t_4 = (__pyx_v_max_time != Py_None);
+    __pyx_t_8 = (__pyx_t_4 != 0);
+    if (__pyx_t_8) {
     } else {
-      __pyx_t_3 = __pyx_t_7;
+      __pyx_t_5 = __pyx_t_8;
       goto __pyx_L12_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_2 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_12);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __Pyx_DECREF_SET(__pyx_t_12, function);
       }
     }
-    __pyx_t_11 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_11, __pyx_t_8, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_3 = __pyx_t_7;
+    __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_12, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_5 = __pyx_t_8;
     __pyx_L12_bool_binop_done:;
-    if (__pyx_t_3) {
+    if (__pyx_t_5) {
 
-      /* "multimcts/mcts.pyx":125
+      /* "multimcts/mcts.pyx":168
  * 
  *             if max_time is not None and time() >= end_time:
  *                 break             # <<<<<<<<<<<<<<
  *             if max_iterations is not None:
  *                 i -= 1
  */
       goto __pyx_L10_break;
 
-      /* "multimcts/mcts.pyx":124
+      /* "multimcts/mcts.pyx":167
  *             self.backpropagate(child, reward)
  * 
  *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if max_iterations is not None:
  */
     }
 
-    /* "multimcts/mcts.pyx":126
+    /* "multimcts/mcts.pyx":169
  *             if max_time is not None and time() >= end_time:
  *                 break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 if i <= 0:
  */
-    __pyx_t_3 = (__pyx_v_max_iterations != Py_None);
-    __pyx_t_7 = (__pyx_t_3 != 0);
-    if (__pyx_t_7) {
+    __pyx_t_5 = (__pyx_v_max_iterations != Py_None);
+    __pyx_t_8 = (__pyx_t_5 != 0);
+    if (__pyx_t_8) {
 
-      /* "multimcts/mcts.pyx":127
+      /* "multimcts/mcts.pyx":170
  *                 break
  *             if max_iterations is not None:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 if i <= 0:
  *                     break
  */
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "multimcts/mcts.pyx":128
+      /* "multimcts/mcts.pyx":171
  *             if max_iterations is not None:
  *                 i -= 1
  *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
-      __pyx_t_7 = ((__pyx_v_i <= 0) != 0);
-      if (__pyx_t_7) {
+      __pyx_t_8 = ((__pyx_v_i <= 0) != 0);
+      if (__pyx_t_8) {
 
-        /* "multimcts/mcts.pyx":129
+        /* "multimcts/mcts.pyx":172
  *                 i -= 1
  *                 if i <= 0:
  *                     break             # <<<<<<<<<<<<<<
  * 
- *         best = self.get_best_child(node)
+ *         best = self.get_best_child(node, exploration_bias)
  */
         goto __pyx_L10_break;
 
-        /* "multimcts/mcts.pyx":128
+        /* "multimcts/mcts.pyx":171
  *             if max_iterations is not None:
  *                 i -= 1
  *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":126
+      /* "multimcts/mcts.pyx":169
  *             if max_time is not None and time() >= end_time:
  *                 break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 if i <= 0:
  */
     }
   }
   __pyx_L10_break:;
 
-  /* "multimcts/mcts.pyx":131
+  /* "multimcts/mcts.pyx":174
  *                     break
  * 
- *         best = self.get_best_child(node)             # <<<<<<<<<<<<<<
+ *         best = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
  * 
  *         if return_type == "state":
  */
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_11 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_11)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_11);
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = NULL;
+  __pyx_t_10 = 0;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_12, function);
+      __pyx_t_10 = 1;
     }
   }
-  __pyx_t_6 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_11, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_node);
-  __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_v_best = __pyx_t_6;
-  __pyx_t_6 = 0;
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_12)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  } else
+  #endif
+  {
+    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    if (__pyx_t_1) {
+      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_1); __pyx_t_1 = NULL;
+    }
+    __Pyx_INCREF(((PyObject *)__pyx_v_node));
+    __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
+    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_t_3);
+    __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  __pyx_v_best = __pyx_t_2;
+  __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":133
- *         best = self.get_best_child(node)
+  /* "multimcts/mcts.pyx":176
+ *         best = self.get_best_child(node, exploration_bias)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
-  __pyx_t_7 = (__Pyx_PyString_Equals(__pyx_v_return_type, __pyx_n_s_state, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __pyx_t_3 = (__pyx_t_7 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_state, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_8 != 0);
+  if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":134
+    /* "multimcts/mcts.pyx":177
  * 
  *         if return_type == "state":
  *             return best.state             # <<<<<<<<<<<<<<
  *         elif return_type == "move":
  *             return best.move
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_state); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 134, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":133
- *         best = self.get_best_child(node)
+    /* "multimcts/mcts.pyx":176
+ *         best = self.get_best_child(node, exploration_bias)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
   }
 
-  /* "multimcts/mcts.pyx":135
+  /* "multimcts/mcts.pyx":178
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
-  __pyx_t_3 = (__Pyx_PyString_Equals(__pyx_v_return_type, __pyx_n_s_move, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
-  __pyx_t_7 = (__pyx_t_3 != 0);
-  if (__pyx_t_7) {
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_move, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_8 = (__pyx_t_5 != 0);
+  if (__pyx_t_8) {
 
-    /* "multimcts/mcts.pyx":136
+    /* "multimcts/mcts.pyx":179
  *             return best.state
  *         elif return_type == "move":
  *             return best.move             # <<<<<<<<<<<<<<
  *         elif return_type == "node":
  *             return best
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_move); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_move); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":135
+    /* "multimcts/mcts.pyx":178
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
   }
 
-  /* "multimcts/mcts.pyx":137
+  /* "multimcts/mcts.pyx":180
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
-  __pyx_t_7 = (__Pyx_PyString_Equals(__pyx_v_return_type, __pyx_n_s_node, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __pyx_t_3 = (__pyx_t_7 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_node, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_8 != 0);
+  if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":138
+    /* "multimcts/mcts.pyx":181
  *             return best.move
  *         elif return_type == "node":
  *             return best             # <<<<<<<<<<<<<<
  * 
- *     def select(self, node:Node) -> Node:
+ *     def select(self, node:Node, exploration_bias:float) -> Node:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_best);
     __pyx_r = __pyx_v_best;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":137
+    /* "multimcts/mcts.pyx":180
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":90
- *         self.exploration_bias = exploration_bias
+  /* "multimcts/mcts.pyx":131
+ *         return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_VALID_RETURN_TYPES);
-  __Pyx_XDECREF(__pyx_v_node);
+  __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XDECREF(__pyx_v_best);
   __Pyx_XDECREF(__pyx_v_return_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":140
+/* "multimcts/mcts.pyx":183
  *             return best
  * 
- *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_4select[] = "Step 1: Selection\n        Traverse the tree for the node we most want to simulate.\n        Looks for an unexplored child of this node's best child's best child's...best child.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_5select = {"select", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_5select, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_4select};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_node = 0;
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
+  double __pyx_v_exploration_bias;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("select (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_node,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -3498,241 +4426,322 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 140, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 183, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 140, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_node = values[1];
+    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
+    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 140, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(__pyx_self, __pyx_v_self, __pyx_v_node);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4select(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node) {
-  PyObject *__pyx_r = NULL;
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
-  __Pyx_INCREF(__pyx_v_node);
+  __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":145
+  /* "multimcts/mcts.pyx":188
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
- *         while not node.is_terminal:             # <<<<<<<<<<<<<<
- *             if not node.is_fully_expanded:
+ *         while not node._is_terminal:             # <<<<<<<<<<<<<<
+ *             if not node._is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = ((!__pyx_t_2) != 0);
-    if (!__pyx_t_3) break;
+    __pyx_t_1 = ((!(__pyx_v_node->_is_terminal != 0)) != 0);
+    if (!__pyx_t_1) break;
 
-    /* "multimcts/mcts.pyx":146
+    /* "multimcts/mcts.pyx":189
  *         """
- *         while not node.is_terminal:
- *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node._is_terminal:
+ *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_2 = ((!__pyx_t_3) != 0);
-    if (__pyx_t_2) {
+    __pyx_t_1 = ((!(__pyx_v_node->_is_fully_expanded != 0)) != 0);
+    if (__pyx_t_1) {
 
-      /* "multimcts/mcts.pyx":147
- *         while not node.is_terminal:
- *             if not node.is_fully_expanded:
+      /* "multimcts/mcts.pyx":190
+ *         while not node._is_terminal:
+ *             if not node._is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
- *                 node = self.get_best_child(node)
+ *                 node = self.get_best_child(node, exploration_bias)
  */
-      __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_5);
+      __Pyx_XDECREF(((PyObject *)__pyx_r));
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_expand); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_r = __pyx_t_1;
-      __pyx_t_1 = 0;
+      __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_node)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_node));
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 190, __pyx_L1_error)
+      __pyx_r = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2);
+      __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":146
+      /* "multimcts/mcts.pyx":189
  *         """
- *         while not node.is_terminal:
- *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node._is_terminal:
+ *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":149
+    /* "multimcts/mcts.pyx":192
  *                 return self.expand(node)
  *             else:
- *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
+ *                 node = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
  * 
  *         return node
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_4 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      __pyx_t_6 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_6 = 1;
         }
       }
-      __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_1);
-      __pyx_t_1 = 0;
+      #if CYTHON_FAST_PYCALL
+      if (PyFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
+        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      } else
+      #endif
+      #if CYTHON_FAST_PYCCALL
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
+        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      } else
+      #endif
+      {
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 192, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        if (__pyx_t_5) {
+          __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
+        }
+        __Pyx_INCREF(((PyObject *)__pyx_v_node));
+        __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
+        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, ((PyObject *)__pyx_v_node));
+        __Pyx_GIVEREF(__pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
+        __pyx_t_4 = 0;
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 192, __pyx_L1_error)
+      __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
+      __pyx_t_2 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":151
- *                 node = self.get_best_child(node)
+  /* "multimcts/mcts.pyx":194
+ *                 node = self.get_best_child(node, exploration_bias)
  * 
  *         return node             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_node);
+  __Pyx_XDECREF(((PyObject *)__pyx_r));
+  __Pyx_INCREF(((PyObject *)__pyx_v_node));
   __pyx_r = __pyx_v_node;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":140
+  /* "multimcts/mcts.pyx":183
  *             return best
  * 
- *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_node);
-  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_XDECREF((PyObject *)__pyx_v_node);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":154
+/* "multimcts/mcts.pyx":197
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(PyObject *__pyx_self, PyObject *__pyx_v_node); /*proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_6expand[] = "Step 2: Expansion\n        Add a new child to this node.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_7expand = {"expand", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_O, __pyx_doc_9multimcts_4mcts_4MCTS_6expand};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(PyObject *__pyx_self, PyObject *__pyx_v_node) {
-  PyObject *__pyx_r = 0;
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_7expand = {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand};
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("expand (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6expand(__pyx_self, ((PyObject *)__pyx_v_node));
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,0};
+    PyObject* values[1] = {0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expand") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+    }
+    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("expand", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6expand(__pyx_v_node);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   PyObject *__pyx_v_move = NULL;
-  PyObject *__pyx_v_child = NULL;
-  PyObject *__pyx_r = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  int __pyx_t_12;
+  int __pyx_t_9;
+  Py_ssize_t __pyx_t_10;
+  int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
 
-  /* "multimcts/mcts.pyx":158
+  /* "multimcts/mcts.pyx":201
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
   {
@@ -3740,30 +4749,30 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "multimcts/mcts.pyx":159
+      /* "multimcts/mcts.pyx":202
  *         """
  *         try:
  *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 202, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_move = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":158
+      /* "multimcts/mcts.pyx":201
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
     }
@@ -3771,266 +4780,255 @@
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "multimcts/mcts.pyx":160
+    /* "multimcts/mcts.pyx":203
  *         try:
  *             move = node.remaining_moves.pop()
  *         except IndexError:             # <<<<<<<<<<<<<<
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
     if (__pyx_t_6) {
       __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 160, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 203, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "multimcts/mcts.pyx":161
+      /* "multimcts/mcts.pyx":204
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
  * 
  *         child = Node(state=node.state.make_move(move), parent=node, move=move)
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 161, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 204, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 161, __pyx_L5_except_error)
+      __PYX_ERR(0, 204, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "multimcts/mcts.pyx":158
+    /* "multimcts/mcts.pyx":201
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "multimcts/mcts.pyx":163
+  /* "multimcts/mcts.pyx":206
  *             raise IndexError("Tried to expand a node with no remaining moves.")
  * 
  *         child = Node(state=node.state.make_move(move), parent=node, move=move)             # <<<<<<<<<<<<<<
  *         node.children.append(child)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_make_move); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-      __Pyx_INCREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_9, function);
+      __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_move);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_state, __pyx_t_5) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_parent, __pyx_v_node) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_move);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_v_child = __pyx_t_5;
-  __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_parent, ((PyObject *)__pyx_v_node)) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_v_child = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_4);
+  __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":164
+  /* "multimcts/mcts.pyx":207
  * 
  *         child = Node(state=node.state.make_move(move), parent=node, move=move)
  *         node.children.append(child)             # <<<<<<<<<<<<<<
  * 
  *         if len(node.remaining_moves) == 0:
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_5, __pyx_v_child); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_9 = __Pyx_PyObject_Append(__pyx_t_4, ((PyObject *)__pyx_v_child)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 207, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":166
+  /* "multimcts/mcts.pyx":209
  *         node.children.append(child)
  * 
  *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node.is_fully_expanded = True
+ *             node._is_fully_expanded = True
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 166, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_12 = ((__pyx_t_11 == 0) != 0);
-  if (__pyx_t_12) {
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_10 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 209, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_11 = ((__pyx_t_10 == 0) != 0);
+  if (__pyx_t_11) {
 
-    /* "multimcts/mcts.pyx":167
+    /* "multimcts/mcts.pyx":210
  * 
  *         if len(node.remaining_moves) == 0:
- *             node.is_fully_expanded = True             # <<<<<<<<<<<<<<
+ *             node._is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
  *         return child
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_v_node->_is_fully_expanded = 1;
 
-    /* "multimcts/mcts.pyx":166
+    /* "multimcts/mcts.pyx":209
  *         node.children.append(child)
  * 
  *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node.is_fully_expanded = True
+ *             node._is_fully_expanded = True
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":169
- *             node.is_fully_expanded = True
+  /* "multimcts/mcts.pyx":212
+ *             node._is_fully_expanded = True
  * 
  *         return child             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_child);
+  __Pyx_XDECREF(((PyObject *)__pyx_r));
+  __Pyx_INCREF(((PyObject *)__pyx_v_child));
   __pyx_r = __pyx_v_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":154
+  /* "multimcts/mcts.pyx":197
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_move);
-  __Pyx_XDECREF(__pyx_v_child);
-  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_XDECREF((PyObject *)__pyx_v_child);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":171
+/* "multimcts/mcts.pyx":214
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_8simulate[] = "Step 3: Simulation (aka playout/rollout)\n        Play out a game, from the given node to termination, and return the final reward.\n        A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.\n\n        Args:\n            node (Node): The node from which to begin the simulation.\n            heuristic (callable): A function that takes a state and returns a move.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_9simulate = {"simulate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_9simulate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_8simulate};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_node = 0;
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
   PyObject *__pyx_v_heuristic = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("simulate (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_node,&__pyx_n_s_heuristic,0};
-    PyObject* values[3] = {0,0,0};
-    values[2] = ((PyObject *)((PyObject *)Py_None));
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_heuristic,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 171, __pyx_L3_error)
-        }
       }
       if (kw_args == 1) {
-        const Py_ssize_t index = 2;
+        const Py_ssize_t index = 1;
         PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 171, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_node = values[1];
-    __pyx_v_heuristic = values[2];
+    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
+    __pyx_v_heuristic = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 171, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulate", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 214, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(__pyx_self, __pyx_v_self, __pyx_v_node, __pyx_v_heuristic);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_heuristic);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_node, PyObject *__pyx_v_heuristic) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic) {
   PyObject *__pyx_v_state = NULL;
   PyObject *__pyx_v_terminal_team = NULL;
   PyObject *__pyx_v_move = NULL;
   PyObject *__pyx_v_reward = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -4041,152 +5039,149 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
 
-  /* "multimcts/mcts.pyx":180
+  /* "multimcts/mcts.pyx":223
  *             heuristic (callable): A function that takes a state and returns a move.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
- *         if node.is_terminal:
+ *         if node._is_terminal:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":182
+  /* "multimcts/mcts.pyx":225
  *         state = node.state
  * 
- *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *         if node._is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 182, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = (__pyx_v_node->_is_terminal != 0);
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":183
+    /* "multimcts/mcts.pyx":226
  * 
- *         if node.is_terminal:
+ *         if node._is_terminal:
  *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_terminal_team = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":182
+    /* "multimcts/mcts.pyx":225
  *         state = node.state
  * 
- *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *         if node._is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":185
+  /* "multimcts/mcts.pyx":228
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":186
+      /* "multimcts/mcts.pyx":229
  *         else:
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 if heuristic is not None:
  *                     move = heuristic(state)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":187
+      /* "multimcts/mcts.pyx":230
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
       __pyx_t_5 = (__pyx_v_heuristic != Py_None);
       __pyx_t_2 = (__pyx_t_5 != 0);
       if (__pyx_t_2) {
 
-        /* "multimcts/mcts.pyx":188
+        /* "multimcts/mcts.pyx":231
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  *                     move = heuristic(state)             # <<<<<<<<<<<<<<
  *                 else:
  *                     move = choice(state.get_legal_moves())
  */
         __Pyx_INCREF(__pyx_v_heuristic);
@@ -4198,55 +5193,55 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_state);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "multimcts/mcts.pyx":187
+        /* "multimcts/mcts.pyx":230
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
         goto __pyx_L6;
       }
 
-      /* "multimcts/mcts.pyx":190
+      /* "multimcts/mcts.pyx":233
  *                     move = heuristic(state)
  *                 else:
  *                     move = choice(state.get_legal_moves())             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
           }
         }
         __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4254,126 +5249,126 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
       }
       __pyx_L6:;
 
-      /* "multimcts/mcts.pyx":191
+      /* "multimcts/mcts.pyx":234
  *                 else:
  *                     move = choice(state.get_legal_moves())
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":193
+  /* "multimcts/mcts.pyx":236
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":194
+  /* "multimcts/mcts.pyx":237
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":195
+    /* "multimcts/mcts.pyx":238
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
  *         return reward
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 195, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
+    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 238, __pyx_L1_error) }
+    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":194
+    /* "multimcts/mcts.pyx":237
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":197
+  /* "multimcts/mcts.pyx":240
  *             reward = {terminal_team: reward}
  * 
  *         return reward             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_reward);
   __pyx_r = __pyx_v_reward;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":171
+  /* "multimcts/mcts.pyx":214
  *         return child
  * 
  *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
@@ -4392,28 +5387,28 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":200
+/* "multimcts/mcts.pyx":243
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate[] = "Step 4: Backpropagation\n        Update all ancestors with the reward from this terminal node.\n        ";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate = {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_node = 0;
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
   PyObject *__pyx_v_reward = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("backpropagate (wrapper)", 0);
@@ -4436,383 +5431,347 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 200, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 243, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 200, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 243, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_node = values[0];
+    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
     __pyx_v_reward = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 200, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 243, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_self, __pyx_v_node, __pyx_v_reward);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_v_node, __pyx_v_reward);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node, PyObject *__pyx_v_reward) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward) {
+  double __pyx_v_val;
+  std::string __pyx_v_ckey;
+  std::map<std::string,float>  __pyx_v_creward;
   PyObject *__pyx_v_key = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_k = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_v = NULL;
+  std::pair<std::string,float>  __pyx_v_item;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  std::map<std::string,float>  __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *(*__pyx_t_9)(PyObject *);
+  int __pyx_t_8;
+  double __pyx_t_9;
   int __pyx_t_10;
-  int __pyx_t_11;
+  std::string __pyx_t_11;
+  int __pyx_t_12;
+  std::map<std::string,float> ::iterator __pyx_t_13;
+  std::pair<std::string,float>  __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
-  __Pyx_INCREF(__pyx_v_node);
-  __Pyx_INCREF(__pyx_v_reward);
+  __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":205
- *         """
- *         # Remove 0-values for efficiency.
- *         reward = {k:v for k,v in reward.items() if v!=0}             # <<<<<<<<<<<<<<
- *         while node is not None:
- *             node.num_visits += 1
+  /* "multimcts/mcts.pyx":249
+ *         cdef double val
+ *         cdef string ckey
+ *         cdef map[string,float] creward = map[string,float]()             # <<<<<<<<<<<<<<
+ *         for key,val in reward.items():
+ *             if val == 0:
+ */
+  try {
+    __pyx_t_1 = std::map<std::string,float> ();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 249, __pyx_L1_error)
+  }
+  __pyx_v_creward = __pyx_t_1;
+
+  /* "multimcts/mcts.pyx":250
+ *         cdef string ckey
+ *         cdef map[string,float] creward = map[string,float]()
+ *         for key,val in reward.items():             # <<<<<<<<<<<<<<
+ *             if val == 0:
+ *                 continue
+ */
+  __pyx_t_3 = 0;
+  if (unlikely(__pyx_v_reward == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+    __PYX_ERR(0, 250, __pyx_L1_error)
+  }
+  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_reward, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_2);
+  __pyx_t_2 = __pyx_t_6;
+  __pyx_t_6 = 0;
+  while (1) {
+    __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
+    if (unlikely(__pyx_t_8 == 0)) break;
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __pyx_v_val = __pyx_t_9;
+
+    /* "multimcts/mcts.pyx":251
+ *         cdef map[string,float] creward = map[string,float]()
+ *         for key,val in reward.items():
+ *             if val == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             ckey = str(key).encode()
+ */
+    __pyx_t_10 = ((__pyx_v_val == 0.0) != 0);
+    if (__pyx_t_10) {
+
+      /* "multimcts/mcts.pyx":252
+ *         for key,val in reward.items():
+ *             if val == 0:
+ *                 continue             # <<<<<<<<<<<<<<
+ *             ckey = str(key).encode()
+ *             creward[ckey] = val
+ */
+      goto __pyx_L3_continue;
+
+      /* "multimcts/mcts.pyx":251
+ *         cdef map[string,float] creward = map[string,float]()
+ *         for key,val in reward.items():
+ *             if val == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             ckey = str(key).encode()
  */
-  { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_reward, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-      __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_5 = 0;
-      __pyx_t_6 = NULL;
-    } else {
-      __pyx_t_5 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 205, __pyx_L5_error)
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_6)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 205, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 205, __pyx_L5_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L5_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_6(__pyx_t_3);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 205, __pyx_L5_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_2);
-      }
-      if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-        PyObject* sequence = __pyx_t_2;
-        Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-        if (unlikely(size != 2)) {
-          if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-          else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 205, __pyx_L5_error)
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
-        }
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_7);
-        #else
-        __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        #endif
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      } else {
-        Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 205, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
-        index = 0; __pyx_t_4 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_4)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_4);
-        index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 205, __pyx_L5_error)
-        __pyx_t_9 = NULL;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        goto __pyx_L9_unpacking_done;
-        __pyx_L8_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_9 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 205, __pyx_L5_error)
-        __pyx_L9_unpacking_done:;
-      }
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_4);
-      __pyx_t_4 = 0;
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 205, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (__pyx_t_10) {
-        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 205, __pyx_L5_error)
-      }
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
-    goto __pyx_L11_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
-    goto __pyx_L1_error;
-    __pyx_L11_exit_scope:;
-  } /* exit inner scope */
-  __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_1);
-  __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":206
- *         # Remove 0-values for efficiency.
- *         reward = {k:v for k,v in reward.items() if v!=0}
+    /* "multimcts/mcts.pyx":253
+ *             if val == 0:
+ *                 continue
+ *             ckey = str(key).encode()             # <<<<<<<<<<<<<<
+ *             creward[ckey] = val
+ * 
+ */
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_6 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_7), NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_11 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_v_ckey = __pyx_t_11;
+
+    /* "multimcts/mcts.pyx":254
+ *                 continue
+ *             ckey = str(key).encode()
+ *             creward[ckey] = val             # <<<<<<<<<<<<<<
+ * 
+ *         cdef pair[string,float] item
+ */
+    (__pyx_v_creward[__pyx_v_ckey]) = __pyx_v_val;
+    __pyx_L3_continue:;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "multimcts/mcts.pyx":257
+ * 
+ *         cdef pair[string,float] item
  *         while node is not None:             # <<<<<<<<<<<<<<
- *             node.num_visits += 1
- *             for key in reward:
+ *             for item in creward:
+ *                 ckey = item.first
  */
   while (1) {
-    __pyx_t_10 = (__pyx_v_node != Py_None);
-    __pyx_t_11 = (__pyx_t_10 != 0);
-    if (!__pyx_t_11) break;
+    __pyx_t_10 = (((PyObject *)__pyx_v_node) != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) break;
 
-    /* "multimcts/mcts.pyx":207
- *         reward = {k:v for k,v in reward.items() if v!=0}
+    /* "multimcts/mcts.pyx":258
+ *         cdef pair[string,float] item
  *         while node is not None:
- *             node.num_visits += 1             # <<<<<<<<<<<<<<
- *             for key in reward:
- *                 node.total_reward[key] += reward[key]
+ *             for item in creward:             # <<<<<<<<<<<<<<
+ *                 ckey = item.first
+ *                 if node._total_reward.count(ckey) == 0:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_13 = __pyx_v_creward.begin();
+    for (;;) {
+      if (!(__pyx_t_13 != __pyx_v_creward.end())) break;
+      __pyx_t_14 = *__pyx_t_13;
+      ++__pyx_t_13;
+      __pyx_v_item = __pyx_t_14;
 
-    /* "multimcts/mcts.pyx":208
+      /* "multimcts/mcts.pyx":259
  *         while node is not None:
- *             node.num_visits += 1
- *             for key in reward:             # <<<<<<<<<<<<<<
- *                 node.total_reward[key] += reward[key]
- *             node = node.parent
+ *             for item in creward:
+ *                 ckey = item.first             # <<<<<<<<<<<<<<
+ *                 if node._total_reward.count(ckey) == 0:
+ *                     node._total_reward[ckey] = 0
+ */
+      __pyx_t_11 = __pyx_v_item.first;
+      __pyx_v_ckey = __pyx_t_11;
+
+      /* "multimcts/mcts.pyx":260
+ *             for item in creward:
+ *                 ckey = item.first
+ *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
+ *                     node._total_reward[ckey] = 0
+ *                 node._total_reward[ckey] += item.second
+ */
+      __pyx_t_12 = ((__pyx_v_node->_total_reward.count(__pyx_v_ckey) == 0) != 0);
+      if (__pyx_t_12) {
+
+        /* "multimcts/mcts.pyx":261
+ *                 ckey = item.first
+ *                 if node._total_reward.count(ckey) == 0:
+ *                     node._total_reward[ckey] = 0             # <<<<<<<<<<<<<<
+ *                 node._total_reward[ckey] += item.second
+ *             node.visit()
+ */
+        (__pyx_v_node->_total_reward[__pyx_v_ckey]) = 0.0;
+
+        /* "multimcts/mcts.pyx":260
+ *             for item in creward:
+ *                 ckey = item.first
+ *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
+ *                     node._total_reward[ckey] = 0
+ *                 node._total_reward[ckey] += item.second
  */
-    if (likely(PyList_CheckExact(__pyx_v_reward)) || PyTuple_CheckExact(__pyx_v_reward)) {
-      __pyx_t_3 = __pyx_v_reward; __Pyx_INCREF(__pyx_t_3); __pyx_t_5 = 0;
-      __pyx_t_6 = NULL;
-    } else {
-      __pyx_t_5 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 208, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 208, __pyx_L1_error)
-    }
-    for (;;) {
-      if (likely(!__pyx_t_6)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 208, __pyx_L1_error)
-          #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          #endif
-        } else {
-          if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 208, __pyx_L1_error)
-          #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          #endif
-        }
-      } else {
-        __pyx_t_1 = __pyx_t_6(__pyx_t_3);
-        if (unlikely(!__pyx_t_1)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 208, __pyx_L1_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_1);
       }
-      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
-      __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":209
- *             node.num_visits += 1
- *             for key in reward:
- *                 node.total_reward[key] += reward[key]             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":262
+ *                 if node._total_reward.count(ckey) == 0:
+ *                     node._total_reward[ckey] = 0
+ *                 node._total_reward[ckey] += item.second             # <<<<<<<<<<<<<<
+ *             node.visit()
  *             node = node.parent
- * 
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_INCREF(__pyx_v_key);
-      __pyx_t_2 = __pyx_v_key;
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 209, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 209, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_11 = __pyx_v_ckey;
+      (__pyx_v_node->_total_reward[__pyx_t_11]) = ((__pyx_v_node->_total_reward[__pyx_t_11]) + __pyx_v_item.second);
 
-      /* "multimcts/mcts.pyx":208
+      /* "multimcts/mcts.pyx":258
+ *         cdef pair[string,float] item
  *         while node is not None:
- *             node.num_visits += 1
- *             for key in reward:             # <<<<<<<<<<<<<<
- *                 node.total_reward[key] += reward[key]
+ *             for item in creward:             # <<<<<<<<<<<<<<
+ *                 ckey = item.first
+ *                 if node._total_reward.count(ckey) == 0:
+ */
+    }
+
+    /* "multimcts/mcts.pyx":263
+ *                     node._total_reward[ckey] = 0
+ *                 node._total_reward[ckey] += item.second
+ *             node.visit()             # <<<<<<<<<<<<<<
  *             node = node.parent
+ * 
  */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_visit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":210
- *             for key in reward:
- *                 node.total_reward[key] += reward[key]
+    /* "multimcts/mcts.pyx":264
+ *                 node._total_reward[ckey] += item.second
+ *             node.visit()
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
  *     @cython.cdivision(True)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
+    __pyx_t_2 = 0;
   }
 
-  /* "multimcts/mcts.pyx":200
+  /* "multimcts/mcts.pyx":243
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v);
-  __Pyx_XDECREF(__pyx_v_node);
-  __Pyx_XDECREF(__pyx_v_reward);
+  __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":213
- * 
- *     @cython.cdivision(True)
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
+/* "multimcts/mcts.pyx":269
+ *     @cython.boundscheck(False)
+ *     @cython.wraparound(False)
+ *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
  *         """Find the child with the highest Upper Confidence Bound (UCB) score.
  *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child[] = "Find the child with the highest Upper Confidence Bound (UCB) score.\n        ucb = (x / n) + C * sqrt(ln(N) / n)\n        x=reward for this node\n        n=number of simulations for this node\n        N=number of simulations for parent node\n        C=exploration bias\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child = {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_node = 0;
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
+  double __pyx_v_exploration_bias;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_best_child (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_node,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -4820,449 +5779,2396 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 213, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 269, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 213, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 269, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_node = values[1];
+    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
+    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 213, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 269, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(__pyx_self, __pyx_v_self, __pyx_v_node);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
   int __pyx_v_visits;
   double __pyx_v_reward;
-  double __pyx_v_subreward;
   double __pyx_v_ucb;
-  double __pyx_v_exploration_bias;
+  double __pyx_v_C;
   double __pyx_v_ln_parent_visits;
-  PyObject *__pyx_v_cur_team = NULL;
+  std::string __pyx_v_cur_team;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best_child = 0;
+  std::pair<std::string,float>  __pyx_v_item;
   double __pyx_v_best_score;
-  PyObject *__pyx_v_best_child = NULL;
-  PyObject *__pyx_v_child = NULL;
-  PyObject *__pyx_r = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  double __pyx_t_2;
+  double __pyx_t_1;
+  std::string __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   PyObject *(*__pyx_t_6)(PyObject *);
   int __pyx_t_7;
   int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  Py_ssize_t __pyx_t_10;
-  PyObject *(*__pyx_t_11)(PyObject *);
+  std::map<std::string,float> ::iterator __pyx_t_9;
+  std::map<std::string,float>  *__pyx_t_10;
+  std::pair<std::string,float>  __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
 
-  /* "multimcts/mcts.pyx":224
+  /* "multimcts/mcts.pyx":280
  *         cdef int visits
- *         cdef double reward, subreward, ucb
- *         cdef double exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
- *         cdef double ln_parent_visits = log(node.num_visits)
+ *         cdef double reward, ucb
+ *         cdef double C = exploration_bias             # <<<<<<<<<<<<<<
+ *         cdef double ln_parent_visits = node.log_visits
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_exploration_bias = __pyx_t_2;
+  __pyx_v_C = __pyx_v_exploration_bias;
 
-  /* "multimcts/mcts.pyx":225
- *         cdef double reward, subreward, ucb
- *         cdef double exploration_bias = self.exploration_bias
- *         cdef double ln_parent_visits = log(node.num_visits)             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":281
+ *         cdef double reward, ucb
+ *         cdef double C = exploration_bias
+ *         cdef double ln_parent_visits = node.log_visits             # <<<<<<<<<<<<<<
  * 
- *         cur_team = node.state.get_current_team()
+ *         cdef string cur_team = node._team
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_ln_parent_visits = log(__pyx_t_2);
+  __pyx_t_1 = __pyx_v_node->log_visits;
+  __pyx_v_ln_parent_visits = __pyx_t_1;
 
-  /* "multimcts/mcts.pyx":227
- *         cdef double ln_parent_visits = log(node.num_visits)
+  /* "multimcts/mcts.pyx":283
+ *         cdef double ln_parent_visits = node.log_visits
  * 
- *         cur_team = node.state.get_current_team()             # <<<<<<<<<<<<<<
+ *         cdef string cur_team = node._team             # <<<<<<<<<<<<<<
  * 
- *         cdef double best_score = -INFINITY
+ *         cdef Node child, best_child
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_v_cur_team = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_v_node->_team;
+  __pyx_v_cur_team = __pyx_t_2;
 
-  /* "multimcts/mcts.pyx":229
- *         cur_team = node.state.get_current_team()
+  /* "multimcts/mcts.pyx":288
+ *         cdef pair[string,float] item
  * 
  *         cdef double best_score = -INFINITY             # <<<<<<<<<<<<<<
- *         best_child:Node = None
  * 
+ *         for child in node.children:
  */
   __pyx_v_best_score = (-INFINITY);
 
-  /* "multimcts/mcts.pyx":230
- * 
+  /* "multimcts/mcts.pyx":290
  *         cdef double best_score = -INFINITY
- *         best_child:Node = None             # <<<<<<<<<<<<<<
- * 
- *         for child in node.children:
- */
-  __Pyx_INCREF(Py_None);
-  __pyx_v_best_child = Py_None;
-
-  /* "multimcts/mcts.pyx":232
- *         best_child:Node = None
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child.num_visits
+ *             visits = child._num_visits
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_4 = __pyx_t_1; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
+    __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 290, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
-      __pyx_t_1 = __pyx_t_6(__pyx_t_4);
-      if (unlikely(!__pyx_t_1)) {
+      __pyx_t_3 = __pyx_t_6(__pyx_t_4);
+      if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 232, __pyx_L1_error)
+          else __PYX_ERR(0, 290, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_GOTREF(__pyx_t_3);
     }
-    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_1);
-    __pyx_t_1 = 0;
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 290, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_3));
+    __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":233
+    /* "multimcts/mcts.pyx":291
  * 
  *         for child in node.children:
- *             visits = child.num_visits             # <<<<<<<<<<<<<<
+ *             visits = child._num_visits             # <<<<<<<<<<<<<<
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  *                 continue
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_7 = __pyx_v_child->_num_visits;
     __pyx_v_visits = __pyx_t_7;
 
-    /* "multimcts/mcts.pyx":234
+    /* "multimcts/mcts.pyx":292
  *         for child in node.children:
- *             visits = child.num_visits
+ *             visits = child._num_visits
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
     __pyx_t_8 = ((__pyx_v_visits == 0) != 0);
     if (__pyx_t_8) {
 
-      /* "multimcts/mcts.pyx":235
- *             visits = child.num_visits
+      /* "multimcts/mcts.pyx":293
+ *             visits = child._num_visits
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             # Relative reward is this child's reward minus its siblings' rewards.
  */
       goto __pyx_L3_continue;
 
-      /* "multimcts/mcts.pyx":234
+      /* "multimcts/mcts.pyx":292
  *         for child in node.children:
- *             visits = child.num_visits
+ *             visits = child._num_visits
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
     }
 
-    /* "multimcts/mcts.pyx":238
+    /* "multimcts/mcts.pyx":296
  * 
  *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child.total_reward[cur_team]             # <<<<<<<<<<<<<<
- *             for subreward in child.total_reward.values():
- *                 reward -= subreward
+ *             reward = 2 * child._total_reward[cur_team]             # <<<<<<<<<<<<<<
+ *             for item in child._total_reward:
+ *                 reward -= item.second
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_reward = __pyx_t_2;
+    __pyx_v_reward = (2.0 * (__pyx_v_child->_total_reward[__pyx_v_cur_team]));
 
-    /* "multimcts/mcts.pyx":239
+    /* "multimcts/mcts.pyx":297
  *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child.total_reward[cur_team]
- *             for subreward in child.total_reward.values():             # <<<<<<<<<<<<<<
- *                 reward -= subreward
+ *             reward = 2 * child._total_reward[cur_team]
+ *             for item in child._total_reward:             # <<<<<<<<<<<<<<
+ *                 reward -= item.second
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
-      }
-    }
-    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-      __pyx_t_9 = __pyx_t_1; __Pyx_INCREF(__pyx_t_9); __pyx_t_10 = 0;
-      __pyx_t_11 = NULL;
-    } else {
-      __pyx_t_10 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 239, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_11 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 239, __pyx_L1_error)
-    }
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_10 = &__pyx_v_child->_total_reward;
+    __pyx_t_9 = __pyx_t_10->begin();
     for (;;) {
-      if (likely(!__pyx_t_11)) {
-        if (likely(PyList_CheckExact(__pyx_t_9))) {
-          if (__pyx_t_10 >= PyList_GET_SIZE(__pyx_t_9)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
-          #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          #endif
-        } else {
-          if (__pyx_t_10 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely(0 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
-          #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_9, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          #endif
-        }
-      } else {
-        __pyx_t_1 = __pyx_t_11(__pyx_t_9);
-        if (unlikely(!__pyx_t_1)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 239, __pyx_L1_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_1);
-      }
-      __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_v_subreward = __pyx_t_2;
+      if (!(__pyx_t_9 != __pyx_t_10->end())) break;
+      __pyx_t_11 = *__pyx_t_9;
+      ++__pyx_t_9;
+      __pyx_v_item = __pyx_t_11;
 
-      /* "multimcts/mcts.pyx":240
- *             reward = 2 * child.total_reward[cur_team]
- *             for subreward in child.total_reward.values():
- *                 reward -= subreward             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":298
+ *             reward = 2 * child._total_reward[cur_team]
+ *             for item in child._total_reward:
+ *                 reward -= item.second             # <<<<<<<<<<<<<<
  * 
- *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+ *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
  */
-      __pyx_v_reward = (__pyx_v_reward - __pyx_v_subreward);
+      __pyx_v_reward = (__pyx_v_reward - __pyx_v_item.second);
 
-      /* "multimcts/mcts.pyx":239
+      /* "multimcts/mcts.pyx":297
  *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child.total_reward[cur_team]
- *             for subreward in child.total_reward.values():             # <<<<<<<<<<<<<<
- *                 reward -= subreward
+ *             reward = 2 * child._total_reward[cur_team]
+ *             for item in child._total_reward:             # <<<<<<<<<<<<<<
+ *                 reward -= item.second
  * 
  */
     }
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "multimcts/mcts.pyx":242
- *                 reward -= subreward
+    /* "multimcts/mcts.pyx":300
+ *                 reward -= item.second
  * 
- *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
+ *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
  * 
  *             if ucb > best_score:
  */
-    __pyx_v_ucb = ((__pyx_v_reward / __pyx_v_visits) + (__pyx_v_exploration_bias * sqrt((__pyx_v_ln_parent_visits / __pyx_v_visits))));
+    __pyx_v_ucb = ((__pyx_v_reward / ((double)__pyx_v_visits)) + (__pyx_v_C * sqrt((__pyx_v_ln_parent_visits / ((double)__pyx_v_visits)))));
 
-    /* "multimcts/mcts.pyx":244
- *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+    /* "multimcts/mcts.pyx":302
+ *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
  * 
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
     __pyx_t_8 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
     if (__pyx_t_8) {
 
-      /* "multimcts/mcts.pyx":245
+      /* "multimcts/mcts.pyx":303
  * 
  *             if ucb > best_score:
  *                 best_score = ucb             # <<<<<<<<<<<<<<
  *                 best_child = child
  * 
  */
       __pyx_v_best_score = __pyx_v_ucb;
 
-      /* "multimcts/mcts.pyx":246
+      /* "multimcts/mcts.pyx":304
  *             if ucb > best_score:
  *                 best_score = ucb
  *                 best_child = child             # <<<<<<<<<<<<<<
  * 
  *         return best_child
  */
-      __Pyx_INCREF(__pyx_v_child);
-      __Pyx_DECREF_SET(__pyx_v_best_child, __pyx_v_child);
+      __Pyx_INCREF(((PyObject *)__pyx_v_child));
+      __Pyx_XDECREF_SET(__pyx_v_best_child, __pyx_v_child);
 
-      /* "multimcts/mcts.pyx":244
- *             ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+      /* "multimcts/mcts.pyx":302
+ *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
  * 
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
     }
 
-    /* "multimcts/mcts.pyx":232
- *         best_child:Node = None
+    /* "multimcts/mcts.pyx":290
+ *         cdef double best_score = -INFINITY
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child.num_visits
+ *             visits = child._num_visits
  *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
  */
     __pyx_L3_continue:;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":248
+  /* "multimcts/mcts.pyx":306
  *                 best_child = child
  * 
  *         return best_child             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_best_child);
+  __Pyx_XDECREF(((PyObject *)__pyx_r));
+  if (unlikely(!__pyx_v_best_child)) { __Pyx_RaiseUnboundLocalError("best_child"); __PYX_ERR(0, 306, __pyx_L1_error) }
+  __Pyx_INCREF(((PyObject *)__pyx_v_best_child));
   __pyx_r = __pyx_v_best_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":213
- * 
- *     @cython.cdivision(True)
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":269
+ *     @cython.boundscheck(False)
+ *     @cython.wraparound(False)
+ *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
  *         """Find the child with the highest Upper Confidence Bound (UCB) score.
  *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_cur_team);
-  __Pyx_XDECREF(__pyx_v_best_child);
-  __Pyx_XDECREF(__pyx_v_child);
+  __Pyx_XDECREF((PyObject *)__pyx_v_child);
+  __Pyx_XDECREF((PyObject *)__pyx_v_best_child);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self.exploration_bias,)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ */
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_v_state = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self.exploration_bias,)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_2 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v__dict = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "(tree fragment)":7
+ *     state = (self.exploration_bias,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_3 = (__pyx_v__dict != Py_None);
+  __pyx_t_4 = (__pyx_t_3 != 0);
+  if (__pyx_t_4) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v__dict);
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_1));
+    __pyx_t_1 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = False
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = (self.exploration_bias,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = False             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, None), state
+ */
+  /*else*/ {
+    __pyx_v_use_setstate = 0;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = False
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, None), state
+ *     else:
+ */
+  __pyx_t_4 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_4) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = False
+ *     if use_setstate:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pyx_unpickle_MCTS); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_203704333);
+    __Pyx_GIVEREF(__pyx_int_203704333);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_203704333);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_2, 2, Py_None);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    __pyx_t_1 = 0;
+    __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = False
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, None), state
+ *     else:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_MCTS); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_203704333);
+    __Pyx_GIVEREF(__pyx_int_203704333);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_203704333);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_state);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ */
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_1__pyx_unpickle_Node(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_1__pyx_unpickle_Node = {"__pyx_unpickle_Node", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_1__pyx_unpickle_Node, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9multimcts_4mcts_1__pyx_unpickle_Node(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Node (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Node", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Node", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_Node") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Node", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Node", 0);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *     __pyx_result = Node.__new__(__pyx_type)
+ */
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = Node.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *     __pyx_result = Node.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *     __pyx_result = Node.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = Node.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *     __pyx_result = Node.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  std::string __pyx_t_4;
+  std::map<std::string,float>  __pyx_t_5;
+  double __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Node__set_state", 0);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[11])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->_children);
+  __Pyx_DECREF(__pyx_v___pyx_result->_children);
+  __pyx_v___pyx_result->_children = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->_is_fully_expanded = __pyx_t_2;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->_is_terminal = __pyx_t_2;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->_move);
+  __Pyx_DECREF(__pyx_v___pyx_result->_move);
+  __pyx_v___pyx_result->_move = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->_num_visits = __pyx_t_3;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->_parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->_parent));
+  __pyx_v___pyx_result->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 6, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->_remaining_moves);
+  __Pyx_DECREF(__pyx_v___pyx_result->_remaining_moves);
+  __pyx_v___pyx_result->_remaining_moves = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 7, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->_state);
+  __Pyx_DECREF(__pyx_v___pyx_result->_state);
+  __pyx_v___pyx_result->_state = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 8, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->_team = __pyx_t_4;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 9, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __pyx_convert_map_from_py_std_3a__3a_string__and_float(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->_total_reward = __pyx_t_5;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 10, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->log_visits = __pyx_t_6;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[11])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_7 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_8 = ((__pyx_t_7 > 11) != 0);
+  if (__pyx_t_8) {
+  } else {
+    __pyx_t_2 = __pyx_t_8;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_8 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_9 = (__pyx_t_8 != 0);
+  __pyx_t_2 = __pyx_t_9;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[11])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_update); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_10 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 11, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_12 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
+      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+      if (likely(__pyx_t_12)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+        __Pyx_INCREF(__pyx_t_12);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_11, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[11])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __pyx_unpickle_MCTS(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_3__pyx_unpickle_MCTS(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_3__pyx_unpickle_MCTS = {"__pyx_unpickle_MCTS", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_3__pyx_unpickle_MCTS, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9multimcts_4mcts_3__pyx_unpickle_MCTS(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_MCTS", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_MCTS", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_MCTS") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_MCTS", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS", 0);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ *     __pyx_result = MCTS.__new__(__pyx_type)
+ */
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = MCTS.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ *     __pyx_result = MCTS.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ *     __pyx_result = MCTS.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = MCTS.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
+ *     __pyx_result = MCTS.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_MCTS(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  double __pyx_t_2;
+  int __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS__set_state", 0);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
+ *     __pyx_result.exploration_bias = __pyx_state[0]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->exploration_bias = __pyx_t_2;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_4 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_5 = ((__pyx_t_4 > 1) != 0);
+  if (__pyx_t_5) {
+  } else {
+    __pyx_t_3 = __pyx_t_5;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_5 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_6 = (__pyx_t_5 != 0);
+  __pyx_t_3 = __pyx_t_6;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_update); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_7 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.exploration_bias = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":32
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":38
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":44
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":50
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":56
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
+  Py_ssize_t __pyx_v_length;
+  char const *__pyx_v_data;
+  std::string __pyx_r;
+  __Pyx_RefNannyDeclarations
+  char const *__pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
+
+  /* "string.from_py":14
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)
+ */
+  __pyx_v_length = 0;
+
+  /* "string.from_py":15
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
+ *     return string(data, length)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_v_data = __pyx_t_1;
+
+  /* "string.from_py":16
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = std::string(__pyx_v_data, __pyx_v_length);
+  goto __pyx_L0;
+
+  /* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "map.to_py":201
+ * 
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ *     o = {}
+ *     cdef const map[X,Y].value_type *key_value
+ */
+
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &__pyx_v_s) {
+  PyObject *__pyx_v_o = NULL;
+  std::map<std::string,float> ::value_type const *__pyx_v_key_value;
+  std::map<std::string,float> ::const_iterator __pyx_v_iter;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____float", 0);
+
+  /* "map.to_py":202
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):
+ *     o = {}             # <<<<<<<<<<<<<<
+ *     cdef const map[X,Y].value_type *key_value
+ *     cdef map[X,Y].const_iterator iter = s.begin()
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_o = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "map.to_py":204
+ *     o = {}
+ *     cdef const map[X,Y].value_type *key_value
+ *     cdef map[X,Y].const_iterator iter = s.begin()             # <<<<<<<<<<<<<<
+ *     while iter != s.end():
+ *         key_value = &cython.operator.dereference(iter)
+ */
+  __pyx_v_iter = __pyx_v_s.begin();
+
+  /* "map.to_py":205
+ *     cdef const map[X,Y].value_type *key_value
+ *     cdef map[X,Y].const_iterator iter = s.begin()
+ *     while iter != s.end():             # <<<<<<<<<<<<<<
+ *         key_value = &cython.operator.dereference(iter)
+ *         o[key_value.first] = key_value.second
+ */
+  while (1) {
+    __pyx_t_2 = ((__pyx_v_iter != __pyx_v_s.end()) != 0);
+    if (!__pyx_t_2) break;
+
+    /* "map.to_py":206
+ *     cdef map[X,Y].const_iterator iter = s.begin()
+ *     while iter != s.end():
+ *         key_value = &cython.operator.dereference(iter)             # <<<<<<<<<<<<<<
+ *         o[key_value.first] = key_value.second
+ *         cython.operator.preincrement(iter)
+ */
+    __pyx_v_key_value = (&(*__pyx_v_iter));
+
+    /* "map.to_py":207
+ *     while iter != s.end():
+ *         key_value = &cython.operator.dereference(iter)
+ *         o[key_value.first] = key_value.second             # <<<<<<<<<<<<<<
+ *         cython.operator.preincrement(iter)
+ *     return o
+ */
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_key_value->second); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_key_value->first); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (unlikely(PyDict_SetItem(__pyx_v_o, __pyx_t_3, __pyx_t_1) < 0)) __PYX_ERR(1, 207, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "map.to_py":208
+ *         key_value = &cython.operator.dereference(iter)
+ *         o[key_value.first] = key_value.second
+ *         cython.operator.preincrement(iter)             # <<<<<<<<<<<<<<
+ *     return o
+ * 
+ */
+    (void)((++__pyx_v_iter));
+  }
+
+  /* "map.to_py":209
+ *         o[key_value.first] = key_value.second
+ *         cython.operator.preincrement(iter)
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "map.to_py":201
+ * 
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ *     o = {}
+ *     cdef const map[X,Y].value_type *key_value
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "map.from_py":174
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef dict d = o
+ *     cdef map[X,Y] m
+ */
+
+static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *__pyx_v_o) {
+  PyObject *__pyx_v_d = 0;
+  std::map<std::string,float>  __pyx_v_m;
+  PyObject *__pyx_v_key = NULL;
+  PyObject *__pyx_v_value = NULL;
+  std::map<std::string,float>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  std::string __pyx_t_8;
+  float __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_float", 0);
+
+  /* "map.from_py":175
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:
+ *     cdef dict d = o             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     for key, value in d.iteritems():
+ */
+  if (!(likely(PyDict_CheckExact(__pyx_v_o))||((__pyx_v_o) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_o)->tp_name), 0))) __PYX_ERR(1, 175, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_o;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_v_d = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "map.from_py":177
+ *     cdef dict d = o
+ *     cdef map[X,Y] m
+ *     for key, value in d.iteritems():             # <<<<<<<<<<<<<<
+ *         m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m
+ */
+  __pyx_t_2 = 0;
+  if (unlikely(__pyx_v_d == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
+    __PYX_ERR(1, 177, __pyx_L1_error)
+  }
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_d, 1, __pyx_n_s_iteritems, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_1);
+  __pyx_t_1 = __pyx_t_5;
+  __pyx_t_5 = 0;
+  while (1) {
+    __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_4);
+    if (unlikely(__pyx_t_7 == 0)) break;
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(1, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
+    __pyx_t_6 = 0;
+
+    /* "map.from_py":178
+ *     cdef map[X,Y] m
+ *     for key, value in d.iteritems():
+ *         m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     return m
+ * 
+ */
+    __pyx_t_8 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+    __pyx_t_9 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_9 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+    __pyx_v_m.insert(std::pair<std::string,float> (((std::string)__pyx_t_8), ((float)__pyx_t_9)));
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "map.from_py":179
+ *     for key, value in d.iteritems():
+ *         m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_m;
+  goto __pyx_L0;
+
+  /* "map.from_py":174
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef dict d = o
+ *     cdef map[X,Y] m
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_d);
+  __Pyx_XDECREF(__pyx_v_key);
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_9multimcts_4mcts_Node *p;
+  PyObject *o;
+  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  p = ((struct __pyx_obj_9multimcts_4mcts_Node *)o);
+  new((void*)&(p->_team)) std::string();
+  new((void*)&(p->_total_reward)) std::map<std::string,float> ();
+  p->_state = Py_None; Py_INCREF(Py_None);
+  p->_move = Py_None; Py_INCREF(Py_None);
+  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  p->_children = Py_None; Py_INCREF(Py_None);
+  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  return o;
+}
+
+static void __pyx_tp_dealloc_9multimcts_4mcts_Node(PyObject *o) {
+  struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  __Pyx_call_destructor(p->_team);
+  __Pyx_call_destructor(p->_total_reward);
+  Py_CLEAR(p->_state);
+  Py_CLEAR(p->_move);
+  Py_CLEAR(p->_parent);
+  Py_CLEAR(p->_children);
+  Py_CLEAR(p->_remaining_moves);
+  (*Py_TYPE(o)->tp_free)(o);
+}
+
+static int __pyx_tp_traverse_9multimcts_4mcts_Node(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
+  if (p->_state) {
+    e = (*v)(p->_state, a); if (e) return e;
+  }
+  if (p->_move) {
+    e = (*v)(p->_move, a); if (e) return e;
+  }
+  if (p->_parent) {
+    e = (*v)(((PyObject *)p->_parent), a); if (e) return e;
+  }
+  if (p->_children) {
+    e = (*v)(p->_children, a); if (e) return e;
+  }
+  if (p->_remaining_moves) {
+    e = (*v)(p->_remaining_moves, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_9multimcts_4mcts_Node(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
+  tmp = ((PyObject*)p->_state);
+  p->_state = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->_move);
+  p->_move = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->_parent);
+  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->_children);
+  p->_children = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->_remaining_moves);
+  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_state(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_parent(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_move(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_children(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_remaining_moves(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(o);
+}
+
+static PyMethodDef __pyx_methods_9multimcts_4mcts_Node[] = {
+  {"visit", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_3visit, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__, METH_O, 0},
+  {0, 0, 0, 0}
+};
+
+static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_Node[] = {
+  {(char *)"state", __pyx_getprop_9multimcts_4mcts_4Node_state, 0, (char *)0, 0},
+  {(char *)"parent", __pyx_getprop_9multimcts_4mcts_4Node_parent, 0, (char *)0, 0},
+  {(char *)"move", __pyx_getprop_9multimcts_4mcts_4Node_move, 0, (char *)0, 0},
+  {(char *)"children", __pyx_getprop_9multimcts_4mcts_4Node_children, 0, (char *)0, 0},
+  {(char *)"remaining_moves", __pyx_getprop_9multimcts_4mcts_4Node_remaining_moves, 0, (char *)0, 0},
+  {0, 0, 0, 0, 0}
+};
+
+static PyTypeObject __pyx_type_9multimcts_4mcts_Node = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "multimcts.mcts.Node", /*tp_name*/
+  sizeof(struct __pyx_obj_9multimcts_4mcts_Node), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9multimcts_4mcts_Node, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n\n    Attributes:\n        children (list): The child nodes of the current node. These represent legal moves that have been visited.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ", /*tp_doc*/
+  __pyx_tp_traverse_9multimcts_4mcts_Node, /*tp_traverse*/
+  __pyx_tp_clear_9multimcts_4mcts_Node, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_9multimcts_4mcts_Node, /*tp_methods*/
+  0, /*tp_members*/
+  __pyx_getsets_9multimcts_4mcts_Node, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  __pyx_pw_9multimcts_4mcts_4Node_1__init__, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9multimcts_4mcts_Node, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+
+static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  PyObject *o;
+  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  return o;
+}
+
+static void __pyx_tp_dealloc_9multimcts_4mcts_MCTS(PyObject *o) {
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  }
+  #endif
+  (*Py_TYPE(o)->tp_free)(o);
+}
+
+static PyObject *__pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(o);
+}
+
+static PyMethodDef __pyx_methods_9multimcts_4mcts_MCTS[] = {
+  {"search", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_3search, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_2search},
+  {"select", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_5select, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_4select},
+  {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand},
+  {"simulate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_9simulate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_8simulate},
+  {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate},
+  {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__, METH_O, 0},
+  {0, 0, 0, 0}
+};
+
+static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_MCTS[] = {
+  {(char *)"exploration_bias", __pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias, 0, (char *)0, 0},
+  {0, 0, 0, 0, 0}
+};
+
+static PyTypeObject __pyx_type_9multimcts_4mcts_MCTS = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "multimcts.mcts.MCTS", /*tp_name*/
+  sizeof(struct __pyx_obj_9multimcts_4mcts_MCTS), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9multimcts_4mcts_MCTS, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  0, /*tp_doc*/
+  0, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_9multimcts_4mcts_MCTS, /*tp_methods*/
+  0, /*tp_members*/
+  __pyx_getsets_9multimcts_4mcts_MCTS, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  __pyx_pw_9multimcts_4mcts_4MCTS_1__init__, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9multimcts_4mcts_MCTS, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
@@ -5304,385 +8210,338 @@
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
   {&__pyx_n_s_Dict, __pyx_k_Dict, sizeof(__pyx_k_Dict), 0, 0, 1, 1},
   {&__pyx_n_s_GameState, __pyx_k_GameState, sizeof(__pyx_k_GameState), 0, 0, 1, 1},
+  {&__pyx_n_u_GameState, __pyx_k_GameState, sizeof(__pyx_k_GameState), 0, 1, 0, 1},
   {&__pyx_n_s_GameState_get_current_team, __pyx_k_GameState_get_current_team, sizeof(__pyx_k_GameState_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_legal_moves, __pyx_k_GameState_get_legal_moves, sizeof(__pyx_k_GameState_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_reward, __pyx_k_GameState_get_reward, sizeof(__pyx_k_GameState_get_reward), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_is_terminal, __pyx_k_GameState_is_terminal, sizeof(__pyx_k_GameState_is_terminal), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_make_move, __pyx_k_GameState_make_move, sizeof(__pyx_k_GameState_make_move), 0, 0, 1, 1},
-  {&__pyx_kp_s_GameState_must_implement_get_cur, __pyx_k_GameState_must_implement_get_cur, sizeof(__pyx_k_GameState_must_implement_get_cur), 0, 0, 1, 0},
-  {&__pyx_kp_s_GameState_must_implement_get_leg, __pyx_k_GameState_must_implement_get_leg, sizeof(__pyx_k_GameState_must_implement_get_leg), 0, 0, 1, 0},
-  {&__pyx_kp_s_GameState_must_implement_get_rew, __pyx_k_GameState_must_implement_get_rew, sizeof(__pyx_k_GameState_must_implement_get_rew), 0, 0, 1, 0},
-  {&__pyx_kp_s_GameState_must_implement_is_term, __pyx_k_GameState_must_implement_is_term, sizeof(__pyx_k_GameState_must_implement_is_term), 0, 0, 1, 0},
-  {&__pyx_kp_s_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 0, 1, 0},
+  {&__pyx_kp_u_GameState_must_implement_get_cur, __pyx_k_GameState_must_implement_get_cur, sizeof(__pyx_k_GameState_must_implement_get_cur), 0, 1, 0, 0},
+  {&__pyx_kp_u_GameState_must_implement_get_leg, __pyx_k_GameState_must_implement_get_leg, sizeof(__pyx_k_GameState_must_implement_get_leg), 0, 1, 0, 0},
+  {&__pyx_kp_u_GameState_must_implement_get_rew, __pyx_k_GameState_must_implement_get_rew, sizeof(__pyx_k_GameState_must_implement_get_rew), 0, 1, 0, 0},
+  {&__pyx_kp_u_GameState_must_implement_is_term, __pyx_k_GameState_must_implement_is_term, sizeof(__pyx_k_GameState_must_implement_is_term), 0, 1, 0, 0},
+  {&__pyx_kp_u_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 1, 0, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_u_Invalid_return_type, __pyx_k_Invalid_return_type, sizeof(__pyx_k_Invalid_return_type), 0, 1, 0, 0},
   {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS, __pyx_k_MCTS, sizeof(__pyx_k_MCTS), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS___init, __pyx_k_MCTS___init, sizeof(__pyx_k_MCTS___init), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_backpropagate, __pyx_k_MCTS_backpropagate, sizeof(__pyx_k_MCTS_backpropagate), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_expand, __pyx_k_MCTS_expand, sizeof(__pyx_k_MCTS_expand), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_get_best_child, __pyx_k_MCTS_get_best_child, sizeof(__pyx_k_MCTS_get_best_child), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_search, __pyx_k_MCTS_search, sizeof(__pyx_k_MCTS_search), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_select, __pyx_k_MCTS_select, sizeof(__pyx_k_MCTS_select), 0, 0, 1, 1},
-  {&__pyx_n_s_MCTS_simulate, __pyx_k_MCTS_simulate, sizeof(__pyx_k_MCTS_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_Move, __pyx_k_Move, sizeof(__pyx_k_Move), 0, 0, 1, 1},
   {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
-  {&__pyx_n_s_Node___init, __pyx_k_Node___init, sizeof(__pyx_k_Node___init), 0, 0, 1, 1},
+  {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
-  {&__pyx_kp_s_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 0, 1, 0},
-  {&__pyx_kp_s_Represents_a_game_state_node_in, __pyx_k_Represents_a_game_state_node_in, sizeof(__pyx_k_Represents_a_game_state_node_in), 0, 0, 1, 0},
+  {&__pyx_kp_u_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 1, 0, 0},
+  {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Rewards, __pyx_k_Rewards, sizeof(__pyx_k_Rewards), 0, 0, 1, 1},
   {&__pyx_n_s_Team, __pyx_k_Team, sizeof(__pyx_k_Team), 0, 0, 1, 1},
-  {&__pyx_kp_s_Tried_to_expand_a_node_with_no_r, __pyx_k_Tried_to_expand_a_node_with_no_r, sizeof(__pyx_k_Tried_to_expand_a_node_with_no_r), 0, 0, 1, 0},
+  {&__pyx_kp_u_Tried_to_expand_a_node_with_no_r, __pyx_k_Tried_to_expand_a_node_with_no_r, sizeof(__pyx_k_Tried_to_expand_a_node_with_no_r), 0, 1, 0, 0},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
-  {&__pyx_n_s_VALID_RETURN_TYPES, __pyx_k_VALID_RETURN_TYPES, sizeof(__pyx_k_VALID_RETURN_TYPES), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_backpropagate, __pyx_k_backpropagate, sizeof(__pyx_k_backpropagate), 0, 0, 1, 1},
-  {&__pyx_n_s_best, __pyx_k_best, sizeof(__pyx_k_best), 0, 0, 1, 1},
-  {&__pyx_n_s_best_child, __pyx_k_best_child, sizeof(__pyx_k_best_child), 0, 0, 1, 1},
-  {&__pyx_n_s_best_score, __pyx_k_best_score, sizeof(__pyx_k_best_score), 0, 0, 1, 1},
   {&__pyx_n_s_child, __pyx_k_child, sizeof(__pyx_k_child), 0, 0, 1, 1},
   {&__pyx_n_s_children, __pyx_k_children, sizeof(__pyx_k_children), 0, 0, 1, 1},
   {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
+  {&__pyx_n_s_ckey, __pyx_k_ckey, sizeof(__pyx_k_ckey), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
-  {&__pyx_n_s_cur_team, __pyx_k_cur_team, sizeof(__pyx_k_cur_team), 0, 0, 1, 1},
-  {&__pyx_n_s_defaultdict, __pyx_k_defaultdict, sizeof(__pyx_k_defaultdict), 0, 0, 1, 1},
+  {&__pyx_n_s_creward, __pyx_k_creward, sizeof(__pyx_k_creward), 0, 0, 1, 1},
+  {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_end_time, __pyx_k_end_time, sizeof(__pyx_k_end_time), 0, 0, 1, 1},
   {&__pyx_n_s_expand, __pyx_k_expand, sizeof(__pyx_k_expand), 0, 0, 1, 1},
   {&__pyx_n_s_exploration_bias, __pyx_k_exploration_bias, sizeof(__pyx_k_exploration_bias), 0, 0, 1, 1},
-  {&__pyx_n_u_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 1, 0, 1},
   {&__pyx_n_s_get_best_child, __pyx_k_get_best_child, sizeof(__pyx_k_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_get_current_team, __pyx_k_get_current_team, sizeof(__pyx_k_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_get_legal_moves, __pyx_k_get_legal_moves, sizeof(__pyx_k_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_get_reward, __pyx_k_get_reward, sizeof(__pyx_k_get_reward), 0, 0, 1, 1},
+  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_heuristic, __pyx_k_heuristic, sizeof(__pyx_k_heuristic), 0, 0, 1, 1},
-  {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_u_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 1, 0, 1},
-  {&__pyx_n_s_is_fully_expanded, __pyx_k_is_fully_expanded, sizeof(__pyx_k_is_fully_expanded), 0, 0, 1, 1},
   {&__pyx_n_s_is_terminal, __pyx_k_is_terminal, sizeof(__pyx_k_is_terminal), 0, 0, 1, 1},
+  {&__pyx_n_s_item, __pyx_k_item, sizeof(__pyx_k_item), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
-  {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
+  {&__pyx_n_s_iteritems, __pyx_k_iteritems, sizeof(__pyx_k_iteritems), 0, 0, 1, 1},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
-  {&__pyx_n_s_ln_parent_visits, __pyx_k_ln_parent_visits, sizeof(__pyx_k_ln_parent_visits), 0, 0, 1, 1},
   {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_make_move, __pyx_k_make_move, sizeof(__pyx_k_make_move), 0, 0, 1, 1},
   {&__pyx_n_s_max_iterations, __pyx_k_max_iterations, sizeof(__pyx_k_max_iterations), 0, 0, 1, 1},
   {&__pyx_n_s_max_time, __pyx_k_max_time, sizeof(__pyx_k_max_time), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 0, 1, 1},
+  {&__pyx_n_u_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 1, 0, 1},
   {&__pyx_n_s_multimcts_mcts, __pyx_k_multimcts_mcts, sizeof(__pyx_k_multimcts_mcts), 0, 0, 1, 1},
   {&__pyx_kp_s_multimcts_mcts_pyx, __pyx_k_multimcts_mcts_pyx, sizeof(__pyx_k_multimcts_mcts_pyx), 0, 0, 1, 0},
   {&__pyx_kp_u_must_be_one_of, __pyx_k_must_be_one_of, sizeof(__pyx_k_must_be_one_of), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+  {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 0, 1, 1},
-  {&__pyx_n_s_num_visits, __pyx_k_num_visits, sizeof(__pyx_k_num_visits), 0, 0, 1, 1},
+  {&__pyx_n_u_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 1, 0, 1},
   {&__pyx_n_s_parent, __pyx_k_parent, sizeof(__pyx_k_parent), 0, 0, 1, 1},
+  {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_MCTS, __pyx_k_pyx_unpickle_MCTS, sizeof(__pyx_k_pyx_unpickle_MCTS), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_Node, __pyx_k_pyx_unpickle_Node, sizeof(__pyx_k_pyx_unpickle_Node), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_remaining_moves, __pyx_k_remaining_moves, sizeof(__pyx_k_remaining_moves), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_return_type, __pyx_k_return_type, sizeof(__pyx_k_return_type), 0, 0, 1, 1},
   {&__pyx_n_s_reward, __pyx_k_reward, sizeof(__pyx_k_reward), 0, 0, 1, 1},
-  {&__pyx_n_s_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 0, 1, 1},
   {&__pyx_n_s_select, __pyx_k_select, sizeof(__pyx_k_select), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
   {&__pyx_n_s_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
+  {&__pyx_n_u_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 1, 0, 1},
   {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
-  {&__pyx_n_u_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 1, 0, 1},
-  {&__pyx_n_s_subreward, __pyx_k_subreward, sizeof(__pyx_k_subreward), 0, 0, 1, 1},
-  {&__pyx_n_s_terminal_team, __pyx_k_terminal_team, sizeof(__pyx_k_terminal_team), 0, 0, 1, 1},
+  {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-  {&__pyx_n_s_total_reward, __pyx_k_total_reward, sizeof(__pyx_k_total_reward), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
-  {&__pyx_n_s_ucb, __pyx_k_ucb, sizeof(__pyx_k_ucb), 0, 0, 1, 1},
-  {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
-  {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
-  {&__pyx_n_s_visits, __pyx_k_visits, sizeof(__pyx_k_visits), 0, 0, 1, 1},
+  {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+  {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
+  {&__pyx_n_s_visit, __pyx_k_visit, sizeof(__pyx_k_visit), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 153, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 203, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "multimcts/mcts.pyx":19
+  /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "multimcts/mcts.pyx":23
+  /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "multimcts/mcts.pyx":29
+  /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "multimcts/mcts.pyx":33
+  /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
- *     def get_reward(self) -> Union[float, Rewards]:
+ *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "multimcts/mcts.pyx":41
+  /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "multimcts/mcts.pyx":108
+  /* "multimcts/mcts.pyx":149
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "multimcts/mcts.pyx":161
+  /* "multimcts/mcts.pyx":204
  *             move = node.remaining_moves.pop()
  *         except IndexError:
  *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
  * 
  *         child = Node(state=node.state.make_move(move), parent=node, move=move)
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "multimcts/mcts.pyx":17
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ */
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_24284988, __pyx_int_53904430, __pyx_int_227935910); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+
+  /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 22, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":21
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":31
+  /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 36, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":35
+  /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Rewards]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 35, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":60
- *         remaining_moves (list): A list of moves that have not yet been tried.
- *     """
- *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self.state = state
- *         self.parent = parent
- */
-  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_parent, __pyx_n_s_move); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_tuple__20 = PyTuple_Pack(2, ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 40, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":80
- * 
- * class MCTS:
- *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
- *         """Initializes an MCTS agent.
- * 
- */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 80, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 80, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":90
- *         self.exploration_bias = exploration_bias
- * 
- *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
- *         """Searches for this state's best move until some limit has been reached.
- * 
- */
-  __pyx_tuple__23 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_max_time, __pyx_n_s_max_iterations, __pyx_n_s_heuristic, __pyx_n_s_return_type, __pyx_n_s_VALID_RETURN_TYPES, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward, __pyx_n_s_best); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 4, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 90, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":140
- *             return best
- * 
- *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 1: Selection
- *         Traverse the tree for the node we most want to simulate.
- */
-  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 140, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":154
+  /* "multimcts/mcts.pyx":197
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_tuple__27 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 154, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 154, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":171
- *         return child
- * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
- *         """Step 3: Simulation (aka playout/rollout)
- *         Play out a game, from the given node to termination, and return the final reward.
- */
-  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_heuristic, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 1, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 171, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 197, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":200
+  /* "multimcts/mcts.pyx":243
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_tuple__31 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 200, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 200, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":213
- * 
- *     @cython.cdivision(True)
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
- */
-  __pyx_tuple__33 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_visits, __pyx_n_s_reward, __pyx_n_s_subreward, __pyx_n_s_ucb, __pyx_n_s_exploration_bias, __pyx_n_s_ln_parent_visits, __pyx_n_s_cur_team, __pyx_n_s_best_score, __pyx_n_s_best_child, __pyx_n_s_child); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_val, __pyx_n_s_ckey, __pyx_n_s_creward, __pyx_n_s_key, __pyx_n_s_item); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 243, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 243, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyList_Type_pop.type = (PyObject*)&PyList_Type;
-  __pyx_umethod_PyString_Type_lower.type = (PyObject*)&PyString_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_24284988 = PyInt_FromLong(24284988L); if (unlikely(!__pyx_int_24284988)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_53904430 = PyInt_FromLong(53904430L); if (unlikely(!__pyx_int_53904430)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_82662024 = PyInt_FromLong(82662024L); if (unlikely(!__pyx_int_82662024)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_203704333 = PyInt_FromLong(203704333L); if (unlikely(!__pyx_int_203704333)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_227935910 = PyInt_FromLong(227935910L); if (unlikely(!__pyx_int_227935910)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_231097371 = PyInt_FromLong(231097371L); if (unlikely(!__pyx_int_231097371)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -5714,18 +8573,54 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_9multimcts_4mcts_Node.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_Node.tp_dictoffset && __pyx_type_9multimcts_4mcts_Node.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_9multimcts_4mcts_Node.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Node, (PyObject *)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_ptype_9multimcts_4mcts_Node = &__pyx_type_9multimcts_4mcts_Node;
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_9multimcts_4mcts_MCTS.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_MCTS.tp_dictoffset && __pyx_type_9multimcts_4mcts_MCTS.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_9multimcts_4mcts_MCTS.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
+  {
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_9multimcts_4mcts_MCTS, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 114, __pyx_L1_error)
+    if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
+      __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__.doc = __pyx_doc_9multimcts_4mcts_4MCTS___init__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
+    }
+  }
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MCTS, (PyObject *)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_ptype_9multimcts_4mcts_MCTS = &__pyx_type_9multimcts_4mcts_MCTS;
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -5843,17 +8738,14 @@
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -5942,673 +8834,424 @@
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  (void)__Pyx_modinit_type_init_code();
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "multimcts/mcts.pyx":1
+  /* "multimcts/mcts.pyx":5
+ * # cython: profile=False
+ * 
  * from time import time             # <<<<<<<<<<<<<<
  * from random import shuffle, choice
- * from collections import defaultdict
+ * from typing import Union, Dict, List, Any
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_time);
   __Pyx_GIVEREF(__pyx_n_s_time);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_time);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_time, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_time, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":2
+  /* "multimcts/mcts.pyx":6
+ * 
  * from time import time
  * from random import shuffle, choice             # <<<<<<<<<<<<<<
- * from collections import defaultdict
  * from typing import Union, Dict, List, Any
+ * 
  */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_shuffle);
   __Pyx_GIVEREF(__pyx_n_s_shuffle);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_shuffle);
   __Pyx_INCREF(__pyx_n_s_choice);
   __Pyx_GIVEREF(__pyx_n_s_choice);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_choice);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_choice); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_choice); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_choice, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_choice, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":3
+  /* "multimcts/mcts.pyx":7
  * from time import time
  * from random import shuffle, choice
- * from collections import defaultdict             # <<<<<<<<<<<<<<
- * from typing import Union, Dict, List, Any
- * 
- */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_defaultdict);
-  __Pyx_GIVEREF(__pyx_n_s_defaultdict);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_defaultdict);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_defaultdict, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "multimcts/mcts.pyx":4
- * from random import shuffle, choice
- * from collections import defaultdict
  * from typing import Union, Dict, List, Any             # <<<<<<<<<<<<<<
  * 
- * cimport cython
+ * from libc.math cimport log, sqrt, INFINITY
  */
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyList_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Union);
   __Pyx_GIVEREF(__pyx_n_s_Union);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Union);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Union);
   __Pyx_INCREF(__pyx_n_s_Dict);
   __Pyx_GIVEREF(__pyx_n_s_Dict);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Dict);
+  PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_Dict);
   __Pyx_INCREF(__pyx_n_s_List);
   __Pyx_GIVEREF(__pyx_n_s_List);
-  PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_List);
+  PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_List);
   __Pyx_INCREF(__pyx_n_s_Any);
   __Pyx_GIVEREF(__pyx_n_s_Any);
-  PyList_SET_ITEM(__pyx_t_2, 3, __pyx_n_s_Any);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Union, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dict, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_1, 3, __pyx_n_s_Any);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Union, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dict, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_List, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":11
+  /* "multimcts/mcts.pyx":16
  * 
  * 
  * Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.             # <<<<<<<<<<<<<<
  * Team = Union[int,str]
  * Rewards = Dict[Team,float]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Move, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Move, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":12
+  /* "multimcts/mcts.pyx":17
  * 
  * Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
  * Team = Union[int,str]             # <<<<<<<<<<<<<<
  * Rewards = Dict[Team,float]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&PyInt_Type)));
-  __Pyx_INCREF(((PyObject *)(&PyString_Type)));
-  __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
-  PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)(&PyString_Type)));
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyInt_Type)));
+  __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
+  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyUnicode_Type)));
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Team, __pyx_t_3) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Team, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "multimcts/mcts.pyx":13
+  /* "multimcts/mcts.pyx":18
  * Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
  * Team = Union[int,str]
  * Rewards = Dict[Team,float]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Team); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Team); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
-  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyFloat_Type)));
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)(&PyFloat_Type)));
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rewards, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rewards, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":16
+  /* "multimcts/mcts.pyx":21
  * 
  * 
  * class GameState:             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":17
+  /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_current_team, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "multimcts/mcts.pyx":21
+  /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
  *         """Returns a list of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_List); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Move); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Move); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_legal_moves, __pyx_t_5) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_move, __pyx_t_3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_u_GameState) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_make_move, __pyx_t_3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "multimcts/mcts.pyx":31
+  /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_terminal, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "multimcts/mcts.pyx":35
+  /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Rewards]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyFloat_Type)));
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_reward, __pyx_t_4) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":16
+  /* "multimcts/mcts.pyx":21
  * 
  * 
  * class GameState:             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "multimcts/mcts.pyx":44
- * 
- * 
- * class Node:             # <<<<<<<<<<<<<<
- *     """Represents a game state node in the MCTS search tree.
- * 
- */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-
-  /* "multimcts/mcts.pyx":60
- *         remaining_moves (list): A list of moves that have not yet been tried.
- *     """
- *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self.state = state
- *         self.parent = parent
- */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_GameState); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_state, __pyx_t_5) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Move); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_move, __pyx_t_5) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__20);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-  /* "multimcts/mcts.pyx":44
- * 
- * 
- * class Node:             # <<<<<<<<<<<<<<
- *     """Represents a game state node in the MCTS search tree.
- * 
- */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_5) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "multimcts/mcts.pyx":79
- * 
- * 
- * class MCTS:             # <<<<<<<<<<<<<<
- *     def __init__(self, exploration_bias:float=1.414):
- *         """Initializes an MCTS agent.
- */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-
-  /* "multimcts/mcts.pyx":80
- * 
- * class MCTS:
- *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
- *         """Initializes an MCTS agent.
- * 
- */
-  __pyx_t_5 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "multimcts/mcts.pyx":90
- *         self.exploration_bias = exploration_bias
- * 
- *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
- *         """Searches for this state's best move until some limit has been reached.
- * 
- */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return_type, ((PyObject*)__pyx_n_s_state)) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_GameState); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Union); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-  __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-  PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&PyInt_Type)));
-  __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
-  __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
-  PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)(&PyFloat_Type)));
-  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_4) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_max_time, __pyx_t_6) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return_type, __pyx_n_u_str) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Union); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_GameState); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Move); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
-  __pyx_t_3 = 0;
-  __pyx_t_4 = 0;
-  __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_1);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_search, __pyx_t_7) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":140
- *             return best
- * 
- *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 1: Selection
- *         Traverse the tree for the node we most want to simulate.
- */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_5) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_select, __pyx_t_5) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-  /* "multimcts/mcts.pyx":154
+  /* "multimcts/mcts.pyx":197
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
 
-  /* "multimcts/mcts.pyx":153
+  /* "multimcts/mcts.pyx":196
  *         return node
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def expand(node:Node) -> Node:
  *         """Step 2: Expansion
  */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_expand, __pyx_t_5) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-  /* "multimcts/mcts.pyx":171
- *         return child
- * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
- *         """Step 3: Simulation (aka playout/rollout)
- *         Play out a game, from the given node to termination, and return the final reward.
- */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_expand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_1) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_1, __pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_simulate, __pyx_t_1) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
 
-  /* "multimcts/mcts.pyx":200
+  /* "multimcts/mcts.pyx":243
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reward, __pyx_t_7) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_4) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
 
-  /* "multimcts/mcts.pyx":199
+  /* "multimcts/mcts.pyx":242
  *         return reward
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def backpropagate(node:Node, reward:Rewards):
  *         """Step 4: Backpropagation
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_4, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_backpropagate, __pyx_t_1) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
 
-  /* "multimcts/mcts.pyx":213
- * 
- *     @cython.cdivision(True)
- *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_1__pyx_unpickle_Node, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Node, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_best_child, __pyx_t_7) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":79
- * 
- * 
- * class MCTS:             # <<<<<<<<<<<<<<
- *     def __init__(self, exploration_bias:float=1.414):
- *         """Initializes an MCTS agent.
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_7) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_3__pyx_unpickle_MCTS, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MCTS, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
- * from time import time             # <<<<<<<<<<<<<<
- * from random import shuffle, choice
- * from collections import defaultdict
+ * # distutils: language=c++             # <<<<<<<<<<<<<<
+ * # cython: language_level=3
+ * # cython: profile=False
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "map.from_py":174
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef dict d = o
+ *     cdef map[X,Y] m
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init multimcts.mcts", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init multimcts.mcts");
@@ -7011,111 +9654,34 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#endif
-
-/* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
-    PyObject **dictptr = NULL;
-    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
-    if (offset) {
-#if CYTHON_COMPILING_IN_CPYTHON
-        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
-#else
-        dictptr = _PyObject_GetDictPtr(obj);
-#endif
-    }
-    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
-}
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
-        return 0;
-    return obj_dict_version == __Pyx_get_object_dict_version(obj);
-}
-#endif
-
-/* GetModuleGlobalName */
-#if CYTHON_USE_DICT_VERSIONS
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
-#else
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
-#endif
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
-    PyObject *result;
-#if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
-    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    } else if (unlikely(PyErr_Occurred())) {
-        return NULL;
-    }
-#else
-    result = PyDict_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
     }
-#endif
-#else
-    result = PyObject_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
     }
-    PyErr_Clear();
-#endif
-    return __Pyx_GetBuiltinName(name);
-}
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
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
 }
-#endif
 
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
@@ -7228,43 +9794,14 @@
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
 #endif
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
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
-}
-
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
     self = PyCFunction_GET_SELF(func);
@@ -7277,14 +9814,59 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
+/* PyObjectCallNoArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
+/* PyCFunctionFastCall */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    }
+}
+#endif
+
 /* PyObjectCallOneArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
     PyObject *args = PyTuple_New(1);
     if (unlikely(!args)) return NULL;
     Py_INCREF(arg);
@@ -7317,94 +9899,155 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
 #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
 #else
-    if (likely(PyCFunction_Check(func)))
+        dictptr = _PyObject_GetDictPtr(obj);
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+}
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
+        return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+/* GetModuleGlobalName */
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+#else
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+#endif
 {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
+    PyObject *result;
+#if !CYTHON_AVOID_BORROWED_REFS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    } else if (unlikely(PyErr_Occurred())) {
+        return NULL;
     }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
+#else
+    result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
     }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+#endif
+#else
+    result = PyObject_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
     }
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
-    return 0;
+    PyErr_Clear();
+#endif
+    return __Pyx_GetBuiltinName(name);
 }
 
-/* UnpackUnboundCMethod */
-static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
-    PyObject *method;
-    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
-    if (unlikely(!method))
-        return -1;
-    target->method = method;
-#if CYTHON_COMPILING_IN_CPYTHON
-    #if PY_MAJOR_VERSION >= 3
-    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
+/* PyObjectCall2Args */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args, *result = NULL;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyFunction_FastCall(function, args, 2);
+    }
     #endif
-    {
-        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
-        target->func = descr->d_method->ml_meth;
-        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyCFunction_FastCall(function, args, 2);
+    }
+    #endif
+    args = PyTuple_New(2);
+    if (unlikely(!args)) goto done;
+    Py_INCREF(arg1);
+    PyTuple_SET_ITEM(args, 0, arg1);
+    Py_INCREF(arg2);
+    PyTuple_SET_ITEM(args, 1, arg2);
+    Py_INCREF(function);
+    result = __Pyx_PyObject_Call(function, args, NULL);
+    Py_DECREF(args);
+    Py_DECREF(function);
+done:
+    return result;
+}
+
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
 #endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
     return 0;
 }
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
 
-/* CallUnboundCMethod0 */
-static PyObject* __Pyx__CallUnboundCMethod0(__Pyx_CachedCFunction* cfunc, PyObject* self) {
-    PyObject *args, *result = NULL;
-    if (unlikely(!cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
-#if CYTHON_ASSUME_SAFE_MACROS
-    args = PyTuple_New(1);
-    if (unlikely(!args)) goto bad;
-    Py_INCREF(self);
-    PyTuple_SET_ITEM(args, 0, self);
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
 #else
-    args = PyTuple_Pack(1, self);
-    if (unlikely(!args)) goto bad;
+    if (likely(PyString_Check(n)))
 #endif
-    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-    Py_DECREF(args);
-bad:
-    return result;
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
+/* GetAttr3 */
+static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        return NULL;
+    __Pyx_PyErr_Clear();
+    Py_INCREF(d);
+    return d;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
+    PyObject *r = __Pyx_GetAttr(o, n);
+    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
 /* pyfrozenset_new */
 static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it) {
     if (it) {
         PyObject* result;
 #if CYTHON_COMPILING_IN_PYPY
@@ -7453,14 +10096,21 @@
     int result = PySet_Contains(set, key);
     if (unlikely(result < 0)) {
         result = __Pyx_PySet_ContainsUnhashable(set, key);
     }
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
+/* PyUnicode_Unicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj) {
+    if (unlikely(obj == Py_None))
+        obj = __pyx_kp_u_None;
+    return __Pyx_NewRef(obj);
+}
+
 /* JoinPyUnicode */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       CYTHON_UNUSED Py_UCS4 max_char) {
 #if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     PyObject *result_uval;
     int result_ukind;
     Py_ssize_t i, char_pos;
@@ -7664,14 +10314,27 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
@@ -7776,14 +10439,53 @@
     if (unlikely(!method)) goto bad;
     result = __Pyx_PyObject_CallNoArg(method);
     Py_DECREF(method);
 bad:
     return result;
 }
 
+/* UnpackUnboundCMethod */
+static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
+    PyObject *method;
+    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
+    if (unlikely(!method))
+        return -1;
+    target->method = method;
+#if CYTHON_COMPILING_IN_CPYTHON
+    #if PY_MAJOR_VERSION >= 3
+    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
+    #endif
+    {
+        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
+        target->func = descr->d_method->ml_meth;
+        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
+    }
+#endif
+    return 0;
+}
+
+/* CallUnboundCMethod0 */
+static PyObject* __Pyx__CallUnboundCMethod0(__Pyx_CachedCFunction* cfunc, PyObject* self) {
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_ASSUME_SAFE_MACROS
+    args = PyTuple_New(1);
+    if (unlikely(!args)) goto bad;
+    Py_INCREF(self);
+    PyTuple_SET_ITEM(args, 0, self);
+#else
+    args = PyTuple_Pack(1, self);
+    if (unlikely(!args)) goto bad;
+#endif
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    Py_DECREF(args);
+bad:
+    return result;
+}
+
 /* pop */
 static CYTHON_INLINE PyObject* __Pyx__PyObject_Pop(PyObject* L) {
     if (Py_TYPE(L) == &PySet_Type) {
         return PySet_Pop(L);
     }
     return __Pyx_PyObject_CallMethod0(L, __pyx_n_s_pop);
 }
@@ -7849,39 +10551,14 @@
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 }
 #endif
 
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
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
@@ -7984,27 +10661,14 @@
 }
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
         if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
@@ -8032,214 +10696,296 @@
             return -1;
         }
     }
     return 0;
 #endif
 }
 
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
     }
     return __Pyx_IterFinish();
 }
 
-/* PyIntCompare */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_NeObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
-    if (op1 == op2) {
-        Py_RETURN_FALSE;
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* UnpackTupleError */
+static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
+    if (t == Py_None) {
+      __Pyx_RaiseNoneNotIterableError();
+    } else if (PyTuple_GET_SIZE(t) < index) {
+      __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
+    } else {
+      __Pyx_RaiseTooManyValuesError(index);
     }
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-        if (a != b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+}
+
+/* UnpackTuple2 */
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
+    PyObject *value1 = NULL, *value2 = NULL;
+#if CYTHON_COMPILING_IN_PYPY
+    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
+    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
+#else
+    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
+    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
+#endif
+    if (decref_tuple) {
+        Py_DECREF(tuple);
     }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        int unequal;
-        unsigned long uintval;
-        Py_ssize_t size = Py_SIZE(op1);
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        if (intval == 0) {
-            if (size != 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-        } else if (intval < 0) {
-            if (size >= 0)
-                Py_RETURN_TRUE;
-            intval = -intval;
-            size = -size;
-        } else {
-            if (size <= 0)
-                Py_RETURN_TRUE;
-        }
-        uintval = (unsigned long) intval;
-#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 4)) {
-            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
+#if CYTHON_COMPILING_IN_PYPY
+bad:
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
 #endif
-#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 3)) {
-            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
+}
+static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
+                                       int has_known_size, int decref_tuple) {
+    Py_ssize_t index;
+    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
+    iternextfunc iternext;
+    iter = PyObject_GetIter(tuple);
+    if (unlikely(!iter)) goto bad;
+    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
+    iternext = Py_TYPE(iter)->tp_iternext;
+    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
+    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
+    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
+    Py_DECREF(iter);
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
+unpacking_failed:
+    if (!has_known_size && __Pyx_IterFinish() == 0)
+        __Pyx_RaiseNeedMoreValuesError(index);
+bad:
+    Py_XDECREF(iter);
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+}
+
+/* dict_iter */
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_source_is_dict) {
+    is_dict = is_dict || likely(PyDict_CheckExact(iterable));
+    *p_source_is_dict = is_dict;
+    if (is_dict) {
+#if !CYTHON_COMPILING_IN_PYPY
+        *p_orig_length = PyDict_Size(iterable);
+        Py_INCREF(iterable);
+        return iterable;
+#elif PY_MAJOR_VERSION >= 3
+        static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
+        PyObject **pp = NULL;
+        if (method_name) {
+            const char *name = PyUnicode_AsUTF8(method_name);
+            if (strcmp(name, "iteritems") == 0) pp = &py_items;
+            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
+            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
+            if (pp) {
+                if (!*pp) {
+                    *pp = PyUnicode_FromString(name + 4);
+                    if (!*pp)
+                        return NULL;
+                }
+                method_name = *pp;
+            }
+        }
 #endif
-#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 2)) {
-            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
+    }
+    *p_orig_length = 0;
+    if (method_name) {
+        PyObject* iter;
+        iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
+        if (!iterable)
+            return NULL;
+#if !CYTHON_COMPILING_IN_PYPY
+        if (PyTuple_CheckExact(iterable) || PyList_CheckExact(iterable))
+            return iterable;
 #endif
-#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 1)) {
-            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
+        iter = PyObject_GetIter(iterable);
+        Py_DECREF(iterable);
+        return iter;
+    }
+    return PyObject_GetIter(iterable);
+}
+static CYTHON_INLINE int __Pyx_dict_iter_next(
+        PyObject* iter_obj, CYTHON_NCP_UNUSED Py_ssize_t orig_length, CYTHON_NCP_UNUSED Py_ssize_t* ppos,
+        PyObject** pkey, PyObject** pvalue, PyObject** pitem, int source_is_dict) {
+    PyObject* next_item;
+#if !CYTHON_COMPILING_IN_PYPY
+    if (source_is_dict) {
+        PyObject *key, *value;
+        if (unlikely(orig_length != PyDict_Size(iter_obj))) {
+            PyErr_SetString(PyExc_RuntimeError, "dictionary changed size during iteration");
+            return -1;
+        }
+        if (unlikely(!PyDict_Next(iter_obj, ppos, &key, &value))) {
+            return 0;
+        }
+        if (pitem) {
+            PyObject* tuple = PyTuple_New(2);
+            if (unlikely(!tuple)) {
+                return -1;
+            }
+            Py_INCREF(key);
+            Py_INCREF(value);
+            PyTuple_SET_ITEM(tuple, 0, key);
+            PyTuple_SET_ITEM(tuple, 1, value);
+            *pitem = tuple;
+        } else {
+            if (pkey) {
+                Py_INCREF(key);
+                *pkey = key;
+            }
+            if (pvalue) {
+                Py_INCREF(value);
+                *pvalue = value;
+            }
+        }
+        return 1;
+    } else if (PyTuple_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyTuple_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyTuple_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else if (PyList_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyList_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyList_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else
 #endif
-            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
-        if (unequal != 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    {
+        next_item = PyIter_Next(iter_obj);
+        if (unlikely(!next_item)) {
+            return __Pyx_IterFinish();
+        }
     }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-        if ((double)a != (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    if (pitem) {
+        *pitem = next_item;
+    } else if (pkey && pvalue) {
+        if (__Pyx_unpack_tuple2(next_item, pkey, pvalue, source_is_dict, source_is_dict, 1))
+            return -1;
+    } else if (pkey) {
+        *pkey = next_item;
+    } else {
+        *pvalue = next_item;
     }
-    return (
-        PyObject_RichCompare(op1, op2, Py_NE));
+    return 1;
 }
 
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
+    PyObject *module = 0;
+    PyObject *global_dict = 0;
+    PyObject *empty_dict = 0;
+    PyObject *list;
     #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long x;
-        long a = PyInt_AS_LONG(op1);
-            x = (long)((unsigned long)a + b);
-            if (likely((x^a) >= 0 || (x^b) >= 0))
-                return PyInt_FromLong(x);
-            return PyLong_Type.tp_as_number->nb_add(op1, op2);
-    }
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (!py_import)
+        goto bad;
     #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
-#endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
-        } else {
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
+    if (from_list)
+        list = from_list;
+    else {
+        empty_list = PyList_New(0);
+        if (!empty_list)
+            goto bad;
+        list = empty_list;
+    }
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
+    empty_dict = PyDict_New();
+    if (!empty_dict)
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                module = PyImport_ImportModuleLevelObject(
+                    name, global_dict, empty_dict, list, 1);
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                        goto bad;
+                    PyErr_Clear();
+                }
             }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (!py_level)
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, global_dict, empty_dict, list, level);
+            #endif
         }
-                x = a + b;
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla + llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
     }
+bad:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
     #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-            double result;
-            PyFPE_START_PROTECT("add", return NULL)
-            result = ((double)a) + (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
+    return module;
+}
+
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
     }
-    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
+    return value;
 }
-#endif
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
@@ -8320,14 +11066,208 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* HasAttr */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (unlikely(!r)) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
+}
+
+/* PyObject_GenericGetAttrNoDict */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'%.50s' object has no attribute '%U'",
+                 tp->tp_name, attr_name);
+#else
+                 "'%.50s' object has no attribute '%.400s'",
+                 tp->tp_name, PyString_AS_STRING(attr_name));
+#endif
+    return NULL;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
+    PyObject *descr;
+    PyTypeObject *tp = Py_TYPE(obj);
+    if (unlikely(!PyString_Check(attr_name))) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    assert(!tp->tp_dictoffset);
+    descr = _PyType_Lookup(tp, attr_name);
+    if (unlikely(!descr)) {
+        return __Pyx_RaiseGenericGetAttributeError(tp, attr_name);
+    }
+    Py_INCREF(descr);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_HAVE_CLASS)))
+    #endif
+    {
+        descrgetfunc f = Py_TYPE(descr)->tp_descr_get;
+        if (unlikely(f)) {
+            PyObject *res = f(descr, obj, (PyObject *)tp);
+            Py_DECREF(descr);
+            return res;
+        }
+    }
+    return descr;
+}
+#endif
+
+/* PyObject_GenericGetAttr */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
+    if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
+}
+#endif
+
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
+/* SetupReduce */
+static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  int ret;
+  PyObject *name_attr;
+  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
+  if (likely(name_attr)) {
+      ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
+  } else {
+      ret = -1;
+  }
+  if (unlikely(ret < 0)) {
+      PyErr_Clear();
+      ret = 0;
+  }
+  Py_XDECREF(name_attr);
+  return ret;
+}
+static int __Pyx_setup_reduce(PyObject* type_obj) {
+    int ret = 0;
+    PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
+    PyObject *object_reduce_ex = NULL;
+    PyObject *reduce = NULL;
+    PyObject *reduce_ex = NULL;
+    PyObject *reduce_cython = NULL;
+    PyObject *setstate = NULL;
+    PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
+#if CYTHON_USE_PYTYPE_LOOKUP
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#else
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#endif
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    if (reduce_ex == object_reduce_ex) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#else
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#endif
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
+            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
+            if (likely(reduce_cython)) {
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+            } else if (reduce == object_reduce || PyErr_Occurred()) {
+                goto __PYX_BAD;
+            }
+            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
+            if (!setstate) PyErr_Clear();
+            if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
+                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
+                if (likely(setstate_cython)) {
+                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                } else if (!setstate || PyErr_Occurred()) {
+                    goto __PYX_BAD;
+                }
+            }
+            PyType_Modified((PyTypeObject*)type_obj);
+        }
+    }
+    goto __PYX_GOOD;
+__PYX_BAD:
+    if (!PyErr_Occurred())
+        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
+    ret = -1;
+__PYX_GOOD:
+#if !CYTHON_USE_PYTYPE_LOOKUP
+    Py_XDECREF(object_reduce);
+    Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
+#endif
+    Py_XDECREF(reduce);
+    Py_XDECREF(reduce_ex);
+    Py_XDECREF(reduce_cython);
+    Py_XDECREF(setstate);
+    Py_XDECREF(setstate_cython);
+    return ret;
+}
+
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
@@ -8349,93 +11289,14 @@
     if (likely(m && m->mp_subscript)) {
         return m->mp_subscript(obj, key);
     }
     return __Pyx_PyObject_GetIndex(obj, key);
 }
 #endif
 
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
-    PyObject *module = 0;
-    PyObject *global_dict = 0;
-    PyObject *empty_dict = 0;
-    PyObject *list;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
-        goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
-        empty_list = PyList_New(0);
-        if (!empty_list)
-            goto bad;
-        list = empty_list;
-    }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
-    empty_dict = PyDict_New();
-    if (!empty_dict)
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
-            #endif
-        }
-    }
-bad:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -9205,14 +12066,34 @@
         result = PyObject_Call(metaclass, margs, mkw);
         Py_DECREF(margs);
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
+/* GetNameInClass */
+static PyObject *__Pyx_GetGlobalNameAfterAttributeLookup(PyObject *name) {
+    PyObject *result;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        return NULL;
+    __Pyx_PyErr_Clear();
+    __Pyx_GetModuleGlobalNameUncached(result, name);
+    return result;
+}
+static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name) {
+    PyObject *result;
+    result = __Pyx_PyObject_GetAttrStr(nmspace, name);
+    if (!result) {
+        result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
+    }
+    return result;
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -9456,14 +12337,52 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -9652,52 +12571,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -9886,14 +12767,52 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
```

### Comparing `multimcts-0.3.1/multimcts/mcts.pyx` & `multimcts-0.4/multimcts/mcts.pyx`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+# distutils: language=c++
+# cython: language_level=3
+# cython: profile=False
+
 from time import time
 from random import shuffle, choice
-from collections import defaultdict
 from typing import Union, Dict, List, Any
 
-cimport cython
-
 from libc.math cimport log, sqrt, INFINITY
+from libcpp.map cimport map
+from libcpp.string cimport string
+from libcpp.pair cimport pair
+cimport cython
 
 
 Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
 Team = Union[int,str]
 Rewards = Dict[Team,float]
 
 
@@ -28,24 +33,24 @@
         """
         raise NotImplementedError("GameState must implement make_move.")
 
     def is_terminal(self) -> bool:
         """Checks if the game is over."""
         raise NotImplementedError("GameState must implement is_terminal.")
 
-    def get_reward(self) -> Union[float, Rewards]:
+    def get_reward(self) -> Union[float,Rewards]:
         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}
         Note: This method is only called on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
 
-class Node:
+cdef class Node:
     """Represents a game state node in the MCTS search tree.
 
     Args:
         state (GameState): The game state at the current node.
         parent (Node): The parent of the current node in the search tree.
         move (Move): The move that was played from the parent node to get to this node.
 
@@ -53,44 +58,80 @@
         children (list): The child nodes of the current node. These represent legal moves that have been visited.
         num_visits (int): The number of times the node has been visited.
         total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.
         is_terminal (bool): Whether the node represents a terminal state.
         is_fully_expanded (bool): Whether all children of the node have been visited.
         remaining_moves (list): A list of moves that have not yet been tried.
     """
+    cdef _state, _move
+    cdef string _team
+    cdef Node _parent
+    cdef _children, _remaining_moves
+    cdef map[string,float] _total_reward
+    cdef int _num_visits
+    cdef double log_visits
+    cdef bint _is_terminal
+    cdef bint _is_fully_expanded
+
     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
-        self.state = state
-        self.parent = parent
-        self.move = move
-
-        self.children:List['Node'] = []
-        self.num_visits:int = 0
-        self.total_reward = defaultdict(float)
+        self._state = state
+        self._parent = parent
+        self._move = move
+        self._team = str(self._state.get_current_team()).encode()
+
+        self._children:List['Node'] = []
+        self._num_visits = 0
+        self.log_visits = -INFINITY
+        self._total_reward = map[string,float]()
+
+        self._is_terminal = self._state.is_terminal()
+        if self._is_terminal:
+            self._is_fully_expanded = True
+            self._remaining_moves = []
+        else:
+            self._is_fully_expanded = False
+            self._remaining_moves = self._state.get_legal_moves()
+            shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
+
+    @property
+    def state(self) -> GameState: return self._state
+    @property
+    def parent(self) -> 'Node': return self._parent
+    @property
+    def move(self) -> Move: return self._move
+    @property
+    def children(self) -> List['Node']: return self._children
+    @property
+    def remaining_moves(self) -> List[Move]: return self._remaining_moves
 
-        self.is_terminal:bool = self.state.is_terminal()
-        self.is_fully_expanded:bool = self.is_terminal
+    @cython.cdivision(True)
+    @cython.boundscheck(False)
+    @cython.wraparound(False)
+    def visit(self):
+        self._num_visits += 1
+        self.log_visits = log(self._num_visits)
 
-        if self.is_fully_expanded:
-            self.remaining_moves = []
-        else:
-            self.remaining_moves = self.state.get_legal_moves()
-            shuffle(self.remaining_moves)
 
+cdef class MCTS:
+    cdef double exploration_bias
 
-class MCTS:
     def __init__(self, exploration_bias:float=1.414):
         """Initializes an MCTS agent.
 
         Args:
             exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.
                 It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).
-                Default is 1.414, which is sqrt(2) and often used in practice.
+                The default √2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
         """
         self.exploration_bias = exploration_bias
 
+    @property
+    def exploration_bias(self) -> float:
+        return self.exploration_bias
+
     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
         """Searches for this state's best move until some limit has been reached.
 
         Args:
             state (GameState): The game state for which to find the best move.
             max_time (int|float): The maximum time to search, in seconds.
             max_iterations (int): The maximum number of selections/simulations to perform.
@@ -105,52 +146,54 @@
             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
 
         if max_time is None and max_iterations is None:
             raise ValueError("One or more of max_time/max_iterations is required.")
 
         node = Node(state)
 
+        cdef double exploration_bias = self.exploration_bias
+
         cdef double end_time
         cdef int i
         if max_time is not None:
             end_time = time() + max_time
         if max_iterations is not None:
             i = max_iterations
 
         while True:
-            child = self.select(node)
+            child = self.select(node, exploration_bias)
             reward = self.simulate(child, heuristic=heuristic)
             self.backpropagate(child, reward)
 
             if max_time is not None and time() >= end_time:
                 break
             if max_iterations is not None:
                 i -= 1
                 if i <= 0:
                     break
 
-        best = self.get_best_child(node)
+        best = self.get_best_child(node, exploration_bias)
 
         if return_type == "state":
             return best.state
         elif return_type == "move":
             return best.move
         elif return_type == "node":
             return best
 
-    def select(self, node:Node) -> Node:
+    def select(self, node:Node, exploration_bias:float) -> Node:
         """Step 1: Selection
         Traverse the tree for the node we most want to simulate.
         Looks for an unexplored child of this node's best child's best child's...best child.
         """
-        while not node.is_terminal:
-            if not node.is_fully_expanded:
+        while not node._is_terminal:
+            if not node._is_fully_expanded:
                 return self.expand(node)
             else:
-                node = self.get_best_child(node)
+                node = self.get_best_child(node, exploration_bias)
 
         return node
 
     @staticmethod
     def expand(node:Node) -> Node:
         """Step 2: Expansion
         Add a new child to this node.
@@ -160,30 +203,30 @@
         except IndexError:
             raise IndexError("Tried to expand a node with no remaining moves.")
 
         child = Node(state=node.state.make_move(move), parent=node, move=move)
         node.children.append(child)
 
         if len(node.remaining_moves) == 0:
-            node.is_fully_expanded = True
+            node._is_fully_expanded = True
 
         return child
 
     def simulate(self, node:Node, *, heuristic=None) -> Rewards:
         """Step 3: Simulation (aka playout/rollout)
         Play out a game, from the given node to termination, and return the final reward.
         A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.
 
         Args:
             node (Node): The node from which to begin the simulation.
             heuristic (callable): A function that takes a state and returns a move.
         """
         state = node.state
 
-        if node.is_terminal:
+        if node._is_terminal:
             terminal_team = node.parent.state.get_current_team()
         else:
             while not state.is_terminal():
                 terminal_team = state.get_current_team()
                 if heuristic is not None:
                     move = heuristic(state)
                 else:
@@ -197,52 +240,67 @@
         return reward
 
     @staticmethod
     def backpropagate(node:Node, reward:Rewards):
         """Step 4: Backpropagation
         Update all ancestors with the reward from this terminal node.
         """
-        # Remove 0-values for efficiency.
-        reward = {k:v for k,v in reward.items() if v!=0}
+        cdef double val
+        cdef string ckey
+        cdef map[string,float] creward = map[string,float]()
+        for key,val in reward.items():
+            if val == 0:
+                continue
+            ckey = str(key).encode()
+            creward[ckey] = val
+
+        cdef pair[string,float] item
         while node is not None:
-            node.num_visits += 1
-            for key in reward:
-                node.total_reward[key] += reward[key]
+            for item in creward:
+                ckey = item.first
+                if node._total_reward.count(ckey) == 0:
+                    node._total_reward[ckey] = 0
+                node._total_reward[ckey] += item.second
+            node.visit()
             node = node.parent
 
     @cython.cdivision(True)
-    def get_best_child(self, node:Node) -> Node:
+    @cython.boundscheck(False)
+    @cython.wraparound(False)
+    def get_best_child(self, node:Node, exploration_bias:float) -> Node:
         """Find the child with the highest Upper Confidence Bound (UCB) score.
         ucb = (x / n) + C * sqrt(ln(N) / n)
         x=reward for this node
         n=number of simulations for this node
         N=number of simulations for parent node
         C=exploration bias
         """
         # Initialize UCB variables.
         cdef int visits
-        cdef double reward, subreward, ucb
-        cdef double exploration_bias = self.exploration_bias
-        cdef double ln_parent_visits = log(node.num_visits)
+        cdef double reward, ucb
+        cdef double C = exploration_bias
+        cdef double ln_parent_visits = node.log_visits
+
+        cdef string cur_team = node._team
 
-        cur_team = node.state.get_current_team()
+        cdef Node child, best_child
+        cdef pair[string,float] item
 
         cdef double best_score = -INFINITY
-        best_child:Node = None
 
         for child in node.children:
-            visits = child.num_visits
+            visits = child._num_visits
             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
                 continue
 
             # Relative reward is this child's reward minus its siblings' rewards.
-            reward = 2 * child.total_reward[cur_team]
-            for subreward in child.total_reward.values():
-                reward -= subreward
+            reward = 2 * child._total_reward[cur_team]
+            for item in child._total_reward:
+                reward -= item.second
 
-            ucb = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
+            ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
 
             if ucb > best_score:
                 best_score = ucb
                 best_child = child
 
         return best_child
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multimcts-0.3.1/multimcts.egg-info/PKG-INFO` & `multimcts-0.4/multimcts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.3.1
+Version: 0.4
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -40,21 +40,26 @@
 ```bash
 pip install multimcts
 ```
 
 
 ## Usage
 
-To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
+Then you can use MCTS to search for the best move. It will search until some limit is reached.
+```python
+state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
+```
+
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
```

### Comparing `multimcts-0.3.1/setup.py` & `multimcts-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
 setup(
     name='multimcts',
-    version='0.3.1',
+    version='0.4',
     description='Monte Carlo Tree Search for multiple teams',
     author='Taylor Vance',
     author_email='mirrors.cities0w@icloud.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/taylorvance/multimcts',
```

